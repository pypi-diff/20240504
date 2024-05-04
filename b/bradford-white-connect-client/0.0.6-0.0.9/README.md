# Comparing `tmp/bradford_white_connect_client-0.0.6.tar.gz` & `tmp/bradford_white_connect_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bradford_white_connect_client-0.0.6.tar", max compression
+gzip compressed data, was "bradford_white_connect_client-0.0.9.tar", max compression
```

## Comparing `bradford_white_connect_client-0.0.6.tar` & `bradford_white_connect_client-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-02-08 20:15:25.929529 bradford_white_connect_client-0.0.6/LICENSE
--rw-r--r--   0        0        0       74 2024-02-08 20:15:25.933529 bradford_white_connect_client-0.0.6/README.md
--rw-r--r--   0        0        0      208 2024-02-08 20:15:25.933529 bradford_white_connect_client-0.0.6/bradford_white_connect_client/__init__.py
--rw-r--r--   0        0        0     6637 2024-02-08 20:15:25.933529 bradford_white_connect_client-0.0.6/bradford_white_connect_client/client.py
--rw-r--r--   0        0        0      233 2024-02-08 20:15:25.933529 bradford_white_connect_client-0.0.6/bradford_white_connect_client/constants.py
--rw-r--r--   0        0        0      572 2024-02-08 20:15:25.933529 bradford_white_connect_client-0.0.6/bradford_white_connect_client/exceptions.py
--rw-r--r--   0        0        0     1522 2024-02-08 20:15:25.933529 bradford_white_connect_client-0.0.6/bradford_white_connect_client/types.py
--rw-r--r--   0        0        0     1521 2024-02-08 20:15:33.365482 bradford_white_connect_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 bradford_white_connect_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/LICENSE
+-rw-r--r--   0        0        0       74 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/README.md
+-rw-r--r--   0        0        0      208 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/bradford_white_connect_client/__init__.py
+-rw-r--r--   0        0        0     8981 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/bradford_white_connect_client/client.py
+-rw-r--r--   0        0        0      233 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/bradford_white_connect_client/constants.py
+-rw-r--r--   0        0        0      572 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/bradford_white_connect_client/exceptions.py
+-rw-r--r--   0        0        0     1522 2024-02-09 02:01:00.011963 bradford_white_connect_client-0.0.9/bradford_white_connect_client/types.py
+-rw-r--r--   0        0        0     1521 2024-02-09 02:01:07.792038 bradford_white_connect_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 bradford_white_connect_client-0.0.9/PKG-INFO
```

### Comparing `bradford_white_connect_client-0.0.6/LICENSE` & `bradford_white_connect_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bradford_white_connect_client-0.0.6/bradford_white_connect_client/client.py` & `bradford_white_connect_client-0.0.9/bradford_white_connect_client/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,46 +47,102 @@
     @retry(
         retry=retry_if_exception_type(BradfordWhiteConnectUnknownException),
         reraise=True,
         wait=wait_fixed(10),
         stop=stop_after_attempt(6),
         before_sleep=before_sleep_log(logger, logging.DEBUG),
     )
-    async def http_get_request(self, uri: str, headers: Dict[str, str]) -> str:
+    async def http_get_request(
+        self,
+        uri: str,
+        headers: Dict[str, str],
+        retrying_after_login: bool = False,
+    ) -> str:
         """
         Sends an HTTP GET request to the specified URI with the given headers.
 
         Args:
-            uri (str): The URI to send the request to.
+            uri (str): The URI to send the GET request to.
             headers (Dict[str, str]): The headers to include in the request.
+            retrying_after_login (bool, optional): Indicates whether the
+            request is being retried after logging in. Defaults to False.
 
         Returns:
-            str: The response text from the server.
+            str: The response body as a string.
 
         Raises:
-            HTTPError: If the response status code is not in the 200-299 range.
+            BradfordWhiteConnectUnknownException: If a 401 status code is
+            received after logging in. requests.exceptions.HTTPError: If a
+            non-2xx status code is received.
         """
         async with self.session.get(uri, headers=headers) as response:
+            # catch access denied errors and attempt to re-authenticate
+            if response.status == 401:
+                # if retrying after login, raise exception
+                if retrying_after_login:
+                    raise BradfordWhiteConnectUnknownException(
+                        "Received status code 401 after logging in"
+                    )
+
+                # update headers with new token
+                logger.debug("Token may be expired - retrying login")
+                await self.authenticate()
+                headers["authorization"] = f"auth_token {self.token}"
+
+                # retry the request
+                return await self.http_get_request(
+                    uri, headers, retrying_after_login=True
+                )
+
             response.raise_for_status()
             return await response.json()
 
-    async def http_post_request(self, uri, headers, data):
+    async def http_post_request(
+        self, uri, headers, data, retrying_after_login: bool = False
+    ):
         """
-        Sends an HTTP POST request.
+        Sends an HTTP POST request to the specified URI.
 
         Args:
             uri (str): The URI to send the request to.
             headers (dict): The headers to include in the request.
-            data (bytes): The data to include in the request body.
+            data (dict): The data to include in the request body.
+            retrying_after_login (bool, optional): Indicates whether
+            the request is being retried after logging in. Defaults to False.
 
         Returns:
-            The response object from the server.
+            dict: The JSON response from the server.
+
+        Raises:
+            BradfordWhiteConnectUnknownException: If a 401 status code is
+            received after logging in. requests.exceptions.HTTPError:
+            If a non-401 status code is received.
         """
+
         # trunk-ignore(flake8/E501)
         async with self.session.post(uri, headers=headers, data=data) as response:
+            # catch access denied errors and attempt to re-authenticate
+            if response.status == 401:
+                # if we're already retrying after logging in,
+                # raise an exception
+                if retrying_after_login:
+                    raise BradfordWhiteConnectUnknownException(
+                        "Received status code 401 after logging in"
+                    )
+
+                # update headers with new token
+                logger.debug("Token may be expired - retrying login")
+                await self.authenticate()
+                headers["authorization"] = f"auth_token {self.token}"
+
+                # retry the request
+                return await self.http_post_request(
+                    uri, headers, data, retrying_after_login=True
+                )
+
             response.raise_for_status()
             return await response.json()
 
     async def get_devices(self):
         headers = {
             "Host": "ads-field.aylanetworks.com",
             "accept": "*/*",
```

### Comparing `bradford_white_connect_client-0.0.6/bradford_white_connect_client/exceptions.py` & `bradford_white_connect_client-0.0.9/bradford_white_connect_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `bradford_white_connect_client-0.0.6/bradford_white_connect_client/types.py` & `bradford_white_connect_client-0.0.9/bradford_white_connect_client/types.py`

 * *Files identical despite different names*

### Comparing `bradford_white_connect_client-0.0.6/pyproject.toml` & `bradford_white_connect_client-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 multi_line_output = 3
 not_skip = "__init__.py"
 sections = "FUTURE,STDLIB,INBETWEENS,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 use_parentheses = true
 
 [tool.poetry]
 name = "bradford_white_connect_client"
-version = "0.0.6"
+version = "0.0.9"
 description = "A Python3, async-friendly client library for Bradford White Connect"
 readme = "README.md"
 authors = ["Andy Blyler <ablyler@blyler.cc>"]
 license = "MIT"
 repository = "https://github.com/ablyler/bradford_white_connect_client"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `bradford_white_connect_client-0.0.6/PKG-INFO` & `bradford_white_connect_client-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bradford_white_connect_client
-Version: 0.0.6
+Version: 0.0.9
 Summary: A Python3, async-friendly client library for Bradford White Connect
 Home-page: https://github.com/ablyler/bradford_white_connect_client
 License: MIT
 Author: Andy Blyler
 Author-email: ablyler@blyler.cc
 Requires-Python: >=3.11.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

