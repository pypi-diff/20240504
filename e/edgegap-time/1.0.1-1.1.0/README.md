# Comparing `tmp/edgegap_time-1.0.1.tar.gz` & `tmp/edgegap_time-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_time-1.0.1.tar", max compression
+gzip compressed data, was "edgegap_time-1.1.0.tar", max compression
```

## Comparing `edgegap_time-1.0.1.tar` & `edgegap_time-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-03 19:55:51.591548 edgegap_time-1.0.1/README.md
--rw-r--r--   0        0        0       17 2024-05-03 19:55:51.591548 edgegap_time-1.0.1/edgegap_time/BUILD
--rw-r--r--   0        0        0       63 2024-05-03 19:55:51.591548 edgegap_time-1.0.1/edgegap_time/__init__.py
--rw-r--r--   0        0        0     1329 2024-05-03 19:55:51.591548 edgegap_time-1.0.1/edgegap_time/_duration.py
--rw-r--r--   0        0        0      399 2024-05-03 19:56:46.447285 edgegap_time-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 20:16:05.431940 edgegap_time-1.1.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 20:16:05.431940 edgegap_time-1.1.0/edgegap_time/BUILD
+-rw-r--r--   0        0        0       63 2024-05-03 20:16:05.431940 edgegap_time-1.1.0/edgegap_time/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-03 20:16:05.431940 edgegap_time-1.1.0/edgegap_time/_duration.py
+-rw-r--r--   0        0        0      399 2024-05-03 20:16:55.268535 edgegap_time-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.0/PKG-INFO
```

### Comparing `edgegap_time-1.0.1/edgegap_time/_duration.py` & `edgegap_time-1.1.0/edgegap_time/_duration.py`

 * *Files identical despite different names*

