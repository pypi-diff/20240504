# Comparing `tmp/oandadata-0.1.2.tar.gz` & `tmp/oandadata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oandadata-0.1.2.tar", max compression
+gzip compressed data, was "oandadata-0.1.3.tar", max compression
```

## Comparing `oandadata-0.1.2.tar` & `oandadata-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1091 2024-05-03 18:46:19.286055 oandadata-0.1.2/License
--rw-r--r--   0        0        0      372 2024-05-03 20:54:14.311131 oandadata-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1115 2024-05-03 20:50:56.113962 oandadata-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-03 18:34:05.603026 oandadata-0.1.2/src/oandadata/__init__.py
--rw-r--r--   0        0        0     1959 2024-05-03 20:09:27.980450 oandadata-0.1.2/src/oandadata/retriever.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 oandadata-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-03 18:46:19.286055 oandadata-0.1.3/License
+-rw-r--r--   0        0        0      358 2024-05-04 18:53:13.661646 oandadata-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1115 2024-05-03 20:50:56.113962 oandadata-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 18:34:05.603026 oandadata-0.1.3/src/oandadata/__init__.py
+-rw-r--r--   0        0        0     1959 2024-05-03 20:09:27.980450 oandadata-0.1.3/src/oandadata/retriever.py
+-rw-r--r--   0        0        0     1932 1970-01-01 00:00:00.000000 oandadata-0.1.3/PKG-INFO
```

### Comparing `oandadata-0.1.2/License` & `oandadata-0.1.3/License`

 * *Files identical despite different names*

### Comparing `oandadata-0.1.2/README.md` & `oandadata-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oandadata-0.1.2/src/oandadata/retriever.py` & `oandadata-0.1.3/src/oandadata/retriever.py`

 * *Files identical despite different names*

### Comparing `oandadata-0.1.2/PKG-INFO` & `oandadata-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: oandadata
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for retrieving financial data.
 Author: Lumi
 Author-email: jafari.nariman@gmail.com
-Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pandas (>=1.3.3,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: pandas
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Financial Data Retrieval Library
 
 
 # oandadata
```

