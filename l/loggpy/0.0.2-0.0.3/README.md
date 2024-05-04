# Comparing `tmp/loggpy-0.0.2.tar.gz` & `tmp/loggpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggpy-0.0.2.tar", last modified: Fri May  3 22:35:53 2024, max compression
+gzip compressed data, was "loggpy-0.0.3.tar", last modified: Sat May  4 03:56:51 2024, max compression
```

## Comparing `loggpy-0.0.2.tar` & `loggpy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:35:53.565802 loggpy-0.0.2/
--rw-rw-rw-   0        0        0     1067 2024-05-03 22:34:14.000000 loggpy-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      266 2024-05-03 22:35:53.564787 loggpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-03 22:34:31.000000 loggpy-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-03 22:35:53.544798 loggpy-0.0.2/loggpy/
--rw-rw-rw-   0        0        0      118 2024-05-03 22:29:43.000000 loggpy-0.0.2/loggpy/__init__.py
--rw-rw-rw-   0        0        0     4325 2024-05-03 22:33:59.000000 loggpy-0.0.2/loggpy/core.py
--rw-rw-rw-   0        0        0     1480 2024-05-03 22:29:43.000000 loggpy-0.0.2/loggpy/defaults.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:35:53.563789 loggpy-0.0.2/loggpy.egg-info/
--rw-rw-rw-   0        0        0      266 2024-05-03 22:35:53.000000 loggpy-0.0.2/loggpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-03 22:35:53.000000 loggpy-0.0.2/loggpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:35:53.000000 loggpy-0.0.2/loggpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 22:35:53.000000 loggpy-0.0.2/loggpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:35:53.565802 loggpy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      463 2024-05-03 22:35:30.000000 loggpy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 03:56:51.002973 loggpy-0.0.3/
+-rw-rw-rw-   0        0        0     1067 2024-05-03 22:34:14.000000 loggpy-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      266 2024-05-04 03:56:51.002973 loggpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-03 22:34:31.000000 loggpy-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 03:56:50.983984 loggpy-0.0.3/loggpy/
+-rw-rw-rw-   0        0        0     5337 2024-05-04 03:55:47.000000 loggpy-0.0.3/loggpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 03:56:51.001973 loggpy-0.0.3/loggpy.egg-info/
+-rw-rw-rw-   0        0        0      266 2024-05-04 03:56:50.000000 loggpy-0.0.3/loggpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-05-04 03:56:50.000000 loggpy-0.0.3/loggpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 03:56:50.000000 loggpy-0.0.3/loggpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 03:56:50.000000 loggpy-0.0.3/loggpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 03:56:51.007970 loggpy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      463 2024-05-03 22:35:30.000000 loggpy-0.0.3/setup.py
```

### Comparing `loggpy-0.0.2/LICENSE.txt` & `loggpy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

