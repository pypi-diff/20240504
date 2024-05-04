# Comparing `tmp/specsy-0.2.2.tar.gz` & `tmp/specsy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsy-0.2.2.tar", last modified: Mon Apr 29 22:53:50 2024, max compression
+gzip compressed data, was "specsy-0.2.3.tar", last modified: Sat May  4 19:11:54 2024, max compression
```

## Comparing `specsy-0.2.2.tar` & `specsy-0.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/
--rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.2/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-04-29 22:53:50.954835 specsy-0.2.2/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.2/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1228 2024-04-29 22:49:42.000000 specsy-0.2.2/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-04-29 22:53:50.954835 specsy-0.2.2/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1535 2024-04-29 22:29:38.000000 specsy-0.2.2/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/
--rw-rw-r--   0 vital     (1000) vital     (1000)      878 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-04-29 22:49:42.000000 specsy-0.2.2/src/specsy/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/core.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/inference/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/inference/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/inference/emission.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/innate/
--rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/innate/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/innate/interpol_pytensor.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3795 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/innate/main.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12905 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/io.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/models/
--rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/models/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16099 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/models/chemistry.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     5282 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/models/chemistry_inference.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.2/src/specsy/models/emissivity.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/models/extinction.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/models/fluxes_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/models/nebular_continuum.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/operations/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/operations/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/operations/interpolation.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/operations/pytensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/operations/tensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/operations/tests.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/plots.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.2/src/specsy/resources/HI_t3_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/resources/HeII_t4_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/resources/HeI_t5_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/resources/gordon_2003_LMC2_supershell.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/resources/gordon_2003_LMC_average.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/resources/gordon_2003_SMC_bar.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/treatement.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy/workflow/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.2/src/specsy/workflow/__init__.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 22:53:50.954835 specsy-0.2.2/src/specsy.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-04-29 22:53:50.000000 specsy-0.2.2/src/specsy.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-04-29 22:53:50.000000 specsy-0.2.2/src/specsy.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-29 22:53:50.000000 specsy-0.2.2/src/specsy.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      277 2024-04-29 22:53:50.000000 specsy-0.2.2/src/specsy.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-04-29 22:53:50.000000 specsy-0.2.2/src/specsy.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.453599 specsy-0.2.3/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.3/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:11:54.453599 specsy-0.2.3/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.3/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1227 2024-05-04 19:10:48.000000 specsy-0.2.3/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-04 19:11:54.453599 specsy-0.2.3/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1535 2024-04-29 22:29:38.000000 specsy-0.2.3/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.445599 specsy-0.2.3/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.3/src/specsy/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-04 19:10:48.000000 specsy-0.2.3/src/specsy/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/core.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/inference/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/inference/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/inference/emission.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/innate/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/innate/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/innate/interpol_pytensor.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3830 2024-05-03 19:46:25.000000 specsy-0.2.3/src/specsy/innate/main.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12911 2024-05-03 20:35:46.000000 specsy-0.2.3/src/specsy/io.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/models/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17030 2024-05-03 21:54:50.000000 specsy-0.2.3/src/specsy/models/chemistry.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.3/src/specsy/models/chemistry_inference.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17176 2024-04-29 21:57:45.000000 specsy-0.2.3/src/specsy/models/emissivity.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    22583 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/extinction.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/fluxes_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/models/nebular_continuum.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy/operations/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/interpolation.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/pytensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/tensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/operations/tests.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/plots.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.453599 specsy-0.2.3/src/specsy/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.3/src/specsy/resources/HI_t3_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/HeII_t4_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/HeI_t5_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/gordon_2003_LMC2_supershell.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/gordon_2003_LMC_average.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/resources/gordon_2003_SMC_bar.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10339 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/treatement.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.453599 specsy-0.2.3/src/specsy/workflow/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.3/src/specsy/workflow/__init__.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:11:54.449599 specsy-0.2.3/src/specsy.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      277 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-04 19:11:54.000000 specsy-0.2.3/src/specsy.egg-info/top_level.txt
```

### Comparing `specsy-0.2.2/PKG-INFO` & `specsy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.2/README.rst` & `specsy-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/pyproject.toml` & `specsy-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [project]
 name = "specsy"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Model fitting package for the chemical analysis of astronomical spectra"
-
 dependencies = ["arviz~=0.18",
                 "astropy~=6.0",
                 "corner~=2.2",
                 "h5netcdf~=1.3.0",
                 "jax~=0.4",
                 "jaxlib==0.4.26",
                 "lime-stable~=1.0",
```

### Comparing `specsy-0.2.2/setup.py` & `specsy-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/__init__.py` & `specsy-0.2.3/src/specsy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,13 +18,15 @@
 
 # Read lime configuration .toml
 _inst_dir = Path(__file__).parent
 _conf_path = _inst_dir/'config.toml'
 with open(_conf_path, mode="rb") as fp:
     _setup_cfg = tomllib.load(fp)
 
+__version__ = _setup_cfg['metadata']['version']
+
 from .io import label_decomposition, load_frame, save_frame, load_cfg, save_cfg
 from .tools import flux_distribution
 from .innate import Innate, load_inference_data, save_inference_data
 from .treatement import SpectraSynthesizer, ChemicalModel
 from .plots import theme
 from .models import *
```

### Comparing `specsy-0.2.2/src/specsy/config.toml` & `specsy-0.2.3/src/specsy/config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'specsy'
-version = '0.2.2'
+version = '0.2.3'
 
 [direct_method_cfg]
 temp_zones.high = ["He1", "He2", "O3", "Ar4", "Ne3", "Cl4", "C3"]
 temp_zones.low  = ["H1", "Ar3", "S2", "S3", "N2", "O2", "Fe3", "C2"]
 parameter_list = ["n_e", "T_low", "T_high", "cHbeta", "tau", "Ar3", "Ar4", "N2", "O2", "O3", "S2", "S3", "He1", "He2",
                   "Cl3","Ne3","Fe3","Teff","logU"]
 temp_low_diag = ['S3_6312A']
```

### Comparing `specsy-0.2.2/src/specsy/core.py` & `specsy-0.2.3/src/specsy/core.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/inference/emission.py` & `specsy-0.2.3/src/specsy/inference/emission.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/innate/interpol_pytensor.py` & `specsy-0.2.3/src/specsy/innate/interpol_pytensor.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/innate/main.py` & `specsy-0.2.3/src/specsy/innate/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         # Object attributes
         self.grid = None
         self.interpl = None
         self.lib_interpl = None
         self.x_range, self.y_range = None, None
 
         # Initiate data and interpolators # TODO Better check
-        self.grid = load_grids(grid) if Path(grid).is_file() else grid
+        grid_path = Path(grid)
+        self.grid = load_grids(grid_path) if grid_path.is_file() else grid
 
         if interpolators is not None:
 
             print(f'\n- Compiling {interpolators} interpolators')
 
             if interpolators == 'pytensor':
                 self.lib_interpl = interpolators
```

### Comparing `specsy-0.2.2/src/specsy/io.py` & `specsy-0.2.3/src/specsy/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Create new column for the lines flux with the requested type (None for user to introduce "line_flux")
     if flux_type is not None:
         lime.tools.extract_fluxes(log, flux_type=flux_type, column_name='line_flux')
 
     # Check for requested lines and their normalization
     if norm_line is not None:
-        lime.tools.normalize_fluxes(log, lines_list, norm_line, flux_column='line_flux', column_name='line_flux')
+        log = lime.tools.normalize_fluxes(log, lines_list, norm_line, flux_column='line_flux', column_name='line_flux')
 
     return log
 
 
 def load_HII_CHI_MISTRY_grid(log_scale=False, log_zero_value = -1000):
 
     # grid_file = 'D:/Dropbox/Astrophysics/Tools/HCm-Teff_v5.01/C17_bb_Teff_30-90_pp.dat'
```

### Comparing `specsy-0.2.2/src/specsy/models/chemistry.py` & `specsy-0.2.3/src/specsy/models/chemistry.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,14 +178,47 @@
 
     # Abundance calculation
     S_H = k1 + k2 * np.log10(S23) + k3 * np.power(np.log10(S23), 2)
 
     return np.mean(S_H), np.std(S_H)
 
 
+def TSIII_from_TOIII_relation(T_high):
+    # From Hagele et al 2006
+    return (1.19 * T_high / 10000.0 - 0.32) * 10000.0
+
+def direct_temp():
+
+    return
+
+
+METHODS_DICT = {'Hagele_2006': TSIII_from_TOIII_relation}
+
+
+def assign_temperature_diagnostic(line_list, diagnostic, temp_assign = True):
+
+    # Check if the mathod is in the library:
+    if diagnostic[0] in METHODS_DICT.keys():
+        diag_func = METHODS_DICT[diagnostic[0]]
+
+    # Confirm is a line:
+    else:
+        try:
+            line = lime.Line(diagnostic[0])
+            diag_func = diagnostic[0]
+        except:
+            raise KeyError(f'Input diagnostic {diagnostic[0]} is not recognized by Specsy')
+
+        if np.any(np.isin(diagnostic[0], line_list)):
+            diag_func = diagnostic[0]
+        else:
+            raise KeyError(f'Input diagnostic line {diagnostic[0]} is not available in observation')
+
+    return diag_func
+
 
 class DmInputs:
 
     def __init__(self, lines_frame, lines_list=None, ext_frame='FRAME', R_v=None, extinction_law=None):
 
         # Attributes
         self.frame = None
@@ -197,15 +230,16 @@
         self.particles = None
 
         # Review the inputs
         self.frame = lime.io.check_file_dataframe(lines_frame, DataFrame, ext=ext_frame)
 
         # Crop to the target lines
         if lines_list is not None:
-            self.frame = self.frame.index.isin(lines_list)
+            idcs = self.frame.index.isin(lines_list)
+            self.frame = self.frame.loc[idcs]
 
         # Declare the inputs
         self.lines = self.frame.index.to_numpy()
         self.particles = self.frame.particle.to_numpy()
         self.fluxes = self.frame.line_flux.to_numpy()
         self.errs = self.frame.line_flux_err.to_numpy()
         self.wave = self.frame.wavelength.to_numpy()
@@ -274,40 +308,39 @@
 
         # Prepare the input data for the fitting
         inputs = DmInputs(lines_frame, lines_list, R_v=self._model.R_v, extinction_law=self._model.extinction_law)
         inputs.review_model(self._model.emiss_grids, self._model.prior_conf, self._model.temp_zones, verbose)
 
         # Prepare auxiliary parameters
         idcs_highTemp_ions = np.isin(inputs.particles, self._model.temp_zones['high'])
-        lowTemp_check = np.any(np.isin(self._model.temp_low_diag, inputs.lines))
-        highTemp_check = np.any(np.isin(self._model.temp_high_diag, inputs.lines))
+        lowTemp_check = assign_temperature_diagnostic(inputs.lines, self._model.temp_low_diag)
+        highTemp_check = assign_temperature_diagnostic(inputs.lines, self._model.temp_high_diag)
 
-        # Confirm all data is available
-        if lowTemp_check or highTemp_check:
-
-            # Output file
-            fname = self.output_path/f'{self.label_fit}_inference_data.nc'
-            print(f'\n- Launching direct method inference: ')
-
-            # Run the model
-            infer_data = direct_method_inference(fname, inputs,
-                                    prior_dict=self._model.prior_conf, idcs_highTemp_ions=idcs_highTemp_ions,
-                                    emiss_interp=self._model.emiss_grids.interpl, eq_tt=self._model.eq_tt,
-                                    fit_Tlow=lowTemp_check, fit_Thigh=highTemp_check)
-
-            # Save the output data
-            output_db = self.output_path / f'{self.label_fit}_infer_db.nc'
-            print(f'-- done, saving the results at: {output_db}')
-            self.package_results(output_db, infer_data, inputs, self._model.prior_conf, true_values=true_values)
-
-        else:
-            msg = (f'\n- The observation does not have temperature diagnostics:'
-                   f'\n-- Low temperature diagnostics: {self._model.temp_low_diag}',
-                   f'\n-- High temperature diagnostics: {self._model.temp_high_diag}')
-            print(msg)
+        # Output file
+        fname = self.output_path/f'{self.label_fit}_inference_data.nc'
+        print(f'\n- Launching direct method inference: ')
+
+        # Run the model
+        infer_data = direct_method_inference(fname, inputs, prior_dict=self._model.prior_conf, idcs_highTemp_ions=idcs_highTemp_ions,
+                                            emiss_interp=self._model.emiss_grids.interpl, eq_tt=self._model.eq_tt,
+                                            Tlow_diag=lowTemp_check, Thigh_diag=highTemp_check)
+
+        # Save the output data
+        output_db = self.output_path / f'{self.label_fit}_infer_db.nc'
+        print(f'-- done, saving the results at: {output_db}')
+        self.package_results(output_db, infer_data, inputs, self._model.prior_conf, true_values=true_values)
+
+
+        # # Confirm all data is available
+        # if lowTemp_check or highTemp_check:
+        # else:
+        #     msg = (f'\n- The observation does not have temperature diagnostics:'
+        #            f'\n-- Low temperature diagnostics: {self._model.temp_low_diag}',
+        #            f'\n-- High temperature diagnostics: {self._model.temp_high_diag}')
+        #     print(msg)
 
         return
 
     def package_results(self, fname, inference_data, inputs=None, prior_dict=None, true_values=None):
 
         # First save it just in case
         az.to_netcdf(inference_data, fname)
```

### Comparing `specsy-0.2.2/src/specsy/models/chemistry_inference.py` & `specsy-0.2.3/src/specsy/models/chemistry_inference.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,35 +34,53 @@
 
     else:
         priorFunc = probDist(param, dist_norm, dist_scale, shape=total_regions) * dist_norm + dist_reLoc
 
     return priorFunc
 
 
-def temperature_selection(self, fit_T_low=True, fit_T_high=True):
-
-    if self.lowTemp_check and fit_T_low:
-        self.set_prior('T_low')
-
-        if self.highTemp_check:
-            self.set_prior('T_high')
-        else:
-            self.prior_vars['T_high'] = TOIII_from_TSIII_relation(self.prior_vars['T_low'])
+# def temperature_selection(self, fit_T_low=True, fit_T_high=True):
+#
+#     if self.lowTemp_check and fit_T_low:
+#         self.set_prior('T_low')
+#
+#         if self.highTemp_check:
+#             self.set_prior('T_high')
+#         else:
+#             self.prior_vars['T_high'] = TOIII_from_TSIII_relation(self.prior_vars['T_low'])
+#
+#     else:
+#         if self.highTemp_check and fit_T_high:
+#             self.set_prior('T_high')
+#
+#         self.prior_vars['T_low'] = TOII_from_TOIII_relation(self.prior_vars['T_high'], self.prior_vars['n_e'])
+#
+#     return
+
+def temperature_selection(Tlow_diag, Thigh_diag, prior_dict):
+
+    # Both diagnostics available
+    if (not callable(Tlow_diag)) and (not callable(Thigh_diag)):
+        Tlow_prior, Thigh_prior = set_prior('T_low', prior_dict), set_prior('T_high', prior_dict)
 
+    # Only one:
     else:
-        if self.highTemp_check and fit_T_high:
-            self.set_prior('T_high')
+        if callable(Tlow_diag):
+            Thigh_prior = set_prior('T_high', prior_dict)
+            Tlow_prior = Tlow_diag(Thigh_prior)
 
-        self.prior_vars['T_low'] = TOII_from_TOIII_relation(self.prior_vars['T_high'], self.prior_vars['n_e'])
+        else:
+            Tlow_prior = set_prior('T_low', prior_dict)
+            Thigh_prior = Thigh_diag(Tlow_prior)
 
-    return
+    return Tlow_prior, Thigh_prior
 
 
 def direct_method_inference(fname, inputs, prior_dict, idcs_highTemp_ions, emiss_interp, eq_tt,
-                            fit_Tlow=True, fit_Thigh=True):
+                            Tlow_diag, Thigh_diag):
 
     # Container synthetic fluxes # FIXME do I need this one for loop inferences
     prior_vars = {}
 
     # Unpack the inputs
     line_arr, ion_arr = inputs.lines, inputs.particles
     flux_arr, err_arr = inputs.fluxes, inputs.errs
@@ -86,17 +104,30 @@
     with pm.Model() as model:
 
         # Declare models parameters priors
         prior_vars['n_e'] = set_prior('n_e', prior_dict)
         prior_vars['cHbeta'] = set_prior('cHbeta', prior_dict)
 
         # Establish models temperature structure
-        # temperature_selection(fit_Tlow, fit_Thigh)
-        prior_vars['T_low'] = set_prior('T_low', prior_dict)
-        prior_vars['T_high'] = set_prior('T_high', prior_dict)
+        # prior_vars['T_low'], prior_vars['T_high'] = temperature_selection(fit_Tlow, fit_Thigh, prior_dict)
+        # prior_vars['T_low'] = set_prior('T_low', prior_dict)
+        # prior_vars['T_high'] = set_prior('T_high', prior_dict)
+        # Both diagnostics available
+        if (not callable(Tlow_diag)) and (not callable(Thigh_diag)):
+            prior_vars['T_low'], prior_vars['T_high'] = set_prior('T_low', prior_dict), set_prior('T_high', prior_dict)
+
+        # Only one:
+        else:
+            if callable(Tlow_diag):
+                prior_vars['T_high'] = set_prior('T_high', prior_dict)
+                prior_vars['T_low'] = Tlow_diag(prior_vars['T_high'])
+
+            else:
+                prior_vars['T_low'] = set_prior('T_low', prior_dict)
+                prior_vars['T_high'] = Thigh_diag(prior_vars['T_low'])
 
         # Define grid interpolation variables
         emisCoord_low = tt.stack([[prior_vars['T_low'][0]], [prior_vars['n_e'][0]]], axis=-1)
         emisCoord_high = tt.stack([[prior_vars['T_high'][0]], [prior_vars['n_e'][0]]], axis=-1)
 
         # Establish models composition
         for ion in ions_unique:
```

### Comparing `specsy-0.2.2/src/specsy/models/emissivity.py` & `specsy-0.2.3/src/specsy/models/emissivity.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/models/extinction.py` & `specsy-0.2.3/src/specsy/models/extinction.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/models/fluxes_line.py` & `specsy-0.2.3/src/specsy/models/fluxes_line.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/models/nebular_continuum.py` & `specsy-0.2.3/src/specsy/models/nebular_continuum.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/operations/interpolation.py` & `specsy-0.2.3/src/specsy/operations/interpolation.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/operations/pytensors.py` & `specsy-0.2.3/src/specsy/operations/pytensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/operations/tensors.py` & `specsy-0.2.3/src/specsy/operations/tensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/operations/tests.py` & `specsy-0.2.3/src/specsy/operations/tests.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/plots.py` & `specsy-0.2.3/src/specsy/plots.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/resources/HI_t3_elec.ascii` & `specsy-0.2.3/src/specsy/resources/HI_t3_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/resources/HeII_t4_elec.ascii` & `specsy-0.2.3/src/specsy/resources/HeII_t4_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/resources/HeI_t5_elec.ascii` & `specsy-0.2.3/src/specsy/resources/HeI_t5_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/tools.py` & `specsy-0.2.3/src/specsy/tools.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy/treatement.py` & `specsy-0.2.3/src/specsy/treatement.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.2/src/specsy.egg-info/PKG-INFO` & `specsy-0.2.3/src/specsy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `specsy-0.2.2/src/specsy.egg-info/SOURCES.txt` & `specsy-0.2.3/src/specsy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

