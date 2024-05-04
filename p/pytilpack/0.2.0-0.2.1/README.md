# Comparing `tmp/pytilpack-0.2.0.tar.gz` & `tmp/pytilpack-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytilpack-0.2.0.tar", max compression
+gzip compressed data, was "pytilpack-0.2.1.tar", max compression
```

## Comparing `pytilpack-0.2.0.tar` & `pytilpack-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2024-05-04 05:29:49.411308 pytilpack-0.2.0/LICENSE
--rw-r--r--   0        0        0      503 2024-05-04 05:29:49.411308 pytilpack-0.2.0/README.md
--rw-r--r--   0        0        0     2154 2024-05-04 05:30:07.367542 pytilpack-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-04 05:29:49.411308 pytilpack-0.2.0/pytilpack/__init__.py
--rw-r--r--   0        0        0     1920 2024-05-04 05:29:49.411308 pytilpack-0.2.0/pytilpack/flask_.py
--rw-r--r--   0        0        0     4444 2024-05-04 05:29:49.411308 pytilpack-0.2.0/pytilpack/openai_.py
--rw-r--r--   0        0        0      690 2024-05-04 05:29:49.411308 pytilpack-0.2.0/pytilpack/python_.py
--rw-r--r--   0        0        0     2365 2024-05-04 05:29:49.411308 pytilpack-0.2.0/pytilpack/sqlalchemy_.py
--rw-r--r--   0        0        0      523 2024-05-04 05:29:49.411308 pytilpack-0.2.0/pytilpack/tqdm_.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 pytilpack-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-04 09:28:47.171854 pytilpack-0.2.1/LICENSE
+-rw-r--r--   0        0        0      503 2024-05-04 09:28:47.171854 pytilpack-0.2.1/README.md
+-rw-r--r--   0        0        0     2182 2024-05-04 09:28:58.599933 pytilpack-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 09:28:47.171854 pytilpack-0.2.1/pytilpack/__init__.py
+-rw-r--r--   0        0        0     1920 2024-05-04 09:28:47.171854 pytilpack-0.2.1/pytilpack/flask_.py
+-rw-r--r--   0        0        0     4444 2024-05-04 09:28:47.171854 pytilpack-0.2.1/pytilpack/openai_.py
+-rw-r--r--   0        0        0      690 2024-05-04 09:28:47.171854 pytilpack-0.2.1/pytilpack/python_.py
+-rw-r--r--   0        0        0     2370 2024-05-04 09:28:47.171854 pytilpack-0.2.1/pytilpack/sqlalchemy_.py
+-rw-r--r--   0        0        0      523 2024-05-04 09:28:47.171854 pytilpack-0.2.1/pytilpack/tqdm_.py
+-rw-r--r--   0        0        0     1621 1970-01-01 00:00:00.000000 pytilpack-0.2.1/PKG-INFO
```

### Comparing `pytilpack-0.2.0/LICENSE` & `pytilpack-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.0/pyproject.toml` & `pytilpack-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytilpack"
-version = "0.2.0"  # using poetry-dynamic-versioning
+version = "0.2.1"  # using poetry-dynamic-versioning
 description = "Python Utility Pack"
 license = "MIT"
 authors = ["aki. <mark@aur.ll.to>"]
 readme = "README.md"
 homepage = "https://github.com/ak110/pytilpack"
 classifiers = [
     "Environment :: Console",
@@ -19,14 +19,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 flask = {version = ">=2.2", optional = true}
 openai = {version = ">=1.25", optional = true}
 sqlalchemy = {version = ">=2.0", optional = true}
 tqdm = {version = ">=4.66", optional = true}
+typing-extensions = ">=4.0"
 
 [tool.poetry.group.dev.dependencies]
 pyfltr = "*"
 
 [tool.poetry.extras]
 all = [
     "flask",
```

### Comparing `pytilpack-0.2.0/pytilpack/flask_.py` & `pytilpack-0.2.1/pytilpack/flask_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.0/pytilpack/openai_.py` & `pytilpack-0.2.1/pytilpack/openai_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.0/pytilpack/python_.py` & `pytilpack-0.2.1/pytilpack/python_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.0/pytilpack/sqlalchemy_.py` & `pytilpack-0.2.1/pytilpack/sqlalchemy_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """SQLAlchemy用のユーティリティ集。"""
 
 import logging
 import time
-import typing
 
 import sqlalchemy
 
 try:
-    from typing import Self
+    from typing import Self  # type: ignore[attr-defined]
 except ImportError:
-    Self = typing.TypeVar("Self")  # type: ignore
+    from typing_extensions import Self
 
 logger = logging.getLogger(__name__)
 
 
 def register_ping():
     """コネクションプールの切断対策。"""
```

### Comparing `pytilpack-0.2.0/pytilpack/tqdm_.py` & `pytilpack-0.2.1/pytilpack/tqdm_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.2.0/PKG-INFO` & `pytilpack-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytilpack
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Utility Pack
 Home-page: https://github.com/ak110/pytilpack
 License: MIT
 Author: aki.
 Author-email: mark@aur.ll.to
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Provides-Extra: openai
 Provides-Extra: sqlalchemy
 Provides-Extra: tqdm
 Requires-Dist: flask (>=2.2) ; extra == "all" or extra == "flask"
 Requires-Dist: openai (>=1.25) ; extra == "all" or extra == "openai"
 Requires-Dist: sqlalchemy (>=2.0) ; extra == "all" or extra == "sqlalchemy"
 Requires-Dist: tqdm (>=4.66) ; extra == "all" or extra == "tqdm"
+Requires-Dist: typing-extensions (>=4.0)
 Description-Content-Type: text/markdown
 
 # pytilpack
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Lint&Test](https://github.com/ak110/pytilpack/actions/workflows/python-app.yml/badge.svg)](https://github.com/ak110/pytilpack/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/pytilpack.svg)](https://badge.fury.io/py/pytilpack)
```

