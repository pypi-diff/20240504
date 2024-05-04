# Comparing `tmp/queue_pipelines-0.1.0.tar.gz` & `tmp/queue_pipelines-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_pipelines-0.1.0.tar", last modified: Sat May  4 11:25:00 2024, max compression
+gzip compressed data, was "queue_pipelines-0.1.1.tar", last modified: Sat May  4 13:47:31 2024, max compression
```

## Comparing `queue_pipelines-0.1.0.tar` & `queue_pipelines-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2652 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2178 2024-05-04 11:24:45.000000 queue_pipelines-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      571 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/src/q/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/src/q/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/src/q/pipelines/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1491 2024-05-04 11:08:58.000000 queue_pipelines-0.1.0/src/q/pipelines/_connect.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/src/q/pipelines/codegen/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/src/q/pipelines/codegen/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/src/q/pipelines/codegen/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2394 2024-05-04 11:01:51.000000 queue_pipelines-0.1.0/src/q/pipelines/codegen/_local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-05-04 10:59:34.000000 queue_pipelines-0.1.0/src/q/pipelines/codegen/_pipelines.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      581 2024-05-04 11:21:19.000000 queue_pipelines-0.1.0/src/q/pipelines/codegen/_pipelines_init.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1889 2024-05-04 11:17:02.000000 queue_pipelines-0.1.0/src/q/pipelines/codegen/_types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/src/q/pipelines/local/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/src/q/pipelines/local/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-04 10:52:13.000000 queue_pipelines-0.1.0/src/q/pipelines/local/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-05-04 10:58:39.000000 queue_pipelines-0.1.0/src/q/pipelines/local/queues.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3779 2024-05-04 11:20:42.000000 queue_pipelines-0.1.0/src/q/pipelines/specs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      493 2024-05-04 10:57:48.000000 queue_pipelines-0.1.0/src/q/pipelines/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 11:25:00.354354 queue_pipelines-0.1.0/src/queue_pipelines.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2652 2024-05-04 11:25:00.000000 queue_pipelines-0.1.0/src/queue_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-04 11:25:00.000000 queue_pipelines-0.1.0/src/queue_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-04 11:25:00.000000 queue_pipelines-0.1.0/src/queue_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-05-04 11:25:00.000000 queue_pipelines-0.1.0/src/queue_pipelines.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-04 11:25:00.000000 queue_pipelines-0.1.0/src/queue_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.941747 queue_pipelines-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 13:47:31.941747 queue_pipelines-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2178 2024-05-04 11:24:45.000000 queue_pipelines-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-05-04 13:47:29.000000 queue_pipelines-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-04 13:47:31.941747 queue_pipelines-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1491 2024-05-04 11:08:58.000000 queue_pipelines-0.1.1/src/q/pipelines/_connect.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/pipelines/codegen/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2394 2024-05-04 11:01:51.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-05-04 10:59:34.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      581 2024-05-04 11:21:19.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines_init.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1889 2024-05-04 11:17:02.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/pipelines/local/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/local/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/local/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-05-04 10:58:39.000000 queue_pipelines-0.1.1/src/q/pipelines/local/queues.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3779 2024-05-04 11:20:42.000000 queue_pipelines-0.1.1/src/q/pipelines/specs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      493 2024-05-04 10:57:48.000000 queue_pipelines-0.1.1/src/q/pipelines/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       93 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/top_level.txt
```

### Comparing `queue_pipelines-0.1.0/PKG-INFO` & `queue_pipelines-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: queue-pipelines
-Version: 0.1.0
+Version: 0.1.1
 Summary: Declarative orchestration of asynchronous queue-based tasks
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: dslog
 Requires-Dist: prettyprinter
-Requires-Dist: templang
+Provides-Extra: all
+Requires-Dist: queue-kv; extra == "all"
+Requires-Dist: templang; extra == "all"
 Provides-Extra: local
 Requires-Dist: queue-kv; extra == "local"
+Provides-Extra: codegen
+Requires-Dist: templang; extra == "codegen"
 
 # Queue Pipelines
 
 > Declarative orchestration of asynchronous queue-based tasks
 
 ## Usage
```

### Comparing `queue_pipelines-0.1.0/README.md` & `queue_pipelines-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/pyproject.toml` & `queue_pipelines-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-pipelines"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Declarative orchestration of asynchronous queue-based tasks"
 dependencies = [
-  "queue-api", "dslog", "prettyprinter", "templang"
+  "queue-api", "dslog", "prettyprinter"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/marciclabas/pipelines.git"
 
 [project.optional-dependencies]
+all = ["queue-kv", "templang"]
 local = ["queue-kv"]
+codegen = ["templang"]
```

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/_connect.py` & `queue_pipelines-0.1.1/src/q/pipelines/_connect.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/codegen/_local.py` & `queue_pipelines-0.1.1/src/q/pipelines/codegen/_local.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/codegen/_pipelines.py` & `queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/codegen/_pipelines_init.py` & `queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines_init.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/codegen/_types.py` & `queue_pipelines-0.1.1/src/q/pipelines/codegen/_types.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/local/queues.py` & `queue_pipelines-0.1.1/src/q/pipelines/local/queues.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/q/pipelines/specs.py` & `queue_pipelines-0.1.1/src/q/pipelines/specs.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.0/src/queue_pipelines.egg-info/PKG-INFO` & `queue_pipelines-0.1.1/src/queue_pipelines.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: queue-pipelines
-Version: 0.1.0
+Version: 0.1.1
 Summary: Declarative orchestration of asynchronous queue-based tasks
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: dslog
 Requires-Dist: prettyprinter
-Requires-Dist: templang
+Provides-Extra: all
+Requires-Dist: queue-kv; extra == "all"
+Requires-Dist: templang; extra == "all"
 Provides-Extra: local
 Requires-Dist: queue-kv; extra == "local"
+Provides-Extra: codegen
+Requires-Dist: templang; extra == "codegen"
 
 # Queue Pipelines
 
 > Declarative orchestration of asynchronous queue-based tasks
 
 ## Usage
```

### Comparing `queue_pipelines-0.1.0/src/queue_pipelines.egg-info/SOURCES.txt` & `queue_pipelines-0.1.1/src/queue_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

