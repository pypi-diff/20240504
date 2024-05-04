# Comparing `tmp/abstract_pandas-0.0.0.5.tar.gz` & `tmp/abstract_pandas-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.5.tar", last modified: Fri May  3 07:53:18 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.6.tar", last modified: Sat May  4 03:08:18 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.5.tar` & `abstract_pandas-0.0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.5/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-05-03 07:53:00.000000 abstract_pandas-0.0.0.5/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.115340 abstract_pandas-0.0.0.5/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/class_manager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    15967 2024-05-03 07:52:16.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      290 2024-05-03 07:49:52.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/test_sol.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/time_module.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      544 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:08:18.660647 abstract_pandas-0.0.0.6/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-04 03:08:18.660647 abstract_pandas-0.0.0.6/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.6/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-04 03:08:18.660647 abstract_pandas-0.0.0.6/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-05-04 03:08:11.000000 abstract_pandas-0.0.0.6/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:08:18.660647 abstract_pandas-0.0.0.6/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:08:18.660647 abstract_pandas-0.0.0.6/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/class_manager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15967 2024-05-03 07:52:16.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/geo_pandas.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/geo_spec.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      290 2024-05-03 07:49:52.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/test_sol.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.6/src/abstract_pandas/time_module.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-04 03:08:18.660647 abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-04 03:08:18.000000 abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      544 2024-05-04 03:08:18.000000 abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-04 03:08:18.000000 abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-04 03:08:18.000000 abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-04 03:08:18.000000 abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.5/setup.py` & `abstract_pandas-0.0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.5',
+    version='0.0.0.6',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.6/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.6/src/abstract_pandas/excel_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.6/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas/geo_pandas.py` & `abstract_pandas-0.0.0.6/src/abstract_pandas/geo_pandas.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas/geo_spec.py` & `abstract_pandas-0.0.0.6/src/abstract_pandas/geo_spec.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas/time_module.py` & `abstract_pandas-0.0.0.6/src/abstract_pandas/time_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.6/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

