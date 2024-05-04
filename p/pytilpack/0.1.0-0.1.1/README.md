# Comparing `tmp/pytilpack-0.1.0.tar.gz` & `tmp/pytilpack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytilpack-0.1.0.tar", max compression
+gzip compressed data, was "pytilpack-0.1.1.tar", max compression
```

## Comparing `pytilpack-0.1.0.tar` & `pytilpack-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-05-04 04:59:16.190245 pytilpack-0.1.0/LICENSE
--rw-r--r--   0        0        0      503 2024-05-04 04:59:16.190245 pytilpack-0.1.0/README.md
--rw-r--r--   0        0        0     2154 2024-05-04 04:59:27.734246 pytilpack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-04 04:59:16.190245 pytilpack-0.1.0/pytilpack/__init__.py
--rw-r--r--   0        0        0     1920 2024-05-04 04:59:16.190245 pytilpack-0.1.0/pytilpack/flask_.py
--rw-r--r--   0        0        0     4444 2024-05-04 04:59:16.190245 pytilpack-0.1.0/pytilpack/openai_.py
--rw-r--r--   0        0        0      690 2024-05-04 04:59:16.190245 pytilpack-0.1.0/pytilpack/python_.py
--rw-r--r--   0        0        0     2289 2024-05-04 04:59:16.190245 pytilpack-0.1.0/pytilpack/sqlalchemy_.py
--rw-r--r--   0        0        0      523 2024-05-04 04:59:16.190245 pytilpack-0.1.0/pytilpack/tqdm_.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 pytilpack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-04 05:15:51.426133 pytilpack-0.1.1/LICENSE
+-rw-r--r--   0        0        0      503 2024-05-04 05:15:51.426133 pytilpack-0.1.1/README.md
+-rw-r--r--   0        0        0     2187 2024-05-04 05:16:02.946123 pytilpack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 05:15:51.426133 pytilpack-0.1.1/pytilpack/__init__.py
+-rw-r--r--   0        0        0     1920 2024-05-04 05:15:51.426133 pytilpack-0.1.1/pytilpack/flask_.py
+-rw-r--r--   0        0        0     4444 2024-05-04 05:15:51.426133 pytilpack-0.1.1/pytilpack/openai_.py
+-rw-r--r--   0        0        0      690 2024-05-04 05:15:51.426133 pytilpack-0.1.1/pytilpack/python_.py
+-rw-r--r--   0        0        0     2289 2024-05-04 05:15:51.426133 pytilpack-0.1.1/pytilpack/sqlalchemy_.py
+-rw-r--r--   0        0        0      523 2024-05-04 05:15:51.426133 pytilpack-0.1.1/pytilpack/tqdm_.py
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 pytilpack-0.1.1/PKG-INFO
```

### Comparing `pytilpack-0.1.0/LICENSE` & `pytilpack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytilpack-0.1.0/pyproject.toml` & `pytilpack-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytilpack"
-version = "0.1.0"  # using poetry-dynamic-versioning
+version = "0.1.1"  # using poetry-dynamic-versioning
 description = "Python Utility Pack"
 license = "MIT"
 authors = ["aki. <mark@aur.ll.to>"]
 readme = "README.md"
 homepage = "https://github.com/ak110/pytilpack"
 classifiers = [
     "Environment :: Console",
@@ -14,15 +14,15 @@
 ]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
-python = ">=3.11,<4.0"
+python = ">=3.11.0rc1,<4.0"  # 3.11.0rc1はubuntu対策
 flask = {version = ">=2.2", optional = true}
 openai = {version = ">=1.25", optional = true}
 sqlalchemy = {version = ">=2.0", optional = true}
 tqdm = {version = ">=4.66", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pyfltr = "*"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytilpack-0.1.0/pytilpack/flask_.py` & `pytilpack-0.1.1/pytilpack/flask_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.1.0/pytilpack/openai_.py` & `pytilpack-0.1.1/pytilpack/openai_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.1.0/pytilpack/python_.py` & `pytilpack-0.1.1/pytilpack/python_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.1.0/pytilpack/sqlalchemy_.py` & `pytilpack-0.1.1/pytilpack/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.1.0/pytilpack/tqdm_.py` & `pytilpack-0.1.1/pytilpack/tqdm_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.1.0/PKG-INFO` & `pytilpack-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytilpack
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Utility Pack
 Home-page: https://github.com/ak110/pytilpack
 License: MIT
 Author: aki.
 Author-email: mark@aur.ll.to
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11.0rc1,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

