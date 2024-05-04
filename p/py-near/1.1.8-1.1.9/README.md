# Comparing `tmp/py_near-1.1.8.tar.gz` & `tmp/py_near-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_near-1.1.8.tar", max compression
+gzip compressed data, was "py_near-1.1.9.tar", max compression
```

## Comparing `py_near-1.1.8.tar` & `py_near-1.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1023 2022-06-08 20:31:53.650813 py_near-1.1.8/LICENSE
--rw-r--r--   0        0        0     3974 2023-01-24 19:13:04.795857 py_near-1.1.8/README.md
--rw-r--r--   0        0        0     1572 2023-10-08 09:55:32.631313 py_near-1.1.8/pyproject.toml
--rw-r--r--   0        0        0       50 2023-01-24 19:13:04.796695 py_near-1.1.8/src/py_near/__init__.py
--rw-r--r--   0        0        0    16767 2023-10-08 09:54:27.455641 py_near-1.1.8/src/py_near/account.py
--rw-r--r--   0        0        0      164 2023-05-05 18:03:26.714114 py_near-1.1.8/src/py_near/constants.py
--rw-r--r--   0        0        0        0 2023-01-24 19:13:04.797084 py_near-1.1.8/src/py_near/dapps/__init__.py
--rw-r--r--   0        0        0      231 2023-01-24 19:13:04.797225 py_near-1.1.8/src/py_near/dapps/core.py
--rw-r--r--   0        0        0       29 2023-01-24 19:13:04.797457 py_near-1.1.8/src/py_near/dapps/ft/__init__.py
--rw-r--r--   0        0        0     6717 2023-01-24 19:13:04.797637 py_near-1.1.8/src/py_near/dapps/ft/async_client.py
--rw-r--r--   0        0        0       92 2023-01-24 19:13:04.797752 py_near-1.1.8/src/py_near/dapps/ft/exceptions.py
--rw-r--r--   0        0        0      186 2023-01-24 19:13:04.797873 py_near-1.1.8/src/py_near/dapps/ft/models.py
--rw-r--r--   0        0        0      946 2023-10-02 06:10:34.045922 py_near-1.1.8/src/py_near/dapps/fts.py
--rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798157 py_near-1.1.8/src/py_near/dapps/keypom/__init__.py
--rw-r--r--   0        0        0     1422 2023-01-24 19:13:04.798347 py_near-1.1.8/src/py_near/dapps/keypom/async_client.py
--rw-r--r--   0        0        0       45 2023-01-24 19:13:04.798480 py_near-1.1.8/src/py_near/dapps/keypom/exceptions.py
--rw-r--r--   0        0        0     2166 2023-01-24 19:13:04.798618 py_near-1.1.8/src/py_near/dapps/keypom/models.py
--rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798770 py_near-1.1.8/src/py_near/dapps/phone/__init__.py
--rw-r--r--   0        0        0     6849 2023-01-24 19:13:04.799023 py_near-1.1.8/src/py_near/dapps/phone/async_client.py
--rw-r--r--   0        0        0       45 2023-01-24 19:13:04.799162 py_near-1.1.8/src/py_near/dapps/phone/exceptions.py
--rw-r--r--   0        0        0      332 2023-01-24 19:13:04.799299 py_near-1.1.8/src/py_near/dapps/phone/models.py
--rw-r--r--   0        0        0       34 2023-01-24 19:13:04.799462 py_near-1.1.8/src/py_near/dapps/staking/__init__.py
--rw-r--r--   0        0        0     5203 2023-01-24 19:13:04.799614 py_near-1.1.8/src/py_near/dapps/staking/async_client.py
--rw-r--r--   0        0        0       92 2023-01-24 19:13:04.799691 py_near-1.1.8/src/py_near/dapps/staking/exceptions.py
--rw-r--r--   0        0        0      124 2023-01-24 19:13:04.799806 py_near-1.1.8/src/py_near/dapps/staking/models.py
--rw-r--r--   0        0        0        0 2023-01-24 19:13:04.799907 py_near-1.1.8/src/py_near/exceptions/__init__.py
--rw-r--r--   0        0        0     5050 2023-07-10 17:19:22.765582 py_near-1.1.8/src/py_near/exceptions/exceptions.py
--rw-r--r--   0        0        0     7642 2023-06-23 01:16:29.606235 py_near-1.1.8/src/py_near/exceptions/provider.py
--rw-r--r--   0        0        0     9426 2023-06-30 22:36:51.489270 py_near-1.1.8/src/py_near/models.py
--rw-r--r--   0        0        0     8394 2023-09-09 08:58:18.064921 py_near-1.1.8/src/py_near/providers.py
--rw-r--r--   0        0        0     3186 2023-10-03 07:17:01.603289 py_near-1.1.8/src/py_near/transactions.py
--rw-r--r--   0        0        0      126 2023-06-26 04:51:57.591322 py_near-1.1.8/src/py_near/utils.py
--rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 py_near-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1023 2022-06-08 20:31:53.650813 py_near-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3974 2023-01-24 19:13:04.795857 py_near-1.1.9/README.md
+-rw-r--r--   0        0        0     1572 2023-10-11 15:04:24.571917 py_near-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-01-24 19:13:04.796695 py_near-1.1.9/src/py_near/__init__.py
+-rw-r--r--   0        0        0    16913 2023-10-11 15:03:20.062797 py_near-1.1.9/src/py_near/account.py
+-rw-r--r--   0        0        0      164 2023-05-05 18:03:26.714114 py_near-1.1.9/src/py_near/constants.py
+-rw-r--r--   0        0        0        0 2023-01-24 19:13:04.797084 py_near-1.1.9/src/py_near/dapps/__init__.py
+-rw-r--r--   0        0        0      231 2023-01-24 19:13:04.797225 py_near-1.1.9/src/py_near/dapps/core.py
+-rw-r--r--   0        0        0       29 2023-01-24 19:13:04.797457 py_near-1.1.9/src/py_near/dapps/ft/__init__.py
+-rw-r--r--   0        0        0     6717 2023-01-24 19:13:04.797637 py_near-1.1.9/src/py_near/dapps/ft/async_client.py
+-rw-r--r--   0        0        0       92 2023-01-24 19:13:04.797752 py_near-1.1.9/src/py_near/dapps/ft/exceptions.py
+-rw-r--r--   0        0        0      186 2023-01-24 19:13:04.797873 py_near-1.1.9/src/py_near/dapps/ft/models.py
+-rw-r--r--   0        0        0      946 2023-10-02 06:10:34.045922 py_near-1.1.9/src/py_near/dapps/fts.py
+-rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798157 py_near-1.1.9/src/py_near/dapps/keypom/__init__.py
+-rw-r--r--   0        0        0     1422 2023-01-24 19:13:04.798347 py_near-1.1.9/src/py_near/dapps/keypom/async_client.py
+-rw-r--r--   0        0        0       45 2023-01-24 19:13:04.798480 py_near-1.1.9/src/py_near/dapps/keypom/exceptions.py
+-rw-r--r--   0        0        0     2166 2023-01-24 19:13:04.798618 py_near-1.1.9/src/py_near/dapps/keypom/models.py
+-rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798770 py_near-1.1.9/src/py_near/dapps/phone/__init__.py
+-rw-r--r--   0        0        0     6849 2023-01-24 19:13:04.799023 py_near-1.1.9/src/py_near/dapps/phone/async_client.py
+-rw-r--r--   0        0        0       45 2023-01-24 19:13:04.799162 py_near-1.1.9/src/py_near/dapps/phone/exceptions.py
+-rw-r--r--   0        0        0      332 2023-01-24 19:13:04.799299 py_near-1.1.9/src/py_near/dapps/phone/models.py
+-rw-r--r--   0        0        0       34 2023-01-24 19:13:04.799462 py_near-1.1.9/src/py_near/dapps/staking/__init__.py
+-rw-r--r--   0        0        0     5203 2023-01-24 19:13:04.799614 py_near-1.1.9/src/py_near/dapps/staking/async_client.py
+-rw-r--r--   0        0        0       92 2023-01-24 19:13:04.799691 py_near-1.1.9/src/py_near/dapps/staking/exceptions.py
+-rw-r--r--   0        0        0      124 2023-01-24 19:13:04.799806 py_near-1.1.9/src/py_near/dapps/staking/models.py
+-rw-r--r--   0        0        0        0 2023-01-24 19:13:04.799907 py_near-1.1.9/src/py_near/exceptions/__init__.py
+-rw-r--r--   0        0        0     5050 2023-07-10 17:19:22.765582 py_near-1.1.9/src/py_near/exceptions/exceptions.py
+-rw-r--r--   0        0        0     7642 2023-06-23 01:16:29.606235 py_near-1.1.9/src/py_near/exceptions/provider.py
+-rw-r--r--   0        0        0     9426 2023-06-30 22:36:51.489270 py_near-1.1.9/src/py_near/models.py
+-rw-r--r--   0        0        0     8394 2023-09-09 08:58:18.064921 py_near-1.1.9/src/py_near/providers.py
+-rw-r--r--   0        0        0     3186 2023-10-03 07:17:01.603289 py_near-1.1.9/src/py_near/transactions.py
+-rw-r--r--   0        0        0      126 2023-06-26 04:51:57.591322 py_near-1.1.9/src/py_near/utils.py
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 py_near-1.1.9/PKG-INFO
```

### Comparing `py_near-1.1.8/LICENSE` & `py_near-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/README.md` & `py_near-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/pyproject.toml` & `py_near-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-near"
-version = "1.1.8"
+version = "1.1.9"
 description="Pretty simple and fully asynchronous framework for working with NEAR blockchain"
 authors = ["pvolnov <petr@herewallet.app>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ed25519 = "^1.5"
@@ -18,15 +18,15 @@
 flake8 = "^4.0.1"
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 base58 = "^2.1.1"
 
 [project]
 name = "py-near"
-version = "1.1.8"
+version = "1.1.9"
 description = "Pretty simple and fully asynchronous framework for working with NEAR blockchaink"
 authors = [ {name = "pvolnov", email = "petr@herewallet.app"} ]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies=["base58", "ed25519", "aiohttp", "py-near-primitives", "pydantic"]
 keywords = ["python", "near", "async"]
 classifiers = [
```

### Comparing `py_near-1.1.8/src/py_near/account.py` & `py_near-1.1.9/src/py_near/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import hashlib
 import json
 import logging
 from typing import List, Union, Dict, Optional
 
 import base58
 import ed25519
+from loguru import logger
 from py_near_primitives import DelegateAction
 
 from py_near import constants
 from py_near import transactions
 from py_near import utils
 from py_near.dapps.ft.async_client import FT
 from py_near.dapps.phone.async_client import Phone
@@ -148,14 +149,17 @@
             except RpcTimeoutError:
                 for _ in range(constants.TIMEOUT_WAIT_RPC // 3):
                     await asyncio.sleep(3)
                     try:
                         result = await self._provider.get_tx(trx_hash, receiver_id)
                     except InternalError:
                         continue
+                    except Exception as e:
+                        logger.exception(e)
+                        continue
                     if result:
                         return result
                 raise RpcTimeoutError("Transaction not found")
 
         except Exception as e:
             raise e
         finally:
```

### Comparing `py_near-1.1.8/src/py_near/dapps/ft/async_client.py` & `py_near-1.1.9/src/py_near/dapps/ft/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/dapps/fts.py` & `py_near-1.1.9/src/py_near/dapps/fts.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/dapps/keypom/async_client.py` & `py_near-1.1.9/src/py_near/dapps/keypom/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/dapps/keypom/models.py` & `py_near-1.1.9/src/py_near/dapps/keypom/models.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/dapps/phone/async_client.py` & `py_near-1.1.9/src/py_near/dapps/phone/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/dapps/staking/async_client.py` & `py_near-1.1.9/src/py_near/dapps/staking/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/exceptions/exceptions.py` & `py_near-1.1.9/src/py_near/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/exceptions/provider.py` & `py_near-1.1.9/src/py_near/exceptions/provider.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/models.py` & `py_near-1.1.9/src/py_near/models.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/providers.py` & `py_near-1.1.9/src/py_near/providers.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/src/py_near/transactions.py` & `py_near-1.1.9/src/py_near/transactions.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.8/PKG-INFO` & `py_near-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-near
-Version: 1.1.8
+Version: 1.1.9
 Summary: Pretty simple and fully asynchronous framework for working with NEAR blockchain
 Author: pvolnov
 Author-email: petr@herewallet.app
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

