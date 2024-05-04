# Comparing `tmp/testpulse-uploader-0.0.8.tar.gz` & `tmp/testpulse-uploader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpulse-uploader-0.0.8.tar", last modified: Sat Feb 10 20:54:45 2024, max compression
+gzip compressed data, was "testpulse-uploader-0.0.9.tar", last modified: Tue Feb 20 20:47:11 2024, max compression
```

## Comparing `testpulse-uploader-0.0.8.tar` & `testpulse-uploader-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dspadini   (501) staff       (20)        0 2024-02-10 20:54:45.741116 testpulse-uploader-0.0.8/
--rw-r--r--   0 dspadini   (501) staff       (20)      277 2024-01-31 11:03:40.000000 testpulse-uploader-0.0.8/LICENSE
--rw-r--r--   0 dspadini   (501) staff       (20)      618 2024-02-10 20:54:45.740678 testpulse-uploader-0.0.8/PKG-INFO
--rw-r--r--   0 dspadini   (501) staff       (20)       55 2024-01-31 11:00:24.000000 testpulse-uploader-0.0.8/README.md
--rw-r--r--   0 dspadini   (501) staff       (20)      800 2024-02-10 20:54:33.000000 testpulse-uploader-0.0.8/pyproject.toml
--rw-r--r--   0 dspadini   (501) staff       (20)       38 2024-02-10 20:54:45.741174 testpulse-uploader-0.0.8/setup.cfg
-drwxr-xr-x   0 dspadini   (501) staff       (20)        0 2024-02-10 20:54:45.740157 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/
--rw-r--r--   0 dspadini   (501) staff       (20)      618 2024-02-10 20:54:45.000000 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/PKG-INFO
--rw-r--r--   0 dspadini   (501) staff       (20)      519 2024-02-10 20:54:45.000000 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 dspadini   (501) staff       (20)        1 2024-02-10 20:54:45.000000 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 dspadini   (501) staff       (20)       56 2024-02-10 20:54:45.000000 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/entry_points.txt
--rw-r--r--   0 dspadini   (501) staff       (20)       34 2024-02-10 20:54:45.000000 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/requires.txt
--rw-r--r--   0 dspadini   (501) staff       (20)        9 2024-02-10 20:54:45.000000 testpulse-uploader-0.0.8/testpulse_uploader.egg-info/top_level.txt
-drwxr-xr-x   0 dspadini   (501) staff       (20)        0 2024-02-10 20:54:45.736788 testpulse-uploader-0.0.8/tests/
--rw-r--r--   0 dspadini   (501) staff       (20)     1115 2024-02-10 20:04:49.000000 testpulse-uploader-0.0.8/tests/test_authentication.py
--rw-r--r--   0 dspadini   (501) staff       (20)     1868 2024-02-10 20:03:41.000000 testpulse-uploader-0.0.8/tests/test_upload.py
--rw-r--r--   0 dspadini   (501) staff       (20)      989 2024-02-05 13:52:57.000000 testpulse-uploader-0.0.8/tests/test_zipper.py
-drwxr-xr-x   0 dspadini   (501) staff       (20)        0 2024-02-10 20:54:45.739792 testpulse-uploader-0.0.8/uploader/
--rw-r--r--   0 dspadini   (501) staff       (20)        0 2024-01-29 11:57:32.000000 testpulse-uploader-0.0.8/uploader/__init__.py
--rw-r--r--   0 dspadini   (501) staff       (20)      790 2024-02-10 20:03:53.000000 testpulse-uploader-0.0.8/uploader/authentication.py
--rw-r--r--   0 dspadini   (501) staff       (20)      958 2024-02-08 16:03:37.000000 testpulse-uploader-0.0.8/uploader/domain.py
--rw-r--r--   0 dspadini   (501) staff       (20)      704 2024-02-03 17:02:10.000000 testpulse-uploader-0.0.8/uploader/exceptions.py
--rwxr-xr-x   0 dspadini   (501) staff       (20)     2554 2024-02-08 16:06:41.000000 testpulse-uploader-0.0.8/uploader/main.py
--rw-r--r--   0 dspadini   (501) staff       (20)     1159 2024-02-10 20:40:24.000000 testpulse-uploader-0.0.8/uploader/upload.py
--rw-r--r--   0 dspadini   (501) staff       (20)      194 2024-02-10 19:40:24.000000 testpulse-uploader-0.0.8/uploader/urls.py
--rw-r--r--   0 dspadini   (501) staff       (20)     1798 2024-02-05 10:46:55.000000 testpulse-uploader-0.0.8/uploader/zipper.py
+drwxr-xr-x   0 ishepard   (501) staff       (20)        0 2024-02-20 20:47:11.611111 testpulse-uploader-0.0.9/
+-rw-r--r--   0 ishepard   (501) staff       (20)      277 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/LICENSE
+-rw-r--r--   0 ishepard   (501) staff       (20)      618 2024-02-20 20:47:11.610923 testpulse-uploader-0.0.9/PKG-INFO
+-rw-r--r--   0 ishepard   (501) staff       (20)       55 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/README.md
+-rw-r--r--   0 ishepard   (501) staff       (20)      800 2024-02-20 20:44:23.000000 testpulse-uploader-0.0.9/pyproject.toml
+-rw-r--r--   0 ishepard   (501) staff       (20)       38 2024-02-20 20:47:11.611151 testpulse-uploader-0.0.9/setup.cfg
+drwxr-xr-x   0 ishepard   (501) staff       (20)        0 2024-02-20 20:47:11.610660 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/
+-rw-r--r--   0 ishepard   (501) staff       (20)      618 2024-02-20 20:47:11.000000 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 ishepard   (501) staff       (20)      519 2024-02-20 20:47:11.000000 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 ishepard   (501) staff       (20)        1 2024-02-20 20:47:11.000000 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 ishepard   (501) staff       (20)       56 2024-02-20 20:47:11.000000 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 ishepard   (501) staff       (20)       34 2024-02-20 20:47:11.000000 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/requires.txt
+-rw-r--r--   0 ishepard   (501) staff       (20)        9 2024-02-20 20:47:11.000000 testpulse-uploader-0.0.9/testpulse_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 ishepard   (501) staff       (20)        0 2024-02-20 20:47:11.609325 testpulse-uploader-0.0.9/tests/
+-rw-r--r--   0 ishepard   (501) staff       (20)     1115 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/tests/test_authentication.py
+-rw-r--r--   0 ishepard   (501) staff       (20)     1453 2024-02-20 18:37:49.000000 testpulse-uploader-0.0.9/tests/test_upload.py
+-rw-r--r--   0 ishepard   (501) staff       (20)      989 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/tests/test_zipper.py
+drwxr-xr-x   0 ishepard   (501) staff       (20)        0 2024-02-20 20:47:11.610515 testpulse-uploader-0.0.9/uploader/
+-rw-r--r--   0 ishepard   (501) staff       (20)        0 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/uploader/__init__.py
+-rw-r--r--   0 ishepard   (501) staff       (20)      790 2024-02-20 20:45:35.000000 testpulse-uploader-0.0.9/uploader/authentication.py
+-rw-r--r--   0 ishepard   (501) staff       (20)     2262 2024-02-20 18:38:53.000000 testpulse-uploader-0.0.9/uploader/domain.py
+-rw-r--r--   0 ishepard   (501) staff       (20)      704 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/uploader/exceptions.py
+-rwxr-xr-x   0 ishepard   (501) staff       (20)     3205 2024-02-20 18:39:02.000000 testpulse-uploader-0.0.9/uploader/main.py
+-rw-r--r--   0 ishepard   (501) staff       (20)     1185 2024-02-20 20:45:35.000000 testpulse-uploader-0.0.9/uploader/upload.py
+-rw-r--r--   0 ishepard   (501) staff       (20)      194 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/uploader/urls.py
+-rw-r--r--   0 ishepard   (501) staff       (20)     1798 2024-02-14 09:26:59.000000 testpulse-uploader-0.0.9/uploader/zipper.py
```

### Comparing `testpulse-uploader-0.0.8/PKG-INFO` & `testpulse-uploader-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpulse-uploader
-Version: 0.0.8
+Version: 0.0.9
 Summary: Upload test results to testpulse
 Author-email: Davide Spadini <spadini.davide@gmail.com>, Mauricio Aniche <mauricioaniche@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `testpulse-uploader-0.0.8/pyproject.toml` & `testpulse-uploader-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "testpulse-uploader"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Davide Spadini", email="spadini.davide@gmail.com" },
   { name="Mauricio Aniche", email="mauricioaniche@gmail.com" }
 ]
 description = "Upload test results to testpulse"
 readme = "README.md"
 dependencies = [
```

### Comparing `testpulse-uploader-0.0.8/testpulse_uploader.egg-info/PKG-INFO` & `testpulse-uploader-0.0.9/testpulse_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpulse-uploader
-Version: 0.0.8
+Version: 0.0.9
 Summary: Upload test results to testpulse
 Author-email: Davide Spadini <spadini.davide@gmail.com>, Mauricio Aniche <mauricioaniche@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `testpulse-uploader-0.0.8/testpulse_uploader.egg-info/SOURCES.txt` & `testpulse-uploader-0.0.9/testpulse_uploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testpulse-uploader-0.0.8/tests/test_authentication.py` & `testpulse-uploader-0.0.9/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `testpulse-uploader-0.0.8/tests/test_zipper.py` & `testpulse-uploader-0.0.9/tests/test_zipper.py`

 * *Files identical despite different names*

### Comparing `testpulse-uploader-0.0.8/uploader/authentication.py` & `testpulse-uploader-0.0.9/uploader/authentication.py`

 * *Files identical despite different names*

### Comparing `testpulse-uploader-0.0.8/uploader/exceptions.py` & `testpulse-uploader-0.0.9/uploader/exceptions.py`

 * *Files identical despite different names*

### Comparing `testpulse-uploader-0.0.8/uploader/main.py` & `testpulse-uploader-0.0.9/uploader/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse
 import logging
 from pathlib import Path
 import re
 from typing import Optional, Pattern
 from uploader.authentication import authenticate
+from uploader.domain import TestRun
 
 from uploader.upload import upload_test_results
 from uploader.zipper import find_files, zip_files
 
 logging.basicConfig(format='%(asctime)s-%(levelname)s:%(filename)s:%(lineno)d %(message)s', level=logging.INFO)
 logger = logging.getLogger(__name__)
 
@@ -63,14 +64,38 @@
     parser.add_argument(
         "-l",
         "--localhost",
         help="Regex pattern to find test results XML files",
         action='store_true'
     )
 
+    parser.add_argument(
+        "-os",
+        "--operating-system",
+        help="OS where the tests run."
+    )
+
+    parser.add_argument(
+        "-lv",
+        "--language-version",
+        help="Language version. For example for Python it can be 3.11, 3.12.. For Java, 17, 21, etc.."
+    )
+
+    parser.add_argument(
+        "-tfv",
+        "--test-framework-version",
+        help="Version of the test framework. For example, Pytest 8.0.0"
+    )
+
+    parser.add_argument(
+        "-ghi",
+        "--github-run-id",
+        help="GitHub Run ID, from the env variable GITHUB_RUN_ID."
+    )
+
     return parser
 
 
 def run(args: argparse.Namespace) -> None:
     root = Path().resolve()
     logger.info('Authenticating...')
     authenticate()
@@ -81,15 +106,18 @@
     zip_file_name = zip_files(files_list=selected_files, root=root)
     if zip_file_name is None:
         return
 
     logger.info(f'Saved zip file in {zip_file_name}.')
 
     logger.info('Uploading to our backend server...')
-    req = upload_test_results(Path(zip_file_name), localhost=args.localhost)
+
+    testRun = TestRun(args)
+
+    req = upload_test_results(Path(zip_file_name), testRun=testRun)
 
     if req is True:
         logger.info('Upload was successful!')
 
 
 def main():
     parser = create_parser()
```

### Comparing `testpulse-uploader-0.0.8/uploader/zipper.py` & `testpulse-uploader-0.0.9/uploader/zipper.py`

 * *Files identical despite different names*

