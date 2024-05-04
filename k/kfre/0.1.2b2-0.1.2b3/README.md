# Comparing `tmp/kfre-0.1.2b2.tar.gz` & `tmp/kfre-0.1.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.2b2.tar", last modified: Sat May  4 06:47:22 2024, max compression
+gzip compressed data, was "kfre-0.1.2b3.tar", last modified: Sat May  4 07:35:38 2024, max compression
```

## Comparing `kfre-0.1.2b2.tar` & `kfre-0.1.2b3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:22.299038 kfre-0.1.2b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 06:47:14.000000 kfre-0.1.2b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-05-04 06:47:22.299038 kfre-0.1.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-04 06:47:14.000000 kfre-0.1.2b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:47:22.299038 kfre-0.1.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-04 06:47:14.000000 kfre-0.1.2b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:22.295038 kfre-0.1.2b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:22.295038 kfre-0.1.2b2/src/kfre/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 06:47:14.000000 kfre-0.1.2b2/src/kfre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 06:47:14.000000 kfre-0.1.2b2/src/kfre/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:22.295038 kfre-0.1.2b2/src/kfre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-05-04 06:47:22.000000 kfre-0.1.2b2/src/kfre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 06:47:22.000000 kfre-0.1.2b2/src/kfre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:47:22.000000 kfre-0.1.2b2/src/kfre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 06:47:22.000000 kfre-0.1.2b2/src/kfre.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 06:47:22.000000 kfre-0.1.2b2/src/kfre.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.012339 kfre-0.1.2b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 07:35:25.000000 kfre-0.1.2b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-04 07:35:38.012339 kfre-0.1.2b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-04 07:35:25.000000 kfre-0.1.2b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:35:38.012339 kfre-0.1.2b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-04 07:35:25.000000 kfre-0.1.2b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.008339 kfre-0.1.2b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.012339 kfre-0.1.2b3/src/kfre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 07:35:25.000000 kfre-0.1.2b3/src/kfre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 07:35:25.000000 kfre-0.1.2b3/src/kfre/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.012339 kfre-0.1.2b3/src/kfre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.2b2/LICENSE.md` & `kfre-0.1.2b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b2/README.md` & `kfre-0.1.2b3/README.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b2/setup.py` & `kfre-0.1.2b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.2_b2",
+    version="0.1.2_b3",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     # long_description=open("README.md").read(),
     long_description=open("min_readme.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     package_dir={"": "src"},  # Directory where your package files are located
```

### Comparing `kfre-0.1.2b2/src/kfre/__init__.py` & `kfre-0.1.2b3/src/kfre/__init__.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b2/src/kfre/main.py` & `kfre-0.1.2b3/src/kfre/main.py`

 * *Files identical despite different names*

