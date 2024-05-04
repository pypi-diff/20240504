# Comparing `tmp/pyauth0-0.1.2.tar.gz` & `tmp/pyauth0-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauth0-0.1.2.tar", last modified: Sat May  4 14:17:59 2024, max compression
+gzip compressed data, was "pyauth0-0.1.3a0.tar", max compression
```

## Comparing `pyauth0-0.1.2.tar` & `pyauth0-0.1.3a0.tar`

### file list

```diff
@@ -1,24 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-04 14:17:54.000000 pyauth0-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 14:17:54.000000 pyauth0-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-04 14:17:59.029268 pyauth0-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-04 14:17:54.000000 pyauth0-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/pyauth0/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/token_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/pyauth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 14:17:54.000000 pyauth0-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:17:59.033268 pyauth0-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-04 14:17:54.000000 pyauth0-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 14:17:54.000000 pyauth0-0.1.2/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-04 14:17:54.000000 pyauth0-0.1.2/test/test_pyauth0.py
+-rw-r--r--   0        0        0     1070 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/LICENSE
+-rw-r--r--   0        0        0     2009 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/README.md
+-rw-r--r--   0        0        0      147 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/errors.py
+-rw-r--r--   0        0        0     3352 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/token_provider.py
+-rw-r--r--   0        0        0     5273 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/token_verifier.py
+-rw-r--r--   0        0        0      533 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 pyauth0-0.1.3a0/PKG-INFO
```

### Comparing `pyauth0-0.1.2/LICENSE` & `pyauth0-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.2/PKG-INFO` & `pyauth0-0.1.3a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: pyauth0
-Version: 0.1.2
+Version: 0.1.3a0
 Summary: Python utilities for Auth0
-Home-page: https://github.com/svaponi/pyauth0
 Author: svaponi
-Author-email: svaponi@proton.me
-Classifier: Development Status :: 4 - Beta
+Author-email: 10941963+svaponi@users.noreply.github.com
+Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-jose>=3.3.0
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: python-dotenv; extra == "test"
 
 # pyauth0
 
 [![Test](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml/badge.svg)](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/svaponi/pyauth0/badge.svg?branch=main)](https://coveralls.io/github/svaponi/pyauth0?branch=main)
 [![PyPI version](https://badge.fury.io/py/pyauth0.svg)](https://badge.fury.io/py/pyauth0)
 
@@ -81,7 +78,8 @@
 
 claim_value = decoded_token.payload.get("http://your-domain.com/claim_name", "default value")
 ```
 
 ## Contribute
 
 If you want to contribute, open a [GitHub Issue](https://github.com/svaponi/pyauth0/issues) and motivate your request.
+
```

### Comparing `pyauth0-0.1.2/README.md` & `pyauth0-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.2/pyauth0/token_provider.py` & `pyauth0-0.1.3a0/pyauth0/token_provider.py`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.2/pyauth0/token_verifier.py` & `pyauth0-0.1.3a0/pyauth0/token_verifier.py`

 * *Files identical despite different names*

