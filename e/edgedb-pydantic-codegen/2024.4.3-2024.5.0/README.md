# Comparing `tmp/edgedb_pydantic_codegen-2024.4.3.tar.gz` & `tmp/edgedb_pydantic_codegen-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgedb_pydantic_codegen-2024.4.3.tar", max compression
+gzip compressed data, was "edgedb_pydantic_codegen-2024.5.0.tar", max compression
```

## Comparing `edgedb_pydantic_codegen-2024.4.3.tar` & `edgedb_pydantic_codegen-2024.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/LICENSE
--rw-r--r--   0        0        0     2946 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/README.md
--rw-r--r--   0        0        0       88 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/__init__.py
--rw-r--r--   0        0        0      621 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/__main__.py
--rw-r--r--   0        0        0    10297 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/generator.py
--rw-r--r--   0        0        0     2013 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/models.py
--rw-r--r--   0        0        0     2057 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/template.py.jinja
--rw-r--r--   0        0        0     1290 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/utils.py
--rw-r--r--   0        0        0      817 2024-04-26 23:38:00.078381 edgedb_pydantic_codegen-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 edgedb_pydantic_codegen-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     2946 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/README.md
+-rw-r--r--   0        0        0       88 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/__init__.py
+-rw-r--r--   0        0        0      621 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/__main__.py
+-rw-r--r--   0        0        0    10297 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/generator.py
+-rw-r--r--   0        0        0     2013 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/models.py
+-rw-r--r--   0        0        0     2057 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/template.py.jinja
+-rw-r--r--   0        0        0     1290 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/utils.py
+-rw-r--r--   0        0        0      817 2024-05-03 23:38:32.060026 edgedb_pydantic_codegen-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 edgedb_pydantic_codegen-2024.5.0/PKG-INFO
```

### Comparing `edgedb_pydantic_codegen-2024.4.3/LICENSE` & `edgedb_pydantic_codegen-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/README.md` & `edgedb_pydantic_codegen-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/__main__.py` & `edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/generator.py` & `edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/generator.py`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/models.py` & `edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/models.py`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/template.py.jinja` & `edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/template.py.jinja`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/edgedb_pydantic_codegen/utils.py` & `edgedb_pydantic_codegen-2024.5.0/edgedb_pydantic_codegen/utils.py`

 * *Files identical despite different names*

### Comparing `edgedb_pydantic_codegen-2024.4.3/pyproject.toml` & `edgedb_pydantic_codegen-2024.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgedb-pydantic-codegen"
-version = "2024.04.3"
+version = "2024.05.0"
 description = "Alternative Python EdgeDB code generator (Pydantic V2 + asyncio, FastAPI compatible)"
 authors = ["NextFire <git@yuru.moe>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Japan7/edgedb-pydantic-codegen"
 
 [tool.poetry.scripts]
@@ -17,15 +17,15 @@
 jinja2 = "^3.0.0"
 ruff = ">=0.1.2,<1"
 # runtime
 pydantic = "^2.0.0"
 orjson = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pyright = "1.1.360"
+pyright = "1.1.361"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 pythonVersion = "3.11"
```

### Comparing `edgedb_pydantic_codegen-2024.4.3/PKG-INFO` & `edgedb_pydantic_codegen-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgedb-pydantic-codegen
-Version: 2024.4.3
+Version: 2024.5.0
 Summary: Alternative Python EdgeDB code generator (Pydantic V2 + asyncio, FastAPI compatible)
 Home-page: https://github.com/Japan7/edgedb-pydantic-codegen
 License: MIT
 Author: NextFire
 Author-email: git@yuru.moe
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

