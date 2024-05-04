# Comparing `tmp/sshared-0.3.0.tar.gz` & `tmp/sshared-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshared-0.3.0.tar", max compression
+gzip compressed data, was "sshared-0.4.0.tar", max compression
```

## Comparing `sshared-0.3.0.tar` & `sshared-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0     1063 2024-04-14 00:41:51.517836 sshared-0.3.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-14 00:41:51.517836 sshared-0.3.0/README.md
--rw-r--r--   0        0        0     1111 2024-04-14 00:41:51.517836 sshared-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/__init__.py
--rw-r--r--   0        0        0       74 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/mongo/__init__.py
--rw-r--r--   0        0        0     5962 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/mongo/document.py
--rw-r--r--   0        0        0      263 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/mongo/meta.py
--rw-r--r--   0        0        0     1687 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/retry/asyncio.py
--rw-r--r--   0        0        0      229 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/retry/event.py
--rw-r--r--   0        0        0     1660 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/retry/sync.py
--rw-r--r--   0        0        0      249 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/struct.py
--rw-r--r--   0        0        0      139 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/time.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 sshared-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-04 01:11:31.319594 sshared-0.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-04 01:11:31.319594 sshared-0.4.0/README.md
+-rw-r--r--   0        0        0     1180 2024-05-04 01:11:31.319594 sshared-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/api/__init__.py
+-rw-r--r--   0        0        0     2049 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/api/exception_handlers.py
+-rw-r--r--   0        0        0      287 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/api/openapi.py
+-rw-r--r--   0        0        0      724 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/api/response.py
+-rw-r--r--   0        0        0      603 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/api/response_spec.py
+-rw-r--r--   0        0        0      342 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/api/structs.py
+-rw-r--r--   0        0        0       74 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/mongo/__init__.py
+-rw-r--r--   0        0        0     5962 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/mongo/document.py
+-rw-r--r--   0        0        0      263 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/mongo/meta.py
+-rw-r--r--   0        0        0     1687 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/retry/asyncio.py
+-rw-r--r--   0        0        0      229 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/retry/event.py
+-rw-r--r--   0        0        0     1660 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/retry/sync.py
+-rw-r--r--   0        0        0      249 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/struct.py
+-rw-r--r--   0        0        0      237 2024-05-04 01:11:31.319594 sshared-0.4.0/sshared/time.py
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 sshared-0.4.0/PKG-INFO
```

### Comparing `sshared-0.3.0/LICENSE` & `sshared-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshared-0.3.0/pyproject.toml` & `sshared-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sshared"
-version = "0.3.0"
+version = "0.4.0"
 description = "后端共享组件"
 authors = ["yezi <yehaowei20060411@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FHU-yezi/sshared"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -14,21 +14,23 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 msgspec = "^0.18.0"
 typing-extensions = "^4.10.0"
 motor = { version ="^3.3.0", optional = true }
+litestar = { version ="^2.8.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 pyright = "^1.1.0"
 
 [tool.poetry.extras]
 mongo = ["motor"]
+api = ["litestar"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `sshared-0.3.0/sshared/mongo/document.py` & `sshared-0.4.0/sshared/mongo/document.py`

 * *Files identical despite different names*

### Comparing `sshared-0.3.0/sshared/retry/asyncio.py` & `sshared-0.4.0/sshared/retry/asyncio.py`

 * *Files identical despite different names*

### Comparing `sshared-0.3.0/sshared/retry/sync.py` & `sshared-0.4.0/sshared/retry/sync.py`

 * *Files identical despite different names*

### Comparing `sshared-0.3.0/PKG-INFO` & `sshared-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshared
-Version: 0.3.0
+Version: 0.4.0
 Summary: 后端共享组件
 Home-page: https://github.com/FHU-yezi/sshared
 License: MIT
 Author: yezi
 Author-email: yehaowei20060411@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
+Provides-Extra: api
 Provides-Extra: mongo
+Requires-Dist: litestar (>=2.8.0,<3.0.0) ; extra == "api"
 Requires-Dist: motor (>=3.3.0,<4.0.0) ; extra == "mongo"
 Requires-Dist: msgspec (>=0.18.0,<0.19.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Project-URL: Repository, https://github.com/FHU-yezi/sshared
 Description-Content-Type: text/markdown
```

