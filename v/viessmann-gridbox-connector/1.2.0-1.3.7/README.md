# Comparing `tmp/viessmann_gridbox_connector-1.2.0.tar.gz` & `tmp/viessmann_gridbox_connector-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viessmann_gridbox_connector-1.2.0.tar", last modified: Thu Apr 25 11:07:16 2024, max compression
+gzip compressed data, was "viessmann_gridbox_connector-1.3.7.tar", last modified: Sat May  4 10:41:37 2024, max compression
```

## Comparing `viessmann_gridbox_connector-1.2.0.tar` & `viessmann_gridbox_connector-1.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/gridbox_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/gridbox_connector/GridboxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/gridbox_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/gridbox_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 11:07:12.000000 viessmann_gridbox_connector-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:07:16.839453 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 11:07:16.000000 viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:37.862652 viessmann_gridbox_connector-1.3.7/gridbox_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/gridbox_connector/GridboxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/gridbox_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/gridbox_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/top_level.txt
```

### Comparing `viessmann_gridbox_connector-1.2.0/LICENSE` & `viessmann_gridbox_connector-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.2.0/PKG-INFO` & `viessmann_gridbox_connector-1.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.2.0
+Version: 1.3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
```

### Comparing `viessmann_gridbox_connector-1.2.0/README.md` & `viessmann_gridbox_connector-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.2.0/gridbox_connector/GridboxConnector.py` & `viessmann_gridbox_connector-1.3.7/gridbox_connector/GridboxConnector.py`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.2.0/viessmann_gridbox_connector.egg-info/PKG-INFO` & `viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.2.0
+Version: 1.3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
```

