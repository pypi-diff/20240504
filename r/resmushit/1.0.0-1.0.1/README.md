# Comparing `tmp/resmushit-1.0.0.tar.gz` & `tmp/resmushit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resmushit-1.0.0.tar", last modified: Sat Apr 13 20:40:16 2024, max compression
+gzip compressed data, was "resmushit-1.0.1.tar", last modified: Sat May  4 13:25:59 2024, max compression
```

## Comparing `resmushit-1.0.0.tar` & `resmushit-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:40:16.750932 resmushit-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 20:40:11.000000 resmushit-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 20:40:11.000000 resmushit-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-13 20:40:16.746932 resmushit-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-13 20:40:11.000000 resmushit-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-13 20:40:11.000000 resmushit-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:40:16.746932 resmushit-1.0.0/resmushit/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-13 20:40:11.000000 resmushit-1.0.0/resmushit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 20:40:11.000000 resmushit-1.0.0/resmushit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-13 20:40:11.000000 resmushit-1.0.0/resmushit/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-13 20:40:11.000000 resmushit-1.0.0/resmushit/resmushit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-13 20:40:11.000000 resmushit-1.0.0/resmushit/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 20:40:16.746932 resmushit-1.0.0/resmushit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-13 20:40:16.000000 resmushit-1.0.0/resmushit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-13 20:40:16.000000 resmushit-1.0.0/resmushit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 20:40:16.000000 resmushit-1.0.0/resmushit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 20:40:16.000000 resmushit-1.0.0/resmushit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 20:40:16.000000 resmushit-1.0.0/resmushit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 20:40:16.750932 resmushit-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-13 20:40:11.000000 resmushit-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:25:59.474547 resmushit-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-04 13:25:55.000000 resmushit-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 13:25:55.000000 resmushit-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-04 13:25:59.474547 resmushit-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-04 13:25:55.000000 resmushit-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 13:25:55.000000 resmushit-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:25:59.474547 resmushit-1.0.1/resmushit/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-04 13:25:55.000000 resmushit-1.0.1/resmushit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-04 13:25:55.000000 resmushit-1.0.1/resmushit/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 13:25:55.000000 resmushit-1.0.1/resmushit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 13:25:55.000000 resmushit-1.0.1/resmushit/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-04 13:25:55.000000 resmushit-1.0.1/resmushit/resmushit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-04 13:25:55.000000 resmushit-1.0.1/resmushit/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:25:59.474547 resmushit-1.0.1/resmushit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-04 13:25:59.000000 resmushit-1.0.1/resmushit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 13:25:59.000000 resmushit-1.0.1/resmushit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 13:25:59.000000 resmushit-1.0.1/resmushit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 13:25:59.000000 resmushit-1.0.1/resmushit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 13:25:59.000000 resmushit-1.0.1/resmushit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 13:25:59.474547 resmushit-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-04 13:25:55.000000 resmushit-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:25:59.474547 resmushit-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-04 13:25:55.000000 resmushit-1.0.1/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-04 13:25:55.000000 resmushit-1.0.1/tests/test_filesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 13:25:55.000000 resmushit-1.0.1/tests/test_from_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 13:25:55.000000 resmushit-1.0.1/tests/test_from_url.py
```

### Comparing `resmushit-1.0.0/LICENSE` & `resmushit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resmushit-1.0.0/PKG-INFO` & `resmushit-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: resmushit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper for resmush.it API
 Home-page: https://resmush.it/
+Download-URL: https://github.com/hemansah/resmushit
 Author: Hemant Sah
 Author-email: hemantsah18@gmail.com
 Maintainer: Hemant Sah
 License: MIT
 Project-URL: Homepage, https://resmush.it/
 Project-URL: Documentation, https://github.com/hemansah/resmushit/blob/master/README.md
 Project-URL: Repository, https://github.com/hemansah/resmushit/
@@ -23,35 +24,34 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6,<=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3
-Requires-Dist: colorama
+Requires-Dist: filetype
 
 # reSmush.it Image Optimizer Python package
 
-  
+[![Downloads](https://static.pepy.tech/badge/resmushit)](https://pepy.tech/project/resmushit)
+![Tests](https://github.com/hemansah/resmushit/actions/workflows/tests.yaml/badge.svg?branch=master)  
 
 ## Project Description
 
 Python3 wrapper for resmush.it API to optimize image file size.
 
-  
+    
 
 [resmush.it](https://resmush.it/) Image Optimizer allows you to use free Image optimization based on reSmush.it API.
 
 reSmush.it provides image size reduction based on several algorithms. The API accept JPG, PNG and GIF files up to 5MB.
 
-  
 
-## Installation
 
-  
+## Installation
 
 1. Install using pip3:
 
   
 
     `$ pip3 install resmushit`
```

### Comparing `resmushit-1.0.0/README.md` & `resmushit-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # reSmush.it Image Optimizer Python package
 
-  
+[![Downloads](https://static.pepy.tech/badge/resmushit)](https://pepy.tech/project/resmushit)
+![Tests](https://github.com/hemansah/resmushit/actions/workflows/tests.yaml/badge.svg?branch=master)  
 
 ## Project Description
 
 Python3 wrapper for resmush.it API to optimize image file size.
 
-  
+    
 
 [resmush.it](https://resmush.it/) Image Optimizer allows you to use free Image optimization based on reSmush.it API.
 
 reSmush.it provides image size reduction based on several algorithms. The API accept JPG, PNG and GIF files up to 5MB.
 
-  
 
-## Installation
 
-  
+## Installation
 
 1. Install using pip3:
 
   
 
     `$ pip3 install resmushit`
```

### Comparing `resmushit-1.0.0/resmushit/__init__.py` & `resmushit-1.0.1/resmushit/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from .resmushit import Resmushit
-from .exceptions import ImageURLNotFoundException, ImagePathNotFoundException
+from typing import Union
 
-def from_url(image_url=None, quality=92, output_dir=".", preserve_exif=False, preserve_filename=False, quiet_mode=False, notime=True, save=True):
-    if image_url:
-        resmushit = Resmushit(image_url=image_url, image_path=None, quality=quality, output_dir=output_dir, preserve_exif=preserve_exif, preserve_filename=preserve_filename, quiet_mode=quiet_mode)
-        return resmushit.optimize(save)
-    raise ImageURLNotFoundException("Please provide an image url")
+def from_url(image_url=None, _type="url", quality=92, output_dir=".", preserve_exif=False, preserve_filename=False, quiet_mode=False, save=True) -> Union[None, bytes]:
+    resmushit = Resmushit(image_url=image_url, _type=_type, image_path=None, quality=quality, output_dir=output_dir, preserve_exif=preserve_exif, preserve_filename=preserve_filename, quiet_mode=quiet_mode)
+    return resmushit.optimize(save=save)
 
-def from_path(image_path=None, quality=92, output_dir=".", preserve_exif=False, preserve_filename=False, quiet_mode=False, notime=True, save=True):
-    if image_path:
-        resmushit = Resmushit(image_path=image_path, image_url=None, quality=quality, output_dir=output_dir, preserve_exif=preserve_exif, preserve_filename=preserve_filename, quiet_mode=quiet_mode)
-        return resmushit.optimize(save)
-    raise ImagePathNotFoundException("Please provide an image path")
+
+def from_path(image_path=None, _type="file", quality=92, output_dir=".", preserve_exif=False, preserve_filename=False, quiet_mode=False, save=True) -> Union[None, bytes]:
+    resmushit = Resmushit(image_path=image_path, _type=_type, image_url=None, quality=quality, output_dir=output_dir, preserve_exif=preserve_exif, preserve_filename=preserve_filename, quiet_mode=quiet_mode)
+    return resmushit.optimize(save=save)
```

### Comparing `resmushit-1.0.0/resmushit/resmushit.py` & `resmushit-1.0.1/resmushit/resmushit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from urllib3 import PoolManager
 from .log import Log
 from .validator import Validator
-
+from typing import Union
 
 class Resmushit:
     """
     Wrapper for Resmush.it API
 
     Args:
         image_url (str): The url of image.
@@ -27,19 +27,21 @@
         `resmushit.from_path(image_path='image.png', quality=95)`
 
         `buffer = resmushit.from_url(image_url="https://ps.w.org/resmushit-image-optimizer/assets/icon-128x128.png", quality=95, save=False)`
 
     """
 
     __MAX_FILESIZE = 5 * 1024 * 1024
+    __API_URL: str = "http://api.resmush.it"
 
     def __init__(
         self,
         image_url: str = None,
         image_path: str = None,
+        _type: str = None,
         quality: int = 92,
         output_dir: str = ".",
         preserve_exif: bool = False,
         preserve_filename: bool = False,
         quiet_mode: bool = False,
     ) -> None:
         if image_path is not None and image_url is not None:
@@ -47,76 +49,78 @@
         elif image_url is not None:
             self.image_url = image_url
             self.image_path = None
         elif image_path is not None:
             self.image_path = image_path
             self.image_url = None
         else:
-            raise ValueError("image_path or image_url is required")
-
+            raise ValueError("image_path or image_url param is required")
+        self._type = _type
         self.quality = quality
         self.output_dir = output_dir
         self.preserve_exif = preserve_exif
         self.preserve_filename = preserve_filename
         self.quiet_mode = quiet_mode
-        self.__API_URL: str = "http://api.resmush.it"
         self._response = None
         self.__logger = Log(quiet_mode=quiet_mode)
 
-    def __call_api(self):
+    @classmethod
+    def _filesize_limit(cls):
+        return cls.__MAX_FILESIZE
+
+    def __call_api(self) -> None:
         try:
             self.__logger.log(
-                message=f"Initializing image optimization with quality factor: {self.quality}%",
-                color="blue",
+                message=f"Initializing image optimization with quality factor: {self.quality}%"
+            )
+            self.__logger.log(
+                message=f"Sending picture {self.filename}.{self.extension} to api..."
             )
-            self.__logger.log(message=f"Sending picture {self.filename} to api...")
-
             http = PoolManager()
             r = http.request(
                 "POST",
-                self.__API_URL + f"/?qlty={self.quality}&exif={self.preserve_exif}",
-                fields={"files": ("image.png", self.imagebytes)},
+                Resmushit.__API_URL
+                + f"/?qlty={self.quality}&exif={self.preserve_exif}",
+                fields={"files": (f"{self.filename}.{self.extension}", self.imagebytes)},
             )
             self._response = json.loads(r.data.decode("utf-8"))
             self.__logger.log(
-                message=f"File optimized by {self._response.get('percent',0)}% (from {self._response.get('src_size',0)//1024}KB to {self._response.get('dest_size',0)//1024}KB). Retrieving...",
-                color="green",
+                message=f"File optimized by {self._response.get('percent',0)}% (from {self._response.get('src_size',0)//1024}KB to {self._response.get('dest_size',0)//1024}KB). Retrieving..."
             )
         except Exception as e:
             raise Exception(f"Error Occurred: {str(e)}")
 
-    def __get_dest_url(self):
+    def __get_dest_url(self) -> str:
         return self._response.get("dest")
 
-    def __download_image(self, dest_url):
+    def __download_image(self, dest_url) -> bytes:
         try:
             http = PoolManager()
             r = http.request("GET", dest_url)
             return r.data
         except Exception as e:
             raise Exception(f"{e}")
 
-    def __save_image(self, imagebytes):
+    def __save_image(self, imagebytes) -> bytes:
         with open(
             os.path.join(
                 self.output_dir,
                 f"{'' if self.preserve_filename else 'optimized-'}{self.filename}"
-                + f"{self.extension}",
+                +"."+ f"{self.extension}",
             ),
             "wb",
         ) as f:
             f.write(imagebytes)
 
-    def optimize(self, save: bool = True):
-        self.path, self.type, self.imagebytes, self.filename, self.extension = (
-            Validator(
-                path=self.image_url or self.image_path,
-                max_file_size=Resmushit.__MAX_FILESIZE,
-            ).validate()
-        )
+    def optimize(self, save: bool = True) -> Union[None, bytes]:
+        self.imagebytes, self.filename, self.extension = Validator(
+            path=self.image_url or self.image_path,
+            max_file_size=Resmushit.__MAX_FILESIZE,
+            _type=self._type,
+        ).validate()
         self.__logger.log(f"Processing: {self.filename}")
         self.__call_api()
 
         dest_url = self.__get_dest_url()
         optimized_imagebytes = self.__download_image(dest_url=dest_url)
         if save:
             self.__save_image(imagebytes=optimized_imagebytes)
```

### Comparing `resmushit-1.0.0/resmushit/validator.py` & `resmushit-1.0.1/resmushit/validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,102 +1,92 @@
 import os
-from io import BytesIO
 from urllib.parse import urlparse
 from urllib3 import PoolManager
-import imghdr
-from .exceptions import FileTooLargeError, InvalidImageExtensionError
+from .exceptions import (FileTooLargeError, 
+                         InvalidImageExtensionError, 
+                         ImageExtensionNotFoundException)
+import filetype
 
 
 class Validator:
     """
         Standard Validator for reSmushit
     """
-    def __init__(self, path, max_file_size):
+    def __init__(self, path, max_file_size, _type):
         self.path = path
-        self.type = None
+        self._type = _type
         self.max_file_size = max_file_size
         self.max_file_size_kb = max_file_size // 1024
         self.__ALLOWED_FILETYPES = ("png", "jpg", "jpeg", "gif", "bmp", "tiff", "tiff")
 
-    def __check_path_type(self):
-        parsed_url = urlparse(self.path)
-
-        if all([parsed_url.scheme, parsed_url.netloc, parsed_url.path]):
-            self.type = "url"
-            return "url"
-
-        if os.path.isfile(self.path) and os.path.exists(self.path):
-            self.type = "file"
-            return "file"
-        else:
-            raise FileNotFoundError(f"File {self.path} does not exist.")
-
     def __check_url_validity(self):
         if urlparse(self.path).scheme in ["http", "https", "ftp"]:
             return True
         else:
             raise ValueError(f"URL scheme required: {self.path}")
 
     def __file_exists(self):
         if os.path.exists(self.path):
             return True
         raise FileNotFoundError(f"{self.path}")
 
-    def __open_image_from_url(self):
+    def _open_image_from_url(self):
         http = PoolManager()
         r = http.request("GET", url=self.path)
         return r.data
 
-    def __open_image_from_path(self):
+    def _open_image_from_path(self):
         data = ""
         with open(self.path, "rb") as f:
             data = f.read()
         return data
 
-    def __find_image_extension(self, imagebytes):
-        return imghdr.what(None, h=imagebytes)
+    def _find_image_extension(self, imagebytes):
+        kind = filetype.guess(obj=imagebytes)
+        if kind.extension:
+            self.extension = kind.extension
+            return kind.extension
+        raise ImageExtensionNotFoundException(f"'{kind.extension}' image extension found")
+
 
     def __check_file_size(self, imagebytes):
 
         if len(imagebytes) > self.max_file_size:
             raise FileTooLargeError(
                 f"Max allowed file size: {self.max_file_size_kb}KB."
             )
 
     def __get_file_name(self):
         filename, _ = os.path.splitext(os.path.basename(urlparse(self.path).path))
         return filename
 
-    def __get_file_extension(self):
-        _, extension = os.path.splitext(os.path.basename(urlparse(self.path).path))
-        if extension == ".jpeg":
-            extension = ".jpg"
-        return extension
+    # def __get_file_extension(self):
+    #     _, extension = os.path.splitext(os.path.basename(urlparse(self.path).path))
+    #     return extension
 
     def __check_allowed_filetypes(self, imagebytes):
-        extension = self.__find_image_extension(imagebytes=imagebytes)
-        if not extension in self.__ALLOWED_FILETYPES:
+        
+        if not self.extension in self.__ALLOWED_FILETYPES:
             raise InvalidImageExtensionError(
-                f"'{extension}' extension type is not allowed.\nAllowed types: {self.__ALLOWED_FILETYPES}"
+                f"'{self.extension}' extension type is not allowed.\nAllowed types: {self.__ALLOWED_FILETYPES}"
             )
 
     def validate(self):
-        _type = self.__check_path_type()
-
-        if _type == "url":
+        if self._type == "url":
             self.__check_url_validity()
-            imagebytes = self.__open_image_from_url()
+            imagebytes = self._open_image_from_url()
+            self._find_image_extension(imagebytes=imagebytes)
             self.__check_allowed_filetypes(imagebytes=imagebytes)
             self.__check_file_size(imagebytes=imagebytes)
             filename = self.__get_file_name()
-            fileext = self.__get_file_extension()
-
-            return self.path, _type, imagebytes, filename, fileext
+            # fileext = self.__get_file_extension()
+            return  imagebytes, filename, self.extension
 
-        if _type == "file":
+        if self._type == "file":
             self.__file_exists()
-            imagebytes = self.__open_image_from_path()
+            imagebytes = self._open_image_from_path()
+            self._find_image_extension(imagebytes=imagebytes)
             self.__check_allowed_filetypes(imagebytes=imagebytes)
             filename = self.__get_file_name()
-            fileext = self.__get_file_extension()
+            # fileext = self.__get_file_extension()
             self.__check_file_size(imagebytes=imagebytes)
-            return self.path, _type, imagebytes, filename, fileext
+            return imagebytes, filename, self.extension
```

### Comparing `resmushit-1.0.0/resmushit.egg-info/PKG-INFO` & `resmushit-1.0.1/resmushit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: resmushit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper for resmush.it API
 Home-page: https://resmush.it/
+Download-URL: https://github.com/hemansah/resmushit
 Author: Hemant Sah
 Author-email: hemantsah18@gmail.com
 Maintainer: Hemant Sah
 License: MIT
 Project-URL: Homepage, https://resmush.it/
 Project-URL: Documentation, https://github.com/hemansah/resmushit/blob/master/README.md
 Project-URL: Repository, https://github.com/hemansah/resmushit/
@@ -23,35 +24,34 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6,<=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3
-Requires-Dist: colorama
+Requires-Dist: filetype
 
 # reSmush.it Image Optimizer Python package
 
-  
+[![Downloads](https://static.pepy.tech/badge/resmushit)](https://pepy.tech/project/resmushit)
+![Tests](https://github.com/hemansah/resmushit/actions/workflows/tests.yaml/badge.svg?branch=master)  
 
 ## Project Description
 
 Python3 wrapper for resmush.it API to optimize image file size.
 
-  
+    
 
 [resmush.it](https://resmush.it/) Image Optimizer allows you to use free Image optimization based on reSmush.it API.
 
 reSmush.it provides image size reduction based on several algorithms. The API accept JPG, PNG and GIF files up to 5MB.
 
-  
 
-## Installation
 
-  
+## Installation
 
 1. Install using pip3:
 
   
 
     `$ pip3 install resmushit`
```

### Comparing `resmushit-1.0.0/setup.py` & `resmushit-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pathlib
 import setuptools
 
 setuptools.setup(
     name="resmushit",
-    version="1.0.0",
+    version="1.0.1",
     description="A wrapper for resmush.it API",
     long_description=pathlib.Path("README.md").read_text(encoding='utf-8'),
     long_description_content_type="text/markdown",
     url="https://resmush.it/",
     author="Hemant Sah",
     author_email="hemantsah18@gmail.com",
     maintainer="Hemant Sah",
+    download_url="https://github.com/hemansah/resmushit",
     license="MIT",
     project_urls={
         "Homepage":"https://resmush.it/",
         "Documentation":"https://github.com/hemansah/resmushit/blob/master/README.md",
         "Repository":"https://github.com/hemansah/resmushit/",
     },
     classifiers=[
@@ -29,11 +30,11 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.6",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Scientific/Engineering :: Image Processing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6,<=3.12",
-    install_requires=['urllib3', 'colorama'],
-    packages=setuptools.find_packages(),
+    install_requires=['urllib3', 'filetype'],
+    packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     include_package_data=True,
 )
```

