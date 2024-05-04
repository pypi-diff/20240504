# Comparing `tmp/ComplexJSON-1.0.1.tar.gz` & `tmp/ComplexJSON-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ComplexJSON-1.0.1.tar", last modified: Wed May  1 21:48:31 2024, max compression
+gzip compressed data, was "ComplexJSON-1.1.0.tar", last modified: Sat May  4 19:27:06 2024, max compression
```

## Comparing `ComplexJSON-1.0.1.tar` & `ComplexJSON-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 21:48:31.663439 ComplexJSON-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-01 21:48:31.648929 ComplexJSON-1.0.1/ComplexJSON/
--rw-rw-rw-   0        0        0      151 2024-05-01 20:26:34.000000 ComplexJSON-1.0.1/ComplexJSON/__init__.py
--rw-rw-rw-   0        0        0      845 2024-05-01 20:24:25.000000 ComplexJSON-1.0.1/ComplexJSON/complexJSONDecoder.py
--rw-rw-rw-   0        0        0      376 2024-05-01 20:24:25.000000 ComplexJSON-1.0.1/ComplexJSON/complexJSONEncoder.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 20:24:25.000000 ComplexJSON-1.0.1/ComplexJSON/funcdef.py
--rw-rw-rw-   0        0        0      279 2024-05-01 19:50:01.000000 ComplexJSON-1.0.1/ComplexJSON/jsondef.py
--rw-rw-rw-   0        0        0       52 2024-05-01 20:24:25.000000 ComplexJSON-1.0.1/ComplexJSON/vardef.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:48:31.662438 ComplexJSON-1.0.1/ComplexJSON.egg-info/
--rw-rw-rw-   0        0        0     3091 2024-05-01 21:48:31.000000 ComplexJSON-1.0.1/ComplexJSON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-05-01 21:48:31.000000 ComplexJSON-1.0.1/ComplexJSON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 21:48:31.000000 ComplexJSON-1.0.1/ComplexJSON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-01 21:48:31.000000 ComplexJSON-1.0.1/ComplexJSON.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1063 2024-05-01 21:30:00.000000 ComplexJSON-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3091 2024-05-01 21:48:31.663439 ComplexJSON-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2592 2024-05-01 21:47:49.000000 ComplexJSON-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 21:48:31.665439 ComplexJSON-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-05-01 21:44:10.000000 ComplexJSON-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:27:06.029583 ComplexJSON-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-04 19:27:06.007908 ComplexJSON-1.1.0/ComplexJSON/
+-rw-rw-rw-   0        0        0      173 2024-05-04 18:11:06.000000 ComplexJSON-1.1.0/ComplexJSON/__init__.py
+-rw-rw-rw-   0        0        0     2166 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/ComplexJSON/complexJSONDecoder.py
+-rw-rw-rw-   0        0        0      924 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/ComplexJSON/complexJSONEncoder.py
+-rw-rw-rw-   0        0        0     3197 2024-05-04 19:24:51.000000 ComplexJSON-1.1.0/ComplexJSON/funcdef.py
+-rw-rw-rw-   0        0        0       52 2024-05-01 20:24:25.000000 ComplexJSON-1.1.0/ComplexJSON/vardef.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:27:06.027582 ComplexJSON-1.1.0/ComplexJSON.egg-info/
+-rw-rw-rw-   0        0        0     3950 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1063 2024-05-01 21:30:00.000000 ComplexJSON-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3950 2024-05-04 19:27:06.029583 ComplexJSON-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3451 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:27:06.031606 ComplexJSON-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/setup.py
```

### Comparing `ComplexJSON-1.0.1/ComplexJSON.egg-info/PKG-INFO` & `ComplexJSON-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ComplexJSON
-Version: 1.0.1
-Summary: This is the simplest module for serialize and deserialize python complex objects
-Home-page: https://github.com/dail45/ComplexJSON
-Author: dail45
-Keywords: json complexobject serialize
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ComplexJSON Library #
 
 ## What is this? ##
 The module allows you serialize your python complex objects to json and deserialize it.
 
 ## How to install ##
 
@@ -94,19 +80,14 @@
 with open("test.json", "wt", encoding="Utf-8") as f:
     json.dump(obj, f, cls=ComplexJSON.ComplexJSONEncoder)
 ...
 with open("test.json", "rt", encoding="Utf-8") as f:
     new_obj = json.load(json_obj, f, cls=ComplexJSON.ComplexJSONDecoder)
 ```
 
-#### Change json module ####
-
-This module by default uses builtin python json module in ComplexJSONEncoder and ComplexJSONDecoder.
-You can change it. Set environ "COMPLEX_JSON_MODULE_NAME" to name of your json library ("json" by default).
-
 #### Change codewords for ComplexJSON ####
 
 By default, the codewords for the module and class are "\_\_module\_\_" and "\_\_class\_\_", respectively
 
 ```python
 class A:
     def __init__(self):
@@ -124,13 +105,61 @@
 ```python
 from ComplexJSON import vardef
 
 vardef.classword = "_c_"
 vardef.moduleword = "_m_"
 ```
 
+Or
+
+```python
+import ComplexJSON
+
+ComplexJSON.vardef.classword = "_c_"
+ComplexJSON.vardef.moduleword = "_m_"
+```
+
 And now A class will be serialized as:
 ```python
 {"a": 1, "b": 2, "_m_": "__main__", "_c_": "A"}
 ```
 
-----------
+#### Remove codewords from json (v1.1+) ####
+
+```python
+from ComplexJSON import vardef
+
+vardef.classword = None  # remove classword from json
+vardef.moduleword = None  # remove moduleword from json
+```
+
+If you remove both, object will be decoded as python dict.
+If you remove moduleword, you need to provide class in classStorage argument in load, loads or ComplexJSONDecoder
+```python
+import ComplexJSON as json
+json.vardef.moduleword = None
+class A:
+    b = 1
+...
+classStorage = [A]
+# or
+classStorage = {"A": A}
+...
+json.loads(obj, classStorage=classStorage)
+# or
+decoder = json.ComplexJSONDecoder(classStorage=classStorage)
+...
+decoder.decode(obj)
+# or 
+json.loads(obj, object_hook=decoder.object_hook)
+```
+
+#### Local codewords (v1.1+) ####
+
+```python
+import ComplexJSON as json
+...
+_json = json.dumps(obj, localClassWord="Type", localModuleWord="Module")
+new_obj = json.loads(_json, localClassWord="Type", localModuleWord="Module")
+```
+
+----------
```

### Comparing `ComplexJSON-1.0.1/LICENSE` & `ComplexJSON-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ComplexJSON-1.0.1/PKG-INFO` & `ComplexJSON-1.1.0/ComplexJSON.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComplexJSON
-Version: 1.0.1
+Version: 1.1.0
 Summary: This is the simplest module for serialize and deserialize python complex objects
 Home-page: https://github.com/dail45/ComplexJSON
 Author: dail45
 Keywords: json complexobject serialize
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -94,19 +94,14 @@
 with open("test.json", "wt", encoding="Utf-8") as f:
     json.dump(obj, f, cls=ComplexJSON.ComplexJSONEncoder)
 ...
 with open("test.json", "rt", encoding="Utf-8") as f:
     new_obj = json.load(json_obj, f, cls=ComplexJSON.ComplexJSONDecoder)
 ```
 
-#### Change json module ####
-
-This module by default uses builtin python json module in ComplexJSONEncoder and ComplexJSONDecoder.
-You can change it. Set environ "COMPLEX_JSON_MODULE_NAME" to name of your json library ("json" by default).
-
 #### Change codewords for ComplexJSON ####
 
 By default, the codewords for the module and class are "\_\_module\_\_" and "\_\_class\_\_", respectively
 
 ```python
 class A:
     def __init__(self):
@@ -124,13 +119,61 @@
 ```python
 from ComplexJSON import vardef
 
 vardef.classword = "_c_"
 vardef.moduleword = "_m_"
 ```
 
+Or
+
+```python
+import ComplexJSON
+
+ComplexJSON.vardef.classword = "_c_"
+ComplexJSON.vardef.moduleword = "_m_"
+```
+
 And now A class will be serialized as:
 ```python
 {"a": 1, "b": 2, "_m_": "__main__", "_c_": "A"}
 ```
 
+#### Remove codewords from json (v1.1+) ####
+
+```python
+from ComplexJSON import vardef
+
+vardef.classword = None  # remove classword from json
+vardef.moduleword = None  # remove moduleword from json
+```
+
+If you remove both, object will be decoded as python dict.
+If you remove moduleword, you need to provide class in classStorage argument in load, loads or ComplexJSONDecoder
+```python
+import ComplexJSON as json
+json.vardef.moduleword = None
+class A:
+    b = 1
+...
+classStorage = [A]
+# or
+classStorage = {"A": A}
+...
+json.loads(obj, classStorage=classStorage)
+# or
+decoder = json.ComplexJSONDecoder(classStorage=classStorage)
+...
+decoder.decode(obj)
+# or 
+json.loads(obj, object_hook=decoder.object_hook)
+```
+
+#### Local codewords (v1.1+) ####
+
+```python
+import ComplexJSON as json
+...
+_json = json.dumps(obj, localClassWord="Type", localModuleWord="Module")
+new_obj = json.loads(_json, localClassWord="Type", localModuleWord="Module")
+```
+
 ----------
```

### Comparing `ComplexJSON-1.0.1/setup.py` & `ComplexJSON-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='ComplexJSON',
-    version='1.0.1',
+    version='1.1.0',
     author='dail45',
     description='This is the simplest module for serialize and deserialize python complex objects',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     url="https://github.com/dail45/ComplexJSON",
     classifiers=[
```

