# Comparing `tmp/request_tea_ok-1.0.0.tar.gz` & `tmp/request_tea_ok-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request_tea_ok-1.0.0.tar", last modified: Sat May  4 19:13:21 2024, max compression
+gzip compressed data, was "request_tea_ok-1.0.1.tar", last modified: Sat May  4 19:34:46 2024, max compression
```

## Comparing `request_tea_ok-1.0.0.tar` & `request_tea_ok-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 19:13:21.009428 request_tea_ok-1.0.0/
--rw-rw-rw-   0        0        0     1080 2024-05-04 18:57:23.000000 request_tea_ok-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      550 2024-05-04 19:13:21.008429 request_tea_ok-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-04 18:56:50.000000 request_tea_ok-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 19:13:21.007432 request_tea_ok-1.0.0/request_tea_ok.egg-info/
--rw-rw-rw-   0        0        0      550 2024-05-04 19:13:20.000000 request_tea_ok-1.0.0/request_tea_ok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-04 19:13:20.000000 request_tea_ok-1.0.0/request_tea_ok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:13:20.000000 request_tea_ok-1.0.0/request_tea_ok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-04 19:13:20.000000 request_tea_ok-1.0.0/request_tea_ok.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-04 19:13:20.000000 request_tea_ok-1.0.0/request_tea_ok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-04 19:13:20.000000 request_tea_ok-1.0.0/request_tea_ok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 19:13:21.009428 request_tea_ok-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-04 19:05:56.000000 request_tea_ok-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:34:46.697899 request_tea_ok-1.0.1/
+-rw-rw-rw-   0        0        0     1080 2024-05-04 18:57:23.000000 request_tea_ok-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1122 2024-05-04 19:34:46.696899 request_tea_ok-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-05-04 19:34:29.000000 request_tea_ok-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:34:46.695902 request_tea_ok-1.0.1/request_tea_ok.egg-info/
+-rw-rw-rw-   0        0        0     1122 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-04 19:34:46.000000 request_tea_ok-1.0.1/request_tea_ok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:34:46.697899 request_tea_ok-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2024-05-04 19:33:32.000000 request_tea_ok-1.0.1/setup.py
```

### Comparing `request_tea_ok-1.0.0/LICENSE` & `request_tea_ok-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `request_tea_ok-1.0.0/setup.py` & `request_tea_ok-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup
 
+with open('README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     author='Wahdalo',
     author_email='ahdx.wtf@gmail.com',
     name='request-tea-ok',
-    version='1.0.0',
+    version='1.0.1',
     description='This function is designed to make HTTP requests to the website app.tea.xyz',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url='https://github.com/wahdalo/tea-python',
     project_urls={
         'Homepage': 'https://github.com/wahdalo/tea-python',
         'Source': 'https://github.com/wahdalo/tea-python',
     },
     py_modules=['request-tea-ok'],
     entry_points={
```

