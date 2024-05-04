# Comparing `tmp/flake8-commas-x-3.0.0.dev2.tar.gz` & `tmp/flake8_commas_x-3.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-commas-x-3.0.0.dev2.tar", last modified: Tue Mar 12 17:26:05 2024, max compression
+gzip compressed data, was "flake8_commas_x-3.0.0.post1.tar", last modified: Sat May  4 13:57:22 2024, max compression
```

## Comparing `flake8-commas-x-3.0.0.dev2.tar` & `flake8_commas_x-3.0.0.post1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:26:05.589977 flake8-commas-x-3.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-03-12 17:26:05.589977 flake8-commas-x-3.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:26:05.585977 flake8-commas-x-3.0.0.dev2/flake8_commas/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/flake8_commas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/flake8_commas/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:26:05.585977 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-03-12 17:26:05.000000 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-12 17:26:05.000000 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 17:26:05.000000 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-12 17:26:05.000000 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 17:26:05.000000 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-12 17:26:05.000000 flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 17:26:05.589977 flake8-commas-x-3.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:26:05.585977 flake8-commas-x-3.0.0.dev2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/test/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-12 17:25:55.000000 flake8-commas-x-3.0.0.dev2/test/test_flake8.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:57:22.197125 flake8_commas_x-3.0.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-05-04 13:57:22.197125 flake8_commas_x-3.0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:57:22.193124 flake8_commas_x-3.0.0.post1/flake8_commas/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/flake8_commas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/flake8_commas/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:57:22.197125 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-05-04 13:57:22.000000 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 13:57:22.000000 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 13:57:22.000000 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 13:57:22.000000 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 13:57:22.000000 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 13:57:22.000000 flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 13:57:22.197125 flake8_commas_x-3.0.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:57:22.197125 flake8_commas_x-3.0.0.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/test/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-04 13:57:12.000000 flake8_commas_x-3.0.0.post1/test/test_flake8.py
```

### Comparing `flake8-commas-x-3.0.0.dev2/CHANGES.rst` & `flake8_commas_x-3.0.0.post1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-3.0.0 (unreleased)
+3.0.0 (2024-03-12)
 ------------------
 
+- Project renamed to ``flake8-commas-x`` to continue maintenance.
 - Support dropped for Python <3.8.
 - Support added for Python 3.12.
 - Drop explicit ``noqa`` handling; this is handled by flake8 now.
 - Remove use of ``pkg_resources`` in favour of ``importlib``.
 - CI moved to GitHub Actions.
```

### Comparing `flake8-commas-x-3.0.0.dev2/LICENSE` & `flake8_commas_x-3.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-commas-x-3.0.0.dev2/PKG-INFO` & `flake8_commas_x-3.0.0.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-commas-x
-Version: 3.0.0.dev2
+Version: 3.0.0.post1
 Summary: Flake8 lint for trailing commas.
 Home-page: https://github.com/PeterJCLaw/flake8-commas/
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 Maintainer: Peter Law
 Maintainer-email: PeterJCLaw@gmail.com
 Classifier: Environment :: Console
@@ -17,32 +17,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Framework :: Flake8
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: flake8>=5
 
 Flake8 Extension to enforce better comma placement.
 ===================================================
 
 **Note:** Forked from PyCQA/flake8-commas to add support for Python 3.12, match
 statement, and other features. Support for Python version below 3.8 has been
 dropped, as well as older (5.x) versions of flake8.
 
+|Build Status| |PyPI - Version|
+
 Usage
 -----
 
 If you are using flake8 it's as easy as:
 
 .. code:: shell
 
-    pip install https://github.com/PeterJCLaw/flake8-commas.git
+    pip install flake8-commas-x
 
 Now you can avoid those annoying merge conflicts on dictionary and list diffs.
 
 Errors
 ------
 
 Different versions of python require commas in different places. Ignore the
@@ -77,17 +80,25 @@
     }
 
     json_data = json.dumps({
         "key": "value",
     }),                      # <-- incorrect trailing comma. json_data is now a tuple. Likely by accident.
 
 
-3.0.0 (unreleased)
+.. |Build Status| image:: https://github.com/PeterJCLaw/flake8-commas/actions/workflows/.github/workflows/tests.yml/badge.svg?branch=main
+   :target: https://github.com/PeterJCLaw/flake8-commas/actions?query=branch%3Amain
+
+.. |PyPI - Version| image:: https://img.shields.io/pypi/v/flake8-commas-x
+   :target: https://pypi.org/project/flake8-commas-x/
+
+
+3.0.0 (2024-03-12)
 ------------------
 
+- Project renamed to ``flake8-commas-x`` to continue maintenance.
 - Support dropped for Python <3.8.
 - Support added for Python 3.12.
 - Drop explicit ``noqa`` handling; this is handled by flake8 now.
 - Remove use of ``pkg_resources`` in favour of ``importlib``.
 - CI moved to GitHub Actions.
```

### Comparing `flake8-commas-x-3.0.0.dev2/flake8_commas/_base.py` & `flake8_commas_x-3.0.0.post1/flake8_commas/_base.py`

 * *Files identical despite different names*

### Comparing `flake8-commas-x-3.0.0.dev2/flake8_commas_x.egg-info/PKG-INFO` & `flake8_commas_x-3.0.0.post1/flake8_commas_x.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-commas-x
-Version: 3.0.0.dev2
+Version: 3.0.0.post1
 Summary: Flake8 lint for trailing commas.
 Home-page: https://github.com/PeterJCLaw/flake8-commas/
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 Maintainer: Peter Law
 Maintainer-email: PeterJCLaw@gmail.com
 Classifier: Environment :: Console
@@ -17,32 +17,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Framework :: Flake8
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: flake8>=5
 
 Flake8 Extension to enforce better comma placement.
 ===================================================
 
 **Note:** Forked from PyCQA/flake8-commas to add support for Python 3.12, match
 statement, and other features. Support for Python version below 3.8 has been
 dropped, as well as older (5.x) versions of flake8.
 
+|Build Status| |PyPI - Version|
+
 Usage
 -----
 
 If you are using flake8 it's as easy as:
 
 .. code:: shell
 
-    pip install https://github.com/PeterJCLaw/flake8-commas.git
+    pip install flake8-commas-x
 
 Now you can avoid those annoying merge conflicts on dictionary and list diffs.
 
 Errors
 ------
 
 Different versions of python require commas in different places. Ignore the
@@ -77,17 +80,25 @@
     }
 
     json_data = json.dumps({
         "key": "value",
     }),                      # <-- incorrect trailing comma. json_data is now a tuple. Likely by accident.
 
 
-3.0.0 (unreleased)
+.. |Build Status| image:: https://github.com/PeterJCLaw/flake8-commas/actions/workflows/.github/workflows/tests.yml/badge.svg?branch=main
+   :target: https://github.com/PeterJCLaw/flake8-commas/actions?query=branch%3Amain
+
+.. |PyPI - Version| image:: https://img.shields.io/pypi/v/flake8-commas-x
+   :target: https://pypi.org/project/flake8-commas-x/
+
+
+3.0.0 (2024-03-12)
 ------------------
 
+- Project renamed to ``flake8-commas-x`` to continue maintenance.
 - Support dropped for Python <3.8.
 - Support added for Python 3.12.
 - Drop explicit ``noqa`` handling; this is handled by flake8 now.
 - Remove use of ``pkg_resources`` in favour of ``importlib``.
 - CI moved to GitHub Actions.
```

### Comparing `flake8-commas-x-3.0.0.dev2/setup.py` & `flake8_commas_x-3.0.0.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 
 setup(
     name='flake8-commas-x',
     author="Peter Law",
     author_email="PeterJCLaw@gmail.com",
     maintainer="Peter Law",
     maintainer_email="PeterJCLaw@gmail.com",
-    version='3.0.0.dev2',
+    version='3.0.0.post1',
     install_requires=['flake8>=5'],
     python_requires='>=3.8',
     url='https://github.com/PeterJCLaw/flake8-commas/',
     long_description=readme + '\n\n' + history,
+    long_description_content_type='text/x-rst',
     description='Flake8 lint for trailing commas.',
     packages=['flake8_commas'],
     test_suite='test',
     include_package_data=True,
     entry_points={
         'flake8.extension': [
             'C81 = flake8_commas:CommaChecker',
```

### Comparing `flake8-commas-x-3.0.0.dev2/test/test_checks.py` & `flake8_commas_x-3.0.0.post1/test/test_checks.py`

 * *Files identical despite different names*

