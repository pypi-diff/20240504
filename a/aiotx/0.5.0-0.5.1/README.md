# Comparing `tmp/aiotx-0.5.0.tar.gz` & `tmp/aiotx-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-0.5.0.tar", last modified: Sat May  4 09:28:45 2024, max compression
+gzip compressed data, was "aiotx-0.5.1.tar", last modified: Sat May  4 10:41:21 2024, max compression
```

## Comparing `aiotx-0.5.0.tar` & `aiotx-0.5.1.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.871361 aiotx-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-04 09:28:40.000000 aiotx-0.5.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-04 09:28:40.000000 aiotx-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-04 09:28:40.000000 aiotx-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-04 09:28:40.000000 aiotx-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-04 09:28:40.000000 aiotx-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-04 09:28:40.000000 aiotx-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-04 09:28:45.871361 aiotx-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-04 09:28:40.000000 aiotx-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/_bitcoin_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/utils/bep20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-04 09:28:40.000000 aiotx-0.5.0/aiotx/utils/erc20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.871361 aiotx-0.5.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 09:28:45.000000 aiotx-0.5.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.859361 aiotx-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/docs/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/docs/clients/bsc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_gas_price.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_last_block.rst
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_token_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/get_transaction_count.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/send_token_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/send_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/bsc_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/docs/clients/btc_client/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/btc_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/docs/clients/eth_client/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/clients/eth_client/to_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-04 09:28:40.000000 aiotx-0.5.0/docs/monitoring.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-04 09:28:40.000000 aiotx-0.5.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-04 09:28:40.000000 aiotx-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 09:28:40.000000 aiotx-0.5.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.863361 aiotx-0.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-04 09:28:40.000000 aiotx-0.5.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 09:28:45.871361 aiotx-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-04 09:28:40.000000 aiotx-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.867361 aiotx-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.855361 aiotx-0.5.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.867361 aiotx-0.5.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:28:45.871361 aiotx-0.5.0/tests/fixtures/cassettes/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_bsc_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_eth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_eth_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-04 09:28:40.000000 aiotx-0.5.0/tests/test_eth_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.874438 aiotx-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.854438 aiotx-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.858438 aiotx-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 10:41:16.000000 aiotx-0.5.1/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 10:41:16.000000 aiotx-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-04 10:41:16.000000 aiotx-0.5.1/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-04 10:41:16.000000 aiotx-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-04 10:41:16.000000 aiotx-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-04 10:41:16.000000 aiotx-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-04 10:41:16.000000 aiotx-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-04 10:41:16.000000 aiotx-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-04 10:41:16.000000 aiotx-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-04 10:41:21.874438 aiotx-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-04 10:41:16.000000 aiotx-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.862439 aiotx-0.5.1/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.862439 aiotx-0.5.1/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/clients/_bitcoin_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.862439 aiotx-0.5.1/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.862439 aiotx-0.5.1/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-04 10:41:16.000000 aiotx-0.5.1/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.874438 aiotx-0.5.1/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-04 10:41:21.000000 aiotx-0.5.1/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-04 10:41:21.000000 aiotx-0.5.1/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:41:21.000000 aiotx-0.5.1/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-04 10:41:21.000000 aiotx-0.5.1/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 10:41:21.000000 aiotx-0.5.1/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.862439 aiotx-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.858438 aiotx-0.5.1/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.866438 aiotx-0.5.1/docs/clients/evm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_contract_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_contract_decimals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/send_token.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/evm_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.866438 aiotx-0.5.1/docs/clients/tron_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/tron_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/tron_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/tron_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/tron_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.866438 aiotx-0.5.1/docs/clients/utxo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/utxo_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/utxo_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/utxo_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/clients/utxo_client/to_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-04 10:41:16.000000 aiotx-0.5.1/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.866438 aiotx-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-04 10:41:16.000000 aiotx-0.5.1/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 10:41:16.000000 aiotx-0.5.1/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 10:41:16.000000 aiotx-0.5.1/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-04 10:41:16.000000 aiotx-0.5.1/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-04 10:41:16.000000 aiotx-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 10:41:16.000000 aiotx-0.5.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.866438 aiotx-0.5.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-04 10:41:16.000000 aiotx-0.5.1/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 10:41:21.874438 aiotx-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-04 10:41:16.000000 aiotx-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.870438 aiotx-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.858438 aiotx-0.5.1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.858438 aiotx-0.5.1/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.870438 aiotx-0.5.1/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:21.874438 aiotx-0.5.1/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/test_bsc_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-04 10:41:16.000000 aiotx-0.5.1/tests/test_eth_monitoring.py
```

### Comparing `aiotx-0.5.0/.github/workflows/lint-check.yml` & `aiotx-0.5.1/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/.github/workflows/python-publish.yml` & `aiotx-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/.github/workflows/static.yml` & `aiotx-0.5.1/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/.github/workflows/test.yml` & `aiotx-0.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/.gitignore` & `aiotx-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/CHANGELOG.md` & `aiotx-0.5.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.5.1]
+- EVM client docs added
+
 ## [0.5.0]
 - AioTxETHClient covered by tests and ready to be used
 - nonce is now optional param to give users enter in manually for sending transactions faster
 - get_contract_decimals function added for EVMClient, now you can get decimals for contracts
 
 ## [0.4.0]
 - Added tests for send and send_token function, they was renamed and changed, getting pending for nonce now
```

### Comparing `aiotx-0.5.0/CODE_OF_CONDUCT.md` & `aiotx-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/CONTRIBUTING.md` & `aiotx-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/LICENSE` & `aiotx-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/PKG-INFO` & `aiotx-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.5.0
+Version: 0.5.1
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
+Project-URL: Documentation, https://grommash9.github.io/aiotx/
+Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -79,12 +81,14 @@
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
 
+https://grommash9.github.io/aiotx/
+
 # Contributing
 Contributions to AioTx are welcome! If you find any bugs, have feature requests, or want to contribute improvements, please open an issue or submit a pull request on the GitHub repository.
 
 # License
 AioTx is open-source software licensed under the MIT License.
```

### Comparing `aiotx-0.5.0/README.md` & `aiotx-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,14 @@
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
 
+https://grommash9.github.io/aiotx/
+
 # Contributing
 Contributions to AioTx are welcome! If you find any bugs, have feature requests, or want to contribute improvements, please open an issue or submit a pull request on the GitHub repository.
 
 # License
 AioTx is open-source software licensed under the MIT License.
```

### Comparing `aiotx-0.5.0/aiotx/clients/__init__.py` & `aiotx-0.5.1/aiotx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/aiotx/clients/_base_client.py` & `aiotx-0.5.1/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/aiotx/clients/_evm_base_client.py` & `aiotx-0.5.1/aiotx/clients/_evm_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/aiotx/exceptions.py` & `aiotx-0.5.1/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/aiotx/utils/bep20_abi.json` & `aiotx-0.5.1/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/aiotx/utils/erc20_abi.json` & `aiotx-0.5.1/aiotx/utils/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/aiotx.egg-info/PKG-INFO` & `aiotx-0.5.1/aiotx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 0.5.0
+Version: 0.5.1
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
+Project-URL: Documentation, https://grommash9.github.io/aiotx/
+Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -79,12 +81,14 @@
 
 # Run the async main function
 asyncio.run(main())
 ```
 
 For more detailed usage examples and API reference, please refer to the documentation.
 
+https://grommash9.github.io/aiotx/
+
 # Contributing
 Contributions to AioTx are welcome! If you find any bugs, have feature requests, or want to contribute improvements, please open an issue or submit a pull request on the GitHub repository.
 
 # License
 AioTx is open-source software licensed under the MIT License.
```

### Comparing `aiotx-0.5.0/aiotx.egg-info/SOURCES.txt` & `aiotx-0.5.1/aiotx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,36 +27,38 @@
 aiotx/utils/bep20_abi.json
 aiotx/utils/erc20_abi.json
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/monitoring.rst
-docs/clients/bsc_client/from_wei.rst
-docs/clients/bsc_client/generate_address.rst
-docs/clients/bsc_client/get_address_from_private_key.rst
-docs/clients/bsc_client/get_balance.rst
-docs/clients/bsc_client/get_block_by_number.rst
-docs/clients/bsc_client/get_gas_price.rst
-docs/clients/bsc_client/get_last_block.rst
-docs/clients/bsc_client/get_token_balance.rst
-docs/clients/bsc_client/get_transaction.rst
-docs/clients/bsc_client/get_transaction_count.rst
-docs/clients/bsc_client/index.rst
-docs/clients/bsc_client/send_token_transaction.rst
-docs/clients/bsc_client/send_transaction.rst
-docs/clients/bsc_client/to_wei.rst
-docs/clients/btc_client/from_wei.rst
-docs/clients/btc_client/generate_address.rst
-docs/clients/btc_client/index.rst
-docs/clients/btc_client/to_wei.rst
-docs/clients/eth_client/from_wei.rst
-docs/clients/eth_client/generate_address.rst
-docs/clients/eth_client/index.rst
-docs/clients/eth_client/to_wei.rst
+docs/testing.rst
+docs/clients/evm_client/from_wei.rst
+docs/clients/evm_client/generate_address.rst
+docs/clients/evm_client/get_address_from_private_key.rst
+docs/clients/evm_client/get_balance.rst
+docs/clients/evm_client/get_block_by_number.rst
+docs/clients/evm_client/get_contract_balance.rst
+docs/clients/evm_client/get_contract_decimals.rst
+docs/clients/evm_client/get_gas_price.rst
+docs/clients/evm_client/get_last_block.rst
+docs/clients/evm_client/get_transaction.rst
+docs/clients/evm_client/get_transaction_count.rst
+docs/clients/evm_client/index.rst
+docs/clients/evm_client/send.rst
+docs/clients/evm_client/send_token.rst
+docs/clients/evm_client/to_wei.rst
+docs/clients/tron_client/from_wei.rst
+docs/clients/tron_client/generate_address.rst
+docs/clients/tron_client/index.rst
+docs/clients/tron_client/to_wei.rst
+docs/clients/utxo_client/from_wei.rst
+docs/clients/utxo_client/generate_address.rst
+docs/clients/utxo_client/index.rst
+docs/clients/utxo_client/to_wei.rst
 examples/aiogram_notificator_bot.png
 examples/aiogram_notificator_bot.py
 examples/block_and_transactions_parser.py
 examples/two_block_parsers.py
 scripts/build_and_test.sh
 tests/conftest.py
 tests/test_bsc_client.py
```

### Comparing `aiotx-0.5.0/docs/Makefile` & `aiotx-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/docs/clients/bsc_client/get_balance.rst` & `aiotx-0.5.1/docs/clients/evm_client/get_balance.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 ===========
 
 .. code-block:: python
 
     async get_balance(address, block_parameter: BlockParam = BlockParam.LATEST) -> int
 
 
-Get the BSC balance of an address at a specific block.
+Get the balance of an address at a specific block.
 
 Parameters:
-    - address (str): The BSC address.
-    - block_parameter (BlockParam, optional): The block parameter (default is `BlockParam.LATEST`).
+    - **address** (str): The address.
+    - **block_parameter** (BlockParam, optional): The block parameter (default is `BlockParam.LATEST`).
 
 Returns:
-    int: The balance in wei.
+    - **int**: The balance in wei.
 
 Example usage:
 
 .. code-block:: python
 
-    balance = await bsc_client.get_balance("0x1234567890123456789012345678901234567890")
+    balance = await eth_client.get_balance(
+        "0x1234567890123456789012345678901234567890"
+        )
```

### Comparing `aiotx-0.5.0/docs/clients/bsc_client/get_transaction_count.rst` & `aiotx-0.5.1/docs/clients/evm_client/get_transaction_count.rst`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 
     async get_transaction_count(address, block_parameter: BlockParam = BlockParam.LATEST) -> int
 
 
 Get the number of transactions sent from an address at a specific block.
 
 Parameters:
-    - address (str): The BSC address.
-    - block_parameter (BlockParam, optional): The block parameter (default is `BlockParam.LATEST`).
+
+    - **address** (str): The address.
+    - **block_parameter** (BlockParam, optional): The block parameter (default is `BlockParam.LATEST`).
 
 Returns:
-    int: The transaction count.
+
+    - **int**: The transaction count.
 
 Example usage:
 
 .. code-block:: python
 
-    transaction_count = await bsc_client.get_transaction_count("0x1234567890123456789012345678901234567890")
+    transaction_count = await eth_client.get_transaction_count(
+        "0x1234567890123456789012345678901234567890"
+        )
```

### Comparing `aiotx-0.5.0/docs/conf.py` & `aiotx-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/docs/index.rst` & `aiotx-0.5.1/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 Welcome to AioTx's documentation!
 ==================================
 
 .. toctree::
    :maxdepth: 10
    :caption: Available Clients:
 
-   clients/bsc_client/index
-   clients/eth_client/index
-   clients/btc_client/index
+   clients/evm_client/index
+   clients/utxo_client/index
+   clients/tron_client/index
 
 .. toctree::
    :maxdepth: 10
    :caption: Monitoring:
 
    monitoring
 
+.. toctree::
+   :maxdepth: 10
+   :caption: Testing:
+
+   testing
+
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `aiotx-0.5.0/docs/make.bat` & `aiotx-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/docs/monitoring.rst` & `aiotx-0.5.1/docs/monitoring.rst`

 * *Files 17% similar despite different names*

```diff
@@ -48,31 +48,51 @@
 Monitoring Multiple Clients
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 You can monitor multiple AioTxBSCClient instances simultaneously by creating separate instances and registering handlers for each one. Here's an example:
 
 .. code-block:: python
 
-    client1 = AioTxBSCClient("NODE_URL", 97)
-    client2 = AioTxBSCClient("NODE_URL", 97)
+    from aiotx.clients import AioTxBSCClient, AioTxETHClient
+    import asyncio
 
-    @client1.monitor.on_block
-    def handle_block_client1(block):
-        print("Client 1 - Block:", block)
-
-    @client2.monitor.on_block
-    def handle_block_client2(block):
-        print("Client 2 - Block:", block)
+    bsc_client = AioTxBSCClient("NODE_URL", 97)
+    eth_client = AioTxETHClient("NODE_URL", 1151511)
+
+    @bsc_client.monitor.on_block
+    def handle_block(block):
+        print("bsc_client: block", block)
+
+    @bsc_client.monitor.on_transaction
+    def handle_transaction(transaction):
+        print("bsc_client: transaction", transaction)
+
+    @eth_client.monitor.on_block
+    def handle_block(block):
+        print("eth_client: block", block)
+
+    @eth_client.monitor.on_transaction
+    def handle_transaction(transaction):
+        print("eth_client: transaction", transaction)
 
     async def main():
-        monitoring_task1 = asyncio.create_task(client1.start_monitoring())
-        monitoring_task2 = asyncio.create_task(client2.start_monitoring())
-        await asyncio.gather(monitoring_task1, monitoring_task2)
+        bsc_task = asyncio.create_task(bsc_client.start_monitoring())
+        eth_task = asyncio.create_task(eth_client.start_monitoring())
+        await asyncio.gather(bsc_task, eth_task)
+
+        try:
+            while True:
+                await asyncio.sleep(1)
+        except KeyboardInterrupt:
+            bsc_client.stop_monitoring()
+            eth_client.stop_monitoring()
+
 
-    asyncio.run(main())
+    if __name__ == "__main__":
+        asyncio.run(main())
 
 Integration with Aiogram
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 You can integrate the monitoring functionality with the Aiogram library to send notifications or perform actions based on the received blocks and transactions. Here's an example:
 
 .. code-block:: python
```

### Comparing `aiotx-0.5.0/examples/aiogram_notificator_bot.png` & `aiotx-0.5.1/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/examples/aiogram_notificator_bot.py` & `aiotx-0.5.1/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/examples/block_and_transactions_parser.py` & `aiotx-0.5.1/examples/block_and_transactions_parser.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/setup.py` & `aiotx-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,18 @@
         "eth_utils",
         "eth_account"
     ],
     extras_require={
         "test": extras_test,
     },
     url="https://github.com/Grommash9/aiotx",
+    project_urls={
+        'Documentation': 'https://grommash9.github.io/aiotx/',
+        'Source': 'https://github.com/Grommash9/aiotx'
+        },
     author="Oleksandr Prudnikov",
     author_email="prudnikov21@icloud.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `aiotx-0.5.0/tests/conftest.py` & `aiotx-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_balance.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_gas_price.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_last_block.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_token_balance.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_transaction.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml` & `aiotx-0.5.1/tests/fixtures/cassettes/eth/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/test_bsc_client.py` & `aiotx-0.5.1/tests/test_bsc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/test_bsc_input_decoding.py` & `aiotx-0.5.1/tests/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/test_bsc_monitoring.py` & `aiotx-0.5.1/tests/test_bsc_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/test_eth_client.py` & `aiotx-0.5.1/tests/test_eth_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/test_eth_input_decoding.py` & `aiotx-0.5.1/tests/test_eth_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-0.5.0/tests/test_eth_monitoring.py` & `aiotx-0.5.1/tests/test_eth_monitoring.py`

 * *Files identical despite different names*

