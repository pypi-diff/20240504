# Comparing `tmp/pyretries-0.2.8.tar.gz` & `tmp/pyretries-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyretries-0.2.8.tar", max compression
+gzip compressed data, was "pyretries-0.2.9.tar", max compression
```

## Comparing `pyretries-0.2.8.tar` & `pyretries-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      877 2023-10-13 17:48:07.558690 pyretries-0.2.8/README.md
--rw-r--r--   0        0        0     1510 2023-10-13 17:48:07.558690 pyretries-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      660 2023-10-13 17:48:07.558690 pyretries-0.2.8/pyretries/__init__.py
--rw-r--r--   0        0        0      311 2023-10-13 17:48:07.558690 pyretries-0.2.8/pyretries/exceptions.py
--rw-r--r--   0        0        0    13041 2023-10-13 17:48:07.558690 pyretries-0.2.8/pyretries/retry.py
--rw-r--r--   0        0        0     9156 2023-10-13 17:48:07.558690 pyretries-0.2.8/pyretries/strategy.py
--rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 pyretries-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      877 2023-12-18 08:14:33.389082 pyretries-0.2.9/README.md
+-rw-r--r--   0        0        0     1524 2023-12-18 08:14:33.393082 pyretries-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      660 2023-12-18 08:14:33.393082 pyretries-0.2.9/pyretries/__init__.py
+-rw-r--r--   0        0        0      311 2023-12-18 08:14:33.393082 pyretries-0.2.9/pyretries/exceptions.py
+-rw-r--r--   0        0        0    13241 2023-12-18 08:14:33.393082 pyretries-0.2.9/pyretries/retry.py
+-rw-r--r--   0        0        0     9156 2023-12-18 08:14:33.393082 pyretries-0.2.9/pyretries/strategy.py
+-rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 pyretries-0.2.9/PKG-INFO
```

### Comparing `pyretries-0.2.8/README.md` & `pyretries-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyretries-0.2.8/pyproject.toml` & `pyretries-0.2.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyretries"
-version = "0.2.8"
+version = "0.2.9"
 description = "A Python retry package based on strategies"
 authors = ["Ben Mezger <me@benmezger.nl>"]
 readme = "README.md"
 packages = [{include = "pyretries"}]
 homepage = "https://benmezger.github.io/pyretries"
 repository = "https://github.com/benmezger/pyretries"
 documentation = "https://benmezger.github.io/pyretries"
@@ -18,18 +18,18 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 black = "^23.9.1"
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 pyright = "^1.1.330.post0"
-pytest-asyncio = "^0.21.1"
+pytest-asyncio = ">=0.21.1,<0.24.0"
 pytest-cov = "^4.1.0"
 mkdocs = "^1.5.3"
-mkdocstrings = {version = "^0.23.0", extras = ["python"]}
+mkdocstrings = {version = ">=0.23,<0.25", extras = ["python"]}
 mkdocs-material = "^9.4.4"
 freezegun = "^1.2.2"
 taskipy = "^1.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyretries-0.2.8/pyretries/__init__.py` & `pyretries-0.2.9/pyretries/__init__.py`

 * *Files identical despite different names*

### Comparing `pyretries-0.2.8/pyretries/retry.py` & `pyretries-0.2.9/pyretries/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,18 @@
                 *(state.args or ()), **(state.kwargs or {})
             )
         except Exception as err:
             exception = err
 
         self._post_exec(state, exception)
 
-    async def __call__(
+    # NOTE: currently, the abtract method is a sync, and here we are defining async.
+    # Pyright will alert about this, so we ignore the type for now until we
+    # have a fix for it
+    async def __call__(  # type:ignore
         self, func: FuncT[ReturnT], *args: t.Any, **kwargs: t.Any
     ) -> ReturnT | Exception | None:
         """
         Executes `func` and applies strategies
 
         Args:
             func: Address to function
```

### Comparing `pyretries-0.2.8/pyretries/strategy.py` & `pyretries-0.2.9/pyretries/strategy.py`

 * *Files identical despite different names*

### Comparing `pyretries-0.2.8/PKG-INFO` & `pyretries-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyretries
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python retry package based on strategies
 Home-page: https://benmezger.github.io/pyretries
 Keywords: retry,python
 Author: Ben Mezger
 Author-email: me@benmezger.nl
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
```

