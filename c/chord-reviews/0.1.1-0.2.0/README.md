# Comparing `tmp/chord_reviews-0.1.1.tar.gz` & `tmp/chord_reviews-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chord_reviews-0.1.1.tar", last modified: Sat May  4 14:08:01 2024, max compression
+gzip compressed data, was "chord_reviews-0.2.0.tar", last modified: Sat May  4 14:10:22 2024, max compression
```

## Comparing `chord_reviews-0.1.1.tar` & `chord_reviews-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:08:01.559028 chord_reviews-0.1.1/
--rw-rw-rw-   0        0        0      479 2024-05-04 14:08:01.559028 chord_reviews-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 14:08:01.559028 chord_reviews-0.1.1/chord_reviews.egg-info/
--rw-rw-rw-   0        0        0      479 2024-05-04 14:08:01.000000 chord_reviews-0.1.1/chord_reviews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-04 14:08:01.000000 chord_reviews-0.1.1/chord_reviews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:08:01.000000 chord_reviews-0.1.1/chord_reviews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-05-04 14:08:01.000000 chord_reviews-0.1.1/chord_reviews.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:08:01.000000 chord_reviews-0.1.1/chord_reviews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 14:08:01.559028 chord_reviews-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      578 2024-05-04 14:01:30.000000 chord_reviews-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:10:22.853861 chord_reviews-0.2.0/
+-rw-rw-rw-   0        0        0      479 2024-05-04 14:10:22.852566 chord_reviews-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 14:10:22.847683 chord_reviews-0.2.0/chord_reviews.egg-info/
+-rw-rw-rw-   0        0        0      479 2024-05-04 14:10:22.000000 chord_reviews-0.2.0/chord_reviews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-04 14:10:22.000000 chord_reviews-0.2.0/chord_reviews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:10:22.000000 chord_reviews-0.2.0/chord_reviews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-04 14:10:22.000000 chord_reviews-0.2.0/chord_reviews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:10:22.000000 chord_reviews-0.2.0/chord_reviews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 14:10:22.853861 chord_reviews-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      578 2024-05-04 14:10:07.000000 chord_reviews-0.2.0/setup.py
```

### Comparing `chord_reviews-0.1.1/setup.py` & `chord_reviews-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chord_reviews',
-    version='0.1.1',
+    version='0.2.0',
     description="Process reviews data, apply text preprocessing, and generate a chord plot visualization showing word co-occurrence patterns and sentiment analysis.",
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'nltk',
         'collections',
```

