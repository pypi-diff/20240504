# Comparing `tmp/upowpy-1.0.5.tar.gz` & `tmp/upowpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upowpy-1.0.5.tar", last modified: Fri May  3 09:20:37 2024, max compression
+gzip compressed data, was "upowpy-1.0.6.tar", last modified: Sat May  4 06:13:57 2024, max compression
```

## Comparing `upowpy-1.0.5.tar` & `upowpy-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 09:20:37.938009 upowpy-1.0.5/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     7888 2024-05-03 09:20:37.937764 upowpy-1.0.5/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     7062 2024-05-03 09:17:36.000000 upowpy-1.0.5/README.md
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-03 09:20:37.938062 upowpy-1.0.5/setup.cfg
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      986 2024-05-03 09:19:56.000000 upowpy-1.0.5/setup.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 09:20:37.933632 upowpy-1.0.5/upowpy/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      510 2024-05-03 05:19:02.000000 upowpy-1.0.5/upowpy/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     4876 2024-05-03 09:15:19.000000 upowpy-1.0.5/upowpy/push.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 09:20:37.936240 upowpy-1.0.5/upowpy/upow_transactions/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowpy-1.0.5/upowpy/upow_transactions/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1441 2024-05-01 07:35:56.000000 upowpy-1.0.5/upowpy/upow_transactions/coinbase_transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowpy-1.0.5/upowpy/upow_transactions/constants.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowpy-1.0.5/upowpy/upow_transactions/helpers.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     8573 2024-05-01 07:36:55.000000 upowpy-1.0.5/upowpy/upow_transactions/transaction.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     4945 2024-05-01 07:36:18.000000 upowpy-1.0.5/upowpy/upow_transactions/transaction_input.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     1522 2024-05-01 07:36:30.000000 upowpy-1.0.5/upowpy/upow_transactions/transaction_output.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 09:20:37.937068 upowpy-1.0.5/upowpy/utils/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)       46 2024-05-03 09:14:11.000000 upowpy-1.0.5/upowpy/utils/__init__.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    17563 2024-05-01 07:48:39.000000 upowpy-1.0.5/upowpy/utils/repository.py
--rw-r--r--   0 georgeprethesh   (501) staff       (20)    22811 2024-05-03 09:14:48.000000 upowpy-1.0.5/upowpy/utils/utils.py
-drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-03 09:20:37.937484 upowpy-1.0.5/upowpy.egg-info/
--rw-r--r--   0 georgeprethesh   (501) staff       (20)     7888 2024-05-03 09:20:37.000000 upowpy-1.0.5/upowpy.egg-info/PKG-INFO
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      568 2024-05-03 09:20:37.000000 upowpy-1.0.5/upowpy.egg-info/SOURCES.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-03 09:20:37.000000 upowpy-1.0.5/upowpy.egg-info/dependency_links.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-03 09:20:37.000000 upowpy-1.0.5/upowpy.egg-info/requires.txt
--rw-r--r--   0 georgeprethesh   (501) staff       (20)        7 2024-05-03 09:20:37.000000 upowpy-1.0.5/upowpy.egg-info/top_level.txt
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-04 06:13:57.674123 upowpy-1.0.6/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     8551 2024-05-04 06:13:57.673859 upowpy-1.0.6/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     7725 2024-05-04 06:11:47.000000 upowpy-1.0.6/README.md
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       38 2024-05-04 06:13:57.674178 upowpy-1.0.6/setup.cfg
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      986 2024-05-04 06:12:54.000000 upowpy-1.0.6/setup.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-04 06:13:57.667644 upowpy-1.0.6/upowpy/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      510 2024-05-03 05:19:02.000000 upowpy-1.0.6/upowpy/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     6034 2024-05-04 06:12:22.000000 upowpy-1.0.6/upowpy/push.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-04 06:13:57.671096 upowpy-1.0.6/upowpy/upow_transactions/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        0 2024-05-01 06:21:00.000000 upowpy-1.0.6/upowpy/upow_transactions/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1441 2024-05-01 07:35:56.000000 upowpy-1.0.6/upowpy/upow_transactions/coinbase_transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      211 2024-03-01 05:05:06.000000 upowpy-1.0.6/upowpy/upow_transactions/constants.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     5524 2024-03-10 06:13:43.000000 upowpy-1.0.6/upowpy/upow_transactions/helpers.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     8573 2024-05-01 07:36:55.000000 upowpy-1.0.6/upowpy/upow_transactions/transaction.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     4945 2024-05-01 07:36:18.000000 upowpy-1.0.6/upowpy/upow_transactions/transaction_input.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     1522 2024-05-01 07:36:30.000000 upowpy-1.0.6/upowpy/upow_transactions/transaction_output.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-04 06:13:57.672669 upowpy-1.0.6/upowpy/utils/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)       46 2024-05-03 09:14:11.000000 upowpy-1.0.6/upowpy/utils/__init__.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    17824 2024-05-04 05:47:05.000000 upowpy-1.0.6/upowpy/utils/repository.py
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)    22916 2024-05-04 06:05:08.000000 upowpy-1.0.6/upowpy/utils/utils.py
+drwxr-xr-x   0 georgeprethesh   (501) staff       (20)        0 2024-05-04 06:13:57.673564 upowpy-1.0.6/upowpy.egg-info/
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)     8551 2024-05-04 06:13:57.000000 upowpy-1.0.6/upowpy.egg-info/PKG-INFO
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      568 2024-05-04 06:13:57.000000 upowpy-1.0.6/upowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        1 2024-05-04 06:13:57.000000 upowpy-1.0.6/upowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)      233 2024-05-04 06:13:57.000000 upowpy-1.0.6/upowpy.egg-info/requires.txt
+-rw-r--r--   0 georgeprethesh   (501) staff       (20)        7 2024-05-04 06:13:57.000000 upowpy-1.0.6/upowpy.egg-info/top_level.txt
```

### Comparing `upowpy-1.0.5/PKG-INFO` & `upowpy-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upowpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain
 Home-page: https://github.com/upowai/upowpy
 Author: upow
 Author-email: contact@upow.ai
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: asttokens==2.4.1
@@ -54,14 +54,16 @@
 
 KEY = "hexKey"
 TO = "wallet_address"
 VOTE_TO = "wallet_address"
 REVOKE_FROM = "wallet_address"
 AMOUNT = "1"
 VOTING_RANGE = "10"
+WALLET = "wallet_address"
+HASH = "tx_hash"
 
 async def send_transaction():
     try:
         transaction_hash = await upow.send_transaction(utils_instance, KEY, TO, AMOUNT)
         print("Transaction hash:", transaction_hash)
     except Exception as e:
         print("Failed to send transaction:", str(e))
@@ -117,14 +119,34 @@
     print("Transaction hash:", transaction_hash)
 
 async def revoke_transaction():
     transaction_hash = await upow.revoke_transaction(utils_instance, KEY, REVOKE_FROM)
     print("Transaction hash:", transaction_hash)
 ```
 
+#### find_balance and find_tx
+
+Find balance using wallet_address and find tx info using tx_hash.
+
+```python
+async def find_balance(WALLET):
+    try:
+        transaction_hash = await upow.get_balance(utils_instance, WALLET)
+        print("Balance:", transaction_hash)
+    except Exception as e:
+        print("Failed to find_balance:", str(e))
+
+async def find_tx(HASH):
+    try:
+        transaction_hash = await upow.find_tx(utils_instance, HASH)
+        print("tx:", transaction_hash)
+    except Exception as e:
+        print("Failed to find tx:", str(e))
+```
+
 ### Running the Code
 
 You can run the asynchronous functions using the asyncio library.
 
 ```python
 import asyncio
 
@@ -134,14 +156,16 @@
     # await stake_transaction()
     # await unstake_transaction()
     # await register_inode_transaction()
     # await deregister_inode_transaction()
     # await register_validator_transaction()
     # await vote_transaction()
     # await revoke_transaction()
+    # await find_balance(WALLET)
+    # await find_tx(HASH)
 
 asyncio.run(main())
 ```
 
 ## Error Handling
 
 The `upowpy` library can raise several exceptions during its operation. Below is a list of the most common exceptions you might encounter, along with their descriptions and suggested actions to take if you encounter them:
```

### Comparing `upowpy-1.0.5/README.md` & `upowpy-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
 KEY = "hexKey"
 TO = "wallet_address"
 VOTE_TO = "wallet_address"
 REVOKE_FROM = "wallet_address"
 AMOUNT = "1"
 VOTING_RANGE = "10"
+WALLET = "wallet_address"
+HASH = "tx_hash"
 
 async def send_transaction():
     try:
         transaction_hash = await upow.send_transaction(utils_instance, KEY, TO, AMOUNT)
         print("Transaction hash:", transaction_hash)
     except Exception as e:
         print("Failed to send transaction:", str(e))
@@ -93,14 +95,34 @@
     print("Transaction hash:", transaction_hash)
 
 async def revoke_transaction():
     transaction_hash = await upow.revoke_transaction(utils_instance, KEY, REVOKE_FROM)
     print("Transaction hash:", transaction_hash)
 ```
 
+#### find_balance and find_tx
+
+Find balance using wallet_address and find tx info using tx_hash.
+
+```python
+async def find_balance(WALLET):
+    try:
+        transaction_hash = await upow.get_balance(utils_instance, WALLET)
+        print("Balance:", transaction_hash)
+    except Exception as e:
+        print("Failed to find_balance:", str(e))
+
+async def find_tx(HASH):
+    try:
+        transaction_hash = await upow.find_tx(utils_instance, HASH)
+        print("tx:", transaction_hash)
+    except Exception as e:
+        print("Failed to find tx:", str(e))
+```
+
 ### Running the Code
 
 You can run the asynchronous functions using the asyncio library.
 
 ```python
 import asyncio
 
@@ -110,14 +132,16 @@
     # await stake_transaction()
     # await unstake_transaction()
     # await register_inode_transaction()
     # await deregister_inode_transaction()
     # await register_validator_transaction()
     # await vote_transaction()
     # await revoke_transaction()
+    # await find_balance(WALLET)
+    # await find_tx(HASH)
 
 asyncio.run(main())
 ```
 
 ## Error Handling
 
 The `upowpy` library can raise several exceptions during its operation. Below is a list of the most common exceptions you might encounter, along with their descriptions and suggested actions to take if you encounter them:
```

### Comparing `upowpy-1.0.5/setup.py` & `upowpy-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="upowpy",
-    version="1.0.5",
+    version="1.0.6",
     author="upow",
     author_email="contact@upow.ai",
     description="upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/upowai/upowpy",
     packages=find_packages(),
```

### Comparing `upowpy-1.0.5/upowpy/push.py` & `upowpy-1.0.6/upowpy/push.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import requests
 from .upow_transactions.helpers import sha256, string_to_bytes
 from .utils.utils import Utils
+import decimal
 
 wallet_utils: Utils = Utils()
 
 
 async def push_tx(tx, wallet_utils: Utils):
     try:
         r = requests.get(
@@ -147,7 +148,42 @@
         if transaction_hash:
             return transaction_hash
         else:
             raise Exception(error_message)
     except Exception as e:
 
         raise
+
+
+async def get_balance(wallet_utils, address: str):
+    try:
+        balance_info = wallet_utils.get_balance_info(address)
+        formatted_total_balance = f"Total Balance: {balance_info[0]}"
+        formatted_stake_balance = f"Staked Balance: {balance_info[2]}"
+
+        balance_details = [formatted_total_balance, formatted_stake_balance]
+
+        if balance_info[1] != decimal.Decimal("0"):
+            formatted_pending_balance = f"Pending Incoming Balance: {balance_info[1]}"
+            balance_details.append(formatted_pending_balance)
+
+        if balance_info[3] != decimal.Decimal("0"):
+            formatted_pending_stake_balance = (
+                f"Pending Staked Balance: {balance_info[3]}"
+            )
+            balance_details.append(formatted_pending_stake_balance)
+
+        if balance_info[4]:
+            balance_details.append("Balance is syncing...")
+
+        return "\n".join(balance_details)
+
+    except Exception as e:
+        raise
+
+
+async def find_tx(wallet_utils: Utils, hash: str):
+    try:
+        balance_info = wallet_utils.get_tx(hash)
+        return balance_info
+    except Exception as e:
+        raise
```

### Comparing `upowpy-1.0.5/upowpy/upow_transactions/coinbase_transaction.py` & `upowpy-1.0.6/upowpy/upow_transactions/coinbase_transaction.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.5/upowpy/upow_transactions/helpers.py` & `upowpy-1.0.6/upowpy/upow_transactions/helpers.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.5/upowpy/upow_transactions/transaction.py` & `upowpy-1.0.6/upowpy/upow_transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.5/upowpy/upow_transactions/transaction_input.py` & `upowpy-1.0.6/upowpy/upow_transactions/transaction_input.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.5/upowpy/upow_transactions/transaction_output.py` & `upowpy-1.0.6/upowpy/upow_transactions/transaction_output.py`

 * *Files identical despite different names*

### Comparing `upowpy-1.0.5/upowpy/utils/repository.py` & `upowpy-1.0.6/upowpy/utils/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 
     def get_dobby_info(self):
         request = requests.get(f"{self.node_url}/dobby_info")
         request.raise_for_status()
         result = request.json()["result"]
         return result
 
+    def get_transaction(self, tx_hash: str):
+        url = f"{self.node_url}/get_transaction?tx_hash={tx_hash}&verify=false"
+        request = requests.get(url)
+        request.raise_for_status()
+        result = request.json()["result"]
+        return result
+
     def get_validators_info(self, inode: str = None):
         params = {"inode": inode} if inode else {}
         request = requests.get(f"{self.node_url}/get_validators_info", params)
         request.raise_for_status()
         result = request.json()
         return result
```

### Comparing `upowpy-1.0.5/upowpy/utils/utils.py` & `upowpy-1.0.6/upowpy/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
             self.NODE_URL = new_url
             self.repo = WalletRepository(self.NODE_URL)
 
     def get_balance_info(self, address: str):
         result = self.repo.get_balance_info(address)
         return result
 
+    def get_tx(self, hash: str):
+        result = self.repo.get_transaction(hash)
+        return result
+
     async def create_transaction(
         self,
         private_key,
         receiving_address,
         amount,
         message: bytes = None,
         send_back_address=None,
```

### Comparing `upowpy-1.0.5/upowpy.egg-info/PKG-INFO` & `upowpy-1.0.6/upowpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upowpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: upowpy is a Python library for interacting with uPow blockchain transactions, including sending funds, staking, voting, and managing nodes and validators on the blockchain
 Home-page: https://github.com/upowai/upowpy
 Author: upow
 Author-email: contact@upow.ai
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: asttokens==2.4.1
@@ -54,14 +54,16 @@
 
 KEY = "hexKey"
 TO = "wallet_address"
 VOTE_TO = "wallet_address"
 REVOKE_FROM = "wallet_address"
 AMOUNT = "1"
 VOTING_RANGE = "10"
+WALLET = "wallet_address"
+HASH = "tx_hash"
 
 async def send_transaction():
     try:
         transaction_hash = await upow.send_transaction(utils_instance, KEY, TO, AMOUNT)
         print("Transaction hash:", transaction_hash)
     except Exception as e:
         print("Failed to send transaction:", str(e))
@@ -117,14 +119,34 @@
     print("Transaction hash:", transaction_hash)
 
 async def revoke_transaction():
     transaction_hash = await upow.revoke_transaction(utils_instance, KEY, REVOKE_FROM)
     print("Transaction hash:", transaction_hash)
 ```
 
+#### find_balance and find_tx
+
+Find balance using wallet_address and find tx info using tx_hash.
+
+```python
+async def find_balance(WALLET):
+    try:
+        transaction_hash = await upow.get_balance(utils_instance, WALLET)
+        print("Balance:", transaction_hash)
+    except Exception as e:
+        print("Failed to find_balance:", str(e))
+
+async def find_tx(HASH):
+    try:
+        transaction_hash = await upow.find_tx(utils_instance, HASH)
+        print("tx:", transaction_hash)
+    except Exception as e:
+        print("Failed to find tx:", str(e))
+```
+
 ### Running the Code
 
 You can run the asynchronous functions using the asyncio library.
 
 ```python
 import asyncio
 
@@ -134,14 +156,16 @@
     # await stake_transaction()
     # await unstake_transaction()
     # await register_inode_transaction()
     # await deregister_inode_transaction()
     # await register_validator_transaction()
     # await vote_transaction()
     # await revoke_transaction()
+    # await find_balance(WALLET)
+    # await find_tx(HASH)
 
 asyncio.run(main())
 ```
 
 ## Error Handling
 
 The `upowpy` library can raise several exceptions during its operation. Below is a list of the most common exceptions you might encounter, along with their descriptions and suggested actions to take if you encounter them:
```

### Comparing `upowpy-1.0.5/upowpy.egg-info/SOURCES.txt` & `upowpy-1.0.6/upowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

