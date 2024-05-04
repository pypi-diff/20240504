# Comparing `tmp/calltrack-0.0.1.tar.gz` & `tmp/calltrack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calltrack-0.0.1.tar", max compression
+gzip compressed data, was "calltrack-0.0.2.tar", max compression
```

## Comparing `calltrack-0.0.1.tar` & `calltrack-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,12 @@
--rw-r--r--   0        0        0        0 2024-05-03 08:28:05.244987 calltrack-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-03 10:10:30.137273 calltrack-0.0.1/calltrack/__init__.py
--rw-r--r--   0        0        0       97 2024-05-03 10:07:38.552167 calltrack-0.0.1/calltrack/setup.py
--rw-r--r--   0        0        0        0 2024-05-03 10:05:16.395151 calltrack-0.0.1/calltrack/src/__init__.py
--rw-r--r--   0        0        0      143 2024-05-03 10:10:32.393288 calltrack-0.0.1/calltrack/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2779 2024-05-03 15:27:06.794168 calltrack-0.0.1/calltrack/src/__pycache__/decorators.cpython-310.pyc
--rw-r--r--   0        0        0     4391 2024-05-03 15:25:43.753514 calltrack-0.0.1/calltrack/src/__pycache__/log_writer.cpython-310.pyc
--rw-r--r--   0        0        0     2485 2024-05-03 15:29:21.747251 calltrack-0.0.1/calltrack/src/decorators.py
--rw-r--r--   0        0        0     2834 2024-05-03 15:25:38.509473 calltrack-0.0.1/calltrack/src/log_writer.py
--rw-r--r--   0        0        0     9186 2024-05-03 15:02:57.318524 calltrack-0.0.1/calltrack/src/main.ipynb
--rw-r--r--   0        0        0     1252 2024-05-03 15:26:37.521936 calltrack-0.0.1/calltrack/src/main.py
--rw-r--r--   0        0        0        0 2024-05-03 10:05:50.791422 calltrack-0.0.1/calltrack/tests/__init__.py
--rw-r--r--   0        0        0      145 2024-05-03 10:09:29.460874 calltrack-0.0.1/calltrack/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4694 2024-05-03 10:22:30.782404 calltrack-0.0.1/calltrack/tests/__pycache__/test_log_writer.cpython-310-pytest-8.2.0.pyc
--rw-r--r--   0        0        0     2025 2024-05-03 10:22:28.846390 calltrack-0.0.1/calltrack/tests/test_log_writer.py
--rw-r--r--   0        0        0      395 2024-05-04 07:50:09.711124 calltrack-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 calltrack-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-03 08:28:05.244987 calltrack-0.0.2/README.md
+-rw-r--r--   0        0        0     2657 2024-05-04 17:04:49.376399 calltrack-0.0.2/calltrack/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-03 10:07:38.552167 calltrack-0.0.2/calltrack/setup.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:05:16.395151 calltrack-0.0.2/calltrack/src/__init__.py
+-rw-r--r--   0        0        0     2874 2024-05-04 17:07:17.388848 calltrack-0.0.2/calltrack/src/calltrack.py
+-rw-r--r--   0        0        0     2648 2024-05-04 12:15:06.335788 calltrack-0.0.2/calltrack/src/decorators.py
+-rw-r--r--   0        0        0      433 2024-05-04 12:05:40.058066 calltrack-0.0.2/calltrack/src/log_queue.py
+-rw-r--r--   0        0        0      398 2024-05-04 12:26:22.259699 calltrack-0.0.2/calltrack/src/utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:05:50.791422 calltrack-0.0.2/calltrack/tests/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-03 10:22:28.846390 calltrack-0.0.2/calltrack/tests/test_log_writer.py
+-rw-r--r--   0        0        0      395 2024-05-04 17:09:23.930612 calltrack-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 calltrack-0.0.2/PKG-INFO
```

### Comparing `calltrack-0.0.1/calltrack/src/log_writer.py` & `calltrack-0.0.2/calltrack/src/calltrack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 import json
 import os
-import uuid
+import warnings
 from abc import ABC, abstractmethod
-from collections import deque
 from datetime import datetime
 from typing import Any
 
+from .log_queue import LogQueue
+from .utils import is_path_creatable
 
-class LogQueue:
-    def __init__(self, name: str):
-        self.name = name
-        self.id = uuid.uuid4()
-        self.queue = deque([])
-
-    def append(self, log: Any) -> None:
-        """Add the log on top of a stack."""
-        self.queue.append(log)
 
-    def popleft(self):
-        return self.queue.popleft()
-
-
-class LogWriter(ABC):
-    """LogWriter Abstract Class"""
+class Calltrack(ABC):
+    """Calltrack Abstract Class"""
 
     def __init__(self, log_queue: LogQueue):
         self.log_queue = log_queue
 
     def flush(self) -> None:
         while self.log_queue.queue:
             self.write(self.log_queue.popleft())
@@ -35,29 +23,41 @@
     def write(
         self,
         log: Any,
     ) -> None:
         """Write logs"""
 
 
-class ConsoleLogWriter(LogWriter):
+class ConsoleCalltrack(Calltrack):
     def write(self, log: Any) -> None:
         print(log)
 
 
-class JSONLogWriter(LogWriter):
+class JSONCalltrack(Calltrack):
     def __init__(
         self, log_queue: LogQueue, save_dir: str, autoflush: bool = False
     ) -> None:
         super().__init__(log_queue=log_queue)
-        self.save_dir = save_dir
+        self._save_dir = save_dir
         self.autoflush = autoflush
 
         self._prepare_dir()
 
+    @property
+    def save_dir(self):
+        return self._save_dir
+
+    @save_dir.setter
+    def save_dir(self, path: str) -> None:
+        if is_path_creatable(path):
+            self._save_dir = path
+            self._prepare_dir()
+        else:
+            warnings.warn("The provided path is ill-formed.")
+
     def flush(self, filename: str | None = None):
         concat_log = {}
         while self.log_queue.queue:
             log = self.log_queue.queue.popleft()
             self._check_log(log)
             concat_log.update(log)
         self.write(concat_log, filename)
```

### Comparing `calltrack-0.0.1/calltrack/tests/test_log_writer.py` & `calltrack-0.0.2/calltrack/tests/test_log_writer.py`

 * *Files identical despite different names*

### Comparing `calltrack-0.0.1/PKG-INFO` & `calltrack-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calltrack
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: WILLIAM PONS
 Author-email: wmpons.pro@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

