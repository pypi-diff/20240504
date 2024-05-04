# Comparing `tmp/hat_aio-0.7.8-cp310.cp311-none-any.whl.zip` & `tmp/hat_aio-0.7.9-cp310.cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,12 @@
-Zip file size: 14841 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1225 b- defN 23-Mar-23 19:16 hat/aio/__init__.py
--rw-r--r--  2.0 unx     2781 b- defN 23-Jun-22 22:49 hat/aio/executor.py
--rw-r--r--  2.0 unx     6887 b- defN 23-Jun-22 22:51 hat/aio/group.py
--rw-r--r--  2.0 unx     8928 b- defN 23-Jun-22 23:01 hat/aio/misc.py
--rw-r--r--  2.0 unx     6139 b- defN 23-Jun-22 23:02 hat/aio/queue.py
--rw-r--r--  2.0 unx     1788 b- defN 23-Jun-22 23:04 hat/aio/wait.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2214 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/METADATA
--rw-r--r--  2.0 unx      114 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/zip-safe
--rw-rw-r--  2.0 unx      915 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/RECORD
-12 files, 42354 bytes uncompressed, 13325 bytes compressed:  68.5%
+Zip file size: 14623 bytes, number of entries: 10
+?rw-------  2.0 unx     8979 b- defN 23-Dec-14 23:41 hat/aio/misc.py
+?rw-------  2.0 unx     1796 b- defN 23-Dec-14 23:41 hat/aio/wait.py
+?rw-------  2.0 unx     1225 b- defN 23-Dec-14 23:41 hat/aio/__init__.py
+?rw-------  2.0 unx     6883 b- defN 23-Dec-14 23:41 hat/aio/group.py
+?rw-------  2.0 unx     3147 b- defN 23-Dec-14 23:41 hat/aio/executor.py
+?rw-------  2.0 unx     6172 b- defN 23-Dec-14 23:41 hat/aio/queue.py
+?rw-------  2.0 unx    11358 b- defN 23-Dec-14 23:41 hat_aio-0.7.9.dist-info/LICENSE
+?rw-------  2.0 unx     2475 b- defN 23-Dec-14 23:41 hat_aio-0.7.9.dist-info/METADATA
+?rw-------  2.0 unx       98 b- defN 23-Dec-14 23:41 hat_aio-0.7.9.dist-info/WHEEL
+?rw-------  2.0 unx      737 b- defN 23-Dec-14 23:41 hat_aio-0.7.9.dist-info/RECORD
+10 files, 42870 bytes uncompressed, 13397 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,37 +1,31 @@
-Filename: hat/aio/__init__.py
-Comment: 
-
-Filename: hat/aio/executor.py
-Comment: 
-
-Filename: hat/aio/group.py
+Filename: hat/aio/misc.py
 Comment: 
 
-Filename: hat/aio/misc.py
+Filename: hat/aio/wait.py
 Comment: 
 
-Filename: hat/aio/queue.py
+Filename: hat/aio/__init__.py
 Comment: 
 
-Filename: hat/aio/wait.py
+Filename: hat/aio/group.py
 Comment: 
 
-Filename: hat_aio-0.7.8.dist-info/LICENSE
+Filename: hat/aio/executor.py
 Comment: 
 
-Filename: hat_aio-0.7.8.dist-info/METADATA
+Filename: hat/aio/queue.py
 Comment: 
 
-Filename: hat_aio-0.7.8.dist-info/WHEEL
+Filename: hat_aio-0.7.9.dist-info/LICENSE
 Comment: 
 
-Filename: hat_aio-0.7.8.dist-info/top_level.txt
+Filename: hat_aio-0.7.9.dist-info/METADATA
 Comment: 
 
-Filename: hat_aio-0.7.8.dist-info/zip-safe
+Filename: hat_aio-0.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: hat_aio-0.7.8.dist-info/RECORD
+Filename: hat_aio-0.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/aio/executor.py

```diff
@@ -1,21 +1,24 @@
-from typing import Awaitable, Callable, Type
 import asyncio
 import concurrent.futures
 import functools
+import typing
 
 from hat.aio.group import Resource, Group
-from hat.aio.misc import uncancellable
+from hat.aio.misc import call_on_cancel, uncancellable
 
 
 class Executor(Resource):
     """Executor wrapping `asyncio.loop.run_in_executor`.
 
     Wrapped executor is created from `executor_cls` with provided `args`.
 
+    If `wait_futures` is ``True``, executor will be closed once all running
+    tasks finishes.
+
     `log_exceptions` is delegated to `async_group`.
 
     Args:
         args: executor args
         executor_cls: executor class
         log_exceptions: log exceptions
 
@@ -27,41 +30,50 @@
         tid2 = await executor2.spawn(threading.get_ident)
         assert tid1 != tid2
 
     """
 
     def __init__(self,
                  *args,
-                 executor_cls: Type[concurrent.futures.Executor] = concurrent.futures.ThreadPoolExecutor,  # NOQA
-                 log_exceptions: bool = True):
+                 executor_cls: typing.Type[concurrent.futures.Executor] = concurrent.futures.ThreadPoolExecutor,  # NOQA
+                 log_exceptions: bool = True,
+                 wait_futures: bool = True):
+        self._wait_futures = wait_futures
         self._executor = executor_cls(*args)
+        self._loop = asyncio.get_running_loop()
         self._async_group = Group(log_exceptions)
 
+        self.async_group.spawn(call_on_cancel, self._executor.shutdown, False)
+
     @property
     def async_group(self):
         """Async group"""
         return self._async_group
 
     def spawn(self,
-              fn: Callable,
+              fn: typing.Callable,
               *args, **kwargs
               ) -> asyncio.Task:
         """Spawn new task"""
-        return self.async_group.spawn(self._spawn, fn, *args, **kwargs)
+        return self.async_group.spawn(self._spawn, fn, args, kwargs)
 
-    async def _spawn(self, fn, *args, **kwargs):
-        loop = asyncio.get_running_loop()
+    async def _spawn(self, fn, args, kwargs):
         func = functools.partial(fn, *args, **kwargs)
-        return await uncancellable(loop.run_in_executor(self._executor, func))
+        coro = self._loop.run_in_executor(self._executor, func)
+
+        if self._wait_futures:
+            coro = uncancellable(coro)
+
+        return await coro
 
 
 def create_executor(*args,
-                    executor_cls: Type[concurrent.futures.Executor] = concurrent.futures.ThreadPoolExecutor,  # NOQA
+                    executor_cls: typing.Type[concurrent.futures.Executor] = concurrent.futures.ThreadPoolExecutor,  # NOQA
                     loop: asyncio.AbstractEventLoop | None = None
-                    ) -> Callable[..., Awaitable]:
+                    ) -> typing.Callable[..., typing.Awaitable]:
     """Create `asyncio.loop.run_in_executor` wrapper.
 
     Wrapped executor is created from `executor_cls` with provided `args`.
 
     This function returns coroutine that takes a function and its arguments,
     executes the function in executor and returns the result.
```

## hat/aio/group.py

```diff
@@ -1,11 +1,11 @@
-from typing import Awaitable, Callable
 import abc
 import asyncio
 import logging
+import typing
 import warnings
 
 
 mlog: logging.Logger = logging.getLogger(__name__)
 """Module logger"""
 
 
@@ -136,15 +136,15 @@
                             else log_exceptions),
             loop=self._loop)
         child._parent = self
         self._children.add(child)
         return child
 
     def wrap(self,
-             obj: Awaitable
+             obj: typing.Awaitable
              ) -> asyncio.Task:
         """Wrap the awaitable object into a Task and schedule its execution.
         Return the Task object.
 
         Resulting task is shielded and can be canceled only with
         `Group.async_close`.
 
@@ -160,15 +160,15 @@
 
         self._tasks.add(task)
         task.add_done_callback(self._on_task_done)
 
         return asyncio.shield(task)
 
     def spawn(self,
-              fn: Callable[..., Awaitable],
+              fn: typing.Callable[..., typing.Awaitable],
               *args, **kwargs
               ) -> asyncio.Task:
         """Wrap the result of a `fn` into a Task and schedule its execution.
         Return the Task object.
 
         Function `fn` is called with provided `args` and `kwargs`.
         Resulting Task is shielded and can be canceled only with
```

## hat/aio/misc.py

```diff
@@ -1,22 +1,22 @@
-from typing import Any, AsyncIterable, Awaitable, Callable, TypeVar
 import asyncio
 import collections
 import collections.abc
 import contextlib
 import inspect
 import signal
 import sys
+import typing
 
 
-T = TypeVar('T')
+T = typing.TypeVar('T')
 
 
-async def first(xs: AsyncIterable[T],
-                fn: Callable[[T], Any] = lambda _: True,
+async def first(xs: typing.AsyncIterable[T],
+                fn: typing.Callable[[T], typing.Any] = lambda _: True,
                 default: T | None = None
                 ) -> T | None:
     """Return the first element from async iterable that satisfies
     predicate `fn`, or `default` if no such element exists.
 
     Result of predicate `fn` can be of any type. Predicate is satisfied if it's
     return value is truthy.
@@ -42,17 +42,17 @@
     async for i in xs:
         if fn(i):
             return i
 
     return default
 
 
-async def uncancellable(obj: Awaitable,
+async def uncancellable(obj: typing.Awaitable,
                         raise_cancel: bool = True
-                        ) -> Any:
+                        ) -> typing.Any:
     """Uncancellable execution of a awaitable object.
 
     Object is scheduled as task, shielded and its execution cannot be
     interrupted.
 
     If `raise_cancel` is `True` and the object gets canceled,
     `asyncio.CancelledError` is reraised after the Future finishes.
@@ -93,32 +93,32 @@
     if exception:
         raise exception
 
     return task.result()
 
 
 # TODO: AsyncCallable rewrite needed
-class _AsyncCallableType(type(Callable), _root=True):
+class _AsyncCallableType(type(typing.Callable), _root=True):
 
     def __init__(self):
         super().__init__(origin=collections.abc.Callable,
-                         nparams=(..., Awaitable | None))
+                         nparams=(..., typing.Awaitable | None))
 
     def __getitem__(self, params):
         if len(params) == 2:
-            params = params[0], params[1] | Awaitable[params[1]]
+            params = params[0], params[1] | typing.Awaitable[params[1]]
 
         return super().__getitem__(params)
 
 
 AsyncCallable = _AsyncCallableType()
 """Async callable"""
 
 
-async def call(fn: AsyncCallable, *args, **kwargs) -> Any:
+async def call(fn: AsyncCallable, *args, **kwargs) -> typing.Any:
     """Call a function or a coroutine (or other callable object).
 
     Call the `fn` with `args` and `kwargs`. If result of this call is
     awaitable, it is awaited and returned. Otherwise, result is immediately
     returned.
 
     Args:
@@ -151,15 +151,15 @@
 
     if inspect.isawaitable(result):
         result = await result
 
     return result
 
 
-async def call_on_cancel(fn: AsyncCallable, *args, **kwargs) -> Any:
+async def call_on_cancel(fn: AsyncCallable, *args, **kwargs) -> typing.Any:
     """Call a function or a coroutine when canceled.
 
     When canceled, `fn` is called with `args` and `kwargs` by using
     `call` coroutine.
 
     Args:
         fn: function or coroutine
@@ -181,18 +181,18 @@
     """
     with contextlib.suppress(asyncio.CancelledError):
         await asyncio.get_running_loop().create_future()
 
     return await call(fn, *args, *kwargs)
 
 
-async def call_on_done(f: Awaitable,
+async def call_on_done(f: typing.Awaitable,
                        fn: AsyncCallable,
                        *args, **kwargs
-                       ) -> Any:
+                       ) -> typing.Any:
     """Call a function or a coroutine when awaitable is done.
 
     When `f` is done, `fn` is called with `args` and `kwargs` by using
     `call` coroutine.
 
     If this coroutine is canceled before `f` is done, `f` is canceled and `fn`
     is not called.
@@ -246,18 +246,18 @@
         #     return uvloop.EventLoopPolicy()
 
         return asyncio.DefaultEventLoopPolicy()
 
     asyncio.set_event_loop_policy(policy or get_default_policy())
 
 
-def run_asyncio(future: Awaitable, *,
+def run_asyncio(future: typing.Awaitable, *,
                 handle_signals: bool = True,
                 loop: asyncio.AbstractEventLoop | None = None
-                ) -> Any:
+                ) -> typing.Any:
     """Run asyncio loop until the `future` is completed and return the result.
 
     If `handle_signals` is ``True``, SIGINT and SIGTERM handlers are
     temporarily overridden. Instead of raising ``KeyboardInterrupt`` on every
     signal reception, Future is canceled only once. Additional signals are
     ignored. On Windows, SIGBREAK (CTRL_BREAK_EVENT) handler is also
     overridden.
```

## hat/aio/queue.py

```diff
@@ -1,11 +1,11 @@
-from typing import Any
 import asyncio
 import collections
 import contextlib
+import typing
 
 
 class QueueClosedError(Exception):
     """Raised when trying to use a closed queue."""
 
 
 class QueueEmptyError(Exception):
@@ -103,30 +103,30 @@
         if self._closed:
             return
 
         self._closed = True
         self._wakeup_all(self._putters)
         self._wakeup_next(self._getters)
 
-    def get_nowait(self) -> Any:
+    def get_nowait(self) -> typing.Any:
         """Return an item if one is immediately available, else raise
         `QueueEmptyError`.
 
         Raises:
             QueueEmptyError
 
         """
         if self.empty():
             raise QueueEmptyError()
 
         item = self._queue.popleft()
         self._wakeup_next(self._putters)
         return item
 
-    def put_nowait(self, item: Any):
+    def put_nowait(self, item: typing.Any):
         """Put an item into the queue without blocking.
 
         If no free slot is immediately available, raise `QueueFullError`.
 
         Raises:
             QueueFullError
 
@@ -136,15 +136,15 @@
 
         if self.full():
             raise QueueFullError()
 
         self._queue.append(item)
         self._wakeup_next(self._getters)
 
-    async def get(self) -> Any:
+    async def get(self) -> typing.Any:
         """Remove and return an item from the queue.
 
         If queue is empty, wait until an item is available.
 
         Raises:
             QueueClosedError
 
@@ -172,15 +172,15 @@
                     if not self.empty() or self._closed:
                         self._wakeup_next(self._getters)
 
                 raise
 
         return self.get_nowait()
 
-    async def put(self, item: Any):
+    async def put(self, item: typing.Any):
         """Put an item into the queue.
 
         If the queue is full, wait until a free slot is available before adding
         the item.
 
         Raises:
             QueueClosedError
@@ -204,15 +204,15 @@
                 if not self.full() and not putter.cancelled():
                     self._wakeup_next(self._putters)
 
                 raise
 
         return self.put_nowait(item)
 
-    async def get_until_empty(self) -> Any:
+    async def get_until_empty(self) -> typing.Any:
         """Empty the queue and return the last item.
 
         If queue is empty, wait until at least one item is available.
 
         Raises:
             QueueClosedError
 
@@ -220,15 +220,15 @@
         item = await self.get()
 
         while not self.empty():
             item = self.get_nowait()
 
         return item
 
-    def get_nowait_until_empty(self) -> Any:
+    def get_nowait_until_empty(self) -> typing.Any:
         """Empty the queue and return the last item if at least one
         item is immediately available, else raise `QueueEmptyError`.
 
         Raises:
             QueueEmptyError
 
         """
```

## hat/aio/wait.py

```diff
@@ -1,37 +1,37 @@
-from typing import Any, Awaitable
 import asyncio
+import typing
 
 from hat.aio.group import Group
 from hat.aio.misc import call_on_done, uncancellable
 
 
 class CancelledWithResultError(asyncio.CancelledError):
     """CancelledError with associated result or exception"""
 
     def __init__(self,
-                 result: Any | None,
+                 result: typing.Any | None,
                  exception: BaseException | None):
         super().__init__()
         self.__result = result
         self.__exception = exception
 
     @property
-    def result(self) -> Any | None:
+    def result(self) -> typing.Any | None:
         """Result"""
         return self.__result
 
     @property
     def exception(self) -> BaseException | None:
         return self.__exception
 
 
-async def wait_for(obj: Awaitable,
+async def wait_for(obj: typing.Awaitable,
                    timeout: float
-                   ) -> Any:
+                   ) -> typing.Any:
     """"Wait for the awaitable object to complete, with timeout.
 
     Implementation `asyncio.wait_for` that ensure propagation of
     CancelledError.
 
     If task is cancelled with objects's result available, instead of
     returning result, this implementation raises `CancelledWithResultError`.
```

## Comparing `hat_aio-0.7.8.dist-info/LICENSE` & `hat_aio-0.7.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_aio-0.7.8.dist-info/METADATA` & `hat_aio-0.7.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: hat-aio
-Version: 0.7.8
+Version: 0.7.9
 Summary: Hat async utility library
-Home-page: https://github.com/hat-open/hat-aio
+Description-Content-Type: text/x-rst
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
+Provides-Extra: dev
+Requires-Dist: hat-doit ~=0.15.5; extra == 'dev'
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
+Project-URL: Homepage, http://hat-open.com
+Project-URL: Repository, https://github.com/hat-open/hat-aio.git
+Project-URL: Documentation, http://hat-aio.hat-open.com
 
 .. _online documentation: https://hat-aio.hat-open.com
 .. _git repository: https://github.com/hat-open/hat-aio.git
 .. _PyPI project: https://pypi.org/project/hat-aio
 .. _pydoit: https://pydoit.org
 .. _Hat Open: https://hat-open.com
 .. _Končar Digital: https://www.koncar.hr/en
@@ -40,20 +43,25 @@
 
     $ pip install hat-aio
 
 
 Build
 -----
 
-Build tool used for `hat-aio` is `pydoit`_. It can be installed together
-with other python dependencies by running::
+To install editable installation, together with python development
+dependencies, run::
+
+    $ pip install -e '.[dev]'
+
+To install only python development dependencies, run::
 
-    $ pip install -r requirements.pip.dev.txt
+    $ pip install -r requirements.pip.txt
 
-For listing available doit tasks, use::
+Build tool used for `hat-aio` is `pydoit`_. For listing available doit tasks,
+use::
 
     $ doit list
 
 Default task::
 
     $ doit
```

## Comparing `hat_aio-0.7.8.dist-info/RECORD` & `hat_aio-0.7.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
+hat/aio/misc.py,sha256=TMAeMwhnoIL1VIwOK8jMvafhR7vH9hB6xWTA0IDTCNM,8979
+hat/aio/wait.py,sha256=WxauOgUe1RRInUIG_M1WynBP1O3QeUd-Q8u3M2pzvPE,1796
 hat/aio/__init__.py,sha256=Z3B9BTS_iZs2sFBp5fACdyukMdoyWxHVF0FtaDaa1A4,1225
-hat/aio/executor.py,sha256=3eTTEansyggm6y64bR624OCD7_Q3WUmbPGVXOSkmZ60,2781
-hat/aio/group.py,sha256=a339T1_xowqAB16UWEHejmYVmzPRVUKVN0oXLwoZk-k,6887
-hat/aio/misc.py,sha256=yjBhM1rW16g8qwlFDX9A6wL1mLVbPqftgASqc8a1S8g,8928
-hat/aio/queue.py,sha256=_VHvzVG2zKI1vSiSsNkKwCjrD-6rkR7USUi2qBDIhVc,6139
-hat/aio/wait.py,sha256=ucMjyjyoyZKYBauZXcOfYOLpQItPCbSaj3HmmlpW9hs,1788
-hat_aio-0.7.8.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_aio-0.7.8.dist-info/METADATA,sha256=rDdFxbIKe92290exfLYlLsc1YxUFTYH997iq-I-417A,2214
-hat_aio-0.7.8.dist-info/WHEEL,sha256=md_Sk-cFyicIH6eY_0BVqmsgC0wAFfbS1oq2bLoZiOk,114
-hat_aio-0.7.8.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_aio-0.7.8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-hat_aio-0.7.8.dist-info/RECORD,,
+hat/aio/group.py,sha256=HlhDda2uVo-dR1EOmDLUtboBE-CSXcscVpUfbMm4gHs,6883
+hat/aio/executor.py,sha256=siW0068FD4p1oUP4T6d6nYsZk2GyWXhqEdJUyB3f1VA,3147
+hat/aio/queue.py,sha256=lzY5vC9sPRaybScAzE2TEufU7LiksDcYYnR4tP_wQq0,6172
+hat_aio-0.7.9.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_aio-0.7.9.dist-info/METADATA,sha256=HL9bqb8BgeCSthFypnlWtiWTY18JOpTVQMUJUnt1z5c,2475
+hat_aio-0.7.9.dist-info/WHEEL,sha256=iwglvRPacSbapBwfIK1MKoh0cig7ezT6dST13qIHOd8,98
+hat_aio-0.7.9.dist-info/RECORD,,
```

