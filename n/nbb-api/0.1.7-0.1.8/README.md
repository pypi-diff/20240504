# Comparing `tmp/nbb_api-0.1.7.tar.gz` & `tmp/nbb_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbb_api-0.1.7.tar", last modified: Sat May  4 19:40:27 2024, max compression
+gzip compressed data, was "nbb_api-0.1.8.tar", last modified: Sat May  4 19:48:16 2024, max compression
```

## Comparing `nbb_api-0.1.7.tar` & `nbb_api-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 19:40:27.457401 nbb_api-0.1.7/
--rw-rw-rw-   0        0        0     1075 2024-05-04 19:18:00.000000 nbb_api-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     3066 2024-05-04 19:40:27.456405 nbb_api-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2024-05-04 19:20:35.000000 nbb_api-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 19:40:27.456405 nbb_api-0.1.7/nbb_api.egg-info/
--rw-rw-rw-   0        0        0     3066 2024-05-04 19:40:27.000000 nbb_api-0.1.7/nbb_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-05-04 19:40:27.000000 nbb_api-0.1.7/nbb_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:40:27.000000 nbb_api-0.1.7/nbb_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-04 19:40:27.000000 nbb_api-0.1.7/nbb_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:40:27.000000 nbb_api-0.1.7/nbb_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 19:40:27.457401 nbb_api-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-04 19:39:59.000000 nbb_api-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:48:16.620365 nbb_api-0.1.8/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 19:18:00.000000 nbb_api-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3066 2024-05-04 19:48:16.619368 nbb_api-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2024-05-04 19:20:35.000000 nbb_api-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:48:16.619368 nbb_api-0.1.8/nbb_api.egg-info/
+-rw-rw-rw-   0        0        0     3066 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:48:16.620365 nbb_api-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-04 19:44:27.000000 nbb_api-0.1.8/setup.py
```

### Comparing `nbb_api-0.1.7/LICENSE` & `nbb_api-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nbb_api-0.1.7/PKG-INFO` & `nbb_api-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbb_api
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB
 Home-page: https://github.com/GabrielPastorello/nbb_api
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international basketball,brazil,ldb,liga-ouro
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nbb_api Version: 0.1.7 Summary: Python package for
+Metadata-Version: 2.1 Name: nbb_api Version: 0.1.8 Summary: Python package for
 easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro
 and LDB Home-page: https://github.com/GabrielPastorello/nbb_api Author: Gabriel
 Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international
 basketball,brazil,ldb,liga-ouro Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
```

### Comparing `nbb_api-0.1.7/README.md` & `nbb_api-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nbb_api-0.1.7/nbb_api.egg-info/PKG-INFO` & `nbb_api-0.1.8/nbb_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbb_api
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB
 Home-page: https://github.com/GabrielPastorello/nbb_api
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international basketball,brazil,ldb,liga-ouro
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nbb_api Version: 0.1.7 Summary: Python package for
+Metadata-Version: 2.1 Name: nbb_api Version: 0.1.8 Summary: Python package for
 easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro
 and LDB Home-page: https://github.com/GabrielPastorello/nbb_api Author: Gabriel
 Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international
 basketball,brazil,ldb,liga-ouro Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
```

### Comparing `nbb_api-0.1.7/setup.py` & `nbb_api-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
             name='nbb_api',
-            version='0.1.7',
+            version='0.1.8',
             description='Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB',
             long_description=long_description,
             long_description_content_type="text/markdown",
             url='https://github.com/GabrielPastorello/nbb_api',
             author='Gabriel Speranza Pastorello',
             author_email='gabriel.pastorello01@gmail.com',
             license='MIT',
```

