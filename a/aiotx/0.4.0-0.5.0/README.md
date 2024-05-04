# Comparing `tmp/aiotx-0.4.0.tar.gz` & `tmp/aiotx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.4.0.tar", last modified: Fri May  3 11:02:04 2024, max compression
+gzip compressed data, was "aiotx-0.5.0.tar", last modified: Sat May  4 09:28:45 2024, max compression
```

## Comparing `aiotx-0.4.0.tar` & `aiotx-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.683173 aiotx-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.671173 aiotx-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 11:01:57.000000 aiotx-0.4.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 11:01:57.000000 aiotx-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-03 11:01:57.000000 aiotx-0.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 11:01:57.000000 aiotx-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-03 11:01:57.000000 aiotx-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-03 11:02:04.683173 aiotx-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-03 11:01:57.000000 aiotx-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/_bitcoin_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 11:01:57.000000 aiotx-0.4.0/aiotx/utils/bep20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 11:02:04.000000 aiotx-0.4.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 11:01:57.000000 aiotx-0.4.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 11:01:57.000000 aiotx-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 11:01:57.000000 aiotx-0.4.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-03 11:01:57.000000 aiotx-0.4.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 11:02:04.683173 aiotx-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 11:01:57.000000 aiotx-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/confest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.671173 aiotx-0.4.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.675173 aiotx-0.4.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:02:04.679173 aiotx-0.4.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 11:01:57.000000 aiotx-0.4.0/tests/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.871361 aiotx-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-04 09:28:40.000000 aiotx-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-04 09:28:40.000000 aiotx-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-04 09:28:40.000000 aiotx-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-04 09:28:40.000000 aiotx-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-04 09:28:40.000000 aiotx-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-04 09:28:45.871361 aiotx-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-04 09:28:40.000000 aiotx-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.871361 aiotx-0.5.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/docs/clients/bsc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_token_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/send_token_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/send_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/docs/clients/btc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/docs/clients/eth_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/to_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/monitoring.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-04 09:28:40.000000 aiotx-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 09:28:40.000000 aiotx-0.5.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-04 09:28:40.000000 aiotx-0.5.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 09:28:45.871361 aiotx-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-04 09:28:40.000000 aiotx-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.867361 aiotx-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.867361 aiotx-0.5.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.871361 aiotx-0.5.0/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_bsc_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_eth_monitoring.py
```

### Comparing `aiotx-0.4.0/.github/workflows/lint-check.yml` & `aiotx-0.5.0/.github/workflows/lint-check.yml`

 * *Files 12% similar despite different names*

```diff
@@ -22,7 +22,8 @@
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest
         pip install .[test]
     - name: Analysing the code with pylint
       run: |
         ruff check --select I aiotx tests 
+        ruff check  aiotx tests
```

### Comparing `aiotx-0.4.0/.github/workflows/python-publish.yml` & `aiotx-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/.github/workflows/test.yml` & `aiotx-0.5.0/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Test
 
 env:
   TEST_BSC_WALLET_PRIVATE_KEY: ${{ secrets.TEST_BSC_WALLET_PRIVATE_KEY }}
+  TEST_ETH_WALLET_PRIVATE_KEY: ${{ secrets.TEST_ETH_WALLET_PRIVATE_KEY }}
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
```

### Comparing `aiotx-0.4.0/.gitignore` & `aiotx-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/CHANGELOG.md` & `aiotx-0.5.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.5.0]
+- AioTxETHClient covered by tests and ready to be used
+- nonce is now optional param to give users enter in manually for sending transactions faster
+- get_contract_decimals function added for EVMClient, now you can get decimals for contracts
+
 ## [0.4.0]
 - Added tests for send and send_token function, they was renamed and changed, getting pending for nonce now
 
 ## [0.3.0]
 - Function for getting current gas price is added and to_wai/from_wai functions are attached to EVM client now
 
 ## [0.2.0]
```

### Comparing `aiotx-0.4.0/PKG-INFO` & `aiotx-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.4.0
+Version: 0.5.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,24 +15,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: eth_keys
 Requires-Dist: eth_utils
 Requires-Dist: eth_account
 Provides-Extra: test
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: pyproj; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: sphinx; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: build; extra == "test"
 Requires-Dist: vcrpy; extra == "test"
 
 ## AioTx
```

### Comparing `aiotx-0.4.0/README.md` & `aiotx-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/aiotx/clients/_base_client.py` & `aiotx-0.5.0/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/aiotx/clients/_evm_base_client.py` & `aiotx-0.5.0/aiotx/clients/_evm_base_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,21 +40,18 @@
     WrongPrivateKey,
 )
 from aiotx.types import BlockParam
 
 
 class AioTxEVMClient(AioTxClient):
     def __init__(self, node_url, chain_id):
-        self.node_url = node_url
+        super().__init__(node_url)
         self.chain_id = chain_id
         self.monitor = EvmMonitor(self)
         self._monitoring_task = None
-        with open("aiotx/utils/bep20_abi.json") as file:
-            bep_20_abi = json.loads(file.read())
-        self._bep20_abi = bep_20_abi
 
     def generate_address(self):
         private_key_bytes = secrets.token_hex(32)
         private_key = "0x" + private_key_bytes
         acct = Account.from_key(private_key)
         return private_key, acct.address
     
@@ -68,23 +65,29 @@
     @staticmethod
     def from_wei(number: int, unit: str) -> Union[int, decimal.Decimal]:
         return currency.from_wei(number, unit)
     
     @staticmethod
     def to_wei(number: Union[int, float, str, decimal.Decimal], unit: str) -> int:
         return currency.to_wei(number, unit)
+    
+    def _get_abi_entries(self):
+        # Redefine that in you client
+        return []
 
     def decode_transaction_input(self, input_data: str) -> dict:
         if input_data == "0x":
             return {
             'function_name': None,
             'parameters': None
         }
-        for abi_entry in self._bep20_abi:
-            function_name = abi_entry['name']
+        for abi_entry in self._get_abi_entries():
+            function_name = abi_entry.get("name")
+            if function_name is None:
+                continue
             input_types = [inp['type'] for inp in abi_entry['inputs']]
             function_signature = f"{function_name}({','.join(input_types)})"
             function_selector = function_signature_to_4byte_selector(function_signature)
 
             if input_data.startswith('0x' + function_selector.hex()):
                 decoded_data = decode(input_types, decode_hex(input_data[10:]))
                 decoded_params = {}
@@ -112,15 +115,14 @@
     async def get_block_by_number(self, block_number: int, transaction_detail_flag: bool = True):
         payload = {"method": "eth_getBlockByNumber", "params": [hex(block_number), transaction_detail_flag]}
         result = await self._make_rpc_call(payload)
         return result
 
     async def get_balance(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         payload = {"method": "eth_getBalance", "params": [address, block_parameter.value]}
-
         result = await self._make_rpc_call(payload)
         balance = result["result"]
         return 0 if balance == "0x" else int(result["result"], 16)
     
     async def get_contract_balance(self, address, contract_address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         function_signature = "balanceOf(address)".encode("UTF-8")
         hash_result = keccak(function_signature)
@@ -133,14 +135,26 @@
                 "params": [{"to": contract_address, "data": data}, block_parameter.value],
             }
 
         result = await self._make_rpc_call(payload)
         balance = result["result"]
         return 0 if balance == "0x" else int(balance, 16)
     
+    async def get_contract_decimals(self, contract_address) -> int:
+        function_signature = "decimals()".encode("UTF-8")
+        hash_result = keccak(function_signature)
+        method_id = hash_result.hex()[:8]
+        payload = {
+            "method": "eth_call",
+            "params": [{"to": contract_address, "data": f"0x{method_id}"}, "latest"],
+        }
+        result = await self._make_rpc_call(payload)
+        decimals = result["result"]
+        return 0 if decimals == "0x" else int(decimals, 16)
+
     async def get_gas_price(self) -> int:
         payload = {"method": "eth_gasPrice", "params": []}
         result = await self._make_rpc_call(payload)
         price = result["result"]
         return 0 if price == "0x" else int(result["result"], 16)
         
     async def get_transaction(self, hash) -> dict:
@@ -155,21 +169,22 @@
     async def get_transactions_count(self, address, block_parameter: BlockParam = BlockParam.LATEST) -> int:
         payload = {"method": "eth_getTransactionCount", "params": [address, block_parameter.value]}
         result = await self._make_rpc_call(payload)
         tx_count = result["result"]
         return 0 if tx_count == "0x" else int(tx_count, 16)
 
     async def send(
-        self, private_key: str, to_address: str, amount: int, gas_price: int = None, gas_limit: int = 21000
+        self, private_key: str, to_address: str, amount: int, nonce: int = None, gas_price: int = None, gas_limit: int = 21000
     ) -> str:
         if gas_price is None:
             gas_price = await self.get_gas_price()
 
         from_address = self.get_address_from_private_key(private_key)
-        nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
+        if nonce is None:
+            nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
         transaction = {
             "nonce": nonce,
             "gasPrice": gas_price,
             "gas": gas_limit,
             "to": to_checksum_address(to_address),
             "value": amount,
             "data": b"",
@@ -183,20 +198,23 @@
 
     async def send_token(
         self,
         private_key: str,
         to_address: str,
         contract_address: str,
         amount: int,
-        gas_price: int,
+        nonce: int = None,
+        gas_price: int = None,
         gas_limit: int = 100000,
     ) -> str:
         from_address = self.get_address_from_private_key(private_key)
-        nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
-
+        if nonce is None:
+            nonce = await self.get_transactions_count(from_address, BlockParam.PENDING)
+        if gas_price is None:
+            gas_price = await self.get_gas_price()
         function_signature = "transfer(address,uint256)"
         function_selector = keccak(function_signature.encode("utf-8"))[:4].hex()
         transfer_data = encode(["address", "uint256"], [to_checksum_address(to_address), amount])
         data = "0x" + function_selector + transfer_data.hex()
 
         transaction = {
             "nonce": nonce,
```

### Comparing `aiotx-0.4.0/aiotx/exceptions.py` & `aiotx-0.5.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/aiotx/utils/bep20_abi.json` & `aiotx-0.5.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/aiotx.egg-info/PKG-INFO` & `aiotx-0.5.0/aiotx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.4.0
+Version: 0.5.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,24 +15,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: eth_keys
 Requires-Dist: eth_utils
 Requires-Dist: eth_account
 Provides-Extra: test
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: pyproj; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: sphinx; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: build; extra == "test"
 Requires-Dist: vcrpy; extra == "test"
 
 ## AioTx
```

### Comparing `aiotx-0.4.0/examples/aiogram_notificator_bot.png` & `aiotx-0.5.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/examples/aiogram_notificator_bot.py` & `aiotx-0.5.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/examples/block_and_transactions_parser.py` & `aiotx-0.5.0/examples/block_and_transactions_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 @client.monitor.on_transaction
 def handle_transaction(transaction):
     print("transaction", transaction)
 
 
 async def main():
-    await client.start_monitoring(584)
+    await client.start_monitoring()
 
     try:
         while True:
             await asyncio.sleep(1)
     except KeyboardInterrupt:
         client.stop_monitoring()
```

### Comparing `aiotx-0.4.0/examples/two_block_parsers.py` & `aiotx-0.5.0/examples/two_block_parsers.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/setup.py` & `aiotx-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 extras_test = (
     [
         "hypothesis",
         "ruff",
         "pyproj",
         "pytest",
         "pytest-cov",
+        "sphinx",
         "pytest-asyncio",
         "tox",
         "build",
         "vcrpy"
     ]
 )
 
@@ -29,15 +30,15 @@
         "wallet",
         "transaction",
     ],
     use_scm_version=True,
     description="An asynchronous library for interacting with various cryptocurrencies and blockchains",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=("tests", "scripts", "examples")),
+    packages=find_packages(exclude=("tests", "scripts", "examples", "docs")),
     package_data={
         "aiotx": ["py.typed"],
     },
     setup_requires=[
         "setuptools_scm",
     ],
     install_requires=[
```

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     body: '{"method": "eth_getTransactionCount", "params": ["0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e",
       "pending"], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x7e"}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x7f"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -20,33 +20,33 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '41'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:45 GMT
+      - Fri, 03 May 2024 10:46:47 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
+      - f1b546936d23e3b5-84b84c7a90242c73
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8aa7e85012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a0ba58900b587e6278f5476fc28a1f09bf4b326bb72e06361642aab898ef8939f8a06296f0183dad417850fb2e9d260a0887c77687b4c47069652fb6dbf4cf3af341"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86b7f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0dd2ec3a72bee9de8e0367fbf926550e1bbac5d4860184dfa22fec644571f1568a05b3b44321e5976a00e23b91aed9e900a0e854b4b31ca47662d375c524ec2a58f"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x247e15f1dc165cb70964bb206c7bd0457490a33042c7a8c80453d250f8f30adb"}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0xdad97e8972e7a4cc72f28944a16aa5782d6562aac483b527c27d1ee88e33ed5a"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -55,62 +55,63 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '103'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:45 GMT
+      - Fri, 03 May 2024 10:46:47 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
+      - f1b546936d23e3b5-84b84c7a90242c73
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8aa7e85012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a00000000000000000000000000000000000000000000003635c9adc5dea0000081e6a02b3a459ca69afce5840f287c4da1138622ba38eed7ea6c66718c5890ae5cfc75a06e928f4a2675fd1dfb3e9edf660ce020a4025f50e7ee3af331828ea1baa3ed01"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86d7f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a884563918244f400008081e5a076bcd75b7ded882a7e7194a6588969a505b9b3e9d9f7fb0a7e0af90244cdd4e5a06b371861ae4283029ad8c2c4a6f8913190b949deeb815bd6028bd88564bc29a3"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
-        transaction underpriced"}}
+      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"insufficient
+        funds for gas * price + value: balance 19594850000960000, tx cost 5000105000000000000,
+        overshot 4980510149999040000"}}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '97'
+      - '190'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:46 GMT
+      - Fri, 03 May 2024 10:46:48 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
+      - f1b546936d23e3b5-2bd95d6b916503dd
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a57e8082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a03d89bf6188b6089d1b3adee999ed9b9005651a98b3859867bb19eef37987bfafa054f02f754f57f7b38c7154fab2dc154e9ef34f1bcd81751806be6477736201f0"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8667f8082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0157babe76ee1d04f5dc9669b033779bc552f8047911e6ef74e20475e804282a7a06524c9fb61bbef7f4c77c67354d106742bd34eb8bc597c769ae9c1f4ebf638e4"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
       string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
@@ -127,26 +128,26 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '127'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:46 GMT
+      - Fri, 03 May 2024 10:46:48 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-dbb2877f11a402e9
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8aa7e85012a05f20082ee4894337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a000000000000000000000000000000000000000000000000000000000000000081e6a01ad77489659872f1037f05f1463bdbc4a4bc88e07770fa29ecf231cea2aa2d2da074b6c5bc9a7d8a704dda251aec574de2d188f66703bf1c39eeab4a504ea1ccbd"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8657f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a808081e5a07650c5abd4d2e0f2d0a377c89381d0d56d762a0f9e94975cbb540363cd058959a01b626479385aad061246df6e54a9f59fa898c1f58b341716a533b5682921d28b"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
       string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
@@ -163,34 +164,34 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '97'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:46 GMT
+      - Fri, 03 May 2024 10:46:48 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
+      - f1b546936d23e3b5-10ebeaeae12fe5d7
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8a87e85012a05f2008094337610d27c682e347c9cd60bd4b3b107c9d34ddd80b844a9059cbb000000000000000000000000f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a0000000000000000000000000000000000000000000000000de0b6b3a764000081e6a0c72ec598dde29546d5047253d68f08bb3259d82eb6bec1da59336c16b3052125a07616ed31466c365c61ceeed698ffcc3fc422de8ce84a21255b9c4806bf2845f9"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8697f85012a05f2008094f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e5a08c87832c5608247b85f2c8d24852172e704ff0cb11edb0db3800c49599d1d5c4a017026aaa07c5ce6b31ce684680146ff681d6a8edfb4c73eaf3d83347b8f4ff97"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
       string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"intrinsic
-        gas too low: gas 0, minimum needed 21632"}}
+        gas too low: gas 0, minimum needed 21000"}}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -199,18 +200,54 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '112'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:47 GMT
+      - Fri, 03 May 2024 10:46:49 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
+      - f1b546936d23e3b5-4291c05108b63f99
+      X-Node-Id:
+      - bnb-smart-chain_bsc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86b7f85012a05f20082ee4894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e5a08eb0828e7d41dc68c8cbfbae52045328afbc4ddb490e982c356151b10d3ec630a00e8a57d4c6a159279e91fddb7f4e0f570a49cb08814da1b36d5828714afd4f16"],
+      "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
+        transaction underpriced"}}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '97'
+      Content-Type:
+      - application/json
+      Date:
+      - Fri, 03 May 2024 10:46:49 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-84b84c7a90242c73
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 interactions:
 - request:
     body: '{"method": "eth_getTransactionCount", "params": ["0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e",
-      "pending"], "jsonrpc": "2.0", "id": 1}'
+      "latest"], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0x7f"}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x82"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -20,231 +20,153 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '41'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:47 GMT
+      - Sat, 04 May 2024 08:29:18 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86b7f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0dd2ec3a72bee9de8e0367fbf926550e1bbac5d4860184dfa22fec644571f1568a05b3b44321e5976a00e23b91aed9e900a0e854b4b31ca47662d375c524ec2a58f"],
-      "jsonrpc": "2.0", "id": 1}'
-    headers: {}
-    method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
-  response:
-    body:
-      string: '{"jsonrpc":"2.0","id":1,"result":"0xdad97e8972e7a4cc72f28944a16aa5782d6562aac483b527c27d1ee88e33ed5a"}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '103'
-      Content-Type:
-      - application/json
-      Date:
-      - Fri, 03 May 2024 10:46:47 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-84b84c7a90242c73
-      X-Node-Id:
-      - bnb-smart-chain_bsc-testnet_iad
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86d7f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a884563918244f400008081e5a076bcd75b7ded882a7e7194a6588969a505b9b3e9d9f7fb0a7e0af90244cdd4e5a06b371861ae4283029ad8c2c4a6f8913190b949deeb815bd6028bd88564bc29a3"],
-      "jsonrpc": "2.0", "id": 1}'
-    headers: {}
-    method: POST
-    uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
-  response:
-    body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"insufficient
-        funds for gas * price + value: balance 19594850000960000, tx cost 5000105000000000000,
-        overshot 4980510149999040000"}}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '190'
-      Content-Type:
-      - application/json
-      Date:
-      - Fri, 03 May 2024 10:46:48 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-2bd95d6b916503dd
+      - f1b546936d23e3b5-4291c05108b63f99
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8667f8082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0157babe76ee1d04f5dc9669b033779bc552f8047911e6ef74e20475e804282a7a06524c9fb61bbef7f4c77c67354d106742bd34eb8bc597c769ae9c1f4ebf638e4"],
-      "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "eth_gasPrice", "params": [], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"transaction
-        underpriced: gas tip cap 0, minimum needed 1000000000"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x123f92da0"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '127'
+      - '48'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:48 GMT
+      - Sat, 04 May 2024 08:29:19 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-dbb2877f11a402e9
+      - f1b546936d23e3b5-4291c05108b63f99
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8657f85012a05f20082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a808081e5a07650c5abd4d2e0f2d0a377c89381d0d56d762a0f9e94975cbb540363cd058959a01b626479385aad061246df6e54a9f59fa898c1f58b341716a533b5682921d28b"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86c8182850123f92da082520894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e6a0b04081f4c041911a511f34e23352c05ee7e46b88dafc9cd7d7f3c168322f3deda00ced47f99dc12d686ea384873f8d37d38ffb5dc0fcb2a5d18c25214a7f7e5245"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
-        transaction underpriced"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x0f47bdb42e18137f1e166e2fee68877fca081e6e6f639c0ce629a363db5a5e1e"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '97'
+      - '103'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:48 GMT
+      - Sat, 04 May 2024 08:29:19 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-10ebeaeae12fe5d7
+      - f1b546936d23e3b5-ecf10b7bc104d983
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf8697f85012a05f2008094f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e5a08c87832c5608247b85f2c8d24852172e704ff0cb11edb0db3800c49599d1d5c4a017026aaa07c5ce6b31ce684680146ff681d6a8edfb4c73eaf3d83347b8f4ff97"],
-      "jsonrpc": "2.0", "id": 1}'
+    body: '{"method": "eth_gasPrice", "params": [], "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"intrinsic
-        gas too low: gas 0, minimum needed 21000"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x123f92da0"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '112'
+      - '48'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:49 GMT
+      - Sat, 04 May 2024 08:29:19 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-4291c05108b63f99
+      - f1b546936d23e3b5-84b84c7a90242c73
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
-    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86b7f85012a05f20082ee4894f9e35e4e1cbcf08e99b84d3f6ff662ba4c306b5a8609184e72a0008081e5a08eb0828e7d41dc68c8cbfbae52045328afbc4ddb490e982c356151b10d3ec630a00e8a57d4c6a159279e91fddb7f4e0f570a49cb08814da1b36d5828714afd4f16"],
+    body: '{"method": "eth_sendRawTransaction", "params": ["0xf86c8183850123f92da0825208943ffecb152f95f7122990ab16eff4b0b5d533497e8609184e72a0008081e6a0fc492839015f1e9bc8381ebea382c72af6ac48c797050584d344bcc20a15437ba05ffcbd6ff4d80f15b143f4cc2b6f6e12f4c7b576f91c20804c4db72f421c01af"],
       "jsonrpc": "2.0", "id": 1}'
     headers: {}
     method: POST
     uri: https://nameless-flashy-snow.bsc-testnet.quiknode.pro/c54e248a38fb9b7a8b31d84d57c1e41b203ed019/
   response:
     body:
-      string: '{"jsonrpc":"2.0","id":1,"error":{"code":-32000,"message":"replacement
-        transaction underpriced"}}
+      string: '{"jsonrpc":"2.0","id":1,"result":"0x1b03c2e3590ed2193130dbbd25596877adc22e746f705b353d6f6b5f7ce0d192"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
       Access-Control-Allow-Methods:
       - GET, POST, OPTIONS
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
-      - '97'
+      - '103'
       Content-Type:
       - application/json
       Date:
-      - Fri, 03 May 2024 10:46:49 GMT
+      - Sat, 04 May 2024 08:29:19 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-84b84c7a90242c73
       X-Node-Id:
       - bnb-smart-chain_bsc-testnet_iad
     status:
```

### Comparing `aiotx-0.4.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-0.5.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.4.0/tests/test_bsc_client.py` & `aiotx-0.5.0/tests/test_bsc_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 import pytest
-from confest import bsc_client, vcr_c  # noqa
+from conftest import vcr_c  # noqa
 
 from aiotx.clients import AioTxBSCClient
 from aiotx.exceptions import (
     AioTxError,
     InvalidArgumentError,
     ReplacementTransactionUnderpriced,
     TransactionNotFound,
@@ -119,15 +119,15 @@
         count = await bsc_client.get_transactions_count(wallet_address)
         assert isinstance(count, int)
         assert expected_count == count
 
 
 
 @vcr_c.use_cassette("bsc/get_gas_price.yaml")
-async def test_send_token_transaction(bsc_client: AioTxBSCClient):
+async def test_send_get_gas_price(bsc_client: AioTxBSCClient):
     result = await bsc_client.get_gas_price()
     assert isinstance(result, int)
     assert result == 5000000000
 
 
 @pytest.mark.parametrize(
     "private_key, to_address, amount, gas_price, gas_limit, expected_exception",
@@ -152,19 +152,52 @@
     Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
     the same VCR data for every get nonce request, we should investigate how we can change that maybe?
     """
     gas_price = bsc_client.to_wei(gas_price, "gwei")
     wei_amount = bsc_client.to_wei(amount, "ether")
     if expected_exception:
         with pytest.raises(expected_exception):
-            await bsc_client.send(private_key, to_address, wei_amount, gas_price, gas_limit)
+            await bsc_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
     else:
-        result = await bsc_client.send(private_key, to_address, wei_amount, gas_price, gas_limit)
+        result = await bsc_client.send(private_key, to_address, wei_amount, gas_price=gas_price, gas_limit=gas_limit)
         assert isinstance(result, str)
 
+
+@pytest.mark.parametrize(
+    "private_key, to_address, amount, expected_exception",
+    [
+        (PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, 0.00001, None),
+        (PRIVATE_KEY_TO_SEND_FROM, "0x3ffeCb152F95f7122990ab16Eff4B0B5d533497e", 0.00001, ReplacementTransactionUnderpriced),
+    ],
+)
+@vcr_c.use_cassette("bsc/send_transaction_with_auto_gas.yaml")
+async def test_send_transaction_with_auto_gas(bsc_client: AioTxBSCClient, private_key, to_address, amount, expected_exception):
+    """
+    Here it's raising ReplacementTransactionUnderpriced and NonceTooLowError because we have reusing
+    the same VCR data for every get nonce request, we should investigate how we can change that maybe?
+    """
+    wei_amount = bsc_client.to_wei(amount, "ether")
+    if expected_exception:
+        with pytest.raises(expected_exception):
+            await bsc_client.send(private_key, to_address, wei_amount)
+    else:
+        result = await bsc_client.send(private_key, to_address, wei_amount)
+        assert isinstance(result, str)
+
+
+@vcr_c.use_cassette("bsc/send_transaction_with_custom_nonce.yaml")
+async def test_send_transaction_with_custom_nonce(bsc_client: AioTxBSCClient):
+    wei_amount = bsc_client.to_wei(0.00001, "ether")
+    sender_address = bsc_client.get_address_from_private_key(PRIVATE_KEY_TO_SEND_FROM)
+    nonce = await bsc_client.get_transactions_count(sender_address)
+    first_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, DESTINATION_ADDRESS, wei_amount, nonce=nonce)
+    assert isinstance(first_tx, str)
+    second_tx = await bsc_client.send(PRIVATE_KEY_TO_SEND_FROM, sender_address, wei_amount, nonce=nonce + 1)
+    assert isinstance(second_tx, str)
+
 @pytest.mark.parametrize(
     "private_key, to_address, contract, amount, gas_price, gas_limit, expected_exception",
     [
         ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS, CONTRACT, 1, 5, 61000, WrongPrivateKey),
         ("87e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938ch", DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, WrongPrivateKey),
         ("e6dah15aa076a932cd9f0663da72f8cfb6d3e23c00ef1269104bd904938chd", DESTINATION_ADDRESS,CONTRACT, 1, 5, 61000, WrongPrivateKey),
         (PRIVATE_KEY_TO_SEND_FROM, "0xf9E35E4e1CbcF08E984d3f6FF662Ba4c306b5a",CONTRACT, 1, 5, 61000, ValueError),
@@ -189,14 +222,32 @@
     """
     gas_price = bsc_client.to_wei(gas_price, "gwei")
     wei_amount = bsc_client.to_wei(amount, "ether")
 
     if expected_exception:
         with pytest.raises(expected_exception):
             await bsc_client.send_token(
-        private_key, to_address, contract, wei_amount, gas_price, gas_limit
+        private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
     )
     else:
         result = await bsc_client.send_token(
-        private_key, to_address, contract, wei_amount, gas_price, gas_limit
+        private_key, to_address, contract, wei_amount, gas_price=gas_price, gas_limit=gas_limit
     )
         assert isinstance(result, str)
+
+
+@pytest.mark.parametrize(
+    "contract, expected_decimals, expected_exception",
+    [
+        (CONTRACT, 18, None),
+        ("0x337610d27c682E347C9cD60BD4b3b107C9d34dD", 18, InvalidArgumentError),
+        ("0x757fc78bb4df4ce6605ae669bf0b71074176aac3", 9, None),
+    ],
+)
+@vcr_c.use_cassette("bsc/get_contract_decimals.yaml")
+async def test_get_contract_decimals(bsc_client: AioTxBSCClient, contract, expected_decimals, expected_exception):
+    if expected_exception:
+        with pytest.raises(expected_exception):
+            await bsc_client.get_contract_decimals(contract)
+    else:
+        decimals = await bsc_client.get_contract_decimals(contract)
+        assert decimals == expected_decimals
```

### Comparing `aiotx-0.4.0/tests/test_bsc_input_decoding.py` & `aiotx-0.5.0/tests/test_bsc_input_decoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-from confest import bsc_client  # noqa
 
 
 @pytest.mark.parametrize("input_data, expected_output", [
     ("0x", {'function_name': None, 'parameters': None}),
 
     ("0xa9059cbb00000000000000000000000012345678901234567890123456789012345678900000000000000000000000000000000000000000000000000000000000000064",
      {'function_name': 'transfer',
```

### Comparing `aiotx-0.4.0/tests/test_bsc_monitoring.py` & `aiotx-0.5.0/tests/test_bsc_monitoring.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-from confest import bsc_client, vcr_c  # noqa
+from conftest import vcr_c
 
 from aiotx.clients import AioTxBSCClient
 
 
 @vcr_c.use_cassette("tests/fixtures/cassettes/bsc/test_async_monitoring.yaml")
 async def test_async_monitoring(bsc_client: AioTxBSCClient):
     blocks = []
```

