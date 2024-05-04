# Comparing `tmp/solidipy_mipt-1.2.2.tar.gz` & `tmp/solidipy_mipt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipy_mipt-1.2.2.tar", last modified: Sat May  4 10:53:28 2024, max compression
+gzip compressed data, was "solidipy_mipt-1.2.3.tar", last modified: Sat May  4 11:22:21 2024, max compression
```

## Comparing `solidipy_mipt-1.2.2.tar` & `solidipy_mipt-1.2.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.552626 solidipy_mipt-1.2.2/
--rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5931 2024-05-04 10:53:28.550636 solidipy_mipt-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4822 2024-04-10 14:10:06.000000 solidipy_mipt-1.2.2/README.md
--rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 10:53:28.553819 solidipy_mipt-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-05-04 10:53:17.000000 solidipy_mipt-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.432942 solidipy_mipt-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.462249 solidipy_mipt-1.2.2/src/solidipy_mipt/
--rw-rw-rw-   0        0        0      352 2024-05-04 09:01:55.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/__init__.py
--rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/_metrics.py
--rw-rw-rw-   0        0        0     6183 2024-05-04 10:41:23.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.514125 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/
--rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/__init__.py
--rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_np_regressor.py
--rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_predictor_abc.py
--rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_wknn.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.520483 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/
--rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/__init__.py
--rw-rw-rw-   0        0        0     1661 2024-05-04 09:18:22.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/distance.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.527978 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/
--rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/__init__.py
--rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/errors.py
--rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/utils/validate.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.544634 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/
--rw-rw-rw-   0        0        0      341 2024-05-04 10:50:15.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/__init__.py
--rw-rw-rw-   0        0        0      739 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/_utils.py
--rw-rw-rw-   0        0        0      329 2024-05-04 09:17:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/colors.py
--rw-rw-rw-   0        0        0     2306 2024-05-04 10:49:49.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/comparison.py
--rw-rw-rw-   0        0        0     4128 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/distribution.py
--rw-rw-rw-   0        0        0     1546 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/regression.py
-drwxrwxrwx   0        0        0        0 2024-05-04 10:53:28.547630 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/
--rw-rw-rw-   0        0        0     5931 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 10:53:28.000000 solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.608171 solidipy_mipt-1.2.3/
+-rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5931 2024-05-04 11:22:21.606055 solidipy_mipt-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4822 2024-04-10 14:10:06.000000 solidipy_mipt-1.2.3/README.md
+-rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 11:22:21.608171 solidipy_mipt-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-05-04 11:21:57.000000 solidipy_mipt-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.494249 solidipy_mipt-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.519156 solidipy_mipt-1.2.3/src/solidipy_mipt/
+-rw-rw-rw-   0        0        0      352 2024-05-04 09:01:55.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/__init__.py
+-rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/_metrics.py
+-rw-rw-rw-   0        0        0     6205 2024-05-04 11:00:39.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.567972 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/
+-rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/_np_regressor.py
+-rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/_predictor_abc.py
+-rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/_wknn.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.572974 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/utils/
+-rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2024-05-04 09:18:22.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/utils/distance.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.582635 solidipy_mipt-1.2.3/src/solidipy_mipt/utils/
+-rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/utils/errors.py
+-rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/utils/validate.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.600751 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/
+-rw-rw-rw-   0        0        0      495 2024-05-04 11:17:20.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/_utils.py
+-rw-rw-rw-   0        0        0     1963 2024-05-04 11:16:31.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/base_diagrams.py
+-rw-rw-rw-   0        0        0      329 2024-05-04 09:17:52.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/colors.py
+-rw-rw-rw-   0        0        0     1493 2024-05-04 11:07:16.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/comparison.py
+-rw-rw-rw-   0        0        0     3603 2024-05-04 11:21:47.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/distribution.py
+-rw-rw-rw-   0        0        0     1461 2024-05-04 10:59:08.000000 solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/regression.py
+drwxrwxrwx   0        0        0        0 2024-05-04 11:22:21.602759 solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/
+-rw-rw-rw-   0        0        0     5931 2024-05-04 11:22:21.000000 solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2024-05-04 11:22:21.000000 solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 11:22:21.000000 solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-04 11:22:21.000000 solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 11:22:21.000000 solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/top_level.txt
```

### Comparing `solidipy_mipt-1.2.2/LICENSE.txt` & `solidipy_mipt-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/PKG-INFO` & `solidipy_mipt-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.2.2
+Version: 1.2.3
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
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.2 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.3 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
```

### Comparing `solidipy_mipt-1.2.2/README.md` & `solidipy_mipt-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/setup.py` & `solidipy_mipt-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="solidipy_mipt",
-    version="1.2.2",
+    version="1.2.3",
     description="Make your ML solid!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework",
     author="Matvei Gorskii",
     author_email="matveygor41@gmail.com",
     classifiers=[
```

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/_metrics.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/_metrics.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/_selection.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,30 +35,30 @@
         >>> data = np.array([
         ...     [-500,-500], [1,1], [2,2], [3,3], [4,4],
         ...     [50,50], [60,60],[70,7], [8,8], [900,900]
         ... ])
         >>> print(get_outliers(data))
     """
 
-    if not callable(key):
-        raise ValueError(
-            "Key must be a callable."
-        )
-
     if key:
+        if not callable(key):
+            raise ValueError(
+                "Key must be a callable."
+            )
+        
         data_sorted = data[np.argsort(key(data))]
     else:
         data_sorted = data[data[:, 1].argsort()]
 
     first_quantile = data_sorted[round(data_sorted.shape[0] * 0.25)]
     third_quantile = data_sorted[round(data_sorted.shape[0] * 0.75)]
     e = (third_quantile - first_quantile) * 1.5
 
-    mask1 = np.prod(data < first_quantile - e, axis=1).astype(np.bool_)
-    mask2 = np.prod(data > third_quantile + e, axis=1).astype(np.bool_)
+    mask1 = np.any(data < first_quantile - e, axis=1).astype(np.bool_)
+    mask2 = np.any(data > third_quantile + e, axis=1).astype(np.bool_)
     outliers = np.arange(0, data.shape[0])
 
     return outliers[mask1 + mask2]
 
 
 def train_test_split(
     X: np.ndarray,
```

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_np_regressor.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/_np_regressor.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_predictor_abc.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/_predictor_abc.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/_wknn.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/_wknn.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/algorithms/utils/distance.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/algorithms/utils/distance.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/utils/errors.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/utils/errors.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/utils/validate.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/utils/validate.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/_utils.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/distribution.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/distribution.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 This module contain methods for distribution visualization.
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from enum import IntEnum
+from .base_diagrams import (
+    visualize_scatter,
+    visualize_violin,
+    visualize_hist,
+    visualize_boxplot
+)
 from ._utils import _save_fig
 
 
 class DiagramType(IntEnum):
     VIOLIN = 1
     HIST = 2
     BOXPLOT = 3
@@ -30,15 +36,14 @@
     Visualize distribution. If distribution is 2D visualize 2 histograms,
       which provides additional information about the distribution of data along the axes.
 
     Args:
         data: The input data for distribution.
         diagram_type: The diagram type.
         path_to_save: Path to save visualization.
-            If empty, show visualization in new window.
             Defaults to "".
 
     Examples:
         >>> import numpy as np
         >>> from solidipy_mipt.visualization import visualize_distribution
         >>> absc = np.random.normal(size=1000)
         >>> ordi = np.random.normal(size=1000)
@@ -65,64 +70,41 @@
     """
     Visualize distribution.
 
     Args:
         data: Data for distribution.
         diagram_type: The diagram type.
         path_to_save: Path to save visualization.
-            If empty, show visualization in new window.
     """
 
     _, axis = plt.subplots(figsize=FIGSIZE)
 
     match(diagram_type):
         case DiagramType.VIOLIN:
-            axis.violinplot(
-                data,
-                vert=False,
-                showmedians=True,
-            )
-            axis.set_yticks([])
-
+            visualize_violin(data, axis)
         case DiagramType.HIST:
-            axis.hist(
-                data,
-                bins=100,
-                color="cornflowerblue",
-                density=True,
-                alpha=0.5,
-            )
-
+            visualize_hist(data, axis)
         case DiagramType.BOXPLOT:
-            axis.boxplot(
-                data,
-                vert=False,
-                patch_artist=True,
-                boxprops=dict(facecolor="blue"),
-                medianprops=dict(color="black"),
-            )
-
+            visualize_boxplot(data, axis)
     if (path_to_save):
         _save_fig(path_to_save)
-    else:
-        plt.show()
 
 
 def _visualize_distribution_2d(
     data: np.ndarray,
     path_to_save: str = "",
 ) -> None:
     """
     Visualize distribution and 2 histograms,
       which provides additional information about the distribution of data along the axes.
 
     Args:
         data: Data for distribution.
         path_to_save: Path to save visualization.
-            If empty, show visualization in new window.
+            Defaults to "".
     """
 
     figure = plt.figure(figsize=(8, 8))
     grid = plt.GridSpec(4, 4, wspace=SPACE, hspace=SPACE)
 
     axis_scatter = figure.add_subplot(grid[:-1, 1:])
     axis_hist_vert = figure.add_subplot(
@@ -158,9 +140,7 @@
     )
 
     axis_hist_hor.invert_yaxis()
     axis_hist_vert.invert_xaxis()
 
     if (path_to_save):
         _save_fig(path_to_save)
-    else:
-        plt.show()
```

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt/visualization/regression.py` & `solidipy_mipt-1.2.3/src/solidipy_mipt/visualization/regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
     Args:
         abscessa: Abscissa of data.
         ordinates: Ordinates of data.
         prediction: Regressor prediction.
         error: Prediction error.
         path_to_save: Path to save visualization.
-            If empty, show visualization in new window.
             Defaults to "".
 
     Examples:
         >>> import numpy as np
         >>> from solidipy_mipt import train_test_split
         >>> X = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
         >>> y = np.array([0, 1, 0, 1])
@@ -46,9 +45,7 @@
     axis.plot(abscissa, predictions - error, label='error', linestyle='--', c="red")
     axis.plot(abscissa, predictions + error, linestyle='--', c="red")
     axis.set_xlim(min(abscissa), max(abscissa))
     axis.legend()
 
     if (path_to_save):
         _save_fig(path_to_save)
-    else:
-        plt.show()
```

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/PKG-INFO` & `solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.2.2
+Version: 1.2.3
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
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.2 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.3 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
```

### Comparing `solidipy_mipt-1.2.2/src/solidipy_mipt.egg-info/SOURCES.txt` & `solidipy_mipt-1.2.3/src/solidipy_mipt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 src/solidipy_mipt/algorithms/utils/__init__.py
 src/solidipy_mipt/algorithms/utils/distance.py
 src/solidipy_mipt/utils/__init__.py
 src/solidipy_mipt/utils/errors.py
 src/solidipy_mipt/utils/validate.py
 src/solidipy_mipt/visualization/__init__.py
 src/solidipy_mipt/visualization/_utils.py
+src/solidipy_mipt/visualization/base_diagrams.py
 src/solidipy_mipt/visualization/colors.py
 src/solidipy_mipt/visualization/comparison.py
 src/solidipy_mipt/visualization/distribution.py
 src/solidipy_mipt/visualization/regression.py
```

