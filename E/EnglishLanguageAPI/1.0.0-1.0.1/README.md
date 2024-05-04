# Comparing `tmp/englishlanguageapi-1.0.0.tar.gz` & `tmp/englishlanguageapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "englishlanguageapi-1.0.0.tar", last modified: Fri May  3 23:52:28 2024, max compression
+gzip compressed data, was "englishlanguageapi-1.0.1.tar", last modified: Sat May  4 00:03:23 2024, max compression
```

## Comparing `englishlanguageapi-1.0.0.tar` & `englishlanguageapi-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.773885 englishlanguageapi-1.0.0/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1812 2024-05-03 23:52:28.770552 englishlanguageapi-1.0.0/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      660 2024-05-03 23:50:09.000000 englishlanguageapi-1.0.0/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1244 2024-05-03 23:47:07.000000 englishlanguageapi-1.0.0/readme.md
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2024-05-03 23:52:28.773885 englishlanguageapi-1.0.0/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.687218 englishlanguageapi-1.0.0/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.713885 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.757218 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/API/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2581 2024-05-03 20:42:49.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/API/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     4909 2024-05-03 22:36:07.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-03 23:52:28.760552 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1812 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      327 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       13 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/requires.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       19 2024-05-03 23:52:28.000000 englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-04 00:03:23.884756 englishlanguageapi-1.0.1/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1812 2024-05-04 00:03:23.884756 englishlanguageapi-1.0.1/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      660 2024-05-04 00:02:26.000000 englishlanguageapi-1.0.1/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1244 2024-05-03 23:47:07.000000 englishlanguageapi-1.0.1/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2024-05-04 00:03:23.891423 englishlanguageapi-1.0.1/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-04 00:03:23.818090 englishlanguageapi-1.0.1/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-04 00:03:23.828090 englishlanguageapi-1.0.1/src/EnglishLanguageAPI/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-04 00:03:23.861423 englishlanguageapi-1.0.1/src/EnglishLanguageAPI/API/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2581 2024-05-03 20:42:49.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI/API/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     4911 2024-05-04 00:02:02.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2024-05-04 00:03:23.874756 englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1812 2024-05-04 00:03:23.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      327 2024-05-04 00:03:23.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2024-05-04 00:03:23.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       13 2024-05-04 00:03:23.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/requires.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       19 2024-05-04 00:03:23.000000 englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/top_level.txt
```

### Comparing `englishlanguageapi-1.0.0/PKG-INFO` & `englishlanguageapi-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnglishLanguageAPI
-Version: 1.0.0
+Version: 1.0.1
 Summary: A CLI tool for looking up the meanings of things.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/guyyatsu/EnglishLanguageAPI
 Project-URL: Issues, https://github.com/guyyatsu/EnglishLanguageAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `englishlanguageapi-1.0.0/pyproject.toml` & `englishlanguageapi-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EnglishLanguageAPI"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 description = "A CLI tool for looking up the meanings of things."
 readme = "readme.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `englishlanguageapi-1.0.0/readme.md` & `englishlanguageapi-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `englishlanguageapi-1.0.0/src/EnglishLanguageAPI/API/__init__.py` & `englishlanguageapi-1.0.1/src/EnglishLanguageAPI/API/__init__.py`

 * *Files identical despite different names*

### Comparing `englishlanguageapi-1.0.0/src/EnglishLanguageAPI/__init__.py` & `englishlanguageapi-1.0.1/src/EnglishLanguageAPI/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from API import EnglishDictionary
-from API import EnglishVocabulary
+from .API import EnglishDictionary
+from .API import EnglishVocabulary
 
 from argparse import ArgumentParser
 from sqlite3 import connect
 from random import choice
 from time import sleep
 
 from logging import basicConfig, info, INFO
```

### Comparing `englishlanguageapi-1.0.0/src/EnglishLanguageAPI.egg-info/PKG-INFO` & `englishlanguageapi-1.0.1/src/EnglishLanguageAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnglishLanguageAPI
-Version: 1.0.0
+Version: 1.0.1
 Summary: A CLI tool for looking up the meanings of things.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/guyyatsu/EnglishLanguageAPI
 Project-URL: Issues, https://github.com/guyyatsu/EnglishLanguageAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

