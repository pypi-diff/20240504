# Comparing `tmp/imgcv-0.4.0.tar.gz` & `tmp/imgcv-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgcv-0.4.0.tar", max compression
+gzip compressed data, was "imgcv-0.5.0.tar", max compression
```

## Comparing `imgcv-0.4.0.tar` & `imgcv-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rwxr-xr-x   0        0        0     1072 2024-03-30 06:48:50.025772 imgcv-0.4.0/LICENSE
--rw-r--r--   0        0        0     1969 2024-03-30 06:48:50.025772 imgcv-0.4.0/README.md
--rw-r--r--   0        0        0      935 2024-03-30 06:49:00.541818 imgcv-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      107 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/__init__.py
--rw-r--r--   0        0        0      644 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/common.py
--rw-r--r--   0        0        0        0 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/connectivity/__init__.py
--rw-r--r--   0        0        0     4249 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/connectivity/connected_components.py
--rw-r--r--   0        0        0        0 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/quantization/__init__.py
--rw-r--r--   0        0        0     1111 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/quantization/reduce_gray_levels.py
--rw-r--r--   0        0        0      398 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/quantization/to_binary.py
--rw-r--r--   0        0        0        0 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/transformations/__init__.py
--rw-r--r--   0        0        0      823 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/transformations/gamma.py
--rw-r--r--   0        0        0      793 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/transformations/logarithmic.py
--rw-r--r--   0        0        0      799 2024-03-30 06:48:50.041772 imgcv-0.4.0/src/imgcv/transformations/negative.py
--rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 imgcv-0.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2024-05-04 07:05:58.189657 imgcv-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1969 2024-05-04 07:05:58.189657 imgcv-0.5.0/README.md
+-rw-r--r--   0        0        0      935 2024-05-04 07:06:08.641720 imgcv-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/__init__.py
+-rw-r--r--   0        0        0      644 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/common.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/connectivity/__init__.py
+-rw-r--r--   0        0        0     4249 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/connectivity/connected_components.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/histogram/__init__.py
+-rw-r--r--   0        0        0     3027 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/histogram/histogram_equalization.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/quantization/__init__.py
+-rw-r--r--   0        0        0     1111 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/quantization/reduce_gray_levels.py
+-rw-r--r--   0        0        0      398 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/quantization/to_binary.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/transformations/__init__.py
+-rw-r--r--   0        0        0      823 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/transformations/gamma.py
+-rw-r--r--   0        0        0      793 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/transformations/logarithmic.py
+-rw-r--r--   0        0        0      799 2024-05-04 07:05:58.209657 imgcv-0.5.0/src/imgcv/transformations/negative.py
+-rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 imgcv-0.5.0/PKG-INFO
```

### Comparing `imgcv-0.4.0/LICENSE` & `imgcv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/README.md` & `imgcv-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/pyproject.toml` & `imgcv-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imgcv"
-version = "0.4.0"
+version = "0.5.0"
 description = "Image Processing Library"
 authors = ["Preet Sojitra"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imgcv-0.4.0/src/imgcv/common.py` & `imgcv-0.5.0/src/imgcv/common.py`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/src/imgcv/connectivity/connected_components.py` & `imgcv-0.5.0/src/imgcv/connectivity/connected_components.py`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/src/imgcv/quantization/reduce_gray_levels.py` & `imgcv-0.5.0/src/imgcv/quantization/reduce_gray_levels.py`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/src/imgcv/transformations/gamma.py` & `imgcv-0.5.0/src/imgcv/transformations/gamma.py`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/src/imgcv/transformations/logarithmic.py` & `imgcv-0.5.0/src/imgcv/transformations/logarithmic.py`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/src/imgcv/transformations/negative.py` & `imgcv-0.5.0/src/imgcv/transformations/negative.py`

 * *Files identical despite different names*

### Comparing `imgcv-0.4.0/PKG-INFO` & `imgcv-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgcv
-Version: 0.4.0
+Version: 0.5.0
 Summary: Image Processing Library
 License: MIT
 Author: Preet Sojitra
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

