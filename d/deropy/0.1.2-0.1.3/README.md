# Comparing `tmp/deropy-0.1.2.tar.gz` & `tmp/deropy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.1.2.tar", last modified: Fri May  3 14:06:05 2024, max compression
+gzip compressed data, was "deropy-0.1.3.tar", last modified: Sat May  4 18:45:33 2024, max compression
```

## Comparing `deropy-0.1.2.tar` & `deropy-0.1.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.174662 deropy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-03 14:05:59.000000 deropy-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-03 14:06:05.174662 deropy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-03 14:05:59.000000 deropy-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.162662 deropy-0.1.2/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.162662 deropy-0.1.2/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/commands/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.166662 deropy-0.1.2/deropy/dvm/
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/Smartcontract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/Wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.170662 deropy-0.1.2/deropy/dvm/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/AddressRaw.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/AddressString.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/AssetValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Atoi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Blid.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/BlockHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/BlockTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Dero.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/DeroValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/HexDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/IsAddressValid.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Itoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapDelete.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapExists.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapGet.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/MapStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Scid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/SendAssetToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/SendDeroToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Sha3256.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Store.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Strlen.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Substr.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/Txid.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/UpdateScCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/dvm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-03 14:05:59.000000 deropy-0.1.2/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.174662 deropy-0.1.2/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 14:06:05.000000 deropy-0.1.2/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:06:05.174662 deropy-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-03 14:05:59.000000 deropy-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:06:05.174662 deropy-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-03 14:05:59.000000 deropy-0.1.2/tests/test_compute_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-03 14:05:59.000000 deropy-0.1.2/tests/test_map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-03 14:05:59.000000 deropy-0.1.2/tests/test_storage_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.890357 deropy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-04 18:45:29.000000 deropy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-04 18:45:33.890357 deropy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-04 18:45:29.000000 deropy-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.882357 deropy-0.1.3/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.882357 deropy-0.1.3/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/commands/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.882357 deropy-0.1.3/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/Wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.890357 deropy-0.1.3/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-04 18:45:29.000000 deropy-0.1.3/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.890357 deropy-0.1.3/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-04 18:45:33.000000 deropy-0.1.3/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-04 18:45:33.000000 deropy-0.1.3/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:45:33.000000 deropy-0.1.3/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-04 18:45:33.000000 deropy-0.1.3/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-04 18:45:33.000000 deropy-0.1.3/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 18:45:33.000000 deropy-0.1.3/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:45:33.890357 deropy-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-04 18:45:29.000000 deropy-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:45:33.890357 deropy-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-04 18:45:29.000000 deropy-0.1.3/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-04 18:45:29.000000 deropy-0.1.3/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-04 18:45:29.000000 deropy-0.1.3/tests/test_storage_functions.py
```

### Comparing `deropy-0.1.2/LICENSE` & `deropy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/PKG-INFO` & `deropy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.1.2/README.md` & `deropy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/commands/configure.py` & `deropy-0.1.3/deropy/commands/configure.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/commands/deploy.py` & `deropy-0.1.3/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/commands/generate.py` & `deropy-0.1.3/deropy/commands/generate.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/Smartcontract.py` & `deropy-0.1.3/deropy/dvm/Smartcontract.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/Wallet.py` & `deropy-0.1.3/deropy/dvm/Wallet.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/AddressRaw.py` & `deropy-0.1.3/deropy/dvm/functions/AddressRaw.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/AddressString.py` & `deropy-0.1.3/deropy/dvm/functions/AddressString.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/AssetValue.py` & `deropy-0.1.3/deropy/dvm/functions/AssetValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Atoi.py` & `deropy-0.1.3/deropy/dvm/functions/Atoi.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/BlockHeight.py` & `deropy-0.1.3/deropy/dvm/functions/BlockHeight.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Dero.py` & `deropy-0.1.3/deropy/dvm/functions/Dero.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/DeroValue.py` & `deropy-0.1.3/deropy/dvm/functions/DeroValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Exists.py` & `deropy-0.1.3/deropy/dvm/functions/Exists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Function.py` & `deropy-0.1.3/deropy/dvm/functions/Function.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/IsAddressValid.py` & `deropy-0.1.3/deropy/dvm/functions/IsAddressValid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Itoa.py` & `deropy-0.1.3/deropy/dvm/functions/Itoa.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Keccak256.py` & `deropy-0.1.3/deropy/dvm/functions/Keccak256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Load.py` & `deropy-0.1.3/deropy/dvm/functions/Load.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/MapExists.py` & `deropy-0.1.3/deropy/dvm/functions/MapExists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/MapStore.py` & `deropy-0.1.3/deropy/dvm/functions/MapStore.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Random.py` & `deropy-0.1.3/deropy/dvm/functions/Random.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Scid.py` & `deropy-0.1.3/deropy/dvm/functions/Scid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/SendAssetToAddress.py` & `deropy-0.1.3/deropy/dvm/functions/SendAssetToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/SendDeroToAddress.py` & `deropy-0.1.3/deropy/dvm/functions/SendDeroToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Sha256.py` & `deropy-0.1.3/deropy/dvm/functions/Sha256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Sha3256.py` & `deropy-0.1.3/deropy/dvm/functions/Sha3256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Signer.py` & `deropy-0.1.3/deropy/dvm/functions/Signer.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Store.py` & `deropy-0.1.3/deropy/dvm/functions/Store.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/Substr.py` & `deropy-0.1.3/deropy/dvm/functions/Substr.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/UpdateScCode.py` & `deropy-0.1.3/deropy/dvm/functions/UpdateScCode.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/functions/__init__.py` & `deropy-0.1.3/deropy/dvm/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy/dvm/utils.py` & `deropy-0.1.3/deropy/dvm/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/deropy.egg-info/PKG-INFO` & `deropy-0.1.3/deropy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.1.2/deropy.egg-info/SOURCES.txt` & `deropy-0.1.3/deropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deropy-0.1.2/setup.py` & `deropy-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.1.2',
+    version=os.getenv('DEROPY_VERSION') or '0.1.3',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `deropy-0.1.2/tests/test_compute_storage.py` & `deropy-0.1.3/tests/test_compute_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,20 +42,20 @@
         {'args': {'key': '50char'}, 'expected': 0}],
     "MapExists": [{'args': {'key': 'key'}, 'expected': 0}],
     "MapStore": [{'args': {'key': 'key', 'value': 'n'}, 'expected': 0}],
     "MapGet": [{'args': {'key': 'key'}, 'expected': 0}],
     "MapDelete": [{'args': {'key': 'key'}, 'expected': 0}],
     "Random": [{'args': {'value': 10}, 'expected': 0}],
     "UpdateScCode": [{'args': {'sc_code': 'this is the new code'}, 'expected': 20*2}],
-    "SendDeroToAddress": [{'args': {'raw_address': '0x1234567890abcdef', 'amount': 100}, 'expected': 18}],
+    "SendDeroToAddress": [{'args': {'raw_address': WalletSimulator.get_raw_address_from_id('hyperbolic'), 'amount': 100}, 'expected': 33}],
     "SendAssetToAddress": [{'args': {
-            'raw_address': '0x1234567890abcdef',
+            'raw_address': WalletSimulator.get_raw_address_from_id('hyperbolic'),
             'asset': '0x1234567890abcdef',
             'amount': 100},
-        'expected': 18*2}],
+        'expected': 33}],
     "Signer": [{'args': {}, 'expected': 0}],
     "Sha256": [{'args': {'s': '0x1234567890abcdef'}, 'expected': 0}],
     "Sha3256": [{'args': {'s': '0x1234567890abcdef'}, 'expected': 0}],
     "Strlen": [{'args': {'s': '0x1234567890abcdef'}, 'expected': 0}],
     "Substr": [{'args': {'s': '0x1234567890abcdef', 'offset': 0, 'lenght': 5}, 'expected': 0}],
 
 }
```

### Comparing `deropy-0.1.2/tests/test_map_functions.py` & `deropy-0.1.3/tests/test_map_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,8 +56,8 @@
             map_get('key')
 
 
 class TestMapExists:
     def test_exists(self):
         map_store('key', 'value')
 
-        assert map_exists('key') is True
+        assert map_exists('key') == 1
```

### Comparing `deropy-0.1.2/tests/test_storage_functions.py` & `deropy-0.1.3/tests/test_storage_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,8 +54,8 @@
             load('key')
 
 
 class TestMapExists:
     def test_exists(self):
         store('key', 'value')
 
-        assert exists('key') is True
+        assert exists('key') == 1
```

