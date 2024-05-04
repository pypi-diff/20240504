# Comparing `tmp/great_expectations_cloud-20240502.0.dev0.tar.gz` & `tmp/great_expectations_cloud-20240503.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240502.0.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240503.0.dev1.tar", max compression
```

## Comparing `great_expectations_cloud-20240502.0.dev0.tar` & `great_expectations_cloud-20240503.0.dev1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-05-02 18:02:54.374021 great_expectations_cloud-20240502.0.dev0/LICENSE
--rw-r--r--   0        0        0     9760 2024-05-02 18:02:54.374021 great_expectations_cloud-20240502.0.dev0/README.md
--rw-r--r--   0        0        0      150 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    17221 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4663 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5918 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9533 2024-05-02 18:02:54.406021 great_expectations_cloud-20240502.0.dev0/pyproject.toml
--rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 great_expectations_cloud-20240502.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-05-04 00:05:39.159692 great_expectations_cloud-20240503.0.dev1/LICENSE
+-rw-r--r--   0        0        0     9760 2024-05-04 00:05:39.159692 great_expectations_cloud-20240503.0.dev1/README.md
+-rw-r--r--   0        0        0      150 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    17221 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4632 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5918 2024-05-04 00:05:39.187692 great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9540 2024-05-04 00:05:39.191692 great_expectations_cloud-20240503.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 great_expectations_cloud-20240503.0.dev1/PKG-INFO
```

### Comparing `great_expectations_cloud-20240502.0.dev0/LICENSE` & `great_expectations_cloud-20240503.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/README.md` & `great_expectations_cloud-20240503.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from collections import defaultdict
 from json import JSONDecodeError
 from typing import TYPE_CHECKING, Any, Final
 
 import great_expectations as gx
 from great_expectations.compatibility import pydantic
-from packaging.version import LegacyVersion, Version
+from packaging.version import Version
 from packaging.version import parse as parse_version
 
 from great_expectations_cloud.agent.actions.unknown import UnknownEventAction
 from great_expectations_cloud.agent.models import (
     Event,
     UnknownEvent,
 )
@@ -111,15 +111,15 @@
 class EventAlreadyRegisteredError(EventError):
     def __init__(self, event_type_name: str, version: str | Version):
         super().__init__(f"Event type {event_type_name} already registered for version {version}.")
 
 
 def _get_major_version(version: str) -> str:
     """Get major version as a string from version as a string. For example, "0.18.0" -> "0"."""
-    parsed: Version | LegacyVersion = parse_version(version)
+    parsed: Version = parse_version(version)
     if not isinstance(parsed, Version):
         raise InvalidVersionError(version)
     return str(parsed.major)
 
 
 version = gx.__version__  # type: ignore[attr-defined] # TODO: fix this
 _GX_MAJOR_VERSION = _get_major_version(str(version))
```

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240503.0.dev1/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240502.0.dev0/pyproject.toml` & `great_expectations_cloud-20240503.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240502.0.dev0"
+version = "20240503.0.dev1"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
@@ -21,15 +21,15 @@
 python = ">=3.8,<3.12"
 great-expectations = "^0.18.13"
 pydantic = "<3"
 pika = "^1.3.1"
 # needed for metrics serialization
 orjson = "^3.9.7, !=3.9.10" # TODO: remove inequality once dep resolution issue is resolved
 # relying on packaging in agent code so declaring it explicitly here
-packaging = "^21.3"
+packaging = ">=21.3,<25.0"
 tenacity = "^8.2.3"
 
 [tool.poetry.extras]
 snowflake = ["snowflake-sqlalchemy"]
 postgres = ["sqlalchemy", "psycopg2-binary"]
 
 [tool.poetry.group.sql.dependencies]
```

### Comparing `great_expectations_cloud-20240502.0.dev0/PKG-INFO` & `great_expectations_cloud-20240503.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240502.0.dev0
+Version: 20240503.0.dev1
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: postgres
 Provides-Extra: snowflake
 Requires-Dist: great-expectations (>=0.18.13,<0.19.0)
 Requires-Dist: orjson (>=3.9.7,<4.0.0,!=3.9.10)
-Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: packaging (>=21.3,<25.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: pydantic (<3)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Project-URL: Repository, https://github.com/great-expectations/cloud
 Description-Content-Type: text/markdown
 
 # cloud
```

