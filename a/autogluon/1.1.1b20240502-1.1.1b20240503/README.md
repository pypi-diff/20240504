# Comparing `tmp/autogluon-1.1.1b20240502.tar.gz` & `tmp/autogluon-1.1.1b20240503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.1b20240502.tar", last modified: Thu May  2 09:05:34 2024, max compression
+gzip compressed data, was "autogluon-1.1.1b20240503.tar", last modified: Fri May  3 09:05:14 2024, max compression
```

## Comparing `autogluon-1.1.1b20240502.tar` & `autogluon-1.1.1b20240503.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-02 09:03:54.000000 autogluon-1.1.1b20240502/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:03:54.000000 autogluon-1.1.1b20240502/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:05:34.107740 autogluon-1.1.1b20240502/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:05:34.000000 autogluon-1.1.1b20240502/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:05:14.916351 autogluon-1.1.1b20240503/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-03 09:05:14.916351 autogluon-1.1.1b20240503/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:05:14.916351 autogluon-1.1.1b20240503/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-03 09:03:38.000000 autogluon-1.1.1b20240503/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:05:14.912351 autogluon-1.1.1b20240503/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:05:14.912351 autogluon-1.1.1b20240503/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:05:14.916351 autogluon-1.1.1b20240503/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:03:38.000000 autogluon-1.1.1b20240503/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:05:14.916351 autogluon-1.1.1b20240503/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:05:14.000000 autogluon-1.1.1b20240503/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.1b20240502/PKG-INFO` & `autogluon-1.1.1b20240503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240502
+Version: 1.1.1b20240503
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.1b20240502/setup.py` & `autogluon-1.1.1b20240503/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.1b20240502/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.1b20240503/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240502
+Version: 1.1.1b20240503
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

