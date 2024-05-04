# Comparing `tmp/fs_attestation_safe_cli-1.0.2.tar.gz` & `tmp/fs_attestation_safe_cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_attestation_safe_cli-1.0.2.tar", last modified: Thu Apr 25 08:55:16 2024, max compression
+gzip compressed data, was "fs_attestation_safe_cli-1.0.3.tar", last modified: Fri May  3 11:50:57 2024, max compression
```

## Comparing `fs_attestation_safe_cli-1.0.2.tar` & `fs_attestation_safe_cli-1.0.3.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.612669 fs_attestation_safe_cli-1.0.2/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)     4099 2024-04-25 08:55:16.612970 fs_attestation_safe_cli-1.0.2/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     3243 2024-04-25 08:53:12.000000 fs_attestation_safe_cli-1.0.2/README.md
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.564170 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     4099 2024-04-25 08:55:16.000000 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     1901 2024-04-25 08:55:16.000000 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-04-25 08:55:16.000000 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)      105 2024-04-25 08:55:16.000000 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/entry_points.txt
--rw-r--r--   0 mohan      (501) staff       (20)      163 2024-04-25 08:55:16.000000 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)       15 2024-04-25 08:55:16.000000 fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.573712 fs_attestation_safe_cli-1.0.2/safe_cli/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/argparse_validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.575063 fs_attestation_safe_cli-1.0.2/safe_cli/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/contracts/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/contracts/safe_to_l2_migration.py
--rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     5829 2024-04-24 04:24:09.000000 fs_attestation_safe_cli-1.0.2/safe_cli/main.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.581187 fs_attestation_safe_cli-1.0.2/safe_cli/operators/
--rw-r--r--   0 mohan      (501) staff       (20)      204 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/exceptions.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.589244 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/hw_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/ledger_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/trezor_exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)    46527 2024-04-24 04:22:26.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/operators/safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19504 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/prompt_parser.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     9529 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/safe_completer_constants.py
--rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)     1313 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/safe_cli/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)       18 2024-04-25 08:54:50.000000 fs_attestation_safe_cli-1.0.2/safe_cli/version.py
--rw-r--r--   0 mohan      (501) staff       (20)      533 2024-04-25 08:55:16.613772 fs_attestation_safe_cli-1.0.2/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-04-25 06:49:01.000000 fs_attestation_safe_cli-1.0.2/setup.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.606419 fs_attestation_safe_cli-1.0.2/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 08:55:16.611607 fs_attestation_safe_cli-1.0.2/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/mocks/balances_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/mocks/data_decoded_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/mocks/multisig_tx_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/mocks/txs_mock.py
--rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/safe_cli_test_case_mixin.py
--rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_argparse_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_entrypoint.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_ethereum_hd_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_hw_wallet_manager.py
--rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_ledger_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_cli.py
--rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_completer.py
--rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_lexer.py
--rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_safe_tx_service_operator.py
--rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_trezor_wallet.py
--rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.2/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.152914 fs_attestation_safe_cli-1.0.3/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)     4099 2024-05-03 11:50:57.153059 fs_attestation_safe_cli-1.0.3/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     3243 2024-04-25 08:53:12.000000 fs_attestation_safe_cli-1.0.3/README.md
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.123332 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     4099 2024-05-03 11:50:57.000000 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     1997 2024-05-03 11:50:57.000000 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-03 11:50:57.000000 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-05-03 11:50:57.000000 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      163 2024-05-03 11:50:57.000000 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)       15 2024-05-03 11:50:57.000000 fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.130155 fs_attestation_safe_cli-1.0.3/safe_cli/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2085 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/argparse_validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.131321 fs_attestation_safe_cli-1.0.3/safe_cli/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)       75 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/contracts/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    28478 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/contracts/safe_to_l2_migration.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1262 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6435 2024-05-02 12:26:17.000000 fs_attestation_safe_cli-1.0.3/safe_cli/main.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.136480 fs_attestation_safe_cli-1.0.3/safe_cli/operators/
+-rw-r--r--   0 mohan      (501) staff       (20)      347 2024-05-02 12:28:51.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)       87 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2945 2024-05-02 12:26:43.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/fs_attestation_auth.py
+-rw-r--r--   0 mohan      (501) staff       (20)    12479 2024-05-03 11:29:16.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/fs_attestation_service_operator.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.140198 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)       98 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1925 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/hw_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7501 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1081 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/ledger_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2555 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1092 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/trezor_exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4527 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)    46367 2024-05-02 12:26:33.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18731 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/operators/safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    24053 2024-05-03 11:26:34.000000 fs_attestation_safe_cli-1.0.3/safe_cli/prompt_parser.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1824 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10873 2024-05-03 11:30:32.000000 fs_attestation_safe_cli-1.0.3/safe_cli/safe_completer_constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7416 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1536 2024-05-03 11:27:04.000000 fs_attestation_safe_cli-1.0.3/safe_cli/safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3329 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/safe_cli/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)       17 2024-05-03 11:50:09.000000 fs_attestation_safe_cli-1.0.3/safe_cli/version.py
+-rw-r--r--   0 mohan      (501) staff       (20)      533 2024-05-03 11:50:57.153526 fs_attestation_safe_cli-1.0.3/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)     1577 2024-04-25 06:49:01.000000 fs_attestation_safe_cli-1.0.3/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.148813 fs_attestation_safe_cli-1.0.3/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-03 11:50:57.152239 fs_attestation_safe_cli-1.0.3/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7755 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/mocks/balances_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2161 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/mocks/data_decoded_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2275 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/mocks/multisig_tx_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4217 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/mocks/txs_mock.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1980 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/safe_cli_test_case_mixin.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2335 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_argparse_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4030 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_entrypoint.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_ethereum_hd_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8216 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_hw_wallet_manager.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8870 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_ledger_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2309 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3051 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_cli.py
+-rw-r--r--   0 mohan      (501) staff       (20)      753 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_completer.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1644 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)      577 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_lexer.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21356 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)    19108 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_safe_tx_service_operator.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9113 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_trezor_wallet.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2050 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1172 2024-04-23 08:41:36.000000 fs_attestation_safe_cli-1.0.3/tests/utils.py
```

### Comparing `fs_attestation_safe_cli-1.0.2/LICENSE` & `fs_attestation_safe_cli-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/PKG-INFO` & `fs_attestation_safe_cli-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs_attestation_safe_cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.2/README.md` & `fs_attestation_safe_cli-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/PKG-INFO` & `fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Modified Command Line Interface for FailSafe Attestation Service to administrate Gnosis Safe Wallets and FailSafe Attestation Guard Contracts
 Home-page: https://github.com/gnosis/safe-cli
 Download-URL: https://github.com/gnosis/safe-cli/releases
 Author: Mohan
 Author-email: mohan@ethlas.com
 License: MIT
 Classifier: Programming Language :: Python
```

### Comparing `fs_attestation_safe_cli-1.0.2/fs_attestation_safe_cli.egg-info/SOURCES.txt` & `fs_attestation_safe_cli-1.0.3/fs_attestation_safe_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 safe_cli/utils.py
 safe_cli/version.py
 safe_cli/contracts/__init__.py
 safe_cli/contracts/safe_to_l2_migration.py
 safe_cli/operators/__init__.py
 safe_cli/operators/enums.py
 safe_cli/operators/exceptions.py
+safe_cli/operators/fs_attestation_auth.py
+safe_cli/operators/fs_attestation_service_operator.py
 safe_cli/operators/safe_operator.py
 safe_cli/operators/safe_tx_service_operator.py
 safe_cli/operators/hw_wallets/__init__.py
 safe_cli/operators/hw_wallets/constants.py
 safe_cli/operators/hw_wallets/exceptions.py
 safe_cli/operators/hw_wallets/hw_wallet.py
 safe_cli/operators/hw_wallets/hw_wallet_manager.py
```

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/argparse_validators.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/contracts/safe_to_l2_migration.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/contracts/safe_to_l2_migration.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/main.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 #!/bin/env python3
 import argparse
 import os
 import sys
 from typing import Optional
 
-from art import text2art
+from art import text2art, tprint
 from eth_typing import ChecksumAddress
 from prompt_toolkit import HTML, PromptSession, print_formatted_text
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.lexers import PygmentsLexer
 
 from safe_cli.argparse_validators import check_ethereum_address
 from safe_cli.operators import (
     SafeOperator,
     SafeServiceNotAvailable,
     SafeTxServiceOperator,
+    FailSafeAttestationServiceOperator
 )
 from safe_cli.prompt_parser import PromptParser
 from safe_cli.safe_completer import SafeCompleter
 from safe_cli.safe_lexer import SafeLexer
 from safe_cli.utils import get_safe_from_owner
 
 from .version import version
 
 
 class SafeCli:
-    def __init__(self, safe_address: ChecksumAddress, node_url: str, safe_tx_service_base_url: str, history: bool):
+    def __init__(self, safe_address: ChecksumAddress, node_url: str, safe_tx_service_base_url: str, fs_attestation_service_base_url: str, history: bool):
         """
         :param safe_address: Safe address
         :param node_url: Ethereum RPC url
         :param history: If `True` keep command history, otherwise history is not kept after closing the CLI
         """
         self.safe_address = safe_address
         self.node_url = node_url
+        self.fs_attestation_service_base_url = fs_attestation_service_base_url
         if history:
             self.session = PromptSession(
                 history=FileHistory(os.path.join(sys.path[0], ".history"))
             )
         else:
             self.session = PromptSession()
-        self.safe_operator = SafeOperator(safe_address, node_url, safe_tx_service_base_url)
-        self.prompt_parser = PromptParser(self.safe_operator)
+        self.safe_operator = SafeOperator(safe_address, node_url)
+        self.fs_attestation_service_operator = FailSafeAttestationServiceOperator(safe_address, node_url, safe_tx_service_base_url, fs_attestation_service_base_url)
+        self.prompt_parser = PromptParser(self.safe_operator, self.fs_attestation_service_operator)
 
     def print_startup_info(self):
+        print_formatted_text(tprint("FailSafe Attestation"))  # Print fancy text
         print_formatted_text(text2art("Safe CLI"))  # Print fancy text
         print_formatted_text(HTML(f"<b><ansigreen>Version {version}</ansigreen></b>"))
         print_formatted_text(
             HTML("<b><ansigreen>Loading Safe information...</ansigreen></b>")
         )
         self.safe_operator.print_info()
 
@@ -124,14 +128,15 @@
     parser.add_argument(
         "address",
         help="The address of the Safe, or an owner address if --get-safes-from-owner is specified.",
         type=check_ethereum_address,
     )
     parser.add_argument("node_url", help="Ethereum node url")
     parser.add_argument("safe_tx_service_base_url", help="Safe Transaction Service Base URL")
+    parser.add_argument("fs_attestation_service_base_url", help="FailSafe Attestation Service API Base URL")
     parser.add_argument(
         "--history",
         action="store_true",
         help="Enable history. By default it's disabled due to security reasons",
         default=False,
     )
     parser.add_argument(
@@ -142,20 +147,20 @@
     )
 
     args = parser.parse_args()
     if args.get_safes_from_owner:
         if (
             safe_address := get_safe_from_owner(args.address, args.node_url)
         ) is not None:
-            return SafeCli(safe_address, args.node_url, args.safe_tx_service_base_url, args.history)
+            return SafeCli(safe_address, args.node_url, args.safe_tx_service_base_url, args.fs_attestation_service_base_url, args.history)
     else:
-        return SafeCli(args.address, args.node_url, args.safe_tx_service_base_url, args.history)
+        return SafeCli(args.address, args.node_url, args.safe_tx_service_base_url, args.fs_attestation_service_base_url, args.history)
 
 
 def main(*args, **kwargs):
     safe_cli = build_safe_cli()
     safe_cli.print_startup_info()
     safe_cli.loop()
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/exceptions.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/hw_wallet.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/hw_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/ledger_exceptions.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/ledger_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/ledger_wallet.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/trezor_exceptions.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/trezor_exceptions.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/hw_wallets/trezor_wallet.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/hw_wallets/trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/safe_operator.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/safe_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,30 +142,28 @@
     safe_contract_1_1_0: Contract
     accounts: Set[LocalAccount] = set()
     default_sender: Optional[LocalAccount]
     executed_transactions: List[str]
     _safe_cli_info: Optional[SafeCliInfo]
     require_all_signatures: bool
 
-    def __init__(self, address: ChecksumAddress, node_url: str, safe_tx_service_base_url: str):
+    def __init__(self, address: ChecksumAddress, node_url: str):
         self.address = address
         self.node_url = node_url
-        self.safe_tx_service_base_url = safe_tx_service_base_url
         self.ethereum_client = EthereumClient(self.node_url)
         self.ens = ENS.from_web3(self.ethereum_client.w3)
         self.network: EthereumNetwork = self.ethereum_client.get_network()
         try:
             self.etherscan = EtherscanClient(self.network)
         except EtherscanClientConfigurationProblem:
             self.etherscan = None
 
         try:
-            self.safe_tx_service = TransactionServiceApi.from_custom_safe_tx_service_base_url(
-                self.ethereum_client,
-                self.safe_tx_service_base_url
+            self.safe_tx_service = TransactionServiceApi.from_ethereum_client(
+                self.ethereum_client
             )
         except EthereumNetworkNotSupported:
             self.safe_tx_service = None
 
         self.safe = Safe(address, self.ethereum_client)
         self.safe_contract = self.safe.contract
         self.safe_contract_1_1_0 = get_safe_V1_1_1_contract(
@@ -1182,8 +1180,8 @@
     def process_command(self, first_command: str, rest_command: List[str]) -> bool:
         if first_command == "help":
             print_formatted_text("I still cannot help you")
         elif first_command == "refresh":
             print_formatted_text("Reloading Safe information")
             self.refresh_safe_cli_info()
 
-        return False
+        return False
```

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/operators/safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/operators/safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/prompt_parser.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/prompt_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,30 @@
     SafeVersionNotSupportedException,
     SameFallbackHandlerException,
     SameMasterCopyException,
     SenderRequiredException,
     ThresholdLimitException,
 )
 from .operators.safe_operator import SafeOperator
+from .operators.fs_attestation_service_operator import FailSafeAttestationServiceOperator
+
+def parse_signers_ip_address_constraints(signers_ip_address_constraints_str: str) -> list:
+    """
+    Parse the signers IP address constraints
+    :param signers_ip_address_constraints:
+    :return: Parsed signers IP address constraints
+    """
+    signers_ip_address_constraints = []
+    for constraint in signers_ip_address_constraints_str.split(","):
+        signers_ip_address_constraint = {}
+        signer, ip_address = constraint.split(":")
+        signers_ip_address_constraint["wallet_address"] = signer
+        signers_ip_address_constraint["ip_address_range"] = ip_address
+        signers_ip_address_constraints.append(signers_ip_address_constraint)
+    return signers_ip_address_constraints
 
 
 def safe_exception(function):
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
         try:
             return function(*args, **kwargs)
@@ -134,28 +150,30 @@
         except SafeOperatorException as e:
             print_formatted_text(HTML(f"<ansired>{e.args[0]}</ansired>"))
 
     return wrapper
 
 
 class PromptParser:
-    def __init__(self, safe_operator: SafeOperator):
+    def __init__(self, safe_operator: SafeOperator, fs_attestation_service_operator: FailSafeAttestationServiceOperator):
         self.mode_parser = argparse.ArgumentParser(prog="")
         self.safe_operator = safe_operator
-        self.prompt_parser = build_prompt_parser(safe_operator)
+        self.fs_attestation_service_operator = fs_attestation_service_operator
+        self.prompt_parser = build_prompt_parser(safe_operator, fs_attestation_service_operator)
 
     def process_command(self, command: str):
         args = self.prompt_parser.parse_args(command.split())
         return args.func(args)
 
 
-def build_prompt_parser(safe_operator: SafeOperator) -> argparse.ArgumentParser:
+def build_prompt_parser(safe_operator: SafeOperator, fs_attestation_service_operator: FailSafeAttestationServiceOperator) -> argparse.ArgumentParser:
     """
     Returns an ArgParse capable of decoding and executing the Safe commands
-    :param safe_operator:
+    :param1 safe_operator:
+    :param2 fs_attestation_service_operator
     :return:
     """
     prompt_parser = argparse.ArgumentParser(prog="")
     subparsers = prompt_parser.add_subparsers()
 
     @safe_exception
     def show_cli_owners(args):
@@ -315,14 +333,35 @@
     def remove_delegate(args):
         safe_operator.remove_delegate(args.address, args.signer)
 
     @safe_exception
     def remove_proposed_transaction(args):
         safe_operator.remove_proposed_transaction(args.safe_tx_hash)
 
+    # Extension methods for FailSafe Attestation Service
+    @safe_exception
+    def fs_attestation_service_auth(args):
+        fs_attestation_service_operator.fs_attestation_user_login(args.safe_cli_owner, args.safe_cli_owner_private_key)
+
+    @safe_exception
+    def fs_attestation_service_enrolment(args):
+        fs_attestation_service_operator.fs_attestation_service_enrolment()
+
+    @safe_exception
+    def fs_attestation_service_deploy_guard_contract(args):
+        fs_attestation_service_operator.fs_attestation_service_deploy_guard_contract()
+
+    @safe_exception
+    def fs_attestation_service_set_constraints(args):
+        fs_attestation_service_operator.fs_attestation_service_set_constraints(args.signer_ip_address_constraints, args.expiry_time_constrint, args.risk_score_threshold_constraint)
+
+    @safe_exception
+    def fs_attestation_settings(args):
+        fs_attestation_service_operator.fs_attestation_settings(args.contact_email_address, args.slack_url)
+
     # Cli owners
     parser_show_cli_owners = subparsers.add_parser("show_cli_owners")
     parser_show_cli_owners.set_defaults(func=show_cli_owners)
 
     parser_load_cli_owners_from_words = subparsers.add_parser(
         "load_cli_owners_from_words"
     )
@@ -538,8 +577,59 @@
         "remove_proposed_transaction"
     )
     parser_remove_proposed_transaction.set_defaults(func=remove_proposed_transaction)
     parser_remove_proposed_transaction.add_argument(
         "safe_tx_hash", type=check_keccak256_hash
     )
 
-    return prompt_parser
+    # FailSafe Attestation Service Auth
+    parser_fs_attestation_service_auth = subparsers.add_parser(
+        "fs_attestation_service_auth"
+    )
+    parser_fs_attestation_service_auth.set_defaults(func=fs_attestation_service_auth)
+    parser_fs_attestation_service_auth.add_argument(
+        "safe_cli_owner", type=str
+    )
+    parser_fs_attestation_service_auth.add_argument(
+        "safe_cli_owner_private_key", type=str
+    )
+
+    # FailSafe Attestation Service Enrollment
+    parser_fs_attestation_service_enrolment = subparsers.add_parser(
+        "fs_attestation_service_enrolment"
+    )
+    parser_fs_attestation_service_enrolment.set_defaults(func=fs_attestation_service_enrolment)
+
+    # FailSafe Attestation Service Deploy Guard Contract
+    parser_fs_attestation_service_deploy_guard_contract = subparsers.add_parser(
+        "fs_attestation_service_deploy_guard_contract"
+    )
+    parser_fs_attestation_service_deploy_guard_contract.set_defaults(func=fs_attestation_service_deploy_guard_contract)
+
+    # FailSafe Attestation Service Set Constraints
+    parser_fs_attestation_service_set_constraints = subparsers.add_parser(
+        "fs_attestation_service_set_constraints"
+    )
+    parser_fs_attestation_service_set_constraints.set_defaults(func=fs_attestation_service_set_constraints)
+    parser_fs_attestation_service_set_constraints.add_argument(
+        "signer_ip_address_constraints", type=parse_signers_ip_address_constraints, help="Comma separated signer wallet address & IP address constraint: Example - 0x649D4d4cd5E09D02c9717EC51066A39FC843b744:172.21.0.8-172.21.0.30, 0x649D4d4cd5E09D02c9717EC51066A39FC843b745:172.21.1.8-172.21.2.30"
+    )
+    parser_fs_attestation_service_set_constraints.add_argument(
+        "expiry_time_constrint", type=int, help="Maximum duration in days within which all the signers should the sign the multi-sig transaction"
+    )
+    parser_fs_attestation_service_set_constraints.add_argument(
+        "risk_score_threshold_constraint", type=float, help="Maximum risk score threshold for a signer wallet address"
+    )
+
+    # FailSafe Attestation Service Settings
+    parser_fs_attestation_settings = subparsers.add_parser(
+        "fs_attestation_settings"
+    )
+    parser_fs_attestation_settings.set_defaults(func=fs_attestation_settings)
+    parser_fs_attestation_settings.add_argument(
+        "contact_email_address", type=str
+    )
+    parser_fs_attestation_settings.add_argument(
+        "slack_url", type=str
+    )
+
+    return prompt_parser
```

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/safe_addresses.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/safe_completer.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/safe_completer_constants.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/safe_completer_constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     "sign-tx": "<safe-tx-hash>",
     "unload_cli_owners": "<address> [<address>...]",
     "update": "",
     "update_version_to_l2": "<address>",
     "blockchain": "",
     "tx-service": "",
     "drain": "<address>",
+    "fs_attestation_service_enrolment": "",
+    "fs_attestation_service_auth": "<safe_cli_owner> <safe_cli_owner_private_key>",
+    "fs_attestation_service_deploy_guard_contract": "",
+    "fs_attestation_service_set_constraints": "<signer_wallet_address:ip_address_range> [<signer_wallet_address:ip_address_range>...] <multi_sig_tx_expiry_duration> <risk_score_threshold>",
+    "fs_attestation_settings": "<contact_email> <slack_web_hook_url>"
 }
 
 safe_commands = list(safe_commands_arguments.keys())
 
 safe_color_arguments = {
     "(read-only)": SAFE_ARGUMENT_COLOR,
     "<account-private-key>": SAFE_ARGUMENT_COLOR,
@@ -211,8 +216,23 @@
     "tx-service": HTML(
         "<b>tx-service</b> enables tx-service integration. Transactions will be sent to the tx-service "
         "instead of blockchain, so they will show up on the interface"
     ),
     "drain": HTML(
         "Command <b>drain</b> will try to send all assets ether and ERC20 to a check-summed account"
     ),
-}
+    "fs_attestation_service_auth": HTML(
+        "Performs authentication into FailSafe Attestation Service using one of the owners wallet address and private key"
+    ),
+    "fs_attestation_service_enrolment": HTML(
+        "Will enroll the current safe wallet address into FailSafe Attestation Service"
+    ),
+    "fs_attestation_service_deploy_guard_contract": HTML(
+        "Will deploy a FailSafe Attestation Service guard contract for the current safe wallet address"
+    ),
+    "fs_attestation_service_set_constraints": HTML(
+        "Will set the ip address range, multi-sig transaction expiry duration and risk score threshold constraints for the current safe wallet address"
+    ),
+    "fs_attestation_settings": HTML(
+        "Will update the additional settings FailSafe Attestation Service settings (contact emails and slack integrations, etc) for the current safe wallet address"
+    ),
+}
```

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/safe_creator.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/safe_lexer.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/safe_lexer.py`

 * *Files 27% similar despite different names*

```diff
@@ -29,14 +29,19 @@
         "change_master_copy",
         "add_delegate",
         "remove_delegate",
         "send_ether",
         "send_erc20",
         "send_erc721",
         "remove_proposed_transaction",
+        "fs_attestation_service_auth",
+        "fs_attestation_service_enrolment",
+        "fs_attestation_service_deploy_guard_contract",
+        "fs_attestation_service_set_constraints",
+        "fs_attestation_settings"
     }
 
     def get_tokens_unprocessed(self, text: str) -> (int, Token, str):
         for index, token, value in BashLexer.get_tokens_unprocessed(self, text):
             if token is Text and value in self.EXTRA_KEYWORDS:
                 yield index, Name.Builtin, value
             elif token is Text and re.search(self.ADDRESS, value):
```

### Comparing `fs_attestation_safe_cli-1.0.2/safe_cli/utils.py` & `fs_attestation_safe_cli-1.0.3/safe_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/setup.cfg` & `fs_attestation_safe_cli-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/setup.py` & `fs_attestation_safe_cli-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/mocks/balances_mock.py` & `fs_attestation_safe_cli-1.0.3/tests/mocks/balances_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/mocks/data_decoded_mock.py` & `fs_attestation_safe_cli-1.0.3/tests/mocks/data_decoded_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/mocks/multisig_tx_mock.py` & `fs_attestation_safe_cli-1.0.3/tests/mocks/multisig_tx_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/mocks/txs_mock.py` & `fs_attestation_safe_cli-1.0.3/tests/mocks/txs_mock.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/safe_cli_test_case_mixin.py` & `fs_attestation_safe_cli-1.0.3/tests/safe_cli_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_argparse_validators.py` & `fs_attestation_safe_cli-1.0.3/tests/test_argparse_validators.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_entrypoint.py` & `fs_attestation_safe_cli-1.0.3/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_ethereum_hd_wallet.py` & `fs_attestation_safe_cli-1.0.3/tests/test_ethereum_hd_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_hw_wallet_manager.py` & `fs_attestation_safe_cli-1.0.3/tests/test_hw_wallet_manager.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_ledger_wallet.py` & `fs_attestation_safe_cli-1.0.3/tests/test_ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_addresses.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_addresses.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_cli.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_cli.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_completer.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_completer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_creator.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_lexer.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_lexer.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_operator.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_safe_tx_service_operator.py` & `fs_attestation_safe_cli-1.0.3/tests/test_safe_tx_service_operator.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_trezor_wallet.py` & `fs_attestation_safe_cli-1.0.3/tests/test_trezor_wallet.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/test_utils.py` & `fs_attestation_safe_cli-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs_attestation_safe_cli-1.0.2/tests/utils.py` & `fs_attestation_safe_cli-1.0.3/tests/utils.py`

 * *Files identical despite different names*

