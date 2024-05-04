# Comparing `tmp/python_redux-0.9.9.tar.gz` & `tmp/python_redux-0.9.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_redux-0.9.9.tar", max compression
+gzip compressed data, was "python_redux-0.9.9a0.tar", max compression
```

## Comparing `python_redux-0.9.9.tar` & `python_redux-0.9.9a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-11-12 10:50:18.883066 python_redux-0.9.9/LICENSE
--rw-r--r--   0        0        0     7425 2023-12-27 20:56:28.648245 python_redux-0.9.9/README.md
--rw-r--r--   0        0        0      909 2023-12-30 19:44:07.833485 python_redux-0.9.9/pyproject.toml
--rw-r--r--   0        0        0       79 2023-12-01 00:43:04.608940 python_redux-0.9.9/redux/__init__.py
--rw-r--r--   0        0        0     2206 2023-12-30 19:43:16.310374 python_redux-0.9.9/redux/basic_types.py
--rw-r--r--   0        0        0     4631 2023-12-27 13:02:46.573904 python_redux-0.9.9/redux/combine_reducers.py
--rw-r--r--   0        0        0    10332 2023-12-30 19:16:53.477653 python_redux-0.9.9/redux/main.py
--rw-r--r--   0        0        0     8080 1970-01-01 00:00:00.000000 python_redux-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-12 10:50:18.883066 python_redux-0.9.9a0/LICENSE
+-rw-r--r--   0        0        0     7425 2023-12-27 20:56:28.648245 python_redux-0.9.9a0/README.md
+-rw-r--r--   0        0        0      911 2023-12-31 08:36:52.841446 python_redux-0.9.9a0/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-12-01 00:43:04.608940 python_redux-0.9.9a0/redux/__init__.py
+-rw-r--r--   0        0        0     2196 2023-12-31 08:36:40.489009 python_redux-0.9.9a0/redux/basic_types.py
+-rw-r--r--   0        0        0     4631 2023-12-27 13:02:46.573904 python_redux-0.9.9a0/redux/combine_reducers.py
+-rw-r--r--   0        0        0    10332 2023-12-30 19:16:53.477653 python_redux-0.9.9a0/redux/main.py
+-rw-r--r--   0        0        0     8082 1970-01-01 00:00:00.000000 python_redux-0.9.9a0/PKG-INFO
```

### Comparing `python_redux-0.9.9/LICENSE` & `python_redux-0.9.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_redux-0.9.9/README.md` & `python_redux-0.9.9a0/README.md`

 * *Files identical despite different names*

### Comparing `python_redux-0.9.9/pyproject.toml` & `python_redux-0.9.9a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-redux"
-version = "0.9.9"
+version = "0.9.9a0"
 description = "Redux implementation for Python"
 authors = ["Sassan Haradji <sassanh@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "redux" }]
 
 [tool.poetry.dependencies]
```

### Comparing `python_redux-0.9.9/redux/basic_types.py` & `python_redux-0.9.9a0/redux/basic_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 ]
 
 
 class InitializationActionError(Exception):
     def __init__(self: InitializationActionError, action: BaseAction) -> None:
         super().__init__(
             f"""The only accepted action type when state is None is "InitAction", \
-action with type "{type(action)}" is passed""",
+action "{action}" is not allowed.""",
         )
 
 
 class InitAction(BaseAction):
     ...
```

### Comparing `python_redux-0.9.9/redux/combine_reducers.py` & `python_redux-0.9.9a0/redux/combine_reducers.py`

 * *Files identical despite different names*

### Comparing `python_redux-0.9.9/redux/main.py` & `python_redux-0.9.9a0/redux/main.py`

 * *Files identical despite different names*

### Comparing `python_redux-0.9.9/PKG-INFO` & `python_redux-0.9.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redux
-Version: 0.9.9
+Version: 0.9.9a0
 Summary: Redux implementation for Python
 License: Apache-2.0
 Author: Sassan Haradji
 Author-email: sassanh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

