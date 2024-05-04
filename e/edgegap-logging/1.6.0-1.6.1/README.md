# Comparing `tmp/edgegap_logging-1.6.0.tar.gz` & `tmp/edgegap_logging-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_logging-1.6.0.tar", max compression
+gzip compressed data, was "edgegap_logging-1.6.1.tar", max compression
```

## Comparing `edgegap_logging-1.6.0.tar` & `edgegap_logging-1.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1993 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/LICENSE
--rw-r--r--   0        0        0     2216 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/README.md
--rw-r--r--   0        0        0       17 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/edgegap_logging/BUILD
--rw-r--r--   0        0        0      217 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/edgegap_logging/__init__.py
--rw-r--r--   0        0        0      847 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/edgegap_logging/_configuration.py
--rw-r--r--   0        0        0      942 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/edgegap_logging/_format.py
--rw-r--r--   0        0        0     1299 2024-05-03 20:16:05.423940 edgegap_logging-1.6.0/edgegap_logging/_logging.py
--rw-r--r--   0        0        0      647 2024-05-03 20:17:00.052595 edgegap_logging-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 edgegap_logging-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2216 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/edgegap_logging/BUILD
+-rw-r--r--   0        0        0      217 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/edgegap_logging/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/edgegap_logging/_configuration.py
+-rw-r--r--   0        0        0      942 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/edgegap_logging/_format.py
+-rw-r--r--   0        0        0     1299 2024-05-04 01:19:22.071513 edgegap_logging-1.6.1/edgegap_logging/_logging.py
+-rw-r--r--   0        0        0      647 2024-05-04 01:20:51.567707 edgegap_logging-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 edgegap_logging-1.6.1/PKG-INFO
```

### Comparing `edgegap_logging-1.6.0/LICENSE` & `edgegap_logging-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.6.0/README.md` & `edgegap_logging-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.6.0/edgegap_logging/_configuration.py` & `edgegap_logging-1.6.1/edgegap_logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.6.0/edgegap_logging/_format.py` & `edgegap_logging-1.6.1/edgegap_logging/_format.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.6.0/edgegap_logging/_logging.py` & `edgegap_logging-1.6.1/edgegap_logging/_logging.py`

 * *Files identical despite different names*

### Comparing `edgegap_logging-1.6.0/pyproject.toml` & `edgegap_logging-1.6.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-logging"
-version = "1.6.0"
+version = "1.6.1"
 description = "The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 colorama = "^0.4.6"
```

### Comparing `edgegap_logging-1.6.0/PKG-INFO` & `edgegap_logging-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-logging
-Version: 1.6.0
+Version: 1.6.1
 Summary: The Edgegap Logging library includes various tools and helpers for interacting with Standard Logging Formatter and Colored Logs. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

