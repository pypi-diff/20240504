# Comparing `tmp/pysparkify-0.26.5.tar.gz` & `tmp/pysparkify-0.26.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkify-0.26.5.tar", last modified: Sat May  4 21:24:23 2024, max compression
+gzip compressed data, was "pysparkify-0.26.6.tar", last modified: Sat May  4 21:30:40 2024, max compression
```

## Comparing `pysparkify-0.26.5.tar` & `pysparkify-0.26.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.746502 pysparkify-0.26.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-04 21:24:23.746502 pysparkify-0.26.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-04 21:24:21.000000 pysparkify-0.26.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.742503 pysparkify-0.26.5/pysparkify/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.742503 pysparkify-0.26.5/pysparkify/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.746502 pysparkify-0.26.5/pysparkify/lib/sink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/sink/csv_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/sink/redshift_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/sink/s3_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/sink/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.746502 pysparkify-0.26.5/pysparkify/lib/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/source/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/source/redshift_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/source/s3_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/source/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/source/source_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.746502 pysparkify-0.26.5/pysparkify/lib/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/transformer/sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/lib/transformer/transformer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.746502 pysparkify-0.26.5/pysparkify/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-04 21:24:21.000000 pysparkify-0.26.5/pysparkify/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:24:23.746502 pysparkify-0.26.5/pysparkify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-04 21:24:23.000000 pysparkify-0.26.5/pysparkify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-04 21:24:23.000000 pysparkify-0.26.5/pysparkify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:24:23.000000 pysparkify-0.26.5/pysparkify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 21:24:23.000000 pysparkify-0.26.5/pysparkify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 21:24:23.000000 pysparkify-0.26.5/pysparkify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 21:24:23.000000 pysparkify-0.26.5/pysparkify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:24:23.746502 pysparkify-0.26.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-04 21:24:21.000000 pysparkify-0.26.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-04 21:30:40.337283 pysparkify-0.26.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-04 21:30:37.000000 pysparkify-0.26.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.333283 pysparkify-0.26.6/pysparkify/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/pysparkify/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/pysparkify/lib/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/sink/csv_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/sink/redshift_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/sink/s3_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/sink/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/pysparkify/lib/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/source/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/source/redshift_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/source/s3_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/source/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/source/source_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/pysparkify/lib/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/transformer/sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/lib/transformer/transformer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/pysparkify/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-04 21:30:37.000000 pysparkify-0.26.6/pysparkify/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:30:40.337283 pysparkify-0.26.6/pysparkify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-04 21:30:40.000000 pysparkify-0.26.6/pysparkify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-04 21:30:40.000000 pysparkify-0.26.6/pysparkify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 21:30:40.000000 pysparkify-0.26.6/pysparkify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 21:30:40.000000 pysparkify-0.26.6/pysparkify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 21:30:40.000000 pysparkify-0.26.6/pysparkify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 21:30:40.000000 pysparkify-0.26.6/pysparkify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:30:40.337283 pysparkify-0.26.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 21:30:37.000000 pysparkify-0.26.6/setup.py
```

### Comparing `pysparkify-0.26.5/PKG-INFO` & `pysparkify-0.26.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.5
+Version: 0.26.6
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pysparkify-0.26.5/README.md` & `pysparkify-0.26.6/README.md`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/app.py` & `pysparkify-0.26.6/pysparkify/lib/app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/sink/redshift_sink.py` & `pysparkify-0.26.6/pysparkify/lib/sink/redshift_sink.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/sink/sink_factory.py` & `pysparkify-0.26.6/pysparkify/lib/sink/sink_factory.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/source/redshift_source.py` & `pysparkify-0.26.6/pysparkify/lib/source/redshift_source.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/source/s3_source.py` & `pysparkify-0.26.6/pysparkify/lib/source/s3_source.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/source/source_factory.py` & `pysparkify-0.26.6/pysparkify/lib/source/source_factory.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/lib/transformer/sql_transformer.py` & `pysparkify-0.26.6/pysparkify/lib/transformer/sql_transformer.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify/tests/test_app.py` & `pysparkify-0.26.6/pysparkify/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/pysparkify.egg-info/PKG-INFO` & `pysparkify-0.26.6/pysparkify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkify
-Version: 0.26.5
+Version: 0.26.6
 Summary: Spark based ETL
 Home-page: https://github.com/raohammad/pysparkify
 Author: Hammad Aslam KHAN
 Author-email: raohammad@gmail.com
 License: MIT
 Keywords: python,pysparkify,etl,bigdata
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pysparkify-0.26.5/pysparkify.egg-info/SOURCES.txt` & `pysparkify-0.26.6/pysparkify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysparkify-0.26.5/setup.py` & `pysparkify-0.26.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='pysparkify',
-    version='0.26.5',
+    version='0.26.6',
     description='Spark based ETL',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hammad Aslam KHAN',
     author_email='raohammad@gmail.com',
     license='MIT',
     keywords=['python', 'pysparkify', 'etl', 'bigdata'],
@@ -27,12 +27,12 @@
     packages=find_packages(),
     install_requires=[
         'pyspark>=3.0.0',
         'pyyaml>=5.3'
     ],
     entry_points={
         'console_scripts': [
-            'pysparkify=lib.app:main'
+            'pysparkify=pysparkify:main'
         ]
     },
     classifiers=CLASSIFIERS,
 )
```

