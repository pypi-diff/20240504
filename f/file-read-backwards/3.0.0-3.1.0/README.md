# Comparing `tmp/file_read_backwards-3.0.0.tar.gz` & `tmp/file_read_backwards-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_read_backwards-3.0.0.tar", last modified: Wed Mar 29 17:45:29 2023, max compression
+gzip compressed data, was "file_read_backwards-3.1.0.tar", last modified: Sat May  4 17:35:35 2024, max compression
```

## Comparing `file_read_backwards-3.0.0.tar` & `file_read_backwards-3.1.0.tar`

### file list

```diff
@@ -1,51 +1,43 @@
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.957931 file_read_backwards-3.0.0/
--rw-r--r--   0 rrobin     (501) staff       (20)      137 2017-11-15 02:50:24.000000 file_read_backwards-3.0.0/AUTHORS.rst
--rw-r--r--   0 rrobin     (501) staff       (20)     3146 2023-03-29 03:47:02.000000 file_read_backwards-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 rrobin     (501) staff       (20)     1313 2023-03-29 17:37:01.000000 file_read_backwards-3.0.0/HISTORY.rst
--rw-r--r--   0 rrobin     (501) staff       (20)     1071 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/LICENSE
--rw-r--r--   0 rrobin     (501) staff       (20)      264 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/MANIFEST.in
--rw-r--r--   0 rrobin     (501) staff       (20)     4084 2023-03-29 17:45:29.958153 file_read_backwards-3.0.0/PKG-INFO
--rw-r--r--   0 rrobin     (501) staff       (20)     1917 2023-03-29 14:41:49.000000 file_read_backwards-3.0.0/README.rst
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.944509 file_read_backwards-3.0.0/docs/
--rw-r--r--   0 rrobin     (501) staff       (20)     6814 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/Makefile
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.934568 file_read_backwards-3.0.0/docs/_build/
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.934732 file_read_backwards-3.0.0/docs/_build/html/
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.950559 file_read_backwards-3.0.0/docs/_build/html/_static/
--rw-r--r--   0 rrobin     (501) staff       (20)      673 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 rrobin     (501) staff       (20)      756 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 rrobin     (501) staff       (20)      829 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 rrobin     (501) staff       (20)      641 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/comment.png
--rw-r--r--   0 rrobin     (501) staff       (20)      222 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 rrobin     (501) staff       (20)      202 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/down.png
--rw-r--r--   0 rrobin     (501) staff       (20)      286 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/file.png
--rw-r--r--   0 rrobin     (501) staff       (20)       90 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 rrobin     (501) staff       (20)       90 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 rrobin     (501) staff       (20)      214 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 rrobin     (501) staff       (20)      203 2017-01-22 17:48:18.000000 file_read_backwards-3.0.0/docs/_build/html/_static/up.png
--rw-r--r--   0 rrobin     (501) staff       (20)       28 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/authors.rst
--rwxr-xr-x   0 rrobin     (501) staff       (20)     8539 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/conf.py
--rw-r--r--   0 rrobin     (501) staff       (20)       33 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/contributing.rst
--rw-r--r--   0 rrobin     (501) staff       (20)      629 2023-03-29 14:41:49.000000 file_read_backwards-3.0.0/docs/file_read_backwards.rst
--rw-r--r--   0 rrobin     (501) staff       (20)       28 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/history.rst
--rw-r--r--   0 rrobin     (501) staff       (20)      290 2017-01-11 21:36:58.000000 file_read_backwards-3.0.0/docs/index.rst
--rw-r--r--   0 rrobin     (501) staff       (20)     1211 2017-11-15 02:56:18.000000 file_read_backwards-3.0.0/docs/installation.rst
--rw-r--r--   0 rrobin     (501) staff       (20)     6485 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/make.bat
--rw-r--r--   0 rrobin     (501) staff       (20)       94 2017-01-22 17:48:24.000000 file_read_backwards-3.0.0/docs/modules.rst
--rw-r--r--   0 rrobin     (501) staff       (20)       27 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/docs/readme.rst
--rw-r--r--   0 rrobin     (501) staff       (20)       45 2017-01-12 00:22:13.000000 file_read_backwards-3.0.0/docs/usage.rst
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.952588 file_read_backwards-3.0.0/file_read_backwards/
--rw-r--r--   0 rrobin     (501) staff       (20)      182 2023-03-29 17:34:29.000000 file_read_backwards-3.0.0/file_read_backwards/__init__.py
--rw-r--r--   0 rrobin     (501) staff       (20)     6499 2023-03-29 14:41:49.000000 file_read_backwards-3.0.0/file_read_backwards/buffer_work_space.py
--rw-r--r--   0 rrobin     (501) staff       (20)     4069 2018-03-28 01:53:09.000000 file_read_backwards-3.0.0/file_read_backwards/file_read_backwards.py
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.955535 file_read_backwards-3.0.0/file_read_backwards.egg-info/
--rw-r--r--   0 rrobin     (501) staff       (20)     4084 2023-03-29 17:45:29.000000 file_read_backwards-3.0.0/file_read_backwards.egg-info/PKG-INFO
--rw-r--r--   0 rrobin     (501) staff       (20)     1131 2023-03-29 17:45:29.000000 file_read_backwards-3.0.0/file_read_backwards.egg-info/SOURCES.txt
--rw-r--r--   0 rrobin     (501) staff       (20)        1 2023-03-29 17:45:29.000000 file_read_backwards-3.0.0/file_read_backwards.egg-info/dependency_links.txt
--rw-r--r--   0 rrobin     (501) staff       (20)        1 2023-03-29 17:45:29.000000 file_read_backwards-3.0.0/file_read_backwards.egg-info/not-zip-safe
--rw-r--r--   0 rrobin     (501) staff       (20)       20 2023-03-29 17:45:29.000000 file_read_backwards-3.0.0/file_read_backwards.egg-info/top_level.txt
--rw-r--r--   0 rrobin     (501) staff       (20)      427 2023-03-29 17:45:29.959178 file_read_backwards-3.0.0/setup.cfg
--rw-r--r--   0 rrobin     (501) staff       (20)     1463 2023-03-29 17:34:29.000000 file_read_backwards-3.0.0/setup.py
-drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2023-03-29 17:45:29.957462 file_read_backwards-3.0.0/tests/
--rw-r--r--   0 rrobin     (501) staff       (20)       24 2016-12-18 19:08:44.000000 file_read_backwards-3.0.0/tests/__init__.py
--rw-r--r--   0 rrobin     (501) staff       (20)    19756 2018-03-28 01:53:09.000000 file_read_backwards-3.0.0/tests/test_buffer_work_space.py
--rw-r--r--   0 rrobin     (501) staff       (20)    11849 2023-03-29 14:41:49.000000 file_read_backwards-3.0.0/tests/test_file_read_backwards.py
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.872686 file_read_backwards-3.1.0/
+-rw-r--r--   0 rrobin     (501) staff       (20)      137 2017-11-15 02:50:24.000000 file_read_backwards-3.1.0/AUTHORS.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)     3146 2023-03-29 03:47:02.000000 file_read_backwards-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)     1392 2024-05-04 17:19:43.000000 file_read_backwards-3.1.0/HISTORY.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)     1071 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/LICENSE
+-rw-r--r--   0 rrobin     (501) staff       (20)      264 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/MANIFEST.in
+-rw-r--r--   0 rrobin     (501) staff       (20)     4214 2024-05-04 17:35:35.872819 file_read_backwards-3.1.0/PKG-INFO
+-rw-r--r--   0 rrobin     (501) staff       (20)     1917 2023-03-29 14:41:49.000000 file_read_backwards-3.1.0/README.rst
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.869611 file_read_backwards-3.1.0/docs/
+-rw-r--r--   0 rrobin     (501) staff       (20)     6814 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/Makefile
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.864781 file_read_backwards-3.1.0/docs/_build/
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.864849 file_read_backwards-3.1.0/docs/_build/html/
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.870142 file_read_backwards-3.1.0/docs/_build/html/_static/
+-rw-r--r--   0 rrobin     (501) staff       (20)      286 2023-03-29 17:34:48.000000 file_read_backwards-3.1.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 rrobin     (501) staff       (20)       90 2023-03-29 17:34:48.000000 file_read_backwards-3.1.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 rrobin     (501) staff       (20)       90 2023-03-29 17:34:48.000000 file_read_backwards-3.1.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 rrobin     (501) staff       (20)       28 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/authors.rst
+-rwxr-xr-x   0 rrobin     (501) staff       (20)     8539 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/conf.py
+-rw-r--r--   0 rrobin     (501) staff       (20)       33 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/contributing.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)      629 2023-03-29 17:49:24.000000 file_read_backwards-3.1.0/docs/file_read_backwards.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)       28 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/history.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)      290 2017-01-11 21:36:58.000000 file_read_backwards-3.1.0/docs/index.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)     1211 2017-11-15 02:56:18.000000 file_read_backwards-3.1.0/docs/installation.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)     6485 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/make.bat
+-rw-r--r--   0 rrobin     (501) staff       (20)       94 2023-03-29 17:49:24.000000 file_read_backwards-3.1.0/docs/modules.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)       27 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/docs/readme.rst
+-rw-r--r--   0 rrobin     (501) staff       (20)       45 2017-01-12 00:22:13.000000 file_read_backwards-3.1.0/docs/usage.rst
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.870930 file_read_backwards-3.1.0/file_read_backwards/
+-rw-r--r--   0 rrobin     (501) staff       (20)      182 2024-05-04 17:24:14.000000 file_read_backwards-3.1.0/file_read_backwards/__init__.py
+-rw-r--r--   0 rrobin     (501) staff       (20)     6499 2023-06-09 03:04:02.000000 file_read_backwards-3.1.0/file_read_backwards/buffer_work_space.py
+-rw-r--r--   0 rrobin     (501) staff       (20)     4069 2023-04-01 03:05:22.000000 file_read_backwards-3.1.0/file_read_backwards/file_read_backwards.py
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.871799 file_read_backwards-3.1.0/file_read_backwards.egg-info/
+-rw-r--r--   0 rrobin     (501) staff       (20)     4214 2024-05-04 17:35:35.000000 file_read_backwards-3.1.0/file_read_backwards.egg-info/PKG-INFO
+-rw-r--r--   0 rrobin     (501) staff       (20)      818 2024-05-04 17:35:35.000000 file_read_backwards-3.1.0/file_read_backwards.egg-info/SOURCES.txt
+-rw-r--r--   0 rrobin     (501) staff       (20)        1 2024-05-04 17:35:35.000000 file_read_backwards-3.1.0/file_read_backwards.egg-info/dependency_links.txt
+-rw-r--r--   0 rrobin     (501) staff       (20)        1 2024-05-04 17:35:35.000000 file_read_backwards-3.1.0/file_read_backwards.egg-info/not-zip-safe
+-rw-r--r--   0 rrobin     (501) staff       (20)       20 2024-05-04 17:35:35.000000 file_read_backwards-3.1.0/file_read_backwards.egg-info/top_level.txt
+-rw-r--r--   0 rrobin     (501) staff       (20)      427 2024-05-04 17:35:35.873140 file_read_backwards-3.1.0/setup.cfg
+-rw-r--r--   0 rrobin     (501) staff       (20)     1513 2024-05-04 17:24:14.000000 file_read_backwards-3.1.0/setup.py
+drwxr-xr-x   0 rrobin     (501) staff       (20)        0 2024-05-04 17:35:35.872482 file_read_backwards-3.1.0/tests/
+-rw-r--r--   0 rrobin     (501) staff       (20)       24 2016-12-18 19:08:44.000000 file_read_backwards-3.1.0/tests/__init__.py
+-rw-r--r--   0 rrobin     (501) staff       (20)    19756 2023-06-09 03:04:02.000000 file_read_backwards-3.1.0/tests/test_buffer_work_space.py
+-rw-r--r--   0 rrobin     (501) staff       (20)    11849 2023-06-09 03:04:02.000000 file_read_backwards-3.1.0/tests/test_file_read_backwards.py
```

### Comparing `file_read_backwards-3.0.0/CONTRIBUTING.rst` & `file_read_backwards-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/HISTORY.rst` & `file_read_backwards-3.1.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -49,7 +49,12 @@
 * Adding readline() function retuns one line at a time with a trailing new line and empty string when it reaches end of file.
   The fine print: the trailing new line will be `os.linesep` (rather than whichever new line type in the file).
 
 3.0.0 (2023-03-29)
 ------------------
 
 * Officially support Python 3.7 - 3.11.
+
+3.1.0 (2024-05-02)
+------------------
+
+* Officially support Python 3.7 - 3.12
```

### Comparing `file_read_backwards-3.0.0/LICENSE` & `file_read_backwards-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/PKG-INFO` & `file_read_backwards-3.1.0/file_read_backwards.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: file_read_backwards
-Version: 3.0.0
+Name: file-read-backwards
+Version: 3.1.0
 Summary: Memory efficient way of reading files line-by-line from the end of file
 Home-page: https://github.com/RobinNil/file_read_backwards
 Author: Robin Robin
 Author-email: robinsquare42@gmail.com
 License: MIT license
 Keywords: file_read_backwards
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 file_read_backwards
 ===============================
 
@@ -140,7 +141,12 @@
 * Adding readline() function retuns one line at a time with a trailing new line and empty string when it reaches end of file.
   The fine print: the trailing new line will be `os.linesep` (rather than whichever new line type in the file).
 
 3.0.0 (2023-03-29)
 ------------------
 
 * Officially support Python 3.7 - 3.11.
+
+3.1.0 (2024-05-02)
+------------------
+
+* Officially support Python 3.7 - 3.12
```

### Comparing `file_read_backwards-3.0.0/README.rst` & `file_read_backwards-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/docs/Makefile` & `file_read_backwards-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/docs/conf.py` & `file_read_backwards-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/docs/file_read_backwards.rst` & `file_read_backwards-3.1.0/docs/file_read_backwards.rst`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/docs/installation.rst` & `file_read_backwards-3.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/docs/make.bat` & `file_read_backwards-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/file_read_backwards/buffer_work_space.py` & `file_read_backwards-3.1.0/file_read_backwards/buffer_work_space.py`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/file_read_backwards/file_read_backwards.py` & `file_read_backwards-3.1.0/file_read_backwards/file_read_backwards.py`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/file_read_backwards.egg-info/PKG-INFO` & `file_read_backwards-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: file-read-backwards
-Version: 3.0.0
+Name: file_read_backwards
+Version: 3.1.0
 Summary: Memory efficient way of reading files line-by-line from the end of file
 Home-page: https://github.com/RobinNil/file_read_backwards
 Author: Robin Robin
 Author-email: robinsquare42@gmail.com
 License: MIT license
 Keywords: file_read_backwards
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 file_read_backwards
 ===============================
 
@@ -140,7 +141,12 @@
 * Adding readline() function retuns one line at a time with a trailing new line and empty string when it reaches end of file.
   The fine print: the trailing new line will be `os.linesep` (rather than whichever new line type in the file).
 
 3.0.0 (2023-03-29)
 ------------------
 
 * Officially support Python 3.7 - 3.11.
+
+3.1.0 (2024-05-02)
+------------------
+
+* Officially support Python 3.7 - 3.12
```

### Comparing `file_read_backwards-3.0.0/setup.py` & `file_read_backwards-3.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 test_requirements = [
     "mock",
 ]
 
 setup(
     name='file_read_backwards',
-    version='3.0.0',
+    version='3.1.0',
     description="Memory efficient way of reading files line-by-line from the end of file",
     long_description=readme + '\n\n' + history,
     author="Robin Robin",
     author_email='robinsquare42@gmail.com',
     url='https://github.com/RobinNil/file_read_backwards',
     packages=[
         'file_read_backwards',
@@ -41,11 +41,12 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     test_suite='tests',
     tests_require=test_requirements
 )
```

### Comparing `file_read_backwards-3.0.0/tests/test_buffer_work_space.py` & `file_read_backwards-3.1.0/tests/test_buffer_work_space.py`

 * *Files identical despite different names*

### Comparing `file_read_backwards-3.0.0/tests/test_file_read_backwards.py` & `file_read_backwards-3.1.0/tests/test_file_read_backwards.py`

 * *Files identical despite different names*

