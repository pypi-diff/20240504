# Comparing `tmp/pretty-confusion-matrix-0.1.1.tar.gz` & `tmp/pretty_confusion_matrix-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretty-confusion-matrix-0.1.1.tar", max compression
+gzip compressed data, was "pretty_confusion_matrix-0.2.0.tar", max compression
```

## Comparing `pretty-confusion-matrix-0.1.1.tar` & `pretty_confusion_matrix-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2021-11-17 02:23:54.483232 pretty-confusion-matrix-0.1.1/LICENSE
--rw-r--r--   0        0        0     2763 2021-11-17 03:12:46.969094 pretty-confusion-matrix-0.1.1/README.md
--rw-r--r--   0        0        0       68 2021-11-17 03:17:09.570851 pretty-confusion-matrix-0.1.1/pretty_confusion_matrix/__init__.py
--rw-r--r--   0        0        0     8339 2021-11-19 14:27:06.781409 pretty-confusion-matrix-0.1.1/pretty_confusion_matrix/pretty_confusion_matrix.py
--rw-r--r--   0        0        0      845 2021-11-19 14:28:14.257309 pretty-confusion-matrix-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3801 2021-11-19 14:28:16.645305 pretty-confusion-matrix-0.1.1/setup.py
--rw-r--r--   0        0        0     3793 2021-11-19 14:28:16.645528 pretty-confusion-matrix-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-28 14:40:30.438224 pretty_confusion_matrix-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3423 2022-09-28 14:47:16.857834 pretty_confusion_matrix-0.2.0/README.md
+-rw-r--r--   0        0        0       68 2022-09-28 14:40:30.446224 pretty_confusion_matrix-0.2.0/pretty_confusion_matrix/__init__.py
+-rw-r--r--   0        0        0     8281 2022-09-28 14:40:30.446224 pretty_confusion_matrix-0.2.0/pretty_confusion_matrix/pretty_confusion_matrix.py
+-rw-r--r--   0        0        0     1022 2024-05-04 05:07:09.076545 pretty_confusion_matrix-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 pretty_confusion_matrix-0.2.0/PKG-INFO
```

### Comparing `pretty-confusion-matrix-0.1.1/LICENSE` & `pretty_confusion_matrix-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretty-confusion-matrix-0.1.1/pretty_confusion_matrix/pretty_confusion_matrix.py` & `pretty_confusion_matrix-0.2.0/pretty_confusion_matrix/pretty_confusion_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,17 +268,14 @@
 
         columns = [
             "class %s" % (i)
             for i in list(ascii_uppercase)[0 : len(np.unique(y_test))]
         ]
 
     confm = confusion_matrix(y_test, predictions)
-    fz = 11
-    figsize = [9, 9]
-    show_null_values = 2
     df_cm = DataFrame(confm, index=columns, columns=columns)
     pp_matrix(
         df_cm,
         fz=fz,
         cmap=cmap,
         figsize=figsize,
         show_null_values=show_null_values,
```

### Comparing `pretty-confusion-matrix-0.1.1/pyproject.toml` & `pretty_confusion_matrix-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 [tool.poetry]
 name = "pretty-confusion-matrix"
-version = "0.1.1"
+version = "0.2.0"
 description = "plot a pretty confusion matrix (like Matlab) in python using seaborn and matplotlib"
 repository = "https://github.com/wcipriano/pretty-print-confusion-matrix"
-authors = ["Khuyen Tran <khuyentran1476@gmail.com>"]
+authors = ["Wagner Cipriano <wagnao@gmail.com>", "Khuyen Tran <khuyentran1476@gmail.com>"]
 keywords = ["confusion matrix"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
-matplotlib = "^3.5.0"
-seaborn = "^0.11.2"
-pandas = "^1.3.4"
-numpy = "^1.21.4"
-sklearn = "^0.0"
-pre-commit = "^2.12.1"
-black = "^21.5b0"
-flake8 = "^3.9.2"
-isort = "^5.8.0"
+python = ">=3.8,<3.12"
+numpy = "^1.24.4"
+matplotlib = [
+    {version = "<=3.8", python = "<=3.8"},
+    {version = "<=4.0", python = ">3.8"},
+]
+seaborn = "^0.13.2"
+pandas = [
+    {version = "<2.1", python = "<3.9"},
+    {version = "<2.3", python = ">=3.9"},
+]
+scikit-learn = "^1.3.2"
 
 [tool.poetry.dev-dependencies]
+pre-commit = "^3.5.0"
+black = "^24.4.2"
+flake8 = "^5.0.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
 	\.git
 | \.hg
```

### Comparing `pretty-confusion-matrix-0.1.1/setup.py` & `pretty_confusion_matrix-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,76 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Confusion Matrix in Python
+Plot a pretty confusion matrix (like Matlab) in python using seaborn and matplotlib
 
-packages = \
-['pretty_confusion_matrix']
+Created on Mon Jun 25 14:17:37 2018
+@author: Wagner Cipriano - wagnerbhbr
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['black>=21.5b0,<22.0',
- 'flake8>=3.9.2,<4.0.0',
- 'isort>=5.8.0,<6.0.0',
- 'matplotlib>=3.5.0,<4.0.0',
- 'numpy>=1.21.4,<2.0.0',
- 'pandas>=1.3.4,<2.0.0',
- 'pre-commit>=2.12.1,<3.0.0',
- 'seaborn>=0.11.2,<0.12.0',
- 'sklearn>=0.0,<0.1']
-
-setup_kwargs = {
-    'name': 'pretty-confusion-matrix',
-    'version': '0.1.1',
-    'description': 'plot a pretty confusion matrix (like Matlab) in python using seaborn and matplotlib',
-    'long_description': "# Confusion Matrix in Python\nPlot a pretty confusion matrix (like Matlab) in python using seaborn and matplotlib\n\n\nCreated on Mon Jun 25 14:17:37 2018\n@author: Wagner Cipriano - wagnerbhbr\n\n\nThis module get a pretty print confusion matrix from a NumPy matrix or from 2 NumPy arrays (`y_test` and `predictions`).\n\n## Installation\n```bash\npip install pretty-confusion-matrix\n```\n\n## Get Started\n\nExamples:\n```python\nimport numpy as np\nimport pandas as pd\nfrom pretty_confusion_matrix import pp_matrix\n\narray = np.array([[13,  0,  1,  0,  2,  0],\n                  [0, 50,  2,  0, 10,  0],\n                  [0, 13, 16,  0,  0,  3],\n                  [0,  0,  0, 13,  1,  0],\n                  [0, 40,  0,  1, 15,  0],\n                  [0,  0,  0,  0,  0, 20]])\n\n# get pandas dataframe\ndf_cm = pd.DataFrame(array, index=range(1, 7), columns=range(1, 7))\n# colormap: see this and choose your more dear\ncmap = 'PuRd'\npp_matrix(df_cm, cmap=cmap)\n```\n![alt text](https://raw.githubusercontent.com/khuyentran1401/pretty-print-confusion-matrix/master/Screenshots/Conf_matrix_default.png)\n\n```python\nimport numpy as np\nfrom pretty_confusion_matrix import pp_matrix_from_data\n\ny_test = np.array([1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2,\n                  3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5])\npredic = np.array([1, 2, 4, 3, 5, 1, 2, 4, 3, 5, 1, 2, 3, 4, 4, 1, 4, 3, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 3, 3, 5, 1, 2, 3, 3, 5, 1, 2,\n                  3, 4, 4, 1, 2, 3, 4, 1, 1, 2, 3, 4, 1, 1, 2, 3, 4, 1, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5])\n\npp_matrix_from_data(y_test, predic)\n```\n\n![alt text](https://raw.githubusercontent.com/khuyentran1401/pretty-print-confusion-matrix/master/Screenshots/Conf_matrix_default_2.png)\n\n\n\n\n## References:\n1. Mat lab confusion matrix\n\n   https://www.mathworks.com/help/nnet/ref/plotconfusion.html\n   \n   https://www.mathworks.com/help/examples/nnet/win64/PlotConfusionMatrixUsingCategoricalLabelsExample_02.png\n\n   https://stackoverflow.com/questions/5821125/how-to-plot-confusion-matrix-with-string-axis-rather-than-integer-in-python/51176855#51176855\n\n\n2. Other Examples in python\n  \n  a) https://stackoverflow.com/a/51176855/1809554\n  \n  b) https://www.programcreek.com/python/example/96197/seaborn.heatmap\n\n  c) http://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html#sphx-glr-auto-examples-model-selection-plot-confusion-matrix-py\n",
-    'author': 'Khuyen Tran',
-    'author_email': 'khuyentran1476@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/wcipriano/pretty-print-confusion-matrix',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
-}
+This module get a pretty print confusion matrix from a NumPy matrix or from 2 NumPy arrays (`y_test` and `predictions`).
 
+## Installation
+```bash
+pip install pretty-confusion-matrix
+```
+
+## Get Started
+
+Examples:
+```python
+import numpy as np
+import pandas as pd
+from pretty_confusion_matrix import pp_matrix
+
+array = np.array([[13,  0,  1,  0,  2,  0],
+                  [0, 50,  2,  0, 10,  0],
+                  [0, 13, 16,  0,  0,  3],
+                  [0,  0,  0, 13,  1,  0],
+                  [0, 40,  0,  1, 15,  0],
+                  [0,  0,  0,  0,  0, 20]])
+
+# get pandas dataframe
+df_cm = pd.DataFrame(array, index=range(1, 7), columns=range(1, 7))
+# colormap: see this and choose your more dear
+cmap = 'PuRd'
+pp_matrix(df_cm, cmap=cmap)
+```
+![alt text](https://raw.githubusercontent.com/khuyentran1401/pretty-print-confusion-matrix/master/Screenshots/Conf_matrix_default.png)
+
+```python
+import numpy as np
+from pretty_confusion_matrix import pp_matrix_from_data
+
+y_test = np.array([1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2,
+                  3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
+predic = np.array([1, 2, 4, 3, 5, 1, 2, 4, 3, 5, 1, 2, 3, 4, 4, 1, 4, 3, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 3, 3, 5, 1, 2, 3, 3, 5, 1, 2,
+                  3, 4, 4, 1, 2, 3, 4, 1, 1, 2, 3, 4, 1, 1, 2, 3, 4, 1, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 4, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
+
+pp_matrix_from_data(y_test, predic)
+```
+
+![alt text](https://raw.githubusercontent.com/khuyentran1401/pretty-print-confusion-matrix/master/Screenshots/Conf_matrix_default_2.png)
+
+
+
+## References:
+### 1. MATLAB confusion matrix:
+
+a) [Plot Confusion](https://www.mathworks.com/help/nnet/ref/plotconfusion.html)
+   
+b) [Plot Confusion Matrix Using Categorical Labels](https://www.mathworks.com/help/examples/nnet/win64/PlotConfusionMatrixUsingCategoricalLabelsExample_02.png)
+
+
+
+### 2. Examples and more on Python:
+
+  a) [How to plot confusion matrix with string axis rather than integer in python](https://stackoverflow.com/questions/5821125/how-to-plot-confusion-matrix-with-string-axis-rather-than-integer-in-python/51176855#51176855)
+  
+  b) [Plot-scikit-learn-classification-report](https://stackoverflow.com/questions/28200786/how-to-plot-scikit-learn-classification-report)
+  
+  c) [Plot-confusion-matrix-with-string-axis-rather-than-integer-in-Python](https://stackoverflow.com/questions/5821125/how-to-plot-confusion-matrix-with-string-axis-rather-than-integer-in-python)
+  
+  d) [Seaborn heatmap](https://www.programcreek.com/python/example/96197/seaborn.heatmap)
+  
+  e) [Sklearn-plot-confusion-matrix-with-labels](https://stackoverflow.com/questions/19233771/sklearn-plot-confusion-matrix-with-labels/31720054)
+
+  f) [Model-selection-plot-confusion-matrix](http://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html#sphx-glr-auto-examples-model-selection-plot-confusion-matrix-py)
 
-setup(**setup_kwargs)
```

### Comparing `pretty-confusion-matrix-0.1.1/PKG-INFO` & `pretty_confusion_matrix-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pretty-confusion-matrix
-Version: 0.1.1
+Version: 0.2.0
 Summary: plot a pretty confusion matrix (like Matlab) in python using seaborn and matplotlib
 Home-page: https://github.com/wcipriano/pretty-print-confusion-matrix
 Keywords: confusion matrix
-Author: Khuyen Tran
-Author-email: khuyentran1476@gmail.com
-Requires-Python: >=3.7.1,<3.11
+Author: Wagner Cipriano
+Author-email: wagnao@gmail.com
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: black (>=21.5b0,<22.0)
-Requires-Dist: flake8 (>=3.9.2,<4.0.0)
-Requires-Dist: isort (>=5.8.0,<6.0.0)
-Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
-Requires-Dist: numpy (>=1.21.4,<2.0.0)
-Requires-Dist: pandas (>=1.3.4,<2.0.0)
-Requires-Dist: pre-commit (>=2.12.1,<3.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
-Requires-Dist: sklearn (>=0.0,<0.1)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (<=3.8) ; python_full_version <= "3.8.0"
+Requires-Dist: matplotlib (<=4.0) ; python_full_version > "3.8.0"
+Requires-Dist: numpy (>=1.24.4,<2.0.0)
+Requires-Dist: pandas (<2.1) ; python_version < "3.9"
+Requires-Dist: pandas (<2.3) ; python_version >= "3.9"
+Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Project-URL: Repository, https://github.com/wcipriano/pretty-print-confusion-matrix
 Description-Content-Type: text/markdown
 
 # Confusion Matrix in Python
 Plot a pretty confusion matrix (like Matlab) in python using seaborn and matplotlib
 
-
 Created on Mon Jun 25 14:17:37 2018
 @author: Wagner Cipriano - wagnerbhbr
 
 
 This module get a pretty print confusion matrix from a NumPy matrix or from 2 NumPy arrays (`y_test` and `predictions`).
 
 ## Installation
@@ -73,26 +71,31 @@
 pp_matrix_from_data(y_test, predic)
 ```
 
 ![alt text](https://raw.githubusercontent.com/khuyentran1401/pretty-print-confusion-matrix/master/Screenshots/Conf_matrix_default_2.png)
 
 
 
-
 ## References:
-1. Mat lab confusion matrix
+### 1. MATLAB confusion matrix:
 
-   https://www.mathworks.com/help/nnet/ref/plotconfusion.html
+a) [Plot Confusion](https://www.mathworks.com/help/nnet/ref/plotconfusion.html)
    
-   https://www.mathworks.com/help/examples/nnet/win64/PlotConfusionMatrixUsingCategoricalLabelsExample_02.png
+b) [Plot Confusion Matrix Using Categorical Labels](https://www.mathworks.com/help/examples/nnet/win64/PlotConfusionMatrixUsingCategoricalLabelsExample_02.png)
 
-   https://stackoverflow.com/questions/5821125/how-to-plot-confusion-matrix-with-string-axis-rather-than-integer-in-python/51176855#51176855
 
 
-2. Other Examples in python
+### 2. Examples and more on Python:
+
+  a) [How to plot confusion matrix with string axis rather than integer in python](https://stackoverflow.com/questions/5821125/how-to-plot-confusion-matrix-with-string-axis-rather-than-integer-in-python/51176855#51176855)
+  
+  b) [Plot-scikit-learn-classification-report](https://stackoverflow.com/questions/28200786/how-to-plot-scikit-learn-classification-report)
   
-  a) https://stackoverflow.com/a/51176855/1809554
+  c) [Plot-confusion-matrix-with-string-axis-rather-than-integer-in-Python](https://stackoverflow.com/questions/5821125/how-to-plot-confusion-matrix-with-string-axis-rather-than-integer-in-python)
   
-  b) https://www.programcreek.com/python/example/96197/seaborn.heatmap
+  d) [Seaborn heatmap](https://www.programcreek.com/python/example/96197/seaborn.heatmap)
+  
+  e) [Sklearn-plot-confusion-matrix-with-labels](https://stackoverflow.com/questions/19233771/sklearn-plot-confusion-matrix-with-labels/31720054)
+
+  f) [Model-selection-plot-confusion-matrix](http://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html#sphx-glr-auto-examples-model-selection-plot-confusion-matrix-py)
 
-  c) http://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html#sphx-glr-auto-examples-model-selection-plot-confusion-matrix-py
```

