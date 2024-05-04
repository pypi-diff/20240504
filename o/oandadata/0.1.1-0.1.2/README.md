# Comparing `tmp/oandadata-0.1.1.tar.gz` & `tmp/oandadata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oandadata-0.1.1.tar", max compression
+gzip compressed data, was "oandadata-0.1.2.tar", max compression
```

## Comparing `oandadata-0.1.1.tar` & `oandadata-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1091 2024-05-03 18:46:19.286055 oandadata-0.1.1/License
--rw-r--r--   0        0        0      349 2024-05-03 20:13:37.553469 oandadata-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 18:34:05.603026 oandadata-0.1.1/src/oandadata/__init__.py
--rw-r--r--   0        0        0     1959 2024-05-03 20:09:27.980450 oandadata-0.1.1/src/oandadata/retriever.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 oandadata-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-03 18:46:19.286055 oandadata-0.1.2/License
+-rw-r--r--   0        0        0      372 2024-05-03 20:54:14.311131 oandadata-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1115 2024-05-03 20:50:56.113962 oandadata-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 18:34:05.603026 oandadata-0.1.2/src/oandadata/__init__.py
+-rw-r--r--   0        0        0     1959 2024-05-03 20:09:27.980450 oandadata-0.1.2/src/oandadata/retriever.py
+-rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 oandadata-0.1.2/PKG-INFO
```

### Comparing `oandadata-0.1.1/License` & `oandadata-0.1.2/License`

 * *Files identical despite different names*

### Comparing `oandadata-0.1.1/src/oandadata/retriever.py` & `oandadata-0.1.2/src/oandadata/retriever.py`

 * *Files identical despite different names*

