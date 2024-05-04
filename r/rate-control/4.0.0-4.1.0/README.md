# Comparing `tmp/rate_control-4.0.0.tar.gz` & `tmp/rate_control-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_control-4.0.0.tar", max compression
+gzip compressed data, was "rate_control-4.1.0.tar", max compression
```

## Comparing `rate_control-4.0.0.tar` & `rate_control-4.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1101 2024-04-30 11:59:05.622581 rate_control-4.0.0/LICENSE
--rw-r--r--   0        0        0     3822 2024-04-30 11:59:05.622581 rate_control-4.0.0/README.rst
--rw-r--r--   0        0        0     2872 2024-04-30 11:59:09.402567 rate_control-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      582 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/__init__.py
--rw-r--r--   0        0        0     3865 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_bucket_group.py
--rw-r--r--   0        0        0      267 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/__init__.py
--rw-r--r--   0        0        0      344 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/__init__.py
--rw-r--r--   0        0        0     2025 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_abc.py
--rw-r--r--   0        0        0     2539 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_base_rate.py
--rw-r--r--   0        0        0      825 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_capacity_updating.py
--rw-r--r--   0        0        0      948 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_token_based.py
--rw-r--r--   0        0        0      997 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_base/_windowed.py
--rw-r--r--   0        0        0     1074 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_fixed_window_counter.py
--rw-r--r--   0        0        0     1412 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_leaky_bucket.py
--rw-r--r--   0        0        0      679 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_buckets/_sliding_window_log.py
--rw-r--r--   0        0        0      179 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/__init__.py
--rw-r--r--   0        0        0     1434 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_abc.py
--rw-r--r--   0        0        0     4580 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_bucket_based.py
--rw-r--r--   0        0        0     1172 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_rate_limiter.py
--rw-r--r--   0        0        0     8930 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_controllers/_scheduler.py
--rw-r--r--   0        0        0      111 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_enums/__init__.py
--rw-r--r--   0        0        0      262 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_enums/_duration.py
--rw-r--r--   0        0        0      350 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_enums/_priority.py
--rw-r--r--   0        0        0      297 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_errors.py
--rw-r--r--   0        0        0      105 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/__init__.py
--rw-r--r--   0        0        0      781 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_mk_repr.py
--rw-r--r--   0        0        0      492 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_protocols.py
--rw-r--r--   0        0        0     1502 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_request.py
--rw-r--r--   0        0        0     1709 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/_helpers/_validation.py
--rw-r--r--   0        0        0        0 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/py.typed
--rw-r--r--   0        0        0      202 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/__init__.py
--rw-r--r--   0        0        0     1560 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_abc.py
--rw-r--r--   0        0        0     1365 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_fifo.py
--rw-r--r--   0        0        0     1340 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_lifo.py
--rw-r--r--   0        0        0     1687 2024-04-30 11:59:05.626581 rate_control-4.0.0/rate_control/queues/_priority.py
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rate_control-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-05-04 07:19:02.649495 rate_control-4.1.0/LICENSE
+-rw-r--r--   0        0        0     3849 2024-05-04 07:19:02.649495 rate_control-4.1.0/README.rst
+-rw-r--r--   0        0        0     2828 2024-05-04 07:19:06.373528 rate_control-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      620 2024-05-04 07:19:02.649495 rate_control-4.1.0/rate_control/__init__.py
+-rw-r--r--   0        0        0     3858 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_bucket_group.py
+-rw-r--r--   0        0        0      267 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_abc.py
+-rw-r--r--   0        0        0     2539 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_base_rate.py
+-rw-r--r--   0        0        0      744 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_capacity_updating.py
+-rw-r--r--   0        0        0      948 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_token_based.py
+-rw-r--r--   0        0        0      997 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_base/_windowed.py
+-rw-r--r--   0        0        0     1074 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_fixed_window_counter.py
+-rw-r--r--   0        0        0     1412 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_leaky_bucket.py
+-rw-r--r--   0        0        0      679 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_buckets/_sliding_window_log.py
+-rw-r--r--   0        0        0      246 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/__init__.py
+-rw-r--r--   0        0        0     1434 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_abc.py
+-rw-r--r--   0        0        0     4580 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_bucket_based.py
+-rw-r--r--   0        0        0     1632 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_noop_controller.py
+-rw-r--r--   0        0        0     1172 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_rate_limiter.py
+-rw-r--r--   0        0        0     8333 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_controllers/_scheduler.py
+-rw-r--r--   0        0        0      111 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_enums/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_enums/_duration.py
+-rw-r--r--   0        0        0      350 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_enums/_priority.py
+-rw-r--r--   0        0        0      297 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_errors.py
+-rw-r--r--   0        0        0      105 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/__init__.py
+-rw-r--r--   0        0        0      781 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_mk_repr.py
+-rw-r--r--   0        0        0      492 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_protocols.py
+-rw-r--r--   0        0        0     1502 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_request.py
+-rw-r--r--   0        0        0     1673 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/_helpers/_validation.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/py.typed
+-rw-r--r--   0        0        0      202 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/__init__.py
+-rw-r--r--   0        0        0     1559 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_abc.py
+-rw-r--r--   0        0        0     1365 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_fifo.py
+-rw-r--r--   0        0        0     1340 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_lifo.py
+-rw-r--r--   0        0        0     1687 2024-05-04 07:19:02.653495 rate_control-4.1.0/rate_control/queues/_priority.py
+-rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 rate_control-4.1.0/PKG-INFO
```

### Comparing `rate_control-4.0.0/LICENSE` & `rate_control-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/README.rst` & `rate_control-4.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 ============
 
 * `Rate limiting <https://rate-control.readthedocs.io/en/latest/quickstart.html#basic-usage>`_
 * `Scheduling requests <https://rate-control.readthedocs.io/en/latest/scheduling.html>`_
 * `Request synchronization <https://rate-control.readthedocs.io/en/latest/synchronization.html>`_
 * `Request prioritization <https://rate-control.readthedocs.io/en/latest/scheduling.html#request-prioritization>`_
 * `Chaining buckets <https://rate-control.readthedocs.io/en/latest/bucket-groups.html>`_
-* Support for both asyncio_ and Trio_, through AnyIO_
+* Supports task cancellation
+* Supports both asyncio_ and Trio_, through AnyIO_
 
 .. _AnyIO: https://github.com/agronholm/anyio
 .. _asyncio: https://docs.python.org/3/library/asyncio.html
 .. _Trio: https://github.com/python-trio/trio
 
 Contributing
 ============
```

### Comparing `rate_control-4.0.0/pyproject.toml` & `rate_control-4.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rate-control"
-version = "4.0.0"
+version = "4.1.0"
 description = "Versatile rate controlling in Python"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/corentin-regent/rate-control"
 repository = "https://github.com/corentin-regent/rate-control"
 documentation = "https://rate-control.readthedocs.io/"
@@ -44,15 +44,14 @@
 typing_extensions = {version = "^4.4.0", python = "<3.12"}
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-anyio = {version = "*", extras = ["trio"]}
 mypy = "^1.6"
 ruff = "^0.4.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -63,15 +62,15 @@
 pytest-subtests = "^0.11.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 enum_tools = {version = "^0.11.0", extras=["sphinx"]}
-furo = "==2024.01.29"
+furo = "==2024.04.27"
 sphinx = "^7.0.0"
 sphinx-autodoc-typehints = "^2.0.0"
 sphinx-tabs = "^3.4.2"
 
 
 [tool.coverage.run]
 branch = true
```

### Comparing `rate_control-4.0.0/rate_control/__init__.py` & `rate_control-4.1.0/rate_control/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 __all__ = [
     'Bucket',
     'BucketGroup',
     'Duration',
     'FixedWindowCounter',
     'LeakyBucket',
+    'NoopController',
     'Priority',
     'RateController',
     'RateLimit',
     'RateLimiter',
     'ReachedMaxPending',
     'Scheduler',
     'SlidingWindowLog',
 ]
 
 from rate_control._bucket_group import BucketGroup
 from rate_control._buckets import Bucket, FixedWindowCounter, LeakyBucket, SlidingWindowLog
-from rate_control._controllers import RateController, RateLimiter, Scheduler
+from rate_control._controllers import NoopController, RateController, RateLimiter, Scheduler
 from rate_control._enums import Duration, Priority
 from rate_control._errors import RateLimit, ReachedMaxPending
```

### Comparing `rate_control-4.0.0/rate_control/_bucket_group.py` & `rate_control-4.1.0/rate_control/_bucket_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,17 @@
     async def __aenter__(self) -> Self:
         self._stack = await AsyncExitStack().__aenter__()
         self._task_group = await self._stack.enter_async_context(create_task_group())
         await self._init_buckets()
         return self
 
     @override
-    async def __aexit__(self, *exc_info: Any) -> bool:
+    async def __aexit__(self, *exc_info: Any) -> None:
         self._task_group.cancel_scope.cancel()
-        return await self._stack.__aexit__(*exc_info)
+        await self._stack.__aexit__(*exc_info)
 
     @override
     def __iter__(self) -> Iterator[Bucket]:
         return iter(self._buckets)
 
     async def _init_buckets(self) -> None:
         for bucket in self._buckets:
```

### Comparing `rate_control-4.0.0/rate_control/_buckets/_base/_abc.py` & `rate_control-4.1.0/rate_control/_buckets/_base/_abc.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 ]
 
 import sys
 from abc import ABC, abstractmethod
 from typing import Any, Optional
 
 from rate_control._errors import RateLimit
-from rate_control._helpers import mk_repr
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if sys.version_info >= (3, 12):
-    from typing import override
+    pass
 else:
-    from typing_extensions import override
+    pass
 
 
 class Bucket(ABC):
     """Abstract base class for buckets."""
 
     __slots__ = ()
 
@@ -34,18 +33,14 @@
 
     async def __aexit__(self, *_: Any) -> Optional[bool]:
         """Exit the bucket context.
 
         It may for example cancel internal background tasks.
         """
 
-    @override
-    def __repr__(self) -> str:
-        return mk_repr(self)
-
     @abstractmethod
     async def wait_for_refill(self) -> None:
         """Wait until some tokens are replenished."""
 
     @abstractmethod
     def can_acquire(self, tokens: float) -> bool:
         """Whether the given amount of tokens can be acquired.
```

### Comparing `rate_control-4.0.0/rate_control/_buckets/_base/_base_rate.py` & `rate_control-4.1.0/rate_control/_buckets/_base/_base_rate.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_buckets/_base/_capacity_updating.py` & `rate_control-4.1.0/rate_control/_buckets/_base/_capacity_updating.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,11 @@
     def update_capacity(self, new_capacity: float) -> None:
         """Update the bucket's token capacity.
 
         Changes take effect instantly, and the amount of remaining tokens is updated accordingly.
 
         Args:
             new_capacity: The new token capacity of the bucket.
-
-        Raises:
-            ValueError: Negative or zero capacity was provided.
         """
         validate_capacity(new_capacity)
         self._tokens += new_capacity - self._capacity
         self._capacity = new_capacity
```

### Comparing `rate_control-4.0.0/rate_control/_buckets/_base/_token_based.py` & `rate_control-4.1.0/rate_control/_buckets/_base/_token_based.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_buckets/_base/_windowed.py` & `rate_control-4.1.0/rate_control/_buckets/_base/_windowed.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_buckets/_fixed_window_counter.py` & `rate_control-4.1.0/rate_control/_buckets/_fixed_window_counter.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_buckets/_leaky_bucket.py` & `rate_control-4.1.0/rate_control/_buckets/_leaky_bucket.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_buckets/_sliding_window_log.py` & `rate_control-4.1.0/rate_control/_buckets/_sliding_window_log.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_controllers/_abc.py` & `rate_control-4.1.0/rate_control/_controllers/_abc.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_controllers/_bucket_based.py` & `rate_control-4.1.0/rate_control/_controllers/_bucket_based.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_controllers/_rate_limiter.py` & `rate_control-4.1.0/rate_control/_controllers/_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_controllers/_scheduler.py` & `rate_control-4.1.0/rate_control/_controllers/_scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 __all__ = [
     'Scheduler',
 ]
 
 import sys
-from contextlib import asynccontextmanager, contextmanager, suppress
+from contextlib import asynccontextmanager, suppress
 from typing import Any, NoReturn, Optional
 
 from anyio import create_task_group, get_cancelled_exc_class
 from anyio.lowlevel import checkpoint
 
 from rate_control._buckets import Bucket
 from rate_control._controllers._bucket_based import BucketBasedRateController
 from rate_control._enums import Priority
 from rate_control._errors import RateLimit, ReachedMaxPending
 from rate_control._helpers import Request, mk_repr
 from rate_control._helpers._validation import validate_max_pending
 from rate_control.queues import PriorityQueue, Queue
 
 if sys.version_info >= (3, 9):
-    from collections.abc import AsyncIterator, Callable, Iterator
+    from collections.abc import AsyncIterator, Callable
 else:
-    from typing import AsyncIterator, Callable, Iterator
+    from typing import AsyncIterator, Callable
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if sys.version_info >= (3, 12):
@@ -32,15 +32,15 @@
 else:
     from typing_extensions import override
 
 
 class Scheduler(BucketBasedRateController):
     """Rate controller that schedules requests for later processing."""
 
-    __slots__ = ('_is_processing_requests', '_max_pending', '_pending_requests', '_queues', '_task_group')
+    __slots__ = ('_max_pending', '_pending_requests', '_queues', '_task_group')
 
     def __init__(
         self,
         *buckets: Bucket,
         should_enter_context: bool = True,
         max_concurrency: Optional[int] = None,
         max_pending: Optional[int] = None,
@@ -61,15 +61,14 @@
                 Defaults to :class:`.PriorityQueue`: requests are processed by ascending weight.
         """
         super().__init__(*buckets, should_enter_context=should_enter_context, max_concurrency=max_concurrency, **kwargs)
         validate_max_pending(max_pending)
         self._max_pending = max_pending
         self._pending_requests = 0
         self._queues = [queue_factory() for _ in Priority]
-        self._is_processing_requests = False
 
     @override
     async def __aenter__(self) -> Self:
         await super().__aenter__()
         self._task_group = await create_task_group().__aenter__()
         if self._bucket is not None:
             self._task_group.start_soon(self._listen_to_refills)
@@ -142,39 +141,24 @@
         if self._bucket is not None:
             self._bucket.acquire(tokens)
         with self._hold_concurrency():
             yield
 
     @override
     def _on_concurrency_release(self) -> None:
-        if self._max_concurrency is not None and self._concurrent_requests < self._max_concurrency:
+        if self._max_concurrency is not None and self._concurrent_requests == self._max_concurrency - 1:
             self._task_group.start_soon(self._process_queued_requests)
 
     async def _process_queued_requests(self) -> None:
-        """Pop and start queued requests while it is possible."""
-        if not self._is_processing_requests:
-            with self._hold_request_processing():
-                await self._process_queues()
-
-    @contextmanager
-    def _hold_request_processing(self) -> Iterator[None]:
-        self._is_processing_requests = True
-        try:
-            yield
-        finally:
-            self._is_processing_requests = False
-
-    async def _process_queues(self) -> None:
         while True:
             try:
                 queue = next(queue for queue in filter(None, self._queues) if self.can_acquire(queue.head().cost))
             except StopIteration:
                 break
-            else:
-                await self._process_next_request(queue)
+            await self._process_next_request(queue)
 
     async def _process_next_request(self, queue: Queue[Request]) -> None:
         """Fire the next request from the queue and wait until the underlying tokens are acquired.
 
         Tokens are not acquired directly in this method,
         in order to support request cancellation.
         """
```

### Comparing `rate_control-4.0.0/rate_control/_helpers/_mk_repr.py` & `rate_control-4.1.0/rate_control/_helpers/_mk_repr.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/_helpers/_request.py` & `rate_control-4.1.0/rate_control/_helpers/_request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     __slots__ = ('_ack_event', 'cost', '_validation_event')
 
     def __init__(self, cost: float, **kwargs: Any) -> None:
         """
         Args:
             cost: The number of tokens requested.
         """
+        super().__init__(**kwargs)
         self.cost = cost
         self._validation_event = Event()
         self._ack_event = Event()
-        super().__init__(**kwargs)
 
     @override
     def __lt__(self, other: Self) -> bool:
         """Comparison operator so that requests can be placed
         in a priority queue and processed by ascending cost.
         """
         return self.cost < other.cost
```

### Comparing `rate_control-4.0.0/rate_control/_helpers/_validation.py` & `rate_control-4.1.0/rate_control/_helpers/_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 __all__ = [
     'validate_capacity',
     'validate_delay',
     'validate_max_concurrency',
     'validate_max_pending',
     'validate_tokens',
 ]
```

### Comparing `rate_control-4.0.0/rate_control/queues/_abc.py` & `rate_control-4.1.0/rate_control/queues/_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Generic, TypeVar
 
 if sys.version_info >= (3, 12):
     from typing import override
 else:
     from typing_extensions import override
 
-
 _T = TypeVar('_T')
 
 
 class Queue(ABC, Generic[_T]):
     """Abstract class for representing a queue."""
 
     __slots__ = ()
```

### Comparing `rate_control-4.0.0/rate_control/queues/_fifo.py` & `rate_control-4.1.0/rate_control/queues/_fifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/queues/_lifo.py` & `rate_control-4.1.0/rate_control/queues/_lifo.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/rate_control/queues/_priority.py` & `rate_control-4.1.0/rate_control/queues/_priority.py`

 * *Files identical despite different names*

### Comparing `rate_control-4.0.0/PKG-INFO` & `rate_control-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-control
-Version: 4.0.0
+Version: 4.1.0
 Summary: Versatile rate controlling in Python
 Home-page: https://github.com/corentin-regent/rate-control
 License: MIT
 Keywords: async,rate limit,schedule,throttle,token bucket
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -51,15 +51,16 @@
 ============
 
 * `Rate limiting <https://rate-control.readthedocs.io/en/latest/quickstart.html#basic-usage>`_
 * `Scheduling requests <https://rate-control.readthedocs.io/en/latest/scheduling.html>`_
 * `Request synchronization <https://rate-control.readthedocs.io/en/latest/synchronization.html>`_
 * `Request prioritization <https://rate-control.readthedocs.io/en/latest/scheduling.html#request-prioritization>`_
 * `Chaining buckets <https://rate-control.readthedocs.io/en/latest/bucket-groups.html>`_
-* Support for both asyncio_ and Trio_, through AnyIO_
+* Supports task cancellation
+* Supports both asyncio_ and Trio_, through AnyIO_
 
 .. _AnyIO: https://github.com/agronholm/anyio
 .. _asyncio: https://docs.python.org/3/library/asyncio.html
 .. _Trio: https://github.com/python-trio/trio
 
 Contributing
 ============
```

