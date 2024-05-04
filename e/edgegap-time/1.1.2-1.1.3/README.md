# Comparing `tmp/edgegap_time-1.1.2.tar.gz` & `tmp/edgegap_time-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_time-1.1.2.tar", max compression
+gzip compressed data, was "edgegap_time-1.1.3.tar", max compression
```

## Comparing `edgegap_time-1.1.2.tar` & `edgegap_time-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-04 01:23:24.193026 edgegap_time-1.1.2/README.md
--rw-r--r--   0        0        0       17 2024-05-04 01:23:24.193026 edgegap_time-1.1.2/edgegap_time/BUILD
--rw-r--r--   0        0        0       63 2024-05-04 01:23:24.193026 edgegap_time-1.1.2/edgegap_time/__init__.py
--rw-r--r--   0        0        0     1329 2024-05-04 01:23:24.193026 edgegap_time-1.1.2/edgegap_time/_duration.py
--rw-r--r--   0        0        0      399 2024-05-04 01:25:04.473499 edgegap_time-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-04 01:27:09.434461 edgegap_time-1.1.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-04 01:27:09.434461 edgegap_time-1.1.3/edgegap_time/BUILD
+-rw-r--r--   0        0        0       63 2024-05-04 01:27:09.434461 edgegap_time-1.1.3/edgegap_time/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-04 01:27:09.434461 edgegap_time-1.1.3/edgegap_time/_duration.py
+-rw-r--r--   0        0        0      493 2024-05-04 01:27:27.486507 edgegap_time-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 edgegap_time-1.1.3/PKG-INFO
```

### Comparing `edgegap_time-1.1.2/edgegap_time/_duration.py` & `edgegap_time-1.1.3/edgegap_time/_duration.py`

 * *Files identical despite different names*

