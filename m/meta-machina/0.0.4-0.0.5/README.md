# Comparing `tmp/meta_machina-0.0.4.tar.gz` & `tmp/meta_machina-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_machina-0.0.4.tar", last modified: Sat May  4 15:23:50 2024, max compression
+gzip compressed data, was "meta_machina-0.0.5.tar", last modified: Sat May  4 15:43:51 2024, max compression
```

## Comparing `meta_machina-0.0.4.tar` & `meta_machina-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.4/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-04 15:04:59.000000 meta_machina-0.0.4/MANIFEST.in
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:23:50.556943 meta_machina-0.0.4/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.4/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      707 2024-05-04 15:21:44.000000 meta_machina-0.0.4/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 15:23:50.556943 meta_machina-0.0.4/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/src/meta_machina/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      930 2024-05-04 15:21:44.000000 meta_machina-0.0.4/src/meta_machina/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.4/src/meta_machina/githf.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      353 2024-05-04 14:26:01.000000 meta_machina-0.0.4/src/meta_machina/machina.yaml
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/src/meta_machina.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      289 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:43:51.517929 meta_machina-0.0.5/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.5/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-04 15:04:59.000000 meta_machina-0.0.5/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:43:51.517929 meta_machina-0.0.5/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.5/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      707 2024-05-04 15:43:28.000000 meta_machina-0.0.5/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 15:43:51.517929 meta_machina-0.0.5/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:43:51.513929 meta_machina-0.0.5/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:43:51.517929 meta_machina-0.0.5/src/meta_machina/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      937 2024-05-04 15:39:15.000000 meta_machina-0.0.5/src/meta_machina/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.5/src/meta_machina/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      353 2024-05-04 14:26:01.000000 meta_machina-0.0.5/src/meta_machina/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:43:51.517929 meta_machina-0.0.5/src/meta_machina.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:43:51.000000 meta_machina-0.0.5/src/meta_machina.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      289 2024-05-04 15:43:51.000000 meta_machina-0.0.5/src/meta_machina.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 15:43:51.000000 meta_machina-0.0.5/src/meta_machina.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 15:43:51.000000 meta_machina-0.0.5/src/meta_machina.egg-info/top_level.txt
```

### Comparing `meta_machina-0.0.4/LICENSE` & `meta_machina-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.4/PKG-INFO` & `meta_machina-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.4
+Version: 0.0.5
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `meta_machina-0.0.4/pyproject.toml` & `meta_machina-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "meta_machina"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "This machine creates machines."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `meta_machina-0.0.4/src/meta_machina/__init__.py` & `meta_machina-0.0.5/src/meta_machina/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Python
 
 """Copyright (c) Alexander Fedotov.
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
 import os
-import githf
+from . import githf
 import yaml
 import ruamel.yaml as ryaml
 
 
 MACHINE_ORGANIZATION_NAME = 'meta-machina'  # or other organization
 PRIVATE_REPO_WITH_TEXT = 'machina'
```

### Comparing `meta_machina-0.0.4/src/meta_machina/githf.py` & `meta_machina-0.0.5/src/meta_machina/githf.py`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.4/src/meta_machina.egg-info/PKG-INFO` & `meta_machina-0.0.5/src/meta_machina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.4
+Version: 0.0.5
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

