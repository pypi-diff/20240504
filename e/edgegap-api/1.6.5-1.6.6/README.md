# Comparing `tmp/edgegap_api-1.6.5.tar.gz` & `tmp/edgegap_api-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_api-1.6.5.tar", max compression
+gzip compressed data, was "edgegap_api-1.6.6.tar", max compression
```

## Comparing `edgegap_api-1.6.5.tar` & `edgegap_api-1.6.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1993 2024-05-04 01:32:07.966506 edgegap_api-1.6.5/LICENSE
--rw-r--r--   0        0        0     2171 2024-05-04 01:32:07.966506 edgegap_api-1.6.5/README.md
--rw-r--r--   0        0        0       17 2024-05-04 01:32:07.966506 edgegap_api-1.6.5/edgegap_api/BUILD
--rw-r--r--   0        0        0      132 2024-05-04 01:32:07.966506 edgegap_api-1.6.5/edgegap_api/__init__.py
--rw-r--r--   0        0        0      648 2024-05-04 01:32:07.966506 edgegap_api-1.6.5/edgegap_api/_configuration.py
--rw-r--r--   0        0        0     3990 2024-05-04 01:32:07.966506 edgegap_api-1.6.5/edgegap_api/_helper.py
--rw-r--r--   0        0        0      763 2024-05-04 01:33:06.066610 edgegap_api-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 edgegap_api-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-04 01:43:13.310644 edgegap_api-1.6.6/LICENSE
+-rw-r--r--   0        0        0     2171 2024-05-04 01:43:13.310644 edgegap_api-1.6.6/README.md
+-rw-r--r--   0        0        0       17 2024-05-04 01:43:13.310644 edgegap_api-1.6.6/edgegap_api/BUILD
+-rw-r--r--   0        0        0      132 2024-05-04 01:43:13.310644 edgegap_api-1.6.6/edgegap_api/__init__.py
+-rw-r--r--   0        0        0      648 2024-05-04 01:43:13.310644 edgegap_api-1.6.6/edgegap_api/_configuration.py
+-rw-r--r--   0        0        0     3990 2024-05-04 01:43:13.310644 edgegap_api-1.6.6/edgegap_api/_helper.py
+-rw-r--r--   0        0        0      763 2024-05-04 01:45:25.199655 edgegap_api-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 edgegap_api-1.6.6/PKG-INFO
```

### Comparing `edgegap_api-1.6.5/LICENSE` & `edgegap_api-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.6.5/README.md` & `edgegap_api-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.6.5/edgegap_api/_configuration.py` & `edgegap_api-1.6.6/edgegap_api/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.6.5/edgegap_api/_helper.py` & `edgegap_api-1.6.6/edgegap_api/_helper.py`

 * *Files identical despite different names*

### Comparing `edgegap_api-1.6.5/pyproject.toml` & `edgegap_api-1.6.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-api"
-version = "1.6.5"
+version = "1.6.6"
 description = "The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_api-1.6.5/PKG-INFO` & `edgegap_api-1.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-api
-Version: 1.6.5
+Version: 1.6.6
 Summary: The Edgegap API library includes various tools and helpers for interacting with RESTful and other types of APIs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

