# Comparing `tmp/alfred_pyflow-0.4.6.tar.gz` & `tmp/alfred_pyflow-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_pyflow-0.4.6.tar", max compression
+gzip compressed data, was "alfred_pyflow-0.4.7.tar", max compression
```

## Comparing `alfred_pyflow-0.4.6.tar` & `alfred_pyflow-0.4.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       15 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/README.md
--rw-r--r--   0        0        0       54 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyflow/__init__.py
--rw-r--r--   0        0        0      542 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyflow/cache.py
--rw-r--r--   0        0        0     6609 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyflow/icon.py
--rw-r--r--   0        0        0     2601 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyflow/item.py
--rw-r--r--   0        0        0     1578 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyflow/testing.py
--rw-r--r--   0        0        0     2344 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyflow/workflow.py
--rw-r--r--   0        0        0     1014 2023-11-25 17:02:40.725062 alfred_pyflow-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.6/setup.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/README.md
+-rw-r--r--   0        0        0       54 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyflow/__init__.py
+-rw-r--r--   0        0        0      542 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyflow/cache.py
+-rw-r--r--   0        0        0     6609 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyflow/icon.py
+-rw-r--r--   0        0        0     2601 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyflow/item.py
+-rw-r--r--   0        0        0     1578 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyflow/testing.py
+-rw-r--r--   0        0        0     2344 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyflow/workflow.py
+-rw-r--r--   0        0        0     1013 2024-05-04 17:56:07.610825 alfred_pyflow-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.7/setup.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 alfred_pyflow-0.4.7/PKG-INFO
```

### Comparing `alfred_pyflow-0.4.6/pyflow/cache.py` & `alfred_pyflow-0.4.7/pyflow/cache.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.6/pyflow/icon.py` & `alfred_pyflow-0.4.7/pyflow/icon.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.6/pyflow/item.py` & `alfred_pyflow-0.4.7/pyflow/item.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.6/pyflow/testing.py` & `alfred_pyflow-0.4.7/pyflow/testing.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.6/pyflow/workflow.py` & `alfred_pyflow-0.4.7/pyflow/workflow.py`

 * *Files identical despite different names*

### Comparing `alfred_pyflow-0.4.6/pyproject.toml` & `alfred_pyflow-0.4.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "alfred-pyflow"
 description = "Minimal library for the development of Alfred Workflows."
 documentation = "https://github.com/fedecalendino/alfred-pyflow/blob/main/README.md"
 homepage = "https://github.com/fedecalendino/alfred-pyflow"
 license = "MIT"
 readme = "README.md"
-version = "0.4.6"
+version = "0.4.7"
 
 authors = [
   "Fede Calendino <fede@calendino.com>",
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
@@ -25,20 +25,20 @@
 packages = [
   { include = "pyflow" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.30.0"
-urllib3 = "1.26.6"
+urllib3 = "2.2.1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3.0"
-coverage = "^7.2.5"
-ddt = "^1.6.0"
+black = "^24.4.2"
+coverage = "^7.5.1"
+ddt = "^1.7.2"
 
 [tool.black]
 line-length = 150
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alfred_pyflow-0.4.6/setup.py` & `alfred_pyflow-0.4.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pyflow']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['requests>=2.30.0,<3.0.0', 'urllib3==1.26.6']
+['requests>=2.30.0,<3.0.0', 'urllib3==2.2.1']
 
 setup_kwargs = {
     'name': 'alfred-pyflow',
-    'version': '0.4.6',
+    'version': '0.4.7',
     'description': 'Minimal library for the development of Alfred Workflows.',
     'long_description': '# alfred-pyflow',
     'author': 'Fede Calendino',
     'author_email': 'fede@calendino.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fedecalendino/alfred-pyflow',
```

### Comparing `alfred_pyflow-0.4.6/PKG-INFO` & `alfred_pyflow-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-pyflow
-Version: 0.4.6
+Version: 0.4.7
 Summary: Minimal library for the development of Alfred Workflows.
 Home-page: https://github.com/fedecalendino/alfred-pyflow
 License: MIT
 Keywords: alfred,workflow
 Author: Fede Calendino
 Author-email: fede@calendino.com
 Requires-Python: >=3.8,<4.0
@@ -16,12 +16,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: requests (>=2.30.0,<3.0.0)
-Requires-Dist: urllib3 (==1.26.6)
+Requires-Dist: urllib3 (==2.2.1)
 Project-URL: Documentation, https://github.com/fedecalendino/alfred-pyflow/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # alfred-pyflow
```

