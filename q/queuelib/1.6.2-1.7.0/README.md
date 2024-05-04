# Comparing `tmp/queuelib-1.6.2.tar.gz` & `tmp/queuelib-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queuelib-1.6.2.tar", last modified: Thu Aug 26 13:42:06 2021, max compression
+gzip compressed data, was "queuelib-1.7.0.tar", last modified: Sat May  4 06:02:51 2024, max compression
```

## Comparing `queuelib-1.6.2.tar` & `queuelib-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 13:42:06.891097 queuelib-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2021-08-26 13:41:56.000000 queuelib-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-08-26 13:41:56.000000 queuelib-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      663 2021-08-26 13:41:56.000000 queuelib-1.6.2/NEWS
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2021-08-26 13:42:06.895097 queuelib-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2021-08-26 13:41:56.000000 queuelib-1.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-08-26 13:41:56.000000 queuelib-1.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 13:42:06.891097 queuelib-1.6.2/queuelib/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/pqueue.py
--rw-r--r--   0 runner    (1001) docker     (121)     9261 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/rrqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 13:42:06.891097 queuelib-1.6.2/queuelib/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6654 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/tests/test_pqueue.py
--rw-r--r--   0 runner    (1001) docker     (121)    10037 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     7121 2021-08-26 13:41:56.000000 queuelib-1.6.2/queuelib/tests/test_rrqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-26 13:42:06.891097 queuelib-1.6.2/queuelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2021-08-26 13:42:06.000000 queuelib-1.6.2/queuelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      392 2021-08-26 13:42:06.000000 queuelib-1.6.2/queuelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-26 13:42:06.000000 queuelib-1.6.2/queuelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-08-26 13:42:06.000000 queuelib-1.6.2/queuelib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-08-26 13:42:06.895097 queuelib-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-08-26 13:41:56.000000 queuelib-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:02:51.436710 queuelib-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-04 06:02:38.000000 queuelib-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 06:02:38.000000 queuelib-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-04 06:02:38.000000 queuelib-1.7.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-04 06:02:51.436710 queuelib-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-04 06:02:38.000000 queuelib-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-04 06:02:38.000000 queuelib-1.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:02:51.432711 queuelib-1.7.0/queuelib/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/pqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/rrqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:02:51.436710 queuelib-1.7.0/queuelib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/tests/test_pqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-04 06:02:38.000000 queuelib-1.7.0/queuelib/tests/test_rrqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:02:51.436710 queuelib-1.7.0/queuelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-04 06:02:51.000000 queuelib-1.7.0/queuelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 06:02:51.000000 queuelib-1.7.0/queuelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:02:51.000000 queuelib-1.7.0/queuelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 06:02:51.000000 queuelib-1.7.0/queuelib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 06:02:51.436710 queuelib-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-04 06:02:38.000000 queuelib-1.7.0/setup.py
```

### Comparing `queuelib-1.6.2/LICENSE` & `queuelib-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `queuelib-1.6.2/NEWS` & `queuelib-1.7.0/NEWS`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Queuelib release notes
 ======================
 
+Version 1.7.0
+-------------
+(released on May 4th, 2024)
+
+No functionality changes with respect to 1.6.2
+
+* Added support for Python 3.10-3.12 and PyPy 3.10
+* Removed support for Python 3.5-3.7
+* Improved type annotations and added the ``py.typed`` file
+* Added ``pre-commit`` configuration
+* Improved linting and CI configuration
+
+
 Version 1.6.2
 -------------
 (released on August 26th, 2021)
 
 No functionality changes with respect to 1.6.1
 
 * Added `python_requires>=3.5` to `setup.py`
```

### Comparing `queuelib-1.6.2/PKG-INFO` & `queuelib-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: queuelib
-Version: 1.6.2
+Version: 1.7.0
 Summary: Collection of persistent (disk-based) and non-persistent (memory-based) queues
 Home-page: https://github.com/scrapy/queuelib
 Author: Scrapy project
 Author-email: info@scrapy.org
 License: BSD
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 queuelib
 ========
 
 .. image:: https://img.shields.io/pypi/v/queuelib.svg
@@ -207,9 +208,7 @@
 
 This software follows `Semantic Versioning`_
 
 .. _Scrapy framework: http://scrapy.org
 .. _scrapy-users: http://groups.google.com/group/scrapy-users
 .. _Semantic Versioning: http://semver.org/
 .. _nosetests: https://nose.readthedocs.org/en/latest/
-
-
```

### Comparing `queuelib-1.6.2/README.rst` & `queuelib-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `queuelib-1.6.2/queuelib/pqueue.py` & `queuelib-1.7.0/queuelib/pqueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
     startprios is a sequence of priorities to start with. If the queue was
     previously closed leaving some priority buckets non-empty, those priorities
     should be passed in startprios.
 
     """
 
-    def __init__(self, qfactory: Callable[[int], BaseQueue], startprios: Iterable[int] = ()) -> None:
+    def __init__(
+        self, qfactory: Callable[[int], BaseQueue], startprios: Iterable[int] = ()
+    ) -> None:
         self.queues = {}
         self.qfactory = qfactory
         for p in startprios:
             self.queues[p] = self.qfactory(p)
         self.curprio = min(startprios) if startprios else None
 
     def push(self, obj: Any, priority: int = 0) -> None:
```

### Comparing `queuelib-1.6.2/queuelib/queue.py` & `queuelib-1.7.0/queuelib/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import json
 import os
 import sqlite3
 import struct
 from abc import abstractmethod
 from collections import deque
 from contextlib import suppress
-from typing import Any, Optional
+from typing import Any, BinaryIO, Deque, Dict, Literal, Optional, cast
 
 
 class _BaseQueueMeta(type):
     """
     Metaclass to check queue classes against the necessary interface
     """
 
-    def __instancecheck__(cls, instance):
-        return cls.__subclasscheck__(type(instance))  # pylint: disable=no-value-for-parameter
+    def __instancecheck__(cls, instance: Any) -> bool:
+        return cls.__subclasscheck__(  # pylint: disable=no-value-for-parameter
+            type(instance)
+        )
 
-    def __subclasscheck__(cls, subclass):
+    def __subclasscheck__(cls, subclass: Any) -> bool:
         return (
             hasattr(subclass, "push")
             and callable(subclass.push)
             and hasattr(subclass, "pop")
             and callable(subclass.pop)
             and hasattr(subclass, "peek")
             and callable(subclass.peek)
@@ -42,40 +44,40 @@
         raise NotImplementedError()
 
     @abstractmethod
     def peek(self) -> Optional[Any]:
         raise NotImplementedError()
 
     @abstractmethod
-    def __len__(self):
+    def __len__(self) -> int:
         raise NotImplementedError()
 
     def close(self) -> None:
         pass
 
 
 class FifoMemoryQueue:
     """In-memory FIFO queue, API compliant with FifoDiskQueue."""
 
     def __init__(self) -> None:
-        self.q = deque()  # type: deque
+        self.q: Deque[Any] = deque()
 
     def push(self, obj: Any) -> None:
         self.q.append(obj)
 
     def pop(self) -> Optional[Any]:
         return self.q.popleft() if self.q else None
 
     def peek(self) -> Optional[Any]:
         return self.q[0] if self.q else None
 
     def close(self) -> None:
         pass
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.q)
 
 
 class LifoMemoryQueue(FifoMemoryQueue):
     """In-memory LIFO queue, API compliant with LifoDiskQueue."""
 
     def pop(self) -> Optional[Any]:
@@ -99,29 +101,29 @@
         self.chunksize = self.info["chunksize"]
         self.headf = self._openchunk(self.info["head"][0], "ab+")
         self.tailf = self._openchunk(self.info["tail"][0])
         os.lseek(self.tailf.fileno(), self.info["tail"][2], os.SEEK_SET)
 
     def push(self, string: bytes) -> None:
         if not isinstance(string, bytes):
-            raise TypeError("Unsupported type: {}".format(type(string).__name__))
+            raise TypeError(f"Unsupported type: {type(string).__name__}")
         hnum, hpos = self.info["head"]
         hpos += 1
         szhdr = struct.pack(self.szhdr_format, len(string))
         os.write(self.headf.fileno(), szhdr + string)
         if hpos == self.chunksize:
             hpos = 0
             hnum += 1
             self.headf.close()
             self.headf = self._openchunk(hnum, "ab+")
         self.info["size"] += 1
         self.info["head"] = [hnum, hpos]
 
-    def _openchunk(self, number: int, mode: str = "rb"):
-        return open(os.path.join(self.path, "q%05d" % number), mode)
+    def _openchunk(self, number: int, mode: Literal["rb", "ab+"] = "rb") -> BinaryIO:
+        return open(os.path.join(self.path, f"q{number:05d}"), mode)
 
     def pop(self) -> Optional[bytes]:
         tnum, tcnt, toffset = self.info["tail"]
         if [tnum, tcnt] >= self.info["head"]:
             return None
         tfd = self.tailf.fileno()
         szhdr = os.read(tfd, self.szhdr_size)
@@ -159,31 +161,31 @@
         self.headf.close()
         self.tailf.close()
         self._saveinfo(self.info)
         if len(self) == 0:
             self._cleanup()
 
     def __len__(self) -> int:
-        return self.info["size"]
+        return cast(int, self.info["size"])
 
-    def _loadinfo(self, chunksize: int) -> dict:
+    def _loadinfo(self, chunksize: int) -> Dict[str, Any]:
         infopath = self._infopath()
         if os.path.exists(infopath):
             with open(infopath) as f:
-                info = json.load(f)
+                info = cast(Dict[str, Any], json.load(f))
         else:
             info = {
                 "chunksize": chunksize,
                 "size": 0,
                 "tail": [0, 0, 0],
                 "head": [0, 0],
             }
         return info
 
-    def _saveinfo(self, info: dict) -> None:
+    def _saveinfo(self, info: Dict[str, Any]) -> None:
         with open(self._infopath(), "w") as f:
             json.dump(info, f)
 
     def _infopath(self) -> str:
         return os.path.join(self.path, "info.json")
 
     def _cleanup(self) -> None:
@@ -197,28 +199,29 @@
 class LifoDiskQueue:
     """Persistent LIFO queue."""
 
     SIZE_FORMAT = ">L"
     SIZE_SIZE = struct.calcsize(SIZE_FORMAT)
 
     def __init__(self, path: str) -> None:
+        self.size: int
         self.path = path
         if os.path.exists(path):
             self.f = open(path, "rb+")
             qsize = self.f.read(self.SIZE_SIZE)
             (self.size,) = struct.unpack(self.SIZE_FORMAT, qsize)
             self.f.seek(0, os.SEEK_END)
         else:
             self.f = open(path, "wb+")
             self.f.write(struct.pack(self.SIZE_FORMAT, 0))
             self.size = 0
 
     def push(self, string: bytes) -> None:
         if not isinstance(string, bytes):
-            raise TypeError("Unsupported type: {}".format(type(string).__name__))
+            raise TypeError(f"Unsupported type: {type(string).__name__}")
         self.f.write(string)
         ssize = struct.pack(self.SIZE_FORMAT, len(string))
         self.f.write(ssize)
         self.size += 1
 
     def pop(self) -> Optional[bytes]:
         if not self.size:
@@ -265,37 +268,37 @@
         self._db = sqlite3.Connection(self._path, timeout=60)
         self._db.text_factory = bytes
         with self._db as conn:
             conn.execute(self._sql_create)
 
     def push(self, item: bytes) -> None:
         if not isinstance(item, bytes):
-            raise TypeError("Unsupported type: {}".format(type(item).__name__))
+            raise TypeError(f"Unsupported type: {type(item).__name__}")
         with self._db as conn:
             conn.execute(self._sql_push, (item,))
 
     def pop(self) -> Optional[bytes]:
         with self._db as conn:
             for id_, item in conn.execute(self._sql_pop):
                 conn.execute(self._sql_del, (id_,))
-                return item
+                return cast(bytes, item)
         return None
 
     def peek(self) -> Optional[bytes]:
         with self._db as conn:
             for _, item in conn.execute(self._sql_pop):
-                return item
+                return cast(bytes, item)
         return None
 
     def close(self) -> None:
         size = len(self)
         self._db.close()
         if not size:
             os.remove(self._path)
 
     def __len__(self) -> int:
         with self._db as conn:
-            return next(conn.execute(self._sql_size))[0]
+            return cast(int, next(conn.execute(self._sql_size))[0])
 
 
 class LifoSQLiteQueue(FifoSQLiteQueue):
     _sql_pop = "SELECT id, item FROM queue ORDER BY id DESC LIMIT 1"
```

### Comparing `queuelib-1.6.2/queuelib/rrqueue.py` & `queuelib-1.7.0/queuelib/rrqueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import deque
-from typing import Any, Callable, Hashable, Iterable, List, Optional
+from collections.abc import Hashable
+from typing import Any, Callable, Iterable, List, Optional
 
 from queuelib.queue import BaseQueue
 
 
 class RoundRobinQueue:
     """A round robin queue implemented using multiple internal queues (typically,
     FIFO queues). The internal queue must implement the following methods:
@@ -19,15 +20,19 @@
     queue was previously closed leaving some domain buckets non-empty, those
     domains should be passed in start_domains.
 
     The queue maintains a fifo queue of keys. The key that went last is popped
     first and the next queue for that key is then popped.
     """
 
-    def __init__(self, qfactory: Callable[[Hashable], BaseQueue], start_domains: Iterable[Hashable] = ()) -> None:
+    def __init__(
+        self,
+        qfactory: Callable[[Hashable], BaseQueue],
+        start_domains: Iterable[Hashable] = (),
+    ) -> None:
         self.queues = {}
         self.qfactory = qfactory
         for key in start_domains:
             self.queues[key] = self.qfactory(key)
         self.key_queue = deque(start_domains)
 
     def push(self, obj: Any, key: Hashable) -> None:
```

### Comparing `queuelib-1.6.2/queuelib/tests/__init__.py` & `queuelib-1.7.0/queuelib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `queuelib-1.6.2/queuelib/tests/test_pqueue.py` & `queuelib-1.7.0/queuelib/tests/test_pqueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
+
 from queuelib.pqueue import PriorityQueue
 from queuelib.queue import (
-    FifoMemoryQueue,
-    LifoMemoryQueue,
     FifoDiskQueue,
-    LifoDiskQueue,
+    FifoMemoryQueue,
     FifoSQLiteQueue,
+    LifoDiskQueue,
+    LifoMemoryQueue,
     LifoSQLiteQueue,
 )
 from queuelib.tests import QueuelibTestCase, track_closed
 
 
 class PQueueTestMixin:
     def setUp(self):
@@ -170,29 +171,37 @@
         q2 = PriorityQueue(self.qfactory, startprios=active)
         self.assertEqual(q2.pop(), b"b")
         self.assertEqual(q2.pop(), b"c")
         self.assertEqual(q2.pop(), b"a")
         self.assertEqual(q2.close(), [])
 
 
-class FifoDiskPriorityQueueTest(PQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class FifoDiskPriorityQueueTest(
+    PQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, prio):
         path = os.path.join(self.qdir, str(prio))
         return track_closed(FifoDiskQueue)(path)
 
 
-class LifoDiskPriorityQueueTest(PQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class LifoDiskPriorityQueueTest(
+    PQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, prio):
         path = os.path.join(self.qdir, str(prio))
         return track_closed(LifoDiskQueue)(path)
 
 
-class FifoSQLitePriorityQueueTest(PQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class FifoSQLitePriorityQueueTest(
+    PQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, prio):
         path = os.path.join(self.qdir, str(prio))
         return track_closed(FifoSQLiteQueue)(path)
 
 
-class LifoSQLitePriorityQueueTest(PQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class LifoSQLitePriorityQueueTest(
+    PQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, prio):
         path = os.path.join(self.qdir, str(prio))
         return track_closed(LifoSQLiteQueue)(path)
```

### Comparing `queuelib-1.6.2/queuelib/tests/test_queue.py` & `queuelib-1.7.0/queuelib/tests/test_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import os
 import glob
+import os
 from abc import abstractmethod
+from typing import Any, List, Optional
 from unittest import mock
-from typing import Any, Optional
 
 import pytest
 
 from queuelib.queue import (
     BaseQueue,
-    FifoMemoryQueue,
-    LifoMemoryQueue,
     FifoDiskQueue,
-    LifoDiskQueue,
+    FifoMemoryQueue,
     FifoSQLiteQueue,
+    LifoDiskQueue,
+    LifoMemoryQueue,
     LifoSQLiteQueue,
 )
 from queuelib.tests import QueuelibTestCase
 
 
 class DummyQueue:
     def __init__(self) -> None:
-        self.q = list()  # type: list
+        self.q: List[Any] = []
 
     def push(self, obj: Any) -> None:
         self.q.append(obj)
 
     def pop(self) -> Optional[Any]:
         return self.q.pop() if self.q else None
 
@@ -209,22 +209,23 @@
         self.assertEqual(q.peek(), b"a")
         self.assertEqual(q.peek(), b"a")
         self.assertEqual(q.pop(), b"a")
         self.assertIsNone(q.peek())
 
 
 class PersistentTestMixin:
-
     chunksize = 100000
 
-    @pytest.mark.xfail(reason="Reenable once Scrapy.squeues stops extending from this testsuite")
+    @pytest.mark.xfail(
+        reason="Reenable once Scrapy.squeues stops extending from this testsuite"
+    )
     def test_non_bytes_raises_typeerror(self):
         q = self.queue()
         self.assertRaises(TypeError, q.push, 0)
-        self.assertRaises(TypeError, q.push, u"")
+        self.assertRaises(TypeError, q.push, "")
         self.assertRaises(TypeError, q.push, None)
         self.assertRaises(TypeError, q.push, lambda x: x)
 
     def test_text_in_windows(self):
         e1 = b"\r\n"
         q = self.queue()
         q.push(e1)
@@ -277,15 +278,17 @@
 
 
 class LifoMemoryQueueTest(LifoTestMixin, QueueTestMixin, QueuelibTestCase):
     def queue(self):
         return LifoMemoryQueue()
 
 
-class FifoDiskQueueTest(FifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase):
+class FifoDiskQueueTest(
+    FifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase
+):
     def queue(self):
         return FifoDiskQueue(self.qpath, chunksize=self.chunksize)
 
     def test_not_szhdr(self):
         q = self.queue()
         q.push(b"something")
         empty_file = open(self.tempfilename(), "w+")
@@ -322,15 +325,17 @@
     chunksize = 3
 
 
 class ChunkSize4FifoDiskQueueTest(FifoDiskQueueTest):
     chunksize = 4
 
 
-class LifoDiskQueueTest(LifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase):
+class LifoDiskQueueTest(
+    LifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase
+):
     def queue(self):
         return LifoDiskQueue(self.qpath)
 
     def test_file_size_shrinks(self):
         """Test size of queue file shrinks when popping items"""
         q = self.queue()
         q.push(b"a")
@@ -339,15 +344,19 @@
         size = os.path.getsize(self.qpath)
         q = self.queue()
         q.pop()
         q.close()
         assert os.path.getsize(self.qpath), size
 
 
-class FifoSQLiteQueueTest(FifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase):
+class FifoSQLiteQueueTest(
+    FifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase
+):
     def queue(self):
         return FifoSQLiteQueue(self.qpath)
 
 
-class LifoSQLiteQueueTest(LifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase):
+class LifoSQLiteQueueTest(
+    LifoTestMixin, PersistentTestMixin, QueueTestMixin, QueuelibTestCase
+):
     def queue(self):
         return LifoSQLiteQueue(self.qpath)
```

### Comparing `queuelib-1.6.2/queuelib/tests/test_rrqueue.py` & `queuelib-1.7.0/queuelib/tests/test_rrqueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 
-from queuelib.rrqueue import RoundRobinQueue
 from queuelib.queue import (
-    FifoMemoryQueue,
-    LifoMemoryQueue,
     FifoDiskQueue,
-    LifoDiskQueue,
+    FifoMemoryQueue,
     FifoSQLiteQueue,
+    LifoDiskQueue,
+    LifoMemoryQueue,
     LifoSQLiteQueue,
 )
-
+from queuelib.rrqueue import RoundRobinQueue
 from queuelib.tests import QueuelibTestCase, track_closed
 
 
 class RRQueueTestMixin:
     def setUp(self):
         super().setUp()
         self.q = RoundRobinQueue(self.qfactory)
@@ -123,33 +122,41 @@
         self.assertEqual(self.q.pop(), b"a")
         self.assertEqual(self.q.pop(), b"b")
         self.assertEqual(self.q.pop(), b"c")
         self.assertEqual(self.q.pop(), None)
         self.assertEqual(self.q.close(), [])
 
 
-class FifoDiskRRQueueTest(RRQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class FifoDiskRRQueueTest(
+    RRQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, key):
         path = os.path.join(self.qdir, str(key))
         return track_closed(FifoDiskQueue)(path)
 
 
-class LifoDiskRRQueueTest(RRQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class LifoDiskRRQueueTest(
+    RRQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, key):
         path = os.path.join(self.qdir, str(key))
         return track_closed(LifoDiskQueue)(path)
 
 
-class FifoSQLiteRRQueueTest(RRQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class FifoSQLiteRRQueueTest(
+    RRQueueTestMixin, FifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, key):
         path = os.path.join(self.qdir, str(key))
         return track_closed(FifoSQLiteQueue)(path)
 
 
-class LifoSQLiteRRQueueTest(RRQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase):
+class LifoSQLiteRRQueueTest(
+    RRQueueTestMixin, LifoTestMixin, DiskTestMixin, QueuelibTestCase
+):
     def qfactory(self, key):
         path = os.path.join(self.qdir, str(key))
         return track_closed(LifoSQLiteQueue)(path)
 
 
 class RRQueueStartDomainsTestMixin:
     def setUp(self):
```

### Comparing `queuelib-1.6.2/queuelib.egg-info/PKG-INFO` & `queuelib-1.7.0/queuelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: queuelib
-Version: 1.6.2
+Version: 1.7.0
 Summary: Collection of persistent (disk-based) and non-persistent (memory-based) queues
 Home-page: https://github.com/scrapy/queuelib
 Author: Scrapy project
 Author-email: info@scrapy.org
 License: BSD
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 queuelib
 ========
 
 .. image:: https://img.shields.io/pypi/v/queuelib.svg
@@ -207,9 +208,7 @@
 
 This software follows `Semantic Versioning`_
 
 .. _Scrapy framework: http://scrapy.org
 .. _scrapy-users: http://groups.google.com/group/scrapy-users
 .. _Semantic Versioning: http://semver.org/
 .. _nosetests: https://nose.readthedocs.org/en/latest/
-
-
```

### Comparing `queuelib-1.6.2/setup.py` & `queuelib-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 setup(
     name="queuelib",
-    version="1.6.2",
+    version="1.7.0",
     license="BSD",
     description="Collection of persistent (disk-based) and non-persistent (memory-based) queues",
     long_description=open("README.rst").read(),
+    long_description_content_type="text/x-rst",
     author="Scrapy project",
     author_email="info@scrapy.org",
     url="https://github.com/scrapy/queuelib",
     packages=find_packages(),
+    package_data={
+        "queuelib": ["py.typed"],
+    },
     platforms=["Any"],
-    python_requires=">=3.5",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
```

