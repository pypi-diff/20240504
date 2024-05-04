# Comparing `tmp/djsce-0.1.7.tar.gz` & `tmp/djsce-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsce-0.1.7.tar", last modified: Sun Dec 17 11:26:03 2023, max compression
+gzip compressed data, was "djsce-0.1.8.tar", last modified: Sat May  4 12:41:42 2024, max compression
```

## Comparing `djsce-0.1.7.tar` & `djsce-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-12-17 11:26:03.923741 djsce-0.1.7/
--rw-rw-rw-   0        0        0     1095 2023-12-11 07:22:54.000000 djsce-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      507 2023-12-17 11:26:03.923741 djsce-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-12-11 08:13:47.000000 djsce-0.1.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-12-17 11:26:03.894100 djsce-0.1.7/djsce/
--rw-rw-rw-   0        0        0       79 2023-12-17 11:25:38.000000 djsce-0.1.7/djsce/__init__.py
--rw-rw-rw-   0        0        0    18825 2023-12-17 11:25:22.000000 djsce-0.1.7/djsce/ai.py
--rw-rw-rw-   0        0        0     2533 2023-12-15 15:54:03.000000 djsce-0.1.7/djsce/de.py
--rw-rw-rw-   0        0        0    78867 2023-12-14 11:23:53.000000 djsce-0.1.7/djsce/dsa.py
--rw-rw-rw-   0        0        0     9690 2023-12-14 13:15:39.000000 djsce-0.1.7/djsce/python.py
-drwxrwxrwx   0        0        0        0 2023-12-17 11:26:03.921836 djsce-0.1.7/djsce.egg-info/
--rw-rw-rw-   0        0        0      507 2023-12-17 11:26:03.000000 djsce-0.1.7/djsce.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-12-17 11:26:03.000000 djsce-0.1.7/djsce.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-17 11:26:03.000000 djsce-0.1.7/djsce.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-12-17 11:26:03.000000 djsce-0.1.7/djsce.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-17 11:26:03.923741 djsce-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-12-17 11:25:44.000000 djsce-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:41:42.364551 djsce-0.1.8/
+-rw-rw-rw-   0        0        0     1095 2023-12-11 07:22:54.000000 djsce-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      537 2024-05-04 12:41:42.364551 djsce-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-12-11 08:13:47.000000 djsce-0.1.8/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 12:41:42.332251 djsce-0.1.8/djsce/
+-rw-rw-rw-   0        0        0      138 2024-05-04 12:39:01.000000 djsce-0.1.8/djsce/__init__.py
+-rw-rw-rw-   0        0        0    18825 2024-05-04 12:39:25.000000 djsce-0.1.8/djsce/ai.py
+-rw-rw-rw-   0        0        0    33347 2024-05-04 12:39:28.000000 djsce-0.1.8/djsce/daa.py
+-rw-rw-rw-   0        0        0     2533 2024-05-04 12:39:32.000000 djsce-0.1.8/djsce/de.py
+-rw-rw-rw-   0        0        0    78867 2023-12-14 11:23:53.000000 djsce-0.1.8/djsce/dsa.py
+-rw-rw-rw-   0        0        0    34344 2024-05-04 12:21:50.000000 djsce-0.1.8/djsce/os.py
+-rw-rw-rw-   0        0        0    25202 2024-05-04 12:38:44.000000 djsce-0.1.8/djsce/poa.py
+-rw-rw-rw-   0        0        0     9690 2023-12-14 13:15:39.000000 djsce-0.1.8/djsce/python.py
+drwxrwxrwx   0        0        0        0 2024-05-04 12:41:42.364551 djsce-0.1.8/djsce.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-05-04 12:41:42.000000 djsce-0.1.8/djsce.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-04 12:41:42.000000 djsce-0.1.8/djsce.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 12:41:42.000000 djsce-0.1.8/djsce.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 12:41:42.000000 djsce-0.1.8/djsce.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 12:41:42.364551 djsce-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      648 2024-05-04 12:12:26.000000 djsce-0.1.8/setup.py
```

### Comparing `djsce-0.1.7/LICENSE` & `djsce-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `djsce-0.1.7/djsce/ai.py` & `djsce-0.1.8/djsce/ai.py`

 * *Files identical despite different names*

### Comparing `djsce-0.1.7/djsce/de.py` & `djsce-0.1.8/djsce/de.py`

 * *Files identical despite different names*

### Comparing `djsce-0.1.7/djsce/dsa.py` & `djsce-0.1.8/djsce/dsa.py`

 * *Files identical despite different names*

### Comparing `djsce-0.1.7/djsce/python.py` & `djsce-0.1.8/djsce/python.py`

 * *Files identical despite different names*

### Comparing `djsce-0.1.7/setup.py` & `djsce-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='djsce',
-  version='0.1.7',
+  version='0.1.8',
   description='DJSCE',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Mihir Panchal',
   author_email='mihirpanchal5400@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

