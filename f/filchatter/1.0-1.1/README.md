# Comparing `tmp/filchatter-1.0.tar.gz` & `tmp/filchatter-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filchatter-1.0.tar", last modified: Sat May  4 05:10:56 2024, max compression
+gzip compressed data, was "filchatter-1.1.tar", last modified: Sat May  4 06:19:45 2024, max compression
```

## Comparing `filchatter-1.0.tar` & `filchatter-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 05:10:56.227146 filchatter-1.0/
--rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.0/LICENSE.md
--rw-rw-rw-   0        0        0      106 2024-05-04 05:10:56.225151 filchatter-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 05:10:56.224154 filchatter-1.0/filchatter.egg-info/
--rw-rw-rw-   0        0        0      106 2024-05-04 05:10:56.000000 filchatter-1.0/filchatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-04 05:10:56.000000 filchatter-1.0/filchatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 05:10:56.000000 filchatter-1.0/filchatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-04 05:10:56.000000 filchatter-1.0/filchatter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 05:10:56.000000 filchatter-1.0/filchatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 05:10:56.000000 filchatter-1.0/filchatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 05:10:56.227146 filchatter-1.0/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-04 05:10:06.000000 filchatter-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:19:45.640353 filchatter-1.1/
+-rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2024-05-04 06:19:45.639356 filchatter-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 06:19:45.637362 filchatter-1.1/filchatter.egg-info/
+-rw-rw-rw-   0        0        0      106 2024-05-04 06:19:45.000000 filchatter-1.1/filchatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-04 06:19:45.000000 filchatter-1.1/filchatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 06:19:45.000000 filchatter-1.1/filchatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-04 06:19:45.000000 filchatter-1.1/filchatter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 06:19:45.000000 filchatter-1.1/filchatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 06:19:45.000000 filchatter-1.1/filchatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 06:19:45.640353 filchatter-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-04 06:16:44.000000 filchatter-1.1/setup.py
```

### Comparing `filchatter-1.0/LICENSE.md` & `filchatter-1.1/LICENSE.md`

 * *Files identical despite different names*

