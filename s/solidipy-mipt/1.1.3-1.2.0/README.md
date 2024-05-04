# Comparing `tmp/solidipy_mipt-1.1.3.tar.gz` & `tmp/solidipy_mipt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipy_mipt-1.1.3.tar", last modified: Tue Apr  9 13:45:58 2024, max compression
+gzip compressed data, was "solidipy_mipt-1.2.0.tar", last modified: Sat May  4 10:23:40 2024, max compression
```

## Comparing `solidipy_mipt-1.1.3.tar` & `solidipy_mipt-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:58.000837 solidipy_mipt-1.1.3/
--rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5921 2024-04-09 13:45:57.998843 solidipy_mipt-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4812 2024-04-07 16:19:13.000000 solidipy_mipt-1.1.3/README.md
--rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 13:45:58.000837 solidipy_mipt-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-04-09 13:45:44.000000 solidipy_mipt-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.947562 solidipy_mipt-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.962024 solidipy_mipt-1.1.3/src/solidipy_mipt/
--rw-rw-rw-   0        0        0      266 2024-04-06 05:51:26.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/__init__.py
--rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/_metrics.py
--rw-rw-rw-   0        0        0     4584 2024-04-07 15:46:23.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.988837 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/
--rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/__init__.py
--rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_np_regressor.py
--rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_predictor_abc.py
--rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_wknn.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.991845 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/
--rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/__init__.py
--rw-rw-rw-   0        0        0     1638 2024-04-07 05:01:27.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/distance.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.995839 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/
--rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/__init__.py
--rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/errors.py
--rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/validate.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.997839 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/
--rw-rw-rw-   0        0        0     5921 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.225946 solidipy_mipt-1.2.0/
+-rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5931 2024-05-04 10:23:40.223126 solidipy_mipt-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4822 2024-04-10 14:10:06.000000 solidipy_mipt-1.2.0/README.md
+-rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 10:23:40.226940 solidipy_mipt-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-04-28 19:57:45.000000 solidipy_mipt-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.083671 solidipy_mipt-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.127347 solidipy_mipt-1.2.0/src/solidipy_mipt/
+-rw-rw-rw-   0        0        0      352 2024-05-04 09:01:55.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/__init__.py
+-rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/_metrics.py
+-rw-rw-rw-   0        0        0     6013 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.187864 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/
+-rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/_np_regressor.py
+-rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/_predictor_abc.py
+-rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/_wknn.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.193207 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/utils/
+-rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2024-05-04 09:18:22.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/utils/distance.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.201311 solidipy_mipt-1.2.0/src/solidipy_mipt/utils/
+-rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/utils/errors.py
+-rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/utils/validate.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.217547 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/
+-rw-rw-rw-   0        0        0      287 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/_utils.py
+-rw-rw-rw-   0        0        0      329 2024-05-04 09:17:52.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/colors.py
+-rw-rw-rw-   0        0        0     4128 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/distribution.py
+-rw-rw-rw-   0        0        0     1546 2024-05-04 10:20:52.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/regression.py
+-rw-rw-rw-   0        0        0     2296 2024-05-04 10:21:08.000000 solidipy_mipt-1.2.0/src/solidipy_mipt/visualization/wknn.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:23:40.220577 solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/
+-rw-rw-rw-   0        0        0     5931 2024-05-04 10:23:39.000000 solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2024-05-04 10:23:40.000000 solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 10:23:39.000000 solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-04 10:23:39.000000 solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 10:23:39.000000 solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/top_level.txt
```

### Comparing `solidipy_mipt-1.1.3/LICENSE.txt` & `solidipy_mipt-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/PKG-INFO` & `solidipy_mipt-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.1.3
+Version: 1.2.0
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
@@ -85,15 +85,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <a id="built-with"></a>
 
 ### Built With
 
-Major frameworks/libraries used to bootstrap solidipy.
+Major frameworks/libraries used to bootstrap solidipy-mipt.
 
 * [NumPy](https://numpy.org/)
 * [Matplotlib](https://matplotlib.org/)
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
@@ -112,15 +112,15 @@
 
 Before installing *Solidipy-MIPT* make sure you have last version of Python3 and pip.
 
 <a id="installation"></a>
 
 ### Installation
 
-You can install solidipy using pip:
+You can install solidipy-mipt using pip:
 
 ```bash
 pip install solidipy-mipt
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.3 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.0 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
@@ -28,21 +28,21 @@
    5. _L_i_c_e_n_s_e
    6. _C_o_n_t_a_c_t
 ## About The Project *Solidipy-MIPT* is a Python library designed to provide a
 solid foundation for machine learning tasks. It includes various machine
 learning algorithms such as Weighted k-nearest neighbors (WKNN) and
 regressions, along with evaluation metrics to assess model performance.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Built With Major frameworks/libraries used to bootstrap solidipy. * [NumPy]
-(https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
+### Built With Major frameworks/libraries used to bootstrap solidipy-mipt. *
+[NumPy](https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites Before installing *Solidipy-MIPT* make sure
 you have last version of Python3 and pip. ### Installation You can install
-solidipy using pip: ```bash pip install solidipy-mipt ```
+solidipy-mipt using pip: ```bash pip install solidipy-mipt ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage #### Simple Weighted KNN example ```python import numpy as np from
 solidipy_mipt import accuracy from solidipy_mipt.algorithms import WKNN X =
 np.array([[1, 2], [3, 4], [5, 6], [7, 8]]) y = np.array([0, 1, 0, 1]) X_train,
 X_test, y_train, y_test = train_test_split( X, y, train_ratio=0.6, shuffle=True
 ) wknn = WKNN() wknn.fit(X_train, y_train) prediction = wknn.predict(X_test)
 print(accuracy(prediction, y_test)) ``` _For more examples, please refer to the
```

### Comparing `solidipy_mipt-1.1.3/README.md` & `solidipy_mipt-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <a id="built-with"></a>
 
 ### Built With
 
-Major frameworks/libraries used to bootstrap solidipy.
+Major frameworks/libraries used to bootstrap solidipy-mipt.
 
 * [NumPy](https://numpy.org/)
 * [Matplotlib](https://matplotlib.org/)
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
@@ -87,15 +87,15 @@
 
 Before installing *Solidipy-MIPT* make sure you have last version of Python3 and pip.
 
 <a id="installation"></a>
 
 ### Installation
 
-You can install solidipy using pip:
+You can install solidipy-mipt using pip:
 
 ```bash
 pip install solidipy-mipt
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -14,21 +14,21 @@
    5. _L_i_c_e_n_s_e
    6. _C_o_n_t_a_c_t
 ## About The Project *Solidipy-MIPT* is a Python library designed to provide a
 solid foundation for machine learning tasks. It includes various machine
 learning algorithms such as Weighted k-nearest neighbors (WKNN) and
 regressions, along with evaluation metrics to assess model performance.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Built With Major frameworks/libraries used to bootstrap solidipy. * [NumPy]
-(https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
+### Built With Major frameworks/libraries used to bootstrap solidipy-mipt. *
+[NumPy](https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites Before installing *Solidipy-MIPT* make sure
 you have last version of Python3 and pip. ### Installation You can install
-solidipy using pip: ```bash pip install solidipy-mipt ```
+solidipy-mipt using pip: ```bash pip install solidipy-mipt ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage #### Simple Weighted KNN example ```python import numpy as np from
 solidipy_mipt import accuracy from solidipy_mipt.algorithms import WKNN X =
 np.array([[1, 2], [3, 4], [5, 6], [7, 8]]) y = np.array([0, 1, 0, 1]) X_train,
 X_test, y_train, y_test = train_test_split( X, y, train_ratio=0.6, shuffle=True
 ) wknn = WKNN() wknn.fit(X_train, y_train) prediction = wknn.predict(X_test)
 print(accuracy(prediction, y_test)) ``` _For more examples, please refer to the
```

### Comparing `solidipy_mipt-1.1.3/setup.py` & `solidipy_mipt-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="solidipy_mipt",
-    version="1.1.3",
+    version="1.2.0",
     description="Make your ML solid!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework",
     author="Matvei Gorskii",
     author_email="matveygor41@gmail.com",
     classifiers=[
```

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/_metrics.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/_metrics.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_np_regressor.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/_np_regressor.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_predictor_abc.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/_predictor_abc.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_wknn.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/_wknn.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/distance.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/algorithms/utils/distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from enum import Enum
 from ...utils.validate import check_size
 
 
 class Metric(Enum):
     """
-    Metric.
+    Metric for calculate distance.
     """
 
     EUCLIDEAN = 1
     MANHATTAN = 2
 
 
 def get_distances(
```

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/utils/errors.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/utils/errors.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt/utils/validate.py` & `solidipy_mipt-1.2.0/src/solidipy_mipt/utils/validate.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/PKG-INFO` & `solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.1.3
+Version: 1.2.0
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
@@ -85,15 +85,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <a id="built-with"></a>
 
 ### Built With
 
-Major frameworks/libraries used to bootstrap solidipy.
+Major frameworks/libraries used to bootstrap solidipy-mipt.
 
 * [NumPy](https://numpy.org/)
 * [Matplotlib](https://matplotlib.org/)
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
@@ -112,15 +112,15 @@
 
 Before installing *Solidipy-MIPT* make sure you have last version of Python3 and pip.
 
 <a id="installation"></a>
 
 ### Installation
 
-You can install solidipy using pip:
+You can install solidipy-mipt using pip:
 
 ```bash
 pip install solidipy-mipt
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.3 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.2.0 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
@@ -28,21 +28,21 @@
    5. _L_i_c_e_n_s_e
    6. _C_o_n_t_a_c_t
 ## About The Project *Solidipy-MIPT* is a Python library designed to provide a
 solid foundation for machine learning tasks. It includes various machine
 learning algorithms such as Weighted k-nearest neighbors (WKNN) and
 regressions, along with evaluation metrics to assess model performance.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-### Built With Major frameworks/libraries used to bootstrap solidipy. * [NumPy]
-(https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
+### Built With Major frameworks/libraries used to bootstrap solidipy-mipt. *
+[NumPy](https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites Before installing *Solidipy-MIPT* make sure
 you have last version of Python3 and pip. ### Installation You can install
-solidipy using pip: ```bash pip install solidipy-mipt ```
+solidipy-mipt using pip: ```bash pip install solidipy-mipt ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage #### Simple Weighted KNN example ```python import numpy as np from
 solidipy_mipt import accuracy from solidipy_mipt.algorithms import WKNN X =
 np.array([[1, 2], [3, 4], [5, 6], [7, 8]]) y = np.array([0, 1, 0, 1]) X_train,
 X_test, y_train, y_test = train_test_split( X, y, train_ratio=0.6, shuffle=True
 ) wknn = WKNN() wknn.fit(X_train, y_train) prediction = wknn.predict(X_test)
 print(accuracy(prediction, y_test)) ``` _For more examples, please refer to the
```

### Comparing `solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/SOURCES.txt` & `solidipy_mipt-1.2.0/src/solidipy_mipt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,8 +14,14 @@
 src/solidipy_mipt/algorithms/_np_regressor.py
 src/solidipy_mipt/algorithms/_predictor_abc.py
 src/solidipy_mipt/algorithms/_wknn.py
 src/solidipy_mipt/algorithms/utils/__init__.py
 src/solidipy_mipt/algorithms/utils/distance.py
 src/solidipy_mipt/utils/__init__.py
 src/solidipy_mipt/utils/errors.py
-src/solidipy_mipt/utils/validate.py
+src/solidipy_mipt/utils/validate.py
+src/solidipy_mipt/visualization/__init__.py
+src/solidipy_mipt/visualization/_utils.py
+src/solidipy_mipt/visualization/colors.py
+src/solidipy_mipt/visualization/distribution.py
+src/solidipy_mipt/visualization/regression.py
+src/solidipy_mipt/visualization/wknn.py
```

