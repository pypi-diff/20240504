# Comparing `tmp/pyauth0-0.1.1.tar.gz` & `tmp/pyauth0-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauth0-0.1.1.tar", last modified: Fri Oct 27 14:48:26 2023, max compression
+gzip compressed data, was "pyauth0-0.1.2.tar", last modified: Sat May  4 14:17:59 2024, max compression
```

## Comparing `pyauth0-0.1.1.tar` & `pyauth0-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 14:48:26.759339 pyauth0-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-27 14:48:11.000000 pyauth0-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-27 14:48:11.000000 pyauth0-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-10-27 14:48:26.755339 pyauth0-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-10-27 14:48:11.000000 pyauth0-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 14:48:26.755339 pyauth0-0.1.1/pyauth0/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-27 14:48:11.000000 pyauth0-0.1.1/pyauth0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-27 14:48:11.000000 pyauth0-0.1.1/pyauth0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-27 14:48:11.000000 pyauth0-0.1.1/pyauth0/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-10-27 14:48:11.000000 pyauth0-0.1.1/pyauth0/token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2023-10-27 14:48:11.000000 pyauth0-0.1.1/pyauth0/token_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 14:48:26.755339 pyauth0-0.1.1/pyauth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-10-27 14:48:26.000000 pyauth0-0.1.1/pyauth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-27 14:48:26.000000 pyauth0-0.1.1/pyauth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 14:48:26.000000 pyauth0-0.1.1/pyauth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-27 14:48:26.000000 pyauth0-0.1.1/pyauth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-27 14:48:26.000000 pyauth0-0.1.1/pyauth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-27 14:48:11.000000 pyauth0-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-27 14:48:11.000000 pyauth0-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 14:48:26.759339 pyauth0-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-10-27 14:48:11.000000 pyauth0-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 14:48:26.755339 pyauth0-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-27 14:48:11.000000 pyauth0-0.1.1/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-27 14:48:11.000000 pyauth0-0.1.1/test/test_pyauth0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-04 14:17:54.000000 pyauth0-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 14:17:54.000000 pyauth0-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-04 14:17:59.029268 pyauth0-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-04 14:17:54.000000 pyauth0-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/pyauth0/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyauth0/token_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/pyauth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 14:17:59.000000 pyauth0-0.1.2/pyauth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 14:17:54.000000 pyauth0-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 14:17:54.000000 pyauth0-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:17:59.033268 pyauth0-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-04 14:17:54.000000 pyauth0-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:17:59.029268 pyauth0-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 14:17:54.000000 pyauth0-0.1.2/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-04 14:17:54.000000 pyauth0-0.1.2/test/test_pyauth0.py
```

### Comparing `pyauth0-0.1.1/LICENSE` & `pyauth0-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.1/PKG-INFO` & `pyauth0-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauth0
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python utilities for Auth0
 Home-page: https://github.com/svaponi/pyauth0
 Author: svaponi
 Author-email: svaponi@proton.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,25 +13,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-jose>=3.3.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: python-dotenv; extra == "test"
 
+# pyauth0
+
 [![Test](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml/badge.svg)](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/svaponi/pyauth0/badge.svg?branch=main)](https://coveralls.io/github/svaponi/pyauth0?branch=main)
 [![PyPI version](https://badge.fury.io/py/pyauth0.svg)](https://badge.fury.io/py/pyauth0)
 
-# pyauth0
-
 Python utilities for [Auth0](https://auth0.com/).
 
+- [Install](#install)
+- [Usage](#usage)
+  - [Get a machine-to-machine token](#get-a-machine-to-machine-token)
+  - [Verify a token](#verify-a-token)
+- [Contribute](#contribute)
+
+## Install
+
+```shell
+pip install pyauth0
+```
+
 ## Usage
 
-Verify a token.
+### Get a machine-to-machine token
 
 ```python
 from pyauth0 import TokenProvider
 from urllib.request import Request, urlopen
 
 token_provider = TokenProvider(
     issuer="your-domain.auth0.com",
@@ -43,33 +55,33 @@
 # Machine to machine request
 response = urlopen(Request(
     "https://api.your-domain.com",
     headers={"authorization": token_provider.get_token().get_authorization()},
 ))
 ```
 
-Get a machine-to-machine token.
+### Verify a token
 
 ```python
 from pyauth0 import TokenVerifier, Auth0Error
 
 token_verifier = TokenVerifier(
     issuer="your-domain.auth0.com",
-    audience="https://your-domain.com/api",
+    audience="https://api.your-domain.com",
     jwks_cache_ttl=60,  # optional
 )
 try:
     decoded_token = token_verifier.verify(
         "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...."
     )
 except Auth0Error as error:
     status_code = error.status_code  # suggested status code (401 or 403)
     code = error.code  # pyauth0 error code (example "token_expired")
     description = error.description  # pyauth0 error description (example "Token is expired.")
     raise error
 
-claim_value = decoded_token.payload.get("http://your-tenant.com/claim_name", "default value")
+claim_value = decoded_token.payload.get("http://your-domain.com/claim_name", "default value")
 ```
 
 ## Contribute
 
 If you want to contribute, open a [GitHub Issue](https://github.com/svaponi/pyauth0/issues) and motivate your request.
```

### Comparing `pyauth0-0.1.1/README.md` & `pyauth0-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+# pyauth0
+
 [![Test](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml/badge.svg)](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/svaponi/pyauth0/badge.svg?branch=main)](https://coveralls.io/github/svaponi/pyauth0?branch=main)
 [![PyPI version](https://badge.fury.io/py/pyauth0.svg)](https://badge.fury.io/py/pyauth0)
 
-# pyauth0
-
 Python utilities for [Auth0](https://auth0.com/).
 
+- [Install](#install)
+- [Usage](#usage)
+  - [Get a machine-to-machine token](#get-a-machine-to-machine-token)
+  - [Verify a token](#verify-a-token)
+- [Contribute](#contribute)
+
+## Install
+
+```shell
+pip install pyauth0
+```
+
 ## Usage
 
-Verify a token.
+### Get a machine-to-machine token
 
 ```python
 from pyauth0 import TokenProvider
 from urllib.request import Request, urlopen
 
 token_provider = TokenProvider(
     issuer="your-domain.auth0.com",
@@ -24,33 +36,33 @@
 # Machine to machine request
 response = urlopen(Request(
     "https://api.your-domain.com",
     headers={"authorization": token_provider.get_token().get_authorization()},
 ))
 ```
 
-Get a machine-to-machine token.
+### Verify a token
 
 ```python
 from pyauth0 import TokenVerifier, Auth0Error
 
 token_verifier = TokenVerifier(
     issuer="your-domain.auth0.com",
-    audience="https://your-domain.com/api",
+    audience="https://api.your-domain.com",
     jwks_cache_ttl=60,  # optional
 )
 try:
     decoded_token = token_verifier.verify(
         "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...."
     )
 except Auth0Error as error:
     status_code = error.status_code  # suggested status code (401 or 403)
     code = error.code  # pyauth0 error code (example "token_expired")
     description = error.description  # pyauth0 error description (example "Token is expired.")
     raise error
 
-claim_value = decoded_token.payload.get("http://your-tenant.com/claim_name", "default value")
+claim_value = decoded_token.payload.get("http://your-domain.com/claim_name", "default value")
 ```
 
 ## Contribute
 
 If you want to contribute, open a [GitHub Issue](https://github.com/svaponi/pyauth0/issues) and motivate your request.
```

### Comparing `pyauth0-0.1.1/pyauth0/token_provider.py` & `pyauth0-0.1.2/pyauth0/token_provider.py`

 * *Files identical despite different names*

### Comparing `pyauth0-0.1.1/pyauth0/token_verifier.py` & `pyauth0-0.1.2/pyauth0/token_verifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,18 +108,18 @@
         if not token:
             raise Auth0Error(
                 status_code=401, code="invalid_token", description="Token is missing."
             )
 
         try:
             header = jwt.get_unverified_headers(token)
-        except jwt.JWSError as error:
+        except Exception as error:
             raise Auth0Error(
                 status_code=401,
-                code="malformed_token",
+                code="invalid_token",
                 description="Malformed token.",
             ) from error
 
         if header["alg"] == "HS256":
             raise Auth0Error(
                 status_code=401,
                 code="invalid_token",
```

### Comparing `pyauth0-0.1.1/pyauth0.egg-info/PKG-INFO` & `pyauth0-0.1.2/pyauth0.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauth0
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python utilities for Auth0
 Home-page: https://github.com/svaponi/pyauth0
 Author: svaponi
 Author-email: svaponi@proton.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,25 +13,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-jose>=3.3.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: python-dotenv; extra == "test"
 
+# pyauth0
+
 [![Test](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml/badge.svg)](https://github.com/svaponi/pyauth0/actions/workflows/run-tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/svaponi/pyauth0/badge.svg?branch=main)](https://coveralls.io/github/svaponi/pyauth0?branch=main)
 [![PyPI version](https://badge.fury.io/py/pyauth0.svg)](https://badge.fury.io/py/pyauth0)
 
-# pyauth0
-
 Python utilities for [Auth0](https://auth0.com/).
 
+- [Install](#install)
+- [Usage](#usage)
+  - [Get a machine-to-machine token](#get-a-machine-to-machine-token)
+  - [Verify a token](#verify-a-token)
+- [Contribute](#contribute)
+
+## Install
+
+```shell
+pip install pyauth0
+```
+
 ## Usage
 
-Verify a token.
+### Get a machine-to-machine token
 
 ```python
 from pyauth0 import TokenProvider
 from urllib.request import Request, urlopen
 
 token_provider = TokenProvider(
     issuer="your-domain.auth0.com",
@@ -43,33 +55,33 @@
 # Machine to machine request
 response = urlopen(Request(
     "https://api.your-domain.com",
     headers={"authorization": token_provider.get_token().get_authorization()},
 ))
 ```
 
-Get a machine-to-machine token.
+### Verify a token
 
 ```python
 from pyauth0 import TokenVerifier, Auth0Error
 
 token_verifier = TokenVerifier(
     issuer="your-domain.auth0.com",
-    audience="https://your-domain.com/api",
+    audience="https://api.your-domain.com",
     jwks_cache_ttl=60,  # optional
 )
 try:
     decoded_token = token_verifier.verify(
         "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...."
     )
 except Auth0Error as error:
     status_code = error.status_code  # suggested status code (401 or 403)
     code = error.code  # pyauth0 error code (example "token_expired")
     description = error.description  # pyauth0 error description (example "Token is expired.")
     raise error
 
-claim_value = decoded_token.payload.get("http://your-tenant.com/claim_name", "default value")
+claim_value = decoded_token.payload.get("http://your-domain.com/claim_name", "default value")
 ```
 
 ## Contribute
 
 If you want to contribute, open a [GitHub Issue](https://github.com/svaponi/pyauth0/issues) and motivate your request.
```

### Comparing `pyauth0-0.1.1/setup.py` & `pyauth0-0.1.2/setup.py`

 * *Files identical despite different names*

