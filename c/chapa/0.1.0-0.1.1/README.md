# Comparing `tmp/chapa-0.1.0.tar.gz` & `tmp/chapa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chapa-0.1.0.tar", last modified: Mon Mar 18 11:29:10 2024, max compression
+gzip compressed data, was "chapa-0.1.1.tar", last modified: Sat May  4 10:56:19 2024, max compression
```

## Comparing `chapa-0.1.0.tar` & `chapa-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:29:10.485873 chapa-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-18 11:28:57.000000 chapa-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-03-18 11:29:10.485873 chapa-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-03-18 11:28:57.000000 chapa-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:29:10.485873 chapa-0.1.0/chapa/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-18 11:28:57.000000 chapa-0.1.0/chapa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28781 2024-03-18 11:28:57.000000 chapa-0.1.0/chapa/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-18 11:28:57.000000 chapa-0.1.0/chapa/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:29:10.485873 chapa-0.1.0/chapa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-03-18 11:29:10.000000 chapa-0.1.0/chapa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-18 11:29:10.000000 chapa-0.1.0/chapa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 11:29:10.000000 chapa-0.1.0/chapa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-18 11:29:10.000000 chapa-0.1.0/chapa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-18 11:29:10.000000 chapa-0.1.0/chapa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-18 11:28:57.000000 chapa-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 11:29:10.485873 chapa-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-18 11:28:57.000000 chapa-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:56:19.375485 chapa-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 10:56:11.000000 chapa-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-04 10:56:19.375485 chapa-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-04 10:56:11.000000 chapa-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:56:19.371485 chapa-0.1.1/chapa/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 10:56:11.000000 chapa-0.1.1/chapa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28781 2024-05-04 10:56:11.000000 chapa-0.1.1/chapa/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-04 10:56:11.000000 chapa-0.1.1/chapa/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:56:19.375485 chapa-0.1.1/chapa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-04 10:56:19.000000 chapa-0.1.1/chapa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-04 10:56:19.000000 chapa-0.1.1/chapa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:56:19.000000 chapa-0.1.1/chapa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 10:56:19.000000 chapa-0.1.1/chapa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 10:56:19.000000 chapa-0.1.1/chapa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-04 10:56:11.000000 chapa-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:56:19.375485 chapa-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-04 10:56:11.000000 chapa-0.1.1/setup.py
```

### Comparing `chapa-0.1.0/LICENSE` & `chapa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chapa-0.1.0/PKG-INFO` & `chapa-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chapa
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK for Chapa API https://developer.chapa.co
 Home-page: https://github.com/chapimenge3/chapa
 Author: Temkin Mengistu (Chapi)
 Author-email: chapimenge3@gmail.com
 Project-URL: Source, https://github.com/chapimenge3/chapa
 Project-URL: Bug Tracker, https://github.com/chapimenge3/chapa/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chapa-0.1.0/README.md` & `chapa-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chapa-0.1.0/chapa/api.py` & `chapa-0.1.1/chapa/api.py`

 * *Files identical despite different names*

### Comparing `chapa-0.1.0/chapa/webhook.py` & `chapa-0.1.1/chapa/webhook.py`

 * *Files identical despite different names*

### Comparing `chapa-0.1.0/chapa.egg-info/PKG-INFO` & `chapa-0.1.1/chapa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chapa
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK for Chapa API https://developer.chapa.co
 Home-page: https://github.com/chapimenge3/chapa
 Author: Temkin Mengistu (Chapi)
 Author-email: chapimenge3@gmail.com
 Project-URL: Source, https://github.com/chapimenge3/chapa
 Project-URL: Bug Tracker, https://github.com/chapimenge3/chapa/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chapa-0.1.0/setup.py` & `chapa-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import os
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
-version_number = os.environ.get('CHAPA_VERSION', '0.1.0')
+version_number = os.environ.get('CHAPA_VERSION', '0.1.1')
 
 setuptools.setup(
     name='chapa',
     version=version_number,
     author='Temkin Mengistu (Chapi)',
     author_email='chapimenge3@gmail.com',
     description='Python SDK for Chapa API https://developer.chapa.co',
```

