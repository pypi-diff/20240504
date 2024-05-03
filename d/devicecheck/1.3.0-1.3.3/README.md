# Comparing `tmp/devicecheck-1.3.0.tar.gz` & `tmp/devicecheck-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/devicecheck/devicecheck/dist/.tmp-x5o3se2f/devicecheck-1.3.0.tar", last modified: Sun Mar 31 12:24:55 2024, max compression
+gzip compressed data, was "/home/runner/work/devicecheck/devicecheck/dist/.tmp-fdvb3kns/devicecheck-1.3.3.tar", last modified: Fri May  3 22:37:27 2024, max compression
```

## Comparing `devicecheck-1.3.0.tar` & `devicecheck-1.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:24:55.000000 devicecheck-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-31 12:24:51.000000 devicecheck-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-03-31 12:24:55.000000 devicecheck-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck/
--rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-03-31 12:24:51.000000 devicecheck-1.3.0/devicecheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-31 12:24:51.000000 devicecheck-1.3.0/devicecheck/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-03-31 12:24:51.000000 devicecheck-1.3.0/devicecheck/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 12:24:55.000000 devicecheck-1.3.0/devicecheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-31 12:24:51.000000 devicecheck-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 12:24:55.000000 devicecheck-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-31 12:24:51.000000 devicecheck-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:37:27.000000 devicecheck-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 22:37:22.000000 devicecheck-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-03 22:37:27.000000 devicecheck-1.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck/
+-rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-05-03 22:37:22.000000 devicecheck-1.3.3/devicecheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-03 22:37:22.000000 devicecheck-1.3.3/devicecheck/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-05-03 22:37:22.000000 devicecheck-1.3.3/devicecheck/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 22:37:27.000000 devicecheck-1.3.3/devicecheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 22:37:22.000000 devicecheck-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:37:27.000000 devicecheck-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 22:37:22.000000 devicecheck-1.3.3/setup.py
```

### Comparing `devicecheck-1.3.0/LICENSE` & `devicecheck-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devicecheck-1.3.0/PKG-INFO` & `devicecheck-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicecheck
-Version: 1.3.0
+Version: 1.3.3
 Summary: Apple DeviceCheck API. Reduce fraudulent use of your services by managing device state and asserting app integrity.
 Home-page: https://github.com/Kylmakalle/devicecheck
 Author: Sergey Akentev
 Author-email: "S. Akentev" <sergey+gh@akentev.com>
 Project-URL: Issue Tracker, https://github.com/Kylmakalle/devicecheck/issues
 Project-URL: Repository, https://github.com/Kylmakalle/devicecheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `devicecheck-1.3.0/devicecheck/__init__.py` & `devicecheck-1.3.3/devicecheck/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Python Implementation of Apple DeviceCheck API
 https://developer.apple.com/documentation/devicecheck/accessing_and_modifying_per-device_data
 
 https://github.com/Kylmakalle/devicecheck
 """
-__version__ = "1.3.0"
+__version__ = "1.3.3"
 __author__ = 'Sergey Akentev (@Kylmakalle)'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024 Sergey Akentev'
 
 import logging
 import os
 import sys
 import typing
 import uuid
+import json
 from time import time
 
 import jwt
 import requests
 
 log = logging.getLogger('devicecheck')
 logging.basicConfig()
@@ -158,23 +159,22 @@
             "json_response": self.json_response,
             "bit_0": self.bit_0,
             "bit_1": self.bit_1,
             "bits_last_update_time": self.bits_last_update_time
         }
 
 
-def parse_apple_response(response: requests.Response, raise_on_error: bool):
-    response_text = response.text
+def parse_apple_response(response_text: str, response_status_code: int, raise_on_error: bool):
     if response_text:
         try:
-            response_json = response.json()
-            return DataAppleResponse(response.status_code, response_json, raise_on_error)
+            response_json = json.loads(response_text)
+            return DataAppleResponse(response_status_code, response_json, raise_on_error)
         except:
             pass
-    return HttpAppleResponse(response.status_code, response_text, raise_on_error)
+    return HttpAppleResponse(response_status_code, response_text, raise_on_error)
 
 
 class DeviceCheck:
     PRODUCTION_URL = "https://api.devicecheck.apple.com"
     DEVELOPMENT_URL = "https://api.development.devicecheck.apple.com"
 
     def __init__(self, team_id: str, bundle_id: str, key_id: str, private_key: [str, typing.IO],
@@ -267,15 +267,15 @@
         payload = {
             'timestamp': get_timestamp_milliseconds(),
             'transaction_id': get_transaction_id(),
             'device_token': token
         }
 
         result = self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
-        return parse_apple_response(result, self.raise_on_error)
+        return parse_apple_response(result.text, result.status_code, self.raise_on_error)
 
     def query_two_bits(self, token: str, *args, **kwargs) -> DataAppleResponse:
         """
         Query two bits of device data
         https://developer.apple.com/documentation/devicecheck/accessing_and_modifying_per-device_data#2910405
         :param token: Base 64–encoded representation of encrypted device information
         :param args: Additional args for requests module
@@ -285,15 +285,15 @@
         endpoint = 'v1/query_two_bits'
         payload = {
             'timestamp': get_timestamp_milliseconds(),
             'transaction_id': get_transaction_id(),
             'device_token': token
         }
         result = self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
-        return parse_apple_response(result, self.raise_on_error)
+        return parse_apple_response(result.text, result.status_code, self.raise_on_error)
 
     def update_two_bits(self, token: str, bit_0: [bool, int] = None, bit_1: [bool, int] = None, *args,
                         **kwargs) -> HttpAppleResponse:
         """
         Update bit(s) of a device data
         https://developer.apple.com/documentation/devicecheck/accessing_and_modifying_per-device_data#2910405
         :param token: Base 64–encoded representation of encrypted device information
@@ -313,15 +313,15 @@
         if bit_0 is not None:
             payload['bit0'] = bool(bit_0)
 
         if bit_1 is not None:
             payload['bit1'] = bool(bit_1)
 
         result = self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
-        return parse_apple_response(result, self.raise_on_error)
+        return parse_apple_response(result.text, result.status_code, self.raise_on_error)
 
     def get_request_url(self, is_dev_env: bool = None):
         """
         Set proper url for development or production.
         :param is_dev_env: Development environment flag
         :return:
         """
```

### Comparing `devicecheck-1.3.0/devicecheck/asyncio.py` & `devicecheck-1.3.3/devicecheck/asyncio.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         endpoint = 'v1/validate_device_token'
         payload = {
             'timestamp': get_timestamp_milliseconds(),
             'transaction_id': get_transaction_id(),
             'device_token': token
         }
 
-        result = await self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
-        return parse_apple_response(result, self.raise_on_error)
+        result_status_code, result_text = await self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
+        return parse_apple_response(result_text, result_status_code, self.raise_on_error)
 
     async def query_two_bits(self, token: str, *args, **kwargs) -> DataAppleResponse:
         """
         Query two bits of device data
         https://developer.apple.com/documentation/devicecheck/accessing_and_modifying_per-device_data#2910405
         :param token: Base 64–encoded representation of encrypted device information
         :param args: Additional args for requests module
@@ -44,16 +44,16 @@
         """
         endpoint = 'v1/query_two_bits'
         payload = {
             'timestamp': get_timestamp_milliseconds(),
             'transaction_id': get_transaction_id(),
             'device_token': token
         }
-        result = await self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
-        return parse_apple_response(result, self.raise_on_error)
+        result_status_code, result_text = await self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
+        return parse_apple_response(result_text, result_status_code, self.raise_on_error)
 
     async def update_two_bits(self, token: str, bit_0: [bool, int] = None, bit_1: [bool, int] = None, *args,
                         **kwargs) -> HttpAppleResponse:
         """
         Update bit(s) of a device data
         https://developer.apple.com/documentation/devicecheck/accessing_and_modifying_per-device_data#2910405
         :param token: Base 64–encoded representation of encrypted device information
@@ -72,16 +72,16 @@
 
         if bit_0 is not None:
             payload['bit0'] = bool(bit_0)
 
         if bit_1 is not None:
             payload['bit1'] = bool(bit_1)
 
-        result = await self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
-        return parse_apple_response(result, self.raise_on_error)
+        result_status_code, result_text = await self._request(self.get_request_url(), endpoint, payload, *args, **kwargs)
+        return parse_apple_response(result_text, result_status_code, self.raise_on_error)
 
     async def _request(self, url, endpoint, payload, retrying_env=False, *args, **kwargs):
         log.debug(f'Sending request to {url}/{endpoint} with data {payload}')
 
         async with self._session.post(f"{url}/{endpoint}", json=payload, headers={"authorization": f"Bearer {self.generate_token()}"}) as response:
             result_text = await response.text()
             log.debug(f"Response: {response.status} {result_text}")
```

### Comparing `devicecheck-1.3.0/devicecheck/decorators.py` & `devicecheck-1.3.3/devicecheck/decorators.py`

 * *Files identical despite different names*

### Comparing `devicecheck-1.3.0/devicecheck.egg-info/PKG-INFO` & `devicecheck-1.3.3/devicecheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicecheck
-Version: 1.3.0
+Version: 1.3.3
 Summary: Apple DeviceCheck API. Reduce fraudulent use of your services by managing device state and asserting app integrity.
 Home-page: https://github.com/Kylmakalle/devicecheck
 Author: Sergey Akentev
 Author-email: "S. Akentev" <sergey+gh@akentev.com>
 Project-URL: Issue Tracker, https://github.com/Kylmakalle/devicecheck/issues
 Project-URL: Repository, https://github.com/Kylmakalle/devicecheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `devicecheck-1.3.0/setup.py` & `devicecheck-1.3.3/setup.py`

 * *Files identical despite different names*

