# Comparing `tmp/fastapi_tarpit-1.0.1.tar.gz` & `tmp/fastapi_tarpit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_tarpit-1.0.1.tar", last modified: Mon Apr 29 15:51:11 2024, max compression
+gzip compressed data, was "fastapi_tarpit-1.0.2.tar", last modified: Sat May  4 21:00:15 2024, max compression
```

## Comparing `fastapi_tarpit-1.0.1.tar` & `fastapi_tarpit-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-04-29 15:51:11.283146 fastapi_tarpit-1.0.1/
--rw-rw-r--   0 mats      (1000) mats      (1000)     1071 2024-04-16 21:29:58.000000 fastapi_tarpit-1.0.1/LICENSE
--rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-04-29 15:51:11.283146 fastapi_tarpit-1.0.1/PKG-INFO
--rw-rw-r--   0 mats      (1000) mats      (1000)     1084 2024-04-25 19:23:39.000000 fastapi_tarpit-1.0.1/README.md
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-04-29 15:51:11.283146 fastapi_tarpit-1.0.1/fastapi_tarpit/
--rw-rw-r--   0 mats      (1000) mats      (1000)      106 2024-04-17 20:42:08.000000 fastapi_tarpit-1.0.1/fastapi_tarpit/__init__.py
--rw-rw-r--   0 mats      (1000) mats      (1000)     4738 2024-04-25 19:35:54.000000 fastapi_tarpit-1.0.1/fastapi_tarpit/tarpit.py
-drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-04-29 15:51:11.283146 fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/
--rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-04-29 15:51:11.000000 fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/PKG-INFO
--rw-rw-r--   0 mats      (1000) mats      (1000)      273 2024-04-29 15:51:11.000000 fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/SOURCES.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)        1 2024-04-29 15:51:11.000000 fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/dependency_links.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)        8 2024-04-29 15:51:11.000000 fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/requires.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)       15 2024-04-29 15:51:11.000000 fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/top_level.txt
--rw-rw-r--   0 mats      (1000) mats      (1000)      693 2024-04-29 15:48:58.000000 fastapi_tarpit-1.0.1/pyproject.toml
--rw-rw-r--   0 mats      (1000) mats      (1000)       38 2024-04-29 15:51:11.283146 fastapi_tarpit-1.0.1/setup.cfg
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/
+-rw-rw-r--   0 mats      (1000) mats      (1000)     1071 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/LICENSE
+-rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/PKG-INFO
+-rw-rw-r--   0 mats      (1000) mats      (1000)     1084 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/README.md
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/fastapi_tarpit/
+-rw-rw-r--   0 mats      (1000) mats      (1000)      106 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/fastapi_tarpit/__init__.py
+-rw-rw-r--   0 mats      (1000) mats      (1000)     5711 2024-05-04 20:58:47.000000 fastapi_tarpit-1.0.2/fastapi_tarpit/tarpit.py
+drwxrwxr-x   0 mats      (1000) mats      (1000)        0 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/
+-rw-r--r--   0 mats      (1000) mats      (1000)     1703 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/PKG-INFO
+-rw-rw-r--   0 mats      (1000) mats      (1000)      273 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)        1 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)        8 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/requires.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)       15 2024-05-04 21:00:15.000000 fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/top_level.txt
+-rw-rw-r--   0 mats      (1000) mats      (1000)      693 2024-05-04 21:00:05.000000 fastapi_tarpit-1.0.2/pyproject.toml
+-rw-rw-r--   0 mats      (1000) mats      (1000)       38 2024-05-04 21:00:15.733099 fastapi_tarpit-1.0.2/setup.cfg
```

### Comparing `fastapi_tarpit-1.0.1/LICENSE` & `fastapi_tarpit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_tarpit-1.0.1/PKG-INFO` & `fastapi_tarpit-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tarpit
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastAPI middleware that purposely delays incoming connections on unused routes
 Author-email: Mats Klepsland <mats.klepsland@gmail.com>
 Project-URL: Homepage, https://github.com/thus/fastapi-tarpit
 Project-URL: Issues, https://github.com/thus/fastapi-tarpit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastapi_tarpit-1.0.1/README.md` & `fastapi_tarpit-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_tarpit-1.0.1/fastapi_tarpit/tarpit.py` & `fastapi_tarpit-1.0.2/fastapi_tarpit/tarpit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 from asyncio import sleep
+from contextlib import contextmanager
 from datetime import datetime, timedelta
+from random import randrange
 from signal import SIGINT, getsignal, signal
 from types import FrameType
-from typing import Any, AsyncIterator, Dict, List, Optional
+from typing import Any, AsyncIterator, Dict, Iterator, List, Optional
 
 from fastapi import FastAPI, Request
 from fastapi.responses import StreamingResponse
 from starlette.datastructures import Address
 from starlette.middleware.base import (BaseHTTPMiddleware,
                                        RequestResponseEndpoint)
 
@@ -42,94 +44,118 @@
                             f"{'minutes' if minutes > 1 else 'minute'}")
     if seconds or not duration_str:
         duration_str.append(f"{seconds} "
                             f"{'second' if seconds == 1 else 'seconds'}")
     return " ".join(duration_str)
 
 
+class TarpitConfig():
+    def __init__(
+            self,
+            interval: int = 2,
+            output_length_min: int = 1,
+            output_length_max: int = 5,
+            logger: Optional[logging.Logger] = None
+    ):
+        self.interval: int = interval
+        self.output_length_min: int = output_length_min
+        self.output_length_max: int = output_length_max
+        self.logger = logger if logger else logging.getLogger(__name__)
+
+
 class TarpitClient:
-    def __init__(self, request: Request, logger: logging.Logger):
+    def __init__(self, request: Request, config: TarpitConfig):
         if isinstance(request.client, Address):
-            self._host = f"{request.client.host}:{request.client.port}"
+            self.host = f"{request.client.host}:{request.client.port}"
         else:
-            self._host = "<undefined>"
-        self._request = request
-        self._logger = logger
-        self._start_time = datetime.now()
-        self._log_next = self._start_time + timedelta(seconds=log_interval[0])
-        self._log_interval_idx = 0
-        self._logging_enabled = True
-        self._logger.info(f"'{self._host}' got stuck in the tarpit visiting "
-                          f"'{request.url.path}'")
-
-    def __del__(self) -> None:
-        duration = duration_pretty_string(datetime.now() - self._start_time)
-        self._logger.info(f"Trapped '{self._host} in the tarpit for "
-                          f"{duration}")
+            self.host = "<undefined>"
+        self.request = request
+        self.config = config
+        self.start_time = datetime.now()
+        self.log_next = self.start_time + timedelta(seconds=log_interval[0])
+        self.log_interval_idx = 0
+        self.logging_enabled = True
+        self.config.logger.info(f"'{self.host}' got stuck in the tarpit "
+                                f"visiting '{request.url.path}'")
+
+    def close(self) -> None:
+        duration = duration_pretty_string(datetime.now() - self.start_time)
+        self.config.logger.info(f"Trapped '{self.host} in the tarpit for "
+                                f"{duration} visiting "
+                                f"'{self.request.url.path}'")
 
     def tick(self) -> None:
         """Used to log how long a host has been stuck in the tarpit at
            different time intervals (minute, hour, day, etc)."""
-        if not self._logging_enabled or datetime.now() < self._log_next:
+        if not self.logging_enabled or datetime.now() < self.log_next:
             return
 
-        duration = duration_pretty_string(datetime.now() - self._start_time)
-        self._logger.info(f"'{self._host}' is still stuck in the tarpit "
-                          f"after {duration}")
+        duration = duration_pretty_string(datetime.now() - self.start_time)
+        self.config.logger.info(f"'{self.host}' is still stuck in the tarpit "
+                                f"after {duration} visiting "
+                                f"'{self.request.url.path}'")
 
-        self._log_interval_idx += 1
+        self.log_interval_idx += 1
         try:
-            seconds = log_interval[self._log_interval_idx]
+            seconds = log_interval[self.log_interval_idx]
         except IndexError:
             # This is unlikely to ever happen, but if it does, then just
             # disable logging.
-            self._logging_enabled = False
-        self._log_next = self._start_time + timedelta(seconds=seconds)
+            self.logging_enabled = False
+        self.log_next = self.start_time + timedelta(seconds=seconds)
 
-
-async def tarpit_stream(client: TarpitClient,
-                        interval: int) -> AsyncIterator[bytes]:
-    while tarpit_running:
-        await sleep(interval)
-        client.tick()
-        yield b"."
+    def generate_bytes(self) -> bytes:
+        length = randrange(self.config.output_length_min,
+                           self.config.output_length_max)
+        return b'.' * length
+
+
+@contextmanager
+def tarpit_connection(request: Request,
+                      config: TarpitConfig) -> Iterator[TarpitClient]:
+    client = TarpitClient(request, config)
+    try:
+        yield client
+    finally:
+        client.close()
+
+
+async def tarpit_stream(request: Request,
+                        config: TarpitConfig) -> AsyncIterator[bytes]:
+    with tarpit_connection(request, config) as client:
+        while tarpit_running:
+            await sleep(config.interval)
+            client.tick()
+            yield client.generate_bytes()
 
 
 class HTTPTarpitMiddleware(BaseHTTPMiddleware):
-    def __init__(
-            self,
-            app: FastAPI,
-            *,
-            interval: int = 2,
-            logger: Optional[logging.Logger] = None
-    ):
-        self._interval: int = interval
-        self._logger = logger if logger else logging.getLogger(__name__)
-        self._routes: Dict[str, int] = {}
+    def __init__(self, app: FastAPI, **kwargs: Any):
+        self.config: TarpitConfig = TarpitConfig(**kwargs)
+        self.routes: Dict[str, int] = {}
 
         default_sigint_handler = getsignal(SIGINT)
 
         def tarpit_shutdown(signum: int, frame: Optional[FrameType]) -> None:
             global tarpit_running
             tarpit_running = False
 
             if default_sigint_handler:
                 default_sigint_handler(signum, frame)  # type: ignore
 
         signal(SIGINT, tarpit_shutdown)
 
         super().__init__(app)
 
-    def _get_routes(self, app: FastAPI) -> None:
+    def get_routes(self, app: FastAPI) -> None:
         for route in app.routes:
-            self._routes[route.path] = 1  # type: ignore
+            self.routes[route.path] = 1  # type: ignore
 
     async def dispatch(self, request: Request,
                        call_next: RequestResponseEndpoint) -> Any:
-        if not self._routes:
-            self._get_routes(request.app)
+        if not self.routes:
+            self.get_routes(request.app)
 
-        if request.url.path not in self._routes:
-            client = TarpitClient(request, self._logger)
-            return StreamingResponse(tarpit_stream(client, self._interval))
+        if request.url.path not in self.routes:
+            return StreamingResponse(tarpit_stream(request, self.config))
 
         return await call_next(request)
```

### Comparing `fastapi_tarpit-1.0.1/fastapi_tarpit.egg-info/PKG-INFO` & `fastapi_tarpit-1.0.2/fastapi_tarpit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tarpit
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastAPI middleware that purposely delays incoming connections on unused routes
 Author-email: Mats Klepsland <mats.klepsland@gmail.com>
 Project-URL: Homepage, https://github.com/thus/fastapi-tarpit
 Project-URL: Issues, https://github.com/thus/fastapi-tarpit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastapi_tarpit-1.0.1/pyproject.toml` & `fastapi_tarpit-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi-tarpit"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Mats Klepsland", email="mats.klepsland@gmail.com" },
 ]
 dependencies = [
   "fastapi",
 ]
 description = "FastAPI middleware that purposely delays incoming connections on unused routes"
```

