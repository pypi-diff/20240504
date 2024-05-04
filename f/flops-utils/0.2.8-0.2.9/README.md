# Comparing `tmp/flops_utils-0.2.8.tar.gz` & `tmp/flops_utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.2.8.tar", max compression
+gzip compressed data, was "flops_utils-0.2.9.tar", max compression
```

## Comparing `flops_utils-0.2.8.tar` & `flops_utils-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.8/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.2.8/flops_utils/logging.py
--rw-r--r--   0        0        0      375 2024-05-04 07:50:33.531038 flops_utils-0.2.8/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      456 2024-05-04 07:54:04.695042 flops_utils-0.2.8/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.8/flops_utils/notifications.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.2.8/flops_utils/types.py
--rw-r--r--   0        0        0      433 2024-05-04 07:54:09.455042 flops_utils-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 flops_utils-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.9/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.2.9/flops_utils/logging.py
+-rw-r--r--   0        0        0      638 2024-05-04 11:24:46.883254 flops_utils-0.2.9/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      456 2024-05-04 07:54:04.695042 flops_utils-0.2.9/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.9/flops_utils/notifications.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.2.9/flops_utils/types.py
+-rw-r--r--   0        0        0      433 2024-05-04 11:24:52.887254 flops_utils-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 flops_utils-0.2.9/PKG-INFO
```

### Comparing `flops_utils-0.2.8/flops_utils/logging.py` & `flops_utils-0.2.9/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.2.8/flops_utils/notifications.py` & `flops_utils-0.2.9/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.2.8/PKG-INFO` & `flops_utils-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flops_utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library containing commong utilities for FLOps
 Author: Alexander Malyuk
 Author-email: malyuk.alexander1999@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

