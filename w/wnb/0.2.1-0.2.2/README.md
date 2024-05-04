# Comparing `tmp/wnb-0.2.1.tar.gz` & `tmp/wnb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnb-0.2.1.tar", last modified: Fri Dec 29 18:56:46 2023, max compression
+gzip compressed data, was "wnb-0.2.2.tar", last modified: Sat May  4 08:52:55 2024, max compression
```

## Comparing `wnb-0.2.1.tar` & `wnb-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 18:56:46.470103 wnb-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-29 18:56:13.000000 wnb-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-29 18:56:13.000000 wnb-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-12-29 18:56:46.470103 wnb-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-12-29 18:56:13.000000 wnb-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-29 18:56:13.000000 wnb-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-29 18:56:46.470103 wnb-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-12-29 18:56:13.000000 wnb-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 18:56:46.466103 wnb-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 18:56:13.000000 wnb-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2023-12-29 18:56:13.000000 wnb-0.2.1/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2023-12-29 18:56:13.000000 wnb-0.2.1/tests/test_gnb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2023-12-29 18:56:13.000000 wnb-0.2.1/tests/test_gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 18:56:46.466103 wnb-0.2.1/wnb/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/_enum_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    12117 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/gnb.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2023-12-29 18:56:13.000000 wnb-0.2.1/wnb/gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 18:56:46.470103 wnb-0.2.1/wnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-12-29 18:56:46.000000 wnb-0.2.1/wnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-12-29 18:56:46.000000 wnb-0.2.1/wnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 18:56:46.000000 wnb-0.2.1/wnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-29 18:56:46.000000 wnb-0.2.1/wnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-29 18:56:46.000000 wnb-0.2.1/wnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:55.684417 wnb-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-04 08:52:29.000000 wnb-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 08:52:29.000000 wnb-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-04 08:52:55.684417 wnb-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-04 08:52:29.000000 wnb-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:55.680417 wnb-0.2.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:29.000000 wnb-0.2.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-04 08:52:29.000000 wnb-0.2.2/benchmarks/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-04 08:52:29.000000 wnb-0.2.2/benchmarks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-04 08:52:29.000000 wnb-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-04 08:52:55.684417 wnb-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-04 08:52:29.000000 wnb-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:55.680417 wnb-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:29.000000 wnb-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-04 08:52:29.000000 wnb-0.2.2/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-04 08:52:29.000000 wnb-0.2.2/tests/test_gnb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-04 08:52:29.000000 wnb-0.2.2/tests/test_gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:55.684417 wnb-0.2.2/wnb/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/_enum_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-04 08:52:29.000000 wnb-0.2.2/wnb/gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:52:55.684417 wnb-0.2.2/wnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-04 08:52:55.000000 wnb-0.2.2/wnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-04 08:52:55.000000 wnb-0.2.2/wnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:52:55.000000 wnb-0.2.2/wnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 08:52:55.000000 wnb-0.2.2/wnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 08:52:55.000000 wnb-0.2.2/wnb.egg-info/top_level.txt
```

### Comparing `wnb-0.2.1/LICENSE` & `wnb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/PKG-INFO` & `wnb-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,73 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 License: BSD License
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.4.1
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: scikit-learn>=1.0.2
 Provides-Extra: dev
-Requires-Dist: pytest==7.3.1; extra == "dev"
-Requires-Dist: black>=23.9.0; extra == "dev"
+Requires-Dist: pytest>=7.3.1; extra == "dev"
+Requires-Dist: black>=24.1.0; extra == "dev"
+Requires-Dist: tqdm>=4.65.0; extra == "dev"
 
-# WNB: General and weighted naive Bayes classifiers
+<div align="center">
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
+</div>
 
-![](https://img.shields.io/badge/version-v0.2.1-green)
-![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
-![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
-[![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
-![](https://img.shields.io/pypi/dm/wnb)
+<div align="center"> <b>General and weighted naive Bayes classifiers</b> </div> <br>
 
+<div align="center">
 
-<p>
-<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
-<br>
-</p>
+![Lastest Release](https://img.shields.io/badge/release-v0.2.2-green)
+[![PyPI Version](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)<br>
+![GitHub Workflow Status (build)](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
+![PyPI License](https://img.shields.io/pypi/l/wnb)
+[![PyPi Downloads](https://static.pepy.tech/badge/wnb)](https://pepy.tech/project/wnb)
+
+</div>
 
 ## Introduction
-Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
-This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
+Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community. This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
 
 ### General naive Bayes
-The issue with the well-known implementations of the naive Bayes algorithm (such as the ones in `sklearn.naive_bayes`
-module) is that they assume a single distribution for the likelihoods of all features. Such an implementation can limit 
-those who need to develop naive Bayes models with different distributions for feature likelihood. And enters **WNB** library!
-It allows you to customize your naive Bayes model by specifying the likelihood distribution of each feature separately.
-You can choose from a range of continuous and discrete probability distributions to design your classifier.
+The issue with the well-known implementations of the naive Bayes algorithm (such as the ones in `sklearn.naive_bayes` module) is that they assume a single distribution for the likelihoods of all features. Such an implementation can limit those who need to develop naive Bayes models with different distributions for feature likelihood. And enters **WNB** library! It allows you to customize your naive Bayes model by specifying the likelihood distribution of each feature separately. You can choose from a range of continuous and discrete probability distributions to design your classifier.
 
 ### Weighted naive Bayes
-Although naive Bayes has many advantages such as simplicity and interpretability, its conditional independence assumption
-rarely holds true in real-world applications. In order to alleviate its conditional independence assumption, many attribute
-weighting naive Bayes (WNB) approaches have been proposed. Most of the proposed methods involve computationally demanding
-optimization problems that do not allow for controlling the model's bias due to class imbalance. Minimum Log-likelihood
-Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision
-rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation
-of gaussian MLD-WNB.
+Although naive Bayes has many advantages such as simplicity and interpretability, its conditional independence assumption rarely holds true in real-world applications. In order to alleviate its conditional independence assumption, many attribute weighting naive Bayes (WNB) approaches have been proposed. Most of the proposed methods involve computationally demanding optimization problems that do not allow for controlling the model's bias due to class imbalance. Minimum Log-likelihood Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation of gaussian MLD-WNB.
 
 ## Installation
-The easiest way to install the wnb library is by using `pip`:
+The easiest way to install the **wnb** library is by using `pip`:
 ```
 pip install wnb
 ```
-This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. 
-Furthermore, it is fully compatible with Scikit-learn API.
+This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. Furthermore, it is fully compatible with Scikit-learn API.
 
-## Getting started
+## Getting started ⚡️
 Here, we show how you can use the library to train general and weighted naive Bayes classifiers. 
 
 ### General naive Bayes
 
 A general naive Bayes model can be set up and used in four simple steps:
 
 1. Import the `GeneralNB` class as well as `Distribution` enum class
@@ -134,15 +126,25 @@
 ```
 
 Then, run pytest:
 ```
 pytest
 ```
 
-## Citation
+## Support us 🤝
+You can support the project in the following ways:
+
+⭐ Star WNB on GitHub (click the star button in the top right corner)
+
+💡 Provide your feedback or propose ideas in the [Issues section](https://github.com/msamsami/weighted-naive-bayes/issues)
+
+📰 Post about WNB on LinkedIn or other platforms
+
+
+## Citation 📚
 If you utilize this repository, please consider citing it with:
 
 ```
 @misc{wnb,
   author = {Mohammd Mehdi Samsami},
   title = {WNB: General and weighted naive Bayes classifiers},
   year = {2023},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wnb-0.2.1/README.md` & `wnb-0.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,41 @@
-# WNB: General and weighted naive Bayes classifiers
+<div align="center">
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
+</div>
 
-![](https://img.shields.io/badge/version-v0.2.1-green)
-![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
-![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
-[![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
-![](https://img.shields.io/pypi/dm/wnb)
+<div align="center"> <b>General and weighted naive Bayes classifiers</b> </div> <br>
 
+<div align="center">
 
-<p>
-<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
-<br>
-</p>
+![Lastest Release](https://img.shields.io/badge/release-v0.2.2-green)
+[![PyPI Version](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)<br>
+![GitHub Workflow Status (build)](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
+![PyPI License](https://img.shields.io/pypi/l/wnb)
+[![PyPi Downloads](https://static.pepy.tech/badge/wnb)](https://pepy.tech/project/wnb)
+
+</div>
 
 ## Introduction
-Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
-This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
+Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community. This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
 
 ### General naive Bayes
-The issue with the well-known implementations of the naive Bayes algorithm (such as the ones in `sklearn.naive_bayes`
-module) is that they assume a single distribution for the likelihoods of all features. Such an implementation can limit 
-those who need to develop naive Bayes models with different distributions for feature likelihood. And enters **WNB** library!
-It allows you to customize your naive Bayes model by specifying the likelihood distribution of each feature separately.
-You can choose from a range of continuous and discrete probability distributions to design your classifier.
+The issue with the well-known implementations of the naive Bayes algorithm (such as the ones in `sklearn.naive_bayes` module) is that they assume a single distribution for the likelihoods of all features. Such an implementation can limit those who need to develop naive Bayes models with different distributions for feature likelihood. And enters **WNB** library! It allows you to customize your naive Bayes model by specifying the likelihood distribution of each feature separately. You can choose from a range of continuous and discrete probability distributions to design your classifier.
 
 ### Weighted naive Bayes
-Although naive Bayes has many advantages such as simplicity and interpretability, its conditional independence assumption
-rarely holds true in real-world applications. In order to alleviate its conditional independence assumption, many attribute
-weighting naive Bayes (WNB) approaches have been proposed. Most of the proposed methods involve computationally demanding
-optimization problems that do not allow for controlling the model's bias due to class imbalance. Minimum Log-likelihood
-Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision
-rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation
-of gaussian MLD-WNB.
+Although naive Bayes has many advantages such as simplicity and interpretability, its conditional independence assumption rarely holds true in real-world applications. In order to alleviate its conditional independence assumption, many attribute weighting naive Bayes (WNB) approaches have been proposed. Most of the proposed methods involve computationally demanding optimization problems that do not allow for controlling the model's bias due to class imbalance. Minimum Log-likelihood Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation of gaussian MLD-WNB.
 
 ## Installation
-The easiest way to install the wnb library is by using `pip`:
+The easiest way to install the **wnb** library is by using `pip`:
 ```
 pip install wnb
 ```
-This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. 
-Furthermore, it is fully compatible with Scikit-learn API.
+This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. Furthermore, it is fully compatible with Scikit-learn API.
 
-## Getting started
+## Getting started ⚡️
 Here, we show how you can use the library to train general and weighted naive Bayes classifiers. 
 
 ### General naive Bayes
 
 A general naive Bayes model can be set up and used in four simple steps:
 
 1. Import the `GeneralNB` class as well as `Distribution` enum class
@@ -103,15 +94,25 @@
 ```
 
 Then, run pytest:
 ```
 pytest
 ```
 
-## Citation
+## Support us 🤝
+You can support the project in the following ways:
+
+⭐ Star WNB on GitHub (click the star button in the top right corner)
+
+💡 Provide your feedback or propose ideas in the [Issues section](https://github.com/msamsami/weighted-naive-bayes/issues)
+
+📰 Post about WNB on LinkedIn or other platforms
+
+
+## Citation 📚
 If you utilize this repository, please consider citing it with:
 
 ```
 @misc{wnb,
   author = {Mohammd Mehdi Samsami},
   title = {WNB: General and weighted naive Bayes classifiers},
   year = {2023},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wnb-0.2.1/setup.py` & `wnb-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     author_email="mehdisamsami@live.com",
     license="BSD License",
     url="https://github.com/msamsami/weighted-naive-bayes",
     long_description=codecs.open(
         path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
     ).read(),
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
+    packages=find_packages(exclude=["tests*"]),
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: BSD License",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8,<3.13",
     install_requires=["pandas>=1.4.1", "scipy>=1.8.0", "scikit-learn>=1.0.2"],
-    extras_require={"dev": ["pytest==7.3.1", "black>=23.9.0"]},
+    extras_require={"dev": ["pytest>=7.3.1", "black>=24.1.0", "tqdm>=4.65.0"]},
 )
```

### Comparing `wnb-0.2.1/tests/test_dist.py` & `wnb-0.2.2/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/tests/test_gnb.py` & `wnb-0.2.2/tests/test_gnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/tests/test_gwnb.py` & `wnb-0.2.2/tests/test_gwnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb/_base.py` & `wnb-0.2.2/wnb/_base.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb/_enum_meta.py` & `wnb-0.2.2/wnb/_enum_meta.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb/_enums.py` & `wnb-0.2.2/wnb/_enums.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb/_typing.py` & `wnb-0.2.2/wnb/_typing.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb/dist.py` & `wnb-0.2.2/wnb/dist.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb/gnb.py` & `wnb-0.2.2/wnb/gnb.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,17 +102,19 @@
         if self.n_classes_ == 1:
             raise ValueError("Classifier can't train when only one class is present")
 
         X = check_array(
             array=X,
             accept_sparse=False,
             accept_large_sparse=False,
-            dtype=None
-            if any(d in self._get_distributions() for d in NonNumericDistributions)
-            else "numeric",
+            dtype=(
+                None
+                if any(d in self._get_distributions() for d in NonNumericDistributions)
+                else "numeric"
+            ),
             force_all_finite=True,
             ensure_2d=True,
             ensure_min_samples=1,
             ensure_min_features=1,
             estimator=self,
         )
 
@@ -203,14 +205,32 @@
                     or dist in Distribution.__members__.values()
                     or (hasattr(dist, "from_data") and hasattr(dist, "__call__"))
                 ):
                     raise ValueError(f"Distribution '{dist}' is not supported.")
 
             self.distributions_ = self.distributions
 
+    @staticmethod
+    def _get_dist_object(name_or_obj):
+        if (
+            isinstance(name_or_obj, Distribution)
+            or name_or_obj in Distribution.__members__.values()
+        ):
+            return AllDistributions[name_or_obj]
+        elif isinstance(name_or_obj, str) and name_or_obj.upper() in [
+            d.name for d in Distribution
+        ]:
+            return AllDistributions[Distribution.__members__[name_or_obj.upper()]]
+        elif isinstance(name_or_obj, str) and name_or_obj.title() in [
+            d.value for d in Distribution
+        ]:
+            return AllDistributions[Distribution(name_or_obj.title())]
+        else:
+            return name_or_obj
+
     def fit(self, X: MatrixLike, y: ArrayLike):
         """Fits general Naive Bayes classifier according to X, y.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             Training vectors, where `n_samples` is the number of samples
@@ -237,20 +257,17 @@
         self._check_inputs(X, y)
 
         y = y_
         self._prepare_parameters()
 
         self.likelihood_params_ = {
             c: [
-                AllDistributions[self.distributions_[i]].from_data(
+                self._get_dist_object(self.distributions_[i]).from_data(
                     X[y == c, i], alpha=self.alpha
                 )
-                if isinstance(self.distributions_[i], Distribution)
-                or self.distributions_[i] in Distribution.__members__.values()
-                else self.distributions_[i].from_data(X[y == c, i], alpha=self.alpha)
                 for i in range(self.n_features_in_)
             ]
             for c in range(self.n_classes_)
         }
 
         return self
 
@@ -290,17 +307,19 @@
         check_is_fitted(self)
 
         # Input validation
         X = check_array(
             array=X,
             accept_large_sparse=False,
             force_all_finite=True,
-            dtype=None
-            if any(d in self._get_distributions() for d in NonNumericDistributions)
-            else "numeric",
+            dtype=(
+                None
+                if any(d in self._get_distributions() for d in NonNumericDistributions)
+                else "numeric"
+            ),
             estimator=self,
         )
 
         # Check if the number of input features matches the data seen during fit
         if X.shape[1] != self.n_features_in_:
             raise ValueError(
                 "Expected input with %d features, got %d instead."
```

### Comparing `wnb-0.2.1/wnb/gwnb.py` & `wnb-0.2.2/wnb/gwnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.2.1/wnb.egg-info/PKG-INFO` & `wnb-0.2.2/wnb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,73 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 License: BSD License
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.4.1
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: scikit-learn>=1.0.2
 Provides-Extra: dev
-Requires-Dist: pytest==7.3.1; extra == "dev"
-Requires-Dist: black>=23.9.0; extra == "dev"
+Requires-Dist: pytest>=7.3.1; extra == "dev"
+Requires-Dist: black>=24.1.0; extra == "dev"
+Requires-Dist: tqdm>=4.65.0; extra == "dev"
 
-# WNB: General and weighted naive Bayes classifiers
+<div align="center">
+<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
+</div>
 
-![](https://img.shields.io/badge/version-v0.2.1-green)
-![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
-![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
-[![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
-![](https://img.shields.io/pypi/dm/wnb)
+<div align="center"> <b>General and weighted naive Bayes classifiers</b> </div> <br>
 
+<div align="center">
 
-<p>
-<img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/docs/logo.png" alt="wnb logo" width="275" />
-<br>
-</p>
+![Lastest Release](https://img.shields.io/badge/release-v0.2.2-green)
+[![PyPI Version](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)<br>
+![GitHub Workflow Status (build)](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
+![PyPI License](https://img.shields.io/pypi/l/wnb)
+[![PyPi Downloads](https://static.pepy.tech/badge/wnb)](https://pepy.tech/project/wnb)
+
+</div>
 
 ## Introduction
-Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community.
-This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
+Naive Bayes is often recognized as one of the most popular classification algorithms in the machine learning community. This package takes naive Bayes to a higher level by providing its implementations in more general and weighted settings.
 
 ### General naive Bayes
-The issue with the well-known implementations of the naive Bayes algorithm (such as the ones in `sklearn.naive_bayes`
-module) is that they assume a single distribution for the likelihoods of all features. Such an implementation can limit 
-those who need to develop naive Bayes models with different distributions for feature likelihood. And enters **WNB** library!
-It allows you to customize your naive Bayes model by specifying the likelihood distribution of each feature separately.
-You can choose from a range of continuous and discrete probability distributions to design your classifier.
+The issue with the well-known implementations of the naive Bayes algorithm (such as the ones in `sklearn.naive_bayes` module) is that they assume a single distribution for the likelihoods of all features. Such an implementation can limit those who need to develop naive Bayes models with different distributions for feature likelihood. And enters **WNB** library! It allows you to customize your naive Bayes model by specifying the likelihood distribution of each feature separately. You can choose from a range of continuous and discrete probability distributions to design your classifier.
 
 ### Weighted naive Bayes
-Although naive Bayes has many advantages such as simplicity and interpretability, its conditional independence assumption
-rarely holds true in real-world applications. In order to alleviate its conditional independence assumption, many attribute
-weighting naive Bayes (WNB) approaches have been proposed. Most of the proposed methods involve computationally demanding
-optimization problems that do not allow for controlling the model's bias due to class imbalance. Minimum Log-likelihood
-Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision
-rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation
-of gaussian MLD-WNB.
+Although naive Bayes has many advantages such as simplicity and interpretability, its conditional independence assumption rarely holds true in real-world applications. In order to alleviate its conditional independence assumption, many attribute weighting naive Bayes (WNB) approaches have been proposed. Most of the proposed methods involve computationally demanding optimization problems that do not allow for controlling the model's bias due to class imbalance. Minimum Log-likelihood Difference WNB (MLD-WNB) is a novel weighting approach that optimizes the weights according to the Bayes optimal decision rule and includes hyperparameters for controlling the model's bias. **WNB** library provides an efficient implementation of gaussian MLD-WNB.
 
 ## Installation
-The easiest way to install the wnb library is by using `pip`:
+The easiest way to install the **wnb** library is by using `pip`:
 ```
 pip install wnb
 ```
-This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. 
-Furthermore, it is fully compatible with Scikit-learn API.
+This library is shipped as an all-in-one module implementation with minimalistic dependencies and requirements. Furthermore, it is fully compatible with Scikit-learn API.
 
-## Getting started
+## Getting started ⚡️
 Here, we show how you can use the library to train general and weighted naive Bayes classifiers. 
 
 ### General naive Bayes
 
 A general naive Bayes model can be set up and used in four simple steps:
 
 1. Import the `GeneralNB` class as well as `Distribution` enum class
@@ -134,15 +126,25 @@
 ```
 
 Then, run pytest:
 ```
 pytest
 ```
 
-## Citation
+## Support us 🤝
+You can support the project in the following ways:
+
+⭐ Star WNB on GitHub (click the star button in the top right corner)
+
+💡 Provide your feedback or propose ideas in the [Issues section](https://github.com/msamsami/weighted-naive-bayes/issues)
+
+📰 Post about WNB on LinkedIn or other platforms
+
+
+## Citation 📚
 If you utilize this repository, please consider citing it with:
 
 ```
 @misc{wnb,
   author = {Mohammd Mehdi Samsami},
   title = {WNB: General and weighted naive Bayes classifiers},
   year = {2023},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

