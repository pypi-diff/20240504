# Comparing `tmp/jeepito-0.2.0.tar.gz` & `tmp/jeepito-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeepito-0.2.0.tar", max compression
+gzip compressed data, was "jeepito-0.2.1.tar", max compression
```

## Comparing `jeepito-0.2.0.tar` & `jeepito-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,16 @@
--rw-r--r--   0        0        0     1504 2023-06-24 06:50:30.635595 jeepito-0.2.0/LICENSE
--rw-r--r--   0        0        0     1326 2024-01-04 17:34:02.922089 jeepito-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2229 2023-09-16 13:07:18.310031 jeepito-0.2.0/src/jeepito/__init__.py
--rw-r--r--   0        0        0     2326 2023-08-20 10:13:30.243516 jeepito-0.2.0/src/jeepito/domain/model.py
--rw-r--r--   0        0        0        0 2024-01-04 17:31:42.988077 jeepito-0.2.0/src/jeepito/messagebus/__init__.py
--rw-r--r--   0        0        0     2326 2023-09-16 12:41:03.762580 jeepito-0.2.0/src/jeepito/messagebus/domain/model.py
--rw-r--r--   0        0        0     1906 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_async/eventstream.py
--rw-r--r--   0        0        0     5616 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_async/registry.py
--rw-r--r--   0        0        0     2090 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_async/repository.py
--rw-r--r--   0        0        0     4298 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_async/unit_of_work.py
--rw-r--r--   0        0        0     1877 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_sync/eventstream.py
--rw-r--r--   0        0        0     5571 2024-01-04 17:21:38.912037 jeepito-0.2.0/src/jeepito/messagebus/service/_sync/registry.py
--rw-r--r--   0        0        0     2047 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_sync/repository.py
--rw-r--r--   0        0        0     4191 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/messagebus/service/_sync/unit_of_work.py
--rw-r--r--   0        0        0      966 2023-09-16 12:59:19.052641 jeepito-0.2.0/src/jeepito/messagebus/service/eventstream.py
--rw-r--r--   0        0        0        0 2023-06-24 06:50:30.678927 jeepito-0.2.0/src/jeepito/py.typed
--rw-r--r--   0        0        0     1906 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/service/_async/eventstream.py
--rw-r--r--   0        0        0     5616 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/service/_async/registry.py
--rw-r--r--   0        0        0     2146 2024-01-04 17:22:41.665602 jeepito-0.2.0/src/jeepito/service/_async/repository.py
--rw-r--r--   0        0        0     4298 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/service/_async/unit_of_work.py
--rw-r--r--   0        0        0     1877 2024-01-04 17:33:58.725403 jeepito-0.2.0/src/jeepito/service/_sync/eventstream.py
--rw-r--r--   0        0        0     5571 2024-01-04 17:33:58.728736 jeepito-0.2.0/src/jeepito/service/_sync/registry.py
--rw-r--r--   0        0        0     2103 2024-01-04 17:33:58.732069 jeepito-0.2.0/src/jeepito/service/_sync/repository.py
--rw-r--r--   0        0        0     4191 2024-01-04 17:33:58.732069 jeepito-0.2.0/src/jeepito/service/_sync/unit_of_work.py
--rw-r--r--   0        0        0      966 2023-09-16 12:59:19.115974 jeepito-0.2.0/src/jeepito/service/eventstream.py
--rw-r--r--   0        0        0     1084 2023-09-16 12:59:19.042641 jeepito-0.2.0/src/jeepito/typing.py
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 jeepito-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-06-24 06:50:30.635595 jeepito-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1326 2024-05-03 22:33:51.271497 jeepito-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2387 2024-05-03 22:29:48.610365 jeepito-0.2.1/src/jeepito/__init__.py
+-rw-r--r--   0        0        0     2326 2023-08-20 10:13:30.243516 jeepito-0.2.1/src/jeepito/domain/model.py
+-rw-r--r--   0        0        0        0 2023-06-24 06:50:30.678927 jeepito-0.2.1/src/jeepito/py.typed
+-rw-r--r--   0        0        0     1906 2024-05-03 22:27:22.236348 jeepito-0.2.1/src/jeepito/service/_async/eventstream.py
+-rw-r--r--   0        0        0     5616 2024-05-03 22:27:22.239682 jeepito-0.2.1/src/jeepito/service/_async/registry.py
+-rw-r--r--   0        0        0     2146 2024-05-03 22:27:22.239682 jeepito-0.2.1/src/jeepito/service/_async/repository.py
+-rw-r--r--   0        0        0     4298 2024-05-03 22:27:22.239682 jeepito-0.2.1/src/jeepito/service/_async/unit_of_work.py
+-rw-r--r--   0        0        0     1877 2024-05-03 22:33:45.614804 jeepito-0.2.1/src/jeepito/service/_sync/eventstream.py
+-rw-r--r--   0        0        0     5571 2024-05-03 22:33:46.124806 jeepito-0.2.1/src/jeepito/service/_sync/registry.py
+-rw-r--r--   0        0        0     2103 2024-05-03 22:33:45.618137 jeepito-0.2.1/src/jeepito/service/_sync/repository.py
+-rw-r--r--   0        0        0     4191 2024-05-03 22:33:45.621470 jeepito-0.2.1/src/jeepito/service/_sync/unit_of_work.py
+-rw-r--r--   0        0        0      966 2024-05-03 22:27:22.239682 jeepito-0.2.1/src/jeepito/service/eventstream.py
+-rw-r--r--   0        0        0     1084 2024-01-04 19:47:58.573375 jeepito-0.2.1/src/jeepito/typing.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 jeepito-0.2.1/PKG-INFO
```

### Comparing `jeepito-0.2.0/LICENSE` & `jeepito-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/pyproject.toml` & `jeepito-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 authors = ["Guillaume Gauvrit <guillaume@gauvr.it>"]
 description = "A message bus library"
 name = "Jeepito"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.pyright]
 include = ["src"]
 typeCheckingMode = "strict"
 
 [[tool.mypy.overrides]]
 disallow_any_generics = true
```

### Comparing `jeepito-0.2.0/src/jeepito/__init__.py` & `jeepito-0.2.1/src/jeepito/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 
 from pydantic import Field
 
 from .domain.model import Command, Event, Message, Metadata, Model
 from .service._async.eventstream import (
     AsyncAbstractEventstreamTransport,
     AsyncEventstreamPublisher,
+    AsyncSinkholeEventstreamTransport,
 )
 from .service._async.registry import AsyncMessageBus, async_listen
 from .service._async.repository import AsyncAbstractRepository
 from .service._async.unit_of_work import (
     AsyncAbstractUnitOfWork,
     AsyncEventstoreAbstractRepository,
     AsyncSinkholeEventstoreRepository,
     AsyncUnitOfWorkTransaction,
 )
 from .service._sync.eventstream import (
     SyncAbstractEventstreamTransport,
     SyncEventstreamPublisher,
+    SyncSinkholeEventstreamTransport,
 )
 from .service._sync.registry import SyncMessageBus, sync_listen
 from .service._sync.repository import SyncAbstractRepository
 from .service._sync.unit_of_work import (
     SyncAbstractUnitOfWork,
     SyncEventstoreAbstractRepository,
     SyncSinkholeEventstoreRepository,
@@ -67,11 +69,13 @@
     "async_listen",
     "sync_listen",
     "AsyncMessageBus",
     "SyncMessageBus",
     # Eventstream
     "AbstractMessageSerializer",
     "AsyncAbstractEventstreamTransport",
+    "AsyncSinkholeEventstreamTransport",
     "AsyncEventstreamPublisher",
     "SyncAbstractEventstreamTransport",
+    "SyncSinkholeEventstreamTransport",
     "SyncEventstreamPublisher",
 ]
```

### Comparing `jeepito-0.2.0/src/jeepito/domain/model.py` & `jeepito-0.2.1/src/jeepito/domain/model.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_async/eventstream.py` & `jeepito-0.2.1/src/jeepito/service/_async/eventstream.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_async/registry.py` & `jeepito-0.2.1/src/jeepito/service/_async/registry.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_async/repository.py` & `jeepito-0.2.1/src/jeepito/service/_async/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 TModel_contra = TypeVar("TModel_contra", bound=Model, contravariant=True)
 
 
 class AsyncAbstractRepository(abc.ABC, Generic[TModel_contra]):
     """Abstract Base Classe for Repository pattern."""
 
+    def __init__(self) -> None:
+        self.seen = []
+
     seen: MutableSequence[TModel_contra]
 
 
 class AsyncEventstoreAbstractRepository(abc.ABC):
     def __init__(self, publisher: Optional[AsyncEventstreamPublisher] = None) -> None:
         self.publisher = publisher
         self.stream_buffer: MutableSequence[Message] = []
```

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_async/unit_of_work.py` & `jeepito-0.2.1/src/jeepito/service/_async/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_sync/eventstream.py` & `jeepito-0.2.1/src/jeepito/service/_sync/eventstream.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_sync/registry.py` & `jeepito-0.2.1/src/jeepito/service/_sync/registry.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_sync/repository.py` & `jeepito-0.2.1/src/jeepito/service/_sync/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 TModel_contra = TypeVar("TModel_contra", bound=Model, contravariant=True)
 
 
 class SyncAbstractRepository(abc.ABC, Generic[TModel_contra]):
     """Abstract Base Classe for Repository pattern."""
 
+    def __init__(self) -> None:
+        self.seen = []
+
     seen: MutableSequence[TModel_contra]
 
 
 class SyncEventstoreAbstractRepository(abc.ABC):
     def __init__(self, publisher: Optional[SyncEventstreamPublisher] = None) -> None:
         self.publisher = publisher
         self.stream_buffer: MutableSequence[Message] = []
```

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/_sync/unit_of_work.py` & `jeepito-0.2.1/src/jeepito/service/_sync/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/messagebus/service/eventstream.py` & `jeepito-0.2.1/src/jeepito/service/eventstream.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/src/jeepito/typing.py` & `jeepito-0.2.1/src/jeepito/typing.py`

 * *Files identical despite different names*

### Comparing `jeepito-0.2.0/PKG-INFO` & `jeepito-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jeepito
-Version: 0.2.0
+Version: 0.2.1
 Summary: A message bus library
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

