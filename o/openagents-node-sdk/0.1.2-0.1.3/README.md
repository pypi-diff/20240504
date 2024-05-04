# Comparing `tmp/openagents_node_sdk-0.1.2.tar.gz` & `tmp/openagents_node_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.1.2.tar", last modified: Sat May  4 09:02:53 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.1.3.tar", last modified: Sat May  4 12:20:10 2024, max compression
```

## Comparing `openagents_node_sdk-0.1.2.tar` & `openagents_node_sdk-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:02:53.380253 openagents_node_sdk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 09:02:53.380253 openagents_node_sdk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:02:53.380253 openagents_node_sdk-0.1.2/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16104 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:02:53.380253 openagents_node_sdk-0.1.2/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 09:02:53.000000 openagents_node_sdk-0.1.2/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-04 09:02:53.000000 openagents_node_sdk-0.1.2/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:02:53.000000 openagents_node_sdk-0.1.2/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-04 09:02:53.000000 openagents_node_sdk-0.1.2/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 09:02:53.000000 openagents_node_sdk-0.1.2/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 09:02:53.380253 openagents_node_sdk-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 09:02:51.000000 openagents_node_sdk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:20:10.168833 openagents_node_sdk-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 12:20:10.168833 openagents_node_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:20:10.168833 openagents_node_sdk-0.1.3/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16104 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:20:10.168833 openagents_node_sdk-0.1.3/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 12:20:10.000000 openagents_node_sdk-0.1.3/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-04 12:20:10.000000 openagents_node_sdk-0.1.3/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:20:10.000000 openagents_node_sdk-0.1.3/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-04 12:20:10.000000 openagents_node_sdk-0.1.3/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 12:20:10.000000 openagents_node_sdk-0.1.3/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 12:20:10.168833 openagents_node_sdk-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 12:20:04.000000 openagents_node_sdk-0.1.3/setup.py
```

### Comparing `openagents_node_sdk-0.1.2/LICENSE` & `openagents_node_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/README.md` & `openagents_node_sdk-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # OpenAgents Node - Python SDK
 
 
 A Python SDK for developing OpenAgents nodes.
 
+## Installation
 
+```bash
+pip install openagents-node-sdk
+```
 
-## Example
+## Usage Example
 
 ```python
 from openagents import JobRunner,OpenAgentsNode,NodeConfig,RunnerConfig
 
 # Define a runner
 class MyRunner (JobRunner):
     def __init__(self):
```

### Comparing `openagents_node_sdk-0.1.2/openagents/Disk.py` & `openagents_node_sdk-0.1.3/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/DiskReader.py` & `openagents_node_sdk-0.1.3/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/DiskWriter.py` & `openagents_node_sdk-0.1.3/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/JobRunner.py` & `openagents_node_sdk-0.1.3/openagents/JobRunner.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/Logger.py` & `openagents_node_sdk-0.1.3/openagents/Logger.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/NodeConfig.py` & `openagents_node_sdk-0.1.3/openagents/NodeConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.1.3/openagents/OpenAgentsNode.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/openagents/RunnerConfig.py` & `openagents_node_sdk-0.1.3/openagents/RunnerConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.2/setup.py` & `openagents_node_sdk-0.1.3/setup.py`

 * *Files identical despite different names*

