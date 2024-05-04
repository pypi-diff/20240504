# Comparing `tmp/meta_machina-0.0.2.tar.gz` & `tmp/meta_machina-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_machina-0.0.2.tar", last modified: Sat May  4 14:50:22 2024, max compression
+gzip compressed data, was "meta_machina-0.0.3.tar", last modified: Sat May  4 15:06:33 2024, max compression
```

## Comparing `meta_machina-0.0.2.tar` & `meta_machina-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.923507 meta_machina-0.0.2/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.2/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       14 2024-05-04 14:49:37.000000 meta_machina-0.0.2/MANIFEST.in
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 14:50:22.923507 meta_machina-0.0.2/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.2/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      611 2024-05-04 14:49:37.000000 meta_machina-0.0.2/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 14:50:22.923507 meta_machina-0.0.2/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.919507 meta_machina-0.0.2/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.923507 meta_machina-0.0.2/src/meta_machina/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-05-04 14:26:01.000000 meta_machina-0.0.2/src/meta_machina/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.2/src/meta_machina/githf.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.923507 meta_machina-0.0.2/src/meta_machina.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      259 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.881598 meta_machina-0.0.3/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.3/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-04 15:04:59.000000 meta_machina-0.0.3/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:06:33.881598 meta_machina-0.0.3/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.3/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      707 2024-05-04 15:04:59.000000 meta_machina-0.0.3/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 15:06:33.881598 meta_machina-0.0.3/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.877598 meta_machina-0.0.3/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.877598 meta_machina-0.0.3/src/meta_machina/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-05-04 14:26:01.000000 meta_machina-0.0.3/src/meta_machina/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.3/src/meta_machina/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      353 2024-05-04 14:26:01.000000 meta_machina-0.0.3/src/meta_machina/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.877598 meta_machina-0.0.3/src/meta_machina.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      289 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/top_level.txt
```

### Comparing `meta_machina-0.0.2/LICENSE` & `meta_machina-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.2/PKG-INFO` & `meta_machina-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.2
+Version: 0.0.3
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `meta_machina-0.0.2/src/meta_machina/__init__.py` & `meta_machina-0.0.3/src/meta_machina/__init__.py`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.2/src/meta_machina/githf.py` & `meta_machina-0.0.3/src/meta_machina/githf.py`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.2/src/meta_machina.egg-info/PKG-INFO` & `meta_machina-0.0.3/src/meta_machina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.2
+Version: 0.0.3
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

