# Comparing `tmp/evnex-0.4.0.tar.gz` & `tmp/evnex-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evnex-0.4.0.tar", max compression
+gzip compressed data, was "evnex-0.4.0a1.tar", max compression
```

## Comparing `evnex-0.4.0.tar` & `evnex-0.4.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-05-04 08:17:56.298814 evnex-0.4.0/LICENSE
--rw-r--r--   0        0        0     1821 2024-05-04 08:17:56.298814 evnex-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/__init__.py
--rw-r--r--   0        0        0    19118 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/api.py
--rw-r--r--   0        0        0       51 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/errors.py
--rw-r--r--   0        0        0        0 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/__init__.py
--rw-r--r--   0        0        0     3740 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/charge_points.py
--rw-r--r--   0        0        0      117 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/commands.py
--rw-r--r--   0        0        0       95 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/cost.py
--rw-r--r--   0        0        0      657 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/org.py
--rw-r--r--   0        0        0      439 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/user.py
--rw-r--r--   0        0        0        0 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/v3/__init__.py
--rw-r--r--   0        0        0     3010 2024-05-04 08:17:56.298814 evnex-0.4.0/evnex/schema/v3/charge_points.py
--rw-r--r--   0        0        0      162 2024-05-04 08:17:56.302814 evnex-0.4.0/evnex/schema/v3/commands.py
--rw-r--r--   0        0        0      429 2024-05-04 08:17:56.302814 evnex-0.4.0/evnex/schema/v3/cost.py
--rw-r--r--   0        0        0      558 2024-05-04 08:17:56.302814 evnex-0.4.0/evnex/schema/v3/generic.py
--rw-r--r--   0        0        0      428 2024-05-04 08:17:56.302814 evnex-0.4.0/evnex/schema/v3/relationships.py
--rw-r--r--   0        0        0      757 2024-05-04 08:17:56.302814 evnex-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 evnex-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-19 22:02:03.569759 evnex-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     1821 2024-01-05 19:24:23.290829 evnex-0.4.0a1/README.md
+-rw-r--r--   0        0        0        0 2024-01-05 06:42:05.589303 evnex-0.4.0a1/evnex/__init__.py
+-rw-r--r--   0        0        0    19096 2024-05-04 07:56:27.067617 evnex-0.4.0a1/evnex/api.py
+-rw-r--r--   0        0        0       51 2022-09-22 21:10:57.492809 evnex-0.4.0a1/evnex/errors.py
+-rw-r--r--   0        0        0        0 2022-09-19 22:02:03.569759 evnex-0.4.0a1/evnex/schema/__init__.py
+-rw-r--r--   0        0        0     3740 2024-05-04 07:54:35.471045 evnex-0.4.0a1/evnex/schema/charge_points.py
+-rw-r--r--   0        0        0      117 2024-05-04 07:46:05.216258 evnex-0.4.0a1/evnex/schema/commands.py
+-rw-r--r--   0        0        0       95 2024-05-04 07:46:05.204258 evnex-0.4.0a1/evnex/schema/cost.py
+-rw-r--r--   0        0        0      657 2024-05-04 07:46:05.208258 evnex-0.4.0a1/evnex/schema/org.py
+-rw-r--r--   0        0        0      439 2024-05-04 07:46:05.228258 evnex-0.4.0a1/evnex/schema/user.py
+-rw-r--r--   0        0        0        0 2022-10-03 22:48:26.060279 evnex-0.4.0a1/evnex/schema/v3/__init__.py
+-rw-r--r--   0        0        0     3010 2024-05-04 07:54:35.459045 evnex-0.4.0a1/evnex/schema/v3/charge_points.py
+-rw-r--r--   0        0        0      162 2024-05-04 07:46:05.224259 evnex-0.4.0a1/evnex/schema/v3/commands.py
+-rw-r--r--   0        0        0      429 2024-05-04 07:46:05.212258 evnex-0.4.0a1/evnex/schema/v3/cost.py
+-rw-r--r--   0        0        0      558 2024-05-04 07:28:47.299582 evnex-0.4.0a1/evnex/schema/v3/generic.py
+-rw-r--r--   0        0        0      428 2024-05-04 07:46:05.220259 evnex-0.4.0a1/evnex/schema/v3/relationships.py
+-rw-r--r--   0        0        0      759 2024-05-04 08:02:27.001413 evnex-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 evnex-0.4.0a1/PKG-INFO
```

### Comparing `evnex-0.4.0/LICENSE` & `evnex-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `evnex-0.4.0/README.md` & `evnex-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `evnex-0.4.0/evnex/api.py` & `evnex-0.4.0a1/evnex/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,17 +311,15 @@
         # Similar to f'https://client-api.evnex.io/v3/charge-points/{charge_point_id}/sessions',
 
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v2/apps/charge-points/{charge_point_id}/transactions",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
-        return EvnexGetChargePointTransactionsResponse.model_validate(
-            json_data
-        ).data.items
+        return EvnexGetChargePointTransactionsResponse.model_validate(json_data).data.items
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_charge_point_sessions(
         self, charge_point_id: str
```

### Comparing `evnex-0.4.0/evnex/schema/charge_points.py` & `evnex-0.4.0a1/evnex/schema/charge_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     solarWithSchedule: bool
     powerSensorInstalled: bool
     solarStartExportPower: float
     solarStopImportPower: float
 
 
 class EvnexChargePointOverrideConfig(BaseModel):
-    chargeNow: bool | Literal["NotSupported"]
+    chargeNow: bool | Literal['NotSupported']
 
 
 class EvnexChargePointBase(BaseModel):
     # Attributes shared by brief and detail endpoints
     id: str
     createdDate: datetime
     updatedDate: datetime
```

### Comparing `evnex-0.4.0/evnex/schema/org.py` & `evnex-0.4.0a1/evnex/schema/org.py`

 * *Files identical despite different names*

### Comparing `evnex-0.4.0/evnex/schema/v3/charge_points.py` & `evnex-0.4.0a1/evnex/schema/v3/charge_points.py`

 * *Files identical despite different names*

### Comparing `evnex-0.4.0/evnex/schema/v3/generic.py` & `evnex-0.4.0a1/evnex/schema/v3/generic.py`

 * *Files identical despite different names*

### Comparing `evnex-0.4.0/pyproject.toml` & `evnex-0.4.0a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evnex"
-version = "0.4.0"
+version = "0.4.0a1"
 description = "A Python wrapper for the EVNEX Cloud API"
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 repository = "https://github.com/hardbyte/python-evnex"
 license = "Apache-2.0"
 
 [tool.poetry.urls]
```

### Comparing `evnex-0.4.0/PKG-INFO` & `evnex-0.4.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evnex
-Version: 0.4.0
+Version: 0.4.0a1
 Summary: A Python wrapper for the EVNEX Cloud API
 Home-page: https://github.com/hardbyte/python-evnex
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

