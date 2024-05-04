# Comparing `tmp/flops_utils-0.2.6.tar.gz` & `tmp/flops_utils-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.2.6.tar", max compression
+gzip compressed data, was "flops_utils-0.2.7.tar", max compression
```

## Comparing `flops_utils-0.2.6.tar` & `flops_utils-0.2.7.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.6/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.2.6/flops_utils/logging.py
--rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.6/flops_utils/notifications.py
--rw-r--r--   0        0        0      414 2024-04-25 13:43:15.670487 flops_utils-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.2.7/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.2.7/flops_utils/logging.py
+-rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.2.7/flops_utils/notifications.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.2.7/flops_utils/types.py
+-rw-r--r--   0        0        0      414 2024-05-03 14:38:05.257615 flops_utils-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.2.7/PKG-INFO
```

### Comparing `flops_utils-0.2.6/flops_utils/logging.py` & `flops_utils-0.2.7/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.2.6/flops_utils/notifications.py` & `flops_utils-0.2.7/flops_utils/notifications.py`

 * *Files identical despite different names*

