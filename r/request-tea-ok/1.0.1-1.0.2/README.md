# Comparing `tmp/request_tea_ok-1.0.1.tar.gz` & `tmp/request_tea_ok-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_tea_ok-1.0.1.tar", last modified: Sat May  4 19:34:46 2024, max compression
+gzip compressed data, was "request_tea_ok-1.0.2.tar", last modified: Sat May  4 19:38:12 2024, max compression
```

## Comparing `request_tea_ok-1.0.1.tar` & `request_tea_ok-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 19:34:46.697899 request_tea_ok-1.0.1/
--rw-rw-rw-   0        0        0     1080 2024-05-04 18:57:23.000000 request_tea_ok-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1122 2024-05-04 19:34:46.696899 request_tea_ok-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-05-04 19:34:29.000000 request_tea_ok-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 19:34:46.695902 request_tea_ok-1.0.1/request_tea_ok.egg-info/
--rw-rw-rw-   0        0        0     1122 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 19:34:46.697899 request_tea_ok-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1010 2024-05-04 19:33:32.000000 request_tea_ok-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:38:12.896440 request_tea_ok-1.0.2/
+-rw-rw-rw-   0        0        0     1080 2024-05-04 18:57:23.000000 request_tea_ok-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1078 2024-05-04 19:38:12.895425 request_tea_ok-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2024-05-04 19:37:51.000000 request_tea_ok-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:38:12.893905 request_tea_ok-1.0.2/request_tea_ok.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-05-04 19:38:12.000000 request_tea_ok-1.0.2/request_tea_ok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-04 19:38:12.000000 request_tea_ok-1.0.2/request_tea_ok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:38:12.000000 request_tea_ok-1.0.2/request_tea_ok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-04 19:38:12.000000 request_tea_ok-1.0.2/request_tea_ok.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-04 19:38:12.000000 request_tea_ok-1.0.2/request_tea_ok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-04 19:38:12.000000 request_tea_ok-1.0.2/request_tea_ok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:38:12.896440 request_tea_ok-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2024-05-04 19:38:01.000000 request_tea_ok-1.0.2/setup.py
```

### Comparing `request_tea_ok-1.0.1/LICENSE` & `request_tea_ok-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `request_tea_ok-1.0.1/PKG-INFO` & `request_tea_ok-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-tea-ok
-Version: 1.0.1
+Version: 1.0.2
 Summary: This function is designed to make HTTP requests to the website app.tea.xyz
 Home-page: https://github.com/wahdalo/tea-python
 Author: Wahdalo
 Author-email: ahdx.wtf@gmail.com
 Project-URL: Homepage, https://github.com/wahdalo/tea-python
 Project-URL: Source, https://github.com/wahdalo/tea-python
 Classifier: License :: OSI Approved :: MIT License
@@ -22,8 +22,8 @@
 
 The project utilizes the `requests` library in Python to send HTTP requests. Its purpose is to simplify user interactions with the website and retrieve responses.
         
 ## Installation : `pip install true-random`
         
 ## 📝 License
         
-* Copyright © 2024 https://github.com/nemanjavidika/builder-tea-rep
+* Copyright © 2024 Ahda
```

### Comparing `request_tea_ok-1.0.1/request_tea_ok.egg-info/PKG-INFO` & `request_tea_ok-1.0.2/request_tea_ok.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-tea-ok
-Version: 1.0.1
+Version: 1.0.2
 Summary: This function is designed to make HTTP requests to the website app.tea.xyz
 Home-page: https://github.com/wahdalo/tea-python
 Author: Wahdalo
 Author-email: ahdx.wtf@gmail.com
 Project-URL: Homepage, https://github.com/wahdalo/tea-python
 Project-URL: Source, https://github.com/wahdalo/tea-python
 Classifier: License :: OSI Approved :: MIT License
@@ -22,8 +22,8 @@
 
 The project utilizes the `requests` library in Python to send HTTP requests. Its purpose is to simplify user interactions with the website and retrieve responses.
         
 ## Installation : `pip install true-random`
         
 ## 📝 License
         
-* Copyright © 2024 https://github.com/nemanjavidika/builder-tea-rep
+* Copyright © 2024 Ahda
```

### Comparing `request_tea_ok-1.0.1/setup.py` & `request_tea_ok-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     author='Wahdalo',
     author_email='ahdx.wtf@gmail.com',
     name='request-tea-ok',
-    version='1.0.1',
+    version='1.0.2',
     description='This function is designed to make HTTP requests to the website app.tea.xyz',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wahdalo/tea-python',
     project_urls={
         'Homepage': 'https://github.com/wahdalo/tea-python',
         'Source': 'https://github.com/wahdalo/tea-python',
```

