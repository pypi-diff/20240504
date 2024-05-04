# Comparing `tmp/notional-0.8.1.tar.gz` & `tmp/notional-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notional-0.8.1.tar", max compression
+gzip compressed data, was "notional-0.8.2.tar", max compression
```

## Comparing `notional-0.8.1.tar` & `notional-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2021-09-20 19:35:00.000000 notional-0.8.1/LICENSE
--rw-r--r--   0        0        0     2357 2023-01-05 14:29:43.601551 notional-0.8.1/README.md
--rw-r--r--   0        0        0     1559 2024-04-07 02:00:02.886877 notional-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      368 2023-08-02 03:16:34.247660 notional-0.8.1/src/notional/__init__.py
--rw-r--r--   0        0        0      294 2023-03-17 13:04:42.774343 notional-0.8.1/src/notional/__main__.py
--rw-r--r--   0        0        0    22381 2024-04-07 01:59:59.936119 notional-0.8.1/src/notional/blocks.py
--rw-r--r--   0        0        0     9915 2024-04-07 01:59:59.936964 notional-0.8.1/src/notional/core.py
--rw-r--r--   0        0        0     4844 2024-04-07 01:59:59.937794 notional-0.8.1/src/notional/iterator.py
--rw-r--r--   0        0        0    13452 2024-04-07 01:59:59.938521 notional-0.8.1/src/notional/orm.py
--rw-r--r--   0        0        0    18566 2023-12-27 15:42:54.107393 notional-0.8.1/src/notional/parser.py
--rw-r--r--   0        0        0    10053 2024-04-07 01:59:59.939658 notional-0.8.1/src/notional/query.py
--rw-r--r--   0        0        0     7943 2024-04-07 01:59:59.940353 notional-0.8.1/src/notional/schema.py
--rw-r--r--   0        0        0    17930 2024-04-07 01:59:59.941235 notional-0.8.1/src/notional/session.py
--rw-r--r--   0        0        0     9580 2024-04-07 02:00:02.887260 notional-0.8.1/src/notional/text.py
--rw-r--r--   0        0        0    30793 2024-04-07 01:59:59.942819 notional-0.8.1/src/notional/types.py
--rw-r--r--   0        0        0     1374 2024-04-07 01:59:59.943721 notional-0.8.1/src/notional/user.py
--rw-r--r--   0        0        0     1299 2024-04-07 01:59:59.944620 notional-0.8.1/src/notional/util.py
--rw-r--r--   0        0        0     1697 2023-03-19 04:03:23.147593 notional-0.8.1/src/notional/version.py
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 notional-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-09-20 19:35:00.000000 notional-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2357 2023-01-05 14:29:43.601551 notional-0.8.2/README.md
+-rw-r--r--   0        0        0     1561 2024-05-04 14:11:59.502067 notional-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-08-02 03:16:34.247660 notional-0.8.2/src/notional/__init__.py
+-rw-r--r--   0        0        0      294 2023-03-17 13:04:42.774343 notional-0.8.2/src/notional/__main__.py
+-rw-r--r--   0        0        0    22381 2024-05-04 13:58:27.163734 notional-0.8.2/src/notional/blocks.py
+-rw-r--r--   0        0        0     9915 2024-05-04 13:58:27.165290 notional-0.8.2/src/notional/core.py
+-rw-r--r--   0        0        0     4844 2024-05-04 13:58:27.167979 notional-0.8.2/src/notional/iterator.py
+-rw-r--r--   0        0        0    13452 2024-05-04 13:58:27.170079 notional-0.8.2/src/notional/orm.py
+-rw-r--r--   0        0        0    18566 2023-12-27 15:42:54.107393 notional-0.8.2/src/notional/parser.py
+-rw-r--r--   0        0        0    10053 2024-05-04 13:58:27.172223 notional-0.8.2/src/notional/query.py
+-rw-r--r--   0        0        0     7943 2024-05-04 13:58:27.172940 notional-0.8.2/src/notional/schema.py
+-rw-r--r--   0        0        0    18378 2024-05-04 13:58:38.297254 notional-0.8.2/src/notional/session.py
+-rw-r--r--   0        0        0     9580 2024-05-04 13:58:27.175825 notional-0.8.2/src/notional/text.py
+-rw-r--r--   0        0        0    30793 2024-05-04 13:58:27.177429 notional-0.8.2/src/notional/types.py
+-rw-r--r--   0        0        0     1374 2024-05-04 13:58:27.178496 notional-0.8.2/src/notional/user.py
+-rw-r--r--   0        0        0     1299 2024-05-04 13:58:27.179769 notional-0.8.2/src/notional/util.py
+-rw-r--r--   0        0        0     1697 2023-03-19 04:03:23.147593 notional-0.8.2/src/notional/version.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 notional-0.8.2/PKG-INFO
```

### Comparing `notional-0.8.1/LICENSE` & `notional-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/README.md` & `notional-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/pyproject.toml` & `notional-0.8.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notional"
-version = "0.8.1"
+version = "0.8.2"
 description = "A high-level interface for the Notion SDK."
 license = "MIT"
 authors = ["Jason Heddings <jheddings@gmail.com>"]
 repository = "https://github.com/jheddings/notional/"
 documentation = "https://jheddings.github.io/notional/"
 readme = "README.md"
 classifiers=[
@@ -14,30 +14,30 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 notion-client = "^2.2.1"
 pydantic = "^1.10.15"
 html5lib = "^1.1"
 urllib3 = "^1.26.18"
-emoji = "^2.11.0"
+emoji = "^2.11.1"
 
 [tool.poetry.group.dev.dependencies]
 GitPython = "^3.1.43"
 pre-commit = "^3.5.0"
-pytest = "^8.1.0"
-coverage = "^7.4.4"
+pytest = "^8.2.0"
+coverage = "^7.5.0"
 pytest-vcr = "^1.0.2"
-mypy = "^1.9.0"
-ruff = "^0.3.5"
+mypy = "^1.10.0"
+ruff = "^0.4.3"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.5.3"
-mkdocstrings = "^0.24.2"
-mkdocs-material = "^9.5.17"
-mkdocstrings-python = "^1.9.2"
+mkdocs = "^1.6.0"
+mkdocstrings = "^0.25.0"
+mkdocs-material = "^9.5.21"
+mkdocstrings-python = "^1.10.0"
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
 
 [tool.ruff.lint]
 select = [
```

### Comparing `notional-0.8.1/src/notional/blocks.py` & `notional-0.8.2/src/notional/blocks.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/core.py` & `notional-0.8.2/src/notional/core.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/iterator.py` & `notional-0.8.2/src/notional/iterator.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/orm.py` & `notional-0.8.2/src/notional/orm.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/parser.py` & `notional-0.8.2/src/notional/parser.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/query.py` & `notional-0.8.2/src/notional/query.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/schema.py` & `notional-0.8.2/src/notional/schema.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/session.py` & `notional-0.8.2/src/notional/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,32 +112,41 @@
         """Notional interface to the API 'blocks/children' endpoint."""
 
         def __call__(self):
             """Return the underlying endpoint in the Notion SDK."""
             return self.session.client.blocks.children
 
         # https://developers.notion.com/reference/patch-block-children
-        def append(self, parent, *blocks: Block):
+        def append(self, parent, *blocks: Block, after: Block = None):
             """Add the given blocks as children of the specified parent.
 
+            If `after` keyword is specified, they are appended after given Block.
+
             The blocks info will be refreshed based on returned data.
 
             `parent` may be any suitable `ObjectReference` type.
             """
 
             parent_id = ObjectReference[parent].id
 
             children = [block.dict() for block in blocks if block is not None]
 
             logger.info("Appending %d blocks to %s ...", len(children), parent_id)
 
-            data = self().append(block_id=parent_id, children=children)
+            if after is None:
+                data = self().append(block_id=parent_id, children=children)
+            else:
+                after_id = str(after.id) if isinstance(after, Block) else after
+                data = self().append(
+                    block_id=parent_id, children=children, after=after_id
+                )
 
             if "results" in data:
-                if len(blocks) == len(data["results"]):
+                # in case of `after`, there is second result
+                if len(blocks) == len(data["results"]) or after is not None:
                     for idx in range(len(blocks)):
                         block = blocks[idx]
                         result = data["results"][idx]
                         block.refresh(**result)
 
                 else:
                     logger.warning("Unable to refresh results; size mismatch")
```

### Comparing `notional-0.8.1/src/notional/text.py` & `notional-0.8.2/src/notional/text.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/types.py` & `notional-0.8.2/src/notional/types.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/user.py` & `notional-0.8.2/src/notional/user.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/util.py` & `notional-0.8.2/src/notional/util.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/src/notional/version.py` & `notional-0.8.2/src/notional/version.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.1/PKG-INFO` & `notional-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: notional
-Version: 0.8.1
+Version: 0.8.2
 Summary: A high-level interface for the Notion SDK.
 Home-page: https://github.com/jheddings/notional/
 License: MIT
 Author: Jason Heddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: emoji (>=2.11.0,<3.0.0)
+Requires-Dist: emoji (>=2.11.1,<3.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: notion-client (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic (>=1.10.15,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Project-URL: Documentation, https://jheddings.github.io/notional/
 Project-URL: Repository, https://github.com/jheddings/notional/
 Description-Content-Type: text/markdown
```

