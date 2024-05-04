# Comparing `tmp/segmentation_skeleton_metrics-4.1.4.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.1.4.tar", last modified: Sat Apr 13 19:29:21 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.5.tar", last modified: Fri May  3 23:59:43 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.1.4.tar` & `segmentation_skeleton_metrics-4.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.013685 segmentation_skeleton_metrics-4.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.017685 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.029685 segmentation_skeleton_metrics-4.1.4/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.041685 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.013685 segmentation_skeleton_metrics-4.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.041685 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 19:29:10.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/merge_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-13 19:29:21.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 19:29:20.000000 segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:29:21.045685 segmentation_skeleton_metrics-4.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 19:29:09.000000 segmentation_skeleton_metrics-4.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.879700 segmentation_skeleton_metrics-4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.843700 segmentation_skeleton_metrics-4.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.847700 segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.847700 segmentation_skeleton_metrics-4.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-03 23:59:43.879700 segmentation_skeleton_metrics-4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.847700 segmentation_skeleton_metrics-4.1.5/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.847700 segmentation_skeleton_metrics-4.1.5/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.851700 segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.863700 segmentation_skeleton_metrics-4.1.5/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.875700 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 23:59:43.879700 segmentation_skeleton_metrics-4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.847700 segmentation_skeleton_metrics-4.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.875700 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 23:59:33.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/merge_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28825 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.879700 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-03 23:59:43.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-03 23:59:43.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:59:43.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 23:59:43.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 23:59:43.000000 segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:59:43.875700 segmentation_skeleton_metrics-4.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 23:59:32.000000 segmentation_skeleton_metrics-4.1.5/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.5/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.5/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.5/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/.gitignore` & `segmentation_skeleton_metrics-4.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/LICENSE` & `segmentation_skeleton_metrics-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/PKG-INFO` & `segmentation_skeleton_metrics-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.4
+Version: 4.1.5
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.4/README.md` & `segmentation_skeleton_metrics-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.5/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.5/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.5/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.5/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/pyproject.toml` & `segmentation_skeleton_metrics-4.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.5/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.5/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.5/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.5/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.5/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.5/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.5/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.5/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/merge_detection.py` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/merge_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         target_swc_paths,
         anisotropy=[1.0, 1.0, 1.0],
         black_holes_xyz_id=None,
         black_hole_radius=24,
         connections_path=None,
         ignore_boundary_mistakes=False,
         output_dir=None,
-        valid_size_threshold=25,
+        valid_size_threshold=40,
         save_swc=False,
     ):
         """
         Constructs skeleton metric object that evaluates the quality of a
         predicted segmentation.
 
         Parameters
@@ -113,31 +113,33 @@
         self.save = save_swc
 
         self.init_black_holes(black_holes_xyz_id)
         self.black_hole_radius = black_hole_radius
 
         # Labels
         self.label_mask = pred_labels
-        self.valid_labels = swc_utils.parse(
-            pred_swc_paths, valid_size_threshold, anisotropy
-        )
+        self.valid_labels = None
+        # swc_utils.parse(
+        #      pred_swc_paths, valid_size_threshold, anisotropy
+        # )
         self.init_equiv_labels(connections_path)
 
         # Build Graphs
-        self.graphs = self.init_graphs(target_swc_paths, [1.0, 1.0, 1.0])
+        self.graphs = self.init_graphs(target_swc_paths, anisotropy)
         self.init_labeled_graphs()
 
         # Build kdtree
         self.init_xyz_to_id_node()
         self.init_kdtree()
         self.rm_spurious_intersections()
 
     # -- Initialize and Label Graphs --
     def init_equiv_labels(self, path):
         if path:
+            assert self.valid_labels is not None, "Must provide valid labels!"
             self.equiv_labels_map = utils.equiv_class_mappings(
                 path, self.valid_labels
             )
             valid_labels = dict()
             for label, values in self.valid_labels.items():
                 equiv_label = self.equiv_labels_map[label]
                 valid_labels[equiv_label] = values
@@ -162,14 +164,15 @@
         Returns
         -------
         None
 
         """
         graphs = dict()
         for path in paths:
+            print(path)
             id = utils.get_id(path)
             graphs[id] = to_graph(path, anisotropy=anisotropy)
         return graphs
 
     def init_labeled_graphs(self):
         """
         Initializes "self.labeled_graphs" by copying each graph in
@@ -337,18 +340,18 @@
                 xyz = tuple(graph.nodes[i]["xyz"])
                 if xyz in self.xyz_to_id_node.keys():
                     self.xyz_to_id_node[xyz][id] = i
                 else:
                     self.xyz_to_id_node[xyz] = {id: i}
 
     def get_pred_coords(self, label):
-        if label in self.valid_labels.keys():
-            return self.valid_labels[label]
-        else:
-            return []
+        if self.valid_labels:
+            if label in self.valid_labels.keys():
+                return self.valid_labels[label]
+        return []
 
     # -- Final Constructor Routines --
     def init_kdtree(self):
         """
         Builds a KD-Tree from the xyz coordinates from all nodes across all
         graphs contained in "self.graphs".
 
@@ -575,14 +578,15 @@
 
         # Check potential merge sites
         t0 = time()
         with ProcessPoolExecutor() as executor:
             processes = []
             for ids, label in self.detect_potential_merges():
                 id_1, id_2 = tuple(ids)
+                continue
                 processes.append(
                     executor.submit(
                         merge_detection.localize,
                         self.graphs[id_1],
                         self.graphs[id_2],
                         self.id_to_label_nodes[id_1][label],
                         self.id_to_label_nodes[id_2][label],
@@ -602,15 +606,15 @@
                     # print(merge_id, d)
                     detected_merges.add(merge_id)
                     if self.save:
                         self.save_swc(site[0], site[1], "merge")
 
                 # Report process
                 if i > cnt * chunk_size:
-                    # utils.progress_bar(i + 1, len(processes))
+                    utils.progress_bar(i + 1, len(processes))
                     cnt += 1
 
         # Update graph
         for (id_1, id_2), label in detected_merges:
             self.process_merge(id_1, label)
             self.process_merge(id_2, label)
```

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     print("Downloading predicted swc files from cloud...")
     print("# zip files:", len(zip_paths))
     for i, path in enumerate(zip_paths):
         valid_labels.update(download(bucket, path, min_size, anisotropy))
         if i > cnt * chunk_size:
             utils.progress_bar(i + 1, len(zip_paths))
             cnt += 1
+        break
 
     # Report Results
     print("\n#Valid Labels:", len(valid_labels))
     print("")
     return valid_labels
```

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.4
+Version: 4.1.5
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.4/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.5/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

