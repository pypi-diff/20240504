# Comparing `tmp/pg_alchemy_kit-0.9.19b0.tar.gz` & `tmp/pg_alchemy_kit-0.9.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_alchemy_kit-0.9.19b0.tar", max compression
+gzip compressed data, was "pg_alchemy_kit-0.9.1b0.tar", max compression
```

## Comparing `pg_alchemy_kit-0.9.19b0.tar` & `pg_alchemy_kit-0.9.1b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.9.19b0/README.md
--rw-r--r--   0        0        0     3361 2024-03-15 17:20:52.235000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PG.py
--rw-r--r--   0        0        0    12877 2024-04-08 02:01:27.341432 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PGUtils.py
--rw-r--r--   0        0        0     6323 2024-03-15 17:21:48.231000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PGUtilsBase.py
--rw-r--r--   0        0        0     5512 2024-03-15 17:22:12.728000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PGUtilsORM.py
--rw-r--r--   0        0        0      353 2023-12-02 13:44:05.554000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/__init__.py
--rw-r--r--   0        0        0      383 2024-05-01 16:40:02.888127 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__init__.py
--rw-r--r--   0        0        0     2548 2024-04-20 23:32:34.684154 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc
--rw-r--r--   0        0        0     4706 2024-04-21 00:55:25.414792 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc
--rw-r--r--   0        0        0     8382 2024-03-21 22:25:25.802000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc
--rw-r--r--   0        0        0    10742 2024-04-20 23:32:34.686799 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc
--rw-r--r--   0        0        0    16328 2024-04-21 00:52:13.046852 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc
--rw-r--r--   0        0        0     4980 2024-02-23 22:12:09.581000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc
--rw-r--r--   0        0        0     8275 2024-02-23 22:14:07.165000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc
--rw-r--r--   0        0        0     5417 2024-02-23 22:16:34.786000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc
--rw-r--r--   0        0        0      460 2024-03-05 23:14:18.543000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      481 2024-04-20 23:34:09.319347 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2441 2024-05-01 16:40:12.259102 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/pg.py
--rw-r--r--   0        0        0     7957 2024-05-01 16:37:23.653530 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/pg_utils.py
--rw-r--r--   0        0        0     5840 2023-11-01 14:19:01.447000 pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/cacheStrategies.py
--rw-r--r--   0        0        0      851 2024-05-01 16:41:46.033482 pg_alchemy_kit-0.9.19b0/pyproject.toml
--rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.9.19b0/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-07-23 05:05:39.685000 pg_alchemy_kit-0.9.1b0/README.md
+-rw-r--r--   0        0        0     3361 2024-03-15 17:20:52.235000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PG.py
+-rw-r--r--   0        0        0    12877 2024-04-08 02:01:27.341432 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtils.py
+-rw-r--r--   0        0        0     6323 2024-03-15 17:21:48.231000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsBase.py
+-rw-r--r--   0        0        0     5512 2024-03-15 17:22:12.728000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsORM.py
+-rw-r--r--   0        0        0      353 2023-12-02 13:44:05.554000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/__init__.py
+-rw-r--r--   0        0        0     2780 2024-04-21 00:55:09.212262 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPG.py
+-rw-r--r--   0        0        0     9426 2024-04-21 00:49:46.175891 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPGUtilsORM.py
+-rw-r--r--   0        0        0      402 2024-03-05 23:13:28.466000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__init__.py
+-rw-r--r--   0        0        0     2548 2024-04-20 23:32:34.684154 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc
+-rw-r--r--   0        0        0     4706 2024-04-21 00:55:25.414792 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc
+-rw-r--r--   0        0        0     8382 2024-03-21 22:25:25.802000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc
+-rw-r--r--   0        0        0    10742 2024-04-20 23:32:34.686799 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc
+-rw-r--r--   0        0        0    16328 2024-04-21 00:52:13.046852 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc
+-rw-r--r--   0        0        0     4980 2024-02-23 22:12:09.581000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc
+-rw-r--r--   0        0        0     8275 2024-02-23 22:14:07.165000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc
+-rw-r--r--   0        0        0     5417 2024-02-23 22:16:34.786000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc
+-rw-r--r--   0        0        0      460 2024-03-05 23:14:18.543000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      481 2024-04-20 23:34:09.319347 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5840 2023-11-01 14:19:01.447000 pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/cacheStrategies.py
+-rw-r--r--   0        0        0      851 2024-04-21 01:01:41.086173 pg_alchemy_kit-0.9.1b0/pyproject.toml
+-rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 pg_alchemy_kit-0.9.1b0/PKG-INFO
```

### Comparing `pg_alchemy_kit-0.9.19b0/README.md` & `pg_alchemy_kit-0.9.1b0/README.md`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PG.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PG.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PGUtils.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtils.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PGUtilsBase.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsBase.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/PGUtilsORM.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/PGUtilsORM.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPG.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsBase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/AsyncPGUtilsORM.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PG.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsBase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/__pycache__/PGUtilsORM.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/asyncio/pg.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/asyncio/AsyncPG.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from .pg_utils import AsyncPGUtilsORM, PGUtilsParams
+from .AsyncPGUtilsORM import AsyncPGUtilsORM, PGUtilsParams
 from contextlib import asynccontextmanager
 from collections.abc import AsyncGenerator
 from sqlalchemy.ext.asyncio import (
     AsyncSession,
     create_async_engine,
     AsyncEngine,
     async_sessionmaker,
     async_scoped_session,
 )
 from asyncio import current_task
 
 from typing import Any, TypedDict, TypeVar
 from typing_extensions import Unpack, NotRequired
+from warnings import warn
 
 
 class InitParams(TypedDict):
     async_engine_kwargs: NotRequired[dict[str, Any]]
     async_pg_utils_kwargs: NotRequired[PGUtilsParams]
     async_session_maker_kwargs: NotRequired[dict[str, Any]]
     echo: NotRequired[bool]
@@ -30,19 +31,15 @@
 
     def initialize(
         self,
         url: str,
         **kwargs: Unpack[InitParams],
     ):
         self.async_pg_utils_kwargs: PGUtilsParams = kwargs.pop(
-            "async_pg_utils_kwargs",
-            {
-                "snake_case": False,
-                "single_transaction": True,
-            },
+            "async_pg_utils_kwargs", {}
         )
         async_session_maker_kwargs: dict[str, Any] = kwargs.pop(
             "async_session_maker_kwargs", {}
         )
         async_engine_kwargs: dict[str, Any] = kwargs.pop("async_engine_kwargs", {})
 
         self.url: str = url
@@ -59,15 +56,27 @@
             **async_session_maker_kwargs,
         )
 
         self.Session = async_scoped_session(
             self.session_factory, scopefunc=current_task
         )
 
-        self.utils = AsyncPGUtilsORM[Any](**self.async_pg_utils_kwargs)
+        self._utils: AsyncPGUtilsORM = AsyncPGUtilsORM(**self.async_pg_utils_kwargs)
+
+    @property
+    def utils(self):
+        warn(
+            "The 'utils' attribute is deprecated and will be removed in a future release. Please use get_utils(model) instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._utils
+
+    def get_utils(self, model: T) -> AsyncPGUtilsORM[T]:
+        return AsyncPGUtilsORM[model](**self.async_pg_utils_kwargs)
 
     @asynccontextmanager
     async def get_session_ctx(self) -> AsyncGenerator[AsyncSession, None]:
         async with self.Session() as session:
             yield session
 
     @asynccontextmanager
```

### Comparing `pg_alchemy_kit-0.9.19b0/pg_alchemy_kit/cacheStrategies.py` & `pg_alchemy_kit-0.9.1b0/pg_alchemy_kit/cacheStrategies.py`

 * *Files identical despite different names*

### Comparing `pg_alchemy_kit-0.9.19b0/pyproject.toml` & `pg_alchemy_kit-0.9.1b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pg-alchemy-kit"
-version = "0.9.19-beta"
+version = "0.9.01-beta"
 description = "A simple wrapper around sqlalchemy to make it easier to use with postgresql"
 authors = ["jsaied99 <jsaied99@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jsaied99/pg-alchemy-kit"
 packages = [{ include = "pg_alchemy_kit" }]
 
 [tool.poetry.dependencies]
```

### Comparing `pg_alchemy_kit-0.9.19b0/PKG-INFO` & `pg_alchemy_kit-0.9.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pg-alchemy-kit
-Version: 0.9.19b0
+Version: 0.9.1b0
 Summary: A simple wrapper around sqlalchemy to make it easier to use with postgresql
 Home-page: https://github.com/jsaied99/pg-alchemy-kit
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: psycopg2-binary (==2.9.3)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.27,<3.0.0)
 Project-URL: Repository, https://github.com/jsaied99/pg-alchemy-kit
 Description-Content-Type: text/markdown
```

