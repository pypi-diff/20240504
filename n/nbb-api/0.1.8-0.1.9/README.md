# Comparing `tmp/nbb_api-0.1.8.tar.gz` & `tmp/nbb_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbb_api-0.1.8.tar", last modified: Sat May  4 19:48:16 2024, max compression
+gzip compressed data, was "nbb_api-0.1.9.tar", last modified: Sat May  4 19:58:23 2024, max compression
```

## Comparing `nbb_api-0.1.8.tar` & `nbb_api-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 19:48:16.620365 nbb_api-0.1.8/
--rw-rw-rw-   0        0        0     1075 2024-05-04 19:18:00.000000 nbb_api-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3066 2024-05-04 19:48:16.619368 nbb_api-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2024-05-04 19:20:35.000000 nbb_api-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 19:48:16.619368 nbb_api-0.1.8/nbb_api.egg-info/
--rw-rw-rw-   0        0        0     3066 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:48:16.000000 nbb_api-0.1.8/nbb_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 19:48:16.620365 nbb_api-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-04 19:44:27.000000 nbb_api-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:58:23.122723 nbb_api-0.1.9/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 19:18:00.000000 nbb_api-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3066 2024-05-04 19:58:23.122723 nbb_api-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2190 2023-03-14 10:59:24.000000 nbb_api-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:58:23.121726 nbb_api-0.1.9/nbb_api.egg-info/
+-rw-rw-rw-   0        0        0     3066 2024-05-04 19:58:23.000000 nbb_api-0.1.9/nbb_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-05-04 19:58:23.000000 nbb_api-0.1.9/nbb_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:58:23.000000 nbb_api-0.1.9/nbb_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-04 19:58:23.000000 nbb_api-0.1.9/nbb_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:58:23.000000 nbb_api-0.1.9/nbb_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:58:23.122723 nbb_api-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-04 19:55:04.000000 nbb_api-0.1.9/setup.py
```

### Comparing `nbb_api-0.1.8/LICENSE` & `nbb_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nbb_api-0.1.8/PKG-INFO` & `nbb_api-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbb_api
-Version: 0.1.8
+Version: 0.1.9
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
-Metadata-Version: 2.1 Name: nbb_api Version: 0.1.8 Summary: Python package for
+Metadata-Version: 2.1 Name: nbb_api Version: 0.1.9 Summary: Python package for
 easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro
 and LDB Home-page: https://github.com/GabrielPastorello/nbb_api Author: Gabriel
 Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international
 basketball,brazil,ldb,liga-ouro Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
```

### Comparing `nbb_api-0.1.8/README.md` & `nbb_api-0.1.9/README.md`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 | --- | ------------- | --------------- | -- | ----- | ----- | ------- | ----- | ---- | ------ | --------- |
 | 0   | McClanahan    | Fortaleza B. C. | 27 | 34.11 | 20.89 | 6.11    | 10.89 | 3.89 | 22     | 2022-23   |
 | 1   | Antonio       | UNIFACISA       | 26 | 31.74 | 17.96 | 6.00    | 8.85  | 3.12 | 11     | 2022-23   |
 | 2   | Thomas        | Corinthians     | 27 | 32.13 | 17.67 | 5.44    | 8.15  | 4.07 | 0      | 2022-23   |
 | 3   | Lucas Mariano | Sesi Franca     | 22 | 27.41 | 17.59 | 7.23    | 7.64  | 2.73 | 28     | 2022-23   |
 | 4   | Lucas Dias    | Sesi Franca     | 20 | 30.65 | 17.50 | 5.85    | 8.60  | 3.05 | 9      | 2022-23   |
 
-Use it wisely!
+Use it wisely!
```

### Comparing `nbb_api-0.1.8/nbb_api.egg-info/PKG-INFO` & `nbb_api-0.1.9/nbb_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbb_api
-Version: 0.1.8
+Version: 0.1.9
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
-Metadata-Version: 2.1 Name: nbb_api Version: 0.1.8 Summary: Python package for
+Metadata-Version: 2.1 Name: nbb_api Version: 0.1.9 Summary: Python package for
 easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro
 and LDB Home-page: https://github.com/GabrielPastorello/nbb_api Author: Gabriel
 Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international
 basketball,brazil,ldb,liga-ouro Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
```

### Comparing `nbb_api-0.1.8/setup.py` & `nbb_api-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
             name='nbb_api',
-            version='0.1.8',
+            version='0.1.9',
             description='Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB',
             long_description=long_description,
             long_description_content_type="text/markdown",
             url='https://github.com/GabrielPastorello/nbb_api',
             author='Gabriel Speranza Pastorello',
             author_email='gabriel.pastorello01@gmail.com',
             license='MIT',
```

