# Comparing `tmp/python-bvk-0.3.0.tar.gz` & `tmp/python-bvk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bvk-0.3.0.tar", last modified: Sun Apr  7 10:10:01 2024, max compression
+gzip compressed data, was "python-bvk-0.3.1.tar", last modified: Sat May  4 18:52:09 2024, max compression
```

## Comparing `python-bvk-0.3.0.tar` & `python-bvk-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.717184 python-bvk-0.3.0/
--rw-r--r--   0 dan       (1000) dan       (1000)    11357 2020-08-07 19:27:30.000000 python-bvk-0.3.0/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)     3405 2024-04-07 10:10:01.717184 python-bvk-0.3.0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     2919 2021-12-14 21:55:17.000000 python-bvk-0.3.0/README.md
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.716184 python-bvk-0.3.0/bvk/
--rw-r--r--   0 dan       (1000) dan       (1000)     1867 2021-12-14 21:50:15.000000 python-bvk-0.3.0/bvk/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)      645 2021-09-25 10:08:10.000000 python-bvk-0.3.0/bvk/items.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3263 2020-08-07 19:27:30.000000 python-bvk-0.3.0/bvk/settings.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.716184 python-bvk-0.3.0/bvk/spiders/
--rw-r--r--   0 dan       (1000) dan       (1000)      161 2020-08-07 19:27:30.000000 python-bvk-0.3.0/bvk/spiders/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)     5219 2024-04-07 09:56:55.000000 python-bvk-0.3.0/bvk/spiders/water_consumption.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.717184 python-bvk-0.3.0/python_bvk.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     3405 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      297 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       23 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        4 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2024-04-07 10:10:01.717184 python-bvk-0.3.0/setup.cfg
--rw-r--r--   0 dan       (1000) dan       (1000)      785 2024-04-07 09:57:47.000000 python-bvk-0.3.0/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-04 18:52:09.972473 python-bvk-0.3.1/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11357 2020-08-07 19:27:30.000000 python-bvk-0.3.1/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)     3405 2024-05-04 18:52:09.971473 python-bvk-0.3.1/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     2919 2021-12-14 21:55:17.000000 python-bvk-0.3.1/README.md
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-04 18:52:09.969473 python-bvk-0.3.1/bvk/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1867 2021-12-14 21:50:15.000000 python-bvk-0.3.1/bvk/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      645 2021-09-25 10:08:10.000000 python-bvk-0.3.1/bvk/items.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3307 2024-04-07 10:58:53.000000 python-bvk-0.3.1/bvk/settings.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-04 18:52:09.970473 python-bvk-0.3.1/bvk/spiders/
+-rw-r--r--   0 dan       (1000) dan       (1000)      161 2020-08-07 19:27:30.000000 python-bvk-0.3.1/bvk/spiders/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     5219 2024-04-07 09:56:55.000000 python-bvk-0.3.1/bvk/spiders/water_consumption.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-05-04 18:52:09.971473 python-bvk-0.3.1/python_bvk.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     3405 2024-05-04 18:52:09.000000 python-bvk-0.3.1/python_bvk.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      297 2024-05-04 18:52:09.000000 python-bvk-0.3.1/python_bvk.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2024-05-04 18:52:09.000000 python-bvk-0.3.1/python_bvk.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       23 2024-05-04 18:52:09.000000 python-bvk-0.3.1/python_bvk.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        4 2024-05-04 18:52:09.000000 python-bvk-0.3.1/python_bvk.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2024-05-04 18:52:09.972473 python-bvk-0.3.1/setup.cfg
+-rw-r--r--   0 dan       (1000) dan       (1000)      785 2024-05-04 18:51:31.000000 python-bvk-0.3.1/setup.py
```

### Comparing `python-bvk-0.3.0/LICENSE` & `python-bvk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bvk-0.3.0/PKG-INFO` & `python-bvk-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bvk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)
 Home-page: https://github.com/dankeder/python-bvk
 Author: Dan Keder
 Author-email: dan.keder@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-bvk-0.3.0/README.md` & `python-bvk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-bvk-0.3.0/bvk/__init__.py` & `python-bvk-0.3.1/bvk/__init__.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.3.0/bvk/items.py` & `python-bvk-0.3.1/bvk/items.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.3.0/bvk/settings.py` & `python-bvk-0.3.1/bvk/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,7 +91,9 @@
 #HTTPCACHE_EXPIRATION_SECS = 0
 #HTTPCACHE_DIR = 'httpcache'
 #HTTPCACHE_IGNORE_HTTP_CODES = []
 #HTTPCACHE_STORAGE = 'scrapy.extensions.httpcache.FilesystemCacheStorage'
 
 LOG_ENABLED = True
 LOG_LEVEL = logging.ERROR
+
+REQUEST_FINGERPRINTER_IMPLEMENTATION='2.7'
```

### Comparing `python-bvk-0.3.0/bvk/spiders/water_consumption.py` & `python-bvk-0.3.1/bvk/spiders/water_consumption.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.3.0/python_bvk.egg-info/PKG-INFO` & `python-bvk-0.3.1/python_bvk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bvk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)
 Home-page: https://github.com/dankeder/python-bvk
 Author: Dan Keder
 Author-email: dan.keder@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-bvk-0.3.0/setup.py` & `python-bvk-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = ["scrapy", "python-dateutil"]
 
 setuptools.setup(
     name="python-bvk",
-    version="0.3.0",
+    version="0.3.1",
     author="Dan Keder",
     author_email="dan.keder@protonmail.com",
     description="Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dankeder/python-bvk",
     packages=setuptools.find_packages(),
```

