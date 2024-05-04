# Comparing `tmp/cached_historical_data_fetcher-0.2.8.tar.gz` & `tmp/cached_historical_data_fetcher-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cached_historical_data_fetcher-0.2.8.tar", max compression
+gzip compressed data, was "cached_historical_data_fetcher-0.2.9.tar", max compression
```

## Comparing `cached_historical_data_fetcher-0.2.8.tar` & `cached_historical_data_fetcher-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2024-01-02 04:43:15.704062 cached_historical_data_fetcher-0.2.8/LICENSE
--rw-r--r--   0        0        0     6783 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/README.md
--rw-r--r--   0        0        0     3036 2024-01-02 04:43:16.536057 cached_historical_data_fetcher-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      319 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/__init__.py
--rw-r--r--   0        0        0      307 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/__init__.py
--rw-r--r--   0        0        0     9869 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/base.py
--rw-r--r--   0        0        0     8319 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/chunk.py
--rw-r--r--   0        0        0     2195 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/id.py
--rw-r--r--   0        0        0     4359 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/io.py
--rw-r--r--   0        0        0        0 2024-01-02 04:43:15.708062 cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/py.typed
--rw-r--r--   0        0        0     8346 1970-01-01 00:00:00.000000 cached_historical_data_fetcher-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6783 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/README.md
+-rw-r--r--   0        0        0     3036 2024-01-03 04:37:37.407352 cached_historical_data_fetcher-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      319 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/__init__.py
+-rw-r--r--   0        0        0      307 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/__init__.py
+-rw-r--r--   0        0        0     9869 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/base.py
+-rw-r--r--   0        0        0     8319 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/chunk.py
+-rw-r--r--   0        0        0     2195 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/id.py
+-rw-r--r--   0        0        0     4359 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/io.py
+-rw-r--r--   0        0        0        0 2024-01-03 04:37:36.667344 cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/py.typed
+-rw-r--r--   0        0        0     8346 1970-01-01 00:00:00.000000 cached_historical_data_fetcher-0.2.9/PKG-INFO
```

### Comparing `cached_historical_data_fetcher-0.2.8/LICENSE` & `cached_historical_data_fetcher-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cached_historical_data_fetcher-0.2.8/README.md` & `cached_historical_data_fetcher-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cached_historical_data_fetcher-0.2.8/pyproject.toml` & `cached_historical_data_fetcher-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cached-historical-data-fetcher"
-version = "0.2.8"
+version = "0.2.9"
 description = "Python utility for fetching any historical data using caching."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/cached-historical-data-fetcher"
 documentation = "https://cached-historical-data-fetcher.readthedocs.io"
 classifiers = [
```

### Comparing `cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/base.py` & `cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/base.py`

 * *Files identical despite different names*

### Comparing `cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/chunk.py` & `cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/chunk.py`

 * *Files identical despite different names*

### Comparing `cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/cache/id.py` & `cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/cache/id.py`

 * *Files identical despite different names*

### Comparing `cached_historical_data_fetcher-0.2.8/src/cached_historical_data_fetcher/io.py` & `cached_historical_data_fetcher-0.2.9/src/cached_historical_data_fetcher/io.py`

 * *Files identical despite different names*

### Comparing `cached_historical_data_fetcher-0.2.8/PKG-INFO` & `cached_historical_data_fetcher-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached-historical-data-fetcher
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python utility for fetching any historical data using caching.
 Home-page: https://github.com/34j/cached-historical-data-fetcher
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

