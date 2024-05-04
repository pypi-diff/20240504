# Comparing `tmp/specsy-0.2.3.tar.gz` & `tmp/specsy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsy-0.2.3.tar", last modified: Sat May  4 19:11:54 2024, max compression
+gzip compressed data, was "specsy-0.2.4.tar", last modified: Sat May  4 19:27:42 2024, max compression
```

## Comparing `specsy-0.2.3.tar` & `specsy-0.2.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.453599 specsy-0.2.3/
--rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.3/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:11:54.453599 specsy-0.2.3/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.3/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1227 2024-05-04 19:10:48.000000 specsy-0.2.3/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-04 19:11:54.453599 specsy-0.2.3/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1535 2024-04-29 22:29:38.000000 specsy-0.2.3/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.445599 specsy-0.2.3/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/
--rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.3/src/specsy/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-04 19:10:48.000000 specsy-0.2.3/src/specsy/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/core.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/inference/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/inference/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/inference/emission.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/innate/
--rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/innate/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/innate/interpol_pytensor.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3830 2024-05-03 19:46:25.000000 specsy-0.2.3/src/specsy/innate/main.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12911 2024-05-03 20:35:46.000000 specsy-0.2.3/src/specsy/io.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/models/
--rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17030 2024-05-03 21:54:50.000000 specsy-0.2.3/src/specsy/models/chemistry.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.3/src/specsy/models/chemistry_inference.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.3/src/specsy/models/emissivity.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/extinction.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/fluxes_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/nebular_continuum.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/operations/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/interpolation.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/pytensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/tensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/tests.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/plots.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.453599 specsy-0.2.3/src/specsy/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/resources/HI_t3_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/HeII_t4_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/HeI_t5_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/gordon_2003_LMC2_supershell.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/gordon_2003_LMC_average.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/gordon_2003_SMC_bar.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/treatement.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.453599 specsy-0.2.3/src/specsy/workflow/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/workflow/__init__.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      277 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.922909 specsy-0.2.4/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.4/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:27:42.922909 specsy-0.2.4/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.4/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1227 2024-05-04 19:27:10.000000 specsy-0.2.4/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-04 19:27:42.922909 specsy-0.2.4/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1535 2024-04-29 22:29:38.000000 specsy-0.2.4/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.918909 specsy-0.2.4/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.918909 specsy-0.2.4/src/specsy/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.4/src/specsy/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-04 19:27:10.000000 specsy-0.2.4/src/specsy/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/core.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.918909 specsy-0.2.4/src/specsy/inference/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/inference/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/inference/emission.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.918909 specsy-0.2.4/src/specsy/innate/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/innate/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/innate/interpol_pytensor.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3830 2024-05-03 19:46:25.000000 specsy-0.2.4/src/specsy/innate/main.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12911 2024-05-04 19:21:02.000000 specsy-0.2.4/src/specsy/io.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.922909 specsy-0.2.4/src/specsy/models/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/models/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17030 2024-05-03 21:54:50.000000 specsy-0.2.4/src/specsy/models/chemistry.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.4/src/specsy/models/chemistry_inference.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.4/src/specsy/models/emissivity.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/models/extinction.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/models/fluxes_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/models/nebular_continuum.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.922909 specsy-0.2.4/src/specsy/operations/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/operations/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/operations/interpolation.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/operations/pytensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/operations/tensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/operations/tests.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/plots.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.922909 specsy-0.2.4/src/specsy/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.4/src/specsy/resources/HI_t3_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/resources/HeII_t4_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/resources/HeI_t5_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/resources/gordon_2003_LMC2_supershell.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/resources/gordon_2003_LMC_average.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/resources/gordon_2003_SMC_bar.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/treatement.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.922909 specsy-0.2.4/src/specsy/workflow/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.4/src/specsy/workflow/__init__.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:27:42.918909 specsy-0.2.4/src/specsy.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:27:42.000000 specsy-0.2.4/src/specsy.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-04 19:27:42.000000 specsy-0.2.4/src/specsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 19:27:42.000000 specsy-0.2.4/src/specsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      277 2024-05-04 19:27:42.000000 specsy-0.2.4/src/specsy.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-04 19:27:42.000000 specsy-0.2.4/src/specsy.egg-info/top_level.txt
```

### Comparing `specsy-0.2.3/PKG-INFO` & `specsy-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.3/README.rst` & `specsy-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/pyproject.toml` & `specsy-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "specsy"
-version = "0.2.3"
+version = "0.2.4"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Model fitting package for the chemical analysis of astronomical spectra"
 dependencies = ["arviz~=0.18",
                 "astropy~=6.0",
```

### Comparing `specsy-0.2.3/setup.py` & `specsy-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/__init__.py` & `specsy-0.2.4/src/specsy/__init__.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/config.toml` & `specsy-0.2.4/src/specsy/config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'specsy'
-version = '0.2.3'
+version = '0.2.4'
 
 [direct_method_cfg]
 temp_zones.high = ["He1", "He2", "O3", "Ar4", "Ne3", "Cl4", "C3"]
 temp_zones.low  = ["H1", "Ar3", "S2", "S3", "N2", "O2", "Fe3", "C2"]
 parameter_list = ["n_e", "T_low", "T_high", "cHbeta", "tau", "Ar3", "Ar4", "N2", "O2", "O3", "S2", "S3", "He1", "He2",
                   "Cl3","Ne3","Fe3","Teff","logU"]
 temp_low_diag = ['S3_6312A']
```

### Comparing `specsy-0.2.3/src/specsy/core.py` & `specsy-0.2.4/src/specsy/core.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/inference/emission.py` & `specsy-0.2.4/src/specsy/inference/emission.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/innate/interpol_pytensor.py` & `specsy-0.2.4/src/specsy/innate/interpol_pytensor.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/innate/main.py` & `specsy-0.2.4/src/specsy/innate/main.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/io.py` & `specsy-0.2.4/src/specsy/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
                norm_line=None):
 
     # Return
     log = lime.load_frame(file_address, page, sample_levels)
 
     # Create new column for the lines flux with the requested type (None for user to introduce "line_flux")
     if flux_type is not None:
-        lime.tools.extract_fluxes(log, flux_type=flux_type, column_name='line_flux')
+        lime.tools.extract_fluxes(log, flux_type=flux_type, column_name='line_extract')
 
     # Check for requested lines and their normalization
     if norm_line is not None:
-        log = lime.tools.normalize_fluxes(log, lines_list, norm_line, flux_column='line_flux', column_name='line_flux')
+        lime.tools.normalize_fluxes(log, lines_list, norm_line, flux_column='line_extract', column_name='line_flux')
 
     return log
 
 
 def load_HII_CHI_MISTRY_grid(log_scale=False, log_zero_value = -1000):
 
     # grid_file = 'D:/Dropbox/Astrophysics/Tools/HCm-Teff_v5.01/C17_bb_Teff_30-90_pp.dat'
```

### Comparing `specsy-0.2.3/src/specsy/models/chemistry.py` & `specsy-0.2.4/src/specsy/models/chemistry.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/models/chemistry_inference.py` & `specsy-0.2.4/src/specsy/models/chemistry_inference.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/models/emissivity.py` & `specsy-0.2.4/src/specsy/models/emissivity.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/models/extinction.py` & `specsy-0.2.4/src/specsy/models/extinction.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/models/fluxes_line.py` & `specsy-0.2.4/src/specsy/models/fluxes_line.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/models/nebular_continuum.py` & `specsy-0.2.4/src/specsy/models/nebular_continuum.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/operations/interpolation.py` & `specsy-0.2.4/src/specsy/operations/interpolation.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/operations/pytensors.py` & `specsy-0.2.4/src/specsy/operations/pytensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/operations/tensors.py` & `specsy-0.2.4/src/specsy/operations/tensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/operations/tests.py` & `specsy-0.2.4/src/specsy/operations/tests.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/plots.py` & `specsy-0.2.4/src/specsy/plots.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/resources/HI_t3_elec.ascii` & `specsy-0.2.4/src/specsy/resources/HI_t3_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/resources/HeII_t4_elec.ascii` & `specsy-0.2.4/src/specsy/resources/HeII_t4_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/resources/HeI_t5_elec.ascii` & `specsy-0.2.4/src/specsy/resources/HeI_t5_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/tools.py` & `specsy-0.2.4/src/specsy/tools.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy/treatement.py` & `specsy-0.2.4/src/specsy/treatement.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.3/src/specsy.egg-info/PKG-INFO` & `specsy-0.2.4/src/specsy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.3/src/specsy.egg-info/SOURCES.txt` & `specsy-0.2.4/src/specsy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

