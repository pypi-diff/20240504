# Comparing `tmp/snapquery-0.0.1.tar.gz` & `tmp/snapquery-0.0.2.tar.gz`

## Comparing `snapquery-0.0.1.tar` & `snapquery-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 snapquery-0.0.1/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.1/.pydevproject
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.1/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.1/scripts/blackisort
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.1/scripts/install
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.1/scripts/test
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.1/snapquery/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 snapquery-0.0.1/snapquery/snapquery_cmd.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 snapquery-0.0.1/snapquery/snapquery_core.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 snapquery-0.0.1/snapquery/snapquery_webserver.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.1/snapquery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 snapquery-0.0.1/tests/test_endpoints.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.1/LICENSE
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.1/README.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 snapquery-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 snapquery-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.2/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.2/.pydevproject
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.2/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.2/scripts/blackisort
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.2/scripts/install
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.2/scripts/test
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/__init__.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/snapquery_cmd.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/snapquery_core.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/snapquery_webserver.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.2/snapquery/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 snapquery-0.0.2/tests/test_restful_api.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.2/README.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 snapquery-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 snapquery-0.0.2/PKG-INFO
```

### Comparing `snapquery-0.0.1/.github/workflows/build.yml` & `snapquery-0.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.1/.github/workflows/upload-to-pypi.yml` & `snapquery-0.0.2/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.1/snapquery/version.py` & `snapquery-0.0.2/snapquery/version.py`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.1/.gitignore` & `snapquery-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.1/LICENSE` & `snapquery-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.1/README.md` & `snapquery-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.1/pyproject.toml` & `snapquery-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 readme = "README.md"
 license = {text = "Apache-2.0"}
 dependencies = [
 	# https://github.com/WolfgangFahl/nicegui_widgets
 	"ngwidgets>=0.14.2",
   # https://pypi.org/project/pyLodStorage/
-  "pyLodStorage>=0.10.3"
+  "pyLodStorage>=0.10.4"
 ]
 
 requires-python = ">=3.9"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `snapquery-0.0.1/PKG-INFO` & `snapquery-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapquery
-Version: 0.0.1
+Version: 0.0.2
 Summary: snapquery: Introduce Named Queries and Named Query Middleware to wikidata
 Project-URL: Home, https://github.com/WolfgangFahl/snapquery
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/snapquery
 Project-URL: Source, https://github.com/WolfgangFahl/snapquery
 Author-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 Maintainer-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 License: Apache-2.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.9
 Requires-Dist: ngwidgets>=0.14.2
-Requires-Dist: pylodstorage>=0.10.3
+Requires-Dist: pylodstorage>=0.10.4
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
 
 # snapQuery
 Tool that helps users preview, annotate, rate, comment, run and explore Wikidata queries on different sparql backends seamlessly. 
 It enhances the user experience by storing the results and comparing the results from different backends and comparing over time.
```

