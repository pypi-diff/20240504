# Comparing `tmp/finlearn-0.0.42.tar.gz` & `tmp/finlearn-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlearn-0.0.42.tar", last modified: Mon Mar 18 22:55:05 2024, max compression
+gzip compressed data, was "finlearn-0.0.43.tar", last modified: Sat May  4 21:06:07 2024, max compression
```

## Comparing `finlearn-0.0.42.tar` & `finlearn-0.0.43.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 22:55:05.636299 finlearn-0.0.42/
--rw-rw-rw-   0        0        0      763 2024-03-18 22:55:05.633072 finlearn-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0      380 2024-03-18 21:40:00.000000 finlearn-0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 22:55:05.609029 finlearn-0.0.42/finlearn/
--rw-rw-rw-   0        0        0       28 2024-03-18 20:53:50.000000 finlearn-0.0.42/finlearn/__init__.py
--rw-rw-rw-   0        0        0     3622 2024-03-18 20:49:35.000000 finlearn-0.0.42/finlearn/plotter.py
-drwxrwxrwx   0        0        0        0 2024-03-18 22:55:05.629698 finlearn-0.0.42/finlearn.egg-info/
--rw-rw-rw-   0        0        0      763 2024-03-18 22:55:05.000000 finlearn-0.0.42/finlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-03-18 22:55:05.000000 finlearn-0.0.42/finlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 22:55:05.000000 finlearn-0.0.42/finlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-18 22:55:05.000000 finlearn-0.0.42/finlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-18 22:55:05.000000 finlearn-0.0.42/finlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 22:55:05.636299 finlearn-0.0.42/setup.cfg
--rw-rw-rw-   0        0        0     1131 2024-03-18 22:55:00.000000 finlearn-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:06:07.191288 finlearn-0.0.43/
+-rw-rw-rw-   0        0        0      855 2024-05-04 21:06:07.183273 finlearn-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-05-04 21:04:29.000000 finlearn-0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 21:06:07.124767 finlearn-0.0.43/finlearn/
+-rw-rw-rw-   0        0        0       28 2024-03-18 20:53:50.000000 finlearn-0.0.43/finlearn/__init__.py
+-rw-rw-rw-   0        0        0     5725 2024-05-04 21:01:29.000000 finlearn-0.0.43/finlearn/plotter.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:06:07.175126 finlearn-0.0.43/finlearn.egg-info/
+-rw-rw-rw-   0        0        0      855 2024-05-04 21:06:06.000000 finlearn-0.0.43/finlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-04 21:06:06.000000 finlearn-0.0.43/finlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 21:06:06.000000 finlearn-0.0.43/finlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-04 21:06:06.000000 finlearn-0.0.43/finlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 21:06:06.000000 finlearn-0.0.43/finlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 21:06:07.191288 finlearn-0.0.43/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2024-05-04 21:05:37.000000 finlearn-0.0.43/setup.py
```

### Comparing `finlearn-0.0.42/setup.py` & `finlearn-0.0.43/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'finlearn'
 DESCRIPTION = 'A one-stop package for entire financial analysis and market prediction using Deep Learning'
-VERSION = '0.0.42'
+VERSION = '0.0.43'
 AUTHOR = 'Ankit Dutta'
 AUTHOR_EMAIL = 'ankitduttaiitkgp@gmail.com'
 #URL = 'https://github.com/your_username/your_repository'
 LICENSE = 'Apache 2.0'
 
 # Read long description from README file
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 # Define dependencies
 INSTALL_REQUIRES = [
     'plotly',
     'yfinance',
+    'matplotlib'
     # Add more dependencies as needed
 ]
 
 # Define additional classifiers
 CLASSIFIERS = [
     'Programming Language :: Python :: 3',
     # Add more classifiers as needed
```

