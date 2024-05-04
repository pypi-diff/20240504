# Comparing `tmp/SMClib.py-1.0.5.tar.gz` & `tmp/SMClib.py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SMClib.py-1.0.5.tar", last modified: Sat May  4 09:07:22 2024, max compression
+gzip compressed data, was "dist\SMClib.py-1.0.6.tar", last modified: Sat May  4 09:12:40 2024, max compression
```

## Comparing `SMClib.py-1.0.5.tar` & `SMClib.py-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/
--rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      624 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMCLIB/
--rw-rw-rw-   0        0        0       44 2024-05-04 09:06:41.000000 SMClib.py-1.0.5/SMCLIB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMClib.py.egg-info/
--rw-rw-rw-   0        0        0      624 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMClib.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMClib.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMClib.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMClib.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/SMClib.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 09:07:22.000000 SMClib.py-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      691 2024-05-04 09:06:54.000000 SMClib.py-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/
+-rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      624 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMCLIB/
+-rw-rw-rw-   0        0        0       73 2024-05-04 09:12:15.000000 SMClib.py-1.0.6/SMCLIB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMClib.py.egg-info/
+-rw-rw-rw-   0        0        0      624 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMClib.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMClib.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMClib.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMClib.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/SMClib.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 09:12:40.000000 SMClib.py-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      691 2024-05-04 09:12:31.000000 SMClib.py-1.0.6/setup.py
```

### Comparing `SMClib.py-1.0.5/LICENSE.txt` & `SMClib.py-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SMClib.py-1.0.5/PKG-INFO` & `SMClib.py-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.5
+Version: 1.0.6
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SMClib.py-1.0.5/SMClib.py.egg-info/PKG-INFO` & `SMClib.py-1.0.6/SMClib.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.5
+Version: 1.0.6
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SMClib.py-1.0.5/setup.py` & `SMClib.py-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SMClib.py',
-  version='1.0.5',
+  version='1.0.6',
   description='biblioteka ułatwiająca prace przy discord botach',
   long_description=open('README.rst').read(),
   url='',  
   author='ESKARABATOS',
   author_email='bartek.torba@interia.pl',
   license='MIT', 
   classifiers=classifiers,
```

