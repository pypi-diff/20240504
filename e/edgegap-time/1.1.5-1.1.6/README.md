# Comparing `tmp/edgegap_time-1.1.5.tar.gz` & `tmp/edgegap_time-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_time-1.1.5.tar", max compression
+gzip compressed data, was "edgegap_time-1.1.6.tar", max compression
```

## Comparing `edgegap_time-1.1.5.tar` & `edgegap_time-1.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/README.md
--rw-r--r--   0        0        0       17 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/edgegap_time/BUILD
--rw-r--r--   0        0        0       63 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/edgegap_time/__init__.py
--rw-r--r--   0        0        0     1329 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/edgegap_time/_duration.py
--rw-r--r--   0        0        0      493 2024-05-04 01:36:23.448222 edgegap_time-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-04 01:43:13.322644 edgegap_time-1.1.6/README.md
+-rw-r--r--   0        0        0       17 2024-05-04 01:43:13.322644 edgegap_time-1.1.6/edgegap_time/BUILD
+-rw-r--r--   0        0        0       63 2024-05-04 01:43:13.322644 edgegap_time-1.1.6/edgegap_time/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-04 01:43:13.322644 edgegap_time-1.1.6/edgegap_time/_duration.py
+-rw-r--r--   0        0        0      493 2024-05-04 01:43:34.110807 edgegap_time-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.6/PKG-INFO
```

### Comparing `edgegap_time-1.1.5/edgegap_time/_duration.py` & `edgegap_time-1.1.6/edgegap_time/_duration.py`

 * *Files identical despite different names*

