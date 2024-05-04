# Comparing `tmp/nbb_api-0.1.5.tar.gz` & `tmp/nbb_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbb_api-0.1.5.tar", last modified: Sun Aug 27 20:19:28 2023, max compression
+gzip compressed data, was "nbb_api-0.1.6.tar", last modified: Sat May  4 19:20:40 2024, max compression
```

## Comparing `nbb_api-0.1.5.tar` & `nbb_api-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-27 20:19:28.980401 nbb_api-0.1.5/
--rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 nbb_api-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2910 2023-08-27 20:19:28.979375 nbb_api-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2190 2023-03-14 10:59:24.000000 nbb_api-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-27 20:19:28.920754 nbb_api-0.1.5/nbb_api/
--rw-rw-rw-   0        0        0        0 2023-03-12 19:02:10.000000 nbb_api-0.1.5/nbb_api/__init__.py
--rw-rw-rw-   0        0        0     2822 2023-03-12 19:02:10.000000 nbb_api-0.1.5/nbb_api/ldb.py
--rw-rw-rw-   0        0        0     2934 2023-03-12 19:02:10.000000 nbb_api-0.1.5/nbb_api/liga_ouro.py
--rw-rw-rw-   0        0        0     5487 2023-03-12 19:02:10.000000 nbb_api-0.1.5/nbb_api/nbb.py
-drwxrwxrwx   0        0        0        0 2023-08-27 20:19:28.976158 nbb_api-0.1.5/nbb_api.egg-info/
--rw-rw-rw-   0        0        0     2910 2023-08-27 20:19:28.000000 nbb_api-0.1.5/nbb_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-08-27 20:19:28.000000 nbb_api-0.1.5/nbb_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-27 20:19:28.000000 nbb_api-0.1.5/nbb_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-27 20:19:28.000000 nbb_api-0.1.5/nbb_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-27 20:19:28.000000 nbb_api-0.1.5/nbb_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-27 20:19:28.981392 nbb_api-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1354 2023-08-27 20:18:01.000000 nbb_api-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:20:40.249381 nbb_api-0.1.6/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 19:18:00.000000 nbb_api-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3066 2024-05-04 19:20:40.249381 nbb_api-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2024-05-04 19:20:35.000000 nbb_api-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:20:40.248382 nbb_api-0.1.6/nbb_api.egg-info/
+-rw-rw-rw-   0        0        0     3066 2024-05-04 19:20:40.000000 nbb_api-0.1.6/nbb_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-05-04 19:20:40.000000 nbb_api-0.1.6/nbb_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:20:40.000000 nbb_api-0.1.6/nbb_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-04 19:20:40.000000 nbb_api-0.1.6/nbb_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:20:40.000000 nbb_api-0.1.6/nbb_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:20:40.249381 nbb_api-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-04 19:19:12.000000 nbb_api-0.1.6/setup.py
```

### Comparing `nbb_api-0.1.5/LICENSE` & `nbb_api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nbb_api-0.1.5/PKG-INFO` & `nbb_api-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,54 @@
-Metadata-Version: 2.1
-Name: nbb_api
-Version: 0.1.5
-Summary: Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB
-Home-page: https://github.com/GabrielPastorello/nbb_api
-Author: Gabriel Speranza Pastorello
-Author-email: gabriel.pastorello01@gmail.com
-License: MIT
-Keywords: nbb,novo basquete brasil,scraper,basketball,international basketball,brazil,ldb,liga-ouro
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-<img src="https://user-images.githubusercontent.com/57769272/224566374-c8c748c7-c663-489f-8b98-d7041ab4092a.png" width="150">
-</p>
-<p align="center">
-    <a href="https://pypi.org/project/nbb-api/">
-        <img src="https://img.shields.io/pypi/v/nbb-api" alt="pypi" />
-    </a>
-    <a href="https://pypi.org/project/nbb-api/">
-        <img src="https://img.shields.io/pypi/pyversions/nbb-api" alt="python version" />
-    </a>
-    <a href="https://pypi.org/project/nbb-api/">
-        <img src="https://img.shields.io/pypi/l/nbb-api" alt="license" />
-    </a>
-</p>
-
-# nbb_api
-
-Python package for easy access to Brazilian basketball data through scraping of [LNB](https://lnb.com.br/) website.
-
-This allows users to obtain statistics, standings, and scores for various seasons and phases of the following tournaments:
-- **NBB** (Novo Basquete Brasil)
-- **LDB** (Liga de Desenvolvimento de Basquete)
-- **Liga Ouro**
-
-## Installing
-### Via `pip`
-This library was written as an exercise for creating my first PyPi package. Hopefully you will find it valuable!
-Install with the following command:
-
-```
-pip install nbb-api
-```
-
-## Documentation
-For documentation about the API methods refer to [the documentation](https://github.com/GabrielPastorello/nbb_api/blob/main/API.md).
-
-## Example of use
-```
-from nbb_api import nbb
-```
-
-```
-nbb.get_stats('2022-23','regular','cestinhas').head()
-```
-Output:
-|     | Jogador       | Equipe          | JO | Min   | Pts   | 3P      | 2P    | LL   | Camisa | Temporada |
-| --- | ------------- | --------------- | -- | ----- | ----- | ------- | ----- | ---- | ------ | --------- |
-| 0   | McClanahan    | Fortaleza B. C. | 27 | 34.11 | 20.89 | 6.11    | 10.89 | 3.89 | 22     | 2022-23   |
-| 1   | Antonio       | UNIFACISA       | 26 | 31.74 | 17.96 | 6.00    | 8.85  | 3.12 | 11     | 2022-23   |
-| 2   | Thomas        | Corinthians     | 27 | 32.13 | 17.67 | 5.44    | 8.15  | 4.07 | 0      | 2022-23   |
-| 3   | Lucas Mariano | Sesi Franca     | 22 | 27.41 | 17.59 | 7.23    | 7.64  | 2.73 | 28     | 2022-23   |
-| 4   | Lucas Dias    | Sesi Franca     | 20 | 30.65 | 17.50 | 5.85    | 8.60  | 3.05 | 9      | 2022-23   |
-
-Use it wisely!
+<p align="center">
+<img src="https://user-images.githubusercontent.com/57769272/224566374-c8c748c7-c663-489f-8b98-d7041ab4092a.png" width="150">
+</p>
+<p align="center">
+    <a href="https://pypi.org/project/nbb-api/">
+        <img src="https://img.shields.io/pypi/v/nbb-api" alt="pypi" />
+    </a>
+    <a href="https://pypi.org/project/nbb-api/">
+        <img src="https://img.shields.io/pypi/pyversions/nbb-api" alt="python version" />
+    </a>
+    <a href="https://pypi.org/project/nbb-api/">
+        <img src="https://img.shields.io/pypi/l/nbb-api" alt="license" />
+    </a>
+</p>
+
+# nbb_api
+
+Python package for easy access to Brazilian basketball data through scraping of [LNB](https://lnb.com.br/) website.
+
+This allows users to obtain statistics, standings, and scores for various seasons and phases of the following tournaments:
+- **NBB** (Novo Basquete Brasil)
+- **LDB** (Liga de Desenvolvimento de Basquete)
+- **Liga Ouro**
+
+## Installing
+### Via `pip`
+This library was written as an exercise for creating my first PyPi package. Hopefully you will find it valuable!
+Install with the following command:
+
+```
+pip install nbb-api
+```
+
+## Documentation
+For documentation about the API methods refer to [the documentation](https://github.com/GabrielPastorello/nbb_api/blob/main/API.md).
+
+## Example of use
+```
+from nbb_api import nbb
+```
+
+```
+nbb.get_stats('2022-23','regular','cestinhas').head()
+```
+Output:
+|     | Jogador       | Equipe          | JO | Min   | Pts   | 3P      | 2P    | LL   | Camisa | Temporada |
+| --- | ------------- | --------------- | -- | ----- | ----- | ------- | ----- | ---- | ------ | --------- |
+| 0   | McClanahan    | Fortaleza B. C. | 27 | 34.11 | 20.89 | 6.11    | 10.89 | 3.89 | 22     | 2022-23   |
+| 1   | Antonio       | UNIFACISA       | 26 | 31.74 | 17.96 | 6.00    | 8.85  | 3.12 | 11     | 2022-23   |
+| 2   | Thomas        | Corinthians     | 27 | 32.13 | 17.67 | 5.44    | 8.15  | 4.07 | 0      | 2022-23   |
+| 3   | Lucas Mariano | Sesi Franca     | 22 | 27.41 | 17.59 | 7.23    | 7.64  | 2.73 | 28     | 2022-23   |
+| 4   | Lucas Dias    | Sesi Franca     | 20 | 30.65 | 17.50 | 5.85    | 8.60  | 3.05 | 9      | 2022-23   |
+
+Use it wisely!
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: nbb_api Version: 0.1.5 Summary: Python package for
-easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro
-and LDB Home-page: https://github.com/GabrielPastorello/nbb_api Author: Gabriel
-Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT
-Keywords: nbb,novo basquete brasil,scraper,basketball,international
-basketball,brazil,ldb,liga-ouro Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE
  [https://user-images.githubusercontent.com/57769272/224566374-c8c748c7-c663-
                           489f-8b98-d7041ab4092a.png]
                         _[_p_y_p_i_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]
 # nbb_api Python package for easy access to Brazilian basketball data through
 scraping of [LNB](https://lnb.com.br/) website. This allows users to obtain
 statistics, standings, and scores for various seasons and phases of the
 following tournaments: - **NBB** (Novo Basquete Brasil) - **LDB** (Liga de
```

### Comparing `nbb_api-0.1.5/nbb_api.egg-info/PKG-INFO` & `nbb_api-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
-Name: nbb-api
-Version: 0.1.5
+Name: nbb_api
+Version: 0.1.6
 Summary: Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB
 Home-page: https://github.com/GabrielPastorello/nbb_api
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international basketball,brazil,ldb,liga-ouro
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.5.3
+Requires-Dist: numpy>=1.24.1
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: pytz>=2022.7
+Requires-Dist: lxml>=4.9.2
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/57769272/224566374-c8c748c7-c663-489f-8b98-d7041ab4092a.png" width="150">
 </p>
 <p align="center">
     <a href="https://pypi.org/project/nbb-api/">
         <img src="https://img.shields.io/pypi/v/nbb-api" alt="pypi" />
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 2.1 Name: nbb-api Version: 0.1.5 Summary: Python package for
+Metadata-Version: 2.1 Name: nbb_api Version: 0.1.6 Summary: Python package for
 easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro
 and LDB Home-page: https://github.com/GabrielPastorello/nbb_api Author: Gabriel
 Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com License: MIT
 Keywords: nbb,novo basquete brasil,scraper,basketball,international
 basketball,brazil,ldb,liga-ouro Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE
+markdown License-File: LICENSE Requires-Dist: pandas>=1.5.3 Requires-Dist:
+numpy>=1.24.1 Requires-Dist: python-dateutil>=2.8.2 Requires-Dist: pytz>=2022.7
+Requires-Dist: lxml>=4.9.2
  [https://user-images.githubusercontent.com/57769272/224566374-c8c748c7-c663-
                           489f-8b98-d7041ab4092a.png]
                         _[_p_y_p_i_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]
 # nbb_api Python package for easy access to Brazilian basketball data through
 scraping of [LNB](https://lnb.com.br/) website. This allows users to obtain
 statistics, standings, and scores for various seasons and phases of the
 following tournaments: - **NBB** (Novo Basquete Brasil) - **LDB** (Liga de
```

### Comparing `nbb_api-0.1.5/setup.py` & `nbb_api-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
             name='nbb_api',
-            version='0.1.5',
+            version='0.1.6',
             description='Python package for easy access to Brazilian basketball data: NBB (Novo Basquete Brasil), Liga Ouro and LDB',
             long_description=long_description,
             long_description_content_type="text/markdown",
             url='https://github.com/GabrielPastorello/nbb_api',
             author='Gabriel Speranza Pastorello',
             author_email='gabriel.pastorello01@gmail.com',
             license='MIT',
```

