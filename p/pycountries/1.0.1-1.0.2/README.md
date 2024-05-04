# Comparing `tmp/pycountries-1.0.1.tar.gz` & `tmp/pycountries-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycountries-1.0.1.tar", last modified: Mon Apr  8 19:24:14 2024, max compression
+gzip compressed data, was "pycountries-1.0.2.tar", last modified: Sat May  4 20:50:44 2024, max compression
```

## Comparing `pycountries-1.0.1.tar` & `pycountries-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 19:24:06.000000 pycountries-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-08 19:24:14.642955 pycountries-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-08 19:24:06.000000 pycountries-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 19:24:06.000000 pycountries-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:24:14.642955 pycountries-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 19:24:06.000000 pycountries-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.638955 pycountries-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/src/pycountries/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    85082 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)    43057 2024-04-08 19:24:06.000000 pycountries-1.0.1/src/pycountries/phones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/src/pycountries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 19:24:14.000000 pycountries-1.0.1/src/pycountries.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:24:14.642955 pycountries-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 19:24:06.000000 pycountries-1.0.1/tests/test_currencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.945775 pycountries-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-04 20:50:39.000000 pycountries-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 20:50:44.945775 pycountries-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-04 20:50:39.000000 pycountries-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-04 20:50:39.000000 pycountries-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:50:44.945775 pycountries-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 20:50:39.000000 pycountries-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.941775 pycountries-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.941775 pycountries-1.0.2/src/pycountries/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85082 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43057 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/phones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.945775 pycountries-1.0.2/src/pycountries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.945775 pycountries-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-04 20:50:39.000000 pycountries-1.0.2/tests/test_currencies.py
```

### Comparing `pycountries-1.0.1/LICENSE.md` & `pycountries-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/PKG-INFO` & `pycountries-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: pycountries
-Version: 1.0.1
+Version: 1.0.2
 Summary: List of existing countries and currencies
+Home-page: https://github.com/koldakov/pycountries
+Author: Ivan Koldakov
 Author-email: Ivan Koldakov <ivan@koldakov.com>
+License: MIT License
 Project-URL: Homepage, https://github.com/koldakov/pycountries
 Project-URL: Issues, https://github.com/koldakov/pycountries/issues
 Keywords: pydantic,fastapi,countries,currencies
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pycountries-1.0.1/README.md` & `pycountries-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/pyproject.toml` & `pycountries-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [project]
 name = "pycountries"
-version = "1.0.1"
+version = "1.0.2"
+license = {text = "MIT License"}
 authors = [
   { name="Ivan Koldakov", email="ivan@koldakov.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `pycountries-1.0.1/src/pycountries/__init__.py` & `pycountries-1.0.2/src/pycountries/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     WrongAmountDigitsNumberError,
     WrongAmountTypeError,
     ZeroAmountNotAllowedError,
 )
 from pycountries.languages import Language
 from pycountries.phones import Phone
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __author__ = "Ivan Koldakov"
 __all__ = [
     "AmountSpecialValuesNotAllowedError",
     "Country",
     "Currency",
     "Language",
     "NegativeAmountNotAllowedError",
```

### Comparing `pycountries-1.0.1/src/pycountries/_base.py` & `pycountries-1.0.2/src/pycountries/_base.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/src/pycountries/countries.py` & `pycountries-1.0.2/src/pycountries/countries.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/src/pycountries/currencies.py` & `pycountries-1.0.2/src/pycountries/currencies.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/src/pycountries/languages.py` & `pycountries-1.0.2/src/pycountries/languages.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/src/pycountries/phones.py` & `pycountries-1.0.2/src/pycountries/phones.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.1/src/pycountries.egg-info/PKG-INFO` & `pycountries-1.0.2/src/pycountries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: pycountries
-Version: 1.0.1
+Version: 1.0.2
 Summary: List of existing countries and currencies
+Home-page: https://github.com/koldakov/pycountries
+Author: Ivan Koldakov
 Author-email: Ivan Koldakov <ivan@koldakov.com>
+License: MIT License
 Project-URL: Homepage, https://github.com/koldakov/pycountries
 Project-URL: Issues, https://github.com/koldakov/pycountries/issues
 Keywords: pydantic,fastapi,countries,currencies
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pycountries-1.0.1/tests/test_currencies.py` & `pycountries-1.0.2/tests/test_currencies.py`

 * *Files identical despite different names*

