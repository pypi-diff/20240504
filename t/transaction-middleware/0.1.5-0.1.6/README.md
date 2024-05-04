# Comparing `tmp/transaction_middleware-0.1.5.tar.gz` & `tmp/transaction_middleware-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction_middleware-0.1.5.tar", max compression
+gzip compressed data, was "transaction_middleware-0.1.6.tar", max compression
```

## Comparing `transaction_middleware-0.1.5.tar` & `transaction_middleware-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-04 10:50:55.556873 transaction_middleware-0.1.5/LICENSE
--rw-r--r--   0        0        0     1380 2024-05-04 10:50:55.556873 transaction_middleware-0.1.5/README.md
--rw-r--r--   0        0        0     1606 2024-05-04 10:51:30.996832 transaction_middleware-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      170 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/__init__.py
--rw-r--r--   0        0        0     1825 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/functions.py
--rw-r--r--   0        0        0      294 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/logging.py
--rw-r--r--   0        0        0      770 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/settings.py
--rw-r--r--   0        0        0     1748 2024-05-04 10:50:55.576873 transaction_middleware-0.1.5/src/transaction_middleware/transaction_middleware.py
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 transaction_middleware-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-04 10:59:41.726120 transaction_middleware-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2079 2024-05-04 10:59:41.726120 transaction_middleware-0.1.6/README.md
+-rw-r--r--   0        0        0     1606 2024-05-04 11:00:15.714395 transaction_middleware-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-05-04 10:59:41.746121 transaction_middleware-0.1.6/src/transaction_middleware/__init__.py
+-rw-r--r--   0        0        0     1825 2024-05-04 10:59:41.746121 transaction_middleware-0.1.6/src/transaction_middleware/functions.py
+-rw-r--r--   0        0        0      294 2024-05-04 10:59:41.746121 transaction_middleware-0.1.6/src/transaction_middleware/logging.py
+-rw-r--r--   0        0        0      770 2024-05-04 10:59:41.746121 transaction_middleware-0.1.6/src/transaction_middleware/settings.py
+-rw-r--r--   0        0        0     1748 2024-05-04 10:59:41.746121 transaction_middleware-0.1.6/src/transaction_middleware/transaction_middleware.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 transaction_middleware-0.1.6/PKG-INFO
```

### Comparing `transaction_middleware-0.1.5/LICENSE` & `transaction_middleware-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.5/pyproject.toml` & `transaction_middleware-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transaction-middleware"
-version = "0.1.5"
+version = "0.1.6"
 description = "Async Transaction Middleware for FastAPI/Starlette"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "transaction_middleware", from = "src"}]
 license = "MIT"
 homepage = "https://impalah.github.io/transaction-middleware/"
 repository = "https://github.com/impalah/transaction-middleware"
```

### Comparing `transaction_middleware-0.1.5/src/transaction_middleware/functions.py` & `transaction_middleware-0.1.6/src/transaction_middleware/functions.py`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.5/src/transaction_middleware/settings.py` & `transaction_middleware-0.1.6/src/transaction_middleware/settings.py`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.5/src/transaction_middleware/transaction_middleware.py` & `transaction_middleware-0.1.6/src/transaction_middleware/transaction_middleware.py`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.5/PKG-INFO` & `transaction_middleware-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-middleware
-Version: 0.1.5
+Version: 0.1.6
 Summary: Async Transaction Middleware for FastAPI/Starlette
 Home-page: https://impalah.github.io/transaction-middleware/
 License: MIT
 Keywords: transaction,middleware,fastapi,starlette
 Author: impalah
 Author-email: impalah@gmail.com
 Requires-Python: >=3.10
@@ -53,31 +53,57 @@
 Transaction Middleware follows the middleware protocol and, therefore, should be added as a middleware to your FastApi or Starlette application.
 
 The steps, using FastAPI:
 
 ```python
 
 from fastapi import FastAPI, Depends
-
 from starlette.requests import Request
 from starlette.responses import Response
+from transaction_middleware import (
+    TransactionMiddleware,
+    get_transaction_id,
+    transaction_id_required,
+)
+
+app: FastAPI = FastAPI()
+app.add_middleware(TransactionMiddleware)
+
+@app.get(
+    "/items/{id}",
+    tags=["Item"],
+)
+async def read_items(
+    request: Request,
+    response: Response,
+    id: str,
+    transaction_id: str = Depends(get_transaction_id()),
+):
+    return {
+        "id": id,
+        "transaction_id": transaction_id if transaction_id else "No transaction ID",
+    }
 
 
 ```
 
 Then set the environment variables (or your .env file)
 
 ```bash
+TRANSACTION_MIDDLEWARE_LOG_LEVEL=DEBUG
+TRANSACTION_MIDDLEWARE_HEADER=X-Transaction-ID
 
 ```
 
-Call the method
+Launch the server.
+
+Call the method you want to test, and, optionally, set the transaction Id on the headers.
 
 ```bash
-curl -X GET http://localhost:8000/ -H "Authorization: Bearer MY_ID_TOKEN"
+curl -X GET http://localhost:8000/items/1234 -H "X-Transaction-ID: 2fyJr1FbRj603pH4rweEfEzQ"
 ```
 
 
 ## Middleware configuration
 
 The middleware configuration is done by environment variables (or using and .env file if your project uses python-dotenv).
```

