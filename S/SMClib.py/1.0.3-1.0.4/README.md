# Comparing `tmp/SMClib.py-1.0.3.tar.gz` & `tmp/SMClib.py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SMClib.py-1.0.3.tar", last modified: Fri May  3 23:23:07 2024, max compression
+gzip compressed data, was "dist\SMClib.py-1.0.4.tar", last modified: Sat May  4 00:02:40 2024, max compression
```

## Comparing `SMClib.py-1.0.3.tar` & `SMClib.py-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/
--rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      624 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMCLIB/
--rw-rw-rw-   0        0        0       40 2024-05-03 23:11:57.000000 SMClib.py-1.0.3/SMCLIB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/
--rw-rw-rw-   0        0        0      624 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/SMClib.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 23:23:07.000000 SMClib.py-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      679 2024-05-03 23:22:53.000000 SMClib.py-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/
+-rw-rw-rw-   0        0        0     1056 2024-05-03 22:53:35.000000 SMClib.py-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      624 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       96 2024-05-03 23:22:15.000000 SMClib.py-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMCLIB/
+-rw-rw-rw-   0        0        0       42 2024-05-04 00:02:28.000000 SMClib.py-1.0.4/SMCLIB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMClib.py.egg-info/
+-rw-rw-rw-   0        0        0      624 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMClib.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMClib.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMClib.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMClib.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/SMClib.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 00:02:40.000000 SMClib.py-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      691 2024-05-04 00:02:32.000000 SMClib.py-1.0.4/setup.py
```

### Comparing `SMClib.py-1.0.3/LICENSE.txt` & `SMClib.py-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SMClib.py-1.0.3/PKG-INFO` & `SMClib.py-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.3
+Version: 1.0.4
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SMClib.py-1.0.3/SMClib.py.egg-info/PKG-INFO` & `SMClib.py-1.0.4/SMClib.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMClib.py
-Version: 1.0.3
+Version: 1.0.4
 Summary: biblioteka ułatwiająca prace przy discord botach
 Home-page: 
 Author: ESKARABATOS
 Author-email: bartek.torba@interia.pl
 License: MIT
 Keywords: SMC Discord
 Classifier: Development Status :: 5 - Production/Stable
```

