# Comparing `tmp/py-memoize-1.1.5.tar.gz` & `tmp/py-memoize-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-memoize-1.1.5.tar", last modified: Fri May  3 19:42:30 2024, max compression
+gzip compressed data, was "py-memoize-1.2.0.tar", last modified: Sat May  4 06:11:50 2024, max compression
```

## Comparing `py-memoize-1.1.5.tar` & `py-memoize-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:42:30.045339 py-memoize-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-03 19:42:18.000000 py-memoize-1.1.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 19:42:18.000000 py-memoize-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-03 19:42:30.045339 py-memoize-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-05-03 19:42:18.000000 py-memoize-1.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:42:30.045339 py-memoize-1.1.5/memoize/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/coerced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/entrybuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/invalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/memoize_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:42:30.045339 py-memoize-1.1.5/py_memoize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-03 19:42:30.000000 py-memoize-1.1.5/py_memoize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:42:30.045339 py-memoize-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-03 19:42:18.000000 py-memoize-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:11:50.894727 py-memoize-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 06:11:42.000000 py-memoize-1.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 06:11:42.000000 py-memoize-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 06:11:50.894727 py-memoize-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17881 2024-05-04 06:11:42.000000 py-memoize-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:11:50.894727 py-memoize-1.2.0/memoize/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/coerced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/entrybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/memoize_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:11:50.894727 py-memoize-1.2.0/py_memoize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:11:50.894727 py-memoize-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-04 06:11:42.000000 py-memoize-1.2.0/setup.py
```

### Comparing `py-memoize-1.1.5/LICENCE` & `py-memoize-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/PKG-INFO` & `py-memoize-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.1.5
+Version: 1.2.0
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/x-rst
 Provides-Extra: tornado
 Provides-Extra: ujson
 License-File: LICENCE
 
@@ -98,14 +99,17 @@
 
 Provided examples use default configuration to cache results in memory.
 For configuration options see `Configurability`_.
 
 You can use ``memoize`` with both `asyncio <https://docs.python.org/3/library/asyncio.html>`_
 and `Tornado <https://github.com/tornadoweb/tornado>`_ -  please see the appropriate example:
 
+.. warning::
+    Support for `Tornado <https://github.com/tornadoweb/tornado>`_ is planned to be removed in the future.
+
 asyncio
 ~~~~~~~
 
 To apply default caching configuration use:
 
 ..
     _example_source: examples/basic/basic_asyncio.py
```

### Comparing `py-memoize-1.1.5/README.rst` & `py-memoize-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 
 Provided examples use default configuration to cache results in memory.
 For configuration options see `Configurability`_.
 
 You can use ``memoize`` with both `asyncio <https://docs.python.org/3/library/asyncio.html>`_
 and `Tornado <https://github.com/tornadoweb/tornado>`_ -  please see the appropriate example:
 
+.. warning::
+    Support for `Tornado <https://github.com/tornadoweb/tornado>`_ is planned to be removed in the future.
+
 asyncio
 ~~~~~~~
 
 To apply default caching configuration use:
 
 ..
     _example_source: examples/basic/basic_asyncio.py
```

### Comparing `py-memoize-1.1.5/memoize/configuration.py` & `py-memoize-1.2.0/memoize/configuration.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/entry.py` & `py-memoize-1.2.0/memoize/entry.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/entrybuilder.py` & `py-memoize-1.2.0/memoize/entrybuilder.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/eviction.py` & `py-memoize-1.2.0/memoize/eviction.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/invalidation.py` & `py-memoize-1.2.0/memoize/invalidation.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/key.py` & `py-memoize-1.2.0/memoize/key.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/serde.py` & `py-memoize-1.2.0/memoize/serde.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/statuses.py` & `py-memoize-1.2.0/memoize/statuses.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/storage.py` & `py-memoize-1.2.0/memoize/storage.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/memoize/wrapper.py` & `py-memoize-1.2.0/memoize/wrapper.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.5/py_memoize.egg-info/PKG-INFO` & `py-memoize-1.2.0/py_memoize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.1.5
+Version: 1.2.0
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/x-rst
 Provides-Extra: tornado
 Provides-Extra: ujson
 License-File: LICENCE
 
@@ -98,14 +99,17 @@
 
 Provided examples use default configuration to cache results in memory.
 For configuration options see `Configurability`_.
 
 You can use ``memoize`` with both `asyncio <https://docs.python.org/3/library/asyncio.html>`_
 and `Tornado <https://github.com/tornadoweb/tornado>`_ -  please see the appropriate example:
 
+.. warning::
+    Support for `Tornado <https://github.com/tornadoweb/tornado>`_ is planned to be removed in the future.
+
 asyncio
 ~~~~~~~
 
 To apply default caching configuration use:
 
 ..
     _example_source: examples/basic/basic_asyncio.py
```

### Comparing `py-memoize-1.1.5/setup.py` & `py-memoize-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
+from setuptools import setup
 
 
 def prepare_description():
     description = open('README.rst', 'rb').read().decode('utf-8')
     # class references work well in generated docs (render links to API docs)
     # but don't work at PyPi - therefore are removed
     description = description.replace(":class:", "")
     return description
 
 
 setup(
     name='py-memoize',
-    version='1.1.5',
+    version='1.2.0',
     author='Michal Zmuda',
     author_email='zmu.michal@gmail.com',
     url='https://github.com/DreamLab/memoize',
     maintainer='DreamLab',
     packages=['memoize'],
     test_suite='tests',
     license='Apache License 2.0',
@@ -38,11 +35,12 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: AsyncIO',
         'Intended Audience :: Developers'
     ]
 )
```

