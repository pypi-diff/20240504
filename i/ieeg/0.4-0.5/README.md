# Comparing `tmp/ieeg-0.4.tar.gz` & `tmp/ieeg-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeg-0.4.tar", last modified: Tue Apr 30 14:56:04 2024, max compression
+gzip compressed data, was "ieeg-0.5.tar", last modified: Fri May  3 22:16:06 2024, max compression
```

## Comparing `ieeg-0.4.tar` & `ieeg-0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.975821 ieeg-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 14:55:53.000000 ieeg-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-30 14:56:04.975821 ieeg-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-30 14:55:53.000000 ieeg-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.963821 ieeg-0.4/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 14:55:53.000000 ieeg-0.4/envs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.959821 ieeg-0.4/ieeg/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.963821 ieeg-0.4/ieeg/calc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.971820 ieeg-0.4/ieeg/calc/_fast/
--rw-r--r--   0 runner    (1001) docker     (127)   160311 2024-04-30 14:56:01.000000 ieeg-0.4/ieeg/calc/_fast/__init__.c
--rw-r--r--   0 runner    (1001) docker     (127)  1463209 2024-04-30 14:56:01.000000 ieeg-0.4/ieeg/calc/_fast/concat.c
--rw-r--r--   0 runner    (1001) docker     (127)  1326106 2024-04-30 14:56:02.000000 ieeg-0.4/ieeg/calc/_fast/mixup.c
--rw-r--r--   0 runner    (1001) docker     (127)  1368686 2024-04-30 14:56:03.000000 ieeg-0.4/ieeg/calc/_fast/permgt.c
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/_fast/ufuncs.c
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    48886 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/mat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/oversample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    36090 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/calc/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.963821 ieeg-0.4/ieeg/decoding/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68915 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/decoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.963821 ieeg-0.4/ieeg/decoding/joint_pca/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/joint_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/joint_pca/alignment_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/joint_pca/cross_pt_decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/joint_pca/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/decoding/preprocessing_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/mt_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/navigate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.971820 ieeg-0.4/ieeg/timefreq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/timefreq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/timefreq/gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)  1367750 2024-04-30 14:56:03.000000 ieeg-0.4/ieeg/timefreq/hilbert.c
--rw-r--r--   0 runner    (1001) docker     (127)    16337 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/timefreq/multitaper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/timefreq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.963821 ieeg-0.4/ieeg/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/viz/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    28087 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/viz/mri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-04-30 14:55:53.000000 ieeg-0.4/ieeg/viz/parula.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.975821 ieeg-0.4/ieeg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-30 14:56:04.000000 ieeg-0.4/ieeg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-30 14:56:04.000000 ieeg-0.4/ieeg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:56:04.000000 ieeg-0.4/ieeg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 14:56:04.000000 ieeg-0.4/ieeg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 14:56:04.000000 ieeg-0.4/ieeg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 14:55:53.000000 ieeg-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:56:04.975821 ieeg-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-30 14:55:53.000000 ieeg-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:56:04.975821 ieeg-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-30 14:55:53.000000 ieeg-0.4/tests/test_ieeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-30 14:55:53.000000 ieeg-0.4/tests/test_mat.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-30 14:55:53.000000 ieeg-0.4/tests/test_mri.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-30 14:55:53.000000 ieeg-0.4/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.499661 ieeg-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 22:15:53.000000 ieeg-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-03 22:16:06.499661 ieeg-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-03 22:15:53.000000 ieeg-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.491661 ieeg-0.5/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 22:15:53.000000 ieeg-0.5/envs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.487661 ieeg-0.5/ieeg/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.487661 ieeg-0.5/ieeg/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.495661 ieeg-0.5/ieeg/calc/_fast/
+-rw-r--r--   0 runner    (1001) docker     (127)   160311 2024-05-03 22:16:02.000000 ieeg-0.5/ieeg/calc/_fast/__init__.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1463209 2024-05-03 22:16:03.000000 ieeg-0.5/ieeg/calc/_fast/concat.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1326106 2024-05-03 22:16:03.000000 ieeg-0.5/ieeg/calc/_fast/mixup.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1368686 2024-05-03 22:16:04.000000 ieeg-0.5/ieeg/calc/_fast/permgt.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/_fast/ufuncs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48892 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/mat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/oversample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36090 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/calc/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.487661 ieeg-0.5/ieeg/decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68915 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/decoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.487661 ieeg-0.5/ieeg/decoding/joint_pca/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/joint_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/joint_pca/alignment_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/joint_pca/cross_pt_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/joint_pca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/decoding/preprocessing_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/mt_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/navigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.495661 ieeg-0.5/ieeg/timefreq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/timefreq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/timefreq/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1367750 2024-05-03 22:16:05.000000 ieeg-0.5/ieeg/timefreq/hilbert.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16337 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/timefreq/multitaper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/timefreq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.491661 ieeg-0.5/ieeg/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/viz/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28087 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/viz/mri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-03 22:15:53.000000 ieeg-0.5/ieeg/viz/parula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.499661 ieeg-0.5/ieeg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-03 22:16:06.000000 ieeg-0.5/ieeg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 22:16:06.000000 ieeg-0.5/ieeg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:16:06.000000 ieeg-0.5/ieeg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 22:16:06.000000 ieeg-0.5/ieeg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 22:16:06.000000 ieeg-0.5/ieeg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-03 22:15:53.000000 ieeg-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:16:06.499661 ieeg-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-03 22:15:53.000000 ieeg-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:16:06.499661 ieeg-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-03 22:15:53.000000 ieeg-0.5/tests/test_ieeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-05-03 22:15:53.000000 ieeg-0.5/tests/test_mat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-03 22:15:53.000000 ieeg-0.5/tests/test_mri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-03 22:15:53.000000 ieeg-0.5/tests/test_stats.py
```

### Comparing `ieeg-0.4/LICENSE` & `ieeg-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/PKG-INFO` & `ieeg-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeg
-Version: 0.4
+Version: 0.5
 Summary: A Python package for iEEG data processing.
 Home-page: https://github.com/coganlab/IEEG_Pipelines
 Author: Aaron Earle-Richardson
 Author-email: Aaron Earle-Richardson <ae166@duke.edu>, Raymond Xiong <raymond.xiong@duke.edu>
 License: MIT License
         
         Copyright (c) 2023 coganlab
@@ -27,19 +27,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/coganlab/IEEG_Pipelines
 Project-URL: Source, https://github.com/coganlab/IEEG_Pipelines
 Project-URL: Issues, https://github.com/coganlab/IEEG_Pipelines/Issues
 Project-URL: Documentation, https://ieeg-pipelines.readthedocs.io/en/latest/
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bids>=0.0
-Requires-Dist: EDFlib-Python
 Requires-Dist: mne
 Requires-Dist: mne-bids
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
```

### Comparing `ieeg-0.4/README.md` & `ieeg-0.5/README.md`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/calc/_fast/__init__.c` & `ieeg-0.5/ieeg/calc/_fast/__init__.c`

 * *Files 0% similar despite different names*

```diff
@@ -9,24 +9,24 @@
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "libraries": [
             "npyrandom",
             "npymath"
         ],
         "library_dirs": [
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/lib",
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/random/lib"
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/lib",
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/random/lib"
         ],
         "name": "ieeg.calc._fast.__init__",
         "sources": [
             "ieeg/calc/_fast/__init__.pyx"
         ]
     },
     "module_name": "ieeg.calc._fast.__init__"
```

### Comparing `ieeg-0.4/ieeg/calc/_fast/concat.c` & `ieeg-0.5/ieeg/calc/_fast/concat.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,34 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "libraries": [
             "npyrandom",
             "npymath"
         ],
         "library_dirs": [
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/lib",
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/random/lib"
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/lib",
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/random/lib"
         ],
         "name": "ieeg.calc._fast.concat",
         "sources": [
             "ieeg/calc/_fast/concat.pyx"
         ]
     },
     "module_name": "ieeg.calc._fast.concat"
@@ -1687,177 +1687,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1890,42 +1890,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -17993,261 +17993,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18256,29 +18256,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18289,15 +18289,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18306,29 +18306,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18339,15 +18339,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18356,29 +18356,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18389,15 +18389,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18406,29 +18406,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18439,15 +18439,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18456,29 +18456,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18489,217 +18489,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18715,15 +18715,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18731,68 +18731,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18800,15 +18800,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18823,15 +18823,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18847,15 +18847,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18863,68 +18863,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18932,15 +18932,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18955,15 +18955,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18979,15 +18979,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18995,68 +18995,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19064,15 +19064,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19087,170 +19087,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28844,26 +28844,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `ieeg-0.4/ieeg/calc/_fast/mixup.c` & `ieeg-0.5/ieeg/calc/_fast/mixup.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,35 +6,35 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/random/bitgen.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/random/bitgen.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "libraries": [
             "npyrandom",
             "npymath"
         ],
         "library_dirs": [
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/lib",
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/random/lib"
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/lib",
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/random/lib"
         ],
         "name": "ieeg.calc._fast.mixup",
         "sources": [
             "ieeg/calc/_fast/mixup.pyx"
         ]
     },
     "module_name": "ieeg.calc._fast.mixup"
@@ -1691,177 +1691,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1899,42 +1899,42 @@
 struct __pyx_obj_4ieeg_4calc_5_fast_5mixup_RNG;
 struct __pyx_obj_4ieeg_4calc_5_fast_5mixup___pyx_scope_struct__spawn;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18487,261 +18487,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18750,29 +18750,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18783,15 +18783,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18800,29 +18800,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18833,15 +18833,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18850,29 +18850,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18883,15 +18883,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18900,29 +18900,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18933,15 +18933,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18950,29 +18950,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18983,217 +18983,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19209,15 +19209,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19225,68 +19225,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19294,15 +19294,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19317,15 +19317,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19341,15 +19341,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19357,68 +19357,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19426,15 +19426,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19449,15 +19449,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19473,15 +19473,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19489,68 +19489,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19558,15 +19558,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19581,170 +19581,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -24313,26 +24313,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `ieeg-0.4/ieeg/calc/_fast/permgt.c` & `ieeg-0.5/ieeg/calc/_fast/permgt.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,35 +6,35 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/random/bitgen.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/random/bitgen.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "libraries": [
             "npyrandom",
             "npymath"
         ],
         "library_dirs": [
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/lib",
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/random/lib"
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/lib",
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/random/lib"
         ],
         "name": "ieeg.calc._fast.permgt",
         "sources": [
             "ieeg/calc/_fast/permgt.pyx"
         ]
     },
     "module_name": "ieeg.calc._fast.permgt"
@@ -1691,177 +1691,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1935,42 +1935,42 @@
 struct __pyx_obj_4ieeg_4calc_5_fast_6permgt_RNG;
 struct __pyx_obj_4ieeg_4calc_5_fast_6permgt___pyx_scope_struct__spawn;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18592,261 +18592,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18855,29 +18855,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18888,15 +18888,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18905,29 +18905,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18938,15 +18938,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18955,29 +18955,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18988,15 +18988,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19005,29 +19005,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19038,15 +19038,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19055,29 +19055,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19088,217 +19088,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19314,15 +19314,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19330,68 +19330,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19399,15 +19399,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19422,15 +19422,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19446,15 +19446,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19462,68 +19462,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19531,15 +19531,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19554,15 +19554,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19578,15 +19578,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19594,68 +19594,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19663,15 +19663,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19686,170 +19686,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25270,26 +25270,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `ieeg-0.4/ieeg/calc/_fast/ufuncs.c` & `ieeg-0.5/ieeg/calc/_fast/ufuncs.c`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/calc/fast.py` & `ieeg-0.5/ieeg/calc/fast.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/calc/mat.py` & `ieeg-0.5/ieeg/calc/mat.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,15 +623,15 @@
 
         new_labels[levels[1] - 1] = (
                 self.labels[levels[0]] @ self.labels[levels[1]]).flatten()
 
         all_idx = ([slice(None) if i != levels[0] else sl for i in
                     range(self.ndim)] for sl in range(self.shape[levels[0]]))
 
-        arrs = [self.__array__()[*idx] for idx in all_idx]
+        arrs = [self.__array__()[tuple(idx)] for idx in all_idx]
         new_array = concatenate_arrays(arrs, axis=levels[1] - 1)
 
         return LabeledArray(new_array, new_labels, dtype=self.dtype)
 
     def take(self, indices, axis=None, **kwargs):
         """Take elements from an array along an axis.
```

### Comparing `ieeg-0.4/ieeg/calc/oversample.py` & `ieeg-0.5/ieeg/calc/oversample.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/calc/reshape.py` & `ieeg-0.5/ieeg/calc/reshape.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/calc/scaling.py` & `ieeg-0.5/ieeg/calc/scaling.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import numpy as np
 from mne import Epochs
 from mne.epochs import BaseEpochs
 from mne.time_frequency import AverageTFR, EpochsTFR
 from mne.utils import logger, verbose
 
-TFR = EpochsTFR | AverageTFR
-
 
 def _log_rescale(baseline, mode='mean'):
     """Log the rescaling method."""
     if baseline is not None:
         msg = 'Applying baseline correction (mode: %s)' % mode
     else:
         msg = 'No baseline correction applied'
@@ -122,35 +120,49 @@
     line.pick(picks)._data = rescale(line.pick(picks)._data, basedata, mode,
                                      False, axes)
     return line
 
 
 @rescale.register
 @verbose
-def _(line: TFR, baseline: TFR,
+def _(line: EpochsTFR, baseline: EpochsTFR,
       mode: str = 'mean', copy: bool = False, picks: list = 'data',
       verbose=None) -> Epochs:
     """Rescale (baseline correct) Epochs"""
     if copy:
         line: Epochs = line.copy()
     if verbose is not False:
         msg = _log_rescale(baseline, mode)
         logger.info(msg)
 
     # Average the baseline across epochs
     basedata = baseline.pick(picks)._data
-    axes = list(range(basedata.ndim))
 
-    # within channels
-    axes.pop(1)
+    # If time frequency then within frequency
+    axes = (0, 3)
+
+    line.pick(picks)._data = rescale(line.pick(picks)._data, basedata, mode,
+                                     False, axes)
+    return line
+
+
+@rescale.register
+@verbose
+def _(line: AverageTFR, baseline: AverageTFR,
+      mode: str = 'mean', copy: bool = False, picks: list = 'data',
+      verbose=None) -> Epochs:
+    """Rescale (baseline correct) Epochs"""
+    if copy:
+        line: Epochs = line.copy()
+    if verbose is not False:
+        msg = _log_rescale(baseline, mode)
+        logger.info(msg)
+
+    # Average the baseline across epochs
+    basedata = baseline.pick(picks)._data
 
     # If time frequency then within frequency
-    if isinstance(line, EpochsTFR):
-        axes = (0, 3)
-    elif isinstance(line, AverageTFR):
-        axes = 2
-    else:
-        axes = tuple(axes)
+    axes = 2
 
     line.pick(picks)._data = rescale(line.pick(picks)._data, basedata, mode,
                                      False, axes)
     return line
```

### Comparing `ieeg-0.4/ieeg/calc/stats.py` & `ieeg-0.5/ieeg/calc/stats.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/decoding/decoders.py` & `ieeg-0.5/ieeg/decoding/decoders.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/decoding/joint_pca/alignment_methods.py` & `ieeg-0.5/ieeg/decoding/joint_pca/alignment_methods.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/decoding/joint_pca/cross_pt_decoders.py` & `ieeg-0.5/ieeg/decoding/joint_pca/cross_pt_decoders.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/decoding/joint_pca/utils.py` & `ieeg-0.5/ieeg/decoding/joint_pca/utils.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/decoding/metrics.py` & `ieeg-0.5/ieeg/decoding/metrics.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/decoding/preprocessing_funcs.py` & `ieeg-0.5/ieeg/decoding/preprocessing_funcs.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/io.py` & `ieeg-0.5/ieeg/io.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/mt_filter.py` & `ieeg-0.5/ieeg/mt_filter.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/navigate.py` & `ieeg-0.5/ieeg/navigate.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/process.py` & `ieeg-0.5/ieeg/process.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/timefreq/gamma.py` & `ieeg-0.5/ieeg/timefreq/gamma.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/timefreq/hilbert.c` & `ieeg-0.5/ieeg/timefreq/hilbert.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,34 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3"
         ],
         "include_dirs": [
-            "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/include"
+            "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "libraries": [
             "npyrandom",
             "npymath"
         ],
         "library_dirs": [
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/core/lib",
-            "/tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/random/lib"
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/core/lib",
+            "/tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/random/lib"
         ],
         "name": "ieeg.timefreq.hilbert",
         "sources": [
             "ieeg/timefreq/hilbert.pyx"
         ]
     },
     "module_name": "ieeg.timefreq.hilbert"
@@ -1687,177 +1687,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1908,42 +1908,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18494,261 +18494,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18757,29 +18757,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18790,15 +18790,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18807,29 +18807,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18840,15 +18840,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18857,29 +18857,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18890,15 +18890,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18907,29 +18907,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18940,15 +18940,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18957,29 +18957,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18990,217 +18990,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19216,15 +19216,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19232,68 +19232,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19301,15 +19301,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19324,15 +19324,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19348,15 +19348,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19364,68 +19364,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19433,15 +19433,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19456,15 +19456,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19480,15 +19480,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19496,68 +19496,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19565,15 +19565,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19588,170 +19588,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25484,26 +25484,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-5fk_mv3i/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-8a5se8k4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `ieeg-0.4/ieeg/timefreq/multitaper.py` & `ieeg-0.5/ieeg/timefreq/multitaper.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/timefreq/utils.py` & `ieeg-0.5/ieeg/timefreq/utils.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/viz/ensemble.py` & `ieeg-0.5/ieeg/viz/ensemble.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/viz/mri.py` & `ieeg-0.5/ieeg/viz/mri.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg/viz/parula.py` & `ieeg-0.5/ieeg/viz/parula.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/ieeg.egg-info/PKG-INFO` & `ieeg-0.5/ieeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeg
-Version: 0.4
+Version: 0.5
 Summary: A Python package for iEEG data processing.
 Home-page: https://github.com/coganlab/IEEG_Pipelines
 Author: Aaron Earle-Richardson
 Author-email: Aaron Earle-Richardson <ae166@duke.edu>, Raymond Xiong <raymond.xiong@duke.edu>
 License: MIT License
         
         Copyright (c) 2023 coganlab
@@ -27,19 +27,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/coganlab/IEEG_Pipelines
 Project-URL: Source, https://github.com/coganlab/IEEG_Pipelines
 Project-URL: Issues, https://github.com/coganlab/IEEG_Pipelines/Issues
 Project-URL: Documentation, https://ieeg-pipelines.readthedocs.io/en/latest/
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bids>=0.0
-Requires-Dist: EDFlib-Python
 Requires-Dist: mne
 Requires-Dist: mne-bids
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
```

### Comparing `ieeg-0.4/ieeg.egg-info/SOURCES.txt` & `ieeg-0.5/ieeg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/pyproject.toml` & `ieeg-0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "A Python package for iEEG data processing."
 authors = [
     {name = "Aaron Earle-Richardson", email = "ae166@duke.edu"},
     {name = "Raymond Xiong", email = "raymond.xiong@duke.edu"}
 ]
 dynamic = ["dependencies", "version"]
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["ieeg*"]
 
 [project.license]
 file = "LICENSE"
```

### Comparing `ieeg-0.4/setup.py` & `ieeg-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 npymath_path = op.normpath(op.join(_numpy_abs, '..', 'lib'))
 npyrandom_path = op.normpath(op.join(_numpy_abs, '..', '..', 'random', 'lib'))
 lib_path = [npymath_path, npyrandom_path]
 if sys.platform == 'win32':
     compile_args = ["/O2"]
 elif sys.platform == 'linux':
     compile_args = ["-O3"]
+elif sys.platform == 'darwin':
+    compile_args = ["-O3"]
 else:
     raise NotImplementedError(f"Platform {sys.platform} not supported.")
 
 try:
     _numpy_abs = op.relpath(_numpy_abs, getcwd())
 except ValueError:
     pass
@@ -73,15 +75,15 @@
         ['ieeg/timefreq/hilbert.c'],  # the Cython source file
         **kwargs
     ),
 ]
 
 setup(
     name='ieeg',
-    version='0.4',
+    version='0.5',
     packages=find_packages(
         where='.',
         include=['ieeg*'],
     ),
     package_dir={"": "."},
     description='A Python package for iEEG data processing.',
     author='Aaron Earle-Richardson',
```

### Comparing `ieeg-0.4/tests/test_ieeg.py` & `ieeg-0.5/tests/test_ieeg.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/tests/test_mat.py` & `ieeg-0.5/tests/test_mat.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/tests/test_mri.py` & `ieeg-0.5/tests/test_mri.py`

 * *Files identical despite different names*

### Comparing `ieeg-0.4/tests/test_stats.py` & `ieeg-0.5/tests/test_stats.py`

 * *Files identical despite different names*

