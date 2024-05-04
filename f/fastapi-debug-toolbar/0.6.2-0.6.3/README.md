# Comparing `tmp/fastapi_debug_toolbar-0.6.2.tar.gz` & `tmp/fastapi_debug_toolbar-0.6.3.tar.gz`

## Comparing `fastapi_debug_toolbar-0.6.2.tar` & `fastapi_debug_toolbar-0.6.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/api.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/py.typed
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/responses.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/settings.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/toolbar.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/types.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/utils.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/headers.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/logging.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/profiling.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/redirects.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/request.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/routes.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/settings.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/sql.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/sqlalchemy.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/timer.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/tortoise.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/versions.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/css/print.css
--rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/css/toolbar.css
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/img/icon-green.svg
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/img/icon-white.svg
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/redirect.js
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/refresh.js
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/timer.js
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/toolbar.js
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/utils.js
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/versions.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/base.html
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/redirect.html
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/includes/panel_button.html
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/includes/panel_content.html
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/headers.html
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/logging.html
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/profiling.html
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/request.html
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/routes.html
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/settings.html
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/sql.html
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/timer.html
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/versions.html
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/.gitignore
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/LICENSE
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/README.md
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/api.py
+-rwxr-xr-x   0        0        0      740 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/dependencies.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/py.typed
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/responses.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/settings.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/toolbar.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/types.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/utils.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/headers.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/logging.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/profiling.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/redirects.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/request.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/routes.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/settings.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/sql.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/sqlalchemy.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/timer.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/tortoise.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/versions.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/css/print.css
+-rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/css/toolbar.css
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/img/icon-green.svg
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/img/icon-white.svg
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/redirect.js
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/refresh.js
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/timer.js
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/toolbar.js
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/utils.js
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/versions.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/base.html
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/redirect.html
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/includes/panel_button.html
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/includes/panel_content.html
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/headers.html
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/logging.html
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/profiling.html
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/request.html
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/routes.html
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/settings.html
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/sql.html
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/timer.html
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/versions.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/README.md
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 fastapi_debug_toolbar-0.6.3/PKG-INFO
```

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/api.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/api.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/middleware.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/settings.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/toolbar.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/toolbar.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/utils.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/__init__.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/headers.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/logging.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/profiling.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/profiling.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     title = "Profiling"
     template = "panels/profiling.html"
 
     async def process_request(self, request: Request) -> Response:
         self.profiler = Profiler(**self.toolbar.settings.PROFILER_OPTIONS)
         is_async = is_coroutine(request["route"].endpoint)
 
-        async def call(func: t.Callable) -> None:
-            await run_in_threadpool(func) if not is_async else func()
+        async def call(f: t.Callable) -> None:
+            await run_in_threadpool(f) if not is_async else f()
 
         await call(self.profiler.start)
 
         try:
             response = await super().process_request(request)
         finally:
             await call(self.profiler.stop)
```

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/redirects.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/redirects.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/request.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/request.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/sql.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/sql.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/sqlalchemy.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/sqlalchemy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 import typing as t
-from contextlib import AsyncExitStack
 from time import perf_counter
 
-from fastapi import HTTPException, Request, Response
-from fastapi.dependencies.utils import solve_dependencies
+from fastapi import Request, Response
 from sqlalchemy import event
 from sqlalchemy.engine import Connection, Engine, ExecutionContext
+from sqlalchemy.exc import UnboundExecutionError
+from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Session
 
+from debug_toolbar.dependencies import get_dependencies
 from debug_toolbar.panels.sql import SQLPanel
 
 
 class SQLAlchemyPanel(SQLPanel):
     title = "SQLAlchemy"
 
     def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
@@ -36,36 +39,36 @@
             )
             * 1000,
             "sql": context.statement,
             "params": context.parameters,
         }
         self.add_query(str(context.engine.url), query)
 
+    def add_bind(self, bind: Connection | Engine):
+        if isinstance(bind, Connection):
+            self.engines.add(bind.engine)
+        else:
+            self.engines.add(bind)
+
     async def add_engines(self, request: Request):
-        route = request["route"]
+        dependencies = await get_dependencies(request)
 
-        if hasattr(route, "dependant"):
-            try:
-                solved_result = await solve_dependencies(
-                    request=request,
-                    dependant=route.dependant,
-                    dependency_overrides_provider=route.dependency_overrides_provider,
-                    async_exit_stack=AsyncExitStack(),
-                )
-            except HTTPException:
-                pass
-            else:
-                for value in solved_result[0].values():
-                    if isinstance(value, Session):
-                        bind = value.get_bind()
+        if dependencies is not None:
+            for value in dependencies.values():
+                if isinstance(value, AsyncSession):
+                    value = value.sync_session
 
-                        if isinstance(bind, Connection):
-                            self.engines.add(bind.engine)
-                        else:
-                            self.engines.add(bind)
+                if isinstance(value, Session):
+                    try:
+                        bind = value.get_bind()
+                    except UnboundExecutionError:
+                        for bind in value._Session__binds.values():  # type: ignore[attr-defined]
+                            self.add_bind(bind)
+                    else:
+                        self.add_bind(bind)
 
     async def process_request(self, request: Request) -> Response:
         await self.add_engines(request)
 
         for engine in self.engines:
             self.register(engine)
         try:
```

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/timer.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/tortoise.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/tortoise.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/panels/versions.py` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/css/toolbar.css` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/css/toolbar.css`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/img/icon-green.svg` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/img/icon-green.svg`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/img/icon-white.svg` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/refresh.js` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/refresh.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/timer.js` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/timer.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/toolbar.js` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/toolbar.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/utils.js` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/utils.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/statics/js/versions.js` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/statics/js/versions.js`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/base.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/redirect.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/includes/panel_button.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/includes/panel_button.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/headers.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/headers.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/logging.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/logging.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/request.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/request.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/routes.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/routes.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/settings.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/settings.html`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   <thead>
     <tr>
       <th>Key</th>
       <th>Value</th>
     </tr>
   </thead>
   <tbody>
-    {% for key, value in settings.dict(exclude=exclude).items() %}
+    {% for key, value in settings.model_dump(exclude=exclude).items() %}
       <tr>
         <td>{{ key|escape }}</td>
         <td><code>{{ value|pprint|escape }}</code></td>
       </tr>
     {% endfor %}
   </tbody>
 </table>
```

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/sql.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/sql.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/timer.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/timer.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/debug_toolbar/templates/panels/versions.html` & `fastapi_debug_toolbar-0.6.3/debug_toolbar/templates/panels/versions.html`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/LICENSE` & `fastapi_debug_toolbar-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/README.md` & `fastapi_debug_toolbar-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/pyproject.toml` & `fastapi_debug_toolbar-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_debug_toolbar-0.6.2/PKG-INFO` & `fastapi_debug_toolbar-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi-debug-toolbar
-Version: 0.6.2
+Version: 0.6.3
 Summary: A debug toolbar for FastAPI.
 Project-URL: homepage, https://github.com/mongkok/fastapi-debug-toolbar
 Project-URL: repository, https://github.com/mongkok/fastapi-debug-toolbar
 Project-URL: documentation, https://fastapi-debug-toolbar.domake.io
 Project-URL: changelog, https://fastapi-debug-toolbar.domake.io/changelog/
 Author-email: Dani <dani@domake.io>
 License-Expression: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-debug-toolbar Version: 0.6.2 Summary: A
+Metadata-Version: 2.3 Name: fastapi-debug-toolbar Version: 0.6.3 Summary: A
 debug toolbar for FastAPI. Project-URL: homepage, https://github.com/mongkok/
 fastapi-debug-toolbar Project-URL: repository, https://github.com/mongkok/
 fastapi-debug-toolbar Project-URL: documentation, https://fastapi-debug-
 toolbar.domake.io Project-URL: changelog, https://fastapi-debug-
 toolbar.domake.io/changelog/ Author-email: Dani
 domake.io> License-Expression: BSD-3-Clause License-File: LICENSE Keywords:
 debug,fastapi,profiling Classifier: Development Status :: 2 - Pre-Alpha
```

