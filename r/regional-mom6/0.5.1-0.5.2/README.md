# Comparing `tmp/regional_mom6-0.5.1.tar.gz` & `tmp/regional_mom6-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regional_mom6-0.5.1.tar", last modified: Tue Apr 30 13:06:49 2024, max compression
+gzip compressed data, was "regional_mom6-0.5.2.tar", last modified: Sat May  4 19:13:14 2024, max compression
```

## Comparing `regional_mom6-0.5.1.tar` & `regional_mom6-0.5.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.748345 regional_mom6-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/common_files/
--rwxr-xr-x   0 runner    (1001) docker     (127)    44918 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_input
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_layout
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_override
--rwxr-xr-x   0 runner    (1001) docker     (127)     1321 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/SIS_input
--rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      912 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/data_table
--rwxr-xr-x   0 runner    (1001) docker     (127)     3255 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/diag_table
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/field_table
--rwxr-xr-x   0 runner    (1001) docker     (127)     1398 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/common_files/input.nml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1264 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/data_table
--rwxr-xr-x   0 runner    (1001) docker     (127)     1436 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/input.nml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.752345 regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1340 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/data_table
--rw-r--r--   0 runner    (1001) docker     (127)   121257 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/demos/reanalysis-forced.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/mom6-file-structure-primer.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/regional_mom6/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/regional_mom6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    83821 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/regional_mom6/regional_mom6.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/regional_mom6/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/regional_mom6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 13:06:49.000000 regional_mom6-0.5.1/regional_mom6.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:06:49.756345 regional_mom6-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/tests/test_expt_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/tests/test_grid_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 13:06:44.000000 regional_mom6-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.734573 regional_mom6-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.726573 regional_mom6-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.726573 regional_mom6-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-04 19:13:14.734573 regional_mom6-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.726573 regional_mom6-0.5.2/demos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.730573 regional_mom6-0.5.2/demos/premade_run_directories/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.730573 regional_mom6-0.5.2/demos/premade_run_directories/common_files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45005 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/MOM_input
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/MOM_layout
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/MOM_override
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1321 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/SIS_input
+-rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      912 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/data_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3255 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/diag_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/field_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1398 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/common_files/input.nml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.730573 regional_mom6-0.5.2/demos/premade_run_directories/era5_surface/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1264 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/era5_surface/data_table
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1436 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/era5_surface/input.nml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.730573 regional_mom6-0.5.2/demos/premade_run_directories/jra_surface/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/jra_surface/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1340 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/premade_run_directories/jra_surface/data_table
+-rw-r--r--   0 runner    (1001) docker     (127)   121257 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/demos/reanalysis-forced.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.730573 regional_mom6-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/mom6-file-structure-primer.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.734573 regional_mom6-0.5.2/regional_mom6/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/regional_mom6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-04 19:13:14.000000 regional_mom6-0.5.2/regional_mom6/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83821 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/regional_mom6/regional_mom6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/regional_mom6/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.734573 regional_mom6-0.5.2/regional_mom6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-04 19:13:14.000000 regional_mom6-0.5.2/regional_mom6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-04 19:13:14.000000 regional_mom6-0.5.2/regional_mom6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:13:14.000000 regional_mom6-0.5.2/regional_mom6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-04 19:13:14.000000 regional_mom6-0.5.2/regional_mom6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 19:13:14.000000 regional_mom6-0.5.2/regional_mom6.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:13:14.734573 regional_mom6-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:13:14.734573 regional_mom6-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/tests/test_expt_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/tests/test_grid_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-04 19:13:11.000000 regional_mom6-0.5.2/tests/test_utils.py
```

### Comparing `regional_mom6-0.5.1/.github/workflows/package.yml` & `regional_mom6-0.5.2/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/.github/workflows/testing.yml` & `regional_mom6-0.5.2/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/.readthedocs.yaml` & `regional_mom6-0.5.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/LICENSE` & `regional_mom6-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/PKG-INFO` & `regional_mom6-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regional_mom6
-Version: 0.5.1
+Version: 0.5.2
 Summary: Automatic generation of regional configurations for Modular Ocean Model v6
 Author: COSIMA community and outside contributors
 Keywords: mom6,regional,ocean modeling,python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bottleneck
 Requires-Dist: dask[array]
```

### Comparing `regional_mom6-0.5.1/README.md` & `regional_mom6-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/README.md` & `regional_mom6-0.5.2/demos/premade_run_directories/README.md`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_input` & `regional_mom6-0.5.2/demos/premade_run_directories/common_files/MOM_input`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                                 !     Kelvin - flat but with rotated land mask.
                                 !     seamount - Gaussian bump for spontaneous motion test case.
                                 !     dumbbell - Sloshing channel with reservoirs on both ends.
                                 !     shelfwave - exponential slope for shelfwave test case.
                                 !     Phillips - ACC-like idealized topography used in the Phillips config.
                                 !     dense - Denmark Strait-like dense water formation and overflow.
                                 !     USER - call a user modified routine.
+TOPO_FILE = "bathymetry.nc"     ! Name of the file containing bathymetry information. 
 MINIMUM_DEPTH = 4.5             !   [m] default = 0.0
                                 ! If MASKING_DEPTH is unspecified, then anything shallower than MINIMUM_DEPTH is
                                 ! assumed to be land and all fluxes are masked out. If MASKING_DEPTH is
                                 ! specified, then all depths shallower than MINIMUM_DEPTH but deeper than
                                 ! MASKING_DEPTH are rounded to MINIMUM_DEPTH.
 MAXIMUM_DEPTH = 6000.0          !   [m]
                                 ! The maximum depth of the ocean.
```

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/common_files/MOM_layout` & `regional_mom6-0.5.2/demos/premade_run_directories/common_files/MOM_layout`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/common_files/SIS_input` & `regional_mom6-0.5.2/demos/premade_run_directories/common_files/SIS_input`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/common_files/data_table` & `regional_mom6-0.5.2/demos/premade_run_directories/common_files/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/common_files/diag_table` & `regional_mom6-0.5.2/demos/premade_run_directories/common_files/diag_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/common_files/input.nml` & `regional_mom6-0.5.2/demos/premade_run_directories/common_files/input.nml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/data_table` & `regional_mom6-0.5.2/demos/premade_run_directories/era5_surface/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/era5_surface/input.nml` & `regional_mom6-0.5.2/demos/premade_run_directories/era5_surface/input.nml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/premade_run_directories/jra_surface/data_table` & `regional_mom6-0.5.2/demos/premade_run_directories/jra_surface/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/demos/reanalysis-forced.ipynb` & `regional_mom6-0.5.2/demos/reanalysis-forced.ipynb`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/docs/Makefile` & `regional_mom6-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/docs/conf.py` & `regional_mom6-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/docs/contributing.md` & `regional_mom6-0.5.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/docs/index.rst` & `regional_mom6-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/docs/installation.md` & `regional_mom6-0.5.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/docs/mom6-file-structure-primer.md` & `regional_mom6-0.5.2/docs/mom6-file-structure-primer.md`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/pyproject.toml` & `regional_mom6-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/regional_mom6/regional_mom6.py` & `regional_mom6-0.5.2/regional_mom6/regional_mom6.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/regional_mom6/utils.py` & `regional_mom6-0.5.2/regional_mom6/utils.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/regional_mom6.egg-info/PKG-INFO` & `regional_mom6-0.5.2/regional_mom6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regional_mom6
-Version: 0.5.1
+Version: 0.5.2
 Summary: Automatic generation of regional configurations for Modular Ocean Model v6
 Author: COSIMA community and outside contributors
 Keywords: mom6,regional,ocean modeling,python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bottleneck
 Requires-Dist: dask[array]
```

### Comparing `regional_mom6-0.5.1/regional_mom6.egg-info/SOURCES.txt` & `regional_mom6-0.5.2/regional_mom6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/tests/test_expt_class.py` & `regional_mom6-0.5.2/tests/test_expt_class.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/tests/test_grid_generation.py` & `regional_mom6-0.5.2/tests/test_grid_generation.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.5.1/tests/test_utils.py` & `regional_mom6-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

