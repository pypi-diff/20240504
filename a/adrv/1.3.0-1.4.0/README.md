# Comparing `tmp/adrv-1.3.0.tar.gz` & `tmp/adrv-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adrv-1.3.0.tar", max compression
+gzip compressed data, was "adrv-1.4.0.tar", max compression
```

## Comparing `adrv-1.3.0.tar` & `adrv-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    14592 2024-04-11 17:21:31.670184 adrv-1.3.0/adrv/__init__.py
--rw-r--r--   0        0        0     1466 2024-03-19 20:59:47.629936 adrv-1.3.0/adrv/_cls.py
--rw-r--r--   0        0        0     1259 2024-03-19 20:22:55.614192 adrv-1.3.0/adrv/bridge.py
--rw-r--r--   0        0        0     1043 2024-03-02 13:18:04.598600 adrv-1.3.0/adrv/utils.py
--rw-r--r--   0        0        0    35802 2024-02-09 22:09:16.946792 adrv-1.3.0/LICENSE
--rw-r--r--   0        0        0      319 2024-04-11 17:20:52.274932 adrv-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6848 2024-03-19 20:59:42.125789 adrv-1.3.0/README.md
--rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 adrv-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    14758 2024-05-03 22:38:07.431535 adrv-1.4.0/adrv/__init__.py
+-rw-r--r--   0        0        0     1261 2024-05-03 22:20:49.774008 adrv-1.4.0/adrv/bridge.py
+-rw-r--r--   0        0        0      544 2024-05-03 22:32:50.296238 adrv-1.4.0/adrv/exceptions.py
+-rw-r--r--   0        0        0      916 2024-05-03 22:32:30.940547 adrv-1.4.0/adrv/models.py
+-rw-r--r--   0        0        0     1043 2024-03-02 13:18:04.598600 adrv-1.4.0/adrv/utils.py
+-rw-r--r--   0        0        0    35802 2024-02-09 22:09:16.946792 adrv-1.4.0/LICENSE
+-rw-r--r--   0        0        0      319 2024-05-03 22:23:09.609505 adrv-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6848 2024-03-19 20:59:42.125789 adrv-1.4.0/README.md
+-rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 adrv-1.4.0/PKG-INFO
```

### Comparing `adrv-1.3.0/adrv/__init__.py` & `adrv-1.4.0/adrv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 import os
 import shutil
 import tempfile
 import time
 import uuid
 import zipfile
 
-from ._cls import *
+from .exceptions import *
+from .models import *
 from .utils import *
 
-VERSION = "1.3.0"
-SUPPORTS = "1.3.0"
+VERSION = "1.4.0"
+SUPPORTS = "1.4.0"
 
 class Disk:
     def __init__(self, name: str = 'vDisk', path: str = './', max_size: int = 1000 ** 2):
         """
         Initializes a Disk instance.
 
         Args:
             name (str, optional): The name of the disk. Defaults to 'vDisk'.
             path (str, optional): The path where the disk will be stored. Defaults to './'.
             max_size (int, optional): The maximum size of the disk in bytes. Defaults to 1000000.
         """
+
         self.name = name.upper()
         self.path = os.path.normpath(os.path.join(path, f"{name}.adrv")).replace('\\', '/')
         self.max_size = Size(max_size)
         self.size = Size(0)
 
         if not zipfile.is_zipfile(self.path):
             if not os.path.exists(path):
@@ -40,25 +42,26 @@
             self.format_disk()
         
         properties = self.__sys_data('Disk/$Properties')
         self.name = properties[0]
         self.max_size = Size(int(properties[1]))
         self.size = Size(os.path.getsize(self.path))
 
-    def __read(self, _path: str) -> str:
+    def __read(self, _path: str) -> bytes:
         """
         Reads content from a file in the disk.
 
         Args:
             _path (str): The path of the file to be read.
             encoding (str | None, optional): The encoding of the file. Defaults to 'UTF-8'.
 
         Returns:
             str: The content of the file.
         """
+
         with open(self.path, 'rb') as _file:
             archive = io.BytesIO(_file.read())
 
             with zipfile.ZipFile(archive, 'r') as zip_buffer:
                 with tempfile.TemporaryDirectory() as tempDir:
                     zip_buffer.extractall(tempDir)
                     vPath = os.path.normpath(_path)
@@ -67,29 +70,30 @@
                     if os.path.exists(tempPath):
                         if os.path.isdir(tempPath):
                             raise FileIsDirectoryError(f"{vPath} is a directory.")
                         else:
                             with open(tempPath, 'rb') as extracted_file:
                                 content = extracted_file.read()
                                 
-                            return content
+                            return content.replace(b'\x0d', b'')
                     else:
                         raise FileNotFoundError(f"{vPath} was not found.")
                     
-    def __write(self, content: str | bytes, _path: str) -> int:
+    def __write(self, content: bytes, _path: str) -> int:
         """
         Writes content to a file in the disk.
 
         Args:
             content (str | bytes): The content to be written.
             _path (str): The path where the content will be written.
 
         Returns:
             int: The size of the content written.
         """
+
         if self.size.raw + len(content) > self.max_size.raw:
             raise FullDiskError(f'Could not write anything at {_path} as its content would overload the disk. Available space: {Size(self.max_size.raw - self.size.raw).literal()} / File size: {len(content)}')
         
         with zipfile.ZipFile(self.path, 'a') as archive:
             with tempfile.TemporaryDirectory() as tempDir:
                 filePath = os.path.normpath(f"{tempDir}/cachedfile")
                 with open(filePath, 'w' if isinstance(content, str) else 'wb') as _file:
@@ -106,14 +110,15 @@
 
         Args:
             _path (str): The path of the file to be deleted.
 
         Returns:
             int: The size of the deleted file.
         """
+
         try:
             _file = self.__read(_path)
             self.size.raw -= len(_file)
         except FileNotFoundError:
             return 0
         
         with tempfile.TemporaryDirectory() as tempDir, tempfile.TemporaryDirectory() as tempCache, zipfile.ZipFile(self.path, 'r') as old_archive:
@@ -140,33 +145,35 @@
             _name (str): The name of the system data.
             _data (str, optional): The data to be written. Defaults to ''.
             _mode (str, optional): The mode of operation ('r', 'w', 'a'). Defaults to 'r'.
 
         Returns:
             list[str] | None: The system data.
         """
+
         _path = os.path.join('/.sys/', _name)
         if _mode == 'r':
-            return self.__read(_path).decode('UTF-8').replace('\r', '').split('\n')
+            return self.__read(_path).decode('UTF-8').split('\n')
         elif _mode == 'w':
-            self.__write(_data, _path)
+            self.__write(_data.encode(), _path)
         elif _mode == 'a':
             data = self.__read(_path).decode('UTF-8')
             if data != '':
-                _data = '\n'.join((data, _data))
+                _data = '\n'.encode().join((data.encode(), _data.encode()))
             
-            self.__write(_data, _path)
+            self.__write(_data.encode(), _path)
 
     def __ls(self) -> list[str]:
         """
         Lists files in the disk.
 
         Returns:
             list[str]: The list of files in the disk.
         """
+
         with zipfile.ZipFile(self.path, 'r') as zip_buffer:
             return list(set(zip_buffer.namelist()))
     
     def format_disk(self, modelPath: str | None = None):
         """
         Formats the disk.
         """
@@ -191,15 +198,15 @@
                     
                     for name in namelist:
                         content = archive.read(name['path'])
                         self.write(name['vPath'], content, 'w')
             else:
                 raise BrokenDiskError(f"{modelPath} is broken.")
         
-        if not self.diagnosis(snooze = True):
+        if not self.diagnosis(snooze = True).result():
             self.extract_all('./.local')
             raise BrokenDiskError("Something went wrong while formatting your disk. It has automatically been extracted in .local")    
 
     def extract_all(self, target: str) -> None:
         """
         Extracts all files from the disk to a target directory.
 
@@ -219,15 +226,15 @@
                 os.makedirs(os.path.dirname(os.path.join(target, _file[0])))
             except FileExistsError:
                 pass
 
             with open(os.path.normpath(os.path.join(target, _file[0])), 'wb') as buffer:
                 buffer.write(self.__read(file))
     
-    def f_list(self, include_ts: bool = False, sys = False) -> list[str | dict]:
+    def f_list(self, include_ts: bool = False, sys: bool = False) -> list[str | dict]:
         """
         Lists files in the disk.
 
         Args:
             include_ts (bool, optional): Whether to include timestamps. Defaults to False.
 
         Returns:
@@ -260,15 +267,15 @@
         """
         Evaluates the health of the disk.
 
         Args:
             snooze (bool, optional): Whether to suppress output. Defaults to False.
 
         Returns:
-            bool: True if the disk is healthy, False otherwise.
+            DiagnoseResponse
         """
 
         if not snooze:
             print("Evaluating health of your disk...")
 
         status = {}
 
@@ -294,36 +301,40 @@
             else:
                 status["PrimaryFiles"] = "\033[32;40mPresent\033[0m"
         except:
             status["PrimaryFiles"] = "\033[31;40mMissing\033[0m"
 
         if not snooze:
             for section, result in status.items():
-                print(section, ": ", result, sep="")
+                print(section, ": ", result, sep = "")
 
         response = DiagnoseResponse()
         response.disk_format = 'Incorrect' not in status['DataFormat']
         response.is_supported = 'Un' not in status['DiskVersion']  # UN-known and UN-supported return False
         response.primary_files = 'Present' in status['PrimaryFiles']
 
         return response
 
 
-    def write(self, vPath: str, content: str | bytes = '', mode: str = 'a') -> int:
+    def write(self, vPath: str, content: str | bytes = b'', mode: str = 'a') -> int:
         """
         Writes content to a file in the disk.
 
         Args:
             vPath (str): The path where the content will be written.
             content (str | bytes, optional): The content to be written. Defaults to ''.
             mode (str, optional): The writing mode ('a', 'w'). Defaults to 'a'.
 
         Returns:
             int: The size of the content written.
         """
+
+        if type(content) == str:
+            content = content.encode()
+
         if mode == 'w':
             _file = { 'path': vPath, 'address': str(uuid.uuid4()), 'timestamp': round(time.time()) }
             self.__delete(_file['address'])
             self.__write(content, _file['address'])
             self.__sys_data('Disk/$Registry', '::'.join(map(str, _file.values())), _mode = 'a')
         elif mode == 'a':
             registry = self.__sys_data('Disk/$Registry')
@@ -331,16 +342,16 @@
                 _file = [ _item for _item in registry if _item.split('::')[0] == vPath ][0].split('::')
             except IndexError:
                 self.write(vPath, content, mode = 'w')
                 return
 
             _file = dict(zip([ 'path', 'address', 'timestamp' ], _file))
 
-            data = self.__read(_file['address'])
-            _data = '\n'.join((str(data), str(content)))
+            data = self.__read(_file['address']).decode()
+            _data = '\n'.encode().join((data.encode(), content))
 
             self.__delete(_file['address'])
             self.__write(_data, _file['address'])
 
         return len(content)
 
     def read(self, vPath: str) -> FileResponse:
@@ -349,14 +360,15 @@
 
         Args:
             vPath (str): The path of the file to be read.
 
         Returns:
             FileResponse: The response containing the file data.
         """
+
         registry = reversed(self.__sys_data('Disk/$Registry'))
         try:
             _file = [ _item for _item in registry if _item.split('::')[0] == vPath ][0].split('::')
         except IndexError:
             raise FileNotFoundError(f"'{vPath}' doesn't exist.")
         
         data = self.__read(f'/{_file[1]}')
```

### Comparing `adrv-1.3.0/adrv/bridge.py` & `adrv-1.4.0/adrv/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from . import Disk
-from ._cls import *
+from .models import *
 
 class PhysicalBridge:
     def __init__(self, disk: Disk):
         self.disk = disk
 
     def bring(self, vPath: str, newPath: str):
         try:
```

### Comparing `adrv-1.3.0/adrv/utils.py` & `adrv-1.4.0/adrv/utils.py`

 * *Files identical despite different names*

### Comparing `adrv-1.3.0/LICENSE` & `adrv-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adrv-1.3.0/README.md` & `adrv-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `adrv-1.3.0/PKG-INFO` & `adrv-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adrv
-Version: 1.3.0
+Version: 1.4.0
 Summary: 
 License: GPL-3.0
 Author: happex
 Author-email: 110610727+okayhappex@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

