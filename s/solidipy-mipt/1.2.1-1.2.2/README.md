# Comparing `tmp/solidipy_mipt-1.2.1.tar.gz` & `tmp/solidipy_mipt-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipy_mipt-1.2.1.tar", last modified: Sat May  4 10:32:18 2024, max compression
+gzip compressed data, was "solidipy_mipt-1.2.2.tar", last modified: Sat May  4 10:53:28 2024, max compression
```

## Comparing `solidipy_mipt-1.2.1.tar` & `solidipy_mipt-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.293045 solidipy_mipt-1.2.1/
--rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5931 2024-05-04 10:32:18.290515 solidipy_mipt-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4822 2024-04-10 14:10:06.000000 solidipy_mipt-1.2.1/README.md
--rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 10:32:18.293045 solidipy_mipt-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-05-04 10:31:46.000000 solidipy_mipt-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.173770 solidipy_mipt-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.204351 solidipy_mipt-1.2.1/src/solidipy_mipt/
--rw-rw-rw-   0        0        0      352 2024-05-04 09:01:55.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/__init__.py
--rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/_metrics.py
--rw-rw-rw-   0        0        0     6013 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.254826 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/
--rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/__init__.py
--rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/_np_regressor.py
--rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/_predictor_abc.py
--rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/_wknn.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.259814 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/utils/
--rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/utils/__init__.py
--rw-rw-rw-   0        0        0     1661 2024-05-04 09:18:22.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/utils/distance.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.268436 solidipy_mipt-1.2.1/src/solidipy_mipt/utils/
--rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/utils/__init__.py
--rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/utils/errors.py
--rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/utils/validate.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.284934 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/
--rw-rw-rw-   0        0        0      290 2024-05-04 10:31:31.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/__init__.py
--rw-rw-rw-   0        0        0      739 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/_utils.py
--rw-rw-rw-   0        0        0      329 2024-05-04 09:17:52.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/colors.py
--rw-rw-rw-   0        0        0     4128 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/distribution.py
--rw-rw-rw-   0        0        0     1546 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/regression.py
--rw-rw-rw-   0        0        0     2296 2024-05-04 10:21:08.000000 solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/wknn.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:32:18.288096 solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/
--rw-rw-rw-   0        0        0     5931 2024-05-04 10:32:18.000000 solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2024-05-04 10:32:18.000000 solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 10:32:18.000000 solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-04 10:32:18.000000 solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 10:32:18.000000 solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.552626 solidipy_mipt-1.2.2/
+-rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5931 2024-05-04 10:53:28.550636 solidipy_mipt-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4822 2024-04-10 14:10:06.000000 solidipy_mipt-1.2.2/README.md
+-rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 10:53:28.553819 solidipy_mipt-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-05-04 10:53:17.000000 solidipy_mipt-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.432942 solidipy_mipt-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.462249 solidipy_mipt-1.2.2/src/solidipy_mipt/
+-rw-rw-rw-   0        0        0      352 2024-05-04 09:01:55.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/__init__.py
+-rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/_metrics.py
+-rw-rw-rw-   0        0        0     6183 2024-05-04 10:41:23.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.514125 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/
+-rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_np_regressor.py
+-rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_predictor_abc.py
+-rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_wknn.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.520483 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/
+-rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2024-05-04 09:18:22.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/distance.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.527978 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/
+-rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/errors.py
+-rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/validate.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.544634 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/
+-rw-rw-rw-   0        0        0      341 2024-05-04 10:50:15.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/_utils.py
+-rw-rw-rw-   0        0        0      329 2024-05-04 09:17:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/colors.py
+-rw-rw-rw-   0        0        0     2306 2024-05-04 10:49:49.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/comparison.py
+-rw-rw-rw-   0        0        0     4128 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/distribution.py
+-rw-rw-rw-   0        0        0     1546 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/regression.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.547630 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/
+-rw-rw-rw-   0        0        0     5931 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/top_level.txt
```

### Comparing `solidipy_mipt-1.2.1/LICENSE.txt` & `solidipy_mipt-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/PKG-INFO` & `solidipy_mipt-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.1 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.2 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
```

### Comparing `solidipy_mipt-1.2.1/README.md` & `solidipy_mipt-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/setup.py` & `solidipy_mipt-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="solidipy_mipt",
-    version="1.2.1",
+    version="1.2.2",
     description="Make your ML solid!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework",
     author="Matvei Gorskii",
     author_email="matveygor41@gmail.com",
     classifiers=[
```

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/_metrics.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/_metrics.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/_selection.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,26 +20,34 @@
 
     Args:
         data: The input data.
         key: The function for comparing data.
 
     Returns:
         outliers: Indeces of outliers.
+    
+    Raises:
+        ValueError: If key is not callable.
 
     Examples:
         >>> from solidipy_mipt import get_outliers
         >>> from solidipy_mipt.visualization import visualize_scatter
         >>> import numpy as np
         >>> data = np.array([
         ...     [-500,-500], [1,1], [2,2], [3,3], [4,4],
         ...     [50,50], [60,60],[70,7], [8,8], [900,900]
         ... ])
         >>> print(get_outliers(data))
     """
 
+    if not callable(key):
+        raise ValueError(
+            "Key must be a callable."
+        )
+
     if key:
         data_sorted = data[np.argsort(key(data))]
     else:
         data_sorted = data[data[:, 1].argsort()]
 
     first_quantile = data_sorted[round(data_sorted.shape[0] * 0.25)]
     third_quantile = data_sorted[round(data_sorted.shape[0] * 0.75)]
```

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/_np_regressor.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_np_regressor.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/_predictor_abc.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_predictor_abc.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/_wknn.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_wknn.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/algorithms/utils/distance.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/distance.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/utils/errors.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/utils/errors.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/utils/validate.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/utils/validate.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/_utils.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/distribution.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/distribution.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/regression.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/regression.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt/visualization/wknn.py` & `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/comparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""Visualization of WKNN.
+"""Visualization of comparison.
 
-This module contain methods for WKNN visualization.
+This module contain methods for comparison visualization.
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from itertools import cycle
 from .colors import Colors
@@ -16,19 +16,19 @@
 def visualize_comparison(
     points: np.ndarray,
     prediction: np.ndarray,
     expectation: np.ndarray,
     path_to_save: str = ""
 ) -> None:
     """
-    Visualize WKNN.
+    Visualize comparison.
 
     Args:
         points: Points.
-        prediction: WKNN predicted labels.
+        prediction: Predicted labels.
         expectation: Expected labels.
         path_to_save: Path to save visualization.
             If empty, show visualization in new window.
             Defaults to "".
 
     Examples:
         >>> import numpy as np
@@ -45,24 +45,24 @@
     # TODO chech sizes of input data
 
     _, (ax1, ax2) = plt.subplots(1, 2, figsize=FIGSIZE)
 
     ax1.set_title("prediction", fontsize=15, fontweight="bold", c="dimgray")
     ax2.set_title("expectation", fontsize=15, fontweight="bold", c="dimgray")
 
-    _visualize_scatter(points, prediction, axis=ax1)
-    _visualize_scatter(points, expectation, axis=ax2)
+    visualize_scatter(points, prediction, axis=ax1)
+    visualize_scatter(points, expectation, axis=ax2)
 
     if (path_to_save):
         _save_fig(path_to_save)
     else:
         plt.show()
 
 
-def _visualize_scatter(
+def visualize_scatter(
     points: np.ndarray,
     labels: np.ndarray,
     colors: list[Colors] | None = None,
     axis: plt.Axes | None = None,
 ) -> None:
     """
     Visualize scatter with labels.
```

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/PKG-INFO` & `solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.1 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.2 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
```

### Comparing `solidipy_mipt-1.2.1/src/solidipy_mipt.egg-info/SOURCES.txt` & `solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 src/solidipy_mipt/algorithms/utils/distance.py
 src/solidipy_mipt/utils/__init__.py
 src/solidipy_mipt/utils/errors.py
 src/solidipy_mipt/utils/validate.py
 src/solidipy_mipt/visualization/__init__.py
 src/solidipy_mipt/visualization/_utils.py
 src/solidipy_mipt/visualization/colors.py
+src/solidipy_mipt/visualization/comparison.py
 src/solidipy_mipt/visualization/distribution.py
-src/solidipy_mipt/visualization/regression.py
-src/solidipy_mipt/visualization/wknn.py
+src/solidipy_mipt/visualization/regression.py
```

