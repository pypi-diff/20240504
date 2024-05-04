# Comparing `tmp/transaction_middleware-0.1.3.tar.gz` & `tmp/transaction_middleware-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction_middleware-0.1.3.tar", max compression
+gzip compressed data, was "transaction_middleware-0.1.4.tar", max compression
```

## Comparing `transaction_middleware-0.1.3.tar` & `transaction_middleware-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-05-02 17:50:44.970679 transaction_middleware-0.1.3/LICENSE
--rw-r--r--   0        0        0     1385 2024-05-02 17:50:44.970679 transaction_middleware-0.1.3/README.md
--rw-r--r--   0        0        0     1610 2024-05-02 17:51:21.482860 transaction_middleware-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      226 2024-05-02 17:50:44.990679 transaction_middleware-0.1.3/src/transaction_middleware/__init__.py
--rw-r--r--   0        0        0     1047 2024-05-02 17:50:44.990679 transaction_middleware-0.1.3/src/transaction_middleware/functions.py
--rw-r--r--   0        0        0      294 2024-05-02 17:50:44.990679 transaction_middleware-0.1.3/src/transaction_middleware/logging.py
--rw-r--r--   0        0        0      745 2024-05-02 17:50:44.990679 transaction_middleware-0.1.3/src/transaction_middleware/settings.py
--rw-r--r--   0        0        0     1765 2024-05-02 17:50:44.990679 transaction_middleware-0.1.3/src/transaction_middleware/transaction_middleware.py
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 transaction_middleware-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 20:44:12.870985 transaction_middleware-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1392 2024-05-03 20:44:12.870985 transaction_middleware-0.1.4/README.md
+-rw-r--r--   0        0        0     1606 2024-05-03 20:44:50.335276 transaction_middleware-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/__init__.py
+-rw-r--r--   0        0        0     1461 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/functions.py
+-rw-r--r--   0        0        0      294 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/logging.py
+-rw-r--r--   0        0        0      745 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/settings.py
+-rw-r--r--   0        0        0     1675 2024-05-03 20:44:12.906985 transaction_middleware-0.1.4/src/transaction_middleware/transaction_middleware.py
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 transaction_middleware-0.1.4/PKG-INFO
```

### Comparing `transaction_middleware-0.1.3/LICENSE` & `transaction_middleware-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.3/README.md` & `transaction_middleware-0.1.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# auth-middleware
+# transaction-middleware
 
 Async Transaction Middleware for FastAPI/Starlette.
 
 ## Installation
 
 Using pip:
```

### Comparing `transaction_middleware-0.1.3/pyproject.toml` & `transaction_middleware-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 [tool.poetry]
 name = "transaction-middleware"
-version = "0.1.3"
+version = "0.1.4"
 description = "Async Transaction Middleware for FastAPI/Starlette"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "transaction_middleware", from = "src"}]
 license = "MIT"
 homepage = "https://impalah.github.io/transaction-middleware/"
 repository = "https://github.com/impalah/transaction-middleware"
 documentation = "https://impalah.github.io/transaction-middleware/"
 keywords = ["transaction", "middleware", "fastapi", "starlette"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Framework :: FastAPI",
     "Programming Language :: Python :: 3",
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
-
-
-
 [tool.poetry.dependencies]
 python = ">=3.10"
 fastapi = ">=0.105.0"
 python-dotenv = "^1.0.0"
 svix-ksuid = ">=0.6.2"
 pydantic = {extras = ["email"], version = ">=2.5.3"}
 loguru = ">=0.7.2"
```

### Comparing `transaction_middleware-0.1.3/src/transaction_middleware/settings.py` & `transaction_middleware-0.1.4/src/transaction_middleware/settings.py`

 * *Files identical despite different names*

### Comparing `transaction_middleware-0.1.3/src/transaction_middleware/transaction_middleware.py` & `transaction_middleware-0.1.4/src/transaction_middleware/transaction_middleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,24 +32,25 @@
         request: Request,
         call_next: RequestResponseEndpoint,
     ) -> Response | JSONResponse:
 
         # Check if transaction ID is already in the request
         transaction_id = request.headers.get(self.header_name)
 
-        # Generate a new transaction Id if it doesnt exists and is required
-        if transaction_id is None and getattr(
-            request.scope["endpoint"], "create_transaction_id", False
-        ):
-            # TODO: allow to specify a custom transaction ID generator
-            transaction_id = str(Ksuid())
-            request.state.transaction_id = transaction_id
-        elif transaction_id is not None:
-            request.state.transaction_id = transaction_id
+        logger.debug("Transaction ID from request: {}", transaction_id)
 
         # Process the request
         response = await call_next(request)
 
+        transaction_id = (
+            request.state.transaction_id
+            if hasattr(request.state, "transaction_id")
+            else None
+        )
+
+        logger.debug("Transaction ID after request: {}", transaction_id)
+
         # Add transaction ID to the response
         if transaction_id:
+            logger.debug(f"Adding Transaction ID to response: {transaction_id}")
             response.headers[self.header_name] = transaction_id
         return response
```

### Comparing `transaction_middleware-0.1.3/PKG-INFO` & `transaction_middleware-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: transaction-middleware
-Version: 0.1.3
+Version: 0.1.4
 Summary: Async Transaction Middleware for FastAPI/Starlette
 Home-page: https://impalah.github.io/transaction-middleware/
 License: MIT
 Keywords: transaction,middleware,fastapi,starlette
 Author: impalah
 Author-email: impalah@gmail.com
 Requires-Python: >=3.10
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -25,15 +25,15 @@
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: svix-ksuid (>=0.6.2)
 Project-URL: Documentation, https://impalah.github.io/transaction-middleware/
 Project-URL: Repository, https://github.com/impalah/transaction-middleware
 Project-URL: Source, https://github.com/impalah/transaction-middleware
 Description-Content-Type: text/markdown
 
-# auth-middleware
+# transaction-middleware
 
 Async Transaction Middleware for FastAPI/Starlette.
 
 ## Installation
 
 Using pip:
```

