# Comparing `tmp/specsy-0.2.5.tar.gz` & `tmp/specsy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsy-0.2.5.tar", last modified: Sat May  4 19:56:42 2024, max compression
+gzip compressed data, was "specsy-0.2.6.tar", last modified: Sat May  4 20:07:01 2024, max compression
```

## Comparing `specsy-0.2.5.tar` & `specsy-0.2.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.864692 specsy-0.2.5/
--rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.5/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:56:42.864692 specsy-0.2.5/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.5/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1227 2024-05-04 19:55:36.000000 specsy-0.2.5/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-04 19:56:42.864692 specsy-0.2.5/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1535 2024-04-29 22:29:38.000000 specsy-0.2.5/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy/
--rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.5/src/specsy/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-04 19:55:36.000000 specsy-0.2.5/src/specsy/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/core.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy/inference/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/inference/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/inference/emission.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy/innate/
--rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/innate/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/innate/interpol_pytensor.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3830 2024-05-03 19:46:25.000000 specsy-0.2.5/src/specsy/innate/main.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    12911 2024-05-04 19:21:02.000000 specsy-0.2.5/src/specsy/io.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy/models/
--rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/models/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17030 2024-05-03 21:54:50.000000 specsy-0.2.5/src/specsy/models/chemistry.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.5/src/specsy/models/chemistry_inference.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17254 2024-05-04 19:53:13.000000 specsy-0.2.5/src/specsy/models/emissivity.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    22659 2024-05-04 19:52:53.000000 specsy-0.2.5/src/specsy/models/extinction.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/models/fluxes_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/models/nebular_continuum.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy/operations/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/operations/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/operations/interpolation.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/operations/pytensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/operations/tensors.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/operations/tests.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/plots.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.5/src/specsy/resources/HI_t3_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/resources/HeII_t4_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/resources/HeI_t5_elec.ascii
--rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/resources/gordon_2003_LMC2_supershell.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/resources/gordon_2003_LMC_average.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/resources/gordon_2003_SMC_bar.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    10320 2024-05-04 19:53:00.000000 specsy-0.2.5/src/specsy/treatement.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.864692 specsy-0.2.5/src/specsy/workflow/
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.5/src/specsy/workflow/__init__.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:56:42.860692 specsy-0.2.5/src/specsy.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     1890 2024-05-04 19:56:42.000000 specsy-0.2.5/src/specsy.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-04 19:56:42.000000 specsy-0.2.5/src/specsy.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 19:56:42.000000 specsy-0.2.5/src/specsy.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      277 2024-05-04 19:56:42.000000 specsy-0.2.5/src/specsy.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-04 19:56:42.000000 specsy-0.2.5/src/specsy.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       17 2024-04-29 21:50:58.000000 specsy-0.2.6/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     1864 2024-05-04 20:07:01.340143 specsy-0.2.6/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      866 2024-04-29 21:50:58.000000 specsy-0.2.6/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1228 2024-05-04 20:06:36.000000 specsy-0.2.6/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      431 2024-05-04 20:07:01.340143 specsy-0.2.6/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1526 2024-05-04 20:05:09.000000 specsy-0.2.6/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.336142 specsy-0.2.6/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      927 2024-04-30 20:35:13.000000 specsy-0.2.6/src/specsy/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     5802 2024-05-04 20:06:36.000000 specsy-0.2.6/src/specsy/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      759 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/core.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/inference/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/inference/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16792 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/inference/emission.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/innate/
+-rw-rw-r--   0 vital     (1000) vital     (1000)       90 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/innate/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4246 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/innate/interpol_pytensor.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3830 2024-05-03 19:46:25.000000 specsy-0.2.6/src/specsy/innate/main.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12911 2024-05-04 19:21:02.000000 specsy-0.2.6/src/specsy/io.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/models/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      243 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/models/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17030 2024-05-03 21:54:50.000000 specsy-0.2.6/src/specsy/models/chemistry.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     6541 2024-05-03 21:52:49.000000 specsy-0.2.6/src/specsy/models/chemistry_inference.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17254 2024-05-04 19:53:13.000000 specsy-0.2.6/src/specsy/models/emissivity.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    22659 2024-05-04 19:52:53.000000 specsy-0.2.6/src/specsy/models/extinction.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/models/fluxes_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     8332 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/models/nebular_continuum.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/operations/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/operations/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10732 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/operations/interpolation.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4535 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/operations/pytensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4631 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/operations/tensors.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1329 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/operations/tests.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    16155 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/plots.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      419 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/resources/Benjamin1999_OpticalDepthFunctionCoefficients.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    21375 2024-04-29 21:50:58.000000 specsy-0.2.6/src/specsy/resources/HI_t3_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)    44530 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/resources/HeII_t4_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)   326042 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/resources/HeI_t5_elec.ascii
+-rw-rw-r--   0 vital     (1000) vital     (1000)      451 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/resources/gordon_2003_LMC2_supershell.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      476 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/resources/gordon_2003_LMC_average.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      483 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/resources/gordon_2003_SMC_bar.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2887 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10320 2024-05-04 19:53:00.000000 specsy-0.2.6/src/specsy/treatement.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy/workflow/
+-rw-rw-r--   0 vital     (1000) vital     (1000)        0 2024-04-29 21:50:59.000000 specsy-0.2.6/src/specsy/workflow/__init__.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 20:07:01.340143 specsy-0.2.6/src/specsy.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     1864 2024-05-04 20:07:01.000000 specsy-0.2.6/src/specsy.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1310 2024-05-04 20:07:01.000000 specsy-0.2.6/src/specsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 20:07:01.000000 specsy-0.2.6/src/specsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      266 2024-05-04 20:07:01.000000 specsy-0.2.6/src/specsy.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        7 2024-05-04 20:07:01.000000 specsy-0.2.6/src/specsy.egg-info/top_level.txt
```

### Comparing `specsy-0.2.5/PKG-INFO` & `specsy-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,14 @@
 Requires-Dist: jaxlib==0.4.26
 Requires-Dist: lime-stable~=1.0
 Requires-Dist: lmfit~=1.3
 Requires-Dist: matplotlib~=3.8
 Requires-Dist: numpy~=1.26
 Requires-Dist: pandas~=2.2.2
 Requires-Dist: pymc~=5.13
-Requires-Dist: PyNeb~=1.1
 Requires-Dist: pytensor~=2.20
 Requires-Dist: scipy~=1.13
 Requires-Dist: six~=1.16.0
 Requires-Dist: toml~=0.10
 Requires-Dist: tomli>=2.0.0; python_version < "3.11"
 Requires-Dist: xarray~=2024.3.0
```

### Comparing `specsy-0.2.5/README.rst` & `specsy-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/pyproject.toml` & `specsy-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "specsy"
-version = "0.2.5"
+version = "0.2.6"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Model fitting package for the chemical analysis of astronomical spectra"
 dependencies = ["arviz~=0.18",
                 "astropy~=6.0",
@@ -14,15 +14,15 @@
                 "jaxlib==0.4.26",
                 "lime-stable~=1.0",
                 "lmfit~=1.3",
                 "matplotlib~=3.8",
                 "numpy~=1.26",
                 "pandas~=2.2.2",
                 "pymc~=5.13",
-                "PyNeb~=1.1",
+                #"PyNeb~=1.1",
                 "pytensor~=2.20",
                 "scipy~=1.13",
                 "six~=1.16.0",
                 "toml~=0.10",
                 "tomli >= 2.0.0 ; python_version < '3.11'",
                 "xarray~=2024.3.0"]
```

### Comparing `specsy-0.2.5/setup.py` & `specsy-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,11 +32,11 @@
           "Programming Language :: Python :: 3.9",
       ],
       packages=find_packages('src'),
       package_dir={'': 'src'},
       package_data={'': ['config.toml', 'inference/*', 'innate/*', 'models/*', 'operations/*', 'resources/*', 'workflow/*']},
       include_package_data=True,
       install_requires=["arviz", "astropy", "h5netcdf", "jax", "jaxlib", "lime-stable", "lmfit", "matplotlib", "numpy",
-                        "pandas", "pymc", "PyNeb", "pytensor", "scipy", "toml", "xarray"],
+                        "pandas", "pymc", "pytensor", "scipy", "toml", "xarray"],
       )
```

### Comparing `specsy-0.2.5/src/specsy/__init__.py` & `specsy-0.2.6/src/specsy/__init__.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/config.toml` & `specsy-0.2.6/src/specsy/config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = 'specsy'
-version = '0.2.5'
+version = '0.2.6'
 
 [direct_method_cfg]
 temp_zones.high = ["He1", "He2", "O3", "Ar4", "Ne3", "Cl4", "C3"]
 temp_zones.low  = ["H1", "Ar3", "S2", "S3", "N2", "O2", "Fe3", "C2"]
 parameter_list = ["n_e", "T_low", "T_high", "cHbeta", "tau", "Ar3", "Ar4", "N2", "O2", "O3", "S2", "S3", "He1", "He2",
                   "Cl3","Ne3","Fe3","Teff","logU"]
 temp_low_diag = ['S3_6312A']
```

### Comparing `specsy-0.2.5/src/specsy/core.py` & `specsy-0.2.6/src/specsy/core.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/inference/emission.py` & `specsy-0.2.6/src/specsy/inference/emission.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/innate/interpol_pytensor.py` & `specsy-0.2.6/src/specsy/innate/interpol_pytensor.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/innate/main.py` & `specsy-0.2.6/src/specsy/innate/main.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/io.py` & `specsy-0.2.6/src/specsy/io.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/models/chemistry.py` & `specsy-0.2.6/src/specsy/models/chemistry.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/models/chemistry_inference.py` & `specsy-0.2.6/src/specsy/models/chemistry_inference.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/models/emissivity.py` & `specsy-0.2.6/src/specsy/models/emissivity.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/models/extinction.py` & `specsy-0.2.6/src/specsy/models/extinction.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/models/fluxes_line.py` & `specsy-0.2.6/src/specsy/models/fluxes_line.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/models/nebular_continuum.py` & `specsy-0.2.6/src/specsy/models/nebular_continuum.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/operations/interpolation.py` & `specsy-0.2.6/src/specsy/operations/interpolation.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/operations/pytensors.py` & `specsy-0.2.6/src/specsy/operations/pytensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/operations/tensors.py` & `specsy-0.2.6/src/specsy/operations/tensors.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/operations/tests.py` & `specsy-0.2.6/src/specsy/operations/tests.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/plots.py` & `specsy-0.2.6/src/specsy/plots.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/resources/HI_t3_elec.ascii` & `specsy-0.2.6/src/specsy/resources/HI_t3_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/resources/HeII_t4_elec.ascii` & `specsy-0.2.6/src/specsy/resources/HeII_t4_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/resources/HeI_t5_elec.ascii` & `specsy-0.2.6/src/specsy/resources/HeI_t5_elec.ascii`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/tools.py` & `specsy-0.2.6/src/specsy/tools.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy/treatement.py` & `specsy-0.2.6/src/specsy/treatement.py`

 * *Files identical despite different names*

### Comparing `specsy-0.2.5/src/specsy.egg-info/PKG-INFO` & `specsy-0.2.6/src/specsy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsy
-Version: 0.2.5
+Version: 0.2.6
 Summary: Model fitting package for the chemical analysis of astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/specsy
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,14 @@
 Requires-Dist: jaxlib==0.4.26
 Requires-Dist: lime-stable~=1.0
 Requires-Dist: lmfit~=1.3
 Requires-Dist: matplotlib~=3.8
 Requires-Dist: numpy~=1.26
 Requires-Dist: pandas~=2.2.2
 Requires-Dist: pymc~=5.13
-Requires-Dist: PyNeb~=1.1
 Requires-Dist: pytensor~=2.20
 Requires-Dist: scipy~=1.13
 Requires-Dist: six~=1.16.0
 Requires-Dist: toml~=0.10
 Requires-Dist: tomli>=2.0.0; python_version < "3.11"
 Requires-Dist: xarray~=2024.3.0
```

### Comparing `specsy-0.2.5/src/specsy.egg-info/SOURCES.txt` & `specsy-0.2.6/src/specsy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

