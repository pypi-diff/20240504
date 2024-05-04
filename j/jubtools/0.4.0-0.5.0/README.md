# Comparing `tmp/jubtools-0.4.0.tar.gz` & `tmp/jubtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubtools-0.4.0.tar", last modified: Fri May  3 13:33:08 2024, max compression
+gzip compressed data, was "jubtools-0.5.0.tar", last modified: Sat May  4 20:04:23 2024, max compression
```

## Comparing `jubtools-0.4.0.tar` & `jubtools-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 13:33:08.163435 jubtools-0.4.0/
--rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.4.0/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-03 13:33:08.163220 jubtools-0.4.0/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.4.0/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 13:33:08.161389 jubtools-0.4.0/jubtools/
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.4.0/jubtools/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1427 2024-05-03 13:17:38.000000 jubtools-0.4.0/jubtools/config.py
--rw-r--r--   0 andy       (501) staff       (20)     1140 2024-05-03 12:30:40.000000 jubtools-0.4.0/jubtools/httptools.py
--rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.4.0/jubtools/misctools.py
--rw-r--r--   0 andy       (501) staff       (20)     4694 2024-05-03 12:07:31.000000 jubtools-0.4.0/jubtools/psql.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.4.0/jubtools/py.typed
--rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.4.0/jubtools/sqlt.py
--rw-r--r--   0 andy       (501) staff       (20)     3757 2024-05-03 13:08:52.000000 jubtools-0.4.0/jubtools/systemtools.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 13:33:08.162796 jubtools-0.4.0/jubtools.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-03 13:33:08.000000 jubtools-0.4.0/jubtools.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-03 13:33:08.000000 jubtools-0.4.0/jubtools.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-03 13:33:08.000000 jubtools-0.4.0/jubtools.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-03 13:33:08.000000 jubtools-0.4.0/jubtools.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-03 13:33:08.000000 jubtools-0.4.0/jubtools.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)      598 2024-05-03 13:32:14.000000 jubtools-0.4.0/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-03 13:33:08.163502 jubtools-0.4.0/setup.cfg
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-03 13:33:08.162639 jubtools-0.4.0/tests/
--rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.4.0/tests/test_config.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.4.0/tests/test_misctools.py
--rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.4.0/tests/test_systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:04:23.698700 jubtools-0.5.0/
+-rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.0/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 20:04:23.698457 jubtools-0.5.0/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.0/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:04:23.696457 jubtools-0.5.0/jubtools/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.0/jubtools/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.0/jubtools/config.py
+-rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.0/jubtools/httptools.py
+-rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.0/jubtools/misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)     4891 2024-05-04 20:02:52.000000 jubtools-0.5.0/jubtools/psql.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.0/jubtools/py.typed
+-rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.0/jubtools/sqlt.py
+-rw-r--r--   0 andy       (501) staff       (20)     3757 2024-05-03 13:08:52.000000 jubtools-0.5.0/jubtools/systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:04:23.698036 jubtools-0.5.0/jubtools.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 20:04:23.000000 jubtools-0.5.0/jubtools.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-04 20:04:23.000000 jubtools-0.5.0/jubtools.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-04 20:04:23.000000 jubtools-0.5.0/jubtools.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-04 20:04:23.000000 jubtools-0.5.0/jubtools.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-04 20:04:23.000000 jubtools-0.5.0/jubtools.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      598 2024-05-04 20:03:53.000000 jubtools-0.5.0/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-04 20:04:23.698762 jubtools-0.5.0/setup.cfg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 20:04:23.697790 jubtools-0.5.0/tests/
+-rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.0/tests/test_config.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.0/tests/test_misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.0/tests/test_systemtools.py
```

### Comparing `jubtools-0.4.0/LICENSE` & `jubtools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jubtools-0.4.0/PKG-INFO` & `jubtools-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.4.0/jubtools/config.py` & `jubtools-0.5.0/jubtools/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import json
 import logging
+import logging.config
 import os
 
 import toml
 
 logger = logging.getLogger(__name__)
 
 CONFIG: dict = {}
@@ -18,14 +20,21 @@
 
     # Then, load from env file, overwriting if necessary
     if env is not None:
         env_filename = os.path.join(CONFIG_DIR, ENV_DIR, env) + ".toml"
         _load_from_file(env_filename)
 
 
+def init_logging(log_config_file: str = "log_config.json"):
+    filename = os.path.join(CONFIG_DIR, log_config_file)
+    with open(filename, "r") as f:
+        log_config = json.load(f)
+        logging.config.dictConfig(log_config)
+
+
 # Get a value from config. Will handle nested key names separated by dots eg. 'db.port'
 def get(full_key: str):
     keys = full_key.split(".")
     vals = CONFIG
     for key in keys:
         if key not in vals:
             raise Exception(f"Config key not present: {full_key}")
```

### Comparing `jubtools-0.4.0/jubtools/httptools.py` & `jubtools-0.5.0/jubtools/httptools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import csv
 from enum import Enum
 import logging
 from typing import Any
 
 import httpx
 
 from jubtools import misctools
 
 logger = logging.getLogger(__name__)
 
 
 class ResponseFormat(str, Enum):
-    JSON = "JSON"
     BYTES = "BYTES"
+    CSV = "CSV"
+    JSON = "JSON"
 
 
 async def get(
     url: str, params: dict[str, Any] = {}, response_format: ResponseFormat = ResponseFormat.JSON
 ):
     logger.info(f"HTTP GET {url} (params {params})")
     try:
@@ -25,15 +27,17 @@
             async with httpx.AsyncClient() as client:
                 resp = await client.get(url, params=params)
                 status = resp.status_code
                 reason = resp.reason_phrase
                 resp.raise_for_status()
 
             match response_format:
-                case ResponseFormat.JSON:
-                    logger.info(f"Response JSON: {resp.json()}")
-                    return resp.json()
                 case ResponseFormat.BYTES:
                     logger.info(f"Response text: {resp.text}")
                     return resp.text
+                case ResponseFormat.CSV:
+                    return list(csv.DictReader(resp.text.splitlines(), delimiter=';'))
+                case ResponseFormat.JSON:
+                    logger.info(f"Response JSON: {resp.json()}")
+                    return resp.json()
     finally:
         logger.info(f"HTTP GET {url} {status} {reason} ({timer.elapsed:.2f}ms)")
```

### Comparing `jubtools-0.4.0/jubtools/psql.py` & `jubtools-0.5.0/jubtools/psql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from contextlib import asynccontextmanager
+from contextvars import ContextVar
+import json
 import os
 import logging
 import time
 from typing import List, Dict, Tuple, Iterable
 
 import asyncpg
 from fastapi import Request
 
-from jubtools import config, misctools
+from jubtools_e import config, misctools
 
 logger = logging.getLogger(__name__)
 
 _POOL = None
 _SQL = {}
+CONN = ContextVar('conn')
 
 
 # Add ability to use 'row.value' syntax, which is shorter and easier than 'row["value"]'
 class Row(asyncpg.Record):
     def __getattr__(self, name):
         return self[name]
 
@@ -35,17 +38,27 @@
         host=host,
         port=port,
         user=user,
         password=password,
         database=database,
         min_size=2,
         record_class=Row,
+        init=init_conn
     )
     logger.info("DB connection pool created")
 
+async def init_conn(conn):
+    logger.info(f"Initialising connection: {conn}")
+    await conn.set_type_codec(
+        'json',
+        encoder=json.dumps,
+        decoder=json.loads,
+        schema='pg_catalog'
+    )
+
 
 async def shutdown():
     global _POOL
 
     if _POOL is not None:
         await _POOL.close()
 
@@ -54,57 +67,49 @@
     global _SQL
     logger.info(f"Store sql: {name}")
     if name in _SQL:
         raise ValueError(f"Duplicate sql: {name}")
     _SQL[name] = sql
 
 
-async def execute(req: Request, name: str, args={}, log_args=True) -> List[Row]:
-    con = req.scope["db_conn"]
-    return await execute_with_conn(con, name, args, log_args)
+async def execute(name: str, args={}, log_args=True) -> List[Row]:
+    conn = CONN.get()
+    return await execute_with_conn(conn, name, args, log_args)
 
 
 async def execute_with_conn(con, name, args={}, log_args=True) -> List[Row]:
     if log_args:
         logger.info(f"Execute sql {name} with args: {args}")
     else:
         logger.info(f"Execute sql {name}")
     sql, params = _get_sql(name, args)
     with misctools.Timer() as timer:
         rs = await con.fetch(sql, *params)
     logger.info(f"{len(rs)} row{'s' if len(rs) != 1 else ''} ({timer.elapsed:.2f}ms)")
     return rs
 
 
-async def execute_sql(req: Request, sql: str, args={}) -> List[Row]:
-    con = req.scope["db_conn"]
-    return await execute_sql_with_conn(con, sql, args)
+async def execute_sql(sql: str, args={}) -> List[Row]:
+    conn = CONN.get()
+    return await execute_sql_with_conn(conn, sql, args)
 
 
-async def execute_sql_with_conn(con, sql: str, args={}) -> List[Row]:
+async def execute_sql_with_conn(conn, sql: str, args={}) -> List[Row]:
     logger.info(f"Execute custom sql with args: {args}")
     sql, params = _format_sql(sql, args)
     with misctools.Timer() as timer:
-        rs = await con.fetch(sql, *params)
+        rs = await conn.fetch(sql, *params)
     logger.info(f"{len(rs)} row{'s' if len(rs) != 1 else ''} ({timer.elapsed:.2f}ms)")
     return rs
 
 
 def transaction(req):
     return Transaction(req.scope["db_conn"])
 
 
-# Aquire a temporary connection object, for performing queries outside a transaction, etc.
-# Should not normally need to be used
-@asynccontextmanager
-async def aquire_conn():
-    async with _POOL.acquire() as con:
-        yield con
-
-
 class Serial(dict):
     def __getitem__(self, key):
         return f"${list(self.keys()).index(key) + 1}"
 
 
 # Get the sql from our saved list and process it with _format_sql
 def _get_sql(name, args) -> Tuple[str, Iterable]:
@@ -118,28 +123,37 @@
 # arguments ("$1"), as named arguments are not supported by asyncpg
 def _format_sql(sql: str, args: Dict) -> Tuple[str, Iterable]:
     params = Serial(args)
     sql = sql.format_map(params)
     return (sql, params.values())
 
 
+@asynccontextmanager
+async def connect():
+    global CONN
+    async with _POOL.acquire() as conn:
+        token = CONN.set(conn)
+        try:
+            yield
+        finally:
+            CONN.reset(token)
+
+
 # Starlette middleware that acquires a db connection before the request, and releases it afterwards
 class ConnMiddleware:
     def __init__(self, app):
         self.app = app
 
     async def __call__(self, scope, receive, send):
         # Ignore calls that are not http requests (eg. startup)
         # Ignore /health requests - we don't need a db connection for these
         if scope["type"] != "http" or scope["path"] == "/health":
             return await self.app(scope, receive, send)
 
-        async with _POOL.acquire() as conn:
-            scope["db_conn"] = conn
-
+        async with connect():
             return await self.app(scope, receive, send)
 
 
 # Basic transaction wrapper which adds timing and logging
 class Transaction(asyncpg.transaction.Transaction):
     def __init__(self, conn):
         self.transaction = conn.transaction()
```

### Comparing `jubtools-0.4.0/jubtools/sqlt.py` & `jubtools-0.5.0/jubtools/sqlt.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.4.0/jubtools/systemtools.py` & `jubtools-0.5.0/jubtools/systemtools.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.4.0/jubtools.egg-info/PKG-INFO` & `jubtools-0.5.0/jubtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.4.0/pyproject.toml` & `jubtools-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "jubtools"
 description = "Shared tools for my own work"
 readme = "README.md"
 license = { file = "LICENSE" }
-version = "0.4.0"
+version = "0.5.0"
 authors = [{ name = "Andrew Morcom", email = "jubulani@fastmail.fm" }]
 requires-python = ">=3.10"
 dependencies = ["fastapi"]
 
 [project.optional-dependencies]
 test = [
     "async_asgi_testclient >= 1.4",
```

### Comparing `jubtools-0.4.0/tests/test_config.py` & `jubtools-0.5.0/tests/test_config.py`

 * *Files identical despite different names*

