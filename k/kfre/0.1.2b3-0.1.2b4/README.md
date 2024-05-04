# Comparing `tmp/kfre-0.1.2b3.tar.gz` & `tmp/kfre-0.1.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.2b3.tar", last modified: Sat May  4 07:35:38 2024, max compression
+gzip compressed data, was "kfre-0.1.2b4.tar", last modified: Sat May  4 15:13:09 2024, max compression
```

## Comparing `kfre-0.1.2b3.tar` & `kfre-0.1.2b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.012339 kfre-0.1.2b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 07:35:25.000000 kfre-0.1.2b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-04 07:35:38.012339 kfre-0.1.2b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-04 07:35:25.000000 kfre-0.1.2b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:35:38.012339 kfre-0.1.2b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-04 07:35:25.000000 kfre-0.1.2b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.008339 kfre-0.1.2b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.012339 kfre-0.1.2b3/src/kfre/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 07:35:25.000000 kfre-0.1.2b3/src/kfre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 07:35:25.000000 kfre-0.1.2b3/src/kfre/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:35:38.012339 kfre-0.1.2b3/src/kfre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 07:35:37.000000 kfre-0.1.2b3/src/kfre.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:13:09.995215 kfre-0.1.2b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 15:12:59.000000 kfre-0.1.2b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-04 15:13:09.995215 kfre-0.1.2b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-04 15:12:59.000000 kfre-0.1.2b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 15:13:09.995215 kfre-0.1.2b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-04 15:12:59.000000 kfre-0.1.2b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:13:09.995215 kfre-0.1.2b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:13:09.995215 kfre-0.1.2b4/src/kfre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 15:12:59.000000 kfre-0.1.2b4/src/kfre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 15:12:59.000000 kfre-0.1.2b4/src/kfre/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:13:09.995215 kfre-0.1.2b4/src/kfre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-04 15:13:09.000000 kfre-0.1.2b4/src/kfre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 15:13:09.000000 kfre-0.1.2b4/src/kfre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:13:09.000000 kfre-0.1.2b4/src/kfre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 15:13:09.000000 kfre-0.1.2b4/src/kfre.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 15:13:09.000000 kfre-0.1.2b4/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.2b3/LICENSE.md` & `kfre-0.1.2b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b3/PKG-INFO` & `kfre-0.1.2b4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.2b3
+Version: 0.1.2b4
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Project-URL: Author Website, https://www.leonshpaner.com
 Project-URL: Documentation, https://lshpaner.github.io/kfre_docs/
 Project-URL: DOI, https://zenodo.org/records/11100222
 Project-URL: Source Code, https://github.com/lshpaner/kfre
@@ -20,17 +20,15 @@
 # KFRE: Kidney Failure Risk Estimator
 
 [![PyPI](https://img.shields.io/pypi/v/kfre.svg)](https://pypi.org/project/kfre/)
 [![Downloads](https://pepy.tech/badge/kfre)](https://pepy.tech/project/kfre)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/lshpaner/kfre/tree/main?tab=License-1-ov-file)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.11100222.svg)](https://doi.org/10.5281/zenodo.11100222)
 
-<div style="pointer-events: none;">
-    <img src="https://raw.githubusercontent.com/lshpaner/lshpaner.github.io/main/docs/kfre_docs/_static/kfre_logo.svg?token=GHSAT0AAAAAACQTRN6VMOSVD5HGPUNSZQUQZRV6EQQ" width="200" style="border: none; outline: none; box-shadow: none;" draggable="false" oncontextmenu="return false;">
-</div>
+<img src="https://raw.githubusercontent.com/lshpaner/kfre/main/assets/kfre_logo.svg" width="200" style="border: none; outline: none; box-shadow: none;" oncontextmenu="return false;">
 
 
 `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
 
 ## Prerequisites
 Before you install `kfre`, ensure you have the following:
```

### Comparing `kfre-0.1.2b3/README.md` & `kfre-0.1.2b4/README.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b3/setup.py` & `kfre-0.1.2b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.2_b3",
+    version="0.1.2_b4",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     # long_description=open("README.md").read(),
     long_description=open("min_readme.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     package_dir={"": "src"},  # Directory where your package files are located
```

### Comparing `kfre-0.1.2b3/src/kfre/__init__.py` & `kfre-0.1.2b4/src/kfre/__init__.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b3/src/kfre/main.py` & `kfre-0.1.2b4/src/kfre/main.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b3/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.2b4/src/kfre.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.2b3
+Version: 0.1.2b4
 Summary: A Python library for kidney failure risk estimation using Tangri's KFRE model
 Author: Leonid Shpaner
 Author-email: Lshpaner@ucla.edu
 Project-URL: Author Website, https://www.leonshpaner.com
 Project-URL: Documentation, https://lshpaner.github.io/kfre_docs/
 Project-URL: DOI, https://zenodo.org/records/11100222
 Project-URL: Source Code, https://github.com/lshpaner/kfre
@@ -20,17 +20,15 @@
 # KFRE: Kidney Failure Risk Estimator
 
 [![PyPI](https://img.shields.io/pypi/v/kfre.svg)](https://pypi.org/project/kfre/)
 [![Downloads](https://pepy.tech/badge/kfre)](https://pepy.tech/project/kfre)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/lshpaner/kfre/tree/main?tab=License-1-ov-file)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.11100222.svg)](https://doi.org/10.5281/zenodo.11100222)
 
-<div style="pointer-events: none;">
-    <img src="https://raw.githubusercontent.com/lshpaner/lshpaner.github.io/main/docs/kfre_docs/_static/kfre_logo.svg?token=GHSAT0AAAAAACQTRN6VMOSVD5HGPUNSZQUQZRV6EQQ" width="200" style="border: none; outline: none; box-shadow: none;" draggable="false" oncontextmenu="return false;">
-</div>
+<img src="https://raw.githubusercontent.com/lshpaner/kfre/main/assets/kfre_logo.svg" width="200" style="border: none; outline: none; box-shadow: none;" oncontextmenu="return false;">
 
 
 `kfre` is a Python library designed to estimate the risk of chronic kidney disease (CKD) progression over two distinct timelines: 2 years and 5 years. Using Tangri's Kidney Failure Risk Equation (KFRE), the library provides tools for healthcare professionals and researchers to predict CKD risk based on patient data. It supports predictions for both males and females and includes specific adjustments for individuals from North American and non-North American regions.
 
 ## Prerequisites
 Before you install `kfre`, ensure you have the following:
```

