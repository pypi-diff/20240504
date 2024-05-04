# Comparing `tmp/zeblok-sdk-1.0.0.tar.gz` & `tmp/zeblok_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeblok-sdk-1.0.0.tar", last modified: Mon Feb 19 10:29:40 2024, max compression
+gzip compressed data, was "zeblok_sdk-1.1.0.tar", last modified: Sat May  4 05:01:02 2024, max compression
```

## Comparing `zeblok-sdk-1.0.0.tar` & `zeblok_sdk-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 10:29:40.278082 zeblok-sdk-1.0.0/
--rw-rw-rw-   0        0        0      158 2023-07-24 20:19:29.000000 zeblok-sdk-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      386 2024-02-19 10:29:40.278082 zeblok-sdk-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4034 2023-12-20 09:11:18.000000 zeblok-sdk-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-19 10:29:40.278082 zeblok-sdk-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      726 2024-02-19 09:57:33.000000 zeblok-sdk-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-19 10:29:40.252578 zeblok-sdk-1.0.0/tests/
--rw-rw-rw-   0        0        0     4023 2023-11-15 08:59:53.000000 zeblok-sdk-1.0.0/tests/test_api_auth.py
--rw-rw-rw-   0        0        0     3926 2023-11-09 07:18:30.000000 zeblok-sdk-1.0.0/tests/test_auth.py
--rw-rw-rw-   0        0        0     5997 2023-11-09 09:04:26.000000 zeblok-sdk-1.0.0/tests/test_datalake_auth.py
--rw-rw-rw-   0        0        0    28486 2023-12-08 10:01:35.000000 zeblok-sdk-1.0.0/tests/test_deploy.py
--rw-rw-rw-   0        0        0     3001 2023-11-02 11:33:51.000000 zeblok-sdk-1.0.0/tests/test_namespace.py
--rw-rw-rw-   0        0        0     7092 2023-11-02 11:41:39.000000 zeblok-sdk-1.0.0/tests/test_orchestration.py
--rw-rw-rw-   0        0        0    13785 2023-11-02 11:24:38.000000 zeblok-sdk-1.0.0/tests/test_plan.py
--rw-rw-rw-   0        0        0     9597 2023-12-08 10:01:35.000000 zeblok-sdk-1.0.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-19 10:29:40.262319 zeblok-sdk-1.0.0/zeblok/
--rw-rw-rw-   0        0        0      327 2024-02-12 00:01:37.000000 zeblok-sdk-1.0.0/zeblok/__init__.py
--rw-rw-rw-   0        0        0     9697 2024-02-12 00:23:26.000000 zeblok-sdk-1.0.0/zeblok/api.py
--rw-rw-rw-   0        0        0     2490 2023-12-20 09:11:18.000000 zeblok-sdk-1.0.0/zeblok/auth.py
-drwxrwxrwx   0        0        0        0 2024-02-19 10:29:40.268560 zeblok-sdk-1.0.0/zeblok/base/
--rw-rw-rw-   0        0        0        0 2023-11-21 08:39:11.000000 zeblok-sdk-1.0.0/zeblok/base/__init__.py
--rw-rw-rw-   0        0        0     4139 2024-02-12 00:14:55.000000 zeblok-sdk-1.0.0/zeblok/base/base_airuns.py
--rw-rw-rw-   0        0        0     1057 2023-12-20 15:23:23.000000 zeblok-sdk-1.0.0/zeblok/base/base_auth.py
--rw-rw-rw-   0        0        0     1534 2023-12-20 09:11:18.000000 zeblok-sdk-1.0.0/zeblok/base/base_service.py
--rw-rw-rw-   0        0        0      292 2023-11-23 06:00:40.000000 zeblok-sdk-1.0.0/zeblok/base/base_zbl.py
--rw-rw-rw-   0        0        0     8944 2024-02-12 05:17:28.000000 zeblok-sdk-1.0.0/zeblok/microservice.py
--rw-rw-rw-   0        0        0     4720 2023-12-20 09:11:18.000000 zeblok-sdk-1.0.0/zeblok/namspace.py
--rw-rw-rw-   0        0        0     7984 2024-02-11 23:22:33.000000 zeblok-sdk-1.0.0/zeblok/orchestration.py
--rw-rw-rw-   0        0        0     6617 2024-02-11 23:46:19.000000 zeblok-sdk-1.0.0/zeblok/plan.py
-drwxrwxrwx   0        0        0        0 2024-02-19 10:29:40.268560 zeblok-sdk-1.0.0/zeblok/utils/
--rw-rw-rw-   0        0        0        0 2023-11-15 02:39:00.000000 zeblok-sdk-1.0.0/zeblok/utils/__init__.py
--rw-rw-rw-   0        0        0     2900 2024-02-11 23:47:06.000000 zeblok-sdk-1.0.0/zeblok/utils/error_message.py
--rw-rw-rw-   0        0        0     2581 2023-12-20 12:08:49.000000 zeblok-sdk-1.0.0/zeblok/utils/errors.py
--rw-rw-rw-   0        0        0      727 2023-11-02 04:35:55.000000 zeblok-sdk-1.0.0/zeblok/utils/misc.py
--rw-rw-rw-   0        0        0     5347 2023-11-15 02:39:40.000000 zeblok-sdk-1.0.0/zeblok/utils/progressbar.py
--rw-rw-rw-   0        0        0    12944 2024-02-12 05:21:35.000000 zeblok-sdk-1.0.0/zeblok/utils/validations.py
-drwxrwxrwx   0        0        0        0 2024-02-19 10:29:40.278082 zeblok-sdk-1.0.0/zeblok_sdk.egg-info/
--rw-rw-rw-   0        0        0      386 2024-02-19 10:29:40.000000 zeblok-sdk-1.0.0/zeblok_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      792 2024-02-19 10:29:40.000000 zeblok-sdk-1.0.0/zeblok_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 10:29:40.000000 zeblok-sdk-1.0.0/zeblok_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-02-19 10:29:40.000000 zeblok-sdk-1.0.0/zeblok_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-19 10:29:40.000000 zeblok-sdk-1.0.0/zeblok_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.605584 zeblok_sdk-1.1.0/
+-rw-rw-rw-   0        0        0      158 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     3730 2024-05-04 05:01:02.604012 zeblok_sdk-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3302 2024-05-04 04:55:41.000000 zeblok_sdk-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 05:01:02.605584 zeblok_sdk-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-04 04:40:25.000000 zeblok_sdk-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.561550 zeblok_sdk-1.1.0/tests/
+-rw-rw-rw-   0        0        0     3913 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0     3107 2024-04-05 01:26:57.000000 zeblok_sdk-1.1.0/tests/test_namespace.py
+-rw-rw-rw-   0        0        0     7198 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_orchestration.py
+-rw-rw-rw-   0        0        0    13891 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_plan.py
+-rw-rw-rw-   0        0        0     9559 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.575035 zeblok_sdk-1.1.0/zeblok/
+-rw-rw-rw-   0        0        0      406 2024-04-10 09:30:10.000000 zeblok_sdk-1.1.0/zeblok/__init__.py
+-rw-rw-rw-   0        0        0     9679 2024-05-02 05:12:43.000000 zeblok_sdk-1.1.0/zeblok/api.py
+-rw-rw-rw-   0        0        0     2490 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.0/zeblok/auth.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.584569 zeblok_sdk-1.1.0/zeblok/base/
+-rw-rw-rw-   0        0        0        0 2023-11-21 08:39:11.000000 zeblok_sdk-1.1.0/zeblok/base/__init__.py
+-rw-rw-rw-   0        0        0     3493 2024-04-10 10:49:32.000000 zeblok_sdk-1.1.0/zeblok/base/base_airuns.py
+-rw-rw-rw-   0        0        0     1057 2023-12-20 15:23:23.000000 zeblok_sdk-1.1.0/zeblok/base/base_auth.py
+-rw-rw-rw-   0        0        0     5250 2024-05-01 05:23:24.000000 zeblok_sdk-1.1.0/zeblok/base/base_dataset.py
+-rw-rw-rw-   0        0        0     1535 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.0/zeblok/base/base_service.py
+-rw-rw-rw-   0        0        0      292 2023-11-23 06:00:40.000000 zeblok_sdk-1.1.0/zeblok/base/base_zbl.py
+-rw-rw-rw-   0        0        0     9729 2024-05-01 04:41:34.000000 zeblok_sdk-1.1.0/zeblok/dataset.py
+-rw-rw-rw-   0        0        0     8945 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.0/zeblok/microservice.py
+-rw-rw-rw-   0        0        0     4720 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.0/zeblok/namespace.py
+-rw-rw-rw-   0        0        0     8274 2024-05-03 08:09:55.000000 zeblok_sdk-1.1.0/zeblok/orchestration.py
+-rw-rw-rw-   0        0        0    14379 2024-05-03 07:28:33.000000 zeblok_sdk-1.1.0/zeblok/pipeline.py
+-rw-rw-rw-   0        0        0     6569 2024-05-03 10:47:22.000000 zeblok_sdk-1.1.0/zeblok/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.592406 zeblok_sdk-1.1.0/zeblok/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-15 02:39:00.000000 zeblok_sdk-1.1.0/zeblok/utils/__init__.py
+-rw-rw-rw-   0        0        0     3261 2024-03-30 04:04:56.000000 zeblok_sdk-1.1.0/zeblok/utils/error_message.py
+-rw-rw-rw-   0        0        0     2916 2024-04-30 10:37:29.000000 zeblok_sdk-1.1.0/zeblok/utils/errors.py
+-rw-rw-rw-   0        0        0      727 2023-11-02 04:35:55.000000 zeblok_sdk-1.1.0/zeblok/utils/misc.py
+-rw-rw-rw-   0        0        0     5347 2023-11-15 02:39:40.000000 zeblok_sdk-1.1.0/zeblok/utils/progressbar.py
+-rw-rw-rw-   0        0        0    13599 2024-04-28 03:10:00.000000 zeblok_sdk-1.1.0/zeblok/utils/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.602048 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3730 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/top_level.txt
```

### Comparing `zeblok-sdk-1.0.0/setup.py` & `zeblok_sdk-1.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from pip._internal.req import parse_requirements
 from setuptools import setup, find_packages
+from pathlib import Path
 import zeblok
 
 DESCRIPTION = 'Zeblok Python SDK'
-LONG_DESCRIPTION = 'Zeblok Python SDK to interact the Zeblok Ai-MicroCloud'
-
+# LONG_DESCRIPTION = 'Zeblok Python SDK to interact the Zeblok Ai-MicroCloud'
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 setup(
     name="zeblok-sdk",
     version=zeblok.__version__,
     author="Karan Pathak",
     author_email="karan@dataturtles.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
+    long_description_content_type='text/markdown',
     url="",
     packages=find_packages(),
     install_requires=[item.requirement for item in parse_requirements('requirements.txt', session=False)],
     python_requires=">=3.9",
     keywords=['python', 'zeblok'],
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
-)
+)
```

### Comparing `zeblok-sdk-1.0.0/tests/test_auth.py` & `zeblok_sdk-1.1.0/tests/test_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import pytest
-from zeblok_old.auth import AuthOld
-from zeblok.utils.errors import InvalidCredentialsError, AuthenticationError, ServerError, InvalidURL
+from zeblok.auth import Auth
+from zeblok.errors import InvalidCredentialsError, AuthenticationError, ServerError, InvalidURL
+
+
+@pytest.fixture()
+def auth_data():
+    return {'username': 'temp_username', 'password': 'temp_password', 'base_url': 'app.zbl-aws.zeblok.com'}
 
 
-@pytest.mark.skip(reason="Old test")
 class TestAuthInstanceCreation:
     def test_invalid_int_username(self, auth_data):
         with pytest.raises(expected_exception=InvalidCredentialsError, match='username can only be of type String'):
             auth_data.pop('username')
-            AuthOld(username=1, **auth_data)
+            Auth(username=1, **auth_data)
 
     def test_invalid_int_password(self, auth_data):
         with pytest.raises(expected_exception=InvalidCredentialsError, match='password can only be of type String'):
             auth_data.pop('password')
-            AuthOld(password=1, **auth_data)
+            Auth(password=1, **auth_data)
 
     def test_invalid_int_base_url(self, auth_data):
         with pytest.raises(expected_exception=InvalidURL, match='base_url can only be of type String'):
             auth_data.pop('base_url')
-            AuthOld(base_url=1, **auth_data)
+            Auth(base_url=1, **auth_data)
 
     def test_invalid_empty_username(self, auth_data):
         with pytest.raises(expected_exception=InvalidCredentialsError, match='username cannot empty'):
             auth_data.pop('username')
-            AuthOld(username='', **auth_data)
+            Auth(username='', **auth_data)
 
     def test_invalid_empty_password(self, auth_data):
         with pytest.raises(expected_exception=InvalidCredentialsError, match='password cannot empty'):
             auth_data.pop('password')
-            AuthOld(password='', **auth_data)
+            Auth(password='', **auth_data)
 
     def test_invalid_empty_base_url(self, auth_data):
         with pytest.raises(expected_exception=InvalidURL, match='base_url cannot empty'):
             auth_data.pop('base_url')
-            AuthOld(base_url='', **auth_data)
+            Auth(base_url='', **auth_data)
 
 
-@pytest.mark.skip(reason="Old test")
 class TestBasicMemberFunctions:
     def test_get_username(self, auth_data):
-        assert AuthOld(**auth_data).get_username() == auth_data['username']
+        assert Auth(**auth_data).get_username() == auth_data['username']
 
     def test_get_password(self, auth_data):
-        assert AuthOld(**auth_data).get_password() == auth_data['password']
+        assert Auth(**auth_data).get_password() == auth_data['password']
 
 
-@pytest.mark.skip(reason="Old test")
 class TestTokenMechanism:
     def test_get_token_from_local(self, auth_data, monkeypatch):
         temp_token = 'temp_token'
-        temp_auth_obj = AuthOld(**auth_data)
+        temp_auth_obj = Auth(**auth_data)
         monkeypatch.setattr(temp_auth_obj, '_Auth__token', temp_token)
         assert temp_auth_obj.get_token() == temp_token
 
     def test_get_token_from_server(self, auth_data, monkeypatch):
         import requests
         temp_token = 'temp_token'
 
@@ -62,15 +64,15 @@
                 self.status_code = 200
 
             @staticmethod
             def json():
                 return {'data': temp_token}
 
         monkeypatch.setattr(requests, 'post', MockResponse)
-        assert AuthOld(**auth_data).get_token() == "Bearer " + temp_token
+        assert Auth(**auth_data).get_token() == "Bearer " + temp_token
 
     def test_get_token_wrong_credentials(self, auth_data, monkeypatch):
         import requests
         error_message = 'wrong_credentials'
 
         class MockResponse:
             def __init__(self, url, headers, data):
@@ -78,20 +80,20 @@
 
             @staticmethod
             def json():
                 return {'message': error_message}
 
         monkeypatch.setattr(requests, 'post', MockResponse)
         with pytest.raises(expected_exception=AuthenticationError, match=error_message):
-            AuthOld(**auth_data).get_token()
+            Auth(**auth_data).get_token()
 
     def test_get_token_unknown_error(self, auth_data, monkeypatch):
         import requests
 
         class MockResponse:
             def __init__(self, url, headers, data):
                 self.status_code = 500
 
         monkeypatch.setattr(requests, 'post', MockResponse)
         with pytest.raises(expected_exception=ServerError,
                            match=f"Status code = {MockResponse('', '', '').status_code}"):
-            AuthOld(**auth_data).get_token()
+            Auth(**auth_data).get_token()
```

### Comparing `zeblok-sdk-1.0.0/tests/test_namespace.py` & `zeblok_sdk-1.1.0/tests/test_namespace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import pathlib
+import os
 import pytest
-from zeblok.namspace import NamespaceOld
-from zeblok.utils.errors import AuthenticationError, ServerError
+from zeblok.namspace import Namespace
+from zeblok.errors import InvalidCredentialsError, AuthenticationError, ServerError, ModelDeploymentError, \
+    InvalidModelFolder, FileUploadError
 import requests
 
 AUTHENTICATION_MESSAGE = 'User not authenticated. Please check your token or api_access_key or api_access_secret'
 TEMP_ERROR_TEXT = 'error_text'
 SECRET_KEY = 'some_secret_key'
 USERNAME = 'temp_username'
 MODEL_FOLDER_PATH = 'temp_model_folder_path'
 TEST_TOKEN = 'Bearer temp-token'
 
 
 @pytest.fixture
 def namespace_data():
-    return NamespaceOld(base_url='temp_base_url')
+    return Namespace(base_url='temp_base_url')
 
 
 class MockServerErrorResponse:
     def __init__(self, url, headers):
         self.status_code = 500
         self.text = TEMP_ERROR_TEXT
```

### Comparing `zeblok-sdk-1.0.0/tests/test_orchestration.py` & `zeblok_sdk-1.1.0/tests/test_orchestration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import pathlib
+import os
 import pytest
-from zeblok.orchestration import OrchestrationOld
-from zeblok.utils.errors import AuthenticationError, ServerError
+from zeblok.orchestration import Orchestration
+from zeblok.errors import InvalidCredentialsError, AuthenticationError, ServerError, ModelDeploymentError, \
+    InvalidModelFolder, FileUploadError
 import requests
 
 AUTHENTICATION_MESSAGE = 'User not authenticated. Please check your token or api_access_key or api_access_secret'
 TEMP_ERROR_TEXT = 'error_text'
 SECRET_KEY = 'some_secret_key'
 USERNAME = 'temp_username'
 MODEL_FOLDER_PATH = 'temp_model_folder_path'
 TEST_TOKEN = 'Bearer temp-token'
 
 
 @pytest.fixture
 def orchestration_data():
-    return OrchestrationOld(base_url='temp_base_url')
+    return Orchestration(base_url='temp_base_url')
 
 
 class MockServerErrorResponse:
     def __init__(self, url, headers):
         self.status_code = 500
         self.text = TEMP_ERROR_TEXT
```

### Comparing `zeblok-sdk-1.0.0/tests/test_plan.py` & `zeblok_sdk-1.1.0/tests/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import pathlib
+import os
 import pytest
-from zeblok.plan import PlanOld
-from zeblok.utils.errors import AuthenticationError, ServerError
+from zeblok.plan import Plan
+from zeblok.errors import InvalidCredentialsError, AuthenticationError, ServerError, ModelDeploymentError, \
+    InvalidModelFolder, FileUploadError
 import requests
 
 AUTHENTICATION_MESSAGE = 'User not authenticated. Please check your token or api_access_key or api_access_secret'
 TEMP_ERROR_TEXT = 'error_text'
 SECRET_KEY = 'some_secret_key'
 USERNAME = 'temp_username'
 MODEL_FOLDER_PATH = 'temp_model_folder_path'
 TEST_TOKEN = 'Bearer temp-token'
 
 
 @pytest.fixture
 def plan_data():
-    return PlanOld(base_url='temp_base_url')
+    return Plan(base_url='temp_base_url')
 
 
 class MockServerErrorResponse:
     def __init__(self, url, headers):
         self.status_code = 500
         self.text = TEMP_ERROR_TEXT
```

### Comparing `zeblok-sdk-1.0.0/tests/test_utils.py` & `zeblok_sdk-1.1.0/tests/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 import pathlib
 import os
-from zeblok.utils import seconds_to_time, Progress
-from zeblok.utils.validations import validate_secret_key, validate_datalake_url, validate_ai_api_name, \
-    validate_model_version, basic_validate_namespace_id, validate_platform_id, validate_model_pipeline, validate_model_folder, \
-    validate_envs_args, validate_token, validate_id
-from zeblok.utils.errors import InvalidCredentialsError, InvalidURL
+from zeblok.utils import seconds_to_time, Progress, validate_secret_key, validate_id, validate_token, \
+    validate_model_pipeline, validate_envs_args, validate_platform_id, validate_namespace_id, validate_deployment_name, \
+    validate_model_version, validate_storage_url, validate_model_folder
+from zeblok.errors import InvalidCredentialsError, InvalidURL
 
 
 @pytest.fixture
 def progress_init():
     return Progress()
 
 
@@ -153,21 +152,21 @@
 
 
 class TestValidateNamespaceId:
     def test_int_namespace_id(self):
         with pytest.raises(
                 expected_exception=ValueError, match="namespace_id can only be of type String"
         ):
-            basic_validate_namespace_id(namespace_id=123)
+            validate_namespace_id(namespace_id=123)
 
     def test_empty_namespace_id(self):
         with pytest.raises(
                 expected_exception=ValueError, match="namespace_id cannot empty"
         ):
-            basic_validate_namespace_id(namespace_id="")
+            validate_namespace_id(namespace_id="")
 
 
 class TestValidateModelVersion:
     def test_int_model_version(self):
         with pytest.raises(
                 expected_exception=ValueError, match="model_version can only be of type String"
         ):
@@ -179,41 +178,41 @@
         ):
             validate_model_version(model_version="")
 
 
 class TestValidateDeploymentName:
     def test_int_deployment_name(self):
         with pytest.raises(
-                expected_exception=ValueError, match="ai_api_type can only be of type String"
+                expected_exception=ValueError, match="deployment_name can only be of type String"
         ):
-            validate_ai_api_name(ai_api_name=123)
+            validate_deployment_name(deployment_name=123)
 
     def test_empty_deployment_name(self):
         with pytest.raises(
-                expected_exception=ValueError, match="ai_api_type cannot empty"
+                expected_exception=ValueError, match="deployment_name cannot empty"
         ):
-            validate_ai_api_name(ai_api_name="")
+            validate_deployment_name(deployment_name="")
 
 
 class TestValidateStorageURL:
     """
     To be deprecated in future versions
     """
 
     def test_int_storage_url(self):
         with pytest.raises(
                 expected_exception=InvalidURL, match="storage_url can only be of type String"
         ):
-            validate_datalake_url(datalake_url=123)
+            validate_storage_url(storage_url=123)
 
     def test_empty_storage_url(self):
         with pytest.raises(
                 expected_exception=InvalidURL, match="storage_url cannot empty"
         ):
-            validate_datalake_url(datalake_url="")
+            validate_storage_url(storage_url="")
 
 
 class TestValidateModelFolder:
 
     def test_empty_folder_path(self):
         with pytest.raises(expected_exception=ValueError, match="Model folder path is empty"):
             validate_model_folder(model_folder_path=pathlib.Path(""))
```

### Comparing `zeblok-sdk-1.0.0/zeblok/api.py` & `zeblok_sdk-1.1.0/zeblok/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Union, Tuple, List, Dict
 from pathlib import Path
 import time
 from .utils.errors import api_error
 import requests
 import json
 from .base.base_airuns import AIRunsBase
-from .auth import APIAuth, DatalakeAuth
-from . import AI_API_DOCKER_FOLDER
+from .auth import APIAuth
+from . import DOCKER_HUB_URL
 from .utils.validations import validate_ai_api_name, validate_ai_api_type
-from .utils.error_message import NO_AI_APIs_STATE
+from .utils.error_message import NO_AI_API_STATE
 from . import PLAN_TYPE_API, PLAN_TYPE_CAAS
 from .utils.error_message import NO_AI_API_IMAGE_NAME
+from .dataset import DataSet
 
 
 class API(AIRunsBase):
-    def __int__(self, api_auth: APIAuth, datalake_auth: DatalakeAuth):
-        super().__init__(api_auth, datalake_auth)
+    def __int__(self, api_auth: APIAuth, dataset: DataSet):
+        super().__init__(api_auth, dataset)
 
     @staticmethod
     def __print_info(ai_apis: List[Dict], state: str, error_message: str = None):
         print(f"AI-APIs with state: {state}")
         if len(ai_apis) > 0:
             for idx, data in enumerate(ai_apis):
                 print(f"\t{idx + 1}. id: {data['id']} | image_name: {data['image_name']} | type: {data['type']}")
@@ -82,15 +83,15 @@
 
     def _create(self, ai_api_name: str, ai_api_type: str) -> Tuple[str, str]:
         validate_ai_api_name(ai_api_name=ai_api_name)
         validate_ai_api_type(ai_api_type=ai_api_type)
 
         image_version = int(time.time())
 
-        image_name = f"{AI_API_DOCKER_FOLDER}/{'-'.join(ai_api_name.strip().split(' '))}:{image_version}".lower()
+        image_name = f"{DOCKER_HUB_URL}/{'-'.join(ai_api_name.strip().split(' '))}:{image_version}".lower()
 
         response = requests.post(
             f"{self._api_auth.app_url}/api/v1/aimodel/",
             headers={'Content-Type': 'application/json'},
             data=json.dumps({"imageName": image_name, "type": ai_api_type.strip()}),
             auth=self._api_auth.get_api_creds()
         )
@@ -116,15 +117,14 @@
         ai_api_data = self.__get(state=state, return_data=True, raise_exception=False, error_message=None)
 
         return image_name.strip() in [_ai_api['image_name'] for _ai_api in ai_api_data]
 
     def create_and_spawn(
             self, ai_api_name: str, model_folder_path: str, ai_api_plan_id: str, namespace_id: str, caas_plan_id: str,
             ai_api_type='llm'
-
     ):
         self._namespace.validate_id(namespace_id=namespace_id, raise_exception=True)
         datacenter_id = self._validate_plan_and_get_datacenter(ai_api_plan_id, PLAN_TYPE_API)
 
         caas_datacenter_id = self._validate_plan_and_get_datacenter(caas_plan_id, PLAN_TYPE_CAAS)
 
         if caas_datacenter_id != datacenter_id:
@@ -216,13 +216,13 @@
             \t{response.text}
             """
         )
 
     def get_all(self, state: str = 'deployed', print_stdout: bool = True):
         ai_api_data = self.__get(
             state=state, return_data=True, raise_exception=False,
-            error_message=NO_AI_APIs_STATE.format(state=state)
+            error_message=NO_AI_API_STATE.format(state=state)
         )
         if print_stdout:
-            self.__print_info(ai_apis=ai_api_data, state=state, error_message=NO_AI_APIs_STATE.format(state=state))
+            self.__print_info(ai_apis=ai_api_data, state=state, error_message=NO_AI_API_STATE.format(state=state))
 
         return ai_api_data
```

### Comparing `zeblok-sdk-1.0.0/zeblok/auth.py` & `zeblok_sdk-1.1.0/zeblok/auth.py`

 * *Files identical despite different names*

### Comparing `zeblok-sdk-1.0.0/zeblok/base/base_airuns.py` & `zeblok_sdk-1.1.0/zeblok/base/base_airuns.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from .base_service import ServiceSpawnBase
 from zipfile import ZipFile
 from pathlib import Path
 import minio
 import os
 from typing import Union
 from ..utils.progressbar import Progress
-from ..utils.errors import BucketDoesNotExistsError,api_error
+from ..utils.errors import api_error, CaaSUploadError
 from ..utils.misc import get_all_file_paths
 from ..utils.validations import validate_model_folder
+from ..dataset import DataSet
 
 
 class AIRunsBase(ServiceSpawnBase):
     __slots__ = ['_plan']
 
-    def __init__(self, api_auth: APIAuth, datalake_auth: DatalakeAuth):
+    def __init__(self, api_auth: APIAuth, dataset: DataSet):
         super().__init__(api_auth)
-        self._datalake_auth = datalake_auth
+        self._dataset = dataset
 
     def _call_containerization_service(
             self, presigned_get_url: str, image_name: str, file_name: str, image_id: str, caas_plan_id: str,
             deployment_type: str, error_msg: str, plan_id: Union[str, list[str], None] = None, autodeploy: bool = False,
             deployment_name: Union[str, None] = None, namespace_id: Union[str, None] = None,
             datacenter_ids: Union[str, list[str], None] = None
     ):
@@ -66,36 +67,21 @@
             for file in file_paths:
                 zip.write(filename=file.as_posix(), arcname=file.relative_to(model_folder_path))
         print("Model zip prepared")
         return model_zipfile_path
 
     def _upload_file_to_datalake(self, file_name: Path) -> str:
         try:
-            client = minio.Minio(
-                endpoint=self._datalake_auth.datalake_url, access_key=self._datalake_auth.datalake_username,
-                secret_key=self._datalake_auth.datalake_secret_key, secure=True
-            )
-
-            if not self._datalake_auth.bucket_exists():
-                raise BucketDoesNotExistsError(f'{self._datalake_auth.bucket_name} does not exists')
-
-            client.fput_object(
-                bucket_name=self._datalake_auth.bucket_name, object_name=f"{file_name.name}",
-                file_path=file_name.as_posix(), content_type="application/zip",
-                progress=Progress(), part_size=10 * 1024 * 1024
-            )
-
-            url = client.presigned_get_object(
-                bucket_name=self._datalake_auth.bucket_name, object_name=f"{file_name.name}",
-                expires=timedelta(hours=3)
-            )
+
+            if not self._dataset.upload_object(local_file_pathname=file_name):
+                raise CaaSUploadError(f"Error Uploading {file_name} to bucket {self._dataset.bucket_name}")
             print("")
+            return self._dataset.get_presigned_url(object_name=file_name.name)
         finally:
             os.remove(file_name)
-        return url
 
     @abstractmethod
     def _create(self, *args, **kwargs):
         pass
 
     @abstractmethod
     def create_and_spawn(self, *args, **kwargs):
```

### Comparing `zeblok-sdk-1.0.0/zeblok/base/base_auth.py` & `zeblok_sdk-1.1.0/zeblok/base/base_auth.py`

 * *Files identical despite different names*

### Comparing `zeblok-sdk-1.0.0/zeblok/base/base_service.py` & `zeblok_sdk-1.1.0/zeblok/base/base_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 
 from ..auth import APIAuth
 from .base_zbl import ZBLBase
 from typing import Union, List
 from ..plan import Plan
-from ..namspace import Namespace
+from ..namespace import Namespace
 from ..utils.error_message import INCOMPATIBLE_SERVICE_PLAN_ID, PLAN_ID_TYPE_UNAVAILABLE, PLAN_ID_DATACENTER_UNAVAILABLE
 
 
 class ServiceSpawnBase(ZBLBase):
     def __init__(self, api_auth: APIAuth):
         super().__init__(api_auth)
         self._plan = Plan(api_auth)
```

### Comparing `zeblok-sdk-1.0.0/zeblok/microservice.py` & `zeblok_sdk-1.1.0/zeblok/microservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .auth import APIAuth
 from .base.base_service import ServiceSpawnBase
 from .plan import Plan
-from .namspace import Namespace
+from .namespace import Namespace
 from .utils.errors import api_error
 from .utils.error_message import NO_MICROSERVICES, NO_MICROSERVICES_ID, INVALID_MICROSERVICE_DISPLAY_NAME
 import requests
 import json
 from typing import List, Union, Dict
 from . import PLAN_TYPE_MICROSERVICE
 from .utils.validations import validate_microservice_name, validate_microservice_display_name, \
```

### Comparing `zeblok-sdk-1.0.0/zeblok/namspace.py` & `zeblok_sdk-1.1.0/zeblok/namespace.py`

 * *Files identical despite different names*

### Comparing `zeblok-sdk-1.0.0/zeblok/orchestration.py` & `zeblok_sdk-1.1.0/zeblok/orchestration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from . import PLAN_TYPE_ORCHESTRATION
 from .utils.errors import api_error
 from .auth import APIAuth
 from .plan import Plan
-from .namspace import Namespace
+from .namespace import Namespace
 from .base.base_service import ServiceSpawnBase
 from .utils.validations import validate_orchestration_name, validate_orchestration_workers
 from .utils.error_message import NO_ORCHESTRATIONS, NO_ORCHESTRATION_ID
 from typing import List, Dict, Union
 
 
 class Orchestration(ServiceSpawnBase):
@@ -21,33 +21,37 @@
     @staticmethod
     def __print_info(orchestrations: List[Dict], error_message: str = None):
         print("Orchestrations:")
         if len(orchestrations) > 0:
             for idx, data in enumerate(orchestrations):
                 print(f"\t{idx + 1}. {data['name']}")
                 print(
-                    f"\t\tid: {data['id']} | description: {data['description']} | default plan: {data['default_plan']} | added by: {data['added_by']} | organisation id: {data['organisation_id']} | is_public: {data['is_public']}"
+                    f"\t\tid: {data['id']} | description: {data['description']} | default plan: {data['default_plan']} | added by: {data['added_by']['username']} ({data['added_by']['id']}) | organisation id: {data['organisation_id']} | is_public: {data['is_public']}"
                 )
                 print(f"\t\tPlans: {', '.join([p['name'] + ' (' + p['id'] + ')' for p in data['plans']])}")
                 print()
         else:
             print("No resources available" if error_message is None else error_message)
 
     def __process_single_element(self, element: Dict) -> Dict:
         e = {
             'id': element.get('_id', None), 'name': element.get('name', None), 'description': element['description'],
-            'added_by': element['addedBy'], 'organisation_id': element['organisationId'],
-            'is_public': element['isPublic'],
+            'organisation_id': element['organisationId'], 'is_public': element['isPublic'],
+            'added_by': {
+                'id': element['addedBy']['_id'], 'name': element['addedBy']['name'],
+                'email': element['addedBy']['email'], 'username': element['addedBy']['username']
+            },
             'plans': [
-                self.__plan.get_filtered_details(plan_id=plan_id, fields_req=['id', 'name']) for plan_id in
+                self.__plan.get_filtered_details(plan_id=_plan['_id'], fields_req=['id', 'name']) for _plan in
                 element['plans']
             ]
         }
 
-        _default_plan = self.__plan.get_filtered_details(plan_id=element['defaultPlan'], fields_req=['id', 'name'])
+        _default_plan = self.__plan.get_filtered_details(plan_id=element['defaultPlan']['_id'],
+                                                         fields_req=['id', 'name'])
 
         e['default_plan'] = f"{_default_plan['name']} ({_default_plan['id']})"
 
         return e
 
     def __process_response(
             self,
```

### Comparing `zeblok-sdk-1.0.0/zeblok/plan.py` & `zeblok_sdk-1.1.0/zeblok/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if len(plans) > 0:
             for idx, data in enumerate(plans):
                 print(f"\t{idx + 1}. {data['name']}")
                 print(
                     f"\t\tid: {data['id']} | type: {data['type']} | price: {data['currency']} {data['price']} | added_by: {data.get('added_by', None)} | is_public: {data['is_public']}"
                 )
                 print(
-                    f"\t\tResources = CPU: {data['resources']['CPU']} vCPU | #GPUs: {data['resources']['GPU']} | Memory: {data['resources']['memory']} GB | Storage: {data['resources']['storage']} GB | Workers: {data['resources']['workers']}"
+                    f"\t\tResources = CPU: {data['resources']['CPU']} vCPU | #GPUs: {data['resources']['GPU']} | Memory: {data['resources']['memory']} GB | Storage: {data['resources']['storage']} GB"
                 )
                 print(f"\t\tData Center = id: {data['data_center']['id']} | name: {data['data_center']['name']}")
                 print(f"\t\tOrganization = id: {data['organization']['id']} | name: {data['organization']['name']}")
                 print()
         else:
             print("No resources available" if error_message is None else error_message)
 
@@ -85,17 +85,17 @@
                 plan_data = list(map(lambda data: cls.__process_single_element(data), __resp_data))
 
         return plan_data
 
     @staticmethod
     def __basic_id_validation(resource_id: str):
         if type(resource_id) is not str:
-            raise TypeError(f'ai_api_plan_id can only be of type String')
+            raise TypeError(f'resource_id can only be of type String')
         if resource_id.strip() == '':
-            raise ValueError(f'ai_api_plan_id cannot empty')
+            raise ValueError(f'resource_id cannot empty')
 
     def __get(
             self, resource_id: str = None, return_data: bool = True,
             raise_exception: bool = True, error_message: str = None,
     ) -> Union[List[Dict], Dict, bool, None]:
         __base_url = f"{self._api_auth.app_url}/api/v1/plans"
```

### Comparing `zeblok-sdk-1.0.0/zeblok/utils/error_message.py` & `zeblok_sdk-1.1.0/zeblok/utils/error_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # GENERAL
 
 INCOMPATIBLE_SERVICE_PLAN_ID = r'The given plan id ({plan_id}) has a service type `{service_type_1}`. Expected a plan with service type `{service_type_2}`.'
 PLAN_ID_TYPE_UNAVAILABLE = r'Could not find the `type` of the plan id ({plan_id}).'
 PLAN_ID_DATACENTER_UNAVAILABLE = r'Could not find the `DataCenter` of the plan id ({plan_id}).'
 
-
 EMPTY_MODEL_FOLDER_PATH = r"model_folder_path is empty"
 MODEL_FOLDER_PATH_NOT_DIR = r"{model_folder_path} is not a Directory."
 MODEL_FOLDER_PATH_DOES_NOT_EXIST = r"No such Directory ({model_folder_path}) found."
 MODEL_FOLDER_PARENT_PATH_NO_WRITE_PERMISSION = r"Directory ({model_folder_path}) does not have write permission."
 
 # API_ACCESS_KEY
 INVALID_API_ACCESS_KEY_TYPE = r'API_ACCESS_KEY can only be of type String'
@@ -39,20 +38,25 @@
 NO_PLAN_ID = r"No plan with id ({plan_id}) in this environment."
 
 # MICROSERVICES
 NO_MICROSERVICES = r"No microservice available in this environment. Please create a microservice."
 NO_MICROSERVICES_ID = r"No microservice with id ({microservice_id}) in this environment."
 INVALID_MICROSERVICE_DISPLAY_NAME = r"MicroService (id: {microservice_id}) has no display_name `{display_name}`."
 
-
 # ORCHESTRATION
 NO_ORCHESTRATIONS = r"No orchestrations available in this environment. Please create an orchestration."
 NO_ORCHESTRATION_ID = r"No orchestration with id ({orchestration_id}) in this environment."
 
+# AI-PIPELINE
+EMPTY_AI_PIPELINE_NAME = r'ai_pipeline_name cannot be empty'
+INVALID_AI_PIPELINE_NAME_TYPE = r"ai_pipeline_name can only be of type String"
+NO_AI_PIPELINE_STATE = r"No AI-Pipeline available in this environment with {state} state."
+NO_AI_PIPELINE_IMAGE_NAME = r"No `created` state AI-Pipeline with image_name ({image_name}) in this environment."
+
 # AI-API
 INVALID_AI_API_NAME_TYPE = r"ai_api_type can only be of type String"
 EMPTY_AI_API_NAME = r'ai_api_type cannot be empty'
 INVALID_AI_API_TYPE_TYPE = r"ai_api_type can only be of type String"
 EMPTY_AI_API_TYPE = r'ai_api_type cannot be empty'
 INVALID_AI_API_TYPE = r"ai_api_type should be one of 'bentoml', 'openvino', 'mlflow','llm'"
-NO_AI_APIs_STATE = r"No AI-APIs available in this environment with {state} state."
+NO_AI_API_STATE = r"No AI-APIs available in this environment with {state} state."
 NO_AI_API_IMAGE_NAME = r"No `ready` state AI-API with image_name ({image_name}) in this environment."
```

### Comparing `zeblok-sdk-1.0.0/zeblok/utils/errors.py` & `zeblok_sdk-1.1.0/zeblok/utils/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,29 @@
 
 
 class BucketDoesNotExistsError(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
+class ObjectDoesNotExistsError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
 class FileUploadError(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
+class FileDownloadError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
 class ModelDeploymentError(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
 class PipelineCreationError(Exception):
     def __init__(self, message):
@@ -77,14 +87,19 @@
 
 
 class AIAPISpawnError(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
+class CaaSUploadError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
 def api_error(status_code: int, message: str = ""):
     if status_code == 200:
         raise NoResourcesError(message if message else "No respective resources in this environment.")
 
     if status_code == 401:
         raise AuthenticationError(
             "User not authenticated. Please check your token or api_access_key or api_access_secret"
```

### Comparing `zeblok-sdk-1.0.0/zeblok/utils/misc.py` & `zeblok_sdk-1.1.0/zeblok/utils/misc.py`

 * *Files identical despite different names*

### Comparing `zeblok-sdk-1.0.0/zeblok/utils/progressbar.py` & `zeblok_sdk-1.1.0/zeblok/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `zeblok-sdk-1.0.0/zeblok/utils/validations.py` & `zeblok_sdk-1.1.0/zeblok/utils/validations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 from pathlib import Path
-from .errors import InvalidCredentialsError, DirectoryNotFoundError, BucketDoesNotExistsError, InvalidBucketName
 from typing import List, Dict
+
+from minio import Minio
+
 from .error_message import MODEL_FOLDER_PATH_DOES_NOT_EXIST, INVALID_AI_API_NAME_TYPE, EMPTY_AI_API_NAME, \
     INVALID_AI_API_TYPE_TYPE, EMPTY_AI_API_TYPE, INVALID_AI_API_TYPE, EMPTY_MODEL_FOLDER_PATH, \
     MODEL_FOLDER_PATH_NOT_DIR, MODEL_FOLDER_PARENT_PATH_NO_WRITE_PERMISSION, INVALID_API_ACCESS_KEY_TYPE, \
     EMPTY_API_ACCESS_KEY, INVALID_API_ACCESS_SECRET_TYPE, EMPTY_API_ACCESS_SECRET, INVALID_DATALAKE_USERNAME_TYPE, \
     EMPTY_DATALAKE_USERNAME, INVALID_DATALAKE_SECRET_KEY_TYPE, EMPTY_DATALAKE_SECRET_KEY, INVALID_BUCKET_NAME_TYPE, \
-    EMPTY_BUCKET_NAME
-from minio import Minio
+    EMPTY_BUCKET_NAME, EMPTY_AI_PIPELINE_NAME, INVALID_AI_PIPELINE_NAME_TYPE
+from .errors import InvalidCredentialsError, DirectoryNotFoundError, BucketDoesNotExistsError, InvalidBucketName
 
 URL_PATTERN_WITHOUT_SCHEME = "^[-a-zA-Z0-9@:%._\\+~#=]{1,256}\\.[a-zA-Z0-9()]{1,6}\\b(?:[-a-zA-Z0-9()@:%_\\+.~#?&\\/=]*)$"
 
 
 def __is_list_of_dicts(variable):
     return isinstance(variable, list) and all(isinstance(item, dict) for item in variable)
 
@@ -326,21 +328,42 @@
         return
 
     for _p in args:
         if _p.get("key", None) is None:
             raise ValueError("`key` key missing args. Please check your input for `ports`.")
 
 
-# def validate_microservice_command(command: str):
-#     if type(command) is not str:
-#         raise ValueError('command parameter can only be of type String')
-#     if command is None:
-#         raise ValueError('command parameter cannot be None')
-#     if command == '':
-#         raise ValueError('command parameter cannot empty')
+def validate_ai_pipeline_name(ai_pipeline_name: str):
+    if ai_pipeline_name is None:
+        raise ValueError("ai_pipeline_name cannot be None")
+    if type(ai_pipeline_name) is not str:
+        raise TypeError(INVALID_AI_PIPELINE_NAME_TYPE)
+    if ai_pipeline_name.strip() == '':
+        raise ValueError(EMPTY_AI_PIPELINE_NAME)
+
+
+def has_permission(filepath: Path, permission: str = "read") -> bool:
+    if permission == "write":
+        try:
+            with open(filepath, "w") as __temp_file:
+                __temp_file.write("Testing write permission in file.")
+            os.remove(filepath)
+            return True
+        except PermissionError as _:
+            return False
+
+    if permission == "read":
+        try:
+            with open(filepath, "r") as __temp_file:
+                pass
+            return True
+        except PermissionError as _:
+            return False
+
+    return False
 
 
 """
 OLD CODE
 """
```

### Comparing `zeblok-sdk-1.0.0/zeblok_sdk.egg-info/SOURCES.txt` & `zeblok_sdk-1.1.0/zeblok_sdk.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 LICENSE.md
 README.md
 setup.py
-tests/test_api_auth.py
 tests/test_auth.py
-tests/test_datalake_auth.py
-tests/test_deploy.py
 tests/test_namespace.py
 tests/test_orchestration.py
 tests/test_plan.py
 tests/test_utils.py
 zeblok/__init__.py
 zeblok/api.py
 zeblok/auth.py
+zeblok/dataset.py
 zeblok/microservice.py
-zeblok/namspace.py
+zeblok/namespace.py
 zeblok/orchestration.py
+zeblok/pipeline.py
 zeblok/plan.py
 zeblok/base/__init__.py
 zeblok/base/base_airuns.py
 zeblok/base/base_auth.py
+zeblok/base/base_dataset.py
 zeblok/base/base_service.py
 zeblok/base/base_zbl.py
 zeblok/utils/__init__.py
 zeblok/utils/error_message.py
 zeblok/utils/errors.py
 zeblok/utils/misc.py
 zeblok/utils/progressbar.py
```

