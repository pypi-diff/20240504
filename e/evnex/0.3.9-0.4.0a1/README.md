# Comparing `tmp/evnex-0.3.9.tar.gz` & `tmp/evnex-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evnex-0.3.9.tar", max compression
+gzip compressed data, was "evnex-0.4.0a1.tar", max compression
```

## Comparing `evnex-0.3.9.tar` & `evnex-0.4.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-01-06 08:47:07.326937 evnex-0.3.9/LICENSE
--rw-r--r--   0        0        0     1821 2024-01-06 08:47:07.326937 evnex-0.3.9/README.md
--rw-r--r--   0        0        0        0 2024-01-06 08:47:07.326937 evnex-0.3.9/evnex/__init__.py
--rw-r--r--   0        0        0    19038 2024-01-06 08:47:07.326937 evnex-0.3.9/evnex/api.py
--rw-r--r--   0        0        0       51 2024-01-06 08:47:07.326937 evnex-0.3.9/evnex/errors.py
--rw-r--r--   0        0        0        0 2024-01-06 08:47:07.326937 evnex-0.3.9/evnex/schema/__init__.py
--rw-r--r--   0        0        0     3761 2024-01-06 08:47:07.326937 evnex-0.3.9/evnex/schema/charge_points.py
--rw-r--r--   0        0        0      184 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/commands.py
--rw-r--r--   0        0        0      162 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/cost.py
--rw-r--r--   0        0        0      717 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/org.py
--rw-r--r--   0        0        0      506 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/user.py
--rw-r--r--   0        0        0        0 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/v3/__init__.py
--rw-r--r--   0        0        0     3084 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/v3/charge_points.py
--rw-r--r--   0        0        0      223 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/v3/commands.py
--rw-r--r--   0        0        0      482 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/v3/cost.py
--rw-r--r--   0        0        0      709 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/v3/generic.py
--rw-r--r--   0        0        0      467 2024-01-06 08:47:07.330937 evnex-0.3.9/evnex/schema/v3/relationships.py
--rw-r--r--   0        0        0      700 2024-01-06 08:47:07.330937 evnex-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 evnex-0.3.9/PKG-INFO
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

### Comparing `evnex-0.3.9/LICENSE` & `evnex-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `evnex-0.3.9/README.md` & `evnex-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `evnex-0.3.9/evnex/api.py` & `evnex-0.4.0a1/evnex/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import logging
 from importlib.metadata import PackageNotFoundError, version
 from typing import Optional
 from warnings import warn
 
 import botocore
-
+import pydantic
+from pydantic_core import from_json
 from httpx import AsyncClient, ReadTimeout
 from pycognito import Cognito
-
-try:
-    from pydantic import v1 as pydantic
-    from pydantic.v1 import BaseSettings, HttpUrl, ValidationError
-except ImportError:
-    import pydantic
-    from pydantic import BaseSettings, HttpUrl, ValidationError
-
+from pydantic import HttpUrl, ValidationError
 from tenacity import retry, retry_if_not_exception_type, wait_random_exponential
 
 from evnex.errors import NotAuthorizedException
 from evnex.schema.charge_points import (
     EvnexChargePoint,
     EvnexChargePointDetail,
     EvnexChargePointLoadSchedule,
@@ -36,14 +30,15 @@
 from evnex.schema.v3.charge_points import (
     EvnexChargePointDetail as EvnexChargePointDetailV3,
     EvnexGetChargePointSessionsResponse,
     EvnexChargePointSession,
 )
 from evnex.schema.v3.commands import EvnexCommandResponse as EvnexCommandResponseV3
 from evnex.schema.v3.generic import EvnexV3APIResponse
+from pydantic_settings import BaseSettings
 
 logger = logging.getLogger("evnex.api")
 
 
 class EvnexConfig(BaseSettings):
     EVNEX_BASE_URL: HttpUrl = "https://client-api.evnex.io"
     EVNEX_COGNITO_USER_POOL_ID: str = "ap-southeast-2_zWnqo6ASv"
@@ -137,15 +132,15 @@
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_user_detail(self) -> EvnexUserDetail:
         response = await self.httpx_client.get(
             "https://client-api.evnex.io/v2/apps/user", headers=self._common_headers
         )
         response_json = await self._check_api_response(response)
-        data = EvnexGetUserResponse(**response_json).data
+        data = EvnexGetUserResponse.model_validate(response_json).data
 
         # Make the assumption that most end users are only in one org
         if len(data.organisations):
             self.org_id = data.organisations[0].id
 
         return data
 
@@ -160,15 +155,15 @@
         logger.debug(
             f"Raw EVNEX API response.\n{response.status_code}\n{response.text}"
         )
 
         response.raise_for_status()
 
         try:
-            return response.json()
+            return from_json(response.text)
         except:
             logger.debug(
                 f"Invalid json response.\n{response.status_code}\n{response.text}"
             )
             raise
 
     @retry(
@@ -182,15 +177,15 @@
             org_id = self.org_id
         logger.debug("Listing org charge points")
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v2/apps/organisations/{org_id}/charge-points",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
-        return EvnexGetChargePointsResponse(**json_data).data.items
+        return EvnexGetChargePointsResponse.model_validate(json_data).data.items
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_org_insight(
         self, days: int, org_id: Optional[str] = None
@@ -200,15 +195,15 @@
         logger.debug("Getting org insight")
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v2/apps/organisations/{org_id}/summary/insights",
             headers=self._common_headers,
             params={"days": days},
         )
         json_data = await self._check_api_response(r)
-        return EvnexGetOrgInsightResponse.parse_obj(json_data).data.items
+        return EvnexGetOrgInsightResponse.model_validate(json_data).data.items
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_charge_point_detail(
         self, charge_point_id: str
@@ -219,15 +214,15 @@
             stacklevel=2,
         )
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v2/apps/charge-points/{charge_point_id}",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
-        return EvnexGetChargePointDetailResponse(**json_data).data
+        return EvnexGetChargePointDetailResponse.model_validate(json_data).data
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type(
             (TypeError, ValidationError, NotAuthorizedException)
         ),
     )
@@ -238,15 +233,16 @@
             f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}",
             headers=self._common_headers,
         )
         logger.debug(
             f"Raw get charge point detail response.\n{r.status_code}\n{r.text}"
         )
         json_data = await self._check_api_response(r)
-        return EvnexV3APIResponse[EvnexChargePointDetailV3](**json_data)
+
+        return EvnexV3APIResponse[EvnexChargePointDetailV3].model_validate(json_data)
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_charge_point_solar_config(
         self, charge_point_id: str
@@ -257,15 +253,15 @@
         """
         r = await self.httpx_client.post(
             f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}/commands/get-solar",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
 
-        return EvnexChargePointSolarConfig(**json_data)
+        return EvnexChargePointSolarConfig.model_validate(json_data)
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type(
             (ValidationError, NotAuthorizedException, ReadTimeout)
         ),
     )
@@ -279,15 +275,15 @@
         """
         r = await self.httpx_client.post(
             f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}/commands/get-override",
             headers=self._common_headers,
             timeout=15,
         )
         json_data = await self._check_api_response(r)
-        return EvnexChargePointOverrideConfig(**json_data)
+        return EvnexChargePointOverrideConfig.model_validate(json_data)
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def set_charge_point_override(
         self, charge_point_id: str, charge_now: bool, connector_id: int = 1
@@ -315,29 +311,29 @@
         # Similar to f'https://client-api.evnex.io/v3/charge-points/{charge_point_id}/sessions',
 
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v2/apps/charge-points/{charge_point_id}/transactions",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
-        return EvnexGetChargePointTransactionsResponse(**json_data).data.items
+        return EvnexGetChargePointTransactionsResponse.model_validate(json_data).data.items
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_charge_point_sessions(
         self, charge_point_id: str
     ) -> list[EvnexChargePointSession]:
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}/sessions",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
-        return EvnexGetChargePointSessionsResponse.parse_obj(json_data).data
+        return EvnexGetChargePointSessionsResponse.model_validate(json_data).data
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type(
             (ValidationError, NotAuthorizedException, ReadTimeout)
         ),
     )
@@ -366,15 +362,15 @@
             headers=self._common_headers,
             # 'Connection': 'Keep-Alive'
             json={"connectorId": connector_id},
             timeout=timeout,
         )
         json_data = await self._check_api_response(r)
 
-        return EvnexCommandResponse.parse_obj(json_data["data"])
+        return EvnexCommandResponse.model_validate(json_data["data"])
 
     async def enable_charger(self, charge_point_id: str, connector_id: int | str = 1):
         await self.set_charger_availability(
             charge_point_id=charge_point_id, available=True, connector_id=connector_id
         )
 
     async def disable_charger(self, charge_point_id: str, connector_id: int | str = 1):
@@ -404,15 +400,15 @@
             f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}/commands/change-availability",
             headers=self._common_headers,
             json={"connectorId": connector_id, "changeAvailabilityType": availability},
             timeout=timeout,
         )
         json_data = await self._check_api_response(r)
 
-        return EvnexCommandResponseV3.parse_obj(json_data["data"])
+        return EvnexCommandResponseV3.model_validate(json_data["data"])
 
     async def unlock_charger(
         self,
         charge_point_id: str,
         available: bool = True,
         connector_id: str = "0",
         timeout=10,
@@ -432,15 +428,15 @@
         r = await self.httpx_client.post(
             f"https://client-api.evnex.io/v2/apps/organisations/{self.org_id}/charge-points/{charge_point_id}/commands/unlock-connector",
             headers=self._common_headers,
             json={"connectorId": connector_id, "changeAvailabilityType": availability},
             timeout=timeout,
         )
         json_data = await self._check_api_response(r)
-        return EvnexCommandResponse.parse_obj(json_data["data"])
+        return EvnexCommandResponse.model_validate(json_data["data"])
 
     async def set_charger_load_profile(
         self,
         charge_point_id: str,
         charging_profile_periods: list[EvnexChargeProfileSegment | dict[str, int]],
         enabled: bool = True,
         duration: int = 86400,
@@ -469,15 +465,15 @@
                 "enabled": enabled,
                 "units": units,
                 "duration": duration,
             },
             timeout=timeout,
         )
         json_data = await self._check_api_response(r)
-        return EvnexChargePointLoadSchedule.parse_obj(json_data["data"])
+        return EvnexChargePointLoadSchedule.model_validate(json_data["data"])
 
     async def set_charge_point_schedule(
         self,
         charge_point_id: str,
         charging_profile_periods: list[EvnexChargeProfileSegment | dict[str, int]],
         enabled: bool = True,
         duration: int = 86400,
@@ -511,8 +507,8 @@
                 # "units": "A",
                 "duration": duration,
                 # "timezone": timezone,
             },
             timeout=timeout,
         )
         json_data = await self._check_api_response(r)
-        return EvnexChargePointLoadSchedule.parse_obj(json_data["data"])
+        return EvnexChargePointLoadSchedule.model_validate(json_data["data"])
```

### Comparing `evnex-0.3.9/evnex/schema/charge_points.py` & `evnex-0.4.0a1/evnex/schema/charge_points.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from datetime import datetime
+from typing import Literal
 
-try:
-    from pydantic.v1 import BaseModel, Field
-except ImportError:
-    from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field
 
 from evnex.schema.cost import EvnexCost
 
 
 class EvnexChargePointConnectorMeter(BaseModel):
     powerType: str  # "AC_1_PHASE"
     updatedDate: datetime
@@ -66,15 +64,15 @@
     solarWithSchedule: bool
     powerSensorInstalled: bool
     solarStartExportPower: float
     solarStopImportPower: float
 
 
 class EvnexChargePointOverrideConfig(BaseModel):
-    chargeNow: bool
+    chargeNow: bool | Literal['NotSupported']
 
 
 class EvnexChargePointBase(BaseModel):
     # Attributes shared by brief and detail endpoints
     id: str
     createdDate: datetime
     updatedDate: datetime
```

### Comparing `evnex-0.3.9/evnex/schema/org.py` & `evnex-0.4.0a1/evnex/schema/org.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from datetime import datetime
 from typing import Any
 
-try:
-    from pydantic.v1 import BaseModel
-except ImportError:
-    from pydantic import BaseModel
+from pydantic import BaseModel
 
 from evnex.schema.cost import EvnexCost
 
 
 class EvnexOrgBrief(BaseModel):
     id: str
     isDefault: bool
     role: int
     createdDate: datetime
     name: str
     slug: str
     tier: int
-    tierDetails: Any
+    tierDetails: Any = None
     updatedDate: datetime
 
 
 class EvnexOrgInsightEntry(BaseModel):
     carbonOffset: float
     costs: list[EvnexCost]
     duration: int
```

### Comparing `evnex-0.3.9/evnex/schema/v3/charge_points.py` & `evnex-0.4.0a1/evnex/schema/v3/charge_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from datetime import datetime
 from typing import Optional, Any
 
-try:
-    from pydantic.v1 import BaseModel, Field
-except ImportError:
-    from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field
 
 from evnex.schema.v3.cost import EvnexElectricityCost, EvnexElectricityCostTotal
 from evnex.schema.v3.relationships import EvnexRelationships
 
 
 class EvnexEnergyTransaction(BaseModel):
     meterStart: float
```

### Comparing `evnex-0.3.9/evnex/schema/v3/generic.py` & `evnex-0.4.0a1/evnex/schema/v3/generic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from typing import Generic, Optional, TypeVar
-
-try:
-    from pydantic.v1 import BaseModel
-
-    GenericModel = BaseModel
-except ImportError:
-    from pydantic import BaseModel
-    from pydantic.generics import GenericModel
-
+from pydantic import BaseModel
 from evnex.schema.v3.relationships import EvnexRelationships
 
+
 ResponseDataT = TypeVar("ResponseDataT")
 
 
 class EvnexV3Include(BaseModel):
     id: str
     type: str
     attributes: dict
 
 
-class EvnexV3Data(GenericModel, Generic[ResponseDataT]):
+class EvnexV3Data(BaseModel, Generic[ResponseDataT]):
     id: str
     type: str
     attributes: ResponseDataT
     relationships: EvnexRelationships
 
 
-class EvnexV3APIResponse(GenericModel, Generic[ResponseDataT]):
+class EvnexV3APIResponse(BaseModel, Generic[ResponseDataT]):
     data: EvnexV3Data[ResponseDataT]
     included: Optional[list[EvnexV3Include]]
```

### Comparing `evnex-0.3.9/pyproject.toml` & `evnex-0.4.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "evnex"
-version = "0.3.9"
+version = "0.4.0a1"
 description = "A Python wrapper for the EVNEX Cloud API"
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 repository = "https://github.com/hardbyte/python-evnex"
 license = "Apache-2.0"
 
 [tool.poetry.urls]
 issues = "https://github.com/hardbyte/python-evnex/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = ">=0.23"
-pycognito = "2023.5.0"
+pycognito = ">2023.5.0,<2025"
 boto3 = "^1.26"
-pydantic = ">1.10"
+pydantic = ">2.0.0,<3.0.0"
 tenacity = "^8.1"
+pydantic-settings = "^2.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.1.4"
+ruff = ">=0.1.4,<0.3.0"
 isort = "^5.10.1"
-pytest = "^7.1"
+pytest = ">7.1,<9.0"
 pre-commit = "^3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `evnex-0.3.9/PKG-INFO` & `evnex-0.4.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: evnex
-Version: 0.3.9
+Version: 0.4.0a1
 Summary: A Python wrapper for the EVNEX Cloud API
 Home-page: https://github.com/hardbyte/python-evnex
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: httpx (>=0.23)
-Requires-Dist: pycognito (==2023.5.0)
-Requires-Dist: pydantic (>1.10)
+Requires-Dist: pycognito (>2023.5.0,<2025)
+Requires-Dist: pydantic (>2.0.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: tenacity (>=8.1,<9.0)
 Project-URL: Repository, https://github.com/hardbyte/python-evnex
 Project-URL: issues, https://github.com/hardbyte/python-evnex/issues
 Description-Content-Type: text/markdown
 
 # python-evnex
```

