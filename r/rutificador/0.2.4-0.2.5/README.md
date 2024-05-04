# Comparing `tmp/rutificador-0.2.4.tar.gz` & `tmp/rutificador-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.2.4.tar", max compression
+gzip compressed data, was "rutificador-0.2.5.tar", max compression
```

## Comparing `rutificador-0.2.4.tar` & `rutificador-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-03 23:06:56.408919 rutificador-0.2.4/LICENSE
--rw-r--r--   0        0        0     4357 2024-05-03 23:06:56.408919 rutificador-0.2.4/README.md
--rw-r--r--   0        0        0     1100 2024-05-03 23:06:56.408919 rutificador-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      101 2024-05-03 23:06:56.412919 rutificador-0.2.4/rutificador/__init__.py
--rw-r--r--   0        0        0     9142 2024-05-03 23:06:56.412919 rutificador-0.2.4/rutificador/main.py
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 rutificador-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-04 17:16:37.739913 rutificador-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4357 2024-05-04 17:16:37.739913 rutificador-0.2.5/README.md
+-rw-r--r--   0        0        0     1100 2024-05-04 17:16:37.739913 rutificador-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      101 2024-05-04 17:16:37.739913 rutificador-0.2.5/rutificador/__init__.py
+-rw-r--r--   0        0        0     9142 2024-05-04 17:16:37.739913 rutificador-0.2.5/rutificador/main.py
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 rutificador-0.2.5/PKG-INFO
```

### Comparing `rutificador-0.2.4/LICENSE` & `rutificador-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.4/README.md` & `rutificador-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.4/pyproject.toml` & `rutificador-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.2.4"
+version = "0.2.5"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://pypi.org/project/rutificador/"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.2.4/rutificador/main.py` & `rutificador-0.2.5/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.4/PKG-INFO` & `rutificador-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.2.4
+Version: 0.2.5
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://pypi.org/project/rutificador/
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
```

