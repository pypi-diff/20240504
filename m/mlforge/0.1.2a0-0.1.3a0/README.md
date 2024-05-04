# Comparing `tmp/mlforge-0.1.2a0.tar.gz` & `tmp/mlforge-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforge-0.1.2a0.tar", last modified: Mon Apr 29 07:35:22 2024, max compression
+gzip compressed data, was "mlforge-0.1.3a0.tar", last modified: Mon Apr 29 07:52:35 2024, max compression
```

## Comparing `mlforge-0.1.2a0.tar` & `mlforge-0.1.3a0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:35:22.016979 mlforge-0.1.2a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-29 07:35:22.016979 mlforge-0.1.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:35:22.016979 mlforge-0.1.2a0/mlforge/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/mlforge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/mlforge/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    34254 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/mlforge/mlforge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/mlforge/progbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:35:22.016979 mlforge-0.1.2a0/mlforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-29 07:35:22.000000 mlforge-0.1.2a0/mlforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 07:35:22.000000 mlforge-0.1.2a0/mlforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:35:22.000000 mlforge-0.1.2a0/mlforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:35:22.000000 mlforge-0.1.2a0/mlforge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:35:22.016979 mlforge-0.1.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:35:22.016979 mlforge-0.1.2a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_add_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_build_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_callable_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_from_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_get_method_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_get_step_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_parse_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_pbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-29 07:35:16.000000 mlforge-0.1.2a0/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.460708 mlforge-0.1.3a0/mlforge/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34254 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/mlforge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/progbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/mlforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_add_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_build_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_callable_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_get_method_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_get_step_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_parse_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_pbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_run.py
```

### Comparing `mlforge-0.1.2a0/LICENSE.txt` & `mlforge-0.1.3a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/PKG-INFO` & `mlforge-0.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforge
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A package to design and run sequential ML pipelines
 Home-page: https://github.com/renero/mlforge
 Author: J. Renero
 Author-email: jesus.renero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlforge-0.1.2a0/README.rst` & `mlforge-0.1.3a0/README.rst`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/mlforge/logconfig.py` & `mlforge-0.1.3a0/mlforge/logconfig.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/mlforge/mlforge.py` & `mlforge-0.1.3a0/mlforge/mlforge.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/mlforge/progbar.py` & `mlforge-0.1.3a0/mlforge/progbar.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/mlforge.egg-info/PKG-INFO` & `mlforge-0.1.3a0/mlforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlforge
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A package to design and run sequential ML pipelines
 Home-page: https://github.com/renero/mlforge
 Author: J. Renero
 Author-email: jesus.renero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlforge-0.1.2a0/mlforge.egg-info/SOURCES.txt` & `mlforge-0.1.3a0/mlforge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/setup.py` & `mlforge-0.1.3a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlforge",
-    version="0.1.2a",
+    version="0.1.3a",
     author="J. Renero",
     author_email="jesus.renero@gmail.com",
     description="A package to design and run sequential ML pipelines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/renero/mlforge",
     classifiers=[
```

### Comparing `mlforge-0.1.2a0/tests/test_add_stages.py` & `mlforge-0.1.3a0/tests/test_add_stages.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_build_params.py` & `mlforge-0.1.3a0/tests/test_build_params.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_callable_method.py` & `mlforge-0.1.3a0/tests/test_callable_method.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_from_config.py` & `mlforge-0.1.3a0/tests/test_from_config.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_from_list.py` & `mlforge-0.1.3a0/tests/test_from_list.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_get_method_signature.py` & `mlforge-0.1.3a0/tests/test_get_method_signature.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_get_step_components.py` & `mlforge-0.1.3a0/tests/test_get_step_components.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_parse_step.py` & `mlforge-0.1.3a0/tests/test_parse_step.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_pbar.py` & `mlforge-0.1.3a0/tests/test_pbar.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.2a0/tests/test_run.py` & `mlforge-0.1.3a0/tests/test_run.py`

 * *Files identical despite different names*

