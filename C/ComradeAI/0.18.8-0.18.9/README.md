# Comparing `tmp/ComradeAI-0.18.8.tar.gz` & `tmp/ComradeAI-0.18.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ComradeAI-0.18.8.tar", last modified: Thu Feb 15 20:42:47 2024, max compression
+gzip compressed data, was "ComradeAI-0.18.9.tar", last modified: Thu Feb 15 20:59:35 2024, max compression
```

## Comparing `ComradeAI-0.18.8.tar` & `ComradeAI-0.18.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 20:42:47.737308 ComradeAI-0.18.8/
-drwxrwxrwx   0        0        0        0 2024-02-15 20:42:47.721648 ComradeAI-0.18.8/ComradeAI/
--rw-rw-rw-   0        0        0     7051 2024-02-15 19:48:26.000000 ComradeAI-0.18.8/ComradeAI/DocumentRoutines.py
--rw-rw-rw-   0        0        0    55695 2024-02-15 19:48:58.000000 ComradeAI-0.18.8/ComradeAI/Mycelium.py
--rw-rw-rw-   0        0        0    27556 2024-02-15 19:48:24.000000 ComradeAI-0.18.8/ComradeAI/Processors.py
--rw-rw-rw-   0        0        0        0 2023-12-26 17:48:02.000000 ComradeAI-0.18.8/ComradeAI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 20:42:47.737308 ComradeAI-0.18.8/ComradeAI.egg-info/
--rw-rw-rw-   0        0        0     2241 2024-02-15 20:42:47.000000 ComradeAI-0.18.8/ComradeAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-02-15 20:42:47.000000 ComradeAI-0.18.8/ComradeAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 20:42:47.000000 ComradeAI-0.18.8/ComradeAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-02-15 20:42:47.000000 ComradeAI-0.18.8/ComradeAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-15 20:42:47.000000 ComradeAI-0.18.8/ComradeAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-12-09 17:43:42.000000 ComradeAI-0.18.8/LICENSE
--rw-rw-rw-   0        0        0       41 2024-01-12 20:02:10.000000 ComradeAI-0.18.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2241 2024-02-15 20:42:47.737308 ComradeAI-0.18.8/PKG-INFO
--rw-rw-rw-   0        0        0     1587 2024-01-18 23:43:44.000000 ComradeAI-0.18.8/README.md
--rw-rw-rw-   0        0        0       80 2024-02-15 19:35:00.000000 ComradeAI-0.18.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-15 20:42:47.752248 ComradeAI-0.18.8/setup.cfg
--rw-rw-rw-   0        0        0      803 2024-02-15 20:42:34.000000 ComradeAI-0.18.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-15 20:59:35.179476 ComradeAI-0.18.9/
+drwxrwxrwx   0        0        0        0 2024-02-15 20:59:35.151892 ComradeAI-0.18.9/ComradeAI/
+-rw-rw-rw-   0        0        0     7051 2024-02-15 19:48:26.000000 ComradeAI-0.18.9/ComradeAI/DocumentRoutines.py
+-rw-rw-rw-   0        0        0    55695 2024-02-15 19:48:58.000000 ComradeAI-0.18.9/ComradeAI/Mycelium.py
+-rw-rw-rw-   0        0        0    27556 2024-02-15 19:48:24.000000 ComradeAI-0.18.9/ComradeAI/Processors.py
+-rw-rw-rw-   0        0        0        0 2023-12-26 17:48:02.000000 ComradeAI-0.18.9/ComradeAI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-15 20:59:35.172734 ComradeAI-0.18.9/ComradeAI.egg-info/
+-rw-rw-rw-   0        0        0     2241 2024-02-15 20:59:34.000000 ComradeAI-0.18.9/ComradeAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-02-15 20:59:35.000000 ComradeAI-0.18.9/ComradeAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-15 20:59:34.000000 ComradeAI-0.18.9/ComradeAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-02-15 20:59:34.000000 ComradeAI-0.18.9/ComradeAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-02-15 20:59:34.000000 ComradeAI-0.18.9/ComradeAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-12-09 17:43:42.000000 ComradeAI-0.18.9/LICENSE
+-rw-rw-rw-   0        0        0       41 2024-01-12 20:02:10.000000 ComradeAI-0.18.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2241 2024-02-15 20:59:35.172734 ComradeAI-0.18.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1587 2024-01-18 23:43:44.000000 ComradeAI-0.18.9/README.md
+-rw-rw-rw-   0        0        0       80 2024-02-15 19:35:00.000000 ComradeAI-0.18.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-02-15 20:59:35.179476 ComradeAI-0.18.9/setup.cfg
+-rw-rw-rw-   0        0        0      803 2024-02-15 20:59:01.000000 ComradeAI-0.18.9/setup.py
```

### Comparing `ComradeAI-0.18.8/ComradeAI/DocumentRoutines.py` & `ComradeAI-0.18.9/ComradeAI/DocumentRoutines.py`

 * *Files identical despite different names*

### Comparing `ComradeAI-0.18.8/ComradeAI/Mycelium.py` & `ComradeAI-0.18.9/ComradeAI/Mycelium.py`

 * *Files identical despite different names*

### Comparing `ComradeAI-0.18.8/ComradeAI/Processors.py` & `ComradeAI-0.18.9/ComradeAI/Processors.py`

 * *Files identical despite different names*

### Comparing `ComradeAI-0.18.8/ComradeAI.egg-info/PKG-INFO` & `ComradeAI-0.18.9/ComradeAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComradeAI
-Version: 0.18.8
+Version: 0.18.9
 Summary: A protocol and SDK for unified AI service interaction
 Home-page: https://github.com/SergeiKarulin/ComradeAI
 Author: Sergei Karulin
 Author-email: sk@spellsystems.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ComradeAI-0.18.8/LICENSE` & `ComradeAI-0.18.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ComradeAI-0.18.8/PKG-INFO` & `ComradeAI-0.18.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComradeAI
-Version: 0.18.8
+Version: 0.18.9
 Summary: A protocol and SDK for unified AI service interaction
 Home-page: https://github.com/SergeiKarulin/ComradeAI
 Author: Sergei Karulin
 Author-email: sk@spellsystems.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ComradeAI-0.18.8/README.md` & `ComradeAI-0.18.9/README.md`

 * *Files identical despite different names*

### Comparing `ComradeAI-0.18.8/setup.py` & `ComradeAI-0.18.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='ComradeAI',
-    version='0.18.8',
+    version='0.18.9',
     packages=find_packages(),
     description='A protocol and SDK for unified AI service interaction',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=requirements,
     author='Sergei Karulin',
     author_email='sk@spellsystems.com',
```

