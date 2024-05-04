# Comparing `tmp/meds_etl-0.1.1.tar.gz` & `tmp/meds_etl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds_etl-0.1.1.tar", last modified: Tue Apr  2 02:17:59 2024, max compression
+gzip compressed data, was "meds_etl-0.2.0.tar", last modified: Sat May  4 21:49:48 2024, max compression
```

## Comparing `meds_etl-0.1.1.tar` & `meds_etl-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.777429 meds_etl-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.777429 meds_etl-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.github/workflows/python-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-02 02:17:55.000000 meds_etl-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 02:17:55.000000 meds_etl-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-02 02:17:59.785429 meds_etl-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-02 02:17:55.000000 meds_etl-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 02:17:55.000000 meds_etl-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:17:59.785429 meds_etl-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.777429 meds_etl-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.781429 meds_etl-0.1.1/src/meds_etl/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/flat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.781429 meds_etl-0.1.1/src/meds_etl/mimic/
--rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   361049 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv
--rw-r--r--   0 runner    (1001) docker     (127)    79196 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv
--rw-r--r--   0 runner    (1001) docker     (127)    79970 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv
--rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv
--rw-r--r--   0 runner    (1001) docker     (127)    32354 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/numerics-summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)    34008 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv
--rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_itemid.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/mimic/concept_map/waveforms-summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)    34130 2024-04-02 02:17:55.000000 meds_etl-0.1.1/src/meds_etl/omop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/src/meds_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 02:17:59.000000 meds_etl-0.1.1/src/meds_etl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:59.785429 meds_etl-0.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:55.000000 meds_etl-0.1.1/tests/data/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-02 02:17:55.000000 meds_etl-0.1.1/tests/test_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-02 02:17:55.000000 meds_etl-0.1.1/tests/test_flat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.991894 meds_etl-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 21:49:44.000000 meds_etl-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.983894 meds_etl-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.983894 meds_etl-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-04 21:49:44.000000 meds_etl-0.2.0/.github/workflows/python-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-04 21:49:44.000000 meds_etl-0.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-04 21:49:44.000000 meds_etl-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 21:49:44.000000 meds_etl-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 21:49:44.000000 meds_etl-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-04 21:49:48.991894 meds_etl-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-04 21:49:44.000000 meds_etl-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-04 21:49:44.000000 meds_etl-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:49:48.991894 meds_etl-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.983894 meds_etl-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.983894 meds_etl-0.2.0/src/meds_etl/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31533 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/flat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.987894 meds_etl-0.2.0/src/meds_etl/mimic/
+-rw-r--r--   0 runner    (1001) docker     (127)    18687 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.987894 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   361049 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    79196 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    79970 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32354 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/numerics-summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    34008 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/proc_itemid.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/mimic/concept_map/waveforms-summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33623 2024-05-04 21:49:44.000000 meds_etl-0.2.0/src/meds_etl/omop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.991894 meds_etl-0.2.0/src/meds_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 21:49:48.000000 meds_etl-0.2.0/src/meds_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.991894 meds_etl-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:48.991894 meds_etl-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:49:44.000000 meds_etl-0.2.0/tests/data/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-04 21:49:44.000000 meds_etl-0.2.0/tests/test_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-04 21:49:44.000000 meds_etl-0.2.0/tests/test_flat.py
```

### Comparing `meds_etl-0.1.1/.github/workflows/python-build.yml` & `meds_etl-0.2.0/.github/workflows/python-build.yml`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/.github/workflows/python-test.yml` & `meds_etl-0.2.0/.github/workflows/python-test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
-  build:
+  test:
 
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python-version: ["3.10"]
 
@@ -22,15 +22,15 @@
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest
     - name: Install MEDS ETL
-      run: python -m pip install .
+      run: python -m pip install ".[duckdb,cpp]"
     - name: Download MIMIC-IV-Demo (v2.2)
       run: |
         # Download the MIMIC-IV-Demo dataset (v2.2) to a tests/data/ directory
         wget -r -N -c --no-host-directories --cut-dirs=1 -np -P tests/data https://physionet.org/files/mimic-iv-demo/2.2/
     - name: Run tests
       run: |
         pytest -v
```

### Comparing `meds_etl-0.1.1/.gitignore` & `meds_etl-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/.pre-commit-config.yaml` & `meds_etl-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/LICENSE` & `meds_etl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/PKG-INFO` & `meds_etl-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: meds_etl
-Version: 0.1.1
-Summary: A data standard for working with event stream data
-License: Apache-2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyarrow>=8
-Requires-Dist: polars>=0.20.10
-Requires-Dist: jsonschema>=4.0.0
-Requires-Dist: meds==0.1.3
-Requires-Dist: typing_extensions>=4.0
-Requires-Dist: datasets>=2.0.0
-Requires-Dist: tqdm>=4.6.0
-
 # meds_etl
 
 A collection of ETLs from common data formats to Medical Event Data Standard (MEDS)
 
 This package library currently supports:
 
 - MIMIC-IV
@@ -26,15 +11,38 @@
 ## Setup
 Create an environment of your choice:
 ```bash
 conda create -n meds_etl
 ```
 Install the package
 ```bash
-python -m pip install .
+pip install meds_etl
+```
+
+## Backends
+
+ETLs are one of the most computationally heavy components of MEDS, so efficiency is very important.
+
+MEDS-ETL has several parallel implementations of core algorithms to balance the tradeoff between efficiency and ease of use.
+
+All commands generally take an additional parameter --backend, that allows users to switch between different backends.
+
+We currently support two backends: polars (the default) and cpp.
+
+Backend information:
+
+- polars (default backend): A Python only implementation that only requires polars to run. The main issue with this implementation is that it is rather inefficient. It's recommended to use as few shards as possible while still avoiding out of memory errors.
+
+- cpp: A custom C++ backend. This backend is very efficient, but might not run on all platforms and has a limited feature set. It's recommended to use the same number of shards as you have CPUs available.
+
+If you want to use either the cpp backend, make sure to install meds_etl with the correct optional dependencies.
+
+```bash
+# For the cpp backend
+pip install "meds_etl[cpp]"
 ```
 
 ## MIMIC-IV
 
 In order to run the MIMIC-IV ETL, simply run the following command:
 
 ```bash
```

### Comparing `meds_etl-0.1.1/pyproject.toml` & `meds_etl-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,30 @@
 readme = "README.md"
 license = {text = "Apache-2.0"}
 
 dependencies = [
     "pyarrow >= 8",
     "polars >= 0.20.10",
     "jsonschema >= 4.0.0",
-    "meds == 0.1.3",
+    "meds == 0.2.0",
     "typing_extensions >= 4.0",
     "datasets >= 2.0.0",
-    "tqdm >= 4.6.0"
+    "tqdm >= 4.6.0",
+    "psutil >= 5.9.0"
 ]
 
+[project.optional-dependencies]
+duckdb = [
+    "duckdb >= 0.10.1"
+]
+cpp = [
+    "meds_etl_cpp == 0.2.0"
+]
+
+
 [project.scripts]
 meds_etl_mimic = "meds_etl.mimic:main"
 meds_etl_omop = "meds_etl.omop:main"
 meds_etl_from_flat = "meds_etl.flat:convert_flat_to_meds_main"
 meds_etl_to_flat = "meds_etl.flat:convert_meds_to_flat_main"
 
 [tool.setuptools_scm]
```

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/__init__.py` & `meds_etl-0.2.0/src/meds_etl/mimic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import argparse
 import json
 import os
 import shutil
 import subprocess
 from importlib.resources import files
+from typing import Iterable
 
 import jsonschema
 import meds
 import polars as pl
 
 import meds_etl
 import meds_etl.flat
 
 MIMIC_VERSION = "2.2"
 
+MIMIC_TIME_FORMATS: Iterable[str] = ("%Y-%m-%d %H:%M:%S%.f", "%Y-%m-%d")
+
 
 def add_dot(code, position):
     return (
         pl.when(code.str.len_chars() > position)
         .then(code.str.slice(0, position) + "." + code.str.slice(position))
         .otherwise(code)
     )
@@ -39,14 +42,16 @@
 
 
 def main():
     parser = argparse.ArgumentParser(prog="meds_etl_mimic", description="Performs an ETL from MIMIC_IV to MEDS")
     parser.add_argument("src_mimic", type=str)
     parser.add_argument("destination", type=str)
     parser.add_argument("--num_shards", type=int, default=100)
+    parser.add_argument("--num_proc", type=int, default=1)
+    parser.add_argument("--backend", type=str, default="polars")
     args = parser.parse_args()
 
     if not os.path.exists(args.src_mimic):
         raise ValueError(f'The source MIMIC_IV folder ("{args.src_mimic}") does not seem to exist?')
 
     src_mimic_version = os.path.join(args.src_mimic, MIMIC_VERSION)
 
@@ -345,21 +350,24 @@
             reader = pl.read_csv_batched(
                 uncompressed_path,
                 infer_schema_length=0,
                 batch_size=10_000_000,
             )
 
             patient_id = pl.col("subject_id").cast(pl.Int64)
-            time = mapping_code["time"]
+            time = meds_etl.flat.parse_time(mapping_code["time"], MIMIC_TIME_FORMATS)
+
             code = mapping_code["code"]
             if "value" in mapping_code:
                 value = mapping_code["value"]
             else:
                 value = pl.lit(None, dtype=str)
 
+            d, n, t = meds_etl.flat.convert_generic_value_to_specific(value)
+
             if "metadata" not in mapping_code:
                 mapping_code["metadata"] = {}
 
             mapping_code["metadata"]["table"] = pl.lit(table_name)
 
             batch_index = 0
             while True:
@@ -379,36 +387,52 @@
                 if mapping_code.get("possibly_null_time", False):
                     table_csv = table_csv.filter(time.is_not_null())
 
                 columns = {
                     "patient_id": patient_id,
                     "time": time,
                     "code": code,
-                    "value": value,
                 }
 
+                columns["datetime_value"] = d
+                columns["numeric_value"] = n
+                columns["text_value"] = t
+
                 for k, v in mapping_code["metadata"].items():
                     columns[k] = v.alias(k)
 
-                event_data = table_csv.select(**columns).collect()
+                try:
+                    event_data = table_csv.select(**columns).collect()
+                except Exception as e:
+                    print("Could not process", table_name, mapping_codes)
+                    print(columns)
+                    raise e
 
                 fname = os.path.join(
                     temp_dir, "flat_data", f'{table_name.replace("/", "_")}_{map_index}_{batch_index}.parquet'
                 )
                 event_data.write_parquet(fname)
 
         os.remove(uncompressed_path)
 
     shutil.rmtree(decompressed_dir)
 
     print("Processing each shard")
 
+    with open(os.path.join(temp_dir, "metadata.json"), "w") as f:
+        f.write("{}\n")
+
     meds_etl.flat.convert_flat_to_meds(
-        temp_dir, os.path.join(args.destination, "result"), num_shards=args.num_shards, num_proc=1
+        temp_dir,
+        os.path.join(args.destination, "result"),
+        num_shards=args.num_shards,
+        num_proc=args.num_proc,
+        backend=args.backend,
     )
+
     shutil.move(os.path.join(args.destination, "result", "data"), os.path.join(args.destination, "data"))
     shutil.rmtree(os.path.join(args.destination, "result"))
 
     shutil.rmtree(temp_dir)
 
     code_metadata = {}
 
@@ -443,15 +467,15 @@
             "descr": pl.col("label"),
             "parent": pl.col("omop_vocabulary_id") + "/" + pl.col("omop_concept_code"),
         },
     }
 
     for fname, mapping_info in code_metadata_files.items():
         with files("meds_etl.mimic.concept_map").joinpath(fname + ".csv").open("rb") as f:
-            table = pl.read_csv(f, infer_schema_length=0)
+            table = pl.read_csv(f.read(), infer_schema_length=0)
             code_and_value = table.select(
                 code=mapping_info["code"], descr=mapping_info["descr"], parent=mapping_info["parent"]
             )
             for code, descr, value in code_and_value.iter_rows():
                 if code in code_metadata:
                     assert (
                         value == code_metadata[code].get("parent_codes", [None])[0]
```

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/LICENSE` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/LICENSE`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/d_labitems_to_loinc.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/inputevents_to_rxnorm.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/lab_itemid_to_loinc.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/meas_chartevents_main.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/meas_chartevents_value.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/numerics-summary.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/numerics-summary.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/outputevents_to_loinc.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/proc_datetimeevents.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/proc_itemid.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/proc_itemid.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/mimic/concept_map/waveforms-summary.csv` & `meds_etl-0.2.0/src/meds_etl/mimic/concept_map/waveforms-summary.csv`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/src/meds_etl/omop.py` & `meds_etl-0.2.0/src/meds_etl/omop.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,100 @@
+from __future__ import annotations
+
 import argparse
+import itertools
 import json
 import multiprocessing
 import os
 import pickle
 import random
 import shutil
 import subprocess
 import tempfile
-from typing import Any, Dict, List, Tuple
+import uuid
+from typing import Any, Dict, Iterable, List, Mapping, Tuple
 
 import jsonschema
 import meds
 import polars as pl
-import pyarrow.parquet as pq
 from tqdm import tqdm
 
 import meds_etl
 import meds_etl.flat
 
 RANDOM_SEED: int = 3422342
 # OMOP constants
 CUSTOMER_CONCEPT_ID_START: int = 2_000_000_000
 DEFAULT_VISIT_CONCEPT_ID: int = 8
 DEFAULT_NOTE_CONCEPT_ID: int = 46235038
 DEFAULT_VISIT_DETAIL_CONCEPT_ID: int = 4203722
 
+OMOP_TIME_FORMATS: Iterable[str] = ("%Y-%m-%d %H:%M:%S%.f", "%Y-%m-%d")
+
+
+def split_list(ls: List[Any], parts: int) -> List[List[Any]]:
+    per_list = (len(ls) + parts - 1) // parts
+    result = []
+
+    for i in range(parts):
+        sublist = ls[i * per_list : (i + 1) * per_list]
+        if len(sublist) > 0:
+            result.append(sublist)
 
-def get_table_files(path_to_src_omop_dir: str, table_name: str, table_details={}) -> List[str]:
-    """Retrieve all .csv/.csv.gz files for the OMOP table given by `table_name` in `path_to_src_omop_dir`
+    return result
+
+
+def get_table_files(path_to_src_omop_dir: str, table_name: str, table_details={}) -> Tuple[List[str], List[str]]:
+    """Retrieve all .csv/.csv.gz/.parquet files for the OMOP table given by `table_name` in `path_to_src_omop_dir`
 
     Because OMOP tables can be quite large for datasets comprising millions
     of patients, those tables are often split into compressed shards. So
     the `measurements` "table" might actually be a folder containing files
     `000000000000.csv.gz` up to `000000000152.csv.gz`. This function
     takes a path corresponding to an OMOP table with its standard name (e.g.,
-    `condition_occurrence`, `measurement`, `observation`) and returns a list
-    of paths, each of which represents a file e.g.,
-    [`measurement/000000000000.csv.gz`, `000000000001.csv.gz`, ..., `000000000152.csv.gz`]
+    `condition_occurrence`, `measurement`, `observation`) and returns two list
+    of paths.
+
+    The first list contains all the csv files. The second list contains all parquet files.
     """
     if table_details.get("file_suffix"):
         table_name += "_" + table_details["file_suffix"]
 
     path_to_table: str = os.path.join(path_to_src_omop_dir, table_name)
 
     if os.path.exists(path_to_table) and os.path.isdir(path_to_table):
-        return [
-            os.path.join(path_to_table, a)
-            for a in os.listdir(path_to_table)
-            if a.endswith(".csv") or a.endswith(".csv.gz")
-        ]
+        csv_files = []
+        parquet_files = []
+
+        for a in os.listdir(path_to_table):
+            fname = os.path.join(path_to_table, a)
+            if a.endswith(".csv") or a.endswith(".csv.gz"):
+                csv_files.append(fname)
+            elif a.endswith(".parquet"):
+                parquet_files.append(fname)
+
+        return csv_files, parquet_files
     elif os.path.exists(path_to_table + ".csv"):
-        return [path_to_table + ".csv"]
+        return [path_to_table + ".csv"], []
     elif os.path.exists(path_to_table + ".csv.gz"):
-        return [path_to_table + ".csv.gz"]
+        return [path_to_table + ".csv.gz"], []
+    elif os.path.exists(path_to_table + ".parquet"):
+        return [], [path_to_table + ".parquet"]
     else:
-        return []
+        return [], []
+
+
+def read_polars_df(fname: str) -> pl.DataFrame:
+    """Read a file that might be a CSV or Parquet file"""
+    if fname.endswith(".csv"):
+        return pl.read_csv(fname)
+    elif fname.endswith(".parquet"):
+        return pl.read_parquet(fname)
+    else:
+        raise RuntimeError("Found file of unknown type " + fname + " expected parquet or csv")
 
 
 def load_file(path_to_decompressed_dir: str, fname: str) -> Any:
     """Load a file from disk, unzip into temporary decompressed directory if needed
 
     Args:
         path_to_decompressed_dir (str): Path where (temporary) decompressed file should be stored
@@ -72,24 +108,231 @@
         subprocess.run(["gunzip", "-c", fname], stdout=file)
         return file
     else:
         # If the file isn't compressed, we don't write anything to `path_to_decompressed_dir`
         return open(fname)
 
 
-def process_table(args):
+def cast_to_datetime(table: pl.LazyFrame, column: str, move_to_end_of_day: bool = False):
+    if table.schema[column] == pl.Utf8():
+        if not move_to_end_of_day:
+            return (meds_etl.flat.parse_time(pl.col(column), OMOP_TIME_FORMATS),)
+        else:
+            # Try to cast time to a datetime but if only the date is available, then use
+            # that date with a timestamp of 23:59:59
+            time = pl.col(column)
+            time = pl.coalesce(
+                time.str.to_datetime("%Y-%m-%d %H:%M:%S%.f", strict=False, time_unit="us"),
+                time.str.to_datetime("%Y-%m-%d", strict=False, time_unit="us").dt.offset_by("1d").dt.offset_by("-1s"),
+            )
+            return time
+    elif table.schema[column] == pl.Date():
+        time = pl.col(column).cast(pl.Datetime(time_unit="us"))
+        if move_to_end_of_day:
+            time = time.dt.offset_by("1d").dt.offset_by("-1s")
+        return time
+    elif isinstance(table.schema[column], pl.Datetime):
+        return pl.col(column).cast(pl.Datetime(time_unit="us"))
+    else:
+        raise RuntimeError("Unknown how to handle date type? " + table.schema[column] + " " + column)
+
+
+def write_event_data(
+    path_to_MEDS_flat_dir: str,
+    get_batch: Any,
+    table_name: str,
+    all_table_details: Iterable[Mapping[str, Any]],
+    concept_id_map: Mapping[int, str],
+    concept_name_map: Mapping[int, str],
+) -> pl.LazyFrame:
+    """Write event data from the given table to event files in MEDS Flat format"""
+    for table_details in all_table_details:
+        batch = get_batch()
+        batch = batch.rename({c: c.lower() for c in batch.columns})
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+        # Determine what to use for the `patient_id` column in MEDS Flat  #
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+        # Define the MEDS Flat `patient_id` (left) to be the `person_id` columns in OMOP (right)
+        patient_id = pl.col("person_id").cast(pl.Int64)
+
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+        # Determine what to use for the `time` column in MEDS Flat  #
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+        # Use special processing for the `PERSON` OMOP table
+        if table_name == "person":
+            # Take the `birth_datetime` if its available, otherwise
+            # construct it from `year_of_birth`, `month_of_birth`, `day_of_birth`
+            time = pl.coalesce(
+                cast_to_datetime(batch, "birth_datetime"),
+                pl.datetime(
+                    pl.col("year_of_birth"),
+                    pl.coalesce(pl.col("month_of_birth"), 1),
+                    pl.coalesce(pl.col("day_of_birth"), 1),
+                    time_unit="us",
+                ),
+            )
+        else:
+            # Use the OMOP table name + `_start_datetime` as the `time` column
+            # if it's available otherwise `_start_date`, `_datetime`, `_date`
+            # in that order of preference
+            options = ["_start_datetime", "_start_date", "_datetime", "_date"]
+            options = [
+                cast_to_datetime(batch, table_name + option, move_to_end_of_day=True)
+                for option in options
+                if table_name + option in batch.columns
+            ]
+            assert len(options) > 0, f"Could not find the time column {batch.columns}"
+            time = pl.coalesce(options)
+
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+        # Determine what to use for the `code` column in MEDS Flat  #
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+        if table_details.get("force_concept_code"):
+            # Rather than getting the concept ID from the source table, we use the concept ID
+            # passed in by the user eg `4083587` for `Birth`
+            source_concept_id = pl.lit(0, dtype=pl.Int64)
+            code = pl.lit(table_details.get("force_concept_code"), dtype=pl.Utf8)
+        else:
+            # Try using the source concept ID, but if it's not available then use the concept ID
+            concept_id_field = table_details.get("concept_id_field", table_name + "_concept_id")
+            concept_id = pl.col(concept_id_field).cast(pl.Int64)
+            if concept_id_field.replace("_concept_id", "_source_concept_id") in batch.columns:
+                source_concept_id = pl.col(concept_id_field.replace("_concept_id", "_source_concept_id")).cast(pl.Int64)
+            else:
+                source_concept_id = pl.lit(0, dtype=pl.Int64)
+
+            # And if the source concept ID and concept ID aren't available, use `fallback_concept_id`
+            fallback_concept_id = pl.lit(table_details.get("fallback_concept_id", None), dtype=pl.Int64)
+
+            concept_id = (
+                pl.when(source_concept_id != 0)
+                .then(source_concept_id)
+                .when(concept_id != 0)
+                .then(concept_id)
+                .otherwise(fallback_concept_id)
+            )
+
+            # Replace values in `concept_id` with the normalized concepts to which they are mapped
+            # based on the `concept_id_map`
+            code = concept_id.replace(concept_id_map)
+
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+        # Determine what to use for the `value` column in MEDS Flat   #
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+        # By default, if the user doesn't specify in `table_details`
+        # what the
+        value = pl.lit(None, dtype=str)
+
+        if table_details.get("string_value_field"):
+            value = pl.col(table_details["string_value_field"])
+        if table_details.get("numeric_value_field"):
+            value = pl.coalesce(pl.col(table_details["numeric_value_field"]), value)
+
+        if table_details.get("concept_id_value_field"):
+            concept_id_value = pl.col(table_details["concept_id_value_field"]).cast(pl.Int64)
+
+            # Normally we would prefer string or numeric value.
+            # But sometimes we get a value_as_concept_id with no string or numeric value.
+            # So we want to define a backup value here
+            #
+            # There are two reasons for this, each with different desired behavior:
+            # 1. OMOP defines a code with a maps to value relationship.
+            #      See https://www.ohdsi.org/web/wiki/doku.php?id=documentation:vocabulary:mapping
+            #      In this cases we generally just want to drop the value, as the data is in source_concept_id
+            # 2. The ETL has decided to put non-maps to value codes in observation for various reasons.
+            #      For instance STARR-OMOP puts shc_medical_hx in here
+            #      In this case, we generally want to create a string value with the source code value.
+
+            backup_value = (
+                pl.when((source_concept_id == 0) & (concept_id_value != 0))
+                .then(
+                    # Source concept 0 indicates we need a backup value since it's not captured by the source
+                    "SOURCE_CODE/"
+                    + pl.col(concept_id_field.replace("_concept_id", "_source_value"))
+                )
+                .otherwise(
+                    # Should be captured by the source concept id, so just map the value to a string.
+                    concept_id_value.map_dict(concept_name_map)
+                )
+            )
+
+            value = pl.coalesce(value, backup_value)
+
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+        # Determine the metadata columns to be stored in MEDS Flat  #
+        # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+        # Every key in the `metadata` dictionary will become a distinct
+        # column in the MEDS Flat file; for each event, the metadata column
+        # and its corresponding value for a given patient will be stored
+        # as event metadata in the MEDS representation
+        metadata = {
+            "table": pl.lit(table_name, dtype=str),
+        }
+
+        if "visit_occurrence_id" in batch.columns:
+            metadata["visit_id"] = pl.col("visit_occurrence_id")
+
+        if "unit_source_value" in batch.columns:
+            metadata["unit"] = pl.col("unit_source_value")
+
+        if "load_table_id" in batch.columns:
+            metadata["clarity_table"] = pl.col("load_table_id")
+
+        if "note_id" in batch.columns:
+            metadata["note_id"] = pl.col("note_id")
+
+        if (table_name + "_end_datetime") in batch.columns:
+            end = cast_to_datetime(batch, table_name + "_end_datetime", move_to_end_of_day=True)
+            metadata["end"] = end
+
+        batch = batch.filter(code.is_not_null())
+
+        columns = {
+            "patient_id": patient_id,
+            "time": time,
+            "code": code,
+        }
+
+        d, n, t = meds_etl.flat.convert_generic_value_to_specific(value)
+
+        columns["datetime_value"] = d
+        columns["numeric_value"] = n
+        columns["text_value"] = t
+
+        # Add metadata columns to the set of MEDS flat dataframe columns
+        for k, v in metadata.items():
+            columns[k] = v.alias(k)
+
+        # We don't worry about partitioning here; let `flat_to_meds` handle that
+        event_data = batch.select(**columns)
+        # Write this part of the MEDS Flat file to disk
+        fname = os.path.join(path_to_MEDS_flat_dir, f'{table_name.replace("/", "_")}_{uuid.uuid4()}.parquet')
+        try:
+            event_data.sink_parquet(fname, compression="zstd", compression_level=1, maintain_order=False)
+        except pl.exceptions.InvalidOperationError as e:
+            print(table_name)
+            print(e)
+            print(event_data.explain(streaming=True))
+            raise e
+
+
+def process_table_csv(args):
     (
         table_file,
         table_name,
         all_table_details,
         concept_id_map_data,
         concept_name_map_data,
         path_to_MEDS_flat_dir,
         path_to_decompressed_dir,
-        map_index,
         verbose,
     ) = args
     """
 
     This function is designed to be called through parallel processing utilities
     such as `pool.imap_unordered(process_table, [args1, args2, ..., argsN])
 
@@ -127,293 +370,90 @@
             batch_index += 1
             batch = table.next_batches(1)  # Returns a list of length 1 containing a table for the batch
             if batch is None:
                 break
 
             batch = batch[0]  # (Because `table.next_batches` returns a list)
 
-            batch = batch.lazy().rename({c: c.lower() for c in batch.columns})
-
-            for i, table_details in enumerate(all_table_details):
-                if verbose:
-                    print(f"Batch {i}")
-
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-                # Determine what to use for the `patient_id` column in MEDS Flat  #
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-
-                # Define the MEDS Flat `patient_id` (left) to be the `person_id` columns in OMOP (right)
-                patient_id = pl.col("person_id").cast(pl.Int64)
-
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-                # Determine what to use for the `time` column in MEDS Flat  #
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-
-                # Use special processing for the `PERSON` OMOP table
-                if table_name == "person":
-                    # Take the `birth_datetime` if its available, otherwise
-                    # construct it from `year_of_birth`, `month_of_birth`, `day_of_birth`
-                    time = pl.coalesce(
-                        pl.col("birth_datetime").str.to_datetime("%Y-%m-%d %H:%M:%S%.f", strict=False, time_unit="ms"),
-                        pl.datetime(
-                            pl.col("year_of_birth"),
-                            pl.coalesce(pl.col("month_of_birth"), 1),
-                            pl.coalesce(pl.col("day_of_birth"), 1),
-                        ),
-                    )
-                else:
-                    # Use the OMOP table name + `_start_datetime` as the `time` column
-                    # if it's available otherwise `_start_date`, `_datetime`, `_date`
-                    # in that order of preference
-                    options = ["_start_datetime", "_start_date", "_datetime", "_date"]
-                    options = [
-                        pl.col(table_name + option) for option in options if table_name + option in batch.columns
-                    ]
-                    assert len(options) > 0, f"Could not find the time column {batch.columns}"
-                    time = pl.coalesce(options)
-
-                    # Try to cast time to a datetime but if only the date is available, then use
-                    # that date with a timestamp of 23:59:59
-                    time = pl.coalesce(
-                        time.str.to_datetime("%Y-%m-%d %H:%M:%S%.f", strict=False, time_unit="ms"),
-                        time.str.to_datetime("%Y-%m-%d", strict=False, time_unit="ms")
-                        .dt.offset_by("1d")
-                        .dt.offset_by("-1s"),
-                    )
-
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-                # Determine what to use for the `code` column in MEDS Flat  #
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-
-                if table_details.get("force_concept_id"):
-                    # Rather than getting the concept ID from the source table, we use the concept ID
-                    # passed in by the user eg `4083587` for `Birth`
-                    concept_id = pl.lit(table_details["force_concept_id"], dtype=pl.Int64)
-                    source_concept_id = pl.lit(0, dtype=pl.Int64)
-                else:
-                    # Try using the source concept ID, but if it's not available then use the concept ID
-                    concept_id_field = table_details.get("concept_id_field", table_name + "_concept_id")
-                    concept_id = pl.col(concept_id_field).cast(pl.Int64)
-                    if concept_id_field.replace("_concept_id", "_source_concept_id") in batch.columns:
-                        source_concept_id = pl.col(concept_id_field.replace("_concept_id", "_source_concept_id")).cast(
-                            pl.Int64
-                        )
-                    else:
-                        source_concept_id = pl.lit(0, dtype=pl.Int64)
-
-                    # And if the source concept ID and concept ID aren't available, use `fallback_concept_id`
-                    fallback_concept_id = pl.lit(table_details.get("fallback_concept_id", None), dtype=pl.Int64)
-
-                    concept_id = (
-                        pl.when(source_concept_id != 0)
-                        .then(source_concept_id)
-                        .when(concept_id != 0)
-                        .then(concept_id)
-                        .otherwise(fallback_concept_id)
-                    )
-
-                # Replace values in `concept_id` with the normalized concepts to which they are mapped
-                # based on the `concept_id_map`
-                code = concept_id.map_dict(concept_id_map)
-
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-                # Determine what to use for the `value` column in MEDS Flat   #
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-
-                # By default, if the user doesn't specify in `table_details`
-                # what the
-                value = pl.lit(None, dtype=str)
-
-                if table_details.get("string_value_field"):
-                    value = pl.col(table_details["string_value_field"])
-                if table_details.get("numeric_value_field"):
-                    value = pl.coalesce(pl.col(table_details["numeric_value_field"]), value)
-
-                if table_details.get("concept_id_value_field"):
-                    concept_id_value = pl.col(table_details["concept_id_value_field"]).cast(pl.Int64)
-
-                    # Normally we would prefer string or numeric value.
-                    # But sometimes we get a value_as_concept_id with no string or numeric value.
-                    # So we want to define a backup value here
-                    #
-                    # There are two reasons for this, each with different desired behavior:
-                    # 1. OMOP defines a code with a maps to value relationship.
-                    #      See https://www.ohdsi.org/web/wiki/doku.php?id=documentation:vocabulary:mapping
-                    #      In this cases we generally just want to drop the value, as the data is in source_concept_id
-                    # 2. The ETL has decided to put non-maps to value codes in observation for various reasons.
-                    #      For instance STARR-OMOP puts shc_medical_hx in here
-                    #      In this case, we generally want to create a string value with the source code value.
-
-                    backup_value = (
-                        pl.when((source_concept_id == 0) & (concept_id_value != 0))
-                        .then(
-                            # Source concept 0 indicates we need a backup value since it's not captured by the source
-                            "SOURCE_CODE/"
-                            + pl.col(concept_id_field.replace("_concept_id", "_source_value"))
-                        )
-                        .otherwise(
-                            # Should be captured by the source concept id, so just map the value to a string.
-                            concept_id_value.map_dict(concept_name_map)
-                        )
-                    )
-
-                    value = pl.coalesce(value, backup_value)
-
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-                # Determine the metadata columns to be stored in MEDS Flat  #
-                # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-
-                # Every key in the `metadata` dictionary will become a distinct
-                # column in the MEDS Flat file; for each event, the metadata column
-                # and its corresponding value for a given patient will be stored
-                # as event metadata in the MEDS representation
-                metadata = {
-                    "table": pl.lit(table_name, dtype=str),
-                }
+            batch = batch.lazy()
 
-                if "visit_occurrence_id" in batch.columns:
-                    metadata["visit_id"] = pl.col("visit_occurrence_id")
-
-                if "unit_source_value" in batch.columns:
-                    metadata["unit"] = pl.col("unit_source_value")
-
-                if "load_table_id" in batch.columns:
-                    metadata["clarity_table"] = pl.col("load_table_id")
-
-                if "note_id" in batch.columns:
-                    metadata["note_id"] = pl.col("note_id")
-
-                if (table_name + "_end_datetime") in batch.columns:
-                    end = pl.col(table_name + "_end_datetime")
-                    end = pl.coalesce(
-                        end.str.to_datetime("%Y-%m-%d %H:%M:%S%.f", strict=False, time_unit="ms"),
-                        end.str.to_datetime("%Y-%m-%d", strict=False, time_unit="ms")
-                        .dt.offset_by("1d")
-                        .dt.offset_by("-1s"),
-                    )
-                    metadata["end"] = end
-
-                batch = batch.filter(code.is_not_null())
-
-                columns = {
-                    "patient_id": patient_id,
-                    "time": time,
-                    "code": code,
-                    "value": value,
-                }
+            write_event_data(
+                path_to_MEDS_flat_dir,
+                lambda: batch.lazy(),
+                table_name,
+                all_table_details,
+                concept_id_map,
+                concept_name_map,
+            )
 
-                # Add metadata columns to the set of MEDS flat dataframe columns
-                for k, v in metadata.items():
-                    columns[k] = v.alias(k)
-
-                # We don't worry about partitioning here; let `flat_to_meds` handle that
-                event_data = batch.select(**columns).collect()
-
-                # Write this part of the MEDS Flat file to disk
-                fname = os.path.join(
-                    path_to_MEDS_flat_dir, f'{table_name.replace("/", "_")}_{map_index}_{batch_index}.parquet'
-                )
-                event_data.write_parquet(fname)
 
+def process_table_parquet(args):
+    (
+        table_files,
+        table_name,
+        all_table_details,
+        concept_id_map_data,
+        concept_name_map_data,
+        path_to_MEDS_flat_dir,
+        verbose,
+    ) = args
+    """
 
-def process_shard(args: tuple[int, str, str]):
-    """Collect measurements across OMOP table shards into MEDS patient timelines
+    This function is designed to be called through parallel processing utilities
+    such as `pool.imap_unordered(process_table, [args1, args2, ..., argsN])
 
     Args:
-        args (tuple): A tuple which contains the following positional variables:
-            shard_index (int): The shard index to which a subset of patient ID's are mapped,
-                used in `path_to_temp_dir` (see  below)
-            path_to_temp_dir (str): Path to the directory where sharded patient measurements are stored.
-                Measurements will be *read* from files in the shard subfolders in this directory.
-            path_to_data_dir (str): Path to the directory where MEDS timelines should be *written*.
-                See below for expected file naming convention.
-
-    Returns:
-        Nothing, but MEDS timelines for the given `shard_index` are written
-        to "{path_to_data_dir}/data_{shard_index}.parquet" and can be read in eg
-        as HuggingFace datasets.
+        args (tuple): A tuple with the following elements:
+            table_file (str): Path to the raw source table file (can be compressed)
+            table_name (str): Name of the source table. Used for table-specific preprocessing
+                and selecting columns which often have the table name embedded within them
+                such as `measurement_datetime` in the `measurement` table.
+            all_table_details (List[Dict[str, Any]]): A list of details about the particular
+                table being processed that help determine how to map from the raw OMOP data
+                to the MEDS standard.
 
-    Raises:
-        ValueError: If any important columns contain null/invalid values
     """
-    shard_index, path_to_temp_dir, path_to_data_dir = args
-    path_to_shard_dir: str = os.path.join(path_to_temp_dir, str(shard_index))
-
-    # (Lazily) concatenate all OMOP table entries for the patients represented in the patient shard
-    events = [pl.scan_parquet(os.path.join(path_to_shard_dir, a)) for a in os.listdir(path_to_shard_dir)]
-    all_events = pl.concat(events, how="diagonal_relaxed")
-
-    # Verify that all important columns have no null entries
-    for important_column in ("patient_id", "time", "code"):
-        rows_with_invalid_code = all_events.filter(pl.col(important_column).is_null()).collect()
-        if len(rows_with_invalid_code) != 0:
-            print("Have rows with invalid " + important_column)
-            for row in rows_with_invalid_code:
-                print(row)
-            raise ValueError("Cannot have rows with invalid " + important_column)
-
-    # Aggregate measurements into events (lazy, not executed until `collect()`)
-    measurement = pl.struct(
-        code=pl.col("code"),
-        text_value=pl.col("text_value"),
-        numeric_value=pl.col("numeric_value"),
-        datetime_value=pl.col("datetime_value"),
-        metadata=pl.col("metadata"),
-    )
+    concept_id_map = pickle.loads(concept_id_map_data)  # 0.25 GB for STARR-OMOP
+    concept_name_map = pickle.loads(concept_name_map_data)  # 0.5GB for STARR-OMOP
+    if verbose:
+        print("Working on ", table_files, table_name, all_table_details)
 
-    grouped_by_time = all_events.groupby("patient_id", "time").agg(measurements=measurement)
+    if not isinstance(all_table_details, list):
+        all_table_details = [all_table_details]
 
-    # Aggregate events into patient timelines (lazy, not executed until `collect()`)
-    event = pl.struct(
-        pl.col("time"),
-        pl.col("measurements"),
+    # Load the source table, decompress if needed
+    write_event_data(
+        path_to_MEDS_flat_dir,
+        lambda: pl.scan_parquet(table_files),
+        table_name,
+        all_table_details,
+        concept_id_map,
+        concept_name_map,
     )
 
-    grouped_by_patient = grouped_by_time.groupby("patient_id").agg(events=event.sort_by(pl.col("time")))
-
-    # We now have our data in the final form, grouped_by_patient, but we have to do one final transformation
-    # We have to convert from polar's large_list to list because large_list is not supported by huggingface
-
-    # We do this conversion using the pyarrow library
-
-    # Save and load our data in order to convert to pyarrow library
-    converted = grouped_by_patient.collect().to_arrow()
-
-    # Now we need to reconstruct the schema
-    # We do this by pulling the metadata schema and then using meds.patient_schema
-    event_schema = converted.schema.field("events").type.value_type
-    measurement_schema = event_schema.field("measurements").type.value_type
-    metadata_schema = measurement_schema.field("metadata").type
-
-    desired_schema = meds.patient_schema(metadata_schema)
-
-    # All the large_lists are now converted to lists, so we are good to load with huggingface
-    casted = converted.cast(desired_schema)
-
-    pq.write_table(casted, os.path.join(path_to_data_dir, f"data_{shard_index}.parquet"))
-
 
 def extract_metadata(path_to_src_omop_dir: str, path_to_decompressed_dir: str, verbose: int = 0) -> Tuple:
     concept_id_map: Dict[int, str] = {}  # [key] concept_id -> [value] concept_code
     concept_name_map: Dict[int, str] = {}  # [key] concept_id -> [value] concept_name
     code_metadata: Dict[str, Any] = {}  # [key] concept_code -> [value] metadata
 
     # Read in the OMOP `CONCEPT` table from disk
     # (see https://ohdsi.github.io/TheBookOfOhdsi/StandardizedVocabularies.html#concepts)
     # and use it to generate metadata file as well as populate maps
     # from (concept ID -> concept code) and (concept ID -> concept name)
     print("Generating metadata from OMOP `concept` table")
-    for concept_file in tqdm(get_table_files(path_to_src_omop_dir, "concept")):
+    for concept_file in tqdm(itertools.chain(*get_table_files(path_to_src_omop_dir, "concept"))):
         # Note: Concept table is often split into gzipped shards by default
         if verbose:
             print(concept_file)
         with load_file(path_to_decompressed_dir, concept_file) as f:
             # Read the contents of the `concept` table shard
             # `load_file` will unzip the file into `path_to_decompressed_dir` if needed
-            concept: pl.DataFrame = pl.read_csv(f.name)
+            concept = read_polars_df(f.name)
+
             concept_id = pl.col("concept_id").cast(pl.Int64)
             code = pl.col("vocabulary_id") + "/" + pl.col("concept_code")
 
             # Convert the table into a dictionary
             result = concept.select(concept_id=concept_id, code=code, name=pl.col("concept_name"))
 
             result = result.to_dict(as_series=False)
@@ -434,41 +474,20 @@
             )
             for i in range(len(custom_concepts["code"])):
                 code_metadata[custom_concepts["code"][i]] = {
                     "description": custom_concepts["description"][i],
                     "parent_codes": [],
                 }
 
-    # Find and store the Concept ID's used for Birth and Death
-    omop_birth_concept_id = None
-    omop_death_concept_id = None
-    for concept_id, code in tqdm(concept_id_map.items(), desc="Finding birth and death codes"):
-        if code == meds.birth_code:
-            omop_birth_concept_id = concept_id
-        elif code == meds.death_code:
-            omop_death_concept_id = concept_id
-        if omop_birth_concept_id is not None and omop_death_concept_id is not None:
-            break
-
-    if omop_birth_concept_id is None or omop_death_concept_id is None:
-        raise ValueError(
-            "The provided OMOP dataset is missing either the birth or death concept. \n"
-            + "Look for SNOMED codes "
-            + meds.birth_code
-            + " and "
-            + meds.death_code
-            + " within concept.csv"
-        )
-
     # Include map from custom concepts to normalized (ie standard ontology)
     # parent concepts, where possible, in the code_metadata dictionary
-    for concept_relationship_file in get_table_files(path_to_src_omop_dir, "concept_relationship"):
+    for concept_relationship_file in itertools.chain(*get_table_files(path_to_src_omop_dir, "concept_relationship")):
         with load_file(path_to_decompressed_dir, concept_relationship_file) as f:
             # This table has `concept_id_1`, `concept_id_2`, `relationship_id` columns
-            concept_relationship = pl.read_csv(f.name)
+            concept_relationship = read_polars_df(f.name)
 
             concept_id_1 = pl.col("concept_id_1").cast(pl.Int64)
             concept_id_2 = pl.col("concept_id_2").cast(pl.Int64)
 
             custom_relationships = (
                 concept_relationship.filter(
                     concept_id_1 > CUSTOMER_CONCEPT_ID_START,
@@ -484,39 +503,39 @@
             ):
                 if concept_id_1 in concept_id_map and concept_id_2 in concept_id_map:
                     code_metadata[concept_id_map[concept_id_1]]["parent_codes"].append(concept_id_map[concept_id_2])
 
     # Extract dataset metadata e.g., the CDM source name and its release date
     datasets: List[str] = []
     dataset_versions: List[str] = []
-    for cdm_source_file in get_table_files(path_to_src_omop_dir, "cdm_source"):
+    for cdm_source_file in itertools.chain(*get_table_files(path_to_src_omop_dir, "cdm_source")):
         with load_file(path_to_decompressed_dir, cdm_source_file) as f:
-            cdm_source = pl.read_csv(f.name)
+            cdm_source = read_polars_df(f.name)
             cdm_source = cdm_source.rename({c: c.lower() for c in cdm_source.columns})
             cdm_source = cdm_source.to_dict(as_series=False)
 
             datasets.extend(cdm_source["cdm_source_name"])
             dataset_versions.extend(cdm_source["cdm_release_date"])
 
     metadata = {
         "dataset_name": "|".join(datasets),  # eg 'Epic Clarity SHC|Epic Clarity LPCH'
-        "dataset_version": "|".join(dataset_versions),  # eg '2024-02-01|2024-02-01'
+        "dataset_version": "|".join(str(a) for a in dataset_versions),  # eg '2024-02-01|2024-02-01'
         "etl_name": "meds_etl.omop",
         "etl_version": meds_etl.__version__,
         "code_metadata": code_metadata,  # `code_metadata` could have >100k keys
     }
     # At this point metadata['code_metadata']['STANFORD_MEAS/AMOXICILLIN/CLAVULANATE']
     # should give a dictionary like
     # {'description': 'AMOXICILLIN/CLAVULANATE', 'parent_codes': ['LOINC/18862-3']}
     # where LOINC Code '18862-3' is a standard concept representing a lab test
     # measurement determining microorganism susceptibility to Amoxicillin+clavulanic acid
 
     jsonschema.validate(instance=metadata, schema=meds.dataset_metadata)
 
-    return metadata, concept_id_map, concept_name_map, omop_birth_concept_id, omop_death_concept_id
+    return metadata, concept_id_map, concept_name_map
 
 
 def main():
     parser = argparse.ArgumentParser(prog="meds_etl_omop", description="Performs an ETL from OMOP v5 to MEDS")
     parser.add_argument(
         "path_to_src_omop_dir",
         type=str,
@@ -532,14 +551,20 @@
         default=100,
         help="Number of shards to use for converting MEDS from the flat format "
         "to MEDS (patients are distributed approximately uniformly at "
         "random across shards and collation/joining of OMOP tables is "
         "performed on a shard-by-shard basis).",
     )
     parser.add_argument("--num_proc", type=int, default=1, help="Number of vCPUs to use for performing the MEDS ETL")
+    parser.add_argument(
+        "--backend",
+        type=str,
+        default="polars",
+        help="The backend to use when performing an ETL. See the README for a discussion on possible backends.",
+    )
     parser.add_argument("--verbose", type=int, default=0)
     parser.add_argument(
         "--continue_job",
         dest="continue_job",
         action="store_true",
         help="If set, the job continues from a previous run, starting after the "
         "conversion to MEDS Flat but before converting from MEDS Flat to MEDS.",
@@ -580,15 +605,15 @@
             shutil.rmtree(path_to_decompressed_dir)
         os.mkdir(path_to_decompressed_dir)
 
         # # # # # # # # # # # # # # # # # # # # # # # # # #
         # Generate metadata.json from OMOP concept table  #
         # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-        metadata, concept_id_map, concept_name_map, omop_birth_concept_id, omop_death_concept_id = extract_metadata(
+        metadata, concept_id_map, concept_name_map = extract_metadata(
             path_to_src_omop_dir=args.path_to_src_omop_dir,
             path_to_decompressed_dir=path_to_decompressed_dir,
             verbose=args.verbose,
         )
 
         # Save the extracted metadata file to disk...
         # We save one copy in the MEDS Flat data directory
@@ -598,21 +623,19 @@
         with open(os.path.join(args.path_to_dest_meds_dir, "metadata.json"), "w") as f:
             json.dump(metadata, f)
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
         # Convert all "measurements" to MEDS Flat, write to disk  #
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-        # tables = retrieve_table_specifications(omop_birth_concept_id)
-
         tables: Dict[str, Any] = {
             # Each key is a `table_name`
             "person": [  # `table_name`s map to `table_details`
                 {
-                    "force_concept_id": omop_birth_concept_id,
+                    "force_concept_code": meds.birth_code,
                 },
                 {
                     "concept_id_field": "gender_concept_id",
                 },
                 {
                     "concept_id_field": "race_concept_id",
                 },
@@ -624,15 +647,15 @@
                 "concept_id_field": "drug_concept_id",
             },
             "visit": {"fallback_concept_id": DEFAULT_VISIT_CONCEPT_ID, "file_suffix": "occurrence"},
             "condition": {
                 "file_suffix": "occurrence",
             },
             "death": {
-                "force_concept_id": omop_death_concept_id,
+                "force_concept_code": meds.death_code,
             },
             "procedure": {
                 "file_suffix": "occurrence",
             },
             "device_exposure": {
                 "concept_id_field": "device_concept_id",
             },
@@ -660,52 +683,75 @@
         concept_id_map_data = pickle.dumps(concept_id_map)
         concept_name_map_data = pickle.dumps(concept_name_map)
 
         # Create a separate task for each table
         # Each subprocess will read in a decompressed file and put all measurements for a given patient
         # into that patient's corresponding shard. This makes creating patient timelines downstream
         # (where timelines incorporate measurements from across different tables) much less RAM intensive.
-        all_tasks = []
+        all_csv_tasks = []
+        all_parquet_tasks = []
         for table_name, table_details in tables.items():
-            table_files = get_table_files(
+            csv_table_files, parquet_table_files = get_table_files(
                 path_to_src_omop_dir=args.path_to_src_omop_dir,
                 table_name=table_name,
                 table_details=table_details[0] if isinstance(table_details, list) else table_details,
             )
 
-            all_tasks.extend(
+            all_csv_tasks.extend(
                 (
                     table_file,
                     table_name,
                     table_details,
                     concept_id_map_data,
                     concept_name_map_data,
                     path_to_MEDS_flat_dir,
                     path_to_decompressed_dir,
-                    map_index,
                     args.verbose,
                 )
-                for map_index, table_file in enumerate(table_files)
+                for table_file in csv_table_files
             )
-        random.seed(RANDOM_SEED)
-        random.shuffle(all_tasks)
+
+            all_parquet_tasks.extend(
+                (
+                    table_files,
+                    table_name,
+                    table_details,
+                    concept_id_map_data,
+                    concept_name_map_data,
+                    path_to_MEDS_flat_dir,
+                    args.verbose,
+                )
+                for table_files in split_list(parquet_table_files, args.num_shards)
+            )
+
+        rng = random.Random(RANDOM_SEED)
+        rng.shuffle(all_csv_tasks)
+        rng.shuffle(all_parquet_tasks)
 
         print("Decompressing OMOP tables, mapping to MEDS Flat format, writing to disk...")
         if args.num_proc > 1:
-            with multiprocessing.get_context("spawn").Pool(args.num_proc, maxtasksperchild=1) as pool:
+            with multiprocessing.get_context("spawn").Pool(args.num_proc) as pool:
                 # Wrap all tasks with tqdm for a progress bar
-                total_tasks = len(all_tasks)
-                with tqdm(total=total_tasks, desc="Mapping OMOP tables -> MEDS format") as pbar:
-                    for _ in pool.imap_unordered(process_table, all_tasks):
+                total_tasks = len(all_csv_tasks)
+                with tqdm(total=total_tasks, desc="Mapping CSV OMOP tables -> MEDS format") as pbar:
+                    for _ in pool.imap_unordered(process_table_csv, all_csv_tasks):
+                        pbar.update()
+
+                total_tasks = len(all_parquet_tasks)
+                with tqdm(total=total_tasks, desc="Mapping Parquet OMOP tables -> MEDS format") as pbar:
+                    for _ in pool.imap_unordered(process_table_parquet, all_parquet_tasks):
                         pbar.update()
 
         else:
             # Useful for debugging `process_table` without multiprocessing
-            for task in tqdm(all_tasks):
-                process_table(task)
+            for task in tqdm(all_csv_tasks):
+                process_table_csv(task)
+
+            for task in tqdm(all_parquet_tasks):
+                process_table_parquet(task)
 
         # TODO: Do we need to do this more often so as to reduce maximum disk storage?
         shutil.rmtree(path_to_decompressed_dir)
 
         print("Finished converting dataset to MEDS Flat.")
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
@@ -714,14 +760,15 @@
 
     print("Converting from MEDS Flat to MEDS...")
     meds_etl.flat.convert_flat_to_meds(
         source_flat_path=path_to_temp_dir,
         target_meds_path=os.path.join(args.path_to_dest_meds_dir, "result"),
         num_shards=args.num_shards,
         num_proc=args.num_proc,
+        backend=args.backend,
     )
     print("...finished converting MEDS Flat to MEDS")
     shutil.move(
         src=os.path.join(args.path_to_dest_meds_dir, "result", "data"),
         dst=os.path.join(args.path_to_dest_meds_dir, "data"),
     )
     shutil.rmtree(path=os.path.join(args.path_to_dest_meds_dir, "result"))
```

### Comparing `meds_etl-0.1.1/src/meds_etl.egg-info/PKG-INFO` & `meds_etl-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: meds_etl
-Version: 0.1.1
+Version: 0.2.0
 Summary: A data standard for working with event stream data
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow>=8
 Requires-Dist: polars>=0.20.10
 Requires-Dist: jsonschema>=4.0.0
-Requires-Dist: meds==0.1.3
+Requires-Dist: meds==0.2.0
 Requires-Dist: typing_extensions>=4.0
 Requires-Dist: datasets>=2.0.0
 Requires-Dist: tqdm>=4.6.0
+Requires-Dist: psutil>=5.9.0
+Provides-Extra: duckdb
+Requires-Dist: duckdb>=0.10.1; extra == "duckdb"
+Provides-Extra: cpp
+Requires-Dist: meds_etl_cpp==0.2.0; extra == "cpp"
 
 # meds_etl
 
 A collection of ETLs from common data formats to Medical Event Data Standard (MEDS)
 
 This package library currently supports:
 
@@ -26,15 +31,38 @@
 ## Setup
 Create an environment of your choice:
 ```bash
 conda create -n meds_etl
 ```
 Install the package
 ```bash
-python -m pip install .
+pip install meds_etl
+```
+
+## Backends
+
+ETLs are one of the most computationally heavy components of MEDS, so efficiency is very important.
+
+MEDS-ETL has several parallel implementations of core algorithms to balance the tradeoff between efficiency and ease of use.
+
+All commands generally take an additional parameter --backend, that allows users to switch between different backends.
+
+We currently support two backends: polars (the default) and cpp.
+
+Backend information:
+
+- polars (default backend): A Python only implementation that only requires polars to run. The main issue with this implementation is that it is rather inefficient. It's recommended to use as few shards as possible while still avoiding out of memory errors.
+
+- cpp: A custom C++ backend. This backend is very efficient, but might not run on all platforms and has a limited feature set. It's recommended to use the same number of shards as you have CPUs available.
+
+If you want to use either the cpp backend, make sure to install meds_etl with the correct optional dependencies.
+
+```bash
+# For the cpp backend
+pip install "meds_etl[cpp]"
 ```
 
 ## MIMIC-IV
 
 In order to run the MIMIC-IV ETL, simply run the following command:
 
 ```bash
```

### Comparing `meds_etl-0.1.1/src/meds_etl.egg-info/SOURCES.txt` & `meds_etl-0.2.0/src/meds_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meds_etl-0.1.1/tests/test_etl.py` & `meds_etl-0.2.0/tests/test_etl.py`

 * *Files identical despite different names*

