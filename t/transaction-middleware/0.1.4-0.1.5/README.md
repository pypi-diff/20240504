# Comparing `tmp/transaction_middleware-0.1.4.tar.gz` & `tmp/transaction_middleware-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction_middleware-0.1.4.tar", max compression
+gzip compressed data, was "transaction_middleware-0.1.5.tar", max compression
```

## Comparing `transaction_middleware-0.1.4.tar` & `transaction_middleware-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-03 20:44:12.870985 transaction_middleware-0.1.4/LICENSE
--rw-r--r--   0        0        0     1392 2024-05-03 20:44:12.870985 transaction_middleware-0.1.4/README.md
--rw-r--r--   0        0        0     1606 2024-05-03 20:44:50.335276 transaction_middleware-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      170 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/__init__.py
--rw-r--r--   0        0        0     1461 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/functions.py
--rw-r--r--   0        0        0      294 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/logging.py
--rw-r--r--   0        0        0      745 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/settings.py
--rw-r--r--   0        0        0     1675 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/transaction_middleware.py
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 transaction_middleware-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-04 10:50:55.556873 transaction_middleware-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1380 2024-05-04 10:50:55.556873 transaction_middleware-0.1.5/README.md
+-rw-r--r--   0        0        0     1606 2024-05-04 10:51:30.996832 transaction_middleware-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/__init__.py
+-rw-r--r--   0        0        0     1825 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/functions.py
+-rw-r--r--   0        0        0      294 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/logging.py
+-rw-r--r--   0        0        0      770 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/settings.py
+-rw-r--r--   0        0        0     1748 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/transaction_middleware.py
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 transaction_middleware-0.1.5/PKG-INFO
```

### Comparing `transaction_middleware-0.1.4/LICENSE` & `transaction_middleware-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.4/README.md` & `transaction_middleware-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,11 +52,11 @@
 
 The main variables are shown in the table below:
 
 | Name | Description | Values | Default |
 | --------- | --------- | --------- | --------- |
 | TRANSACTION_MIDDLEWARE_LOG_LEVEL | Log level for the application | DEBUG, INFO, WARNING, ERROR, CRITICAL | INFO |
 | TRANSACTION_MIDDLEWARE_LOG_FORMAT | Log format | See python logger documentation | %(log_color)s%(levelname)-9s%(reset)s %(asctime)s %(name)s %(message)s |
-| TRANSACTION_MIDDLEWARE_DISABLED | Transaction middleware enabled/disabled | false, true | false |
+| TRANSACTION_MIDDLEWARE_HEADER | Name for the header | Any String | X-Transaction-ID |
```

### Comparing `transaction_middleware-0.1.4/pyproject.toml` & `transaction_middleware-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transaction-middleware"
-version = "0.1.4"
+version = "0.1.5"
 description = "Async Transaction Middleware for FastAPI/Starlette"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "transaction_middleware", from = "src"}]
 license = "MIT"
 homepage = "https://impalah.github.io/transaction-middleware/"
 repository = "https://github.com/impalah/transaction-middleware"
```

### Comparing `transaction_middleware-0.1.4/src/transaction_middleware/functions.py` & `transaction_middleware-0.1.5/src/transaction_middleware/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from functools import wraps
-from typing import List
+from typing import Callable, List
 
 from fastapi import HTTPException, Request
 from ksuid import Ksuid
 
 from transaction_middleware.logging import logger
+from transaction_middleware.settings import settings
 
 
 def get_transaction_id(
     create_if_missing: bool = True,
-    header_name: str = "X-Transaction-ID",
+    header_name: str = settings.TRANSACTION_MIDDLEWARE_HEADER,
+    generator: Callable[[], str] = lambda: str(Ksuid()),
 ) -> str:
     """Get the transaction ID from the request headers or generate a new one.
 
     Args:
         create_if_missing (bool, optional): If True, generates a new transaction ID if not found in the request headers. Defaults to True.
-        request (Request): _description_
+        header_name (str, optional): Name of the header to look for the transaction ID. Defaults to settings.TRANSACTION_MIDDLEWARE_HEADER.
+        generator (Callable[[], str], optional): Function to generate a new transaction ID. Defaults to lambda: str(Ksuid()).
 
     Raises:
         HTTPException: _description_
 
     Returns:
         str: _description_
     """
@@ -37,13 +40,13 @@
 
         if not transaction_id:
             # Extract transaction id from request if does not exists on state
             transaction_id = request.headers.get(header_name)
             logger.debug(f"Transaction ID from headers: {transaction_id}")
 
         if transaction_id is None and create_if_missing:
-            transaction_id = str(Ksuid())
+            transaction_id = generator()
             request.state.transaction_id = transaction_id
 
         return transaction_id
 
     return _get_transaction_id
```

### Comparing `transaction_middleware-0.1.4/src/transaction_middleware/settings.py` & `transaction_middleware-0.1.5/src/transaction_middleware/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,13 +12,15 @@
     TRANSACTION_MIDDLEWARE_LOG_FORMAT: str = config(
         "TRANSACTION_MIDDLEWARE_LOG_FORMAT",
         cast=str,
         default="<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>",
     )
 
     # Disable transaction for the whole application
-    TRANSACTION_MIDDLEWARE_DISABLED = config(
-        "TRANSACTION_MIDDLEWARE_DISABLED", cast=bool, default=False
+    TRANSACTION_MIDDLEWARE_HEADER = config(
+        "TRANSACTION_MIDDLEWARE_HEADER",
+        cast=str,
+        default="X-Transaction-ID",
     )
 
 
 settings = Settings()
```

### Comparing `transaction_middleware-0.1.4/src/transaction_middleware/transaction_middleware.py` & `transaction_middleware-0.1.5/src/transaction_middleware/transaction_middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 from fastapi.security.utils import get_authorization_scheme_param
 from ksuid import Ksuid
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from transaction_middleware.logging import logger
+from transaction_middleware.settings import settings
 
 
 class TransactionMiddleware(BaseHTTPMiddleware):
     """Transaction middleware for FastAPI
     Manages transaction IDs in the request.
 
     Args:
         BaseHTTPMiddleware (_type_): _description_
     """
 
     def __init__(
         self,
-        header_name: str = "X-Transaction-ID",
+        header_name: str = settings.TRANSACTION_MIDDLEWARE_HEADER,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.header_name = header_name
 
     async def dispatch(
```

### Comparing `transaction_middleware-0.1.4/PKG-INFO` & `transaction_middleware-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-middleware
-Version: 0.1.4
+Version: 0.1.5
 Summary: Async Transaction Middleware for FastAPI/Starlette
 Home-page: https://impalah.github.io/transaction-middleware/
 License: MIT
 Keywords: transaction,middleware,fastapi,starlette
 Author: impalah
 Author-email: impalah@gmail.com
 Requires-Python: >=3.10
@@ -83,12 +83,12 @@
 
 The main variables are shown in the table below:
 
 | Name | Description | Values | Default |
 | --------- | --------- | --------- | --------- |
 | TRANSACTION_MIDDLEWARE_LOG_LEVEL | Log level for the application | DEBUG, INFO, WARNING, ERROR, CRITICAL | INFO |
 | TRANSACTION_MIDDLEWARE_LOG_FORMAT | Log format | See python logger documentation | %(log_color)s%(levelname)-9s%(reset)s %(asctime)s %(name)s %(message)s |
-| TRANSACTION_MIDDLEWARE_DISABLED | Transaction middleware enabled/disabled | false, true | false |
+| TRANSACTION_MIDDLEWARE_HEADER | Name for the header | Any String | X-Transaction-ID |
```

