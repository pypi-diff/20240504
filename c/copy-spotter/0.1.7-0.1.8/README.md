# Comparing `tmp/copy-spotter-0.1.7.tar.gz` & `tmp/copy-spotter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-spotter-0.1.7.tar", last modified: Sat May  4 15:03:59 2024, max compression
+gzip compressed data, was "copy-spotter-0.1.8.tar", last modified: Sat May  4 15:05:53 2024, max compression
```

## Comparing `copy-spotter-0.1.7.tar` & `copy-spotter-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:59.800205 copy-spotter-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 15:03:59.800205 copy-spotter-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:59.796205 copy-spotter-0.1.7/copy_spotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 15:03:59.000000 copy-spotter-0.1.7/copy_spotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-04 15:03:59.000000 copy-spotter-0.1.7/copy_spotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:03:59.000000 copy-spotter-0.1.7/copy_spotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 15:03:59.000000 copy-spotter-0.1.7/copy_spotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 15:03:59.000000 copy-spotter-0.1.7/copy_spotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 15:03:59.000000 copy-spotter-0.1.7/copy_spotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:59.800205 copy-spotter-0.1.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 15:03:59.800205 copy-spotter-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:59.800205 copy-spotter-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:59.800205 copy-spotter-0.1.7/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/test_html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/test_html_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/test_processing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-04 15:03:43.000000 copy-spotter-0.1.7/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:53.380487 copy-spotter-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 15:05:53.380487 copy-spotter-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:53.376487 copy-spotter-0.1.8/copy_spotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 15:05:53.000000 copy-spotter-0.1.8/copy_spotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-04 15:05:53.000000 copy-spotter-0.1.8/copy_spotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:05:53.000000 copy-spotter-0.1.8/copy_spotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 15:05:53.000000 copy-spotter-0.1.8/copy_spotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 15:05:53.000000 copy-spotter-0.1.8/copy_spotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 15:05:53.000000 copy-spotter-0.1.8/copy_spotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:53.380487 copy-spotter-0.1.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-04 15:05:53.380487 copy-spotter-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:53.380487 copy-spotter-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:53.380487 copy-spotter-0.1.8/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/test_html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/test_html_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/test_processing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-04 15:05:38.000000 copy-spotter-0.1.8/tests/scripts/test_utils.py
```

### Comparing `copy-spotter-0.1.7/LICENSE` & `copy-spotter-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/PKG-INFO` & `copy-spotter-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.7
+Version: 0.1.8
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `copy-spotter-0.1.7/README.md` & `copy-spotter-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/copy_spotter.egg-info/PKG-INFO` & `copy-spotter-0.1.8/copy_spotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-spotter
-Version: 0.1.7
+Version: 0.1.8
 Summary: Make plagiarism detection easier. This package will find similar sentences between given files and highlight them in a side by side comparison.
 Home-page: https://github.com/Wazzabeee/copy-spotter
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `copy-spotter-0.1.7/copy_spotter.egg-info/SOURCES.txt` & `copy-spotter-0.1.8/copy_spotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/scripts/html_utils.py` & `copy-spotter-0.1.8/scripts/html_utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/scripts/html_writing.py` & `copy-spotter-0.1.8/scripts/html_writing.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/scripts/main.py` & `copy-spotter-0.1.8/scripts/main.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/scripts/processing_files.py` & `copy-spotter-0.1.8/scripts/processing_files.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/scripts/similarity.py` & `copy-spotter-0.1.8/scripts/similarity.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/scripts/utils.py` & `copy-spotter-0.1.8/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/setup.py` & `copy-spotter-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `copy-spotter-0.1.7/tests/scripts/test_utils.py` & `copy-spotter-0.1.8/tests/scripts/test_utils.py`

 * *Files identical despite different names*

