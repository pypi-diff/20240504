# Comparing `tmp/bidskit-2024.1.12.tar.gz` & `tmp/bidskit-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bidskit-2024.1.12.tar", last modified: Sat Jan 13 01:05:34 2024, max compression
+gzip compressed data, was "bidskit-2024.5.3.tar", last modified: Fri May  3 23:13:39 2024, max compression
```

## Comparing `bidskit-2024.1.12.tar` & `bidskit-2024.5.3.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-01-13 01:05:34.766119 bidskit-2024.1.12/
--rw-r--r--   0 jmt        (501) staff       (20)     1073 2022-07-07 21:29:09.000000 bidskit-2024.1.12/LICENSE.md
--rw-r--r--   0 jmt        (501) staff       (20)     1770 2024-01-13 01:05:34.766007 bidskit-2024.1.12/PKG-INFO
--rw-r--r--   0 jmt        (501) staff       (20)      977 2023-02-16 22:56:27.000000 bidskit-2024.1.12/README.md
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-01-13 01:05:34.764466 bidskit-2024.1.12/bidskit/
--rw-r--r--   0 jmt        (501) staff       (20)      217 2022-10-11 18:01:05.000000 bidskit-2024.1.12/bidskit/__init__.py
--rwxr-xr-x   0 jmt        (501) staff       (20)    14387 2024-01-13 00:39:57.000000 bidskit-2024.1.12/bidskit/__main__.py
--rw-r--r--   0 jmt        (501) staff       (20)     1842 2023-09-07 22:01:59.000000 bidskit-2024.1.12/bidskit/bidsjson.py
--rw-r--r--   0 jmt        (501) staff       (20)     5494 2023-02-16 22:55:11.000000 bidskit-2024.1.12/bidskit/bidstree.py
--rw-r--r--   0 jmt        (501) staff       (20)    14190 2023-09-07 22:01:59.000000 bidskit-2024.1.12/bidskit/dcm2niix.py
--rw-r--r--   0 jmt        (501) staff       (20)     3791 2023-09-07 22:01:59.000000 bidskit-2024.1.12/bidskit/flywheel.py
--rw-r--r--   0 jmt        (501) staff       (20)    16042 2023-09-07 22:01:59.000000 bidskit-2024.1.12/bidskit/fmaps.py
--rw-r--r--   0 jmt        (501) staff       (20)    12173 2023-02-16 22:55:11.000000 bidskit-2024.1.12/bidskit/io.py
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-01-13 01:05:34.765872 bidskit-2024.1.12/bidskit/templates/
--rw-r--r--   0 jmt        (501) staff       (20)       37 2022-08-23 19:23:24.000000 bidskit-2024.1.12/bidskit/templates/CHANGES
--rw-r--r--   0 jmt        (501) staff       (20)     5613 2023-02-16 22:55:11.000000 bidskit-2024.1.12/bidskit/templates/README
--rw-r--r--   0 jmt        (501) staff       (20)       43 2023-02-16 22:55:11.000000 bidskit-2024.1.12/bidskit/templates/bidsignore
--rw-r--r--   0 jmt        (501) staff       (20)      326 2022-08-23 19:23:24.000000 bidskit-2024.1.12/bidskit/templates/dataset_description.json
--rw-r--r--   0 jmt        (501) staff       (20)      652 2022-08-23 19:23:24.000000 bidskit-2024.1.12/bidskit/templates/participants.json
--rw-r--r--   0 jmt        (501) staff       (20)    19281 2022-09-29 23:26:19.000000 bidskit-2024.1.12/bidskit/translate.py
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-01-13 01:05:34.765308 bidskit-2024.1.12/bidskit.egg-info/
--rw-r--r--   0 jmt        (501) staff       (20)     1770 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/PKG-INFO
--rw-r--r--   0 jmt        (501) staff       (20)      578 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/SOURCES.txt
--rw-r--r--   0 jmt        (501) staff       (20)        1 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/dependency_links.txt
--rw-r--r--   0 jmt        (501) staff       (20)       50 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/entry_points.txt
--rw-r--r--   0 jmt        (501) staff       (20)        1 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/not-zip-safe
--rw-r--r--   0 jmt        (501) staff       (20)       38 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/requires.txt
--rw-r--r--   0 jmt        (501) staff       (20)        8 2024-01-13 01:05:34.000000 bidskit-2024.1.12/bidskit.egg-info/top_level.txt
--rw-r--r--   0 jmt        (501) staff       (20)       38 2024-01-13 01:05:34.766163 bidskit-2024.1.12/setup.cfg
--rw-r--r--   0 jmt        (501) staff       (20)     8779 2024-01-13 01:05:23.000000 bidskit-2024.1.12/setup.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-05-03 23:13:39.939794 bidskit-2024.5.3/
+-rw-r--r--   0 jmt        (501) staff       (20)     1073 2022-07-07 21:29:09.000000 bidskit-2024.5.3/LICENSE.md
+-rw-r--r--   0 jmt        (501) staff       (20)     1851 2024-05-03 23:13:39.939630 bidskit-2024.5.3/PKG-INFO
+-rw-r--r--   0 jmt        (501) staff       (20)      976 2024-05-03 22:35:00.000000 bidskit-2024.5.3/README.md
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-05-03 23:13:39.937785 bidskit-2024.5.3/bidskit/
+-rw-r--r--   0 jmt        (501) staff       (20)      217 2022-10-11 18:01:05.000000 bidskit-2024.5.3/bidskit/__init__.py
+-rwxr-xr-x   0 jmt        (501) staff       (20)    14387 2024-01-13 00:39:57.000000 bidskit-2024.5.3/bidskit/__main__.py
+-rw-r--r--   0 jmt        (501) staff       (20)     1842 2023-09-07 22:01:59.000000 bidskit-2024.5.3/bidskit/bidsjson.py
+-rw-r--r--   0 jmt        (501) staff       (20)     5494 2023-02-16 22:55:11.000000 bidskit-2024.5.3/bidskit/bidstree.py
+-rw-r--r--   0 jmt        (501) staff       (20)    14190 2023-09-07 22:01:59.000000 bidskit-2024.5.3/bidskit/dcm2niix.py
+-rw-r--r--   0 jmt        (501) staff       (20)     3791 2023-09-07 22:01:59.000000 bidskit-2024.5.3/bidskit/flywheel.py
+-rw-r--r--   0 jmt        (501) staff       (20)    16042 2023-09-07 22:01:59.000000 bidskit-2024.5.3/bidskit/fmaps.py
+-rw-r--r--   0 jmt        (501) staff       (20)    12173 2023-02-16 22:55:11.000000 bidskit-2024.5.3/bidskit/io.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-05-03 23:13:39.939130 bidskit-2024.5.3/bidskit/templates/
+-rw-r--r--   0 jmt        (501) staff       (20)       37 2022-08-23 19:23:24.000000 bidskit-2024.5.3/bidskit/templates/CHANGES
+-rw-r--r--   0 jmt        (501) staff       (20)     5613 2023-02-16 22:55:11.000000 bidskit-2024.5.3/bidskit/templates/README
+-rw-r--r--   0 jmt        (501) staff       (20)       43 2023-02-16 22:55:11.000000 bidskit-2024.5.3/bidskit/templates/bidsignore
+-rw-r--r--   0 jmt        (501) staff       (20)      326 2022-08-23 19:23:24.000000 bidskit-2024.5.3/bidskit/templates/dataset_description.json
+-rw-r--r--   0 jmt        (501) staff       (20)      652 2022-08-23 19:23:24.000000 bidskit-2024.5.3/bidskit/templates/participants.json
+-rw-r--r--   0 jmt        (501) staff       (20)    19281 2022-09-29 23:26:19.000000 bidskit-2024.5.3/bidskit/translate.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-05-03 23:13:39.939470 bidskit-2024.5.3/bidskit.egg-info/
+-rw-r--r--   0 jmt        (501) staff       (20)     1851 2024-05-03 23:13:39.000000 bidskit-2024.5.3/bidskit.egg-info/PKG-INFO
+-rw-r--r--   0 jmt        (501) staff       (20)      604 2024-05-03 23:13:39.000000 bidskit-2024.5.3/bidskit.egg-info/SOURCES.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        1 2024-05-03 23:13:39.000000 bidskit-2024.5.3/bidskit.egg-info/dependency_links.txt
+-rw-r--r--   0 jmt        (501) staff       (20)       50 2024-05-03 23:13:39.000000 bidskit-2024.5.3/bidskit.egg-info/entry_points.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        1 2024-01-13 01:05:34.000000 bidskit-2024.5.3/bidskit.egg-info/not-zip-safe
+-rw-r--r--   0 jmt        (501) staff       (20)       38 2024-05-03 23:13:39.000000 bidskit-2024.5.3/bidskit.egg-info/requires.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        8 2024-05-03 23:13:39.000000 bidskit-2024.5.3/bidskit.egg-info/top_level.txt
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2024-05-03 23:13:39.939335 bidskit-2024.5.3/bin/
+-rwxr-xr-x   0 jmt        (501) staff       (20)     3617 2024-05-03 23:11:31.000000 bidskit-2024.5.3/bin/bidsdump
+-rwxr-xr-x   0 jmt        (501) staff       (20)     1807 2024-05-03 23:10:15.000000 bidskit-2024.5.3/bin/bidsmeta
+-rw-r--r--   0 jmt        (501) staff       (20)       38 2024-05-03 23:13:39.939827 bidskit-2024.5.3/setup.cfg
+-rw-r--r--   0 jmt        (501) staff       (20)     8915 2024-05-03 22:43:02.000000 bidskit-2024.5.3/setup.py
```

### Comparing `bidskit-2024.1.12/LICENSE.md` & `bidskit-2024.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/PKG-INFO` & `bidskit-2024.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bidskit
-Version: 2024.1.12
+Version: 2024.5.3
 Summary: BIDS curation toolkit
 Home-page: https://github.com/jmtyszka/bidskit
 Author: Julian Michael Tyszka
 Author-email: jmt@caltech.edu
 Project-URL: Bug Reports, https://github.com/jmtyszka/bidskit/issues
 Project-URL: Funding, http://conte.caltech.edu/
 Project-URL: Source, https://github.com/jmtyszka/bidskit/
@@ -14,18 +14,21 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: pydicom>=2.2
+Requires-Dist: pybids>=0.15
+Requires-Dist: numpy>=1.21
 
 # BIDSKIT
 
-### Version 2023.2.16
+### Version 2024.5.3
 Python utilities for converting from DICOM to BIDS neuroimaging formats.
 
 The *bidskit* console command takes a directory tree containing imaging series from one or more subjects (eg T1w MPRAGE, BOLD EPI, Fieldmaps), converts the imaging data to Nifti-1 format with JSON metadata files (sidecars) and populates a directory tree according to the latest BIDS specification.
 
 ## Documentation
 #### [Installation Instructions](docs/Installation.md)
 #### [Quick Start Guide](docs/QuickStart.md)
```

### Comparing `bidskit-2024.1.12/README.md` & `bidskit-2024.5.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BIDSKIT
 
-### Version 2023.2.16
+### Version 2024.5.3
 Python utilities for converting from DICOM to BIDS neuroimaging formats.
 
 The *bidskit* console command takes a directory tree containing imaging series from one or more subjects (eg T1w MPRAGE, BOLD EPI, Fieldmaps), converts the imaging data to Nifti-1 format with JSON metadata files (sidecars) and populates a directory tree according to the latest BIDS specification.
 
 ## Documentation
 #### [Installation Instructions](docs/Installation.md)
 #### [Quick Start Guide](docs/QuickStart.md)
```

### Comparing `bidskit-2024.1.12/bidskit/__main__.py` & `bidskit-2024.5.3/bidskit/__main__.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/bidsjson.py` & `bidskit-2024.5.3/bidskit/bidsjson.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/bidstree.py` & `bidskit-2024.5.3/bidskit/bidstree.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/dcm2niix.py` & `bidskit-2024.5.3/bidskit/dcm2niix.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/flywheel.py` & `bidskit-2024.5.3/bidskit/flywheel.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/fmaps.py` & `bidskit-2024.5.3/bidskit/fmaps.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/io.py` & `bidskit-2024.5.3/bidskit/io.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/templates/README` & `bidskit-2024.5.3/bidskit/templates/README`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/templates/participants.json` & `bidskit-2024.5.3/bidskit/templates/participants.json`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit/translate.py` & `bidskit-2024.5.3/bidskit/translate.py`

 * *Files identical despite different names*

### Comparing `bidskit-2024.1.12/bidskit.egg-info/PKG-INFO` & `bidskit-2024.5.3/bidskit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bidskit
-Version: 2024.1.12
+Version: 2024.5.3
 Summary: BIDS curation toolkit
 Home-page: https://github.com/jmtyszka/bidskit
 Author: Julian Michael Tyszka
 Author-email: jmt@caltech.edu
 Project-URL: Bug Reports, https://github.com/jmtyszka/bidskit/issues
 Project-URL: Funding, http://conte.caltech.edu/
 Project-URL: Source, https://github.com/jmtyszka/bidskit/
@@ -14,18 +14,21 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: pydicom>=2.2
+Requires-Dist: pybids>=0.15
+Requires-Dist: numpy>=1.21
 
 # BIDSKIT
 
-### Version 2023.2.16
+### Version 2024.5.3
 Python utilities for converting from DICOM to BIDS neuroimaging formats.
 
 The *bidskit* console command takes a directory tree containing imaging series from one or more subjects (eg T1w MPRAGE, BOLD EPI, Fieldmaps), converts the imaging data to Nifti-1 format with JSON metadata files (sidecars) and populates a directory tree according to the latest BIDS specification.
 
 ## Documentation
 #### [Installation Instructions](docs/Installation.md)
 #### [Quick Start Guide](docs/QuickStart.md)
```

### Comparing `bidskit-2024.1.12/bidskit.egg-info/SOURCES.txt` & `bidskit-2024.5.3/bidskit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 bidskit.egg-info/not-zip-safe
 bidskit.egg-info/requires.txt
 bidskit.egg-info/top_level.txt
 bidskit/templates/CHANGES
 bidskit/templates/README
 bidskit/templates/bidsignore
 bidskit/templates/dataset_description.json
-bidskit/templates/participants.json
+bidskit/templates/participants.json
+bin/bidsdump
+bin/bidsmeta
```

### Comparing `bidskit-2024.1.12/setup.py` & `bidskit-2024.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2024.1.12',  # Required
+    version='2024.5.3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='BIDS curation toolkit',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -172,14 +172,20 @@
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files
     #
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
     # data_files=[('my_data', ['data/data_file'])],  # Optional
 
+    # Legacy scripts argument for standalone scripts in bin/ folder
+    scripts=[
+        'bin/bidsdump',
+        'bin/bidsmeta'
+    ],
+
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
```

