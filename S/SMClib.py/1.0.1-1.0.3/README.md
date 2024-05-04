# Comparing `tmp/SMClib.py-1.0.1.tar.gz` & `tmp/SMClib.py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SMClib.py-1.0.1.tar", last modified: Fri May  3 23:19:26 2024, max compression
+gzip compressed data, was "dist\SMClib.py-1.0.3.tar", last modified: Fri May  3 23:23:07 2024, max compression
```

## Comparing `SMClib.py-1.0.1.tar` & `SMClib.py-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/
--rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      567 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-05-03 23:19:02.000000 SMClib.py-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMCLIB/
--rw-rw-rw-   0        0        0       40 2024-05-03 23:11:57.000000 SMClib.py-1.0.1/SMCLIB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/
--rw-rw-rw-   0        0        0      567 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      679 2024-05-03 23:19:04.000000 SMClib.py-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/
+-rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      624 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMCLIB/
+-rw-rw-rw-   0        0        0       40 2024-05-03 23:11:57.000000 SMClib.py-1.0.3/SMCLIB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/
+-rw-rw-rw-   0        0        0      624 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      679 2024-05-03 23:22:53.000000 SMClib.py-1.0.3/setup.py
```

### Comparing `SMClib.py-1.0.1/LICENSE.txt` & `SMClib.py-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SMClib.py-1.0.1/setup.py` & `SMClib.py-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SMClib.py',
-  version='1.0.1',
+  version='1.0.3',
   description='biblioteka ułatwiająca prace przy discord botach',
   long_description=open('README.rst').read(),
   url='',  
   author='ESKARABATOS',
   author_email='bartek.torba@interia.pl',
   license='MIT', 
   classifiers=classifiers,
```

