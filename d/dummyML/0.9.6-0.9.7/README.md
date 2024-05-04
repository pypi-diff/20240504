# Comparing `tmp/dummyml-0.9.6.tar.gz` & `tmp/dummyml-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dummyml-0.9.6.tar", last modified: Wed May  1 06:15:58 2024, max compression
+gzip compressed data, was "dummyml-0.9.7.tar", last modified: Sat May  4 05:19:53 2024, max compression
```

## Comparing `dummyml-0.9.6.tar` & `dummyml-0.9.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1073 2021-08-31 02:36:50.000000 dummyml-0.9.6/LICENSE.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      183 2021-08-31 02:36:50.000000 dummyml-0.9.6/MANIFEST.in
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1985 2024-05-01 06:15:58.867903 dummyml-0.9.6/PKG-INFO
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      975 2024-05-01 05:08:30.000000 dummyml-0.9.6/README.md
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2021-12-03 04:35:32.000000 dummyml-0.9.6/TODO.md
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      103 2021-08-31 02:36:50.000000 dummyml-0.9.6/pyproject.toml
--rw-rw-r--   0 yipeng    (1000) yipeng    (1000)       38 2024-05-01 06:15:58.867903 dummyml-0.9.6/setup.cfg
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1469 2024-05-01 06:15:36.000000 dummyml-0.9.6/setup.py
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/src/
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/src/dummyML/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)       40 2022-11-24 05:03:26.000000 dummyml-0.9.6/src/dummyML/__init__.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    10219 2022-11-29 00:18:52.000000 dummyml-0.9.6/src/dummyML/automate_analysis.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11477 2022-11-28 22:39:56.000000 dummyml-0.9.6/src/dummyML/automate_modeling_evaluation.py
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/src/dummyML/evaluate_models/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyml-0.9.6/src/dummyML/evaluate_models/__init__.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8836 2022-11-25 04:29:13.000000 dummyml-0.9.6/src/dummyML/evaluate_models/classification_metrics.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8644 2022-11-28 21:06:48.000000 dummyml-0.9.6/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3458 2022-11-24 04:56:55.000000 dummyml-0.9.6/src/dummyML/evaluate_models/regression_metrics.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8673 2022-11-24 05:03:07.000000 dummyml-0.9.6/src/dummyML/preprocessing.py
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/src/dummyML/select_fit_models/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyml-0.9.6/src/dummyML/select_fit_models/__init__.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    29719 2022-11-24 05:03:54.000000 dummyml-0.9.6/src/dummyML/select_fit_models/classification_models.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11845 2022-11-24 05:05:42.000000 dummyml-0.9.6/src/dummyML/select_fit_models/imbalanced_classification_models.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    23287 2022-11-24 05:05:48.000000 dummyml-0.9.6/src/dummyML/select_fit_models/regression_models.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11534 2022-11-24 04:56:55.000000 dummyml-0.9.6/src/dummyML/utilities.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)       90 2024-05-01 06:15:49.000000 dummyml-0.9.6/src/dummyML/version.py
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/src/dummyML.egg-info/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1985 2024-05-01 06:15:58.000000 dummyml-0.9.6/src/dummyML.egg-info/PKG-INFO
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      924 2024-05-01 06:15:58.000000 dummyml-0.9.6/src/dummyML.egg-info/SOURCES.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2024-05-01 06:15:58.000000 dummyml-0.9.6/src/dummyML.egg-info/dependency_links.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)      174 2024-05-01 06:15:58.000000 dummyml-0.9.6/src/dummyML.egg-info/requires.txt
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)        8 2024-05-01 06:15:58.000000 dummyml-0.9.6/src/dummyML.egg-info/top_level.txt
-drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-01 06:15:58.867903 dummyml-0.9.6/tests/
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3918 2022-11-29 00:53:33.000000 dummyml-0.9.6/tests/test_automate_analysis.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1397 2022-11-29 00:54:22.000000 dummyml-0.9.6/tests/test_preprocessing.py
--rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1514 2022-11-29 00:54:36.000000 dummyml-0.9.6/tests/test_utilities.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.099707 dummyml-0.9.7/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1073 2021-08-31 02:36:50.000000 dummyml-0.9.7/LICENSE.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      183 2021-08-31 02:36:50.000000 dummyml-0.9.7/MANIFEST.in
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1991 2024-05-04 05:19:53.099707 dummyml-0.9.7/PKG-INFO
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      975 2024-05-01 05:08:30.000000 dummyml-0.9.7/README.md
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2021-12-03 04:35:32.000000 dummyml-0.9.7/TODO.md
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      103 2021-08-31 02:36:50.000000 dummyml-0.9.7/pyproject.toml
+-rw-rw-r--   0 yipeng    (1000) yipeng    (1000)       38 2024-05-04 05:19:53.099707 dummyml-0.9.7/setup.cfg
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1475 2024-05-04 04:56:51.000000 dummyml-0.9.7/setup.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.095708 dummyml-0.9.7/src/
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.095708 dummyml-0.9.7/src/dummyML/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)       40 2022-11-24 05:03:26.000000 dummyml-0.9.7/src/dummyML/__init__.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    10219 2022-11-29 00:18:52.000000 dummyml-0.9.7/src/dummyML/automate_analysis.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11477 2022-11-28 22:39:56.000000 dummyml-0.9.7/src/dummyML/automate_modeling_evaluation.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.099707 dummyml-0.9.7/src/dummyML/evaluate_models/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyml-0.9.7/src/dummyML/evaluate_models/__init__.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8836 2022-11-25 04:29:13.000000 dummyml-0.9.7/src/dummyML/evaluate_models/classification_metrics.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8644 2022-11-28 21:06:48.000000 dummyml-0.9.7/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3458 2022-11-24 04:56:55.000000 dummyml-0.9.7/src/dummyML/evaluate_models/regression_metrics.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     8673 2022-11-24 05:03:07.000000 dummyml-0.9.7/src/dummyML/preprocessing.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.099707 dummyml-0.9.7/src/dummyML/select_fit_models/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        0 2022-11-24 04:56:55.000000 dummyml-0.9.7/src/dummyML/select_fit_models/__init__.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    29719 2022-11-24 05:03:54.000000 dummyml-0.9.7/src/dummyML/select_fit_models/classification_models.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11845 2022-11-24 05:05:42.000000 dummyml-0.9.7/src/dummyML/select_fit_models/imbalanced_classification_models.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    23287 2022-11-24 05:05:48.000000 dummyml-0.9.7/src/dummyML/select_fit_models/regression_models.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)    11534 2022-11-24 04:56:55.000000 dummyml-0.9.7/src/dummyML/utilities.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)       90 2024-05-04 04:55:16.000000 dummyml-0.9.7/src/dummyML/version.py
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.099707 dummyml-0.9.7/src/dummyML.egg-info/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1991 2024-05-04 05:19:53.000000 dummyml-0.9.7/src/dummyML.egg-info/PKG-INFO
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      924 2024-05-04 05:19:53.000000 dummyml-0.9.7/src/dummyML.egg-info/SOURCES.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        1 2024-05-04 05:19:53.000000 dummyml-0.9.7/src/dummyML.egg-info/dependency_links.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)      174 2024-05-04 05:19:53.000000 dummyml-0.9.7/src/dummyML.egg-info/requires.txt
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)        8 2024-05-04 05:19:53.000000 dummyml-0.9.7/src/dummyML.egg-info/top_level.txt
+drwxrwxr-x   0 yipeng    (1000) yipeng    (1000)        0 2024-05-04 05:19:53.099707 dummyml-0.9.7/tests/
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     3918 2022-11-29 00:53:33.000000 dummyml-0.9.7/tests/test_automate_analysis.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1397 2022-11-29 00:54:22.000000 dummyml-0.9.7/tests/test_preprocessing.py
+-rw-r--r--   0 yipeng    (1000) yipeng    (1000)     1514 2022-11-29 00:54:36.000000 dummyml-0.9.7/tests/test_utilities.py
```

### Comparing `dummyml-0.9.6/LICENSE.txt` & `dummyml-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/PKG-INFO` & `dummyml-0.9.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dummyML
-Version: 0.9.6
+Version: 0.9.7
 Summary: Automated data analysis pipelines on tabular data for data analyst
-Home-page: https://gitlab.com/YipengUva/dummyML_pkg
+Home-page: https://gitlab.com/YipengUva/end2endml_pkg
 Author: Yipeng Song
 Author-email: yipeng.song@hotmail.com
-Project-URL: Bug Tracker, https://gitlab.com/YipengUva/dummyML_pkg/issues
+Project-URL: Bug Tracker, https://gitlab.com/YipengUva/end2endml_pkg/-/issues
 Keywords: data analysis,machine learning,automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy<=1.26,>=1.19
-Requires-Dist: pandas<=1.5,>=1.1
+Requires-Dist: pandas<=1.4,>=1.1
 Requires-Dist: imbalanced-learn<=0.10,>=0.8
 Requires-Dist: scikit-learn<=1.2,>=1.0
 Requires-Dist: pandas-profiling<=3.3,>=2.9
 Requires-Dist: joblib<=1.2,>=1.0
 Requires-Dist: xgboost<=1.5,>=1.4
 Requires-Dist: optuna<=2.10,>=2.7
```

### Comparing `dummyml-0.9.6/README.md` & `dummyml-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/setup.py` & `dummyml-0.9.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # setup
 setup(
     name="dummyML",
-    version="0.9.6",
+    version="0.9.7",
     author="Yipeng Song",
     author_email="yipeng.song@hotmail.com",
     description="Automated data analysis pipelines on tabular data for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitlab.com/YipengUva/dummyML_pkg",
+    url="https://gitlab.com/YipengUva/end2endml_pkg",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords="data analysis, machine learning, automation",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.6,<4",
     install_requires=[
         "numpy>=1.19, <=1.26",
-        "pandas>=1.1, <=1.5",
+        "pandas>=1.1, <=1.4",
         "imbalanced-learn>=0.8, <=0.10",
         "scikit-learn>=1.0, <=1.2",
         "pandas-profiling>=2.9, <=3.3",
         "joblib>=1.0, <=1.2",
         "xgboost>=1.4, <=1.5",
         "optuna>=2.7, <=2.10",
     ],
     project_urls={
-        "Bug Tracker": "https://gitlab.com/YipengUva/dummyML_pkg/issues",
+        "Bug Tracker": "https://gitlab.com/YipengUva/end2endml_pkg/-/issues",
     },
 )
```

### Comparing `dummyml-0.9.6/src/dummyML/automate_analysis.py` & `dummyml-0.9.7/src/dummyML/automate_analysis.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/automate_modeling_evaluation.py` & `dummyml-0.9.7/src/dummyML/automate_modeling_evaluation.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/evaluate_models/classification_metrics.py` & `dummyml-0.9.7/src/dummyML/evaluate_models/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py` & `dummyml-0.9.7/src/dummyML/evaluate_models/classification_metrics_imb_cutoff.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/evaluate_models/regression_metrics.py` & `dummyml-0.9.7/src/dummyML/evaluate_models/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/preprocessing.py` & `dummyml-0.9.7/src/dummyML/preprocessing.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/select_fit_models/classification_models.py` & `dummyml-0.9.7/src/dummyML/select_fit_models/classification_models.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/select_fit_models/imbalanced_classification_models.py` & `dummyml-0.9.7/src/dummyML/select_fit_models/imbalanced_classification_models.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/select_fit_models/regression_models.py` & `dummyml-0.9.7/src/dummyML/select_fit_models/regression_models.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML/utilities.py` & `dummyml-0.9.7/src/dummyML/utilities.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/src/dummyML.egg-info/PKG-INFO` & `dummyml-0.9.7/src/dummyML.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dummyML
-Version: 0.9.6
+Version: 0.9.7
 Summary: Automated data analysis pipelines on tabular data for data analyst
-Home-page: https://gitlab.com/YipengUva/dummyML_pkg
+Home-page: https://gitlab.com/YipengUva/end2endml_pkg
 Author: Yipeng Song
 Author-email: yipeng.song@hotmail.com
-Project-URL: Bug Tracker, https://gitlab.com/YipengUva/dummyML_pkg/issues
+Project-URL: Bug Tracker, https://gitlab.com/YipengUva/end2endml_pkg/-/issues
 Keywords: data analysis,machine learning,automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy<=1.26,>=1.19
-Requires-Dist: pandas<=1.5,>=1.1
+Requires-Dist: pandas<=1.4,>=1.1
 Requires-Dist: imbalanced-learn<=0.10,>=0.8
 Requires-Dist: scikit-learn<=1.2,>=1.0
 Requires-Dist: pandas-profiling<=3.3,>=2.9
 Requires-Dist: joblib<=1.2,>=1.0
 Requires-Dist: xgboost<=1.5,>=1.4
 Requires-Dist: optuna<=2.10,>=2.7
```

### Comparing `dummyml-0.9.6/src/dummyML.egg-info/SOURCES.txt` & `dummyml-0.9.7/src/dummyML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/tests/test_automate_analysis.py` & `dummyml-0.9.7/tests/test_automate_analysis.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/tests/test_preprocessing.py` & `dummyml-0.9.7/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `dummyml-0.9.6/tests/test_utilities.py` & `dummyml-0.9.7/tests/test_utilities.py`

 * *Files identical despite different names*

