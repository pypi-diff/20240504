# Comparing `tmp/logiclayer-0.3.3.tar.gz` & `tmp/logiclayer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer-0.3.3.tar", max compression
+gzip compressed data, was "logiclayer-0.3.4.tar", max compression
```

## Comparing `logiclayer-0.3.3.tar` & `logiclayer-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-19 17:21:53.322917 logiclayer-0.3.3/LICENSE
--rw-r--r--   0        0        0     3574 2024-04-19 17:21:53.322917 logiclayer-0.3.3/PACKAGE.md
--rw-r--r--   0        0        0      639 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/__init__.py
--rw-r--r--   0        0        0      894 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/auth.py
--rw-r--r--   0        0        0      623 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/common.py
--rw-r--r--   0        0        0     2689 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/decorators.py
--rw-r--r--   0        0        0     5201 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/logiclayer.py
--rw-r--r--   0        0        0     4058 2024-04-19 17:21:53.322917 logiclayer-0.3.3/logiclayer/module.py
--rw-r--r--   0        0        0      580 2024-04-19 17:21:53.326917 logiclayer-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 logiclayer-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-03 23:00:48.417325 logiclayer-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3574 2024-05-03 23:00:48.417325 logiclayer-0.3.4/PACKAGE.md
+-rw-r--r--   0        0        0      639 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/__init__.py
+-rw-r--r--   0        0        0      894 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/auth.py
+-rw-r--r--   0        0        0      623 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/common.py
+-rw-r--r--   0        0        0     2689 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/decorators.py
+-rw-r--r--   0        0        0     5314 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/logiclayer.py
+-rw-r--r--   0        0        0     4154 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/module.py
+-rw-r--r--   0        0        0      600 2024-05-03 23:00:48.421326 logiclayer-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 logiclayer-0.3.4/PKG-INFO
```

### Comparing `logiclayer-0.3.3/LICENSE` & `logiclayer-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.3/PACKAGE.md` & `logiclayer-0.3.4/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.3/logiclayer/__init__.py` & `logiclayer-0.3.4/logiclayer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """LogicLayer module."""
 
 __title__ = "logiclayer"
 __description__ = (
     "A framework to quickly compose and use multiple functionalities as endpoints."
 )
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 __all__ = (
     "AuthProvider",
     "AuthToken",
     "AuthTokenType",
     "exception_handler",
     "healthcheck",
```

### Comparing `logiclayer-0.3.3/logiclayer/auth.py` & `logiclayer-0.3.4/logiclayer/auth.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.3/logiclayer/common.py` & `logiclayer-0.3.4/logiclayer/common.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.3/logiclayer/decorators.py` & `logiclayer-0.3.4/logiclayer/decorators.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.3/logiclayer/logiclayer.py` & `logiclayer-0.3.4/logiclayer/logiclayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,13 +138,17 @@
         except Exception as exc:
             logger.error("Healthcheck failure", exc_info=exc)
         else:
             return Response(status_code=HTTP_204_NO_CONTENT)
 
         raise HTTPException(500, "One of the healthchecks failed.")
 
+    def healthcheck(self, fn: "CallableMayReturnCoroutine[bool]"):
+        self.add_check(fn)
+        return fn
+
     def route(self, path: str, **kwargs):
         def route_decorator(fn):
             self.add_route(path, fn, **kwargs)
             return fn
 
         return route_decorator
```

### Comparing `logiclayer-0.3.3/logiclayer/module.py` & `logiclayer-0.3.4/logiclayer/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses as dcls
 from collections import defaultdict
 from enum import Enum, auto
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type, Union
 
 from fastapi import APIRouter
+from pydantic import BaseModel, ConfigDict
 
 from .auth import AuthProvider, VoidAuthProvider
 from .common import LOGICLAYER_METHOD_ATTR, CallableMayReturnCoroutine
 
 if TYPE_CHECKING:
     from .logiclayer import LogicLayer
 
@@ -114,13 +115,14 @@
 
         for item in self._llroutes:
             router.add_api_route(item.path, item.bound_to(self), **item.kwargs)
 
         app.include_router(router, **kwargs)
 
 
-@dcls.dataclass
-class ModuleStatus:
+class ModuleStatus(BaseModel):
+    model_config = ConfigDict(extra="allow", frozen=True)
+
     module: str
     version: str
     debug: Union[bool, dict]
-    extras: dict
+    status: str
```

### Comparing `logiclayer-0.3.3/PKG-INFO` & `logiclayer-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logiclayer
-Version: 0.3.3
+Version: 0.3.4
 Summary: A framework to quickly compose and use multiple functionalities as endpoints.
 Home-page: https://github.com/Datawheel/logiclayer
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncio (>=3.4.0,<4.0.0)
 Requires-Dist: fastapi (>=0.100,<1.0)
+Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Project-URL: Repository, https://github.com/Datawheel/logiclayer
 Description-Content-Type: text/markdown
 
 A simple framework to quickly compose and use multiple functionalities as endpoints.  
 LogicLayer is built upon FastAPI to provide a simple way to group functionalities into reusable modules.
 
 <p>
```

