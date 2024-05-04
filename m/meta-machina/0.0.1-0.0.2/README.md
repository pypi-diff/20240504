# Comparing `tmp/meta_machina-0.0.1.tar.gz` & `tmp/meta_machina-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_machina-0.0.1.tar", last modified: Sat May  4 14:32:33 2024, max compression
+gzip compressed data, was "meta_machina-0.0.2.tar", last modified: Sat May  4 14:50:22 2024, max compression
```

## Comparing `meta_machina-0.0.1.tar` & `meta_machina-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:32:33.163290 meta_machina-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.1/LICENSE
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 14:32:33.163290 meta_machina-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      611 2024-05-04 14:26:01.000000 meta_machina-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 14:32:33.163290 meta_machina-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:32:33.163290 meta_machina-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:32:33.163290 meta_machina-0.0.1/src/meta_machina/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-05-04 14:26:01.000000 meta_machina-0.0.1/src/meta_machina/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.1/src/meta_machina/githf.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:32:33.163290 meta_machina-0.0.1/src/meta_machina.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 14:32:33.000000 meta_machina-0.0.1/src/meta_machina.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      247 2024-05-04 14:32:33.000000 meta_machina-0.0.1/src/meta_machina.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 14:32:33.000000 meta_machina-0.0.1/src/meta_machina.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 14:32:33.000000 meta_machina-0.0.1/src/meta_machina.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.923507 meta_machina-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.2/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       14 2024-05-04 14:49:37.000000 meta_machina-0.0.2/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 14:50:22.923507 meta_machina-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      611 2024-05-04 14:49:37.000000 meta_machina-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 14:50:22.923507 meta_machina-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.919507 meta_machina-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.923507 meta_machina-0.0.2/src/meta_machina/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-05-04 14:26:01.000000 meta_machina-0.0.2/src/meta_machina/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.2/src/meta_machina/githf.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 14:50:22.923507 meta_machina-0.0.2/src/meta_machina.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      259 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 14:50:22.000000 meta_machina-0.0.2/src/meta_machina.egg-info/top_level.txt
```

### Comparing `meta_machina-0.0.1/LICENSE` & `meta_machina-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.1/PKG-INFO` & `meta_machina-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.1
+Version: 0.0.2
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `meta_machina-0.0.1/pyproject.toml` & `meta_machina-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "meta_machina"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "This machine creates machines."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `meta_machina-0.0.1/src/meta_machina/__init__.py` & `meta_machina-0.0.2/src/meta_machina/__init__.py`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.1/src/meta_machina/githf.py` & `meta_machina-0.0.2/src/meta_machina/githf.py`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.1/src/meta_machina.egg-info/PKG-INFO` & `meta_machina-0.0.2/src/meta_machina.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.1
+Version: 0.0.2
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

