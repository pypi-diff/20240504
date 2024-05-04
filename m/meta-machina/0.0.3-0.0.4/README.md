# Comparing `tmp/meta_machina-0.0.3.tar.gz` & `tmp/meta_machina-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_machina-0.0.3.tar", last modified: Sat May  4 15:06:33 2024, max compression
+gzip compressed data, was "meta_machina-0.0.4.tar", last modified: Sat May  4 15:23:50 2024, max compression
```

## Comparing `meta_machina-0.0.3.tar` & `meta_machina-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.881598 meta_machina-0.0.3/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.3/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-04 15:04:59.000000 meta_machina-0.0.3/MANIFEST.in
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:06:33.881598 meta_machina-0.0.3/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.3/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      707 2024-05-04 15:04:59.000000 meta_machina-0.0.3/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 15:06:33.881598 meta_machina-0.0.3/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.877598 meta_machina-0.0.3/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.877598 meta_machina-0.0.3/src/meta_machina/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      847 2024-05-04 14:26:01.000000 meta_machina-0.0.3/src/meta_machina/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.3/src/meta_machina/githf.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      353 2024-05-04 14:26:01.000000 meta_machina-0.0.3/src/meta_machina/machina.yaml
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:06:33.877598 meta_machina-0.0.3/src/meta_machina.egg-info/
--rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      289 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 15:06:33.000000 meta_machina-0.0.3/src/meta_machina.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.4/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-04 15:04:59.000000 meta_machina-0.0.4/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:23:50.556943 meta_machina-0.0.4/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.4/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      707 2024-05-04 15:21:44.000000 meta_machina-0.0.4/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 15:23:50.556943 meta_machina-0.0.4/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/src/meta_machina/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      930 2024-05-04 15:21:44.000000 meta_machina-0.0.4/src/meta_machina/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.4/src/meta_machina/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      353 2024-05-04 14:26:01.000000 meta_machina-0.0.4/src/meta_machina/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 15:23:50.556943 meta_machina-0.0.4/src/meta_machina.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      669 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      289 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 15:23:50.000000 meta_machina-0.0.4/src/meta_machina.egg-info/top_level.txt
```

### Comparing `meta_machina-0.0.3/LICENSE` & `meta_machina-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.3/PKG-INFO` & `meta_machina-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.3
+Version: 0.0.4
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `meta_machina-0.0.3/pyproject.toml` & `meta_machina-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "meta_machina"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "This machine creates machines."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `meta_machina-0.0.3/src/meta_machina/__init__.py` & `meta_machina-0.0.4/src/meta_machina/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # Python
 
 """Copyright (c) Alexander Fedotov.
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
+import os
 import githf
 import yaml
 import ruamel.yaml as ryaml
 
 
 MACHINE_ORGANIZATION_NAME = 'meta-machina'  # or other organization
 PRIVATE_REPO_WITH_TEXT = 'machina'
@@ -16,14 +17,15 @@
 try:
     gh = githf.connectto_repo(organization=MACHINE_ORGANIZATION_NAME,
                               repository_name=PRIVATE_REPO_WITH_TEXT,
                               private=True)
     MACHINE_YAML = githf.read_file(repository=gh, file_path='machina.yaml')
     META_MACHINA = yaml.load(MACHINE_YAML, Loader=yaml.FullLoader)
 except Exception as e:
-    with open('machina.yaml', 'r') as f:
+    machina_path = os.path.join(os.path.dirname(__file__), 'machina.yaml')
+    with open(machina_path, 'r') as f:
         META_MACHINA= ryaml.load(f)
 
 
 if __name__ == '__main__':
     print('You have launched main')
```

### Comparing `meta_machina-0.0.3/src/meta_machina/githf.py` & `meta_machina-0.0.4/src/meta_machina/githf.py`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.3/src/meta_machina.egg-info/PKG-INFO` & `meta_machina-0.0.4/src/meta_machina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_machina
-Version: 0.0.3
+Version: 0.0.4
 Summary: This machine creates machines.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/meta-machina/meta-machina
 Project-URL: Bug Tracker, https://github.com/meta-machina/meta-machina/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

