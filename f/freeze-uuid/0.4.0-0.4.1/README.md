# Comparing `tmp/freeze_uuid-0.4.0.tar.gz` & `tmp/freeze_uuid-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_uuid-0.4.0.tar", last modified: Sun Apr 21 19:04:13 2024, max compression
+gzip compressed data, was "freeze_uuid-0.4.1.tar", last modified: Fri May  3 18:23:31 2024, max compression
```

## Comparing `freeze_uuid-0.4.0.tar` & `freeze_uuid-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.563493 freeze_uuid-0.4.0/freeze_uuid/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/freeze_uuid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/freeze_uuid/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/freeze_uuid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 19:04:13.000000 freeze_uuid-0.4.0/freeze_uuid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:04:13.567493 freeze_uuid-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:13.563493 freeze_uuid-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-21 19:04:09.000000 freeze_uuid-0.4.0/tests/testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:23:31.847414 freeze_uuid-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-03 18:23:31.847414 freeze_uuid-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:23:31.847414 freeze_uuid-0.4.1/freeze_uuid/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/freeze_uuid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/freeze_uuid/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:23:31.847414 freeze_uuid-0.4.1/freeze_uuid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-03 18:23:31.000000 freeze_uuid-0.4.1/freeze_uuid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-03 18:23:31.000000 freeze_uuid-0.4.1/freeze_uuid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:23:31.000000 freeze_uuid-0.4.1/freeze_uuid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 18:23:31.000000 freeze_uuid-0.4.1/freeze_uuid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:23:31.847414 freeze_uuid-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:23:31.847414 freeze_uuid-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-03 18:23:27.000000 freeze_uuid-0.4.1/tests/testdata.py
```

### Comparing `freeze_uuid-0.4.0/LICENSE` & `freeze_uuid-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_uuid-0.4.0/PKG-INFO` & `freeze_uuid-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-uuid
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package for mocking uuid.
 Author: Alexander Balashov
 Author-email: alaex777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `freeze_uuid-0.4.0/README.md` & `freeze_uuid-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `freeze_uuid-0.4.0/freeze_uuid/main.py` & `freeze_uuid-0.4.1/freeze_uuid/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 DEFAULT_VALUE = '00000000-0000-0000-0000-000000000000'
 
 VALUES = [DEFAULT_VALUE]
 COUNT = 0
 
 
 class FakeUUID(uuid.UUID):
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         global COUNT
         self.value = VALUES[COUNT] if COUNT < len(VALUES) else VALUES[-1]
-        self.int = int(self.value.replace('-', ''), 16)
+        self.int = int(self.value.replace('-', ''), 16)  # type: ignore
         COUNT += 1
 
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value: Any) -> None:
         object.__setattr__(self, name, value)
 
     def __str__(self) -> str:
         return self.value
 
     def __eq__(self, __value: object) -> bool:
         return str(__value) == self.value
 
 
 def freeze_uuid(values: Union[str, list] = DEFAULT_VALUE) -> Callable:
     def inner(func: Callable) -> Callable:
-        def value_magic():
+        def value_magic() -> None:
             global VALUES
             if isinstance(values, str):
                 VALUES = [values]
             else:
                 VALUES = values
 
             global COUNT
@@ -67,15 +67,15 @@
             return async_wrapper
 
         return wrapper
     return inner
 
 
 class freeze_uuid_manager:
-    def __init__(self, values: Union[str, list[str]]) -> None:
+    def __init__(self, values: Union[str, list[str]] = DEFAULT_VALUE) -> None:
         global VALUES
         if isinstance(values, str):
             VALUES = [values]
         else:
             VALUES = values
 
         for value in VALUES:
@@ -85,9 +85,9 @@
         COUNT = 0
 
         self.prev_uuid = uuid.UUID
 
     def __enter__(self) -> None:
         uuid.UUID = FakeUUID
 
-    def __exit__(self, *args) -> None:
+    def __exit__(self, *args: Any) -> None:
         uuid.UUID = self.prev_uuid
```

### Comparing `freeze_uuid-0.4.0/freeze_uuid.egg-info/PKG-INFO` & `freeze_uuid-0.4.1/freeze_uuid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-uuid
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package for mocking uuid.
 Author: Alexander Balashov
 Author-email: alaex777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `freeze_uuid-0.4.0/setup.py` & `freeze_uuid-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='freeze-uuid',
-    version='0.4.0',
+    version='0.4.1',
     author='Alexander Balashov',
     author_email='alaex777@gmail.com',
     description='Python package for mocking uuid.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

