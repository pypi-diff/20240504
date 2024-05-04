# Comparing `tmp/pyauth0-0.1.3a0.tar.gz` & `tmp/pyauth0-0.1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauth0-0.1.3a0.tar", max compression
+gzip compressed data, was "pyauth0-0.1.3a1.tar", max compression
```

## Comparing `pyauth0-0.1.3a0.tar` & `pyauth0-0.1.3a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/LICENSE
--rw-r--r--   0        0        0     2009 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/README.md
--rw-r--r--   0        0        0      147 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/__init__.py
--rw-r--r--   0        0        0      241 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/errors.py
--rw-r--r--   0        0        0     3352 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/token_provider.py
--rw-r--r--   0        0        0     5273 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyauth0/token_verifier.py
--rw-r--r--   0        0        0      533 2024-05-04 15:16:29.902042 pyauth0-0.1.3a0/pyproject.toml
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 pyauth0-0.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/LICENSE
+-rw-r--r--   0        0        0     2009 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/README.md
+-rw-r--r--   0        0        0      147 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/pyauth0/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/pyauth0/errors.py
+-rw-r--r--   0        0        0     3352 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/pyauth0/token_provider.py
+-rw-r--r--   0        0        0     5273 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/pyauth0/token_verifier.py
+-rw-r--r--   0        0        0      533 2024-05-04 15:28:27.719828 pyauth0-0.1.3a1/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 pyauth0-0.1.3a1/PKG-INFO
```

### Comparing `pyauth0-0.1.3a0/LICENSE` & `pyauth0-0.1.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.3a0/README.md` & `pyauth0-0.1.3a1/README.md`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.3a0/pyauth0/token_provider.py` & `pyauth0-0.1.3a1/pyauth0/token_provider.py`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.3a0/pyauth0/token_verifier.py` & `pyauth0-0.1.3a1/pyauth0/token_verifier.py`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.3a0/pyproject.toml` & `pyauth0-0.1.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyauth0"
-version = "0.1.3a0"
+version = "0.1.3a1"
 description = "Python utilities for Auth0"
 authors = ["svaponi <10941963+svaponi@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 python-jose = "^3.3.0"
```

### Comparing `pyauth0-0.1.3a0/PKG-INFO` & `pyauth0-0.1.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauth0
-Version: 0.1.3a0
+Version: 0.1.3a1
 Summary: Python utilities for Auth0
 Author: svaponi
 Author-email: 10941963+svaponi@users.noreply.github.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

