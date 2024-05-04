# Comparing `tmp/graph_judge-0.0.5.tar.gz` & `tmp/graph_judge-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_judge-0.0.5.tar", last modified: Thu May  2 20:50:55 2024, max compression
+gzip compressed data, was "graph_judge-0.0.6.tar", last modified: Sat May  4 05:06:38 2024, max compression
```

## Comparing `graph_judge-0.0.5.tar` & `graph_judge-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:50:55.388730 graph_judge-0.0.5/
--rw-rw-rw-   0        0        0    35823 2024-05-02 20:48:29.000000 graph_judge-0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0      256 2024-05-02 20:50:55.388730 graph_judge-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-05-02 20:50:54.000000 graph_judge-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 20:50:55.385060 graph_judge-0.0.5/graph_judge/
--rw-rw-rw-   0        0        0       24 2024-05-02 20:49:38.000000 graph_judge-0.0.5/graph_judge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:50:55.387723 graph_judge-0.0.5/graph_judge.egg-info/
--rw-rw-rw-   0        0        0      256 2024-05-02 20:50:55.000000 graph_judge-0.0.5/graph_judge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-02 20:50:55.000000 graph_judge-0.0.5/graph_judge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:50:55.000000 graph_judge-0.0.5/graph_judge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-02 20:50:55.000000 graph_judge-0.0.5/graph_judge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:50:55.390074 graph_judge-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-05-02 20:50:05.000000 graph_judge-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:06:38.652583 graph_judge-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2024-05-04 00:53:17.000000 graph_judge-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0      256 2024-05-04 05:06:38.651548 graph_judge-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-05-04 00:53:17.000000 graph_judge-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 05:06:38.642551 graph_judge-0.0.6/graph_judge/
+-rw-rw-rw-   0        0        0     4092 2024-05-04 04:57:33.000000 graph_judge-0.0.6/graph_judge/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-05-04 04:42:45.000000 graph_judge-0.0.6/graph_judge/result.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:06:38.649548 graph_judge-0.0.6/graph_judge.egg-info/
+-rw-rw-rw-   0        0        0      256 2024-05-04 05:06:38.000000 graph_judge-0.0.6/graph_judge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-04 05:06:38.000000 graph_judge-0.0.6/graph_judge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 05:06:38.000000 graph_judge-0.0.6/graph_judge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-04 05:06:38.000000 graph_judge-0.0.6/graph_judge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 05:06:38.653549 graph_judge-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-05-04 05:06:36.000000 graph_judge-0.0.6/setup.py
```

### Comparing `graph_judge-0.0.5/LICENSE.md` & `graph_judge-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `graph_judge-0.0.5/setup.py` & `graph_judge-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

