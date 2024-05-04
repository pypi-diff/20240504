# Comparing `tmp/nonebot_plugin_access_control_api-1.1.2.tar.gz` & `tmp/nonebot_plugin_access_control_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control_api-1.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control_api-1.2.0.tar", max compression
```

## Comparing `nonebot_plugin_access_control_api-1.1.2.tar` & `nonebot_plugin_access_control_api-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1064 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/LICENSE
--rw-r--r--   0        0        0    10248 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/README.MD
--rw-r--r--   0        0        0     1663 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      673 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/__init__.py
--rw-r--r--   0        0        0     4459 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/context.py
--rw-r--r--   0        0        0      577 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/errors.py
--rw-r--r--   0        0        0     2160 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/event_bus.py
--rw-r--r--   0        0        0        0 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/models/__init__.py
--rw-r--r--   0        0        0      198 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/models/permission.py
--rw-r--r--   0        0        0      785 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/models/rate_limit.py
--rw-r--r--   0        0        0      525 2023-11-26 12:40:07.403926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/__init__.py
--rw-r--r--   0        0        0       30 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/__init__.py
--rw-r--r--   0        0        0     1445 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/factory.py
--rw-r--r--   0        0        0      647 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/patcher.py
--rw-r--r--   0        0        0     2135 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/permission.py
--rw-r--r--   0        0        0     2431 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/rate_limit.py
--rw-r--r--   0        0        0      327 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/contextvars.py
--rw-r--r--   0        0        0      320 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/__init__.py
--rw-r--r--   0        0        0      716 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/factory.py
--rw-r--r--   0        0        0      839 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/nonebot_service.py
--rw-r--r--   0        0        0      355 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/patcher.py
--rw-r--r--   0        0        0     1631 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/permission.py
--rw-r--r--   0        0        0      704 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/plugin_service.py
--rw-r--r--   0        0        0     2564 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/rate_limit.py
--rw-r--r--   0        0        0      687 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/service.py
--rw-r--r--   0        0        0     2303 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/service_base.py
--rw-r--r--   0        0        0      571 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/subservice.py
--rw-r--r--   0        0        0      324 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      978 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/methods.py
--rw-r--r--   0        0        0     2943 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/nonebot_service.py
--rw-r--r--   0        0        0     1070 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/plugin_service.py
--rw-r--r--   0        0        0     7015 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/service.py
--rw-r--r--   0        0        0      991 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/subservice.py
--rw-r--r--   0        0        0     1740 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/subservice_owner.py
--rw-r--r--   0        0        0      177 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/__init__.py
--rw-r--r--   0        0        0      753 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/extractor/__init__.py
--rw-r--r--   0        0        0      181 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/extractor/base.py
--rw-r--r--   0        0        0     1345 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/extractor/chain.py
--rw-r--r--   0        0        0     1538 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/manager.py
--rw-r--r--   0        0        0      287 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/model.py
--rw-r--r--   0        0        0        0 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/utils/__init__.py
--rw-r--r--   0        0        0      224 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/utils/call_with_params.py
--rw-r--r--   0        0        0      279 2023-11-26 12:40:07.407926 nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/utils/superuser.py
--rw-r--r--   0        0        0    11071 1970-01-01 00:00:00.000000 nonebot_plugin_access_control_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/LICENSE
+-rw-r--r--   0        0        0    10248 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/README.MD
+-rw-r--r--   0        0        0     1617 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      577 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/__init__.py
+-rw-r--r--   0        0        0     4451 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/context.py
+-rw-r--r--   0        0        0      455 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/errors.py
+-rw-r--r--   0        0        0     2160 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/event_bus.py
+-rw-r--r--   0        0        0        0 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/models/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/models/permission.py
+-rw-r--r--   0        0        0      777 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/models/rate_limit.py
+-rw-r--r--   0        0        0      525 2024-05-04 08:36:07.224605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/factory.py
+-rw-r--r--   0        0        0      647 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/patcher.py
+-rw-r--r--   0        0        0     2135 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/permission.py
+-rw-r--r--   0        0        0     2431 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/rate_limit.py
+-rw-r--r--   0        0        0      327 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/contextvars.py
+-rw-r--r--   0        0        0      320 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/factory.py
+-rw-r--r--   0        0        0      807 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/nonebot_service.py
+-rw-r--r--   0        0        0      355 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/patcher.py
+-rw-r--r--   0        0        0     1631 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/permission.py
+-rw-r--r--   0        0        0      696 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/plugin_service.py
+-rw-r--r--   0        0        0     2500 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      683 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/service.py
+-rw-r--r--   0        0        0     2303 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/service_base.py
+-rw-r--r--   0        0        0      567 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/subservice.py
+-rw-r--r--   0        0        0      324 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      978 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/methods.py
+-rw-r--r--   0        0        0     2943 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/nonebot_service.py
+-rw-r--r--   0        0        0     1070 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/plugin_service.py
+-rw-r--r--   0        0        0     7015 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/service.py
+-rw-r--r--   0        0        0      991 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/subservice.py
+-rw-r--r--   0        0        0     1740 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/subservice_owner.py
+-rw-r--r--   0        0        0      177 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/extractor/base.py
+-rw-r--r--   0        0        0     1345 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/extractor/chain.py
+-rw-r--r--   0        0        0     1538 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/manager.py
+-rw-r--r--   0        0        0      287 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/model.py
+-rw-r--r--   0        0        0        0 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/utils/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/utils/call_with_params.py
+-rw-r--r--   0        0        0      279 2024-05-04 08:36:07.228605 nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/utils/superuser.py
+-rw-r--r--   0        0        0    11023 1970-01-01 00:00:00.000000 nonebot_plugin_access_control_api-1.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/LICENSE` & `nonebot_plugin_access_control_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/README.MD` & `nonebot_plugin_access_control_api-1.2.0/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/pyproject.toml` & `nonebot_plugin_access_control_api-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control-api"
-version = "1.1.2"
+version = "1.2.0"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/bot-ssttkkl/nonebot-plugin-access-control"
 packages = [
     { include = "nonebot_plugin_access_control_api", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.1.0"
-ssttkkl-nonebot-utils = ">=0.1.17"
+nonebot2 = ">=2.2.0, <3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.275"
 isort = "^5.10.1"
 black = "^23.1.0"
 pre-commit = "^3.1.0"
 
 setuptools = "^68.1.2"
-nb-cli = "^1.2.5"
-nonebot-plugin-apscheduler = "^0.3.0"
+nb-cli = "*"
+nonebot-plugin-apscheduler = "*"
 
-nonebot2 = {extras = ["fastapi"], version = "^2.1.2"}
+nonebot2 = {extras = ["fastapi"], version = "*"}
 nonebot-adapter-onebot = "*"
 nonebot-adapter-kaiheila = "*"
-nonebot-adapter-qqguild = "*"
+nonebot-adapter-qq = "*"
 nonebot-adapter-telegram = "*"
 nonebot-adapter-console = "*"
 nonebot-adapter-feishu = "*"
 
 nonebug = "^0.3.5"
 pytest = "^7.4.3"
 pytest-asyncio = "^0.21.1"
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/__init__.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 nonebot-plugin-access-control-api
 
 @Author         : ssttkkl
 @License        : MIT
 @GitHub         : https://github.com/bot-ssttkkl/nonebot-access-control-api
 """
-from nonebot import require
-
-require("nonebot_plugin_session")
-require("ssttkkl_nonebot_utils")
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="权限控制API",
     description="为插件开发者提供适配nonebot-plugin-access-control的API",
     usage="参考 https://github.com/bot-ssttkkl/nonebot-plugin-access-control-api",
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/context.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 T = TypeVar("T")
 T2 = TypeVar("T2")
 
 
 class Provider(ABC, Generic[T]):
     @abstractmethod
-    def provide(self) -> T:
-        ...
+    def provide(self) -> T: ...
 
 
 class InstanceProvider(Provider[T], Generic[T]):
     def __init__(self, instance: T):
         self._instance = instance
 
     def provide(self) -> T:
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/event_bus.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/models/rate_limit.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/models/rate_limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     rule_id: str
     user: str
     acquire_time: datetime
     expire_time: datetime
 
 
 class IRateLimitToken(ABC):
-    async def retire(self):
-        ...
+    async def retire(self): ...
 
 
 class AcquireTokenResult(NamedTuple):
     success: bool
     token: Optional[IRateLimitToken] = None
     violating: Optional[Sequence[RateLimitRule]] = None
     available_time: Optional[datetime] = None
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/__init__.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/factory.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/factory.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/patcher.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/patcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/permission.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/_dummy/rate_limit.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/_dummy/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/factory.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,18 @@
 from . import IService
 from .patcher import IServicePatcher
 from .rate_limit import IServiceRateLimit
 from .permission import IServicePermission
 
 
 class IServiceComponentFactory(Protocol):
-    def create_patcher_impl(self, service: IService) -> IServicePatcher:
-        ...
+    def create_patcher_impl(self, service: IService) -> IServicePatcher: ...
 
-    def typeof_patcher_impl(self) -> type[IServicePatcher]:
-        ...
+    def typeof_patcher_impl(self) -> type[IServicePatcher]: ...
 
-    def create_permission_impl(self, service: IService) -> IServicePermission:
-        ...
+    def create_permission_impl(self, service: IService) -> IServicePermission: ...
 
-    def typeof_permission_impl(self) -> type[IServicePermission]:
-        ...
+    def typeof_permission_impl(self) -> type[IServicePermission]: ...
 
-    def create_rate_limit_impl(self, service: IService) -> IServiceRateLimit:
-        ...
+    def create_rate_limit_impl(self, service: IService) -> IServiceRateLimit: ...
 
-    def typeof_rate_limit_impl(self) -> type[IServiceRateLimit]:
-        ...
+    def typeof_rate_limit_impl(self) -> type[IServiceRateLimit]: ...
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/nonebot_service.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/nonebot_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,18 @@
 T_ChildService = TypeVar("T_ChildService", bound=IPluginService, covariant=True)
 
 
 class INoneBotService(
     IService[T_Service, None, T_ChildService],
     ABC,
 ):
-    def create_plugin_service(self, plugin_name: str) -> T_ChildService:
-        ...
+    def create_plugin_service(self, plugin_name: str) -> T_ChildService: ...
 
     def get_plugin_service(
         self, plugin_name: str, *, raise_on_not_exists: bool = False
-    ) -> Optional[T_ChildService]:
-        ...
+    ) -> Optional[T_ChildService]: ...
 
-    def get_or_create_plugin_service(self, plugin_name: str) -> T_ChildService:
-        ...
+    def get_or_create_plugin_service(self, plugin_name: str) -> T_ChildService: ...
 
     def get_service_by_qualified_name(
         self, qualified_name: str, *, raise_on_not_exists: bool = False
-    ) -> Optional[T_Service]:
-        ...
+    ) -> Optional[T_Service]: ...
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/permission.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/plugin_service.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/plugin_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 class IPluginService(
     IService[T_Service, T_ParentService, T_ChildService],
     ISubServiceOwner[T_ChildService],
     ABC,
 ):
     @property
     @abstractmethod
-    def auto_created(self) -> bool:
-        ...
+    def auto_created(self) -> bool: ...
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/rate_limit.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/rate_limit.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,44 +19,38 @@
     @abstractmethod
     def on_remove_rate_limit_rule(self, func: Optional[T_Listener] = None):
         raise NotImplementedError()
 
     @abstractmethod
     def get_rate_limit_rules_by_subject(
         self, *subject: str, trace: bool = True
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        ...
+    ) -> AsyncGenerator[RateLimitRule, None]: ...
 
     @abstractmethod
     def get_rate_limit_rules(
         self, *, trace: bool = True
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        ...
+    ) -> AsyncGenerator[RateLimitRule, None]: ...
 
     @classmethod
     @abstractmethod
     def get_all_rate_limit_rules_by_subject(
         cls, *subject: str
-    ) -> AsyncGenerator[RateLimitRule, None]:
-        ...
+    ) -> AsyncGenerator[RateLimitRule, None]: ...
 
     @classmethod
     @abstractmethod
-    def get_all_rate_limit_rules(cls) -> AsyncGenerator[RateLimitRule, None]:
-        ...
+    def get_all_rate_limit_rules(cls) -> AsyncGenerator[RateLimitRule, None]: ...
 
     @abstractmethod
     async def add_rate_limit_rule(
         self, subject: str, time_span: timedelta, limit: int, overwrite: bool = False
-    ) -> RateLimitRule:
-        ...
+    ) -> RateLimitRule: ...
 
     @classmethod
-    async def remove_rate_limit_rule(cls, rule_id: str) -> bool:
-        ...
+    async def remove_rate_limit_rule(cls, rule_id: str) -> bool: ...
 
     async def acquire_token_for_rate_limit(
         self, bot: Bot, event: Event
     ) -> Optional[IRateLimitToken]:
         result = await self.acquire_token_for_rate_limit_receiving_result(bot, event)
         return result.token
 
@@ -74,14 +68,12 @@
             *subject
         )
         return result.token
 
     @abstractmethod
     async def acquire_token_for_rate_limit_by_subjects_receiving_result(
         self, *subject: str
-    ) -> AcquireTokenResult:
-        ...
+    ) -> AcquireTokenResult: ...
 
     @classmethod
     @abstractmethod
-    async def clear_rate_limit_tokens(cls):
-        ...
+    async def clear_rate_limit_tokens(cls): ...
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/service.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 class IService(
     Generic[T_Service, T_ParentService, T_ChildService],
     IServiceBase[T_Service, T_ParentService, T_ChildService],
     IServicePatcher,
     IServicePermission,
     IServiceRateLimit,
     ABC,
-):
-    ...
+): ...
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/service_base.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/service_base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/interface/subservice.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/interface/subservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,8 @@
 
 
 class ISubService(
     Generic[T_Service, T_ParentService, T_ChildService],
     IService[T_Service, T_ParentService, T_ChildService],
     ISubServiceOwner[T_ChildService],
     ABC,
-):
-    ...
+): ...
```

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/methods.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/nonebot_service.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/nonebot_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/plugin_service.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/plugin_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/service.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/subservice.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/service/subservice_owner.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/extractor/__init__.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/extractor/chain.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/extractor/chain.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/src/nonebot_plugin_access_control_api/subject/manager.py` & `nonebot_plugin_access_control_api-1.2.0/src/nonebot_plugin_access_control_api/subject/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control_api-1.1.2/PKG-INFO` & `nonebot_plugin_access_control_api-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control-api
-Version: 1.1.2
+Version: 1.2.0
 Summary: 
 Home-page: https://github.com/bot-ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nonebot2 (>=2.1.0,<3.0.0)
-Requires-Dist: ssttkkl-nonebot-utils (>=0.1.17)
+Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Project-URL: Repository, https://github.com/bot-ssttkkl/nonebot-plugin-access-control
 Description-Content-Type: text/plain
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
```

