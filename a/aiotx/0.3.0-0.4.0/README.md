# Comparing `tmp/aiotx-0.3.0.tar.gz` & `tmp/aiotx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.3.0.tar", last modified: Fri May  3 09:31:28 2024, max compression
+gzip compressed data, was "aiotx-0.4.0.tar", last modified: Fri May  3 11:02:04 2024, max compression
```

## Comparing `aiotx-0.3.0.tar` & `aiotx-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.360614 aiotx-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 09:31:20.000000 aiotx-0.3.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 09:31:20.000000 aiotx-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 09:31:20.000000 aiotx-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 09:31:20.000000 aiotx-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-03 09:31:20.000000 aiotx-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 09:31:28.360614 aiotx-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-03 09:31:20.000000 aiotx-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/_bitcoin_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 09:31:20.000000 aiotx-0.3.0/aiotx/utils/bep20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.360614 aiotx-0.3.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 09:31:28.000000 aiotx-0.3.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 09:31:20.000000 aiotx-0.3.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 09:31:20.000000 aiotx-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 09:31:20.000000 aiotx-0.3.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-03 09:31:20.000000 aiotx-0.3.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 09:31:28.360614 aiotx-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 09:31:20.000000 aiotx-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/confest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.352614 aiotx-0.3.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:31:28.356614 aiotx-0.3.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 09:31:20.000000 aiotx-0.3.0/tests/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.683173 aiotx-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.671173 aiotx-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 11:01:57.000000 aiotx-0.4.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 11:01:57.000000 aiotx-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 11:01:57.000000 aiotx-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 11:01:57.000000 aiotx-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-03 11:01:57.000000 aiotx-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-03 11:02:04.683173 aiotx-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-03 11:01:57.000000 aiotx-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/utils/bep20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 11:01:57.000000 aiotx-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 11:01:57.000000 aiotx-0.4.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-03 11:01:57.000000 aiotx-0.4.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 11:02:04.683173 aiotx-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 11:01:57.000000 aiotx-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/confest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.671173 aiotx-0.4.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/test_bsc_monitoring.py
```

### Comparing `aiotx-0.3.0/.github/workflows/lint-check.yml` & `aiotx-0.4.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/.github/workflows/python-publish.yml` & `aiotx-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/.github/workflows/test.yml` & `aiotx-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/.gitignore` & `aiotx-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/CHANGELOG.md` & `aiotx-0.4.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.4.0]
+- Added tests for send and send_token function, they was renamed and changed, getting pending for nonce now
+
 ## [0.3.0]
 - Function for getting current gas price is added and to_wai/from_wai functions are attached to EVM client now
 
 ## [0.2.0]
 - block/transactions monitoring added, examples of usage added, tx input decoding added
 
 ## [0.1.0]
```

### Comparing `aiotx-0.3.0/PKG-INFO` & `aiotx-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.3.0
+Version: 0.4.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -53,26 +53,30 @@
 
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
 from aiotx import AioTxBSCClient
 
+bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
+
 async def main():
-    bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
-    
     # Create a new wallet
-    address, private_key = await bsc_client.generate_address()
+    address, private_key = bsc_client.generate_address()
     
     # Retrieve the wallet balance
     balance = await bsc_client.get_balance(address)
     print(f"Wallet balance: {balance}")
 
-    # Send transaction
-    tx_id = await bsc_client.send_transaction(private_key, to_address, amount, gas_price, gas_limit)
+    # Send BNB
+    tx_id = await bsc_client.send(private_key, to_address, amount)
+    print(f"Your tx: {tx_id}")
+
+    # Send any token
+    tx_id = await bsc_client.send_token(private_key, to_address, contract_address, amount)
     print(f"Your tx: {tx_id}")
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
```

### Comparing `aiotx-0.3.0/README.md` & `aiotx-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,26 +17,30 @@
 
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
 from aiotx import AioTxBSCClient
 
+bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
+
 async def main():
-    bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
-    
     # Create a new wallet
-    address, private_key = await bsc_client.generate_address()
+    address, private_key = bsc_client.generate_address()
     
     # Retrieve the wallet balance
     balance = await bsc_client.get_balance(address)
     print(f"Wallet balance: {balance}")
 
-    # Send transaction
-    tx_id = await bsc_client.send_transaction(private_key, to_address, amount, gas_price, gas_limit)
+    # Send BNB
+    tx_id = await bsc_client.send(private_key, to_address, amount)
+    print(f"Your tx: {tx_id}")
+
+    # Send any token
+    tx_id = await bsc_client.send_token(private_key, to_address, contract_address, amount)
     print(f"Your tx: {tx_id}")
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
```

### Comparing `aiotx-0.3.0/aiotx/clients/_base_client.py` & `aiotx-0.4.0/aiotx/clients/_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import concurrent.futures
 
 
 class AioTxClient:
     def __init__(self, node_url):
         self.node_url = node_url
         self.monitor = BlockMonitor(self)
         self._monitoring_task = None
@@ -28,15 +27,15 @@
                 await self.monitor.start(monitoring_start_block)
         except asyncio.CancelledError:
             pass
 
     async def get_block_by_number(self, block_number: int):
         pass
 
-    async def get_last_block(self) -> int:
+    async def get_last_block_number(self) -> int:
         pass
 
 class BlockMonitor:   
     def __init__(self, client: AioTxClient):
         self.client = client
         self.block_handlers = []
         self.transaction_handlers = []
```

### Comparing `aiotx-0.3.0/aiotx/clients/_evm_base_client.py` & `aiotx-0.4.0/aiotx/clients/_evm_base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
+import binascii
 import decimal
 import json
 import secrets
 from typing import Union
 
 import aiohttp
 from eth_abi import decode, encode
 from eth_account import Account
-from eth_typing import HexStr
 from eth_utils import (
     currency,
     decode_hex,
     function_signature_to_4byte_selector,
     keccak,
     to_checksum_address,
     to_hex,
@@ -33,14 +33,15 @@
     NonceTooLowError,
     ReplacementTransactionUnderpriced,
     StackLimitReachedError,
     TraceRequestLimitExceededError,
     TransactionCostExceedsGasLimitError,
     TransactionNotFound,
     VMExecutionError,
+    WrongPrivateKey,
 )
 from aiotx.types import BlockParam
 
 
 class AioTxEVMClient(AioTxClient):
     def __init__(self, node_url, chain_id):
         self.node_url = node_url
@@ -53,54 +54,29 @@
 
     def generate_address(self):
         private_key_bytes = secrets.token_hex(32)
         private_key = "0x" + private_key_bytes
         acct = Account.from_key(private_key)
         return private_key, acct.address
     
+    def get_address_from_private_key(self, private_key: str):
+        try:
+            from_address = Account.from_key(private_key).address
+        except binascii.Error as e:
+            raise WrongPrivateKey(e)
+        return to_checksum_address(from_address)
+    
     @staticmethod
     def from_wei(number: int, unit: str) -> Union[int, decimal.Decimal]:
         return currency.from_wei(number, unit)
     
     @staticmethod
     def to_wei(number: Union[int, float, str, decimal.Decimal], unit: str) -> int:
         return currency.to_wei(number, unit)
 
-    def get_address_from_private_key(self, private_key: str):
-        sender_address = Account.from_key(private_key).address
-        return to_checksum_address(sender_address)
-
-    async def get_last_block(self) -> int:
-        payload = {"method": "eth_blockNumber", "params": []}
-        result = await self._make_rpc_call(payload)
-        last_block = result["result"]
-        return int(last_block, 16)
-
-    async def get_balance(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
-        payload = {"method": "eth_getBalance", "params": [address, block_parameter.value]}
-
-        result = await self._make_rpc_call(payload)
-        balance = result["result"]
-        return 0 if balance == "0x" else int(result["result"], 16)
-    
-    async def get_gas_price(self) -> int:
-        payload = {"method": "eth_gasPrice", "params": []}
-        result = await self._make_rpc_call(payload)
-        price = result["result"]
-        return 0 if price == "0x" else int(result["result"], 16)
-        
-    async def get_transaction(self, hash) -> dict:
-        payload = {"method": "eth_getTransactionByHash", "params": [hash]}
-        result = await self._make_rpc_call(payload)
-        if result["result"] is None:
-            raise TransactionNotFound(f"Transaction {hash} not found!")
-        tx_data = result["result"]
-        tx_data["aiotx_decoded_input"] = self.decode_transaction_input(tx_data["input"])
-        return tx_data
-    
     def decode_transaction_input(self, input_data: str) -> dict:
         if input_data == "0x":
             return {
             'function_name': None,
             'parameters': None
         }
         for abi_entry in self._bep20_abi:
@@ -122,92 +98,115 @@
                     'parameters': decoded_params
                 }
 
         return {
             'function_name': None,
             'parameters': None
         }
-        
+
+    async def get_last_block_number(self) -> int:
+        payload = {"method": "eth_blockNumber", "params": []}
+        result = await self._make_rpc_call(payload)
+        last_block = result["result"]
+        return int(last_block, 16)
+    
     async def get_block_by_number(self, block_number: int, transaction_detail_flag: bool = True):
         payload = {"method": "eth_getBlockByNumber", "params": [hex(block_number), transaction_detail_flag]}
         result = await self._make_rpc_call(payload)
         return result
 
-    async def get_token_balance(self, address, contract_address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
+    async def get_balance(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
+        payload = {"method": "eth_getBalance", "params": [address, block_parameter.value]}
+
+        result = await self._make_rpc_call(payload)
+        balance = result["result"]
+        return 0 if balance == "0x" else int(result["result"], 16)
+    
+    async def get_contract_balance(self, address, contract_address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         function_signature = "balanceOf(address)".encode("UTF-8")
         hash_result = keccak(function_signature)
         method_id = hash_result.hex()[:8]
         padded_address = address.lower().replace("0x", "").zfill(64)
         data = f"0x{method_id}{padded_address}"
 
         payload = {
                 "method": "eth_call",
                 "params": [{"to": contract_address, "data": data}, block_parameter.value],
             }
 
         result = await self._make_rpc_call(payload)
         balance = result["result"]
         return 0 if balance == "0x" else int(balance, 16)
-
-    async def get_transaction_count(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
+    
+    async def get_gas_price(self) -> int:
+        payload = {"method": "eth_gasPrice", "params": []}
+        result = await self._make_rpc_call(payload)
+        price = result["result"]
+        return 0 if price == "0x" else int(result["result"], 16)
+        
+    async def get_transaction(self, hash) -> dict:
+        payload = {"method": "eth_getTransactionByHash", "params": [hash]}
+        result = await self._make_rpc_call(payload)
+        if result["result"] is None:
+            raise TransactionNotFound(f"Transaction {hash} not found!")
+        tx_data = result["result"]
+        tx_data["aiotx_decoded_input"] = self.decode_transaction_input(tx_data["input"])
+        return tx_data
+    
+    async def get_transactions_count(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         payload = {"method": "eth_getTransactionCount", "params": [address, block_parameter.value]}
         result = await self._make_rpc_call(payload)
         tx_count = result["result"]
         return 0 if tx_count == "0x" else int(tx_count, 16)
 
-    async def send_transaction(
-        self, private_key: str, to_address: str, amount: int, gas_price: int, gas_limit: int = 21000
+    async def send(
+        self, private_key: str, to_address: str, amount: int, gas_price: int = None, gas_limit: int = 21000
     ) -> str:
+        if gas_price is None:
+            gas_price = await self.get_gas_price()
 
-        from_address = Account.from_key(private_key).address
-        nonce = await self.get_transaction_count(from_address)
-        raw_transaction = self.build_raw_transaction(private_key, to_address, nonce, amount, gas_price, gas_limit)
-
-        payload = {"method": "eth_sendRawTransaction", "params": [raw_transaction]}
-
-        result = await self._make_rpc_call(payload)
-        return result
-
-    def build_raw_transaction(
-        self, private_key: str, to_address: str, nonce: int, amount_in_wei: int, gas_price: int, gas_limit: int = 21000
-    ) -> HexStr:
+        from_address = self.get_address_from_private_key(private_key)
+        nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
         transaction = {
             "nonce": nonce,
             "gasPrice": gas_price,
             "gas": gas_limit,
-            "to": to_address,
-            "value": amount_in_wei,
+            "to": to_checksum_address(to_address),
+            "value": amount,
             "data": b"",
             "chainId": self.chain_id,
         }
         signed_transaction = Account.sign_transaction(transaction, private_key)
         raw_tx = to_hex(signed_transaction.rawTransaction)
-        return raw_tx
+        payload = {"method": "eth_sendRawTransaction", "params": [raw_tx]}
+        result = await self._make_rpc_call(payload)
+        return result["result"]
 
-    async def send_token_transaction(
+    async def send_token(
         self,
         private_key: str,
         to_address: str,
-        token_address: str,
+        contract_address: str,
         amount: int,
         gas_price: int,
         gas_limit: int = 100000,
     ) -> str:
-        sender_address = Account.from_key(private_key).address
+        from_address = self.get_address_from_private_key(private_key)
+        nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
 
         function_signature = "transfer(address,uint256)"
         function_selector = keccak(function_signature.encode("utf-8"))[:4].hex()
-        transfer_data = encode(["address", "uint256"], [to_address, amount])
+        transfer_data = encode(["address", "uint256"], [to_checksum_address(to_address), amount])
         data = "0x" + function_selector + transfer_data.hex()
 
         transaction = {
-            "nonce": await self.get_transaction_count(sender_address),
+            "nonce": nonce,
             "gasPrice": gas_price,
             "gas": gas_limit,
-            "to": token_address,
+            "to": contract_address,
             "value": 0,
             "data": data,
             "chainId": self.chain_id,
         }
 
         signed_transaction = Account.sign_transaction(transaction, private_key)
         raw_tx = to_hex(signed_transaction.rawTransaction)
@@ -274,15 +273,15 @@
         self.block_handlers = []
         self.transaction_handlers = []
         self.running = False
         self._latest_block = None
 
     async def poll_blocks(self,):
         if self._latest_block is None:
-            self._latest_block = await self.client.get_last_block()
+            self._latest_block = await self.client.get_last_block_number()
         block = await self.client.get_block_by_number(self._latest_block)
         await self.process_block(block["result"])
         self._latest_block = self._latest_block + 1
 
     async def process_block(self, block):
         for handler in self.block_handlers:
             if asyncio.iscoroutinefunction(handler):
```

### Comparing `aiotx-0.3.0/aiotx/exceptions.py` & `aiotx-0.4.0/aiotx/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,8 +50,11 @@
 class InternalJSONAioTxError(AioTxError):
     pass
 
 class TransactionNotFound(AioTxError):
     pass
 
 class ReplacementTransactionUnderpriced(AioTxError):
+    pass
+
+class WrongPrivateKey(AioTxError):
     pass
```

### Comparing `aiotx-0.3.0/aiotx/utils/bep20_abi.json` & `aiotx-0.4.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/aiotx.egg-info/PKG-INFO` & `aiotx-0.4.0/aiotx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.3.0
+Version: 0.4.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -53,26 +53,30 @@
 
 # Usage
 Here's a simple example of how to use AioTx to create a wallet and retrieve its balance:
 
 ```
 from aiotx import AioTxBSCClient
 
+bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
+
 async def main():
-    bsc_client = AioTxBSCClient(node_url="https://example.com", chain_id=97)
-    
     # Create a new wallet
-    address, private_key = await bsc_client.generate_address()
+    address, private_key = bsc_client.generate_address()
     
     # Retrieve the wallet balance
     balance = await bsc_client.get_balance(address)
     print(f"Wallet balance: {balance}")
 
-    # Send transaction
-    tx_id = await bsc_client.send_transaction(private_key, to_address, amount, gas_price, gas_limit)
+    # Send BNB
+    tx_id = await bsc_client.send(private_key, to_address, amount)
+    print(f"Your tx: {tx_id}")
+
+    # Send any token
+    tx_id = await bsc_client.send_token(private_key, to_address, contract_address, amount)
     print(f"Your tx: {tx_id}")
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
```

### Comparing `aiotx-0.3.0/aiotx.egg-info/SOURCES.txt` & `aiotx-0.4.0/aiotx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/examples/aiogram_notificator_bot.png` & `aiotx-0.4.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/examples/aiogram_notificator_bot.py` & `aiotx-0.4.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/examples/block_and_transactions_parser.py` & `aiotx-0.4.0/examples/block_and_transactions_parser.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/examples/two_block_parsers.py` & `aiotx-0.4.0/examples/two_block_parsers.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/setup.py` & `aiotx-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/confest.py` & `aiotx-0.4.0/tests/confest.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-0.4.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/test_bsc_input_decoding.py` & `aiotx-0.4.0/tests/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.3.0/tests/test_bsc_monitoring.py` & `aiotx-0.4.0/tests/test_bsc_monitoring.py`

 * *Files identical despite different names*

