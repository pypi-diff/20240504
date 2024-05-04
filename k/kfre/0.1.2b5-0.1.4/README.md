# Comparing `tmp/kfre-0.1.2b5.tar.gz` & `tmp/kfre-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.2b5.tar", last modified: Sat May  4 16:19:13 2024, max compression
+gzip compressed data, was "kfre-0.1.4.tar", last modified: Sat May  4 20:20:25 2024, max compression
```

## Comparing `kfre-0.1.2b5.tar` & `kfre-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:19:13.077722 kfre-0.1.2b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 16:19:05.000000 kfre-0.1.2b5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-04 16:19:13.077722 kfre-0.1.2b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-05-04 16:19:05.000000 kfre-0.1.2b5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:19:13.077722 kfre-0.1.2b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-04 16:19:05.000000 kfre-0.1.2b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:19:13.077722 kfre-0.1.2b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:19:13.077722 kfre-0.1.2b5/src/kfre/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 16:19:05.000000 kfre-0.1.2b5/src/kfre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 16:19:05.000000 kfre-0.1.2b5/src/kfre/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:19:13.077722 kfre-0.1.2b5/src/kfre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-04 16:19:13.000000 kfre-0.1.2b5/src/kfre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 16:19:13.000000 kfre-0.1.2b5/src/kfre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:19:13.000000 kfre-0.1.2b5/src/kfre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 16:19:13.000000 kfre-0.1.2b5/src/kfre.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 16:19:13.000000 kfre-0.1.2b5/src/kfre.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:20:25.149416 kfre-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 20:20:15.000000 kfre-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-04 20:20:25.149416 kfre-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-05-04 20:20:15.000000 kfre-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:20:25.149416 kfre-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-04 20:20:15.000000 kfre-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:20:25.149416 kfre-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:20:25.149416 kfre-0.1.4/src/kfre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 20:20:15.000000 kfre-0.1.4/src/kfre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 20:20:15.000000 kfre-0.1.4/src/kfre/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:20:25.149416 kfre-0.1.4/src/kfre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-04 20:20:25.000000 kfre-0.1.4/src/kfre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 20:20:25.000000 kfre-0.1.4/src/kfre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:20:25.000000 kfre-0.1.4/src/kfre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 20:20:25.000000 kfre-0.1.4/src/kfre.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 20:20:25.000000 kfre-0.1.4/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.2b5/LICENSE.md` & `kfre-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b5/README.md` & `kfre-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 ## License
 `kfre` is distributed under the MIT License. See [`LICENSE`](LICENSE.md) for more information.
 
 ## Support
 If you have any questions or issues with `kfre`, please open an issue on this GitHub repository.
 
 ## Acknowledgements
-Tangri's KFRE model and its contributions to kidney disease research.
+The KFRE model developed by Tangri et al. has made significant contributions to kidney disease research.
 
-The `kfre` library is based on the risk prediction models developed in the following studies. Please refer to these studies for an in-depth understanding of the kidney failure risk prediction models used within this library.
+The `kfre` library is based on the risk prediction models developed in the studies referenced below. Please refer to these studies for an in-depth understanding of the kidney failure risk prediction models used within this library.
 
 
 ## References
 
 1. Tangri N, Grams ME, Levey AS, Coresh J, Appel LJ, Astor BC, Chodick G, Collins AJ, Djurdjev O, Elley CR, Evans M, Garg AX, Hallan SI, Inker LA, Ito S, Jee SH, Kovesdy CP, Kronenberg F, Heerspink HJL, Marks A, Nadkarni GN, Navaneethan SD, Nelson RG, Titze S, Sarnak MJ, Stengel B, Woodward M, Iseki K, for the CKD Prognosis Consortium. (2016). *Multinational assessment of accuracy of equations for predicting risk of kidney failure: A meta-analysis. JAMA,* **315**(2), 164–174. doi: 10.1001/jama.2015.18202.
 
 2. Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O., Naimark, D., Levin, A., & Levey, A. S. (2011). *A predictive model for progression of chronic kidney disease to kidney failure. JAMA,* **305**(15), 1553-1559. doi: 10.1001/jama.2011.451.
```

### Comparing `kfre-0.1.2b5/setup.py` & `kfre-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.2_b5",
+    version="0.1.4",
     author="Leonid Shpaner",
-    author_email="Lshpaner@ucla.edu",
-    description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
-    # long_description=open("README.md").read(),
+    author_email="lshpaner@ucla.edu",
+    description="A Python library for estimating kidney failure risk using the KFRE model developed by Tangri et al.",
     long_description=open("min_readme.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     package_dir={"": "src"},  # Directory where your package files are located
     # Automatically find packages in the specified directory
     packages=find_packages(where="src"),
     project_urls={  # Optional
         "Author Website": "https://www.leonshpaner.com",
         "Documentation": "https://lshpaner.github.io/kfre_docs/",
-        "DOI": "https://zenodo.org/records/11100222",
+        "Zenodo Archive": "https://zenodo.org/records/11100222",
         "Source Code": "https://github.com/lshpaner/kfre",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],  # Classifiers for the package
     python_requires=">=3.6",  # Minimum version of Python required
     install_requires=[
-        "numpy>=1.18.5",  # Example of a required library with a minimum version
-        "pandas>=1.0.5",  # Example of another required library with a minimum version
+        "numpy>=1.18.5",  # Minimum version of numpy required
+        "pandas>=1.0.5",  # Minimum version of pandas required
     ],
 )
```

### Comparing `kfre-0.1.2b5/src/kfre/__init__.py` & `kfre-0.1.4/src/kfre/__init__.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.2b5/src/kfre/main.py` & `kfre-0.1.4/src/kfre/main.py`

 * *Files identical despite different names*

