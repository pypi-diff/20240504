# Comparing `tmp/queue_pipelines-0.1.1.tar.gz` & `tmp/queue_pipelines-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_pipelines-0.1.1.tar", last modified: Sat May  4 13:47:31 2024, max compression
+gzip compressed data, was "queue_pipelines-0.1.2.tar", last modified: Sat May  4 15:40:24 2024, max compression
```

## Comparing `queue_pipelines-0.1.1.tar` & `queue_pipelines-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.941747 queue_pipelines-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 13:47:31.941747 queue_pipelines-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2178 2024-05-04 11:24:45.000000 queue_pipelines-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-05-04 13:47:29.000000 queue_pipelines-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-04 13:47:31.941747 queue_pipelines-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/pipelines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1491 2024-05-04 11:08:58.000000 queue_pipelines-0.1.1/src/q/pipelines/_connect.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/pipelines/codegen/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2394 2024-05-04 11:01:51.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_local.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-05-04 10:59:34.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      581 2024-05-04 11:21:19.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines_init.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1889 2024-05-04 11:17:02.000000 queue_pipelines-0.1.1/src/q/pipelines/codegen/_types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/q/pipelines/local/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/local/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-04 10:52:13.000000 queue_pipelines-0.1.1/src/q/pipelines/local/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-05-04 10:58:39.000000 queue_pipelines-0.1.1/src/q/pipelines/local/queues.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3779 2024-05-04 11:20:42.000000 queue_pipelines-0.1.1/src/q/pipelines/specs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      493 2024-05-04 10:57:48.000000 queue_pipelines-0.1.1/src/q/pipelines/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 13:47:31.931747 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       93 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-04 13:47:31.000000 queue_pipelines-0.1.1/src/queue_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2178 2024-05-04 15:40:22.000000 queue_pipelines-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-05-04 15:40:22.000000 queue_pipelines-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-04 15:33:49.000000 queue_pipelines-0.1.2/src/q/pipelines/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/codegen/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      190 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2126 2024-05-04 14:18:33.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      581 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines_init.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2098 2024-05-04 14:49:38.000000 queue_pipelines-0.1.2/src/q/pipelines/codegen/_types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/local/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/local/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/local/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      846 2024-05-04 15:29:13.000000 queue_pipelines-0.1.2/src/q/pipelines/local/queues.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/q/pipelines/runners/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-04 15:33:30.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-05-04 15:33:43.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1447 2024-05-04 15:32:51.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/_connect.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-05-04 15:35:47.000000 queue_pipelines-0.1.2/src/q/pipelines/runners/_run.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3779 2024-05-04 13:50:58.000000 queue_pipelines-0.1.2/src/q/pipelines/specs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      484 2024-05-04 14:07:32.000000 queue_pipelines-0.1.2/src/q/pipelines/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-04 15:40:24.176299 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2796 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      809 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       93 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-04 15:40:24.000000 queue_pipelines-0.1.2/src/queue_pipelines.egg-info/top_level.txt
```

### Comparing `queue_pipelines-0.1.1/PKG-INFO` & `queue_pipelines-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-pipelines
-Version: 0.1.1
+Version: 0.1.2
 Summary: Declarative orchestration of asynchronous queue-based tasks
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: dslog
```

### Comparing `queue_pipelines-0.1.1/README.md` & `queue_pipelines-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.1/pyproject.toml` & `queue_pipelines-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-pipelines"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Declarative orchestration of asynchronous queue-based tasks"
 dependencies = [
   "queue-api", "dslog", "prettyprinter"
 ]
```

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/_connect.py` & `queue_pipelines-0.1.2/src/q/pipelines/runners/_connect.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from typing import TypeVar
-from functools import partial
 import asyncio
 from haskellian import IsLeft
-from q.api import ReadQueue, WriteQueue
 from dslog import Logger
-from .specs import OutId
-from .types import PipelineQueues
+from q.api import ReadQueue, WriteQueue
+from ..specs import OutId
+from ..types import Queues
 
 Id = TypeVar('Id', bound=str)
 A = TypeVar('A')
 B = TypeVar('B')
 
 def input_item(id: Id, item: A) -> tuple[Id, A]:
   return id, item
 
 async def connect(
   Qin: ReadQueue[A],
   Qout: WriteQueue[B],
-  queues: PipelineQueues[Id, A], *,
+  queues: Queues[Id, A], *,
   input_task: Id,
   logger = Logger.rich().prefix('[CONNECT]')
 ):
   async def connect_output(name: str, Qw: ReadQueue[tuple[OutId[Id], A]]):
     while True:
       try:
         id, (next_id, next_inp) = (await Qw.read()).unsafe()
```

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/codegen/_local.py` & `queue_pipelines-0.1.2/src/q/pipelines/codegen/_local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # BEGIN
 from typing_extensions import Literal, Any, Unpack
-from haskellian import promise as P
 from dslog import Logger
 from q.api import ReadQueue, WriteQueue
 from q.kv import QueueKV
-from q.pipelines import local as loc, connect as raw_connect
+import q.pipelines as qp
 AnyT: type = Any # type: ignore
 # UNCOMMENT from MODULE import INPUT, OUTPUT, SPEC_VARIABLE
 # UNCOMMENT from TYPES import Queues, Pipelines
 from ._types import Queues, Pipelines # DELETE
 INPUT = int # DELETE
 OUTPUT = int # DELETE
 
@@ -23,46 +22,35 @@
   return QueueKV.at(OUTPUT, output_path, protocol=protocol)
 
 SPEC_VARIABLE = ... # DELETE
 def queues(
   path: str, *,
   protocol: Literal['sqlite', 'fs'] = 'sqlite',
 ) -> Queues:
-  return loc.local_queues(path, SPEC_VARIABLE, protocol=protocol) # type: ignore
+  return qp.local.local_queues(path, SPEC_VARIABLE, protocol=protocol) # type: ignore
 
-@P.run
 async def connect(
   Qin: ReadQueue[INPUT],
   Qout: WriteQueue[OUTPUT],
   queues: Queues, *,
   logger = Logger.rich().prefix('[CONNECT]')
 ):
-  await raw_connect(Qin, Qout, queues, input_task='INPUT_TASK', logger=logger) # type: ignore
+  await qp.connect(Qin, Qout, queues, input_task='INPUT_TASK', logger=logger) # type: ignore
 
 def run_pipelines(queues: Queues, **pipelines: Unpack[Pipelines]):
-  from multiprocessing import Process
-  processes = {
-    task: Process(target=pipelines[task], args=queues[task])
-    for task in queues.keys()
-  }
-  for process in processes.values():
-    process.start()
-  for process in processes.values():
-    process.join()
+  qp.run_pipelines(queues, **pipelines) # type: ignore
 
 def run(
   Qin: ReadQueue[INPUT],
   Qout: WriteQueue[OUTPUT],
-  queues: Queues, **pipelines: Unpack[Pipelines]
+  queues: Queues,
+  connect_logger = Logger.rich().prefix('[CONNECT]'),
+  **pipelines: Unpack[Pipelines]
 ):
-  from multiprocessing import Process
-  p = Process(target=connect, args=(Qin, Qout, queues))
-  p.start()
-  run_pipelines(queues, **pipelines)
-  p.join()
+  qp.run(Qin, Qout, queues, input_task='INPUT_TASK', connect_logger=connect_logger, **pipelines) # type: ignore
 
 __all__ = ['input_queue', 'output_queue', 'queues', 'connect', 'run_pipelines', 'run']
 
 # END
 from templang import parse
 from q.pipelines import Tasks
```

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines.py` & `queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/codegen/_pipelines_init.py` & `queue_pipelines-0.1.2/src/q/pipelines/codegen/_pipelines_init.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/codegen/_types.py` & `queue_pipelines-0.1.2/src/q/pipelines/codegen/_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # BEGIN
-from typing import Literal, TypedDict, Union, overload
+from typing import Literal, TypedDict, Union, overload, TypeAlias
 from q.api import ReadQueue, WriteQueue
 from q.pipelines import TaskQueues, Pipeline
 # UNCOMMENT from MODULE import MOD_IMPORTS
 
 INPUT = int # DELETE
 OUTPUT_TYPE = int # DELETE
 
@@ -35,32 +35,37 @@
   # END 
 
 class Pipelines(TypedDict):
   # LOOP TASK TSKID
   TSKID: Pipeline[TASK.In, TASK.Out]
   # END
 
+T_INP = T_OUT = int # DELETE
+QueueIn: TypeAlias = ReadQueue[T_INP]
+QueueOut: TypeAlias = WriteQueue[T_OUT]
+
 __all__ = [
   # LOOP TASK
   'TASK',
   # END
-  'Queues', 'Pipelines',
+  'Queues', 'Pipelines', 'QueueIn', 'QueueOut',
 ]
 # END
 from templang import parse
 from ..specs import Tasks
 
 def types(tasks: Tasks, module: str) -> str:
   with open(__file__) as f:
     source = f.read()
 
   imports = ', '.join(set(tasks.InType(id).__name__ for id in tasks.tasks.keys()))
 
   translations = {
     'MODULE': module, 'MOD_IMPORTS': imports + ', ' + tasks.Output.__name__,
+    'T_INP': tasks.Input.__name__, 'T_OUT': tasks.Output.__name__,
     'TASK': [], 'TSKID': [], 'INPUT': [], 'OUTPUT_ID': [], 'OUTPUT_TYPE': [],
   }
 
   for id, task in tasks.tasks.items():
     translations['TASK'].append(id.title())
     translations['TSKID'].append(id)
     translations['INPUT'].append(task.Input.__name__)
```

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/local/queues.py` & `queue_pipelines-0.1.2/src/q/pipelines/local/queues.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeVar, Any, Literal
 import os
 from q.kv import QueueKV
-from ..specs import Task, Tasks, OutId
-from ..types import TaskQueues, PipelineQueues
+from ..specs import Task, Tasks
+from ..types import TaskQueues, Queues
 
 T = TypeVar('T')
 Id = TypeVar('Id', bound=str)
 Out = TypeVar('Out', bound=tuple)
 
 def task_queues(
   path: str,
@@ -18,15 +18,15 @@
     QueueKV.at(task.Input, os.path.join(path, 'in'), protocol=protocol),
     QueueKV.at(OutputType, os.path.join(path, 'out'), protocol=protocol),
   )
 
 def local_queues(
   path: str, tasks: Tasks[T, Any, Id],
   *, protocol: Literal['sqlite', 'fs'] = 'sqlite',
-) -> PipelineQueues[Id, T]:
+) -> Queues[Id, T]:
   return {
     id: task_queues(
       path=os.path.join(path, id), task=task,
       OutputType=tasks.OutType(id),
       protocol=protocol
     )
     for id, task in tasks.tasks.items()
```

### Comparing `queue_pipelines-0.1.1/src/q/pipelines/specs.py` & `queue_pipelines-0.1.2/src/q/pipelines/specs.py`

 * *Files identical despite different names*

### Comparing `queue_pipelines-0.1.1/src/queue_pipelines.egg-info/PKG-INFO` & `queue_pipelines-0.1.2/src/queue_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queue-pipelines
-Version: 0.1.1
+Version: 0.1.2
 Summary: Declarative orchestration of asynchronous queue-based tasks
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/pipelines.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: queue-api
 Requires-Dist: dslog
```

### Comparing `queue_pipelines-0.1.1/src/queue_pipelines.egg-info/SOURCES.txt` & `queue_pipelines-0.1.2/src/queue_pipelines.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 README.md
 pyproject.toml
 src/q/pipelines/__init__.py
 src/q/pipelines/__init__.pyi
-src/q/pipelines/_connect.py
 src/q/pipelines/specs.py
 src/q/pipelines/types.py
 src/q/pipelines/codegen/__init__.py
 src/q/pipelines/codegen/__init__.pyi
 src/q/pipelines/codegen/_local.py
 src/q/pipelines/codegen/_pipelines.py
 src/q/pipelines/codegen/_pipelines_init.py
 src/q/pipelines/codegen/_types.py
 src/q/pipelines/local/__init__.py
 src/q/pipelines/local/__init__.pyi
 src/q/pipelines/local/queues.py
+src/q/pipelines/runners/__init__.py
+src/q/pipelines/runners/__init__.pyi
+src/q/pipelines/runners/_connect.py
+src/q/pipelines/runners/_run.py
 src/queue_pipelines.egg-info/PKG-INFO
 src/queue_pipelines.egg-info/SOURCES.txt
 src/queue_pipelines.egg-info/dependency_links.txt
 src/queue_pipelines.egg-info/requires.txt
 src/queue_pipelines.egg-info/top_level.txt
```

