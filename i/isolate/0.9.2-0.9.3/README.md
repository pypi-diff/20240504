# Comparing `tmp/isolate-0.9.2.tar.gz` & `tmp/isolate-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isolate-0.9.2.tar", max compression
+gzip compressed data, was "isolate-0.9.3.tar", max compression
```

## Comparing `isolate-0.9.2.tar` & `isolate-0.9.3.tar`

### file list

```diff
@@ -1,47 +1,53 @@
--rw-r--r--   0        0        0     2722 2023-01-31 18:54:56.038926 isolate-0.9.2/README.md
--rw-r--r--   0        0        0      939 2023-01-31 18:55:04.115054 isolate-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      157 2023-01-31 18:54:56.038926 isolate-0.9.2/src/isolate/__init__.py
--rw-r--r--   0        0        0       91 2023-01-31 18:54:56.038926 isolate-0.9.2/src/isolate/backends/__init__.py
--rw-r--r--   0        0        0     4105 2023-01-31 18:54:56.038926 isolate-0.9.2/src/isolate/backends/_base.py
--rw-r--r--   0        0        0     7162 2023-01-31 18:54:56.038926 isolate-0.9.2/src/isolate/backends/common.py
--rw-r--r--   0        0        0     7055 2023-01-31 18:54:56.038926 isolate-0.9.2/src/isolate/backends/conda.py
--rw-r--r--   0        0        0     1366 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/backends/local.py
--rw-r--r--   0        0        0     5356 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/backends/pyenv.py
--rw-r--r--   0        0        0     4208 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/backends/remote.py
--rw-r--r--   0        0        0     3084 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/backends/settings.py
--rw-r--r--   0        0        0     5346 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/backends/virtualenv.py
--rw-r--r--   0        0        0      722 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/__init__.py
--rw-r--r--   0        0        0      118 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/_local/__init__.py
--rw-r--r--   0        0        0     6251 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/_local/_base.py
--rw-r--r--   0        0        0     1552 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/_local/agent_startup.py
--rw-r--r--   0        0        0     3475 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/common.py
--rw-r--r--   0        0        0       71 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/__init__.py
--rw-r--r--   0        0        0     5503 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/_base.py
--rw-r--r--   0        0        0     7677 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/agent.py
--rw-r--r--   0        0        0      788 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/configuration.py
--rw-r--r--   0        0        0      389 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/__init__.py
--rw-r--r--   0        0        0      568 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/agent.proto
--rw-r--r--   0        0        0     1344 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/agent_pb2.py
--rw-r--r--   0        0        0     1970 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/agent_pb2.pyi
--rw-r--r--   0        0        0     2451 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/agent_pb2_grpc.py
--rw-r--r--   0        0        0     1172 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/common.proto
--rw-r--r--   0        0        0     2141 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/common_pb2.py
--rw-r--r--   0        0        0     6413 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/common_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/definitions/common_pb2_grpc.py
--rw-r--r--   0        0        0     2130 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/grpc/interface.py
--rw-r--r--   0        0        0      117 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/ipc/__init__.py
--rw-r--r--   0        0        0     8434 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/ipc/_base.py
--rw-r--r--   0        0        0     6837 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/connections/ipc/agent.py
--rw-r--r--   0        0        0     9896 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/interface.py
--rw-r--r--   0        0        0     1818 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/logs.py
--rw-r--r--   0        0        0     1502 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/registry.py
--rw-r--r--   0        0        0       65 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/__init__.py
--rw-r--r--   0        0        0      488 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/definitions/__init__.py
--rw-r--r--   0        0        0      731 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/definitions/server.proto
--rw-r--r--   0        0        0     1825 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/definitions/server_pb2.py
--rw-r--r--   0        0        0     3306 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/definitions/server_pb2.pyi
--rw-r--r--   0        0        0     2548 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/definitions/server_pb2_grpc.py
--rw-r--r--   0        0        0      687 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/interface.py
--rw-r--r--   0        0        0    11038 2023-01-31 18:54:56.042926 isolate-0.9.2/src/isolate/server/server.py
--rw-r--r--   0        0        0     4282 2023-01-31 18:55:05.491849 isolate-0.9.2/setup.py
--rw-r--r--   0        0        0     3473 2023-01-31 18:55:05.492447 isolate-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2722 2023-02-03 09:12:01.140532 isolate-0.9.3/README.md
+-rw-r--r--   0        0        0      939 2023-02-03 09:12:09.972659 isolate-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/__init__.py
+-rw-r--r--   0        0        0       91 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/__init__.py
+-rw-r--r--   0        0        0     4105 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/_base.py
+-rw-r--r--   0        0        0     7162 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/common.py
+-rw-r--r--   0        0        0     7055 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/conda.py
+-rw-r--r--   0        0        0     1366 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/local.py
+-rw-r--r--   0        0        0     5356 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/pyenv.py
+-rw-r--r--   0        0        0     4208 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/remote.py
+-rw-r--r--   0        0        0     3084 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/settings.py
+-rw-r--r--   0        0        0     5346 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/backends/virtualenv.py
+-rw-r--r--   0        0        0      722 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/__init__.py
+-rw-r--r--   0        0        0      118 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/_local/__init__.py
+-rw-r--r--   0        0        0     6251 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/_local/_base.py
+-rw-r--r--   0        0        0     1552 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/_local/agent_startup.py
+-rw-r--r--   0        0        0     3475 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/common.py
+-rw-r--r--   0        0        0       71 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/__init__.py
+-rw-r--r--   0        0        0     5503 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/_base.py
+-rw-r--r--   0        0        0     7677 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/agent.py
+-rw-r--r--   0        0        0      788 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/configuration.py
+-rw-r--r--   0        0        0      389 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/__init__.py
+-rw-r--r--   0        0        0      568 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/agent.proto
+-rw-r--r--   0        0        0     1344 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/agent_pb2.py
+-rw-r--r--   0        0        0     1970 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/agent_pb2.pyi
+-rw-r--r--   0        0        0     2451 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     1172 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/common.proto
+-rw-r--r--   0        0        0     2141 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/common_pb2.py
+-rw-r--r--   0        0        0     6413 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/common_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/definitions/common_pb2_grpc.py
+-rw-r--r--   0        0        0     2130 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/grpc/interface.py
+-rw-r--r--   0        0        0      117 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/ipc/__init__.py
+-rw-r--r--   0        0        0     8434 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/ipc/_base.py
+-rw-r--r--   0        0        0     6837 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/connections/ipc/agent.py
+-rw-r--r--   0        0        0     9896 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/interface.py
+-rw-r--r--   0        0        0     1818 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/logs.py
+-rw-r--r--   0        0        0     1502 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/registry.py
+-rw-r--r--   0        0        0       65 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/__init__.py
+-rw-r--r--   0        0        0      488 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/definitions/__init__.py
+-rw-r--r--   0        0        0      731 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/definitions/server.proto
+-rw-r--r--   0        0        0     1825 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/definitions/server_pb2.py
+-rw-r--r--   0        0        0     3306 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/definitions/server_pb2.pyi
+-rw-r--r--   0        0        0     2548 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/definitions/server_pb2_grpc.py
+-rw-r--r--   0        0        0      282 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/health/__init__.py
+-rw-r--r--   0        0        0      455 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/health/health.proto
+-rw-r--r--   0        0        0     1783 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/health/health_pb2.py
+-rw-r--r--   0        0        0     2546 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/health/health_pb2.pyi
+-rw-r--r--   0        0        0     4005 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/health/health_pb2_grpc.py
+-rw-r--r--   0        0        0     1249 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/health_server.py
+-rw-r--r--   0        0        0      687 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/interface.py
+-rw-r--r--   0        0        0    11159 2023-02-03 09:12:01.144533 isolate-0.9.3/src/isolate/server/server.py
+-rw-r--r--   0        0        0     4308 2023-02-03 09:12:11.335535 isolate-0.9.3/setup.py
+-rw-r--r--   0        0        0     3473 2023-02-03 09:12:11.336057 isolate-0.9.3/PKG-INFO
```

### Comparing `isolate-0.9.2/README.md` & `isolate-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/pyproject.toml` & `isolate-0.9.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "isolate"
-version = "0.9.2"
+version = "0.9.3"
 readme = "README.md"
 description = "Managed isolated environments for Python"
 authors = ["Features & Labels <hello@fal.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 virtualenv = ">=20.4"
```

### Comparing `isolate-0.9.2/src/isolate/backends/_base.py` & `isolate-0.9.3/src/isolate/backends/_base.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/common.py` & `isolate-0.9.3/src/isolate/backends/common.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/conda.py` & `isolate-0.9.3/src/isolate/backends/conda.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/local.py` & `isolate-0.9.3/src/isolate/backends/local.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/pyenv.py` & `isolate-0.9.3/src/isolate/backends/pyenv.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/remote.py` & `isolate-0.9.3/src/isolate/backends/remote.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/settings.py` & `isolate-0.9.3/src/isolate/backends/settings.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/backends/virtualenv.py` & `isolate-0.9.3/src/isolate/backends/virtualenv.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/__init__.py` & `isolate-0.9.3/src/isolate/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/_local/_base.py` & `isolate-0.9.3/src/isolate/connections/_local/_base.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/_local/agent_startup.py` & `isolate-0.9.3/src/isolate/connections/_local/agent_startup.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/common.py` & `isolate-0.9.3/src/isolate/connections/common.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/_base.py` & `isolate-0.9.3/src/isolate/connections/grpc/_base.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/agent.py` & `isolate-0.9.3/src/isolate/connections/grpc/agent.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/configuration.py` & `isolate-0.9.3/src/isolate/connections/grpc/configuration.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/agent.proto` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/agent.proto`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/agent_pb2.py` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/agent_pb2.pyi` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/agent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/agent_pb2_grpc.py` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/common.proto` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/common.proto`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/common_pb2.py` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/common_pb2.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/definitions/common_pb2.pyi` & `isolate-0.9.3/src/isolate/connections/grpc/definitions/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/grpc/interface.py` & `isolate-0.9.3/src/isolate/connections/grpc/interface.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/ipc/_base.py` & `isolate-0.9.3/src/isolate/connections/ipc/_base.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/connections/ipc/agent.py` & `isolate-0.9.3/src/isolate/connections/ipc/agent.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/interface.py` & `isolate-0.9.3/src/isolate/interface.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/logs.py` & `isolate-0.9.3/src/isolate/logs.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/registry.py` & `isolate-0.9.3/src/isolate/registry.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/server/definitions/server.proto` & `isolate-0.9.3/src/isolate/server/definitions/server.proto`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/server/definitions/server_pb2.py` & `isolate-0.9.3/src/isolate/server/definitions/server_pb2.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/server/definitions/server_pb2.pyi` & `isolate-0.9.3/src/isolate/server/definitions/server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/server/definitions/server_pb2_grpc.py` & `isolate-0.9.3/src/isolate/server/definitions/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/server/interface.py` & `isolate-0.9.3/src/isolate/server/interface.py`

 * *Files identical despite different names*

### Comparing `isolate-0.9.2/src/isolate/server/server.py` & `isolate-0.9.3/src/isolate/server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 )
 from isolate.backends.common import active_python
 from isolate.backends.local import LocalPythonEnvironment
 from isolate.backends.virtualenv import VirtualPythonEnvironment
 from isolate.connections.grpc import AgentError, LocalPythonGRPC
 from isolate.connections.grpc.configuration import get_default_options
 from isolate.logs import Log, LogLevel, LogSource
-from isolate.server import definitions
+from isolate.server import definitions, health
+from isolate.server.health_server import HealthServicer
 from isolate.server.interface import from_grpc, to_grpc
 
 # Whether to inherit all the packages from the current environment or not.
 INHERIT_FROM_LOCAL = os.getenv("ISOLATE_INHERIT_FROM_LOCAL") == "1"
 
 # Number of threads that the gRPC server will use.
 MAX_THREADS = int(os.getenv("MAX_THREADS", 5))
@@ -288,14 +289,15 @@
 def main() -> None:
     server = grpc.server(
         futures.ThreadPoolExecutor(max_workers=MAX_THREADS),
         options=get_default_options(),
     )
     with BridgeManager() as bridge_manager:
         definitions.register_isolate(IsolateServicer(bridge_manager), server)
+        health.register_health(HealthServicer(), server)
 
         server.add_insecure_port(f"[::]:50001")
         print("Started listening at localhost:50001")
 
         server.start()
         server.wait_for_termination()
```

### Comparing `isolate-0.9.2/setup.py` & `isolate-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
  'isolate.backends',
  'isolate.connections',
  'isolate.connections._local',
  'isolate.connections.grpc',
  'isolate.connections.grpc.definitions',
  'isolate.connections.ipc',
  'isolate.server',
- 'isolate.server.definitions']
+ 'isolate.server.definitions',
+ 'isolate.server.health']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'grpcio>=1.49',
@@ -33,15 +34,15 @@
                       'local = isolate.backends.local:LocalPythonEnvironment',
                       'pyenv = isolate.backends.pyenv:PyenvEnvironment',
                       'virtualenv = '
                       'isolate.backends.virtualenv:VirtualPythonEnvironment']}
 
 setup_kwargs = {
     'name': 'isolate',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Managed isolated environments for Python',
     'long_description': '# Isolate\n\n> :warning: **Isolate** is still very young, and none of the APIs should be considered stable.\n\nRun any Python function, with any dependencies, in any machine you want. Isolate offers a\npluggable end-to-end solution for building, managing, and using isolated environments (virtualenv,\nconda, remote, and more).\n\n## Try it!\n\n```py\nfrom isolate import Template, LocalBox\n\n# Build you first environment by specifying its kind (like virtualenv or conda)\ntemplate = Template("virtualenv")\n\n# Add some packages to it.\ntemplate << "pyjokes==0.5.0"\n\n# Forward it to a box (your local machine, or a remote machine)\nenvironment = template >> LocalBox()\n\n# And then, finally try executing some code\n\ndef get_pyjokes_version():\n    import pyjokes\n\n    return pyjokes.__version__\n\n# If pyjokes==0.6.0 is installed in your local environment, it is going to print\n# 0.6.0 here.\nprint("Installed pyjokes version: ", get_pyjokes_version())\n\n# But if you run the same function in an isolated environment, you\'ll get\n# 0.5.0.\nprint("Isolated pyjokes version: ", environment.run(get_pyjokes_version))\n```\n\n## Motivation\n\n![XKCD 1987](https://imgs.xkcd.com/comics/python_environment.png)\n\nThe fact that nearly every piece of software uses some other libraries or some\nother programs is undeniable. Each of these come with their set of dependencies,\nand this chain moves forward. Once there are enough \'nodes\' in the chain, then\nthe ["dependency mess"](https://en.wikipedia.org/wiki/Dependency_hell) starts\nto surface and our lives become much harder.\n\nPython tried to solve it by recommending the "virtual environment" concept. In\ntheory it was designed to isolate environments of different projects, so my project\nA can depend on `pandas==1.0.0` while B depends on `pandas==2.0.0` and whichever\nproject I choose to work with, I just activate its own environment.\n\nOverall this was a very nice solution that did work, and still continues to work\nfor this use case. But as with every other scoped fix, in time other problems started\nto appear that demand a much narrower scope (like defining module-level dependencies,\nor even function-level ones for cloud runtimes that allow seamless integration with the\nrest of your code running in a different machine).\n\nHowever, unlike "virtual environment" concept, each of the projects that tried to tackle\nthis problem lacked a universal interface which one can simply define a set of requirements\n(this might be dependencies, size of the machine that is needed to run it, or something completely\ndifferent) and can change it without any loss. Isolate is working towards a future where this\ntransititon is as seamless as the transition from your local environment to the remote\nenvironment.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `isolate-0.9.2/PKG-INFO` & `isolate-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isolate
-Version: 0.9.2
+Version: 0.9.3
 Summary: Managed isolated environments for Python
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

