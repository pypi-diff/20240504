# Comparing `tmp/diwork-1.0.0.tar.gz` & `tmp/diwork-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diwork-1.0.0.tar", last modified: Sat May  4 08:24:57 2024, max compression
+gzip compressed data, was "diwork-1.1.0.tar", last modified: Sat May  4 10:02:21 2024, max compression
```

## Comparing `diwork-1.0.0.tar` & `diwork-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 08:24:57.396665 diwork-1.0.0/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.0.0/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)       96 2024-05-04 08:24:57.396665 diwork-1.0.0/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      421 2023-02-18 08:28:20.000000 diwork-1.0.0/README.md
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 08:24:57.393665 diwork-1.0.0/diwork/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.0.0/diwork/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.0.0/diwork/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-04 07:57:25.000000 diwork-1.0.0/diwork/__version__.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 08:24:57.395665 diwork-1.0.0/diwork/diwork_mains/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      540 2023-03-17 21:42:04.000000 diwork-1.0.0/diwork/diwork_mains/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5734 2023-05-08 08:27:25.000000 diwork-1.0.0/diwork/diwork_mains/diwork_archive.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     4981 2023-03-23 06:34:14.000000 diwork-1.0.0/diwork/diwork_mains/diwork_clone.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     7521 2023-03-17 19:19:40.000000 diwork-1.0.0/diwork/diwork_mains/diwork_diff.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     3241 2023-02-18 08:20:12.000000 diwork-1.0.0/diwork/diwork_mains/diwork_difx.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9181 2023-04-11 08:18:44.000000 diwork-1.0.0/diwork/diwork_mains/diwork_exec.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5170 2023-03-23 06:31:31.000000 diwork-1.0.0/diwork/diwork_mains/diwork_hash.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.0.0/diwork/diwork_mains/diwork_help.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2900 2023-03-09 08:12:58.000000 diwork-1.0.0/diwork/diwork_mains/diwork_repeats.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     9064 2023-03-09 21:18:05.000000 diwork-1.0.0/diwork/diwork_mains/diwork_sshclone.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 08:24:57.395665 diwork-1.0.0/diwork/diwork_ways/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      555 2023-03-23 06:32:56.000000 diwork-1.0.0/diwork/diwork_ways/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      982 2023-02-17 14:44:34.000000 diwork-1.0.0/diwork/diwork_ways/diwork_parse.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    10603 2023-03-23 06:32:43.000000 diwork-1.0.0/diwork/diwork_ways/diwork_sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1293 2024-05-04 08:01:27.000000 diwork-1.0.0/diwork/main.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 08:24:57.396665 diwork-1.0.0/diwork.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)       96 2024-05-04 08:24:57.000000 diwork-1.0.0/diwork.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      755 2024-05-04 08:24:57.000000 diwork-1.0.0/diwork.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-04 08:24:57.000000 diwork-1.0.0/diwork.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-04 08:24:57.000000 diwork-1.0.0/diwork.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-05-04 08:24:57.000000 diwork-1.0.0/diwork.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-04 08:24:57.000000 diwork-1.0.0/diwork.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.0.0/pyproject.toml
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-04 08:24:57.396665 diwork-1.0.0/setup.cfg
--rw-r--r--   0 the220th  (1000) the220th  (1000)      981 2024-05-04 08:24:52.000000 diwork-1.0.0/setup.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.072634 diwork-1.1.0/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2023-02-10 11:11:21.000000 diwork-1.1.0/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 10:02:21.071634 diwork-1.1.0/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      211 2024-05-04 08:36:38.000000 diwork-1.1.0/README.md
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.069634 diwork-1.1.0/diwork/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      343 2024-05-04 08:22:40.000000 diwork-1.1.0/diwork/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      115 2024-05-04 08:01:22.000000 diwork-1.1.0/diwork/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       47 2024-05-04 08:33:46.000000 diwork-1.1.0/diwork/__version__.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.071634 diwork-1.1.0/diwork/diwork_mains/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      734 2024-05-04 08:48:21.000000 diwork-1.1.0/diwork/diwork_mains/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5734 2023-05-08 08:27:25.000000 diwork-1.1.0/diwork/diwork_mains/diwork_archive.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5032 2024-05-04 08:53:21.000000 diwork-1.1.0/diwork/diwork_mains/diwork_clone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     7521 2023-03-17 19:19:40.000000 diwork-1.1.0/diwork/diwork_mains/diwork_diff.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     4099 2024-05-04 10:01:13.000000 diwork-1.1.0/diwork/diwork_mains/diwork_diffclone.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     3241 2023-02-18 08:20:12.000000 diwork-1.1.0/diwork/diwork_mains/diwork_difx.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9181 2023-04-11 08:18:44.000000 diwork-1.1.0/diwork/diwork_mains/diwork_exec.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5170 2023-03-23 06:31:31.000000 diwork-1.1.0/diwork/diwork_mains/diwork_hash.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      582 2023-02-18 08:13:38.000000 diwork-1.1.0/diwork/diwork_mains/diwork_help.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2900 2023-03-09 08:12:58.000000 diwork-1.1.0/diwork/diwork_mains/diwork_repeats.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     9064 2023-03-09 21:18:05.000000 diwork-1.1.0/diwork/diwork_mains/diwork_sshclone.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.071634 diwork-1.1.0/diwork/diwork_ways/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      571 2024-05-04 09:30:24.000000 diwork-1.1.0/diwork/diwork_ways/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      982 2023-02-17 14:44:34.000000 diwork-1.1.0/diwork/diwork_ways/diwork_parse.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    10791 2024-05-04 09:52:54.000000 diwork-1.1.0/diwork/diwork_ways/diwork_sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1390 2024-05-04 09:37:47.000000 diwork-1.1.0/diwork/main.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-04 10:02:21.071634 diwork-1.1.0/diwork.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      116 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      795 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       44 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       14 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        7 2024-05-04 10:02:21.000000 diwork-1.1.0/diwork.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       81 2024-05-04 07:49:04.000000 diwork-1.1.0/pyproject.toml
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-04 10:02:21.072634 diwork-1.1.0/setup.cfg
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      997 2024-05-04 08:57:56.000000 diwork-1.1.0/setup.py
```

### Comparing `diwork-1.0.0/LICENSE` & `diwork-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_archive.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_archive.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_clone.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import sys
 import argparse 
 import shutil
 
 from diwork_ways import *
 
 def define_clone_command() -> "str":
-    if sys.platform == "linux" or platform == "linux2" or sys.platform == "darwin":
+    if sys.platform == "linux" or sys.platform == "linux2" or sys.platform == "darwin":
         return "cp"
-    elif sys.platform == "win32": # In windows cp == copy
+    elif sys.platform == "win32":  # In windows cp == copy
         return "copy"
     else:
         pout("(define_clone_command) Failed successfully. ")
 
 def cp(src: str, dest: str, copy_mode: int = 0) -> None:
     if(copy_mode == 0):
         shutil.copy(src, dest)
@@ -52,18 +52,18 @@
         exit()
     if(is_folder(folder2_abs) == False):
         pout(f"\"{folder2_abs}\" is not folder. ")
         exit()
     
     if(folder1_abs in folder2_abs):
         pout(f"Directory \"{folder1_abs}\" contains directory \"{folder2_abs}\". Exiting...")
-        exit()
+        input("Enter to continue...")
     if(folder2_abs in folder1_abs):
         pout(f"Directory \"{folder2_abs}\" contains directory \"{folder1_abs}\". Exiting...")
-        exit()
+        input("Enter to continue...")
     symlink_mode = args.symlink_mode
     copy_mode = args.copy_mode
     
     delete_all_if_dir_not_empty(folder2_abs)
     pout("Clonning...")
 
     dirs_abs_1 = getDirsList(folder1_abs)
```

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_diff.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_diff.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_difx.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_difx.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_exec.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_exec.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_hash.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_hash.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_help.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_help.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_repeats.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_repeats.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_mains/diwork_sshclone.py` & `diwork-1.1.0/diwork/diwork_mains/diwork_sshclone.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_ways/__init__.py` & `diwork-1.1.0/diwork/diwork_ways/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 
 from .diwork_sup import *
 
 from .diwork_parse import common_init_parser, common_init_parse
 
 __all__ = [
     "Global", "getFilesList", "getDirsList", "is_folder", "is_file", "is_exists", "is_folder_empty", "rel_path", "rm_folder_content", 
-    "check_files_exists_or_exit", "pout", "write2File_str", "mkdir", "get_link_unwinding", "get_nice_size", "get_time_str", 
+    "check_files_exists_or_exit", "pout", "write2File_str", "mkdir", "get_link_unwinding", "get_nice_size", "get_time_str", "get_time_file",
     "get_hash_file", "get_hash_str", "get_hash_of_hashes", 
     "exclude_files", "delete_all_if_dir_not_empty", "exe",
     "common_init_parser", "common_init_parse"
 ]
```

### Comparing `diwork-1.0.0/diwork/diwork_ways/diwork_parse.py` & `diwork-1.1.0/diwork/diwork_ways/diwork_parse.py`

 * *Files identical despite different names*

### Comparing `diwork-1.0.0/diwork/diwork_ways/diwork_sup.py` & `diwork-1.1.0/diwork/diwork_ways/diwork_sup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     
 
 
 def getFilesList(dirPath: str) -> list:
     return [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in files]
 
 def getDirsList(dirPath: str) -> list:
-    return [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in subdirs]
+    dirs = [os.path.join(path, name) for path, subdirs, files in os.walk(dirPath) for name in subdirs]
+    return list(set(dirs))
 
 # return False, if folder_path not exists or folder_path is not folder
 def is_folder(folder_path: str) -> bool:
     return os.path.isdir(folder_path)
 
 # return False, if file_path not exists or file_path is not file
 def is_file(file_path: str) -> bool:
@@ -108,14 +109,18 @@
         return f"{size_bytes // (1024*1024*1024*1024)} TB"
 
 def get_time_str() -> str:
     # time_str = datetime.datetime.now().strftime("[%y.%m.%d %H:%M:%S.%f]")
     time_str = datetime.datetime.now().strftime("%y.%m.%d %H:%M:%S")
     return time_str
 
+def get_time_file(file_path: str) -> str:
+    dt_m = datetime.datetime.fromtimestamp(os.path.getmtime(file_path))
+    return dt_m.strftime("%d.%m.%Y_%H-%M-%S")
+
 def get_hash_file(file_path: str) -> str:
     if(Global.hash_mode == 1):
         buff_BLOCKSIZE = 65536 # 64 kB
         sha = hashlib.sha256()
         with open(file_path, "rb") as temp:
             file_buffer = temp.read(buff_BLOCKSIZE)
             while len(file_buffer) > 0:
```

### Comparing `diwork-1.0.0/diwork/main.py` & `diwork-1.1.0/diwork/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 from diwork_mains import *
 
 from . import __version__
 
 VERSION = __version__
 
 def main():
-    MODULES = "{help, hash, clone, sshclone, diff, difx, repeats, exec, archive}"
+    MODULES = "{help, hash, clone, diffclone, sshclone, diff, difx, repeats, exec, archive}"
     SyntaxError_str = f"Syntax error. Expected: \"> python folder_work.py {MODULES} ...\""
     argc = len(sys.argv)
     Global.version = VERSION
     if(argc < 2):
         pout(SyntaxError_str)
         exit()
     else:
         sub_modul_name = sys.argv[1]
         if(sub_modul_name == "hash"):
             main_hash(sys.argv[2:])
         elif(sub_modul_name == "clone"):
             main_clone(sys.argv[2:])
+        elif(sub_modul_name == "diffclone"):
+            main_diffclone(sys.argv[2:])
         elif(sub_modul_name == "sshclone"):
             main_sshclone(sys.argv[2:])
         elif(sub_modul_name == "diff"):
             main_diff(sys.argv[2:])
         elif(sub_modul_name == "repeats"):
             main_repeats(sys.argv[2:])
         elif(sub_modul_name == "difx"):
```

### Comparing `diwork-1.0.0/diwork.egg-info/SOURCES.txt` & `diwork-1.1.0/diwork.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 diwork.egg-info/entry_points.txt
 diwork.egg-info/requires.txt
 diwork.egg-info/top_level.txt
 diwork/diwork_mains/__init__.py
 diwork/diwork_mains/diwork_archive.py
 diwork/diwork_mains/diwork_clone.py
 diwork/diwork_mains/diwork_diff.py
+diwork/diwork_mains/diwork_diffclone.py
 diwork/diwork_mains/diwork_difx.py
 diwork/diwork_mains/diwork_exec.py
 diwork/diwork_mains/diwork_hash.py
 diwork/diwork_mains/diwork_help.py
 diwork/diwork_mains/diwork_repeats.py
 diwork/diwork_mains/diwork_sshclone.py
 diwork/diwork_ways/__init__.py
```

### Comparing `diwork-1.0.0/setup.py` & `diwork-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     exec(ver_file.read(), main_ns)
 
 setup(
     name="diwork",
     version=main_ns["__version__"],
     install_requires=[
         "argparse",
+        "tqdm",
     ],
     packages=find_packages(
         # All keyword arguments below are optional:
         where='.',  # '.' by default or "src"
     ),
     entry_points={
         "console_scripts": [
```

