# Comparing `tmp/SMClib.py-1.0.0.tar.gz` & `tmp/SMClib.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SMClib.py-1.0.0.tar", last modified: Fri May  3 22:58:28 2024, max compression
+gzip compressed data, was "dist\SMClib.py-1.0.1.tar", last modified: Fri May  3 23:19:26 2024, max compression
```

## Comparing `SMClib.py-1.0.0.tar` & `SMClib.py-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/
--rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      524 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/SMCLIB/
--rw-rw-rw-   0        0        0      181 2024-05-03 22:44:35.000000 SMClib.py-1.0.0/SMCLIB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/SMClib.py.egg-info/
--rw-rw-rw-   0        0        0      524 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/SMClib.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/SMClib.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/SMClib.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/SMClib.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:58:28.000000 SMClib.py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      679 2024-05-03 22:58:26.000000 SMClib.py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/
+-rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      567 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-05-03 23:19:02.000000 SMClib.py-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMCLIB/
+-rw-rw-rw-   0        0        0       40 2024-05-03 23:11:57.000000 SMClib.py-1.0.1/SMCLIB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/
+-rw-rw-rw-   0        0        0      567 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/SMClib.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:19:26.000000 SMClib.py-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      679 2024-05-03 23:19:04.000000 SMClib.py-1.0.1/setup.py
```

### Comparing `SMClib.py-1.0.0/LICENSE.txt` & `SMClib.py-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SMClib.py-1.0.0/PKG-INFO` & `SMClib.py-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
+
+# Windows
+pip install SMClib.py==1.0.1
```

### Comparing `SMClib.py-1.0.0/SMClib.py.egg-info/PKG-INFO` & `SMClib.py-1.0.1/SMClib.py.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
+
+# Windows
+pip install SMClib.py==1.0.1
```

### Comparing `SMClib.py-1.0.0/setup.py` & `SMClib.py-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SMClib.py',
-  version='1.0.0',
+  version='1.0.1',
   description='biblioteka ułatwiająca prace przy discord botach',
   long_description=open('README.rst').read(),
   url='',  
   author='ESKARABATOS',
   author_email='bartek.torba@interia.pl',
   license='MIT', 
   classifiers=classifiers,
```

