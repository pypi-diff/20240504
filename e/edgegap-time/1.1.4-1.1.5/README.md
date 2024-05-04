# Comparing `tmp/edgegap_time-1.1.4.tar.gz` & `tmp/edgegap_time-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_time-1.1.4.tar", max compression
+gzip compressed data, was "edgegap_time-1.1.5.tar", max compression
```

## Comparing `edgegap_time-1.1.4.tar` & `edgegap_time-1.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-04 01:32:07.974506 edgegap_time-1.1.4/README.md
--rw-r--r--   0        0        0       17 2024-05-04 01:32:07.974506 edgegap_time-1.1.4/edgegap_time/BUILD
--rw-r--r--   0        0        0       63 2024-05-04 01:32:07.974506 edgegap_time-1.1.4/edgegap_time/__init__.py
--rw-r--r--   0        0        0     1329 2024-05-04 01:32:07.974506 edgegap_time-1.1.4/edgegap_time/_duration.py
--rw-r--r--   0        0        0      493 2024-05-04 01:32:26.602539 edgegap_time-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/README.md
+-rw-r--r--   0        0        0       17 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/edgegap_time/BUILD
+-rw-r--r--   0        0        0       63 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/edgegap_time/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-04 01:34:08.346442 edgegap_time-1.1.5/edgegap_time/_duration.py
+-rw-r--r--   0        0        0      493 2024-05-04 01:36:23.448222 edgegap_time-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.5/PKG-INFO
```

### Comparing `edgegap_time-1.1.4/edgegap_time/_duration.py` & `edgegap_time-1.1.5/edgegap_time/_duration.py`

 * *Files identical despite different names*

