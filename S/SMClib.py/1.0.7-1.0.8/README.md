# Comparing `tmp/SMClib.py-1.0.7.tar.gz` & `tmp/SMClib.py-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SMClib.py-1.0.7.tar", last modified: Sat May  4 09:18:45 2024, max compression
+gzip compressed data, was "dist\SMClib.py-1.0.8.tar", last modified: Sat May  4 09:23:35 2024, max compression
```

## Comparing `SMClib.py-1.0.7.tar` & `SMClib.py-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/
--rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      624 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMCLIB/
--rw-rw-rw-   0        0        0       48 2024-05-04 09:18:31.000000 SMClib.py-1.0.7/SMCLIB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMClib.py.egg-info/
--rw-rw-rw-   0        0        0      624 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMClib.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMClib.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMClib.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMClib.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/SMClib.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 09:18:45.000000 SMClib.py-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      691 2024-05-04 09:18:39.000000 SMClib.py-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/
+-rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      624 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMCLIB/
+-rw-rw-rw-   0        0        0       87 2024-05-04 09:23:25.000000 SMClib.py-1.0.8/SMCLIB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMClib.py.egg-info/
+-rw-rw-rw-   0        0        0      624 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMClib.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMClib.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMClib.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMClib.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/SMClib.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 09:23:35.000000 SMClib.py-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      691 2024-05-04 09:23:30.000000 SMClib.py-1.0.8/setup.py
```

### Comparing `SMClib.py-1.0.7/LICENSE.txt` & `SMClib.py-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SMClib.py-1.0.7/PKG-INFO` & `SMClib.py-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.7
+Version: 1.0.8
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SMClib.py-1.0.7/SMClib.py.egg-info/PKG-INFO` & `SMClib.py-1.0.8/SMClib.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.7
+Version: 1.0.8
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SMClib.py-1.0.7/setup.py` & `SMClib.py-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SMClib.py',
-  version='1.0.7',
+  version='1.0.8',
   description='biblioteka ułatwiająca prace przy discord botach',
   long_description=open('README.rst').read(),
   url='',  
   author='ESKARABATOS',
   author_email='bartek.torba@interia.pl',
   license='MIT', 
   classifiers=classifiers,
```

