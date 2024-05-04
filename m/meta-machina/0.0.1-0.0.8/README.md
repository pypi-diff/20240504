# Comparing `tmp/meta_machina-0.0.1.tar.gz` & `tmp/meta_machina-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_machina-0.0.1.tar", last modified: Sat May  4 14:32:33 2024, max compression
+gzip compressed data, was "meta_machina-0.0.8.tar", last modified: Sat May  4 19:51:19 2024, max compression
```

## Comparing `meta_machina-0.0.1.tar` & `meta_machina-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,18 @@
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
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 19:51:19.783457 meta_machina-0.0.8/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2024-05-04 14:09:34.000000 meta_machina-0.0.8/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       31 2024-05-04 15:04:59.000000 meta_machina-0.0.8/MANIFEST.in
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      755 2024-05-04 19:51:19.779457 meta_machina-0.0.8/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      139 2024-05-04 14:26:01.000000 meta_machina-0.0.8/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      759 2024-05-04 19:50:07.000000 meta_machina-0.0.8/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2024-05-04 19:51:19.783457 meta_machina-0.0.8/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 19:51:19.779457 meta_machina-0.0.8/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 19:51:19.779457 meta_machina-0.0.8/src/meta_machina/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      920 2024-05-04 19:50:07.000000 meta_machina-0.0.8/src/meta_machina/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     2421 2024-05-04 14:09:34.000000 meta_machina-0.0.8/src/meta_machina/githf.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      353 2024-05-04 14:26:01.000000 meta_machina-0.0.8/src/meta_machina/machina.yaml
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2024-05-04 19:51:19.779457 meta_machina-0.0.8/src/meta_machina.egg-info/
+-rw-r--r--   0 alxfed    (1001) alxfed    (1001)      755 2024-05-04 19:51:19.000000 meta_machina-0.0.8/src/meta_machina.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      328 2024-05-04 19:51:19.000000 meta_machina-0.0.8/src/meta_machina.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2024-05-04 19:51:19.000000 meta_machina-0.0.8/src/meta_machina.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       30 2024-05-04 19:51:19.000000 meta_machina-0.0.8/src/meta_machina.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       13 2024-05-04 19:51:19.000000 meta_machina-0.0.8/src/meta_machina.egg-info/top_level.txt
```

### Comparing `meta_machina-0.0.1/LICENSE` & `meta_machina-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meta_machina-0.0.1/pyproject.toml` & `meta_machina-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
+[tool.setuptools.packages.find]
+where = ["src"]
 [project]
 name = "meta_machina"
-version = "0.0.1"
+version = "0.0.8"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "This machine creates machines."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
+keywords = ["meta-machina", "ai"]
+dependencies = [
+    "PyGithub >= 2.3.0",
+    "PyYAML >= 6.0.1"
+]
 [project.urls]
 "Homepage" = "https://github.com/meta-machina/meta-machina"
 "Bug Tracker" = "https://github.com/meta-machina/meta-machina/issues"
```

### Comparing `meta_machina-0.0.1/src/meta_machina/githf.py` & `meta_machina-0.0.8/src/meta_machina/githf.py`

 * *Files identical despite different names*

