# Comparing `tmp/openagents_grpc_proto-0.7.7.tar.gz` & `tmp/openagents_grpc_proto-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_grpc_proto-0.7.7.tar", last modified: Sat May  4 08:15:03 2024, max compression
+gzip compressed data, was "openagents_grpc_proto-0.7.8.tar", last modified: Sat May  4 08:33:50 2024, max compression
```

## Comparing `openagents_grpc_proto-0.7.7.tar` & `openagents_grpc_proto-0.7.8.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:15:03.331731 openagents_grpc_proto-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 08:15:03.331731 openagents_grpc_proto-0.7.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:15:03.327731 openagents_grpc_proto-0.7.7/openagents_grpc_proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobInput_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobParam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobParam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobResult_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobResult_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobState_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobStatus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/Job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/Job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/Log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    45184 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto/rpc_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:15:03.327731 openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 08:15:03.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-04 08:15:03.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:15:03.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-04 08:15:03.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 08:15:03.000000 openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:15:03.331731 openagents_grpc_proto-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-04 08:15:02.000000 openagents_grpc_proto-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:33:50.553750 openagents_grpc_proto-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 08:33:50.553750 openagents_grpc_proto-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:33:50.553750 openagents_grpc_proto-0.7.8/openagents_grpc_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobInput_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobParam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobParam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobResult_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobResult_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobState_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobStatus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/Job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/Job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/Log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45184 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto/rpc_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:33:50.553750 openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 08:33:50.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-04 08:33:50.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:33:50.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-04 08:33:50.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 08:33:50.000000 openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:33:50.553750 openagents_grpc_proto-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 08:33:49.000000 openagents_grpc_proto-0.7.8/setup.py
```

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobInput_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobInput_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobInput_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobInput_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobParam_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobParam_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobParam_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobParam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobResult_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobResult_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobResult_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobResult_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobState_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobState_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobState_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobState_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobStatus_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/JobStatus_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/JobStatus_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/Job_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/Job_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/Job_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/Job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/Log_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/Log_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/Log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/rpc_pb2.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto/rpc_pb2_grpc.py` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto/rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.7.7/openagents_grpc_proto.egg-info/SOURCES.txt` & `openagents_grpc_proto-0.7.8/openagents_grpc_proto.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+MANIFEST.in
+VERSION
 setup.py
 openagents_grpc_proto/JobInput_pb2.py
 openagents_grpc_proto/JobInput_pb2_grpc.py
 openagents_grpc_proto/JobParam_pb2.py
 openagents_grpc_proto/JobParam_pb2_grpc.py
 openagents_grpc_proto/JobResult_pb2.py
 openagents_grpc_proto/JobResult_pb2_grpc.py
```

