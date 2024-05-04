# Comparing `tmp/tesseract_olap-0.9.4.tar.gz` & `tmp/tesseract_olap-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.9.4.tar", max compression
+gzip compressed data, was "tesseract_olap-0.9.5.tar", max compression
```

## Comparing `tesseract_olap-0.9.4.tar` & `tesseract_olap-0.9.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2589 2024-04-19 21:02:01.618058 tesseract_olap-0.9.4/PACKAGE.md
--rw-r--r--   0        0        0     1320 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      562 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/__init__.py
--rw-r--r--   0        0        0      377 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0     2707 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/cache.py
--rw-r--r--   0        0        0       79 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     7219 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     2714 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0    20624 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     3743 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0     2761 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/valkey.py
--rw-r--r--   0        0        0      571 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0     2461 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      385 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      787 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/backend.py
--rw-r--r--   0        0        0     3682 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/query.py
--rw-r--r--   0        0        0     3712 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/schema.py
--rw-r--r--   0        0        0      741 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/server.py
--rw-r--r--   0        0        0      511 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0    11052 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     6492 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     4550 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1166 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     3318 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0    12543 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    13039 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0    10178 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1763 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3587 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     4744 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     2542 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     9528 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0    11992 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/parser.py
--rw-r--r--   0        0        0     5306 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/public.py
--rw-r--r--   0        0        0     4824 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23758 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    18520 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0     4674 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     3713 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     2589 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/PACKAGE.md
+-rw-r--r--   0        0        0     1320 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      562 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0      377 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0     2707 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/cache.py
+-rw-r--r--   0        0        0       79 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     7219 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     2714 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0    20624 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     3743 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0     2761 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/valkey.py
+-rw-r--r--   0        0        0      571 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0     2461 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      787 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/__init__.py
+-rw-r--r--   0        0        0     1596 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/backend.py
+-rw-r--r--   0        0        0     3682 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/query.py
+-rw-r--r--   0        0        0     3712 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/schema.py
+-rw-r--r--   0        0        0      741 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/server.py
+-rw-r--r--   0        0        0      511 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0    11052 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     6259 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     4284 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1166 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     3318 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0    12543 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    13039 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0    10178 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1763 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5432 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3587 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     4744 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     2542 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     9796 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0    11992 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/parser.py
+-rw-r--r--   0        0        0     5576 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/public.py
+-rw-r--r--   0        0        0     4824 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23758 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    18520 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0     4674 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     3713 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.5/PKG-INFO
```

### Comparing `tesseract_olap-0.9.4/PACKAGE.md` & `tesseract_olap-0.9.5/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/pyproject.toml` & `tesseract_olap-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.9.4"
+version = "0.9.5"
 description = "A simple OLAP library."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
   "Jelmy Hermosilla <jelmy@datawheel.us>",
 ]
 maintainers = [
   "Francisco Abarzua <francisco@datawheel.us>",
@@ -33,15 +33,15 @@
 redis = ["redis"]
 
 [tool.poetry.group.dev.dependencies]
 clickhouse-cityhash = "^1.0.2.4"
 clickhouse-driver = "^0.2.0"
 fastapi = ">=0.100.0"
 granian = {extras = ["reload"], version = "^1.1.2"}
-logiclayer = "^0.3.2"
+logiclayer = "^0.3.4"
 lxml-stubs = "^0.4.0"
 pytest = "^8.0.0"
 pytest-asyncio = "^0.20.0"
 redis = "^5.0.3"
 ruff = "^0.3.0"
 sqlparse = "^0.4.0"
 tomli = "^2.0.1"
```

### Comparing `tesseract_olap-0.9.4/tesseract_olap/__init__.py` & `tesseract_olap-0.9.5/tesseract_olap/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = "tesseract-olap"
 __description__ = "A simple OLAP library."
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 __all__ = (
     "DataRequest",
     "DataRequestParams",
     "MembersRequest",
     "MembersRequestParams",
     "NotAuthorized",
```

### Comparing `tesseract_olap-0.9.4/tesseract_olap/backend/cache.py` & `tesseract_olap-0.9.5/tesseract_olap/backend/cache.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/backend/models.py` & `tesseract_olap-0.9.5/tesseract_olap/backend/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/backend/valkey.py` & `tesseract_olap-0.9.5/tesseract_olap/backend/valkey.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/common/__init__.py` & `tesseract_olap-0.9.5/tesseract_olap/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/common/strings.py` & `tesseract_olap-0.9.5/tesseract_olap/common/strings.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/exceptions/__init__.py` & `tesseract_olap-0.9.5/tesseract_olap/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/exceptions/backend.py` & `tesseract_olap-0.9.5/tesseract_olap/exceptions/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/exceptions/query.py` & `tesseract_olap-0.9.5/tesseract_olap/exceptions/query.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/exceptions/schema.py` & `tesseract_olap-0.9.5/tesseract_olap/exceptions/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/exceptions/server.py` & `tesseract_olap-0.9.5/tesseract_olap/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.9.5/tesseract_olap/logiclayer/dependencies.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.9.5/tesseract_olap/logiclayer/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import logiclayer as ll
 from fastapi import Depends, Request
 from fastapi.responses import JSONResponse, RedirectResponse
 
-from tesseract_olap import __version__ as tesseract_version
+import tesseract_olap as olap
 from tesseract_olap.exceptions import QueryError, TesseractError
 from tesseract_olap.exceptions.query import NotAuthorized
 from tesseract_olap.query import DataQuery, DataRequest, MembersQuery, MembersRequest
 from tesseract_olap.schema import TesseractCube, TesseractSchema
 from tesseract_olap.server import OlapServer
 
 from .dependencies import auth_token, dataquery_params, membersquery_params
 from .response import (
     MembersResModel,
     ResponseFormat,
-    StatusResModel,
     data_response,
     members_response,
 )
 
+DEBUG_INFO = {
+    "git_branch": os.getenv("GIT_BRANCH", ""),
+    "git_hash": os.getenv("GIT_HASH", ""),
+}
+
 
 class TesseractModule(ll.LogicLayerModule):
     """Tesseract OLAP server module for LogicLayer.
 
     It must be initialized with a :class:`logiclayer.OlapServer` instance, but
     can also be created directly with the schema path and the connection string
     using the helper method `TesseractModule.new(connection, schema)`.
@@ -50,36 +54,26 @@
         """Creates a new :class:`TesseractModule` instance from the strings with
         the path to the schema file (or the schema content itself), and with the
         connection string to the backend.
         """
         server = OlapServer(backend=connection, schema=schema, cache=cache)
         return cls(server)
 
-    def get_debug_meta(self):
-        """Generates some extra info if the app is running in debug mode."""
-        if not self.debug:
-            return False
-
-        return {
-            "git_branch": os.getenv("GIT_BRANCH", ""),
-            "git_hash": os.getenv("GIT_HASH", ""),
-        }
-
     @ll.healthcheck
     def healthcheck(self):
         return self.server.ping()
 
     @ll.route("GET", "/")
-    def module_status(self) -> StatusResModel:
+    def module_status(self) -> ll.ModuleStatus:
         """Retrieves operational information about this instance of TesseractModule."""
-        return StatusResModel(
-            debug=self.get_debug_meta(),
-            software="tesseract-olap[python]",
+        return ll.ModuleStatus(
+            module=olap.__title__,
+            version=olap.__version__,
+            debug=DEBUG_INFO if self.debug else False,
             status="ok" if self.server.ping() else "error",
-            version=tesseract_version,
         )
 
     @ll.route("GET", "/cubes", name="public_schema")
     def public_schema(
         self,
         locale: Optional[str] = None,
         token: Optional[ll.AuthToken] = Depends(auth_token),
```

### Comparing `tesseract_olap-0.9.4/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.9.5/tesseract_olap/logiclayer/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 import tempfile as tmp
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict, List, Mapping, Optional, Union
+from typing import List, Mapping, Optional
 
 import orjson
 import polars as pl
 from fastapi import HTTPException
 from fastapi.responses import FileResponse, Response
 from starlette.background import BackgroundTask
-from typing_extensions import Literal
 
 from tesseract_olap.backend import Result
 from tesseract_olap.common import AnyDict
 from tesseract_olap.query import DataQuery, DataRequest, MembersQuery, MembersRequest
 from tesseract_olap.schema import Annotations, MemberType, TesseractProperty
 
 
@@ -33,22 +32,14 @@
     ResponseFormat.jsonrecords: "application/json",
     ResponseFormat.parquet: "application/vnd.apache.parquet",
     ResponseFormat.tsv: "text/tab-separated-values",
 }
 
 
 @dataclass(eq=False, order=False)
-class StatusResModel:
-    software: Literal["tesseract-olap[python]"]
-    status: Literal["ok", "error"]
-    version: str
-    debug: Union[Dict[str, str], Literal[False]] = False
-
-
-@dataclass(eq=False, order=False)
 class MembersResModel:
     name: str
     caption: str
     depth: int
     annotations: Annotations
     properties: List["TesseractProperty"]
     dtypes: Mapping[str, MemberType]
```

### Comparing `tesseract_olap-0.9.4/tesseract_olap/query/__init__.py` & `tesseract_olap-0.9.5/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/query/enums.py` & `tesseract_olap-0.9.5/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/query/models.py` & `tesseract_olap-0.9.5/tesseract_olap/query/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/query/queries.py` & `tesseract_olap-0.9.5/tesseract_olap/query/queries.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/query/requests.py` & `tesseract_olap-0.9.5/tesseract_olap/query/requests.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/aggregators.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/csv.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/csv.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/enums.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/json.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/json.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/models.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 
 
 class Entity:
     name: str
     annotations: Annotations
     captions: CaptionSet
     acl: AccessControl
+    visible: bool
 
     def get_annotation(self, name: str) -> Optional[str]:
         """Retrieves an annotation for the entity.
         If the annotation is not defined, raises a :class:`KeyError`.
         """
         return self.annotations[name]
 
@@ -151,40 +152,43 @@
     name: str
     default_hierarchy: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     dim_type: DimensionType = DimensionType.STANDARD
     foreign_key: Optional[str] = None
     hierarchy_map: Mapping[str, "Hierarchy"] = field(default_factory=immu.Map)
+    visible: bool = True
 
     def get_default_hierarchy(self):
         return self.hierarchy_map[self.default_hierarchy]
 
 
 @dataclass(eq=True, frozen=True)
 class Hierarchy(Entity):
     name: str
     primary_key: str
     table: Union["InlineTable", "Table", str, None]
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     default_member: Optional[Tuple[str, str]] = None
     level_map: Mapping[str, "Level"] = field(default_factory=immu.Map)
+    visible: bool = True
 
 
 @dataclass(eq=True, frozen=True)
 class Level(Entity):
     name: str
     depth: int
     key_column: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     name_column_map: Mapping[str, str] = field(default_factory=immu.Map)
     key_type: MemberType = MemberType.STRING
     property_map: Mapping[str, "Property"] = field(default_factory=immu.Map)
+    visible: bool = True
 
     def get_name_column(self, locale: str = "xx") -> Optional[str]:
         return get_localization(self.name_column_map, locale)
 
     def get_locale_available(self) -> Set[str]:
         return set(self.captions.keys()).union(self.name_column_map.keys())
 
@@ -192,14 +196,15 @@
 @dataclass(eq=True, frozen=True)
 class Property(Entity):
     name: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     key_column_map: Mapping[str, str] = field(default_factory=immu.Map)
     key_type: MemberType = MemberType.STRING
+    visible: bool = True
 
     def get_key_column(self, locale: str = "xx") -> str:
         return get_localization(self.key_column_map, locale, force=True)
 
     def get_locale_available(self) -> Set[str]:
         return set(self.captions.keys()).union(self.key_column_map.keys())
 
@@ -208,28 +213,30 @@
 class Measure(Entity):
     name: str
     key_column: str
     aggregator: Aggregator = field(default_factory=Count)
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     submeasures: Mapping[str, "AnyMeasure"] = field(default_factory=immu.Map)
+    visible: bool = True
 
     def and_submeasures(self):
         yield self
         yield from self.submeasures.values()
 
 
 @dataclass(eq=True, frozen=True)
 class CalculatedMeasure(Entity):
     name: str
     formula: AST
     aggregator: Aggregator = field(default_factory=Count)
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     submeasures: Mapping[str, "AnyMeasure"] = field(default_factory=immu.Map)
+    visible: bool = True
 
     def and_submeasures(self):
         yield self
         yield from self.submeasures.values()
 
     @staticmethod
     def _parse_formula(formula: str) -> AST:
@@ -252,45 +259,49 @@
 
     name: str
     source: str
     foreign_key: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     hierarchy_map: Mapping[str, "HierarchyUsage"] = field(default_factory=immu.Map)
+    visible: bool = True
 
 
 @dataclass(eq=True, frozen=True)
 class HierarchyUsage(Usage):
     """Establishes the usage of a :class:`Hierarchy` defined in a
     :class:`SharedDimension`.
     """
 
     name: str
     source: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     level_map: Mapping[str, "LevelUsage"] = field(default_factory=immu.Map)
+    visible: bool = True
 
 
 @dataclass(eq=True, frozen=True)
 class LevelUsage(Usage):
     """Establishes the usage of a :class:`Level` defined in a :class:`Hierarchy`
     under a :class:`SharedDimension`.
     """
 
     name: str
     source: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     property_map: Mapping[str, "PropertyUsage"] = field(default_factory=immu.Map)
+    visible: bool = True
 
 
 @dataclass(eq=True, frozen=True)
 class PropertyUsage(Usage):
     """Establishes the usage of a :class:`Property` defined in a :class:`Level`
     under a :class:`SharedDimension`.
     """
 
     name: str
     source: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
+    visible: bool = True
```

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/parser.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/parser.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/public.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/public.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,17 +52,20 @@
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             dimensions=[
                 TesseractDimension.from_entity(item, locale)
                 for item in entity.dimensions
+                if item.visible
             ],
             measures=[
-                TesseractMeasure.from_entity(item, locale) for item in entity.measures
+                TesseractMeasure.from_entity(item, locale)
+                for item in entity.measures
+                if item.visible
             ],
             annotations=dict(entity.annotations),
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
 class TesseractMeasure:
@@ -77,15 +80,17 @@
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             aggregator=str(entity.aggregator),
             annotations=dict(entity.annotations),
             attached=[
-                cls.from_entity(item, locale) for item in entity.submeasures.values()
+                cls.from_entity(item, locale)
+                for item in entity.submeasures.values()
+                if item.visible
             ],
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
 class TesseractDimension:
     name: str
@@ -102,14 +107,15 @@
             name=entity.name,
             caption=entity.get_caption(locale),
             type=entity.dim_type,
             annotations=dict(entity.annotations),
             hierarchies=[
                 TesseractHierarchy.from_entity(item, locale)
                 for item in entity.hierarchies
+                if item.visible
             ],
             default_hierarchy=entity._entity.default_hierarchy,
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
 class TesseractHierarchy:
@@ -121,15 +127,19 @@
     @classmethod
     def from_entity(cls, entity: traverse.HierarchyTraverser, locale: str):
         """Generates a dataclass-schema object describing this entity."""
         return cls(
             name=entity.name,
             caption=entity.get_caption(locale),
             annotations=dict(entity.annotations),
-            levels=[TesseractLevel.from_entity(item, locale) for item in entity.levels],
+            levels=[
+                TesseractLevel.from_entity(item, locale)
+                for item in entity.levels
+                if item.visible
+            ],
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
 class TesseractLevel:
     name: str
     caption: str
@@ -144,14 +154,15 @@
             name=entity.name,
             caption=entity.get_caption(locale),
             depth=entity.depth,
             annotations=dict(entity.annotations),
             properties=[
                 TesseractProperty.from_entity(item, locale)
                 for item in entity.properties
+                if item.visible
             ],
         )
 
 
 @dataclass(eq=False, frozen=True, order=False)
 class TesseractProperty:
     name: str
```

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.9.5/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/traverse.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/schema/xml.py` & `tesseract_olap-0.9.5/tesseract_olap/schema/xml.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/server/schema.py` & `tesseract_olap-0.9.5/tesseract_olap/server/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/tesseract_olap/server/server.py` & `tesseract_olap-0.9.5/tesseract_olap/server/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.4/PKG-INFO` & `tesseract_olap-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.9.4
+Version: 0.9.5
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
```

