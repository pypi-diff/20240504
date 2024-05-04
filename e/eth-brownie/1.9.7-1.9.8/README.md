# Comparing `tmp/eth-brownie-1.9.7.tar.gz` & `tmp/eth-brownie-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eth-brownie-1.9.7.tar", last modified: Sun Jul  5 21:29:42 2020, max compression
+gzip compressed data, was "dist/eth-brownie-1.9.8.tar", last modified: Fri Jul 10 02:07:43 2020, max compression
```

## Comparing `eth-brownie-1.9.7.tar` & `eth-brownie-1.9.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/
--rw-rw-r--   0 computer  (1001) computer  (1001)     1076 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/LICENSE
--rw-rw-r--   0 computer  (1001) computer  (1001)      149 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/MANIFEST.in
--rw-rw-r--   0 computer  (1001) computer  (1001)     6482 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/PKG-INFO
--rw-rw-r--   0 computer  (1001) computer  (1001)     4678 2020-07-03 22:58:03.000000 eth-brownie-1.9.7/README.md
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/
--rw-rw-r--   0 computer  (1001) computer  (1001)      654 2020-06-12 07:17:42.000000 eth-brownie-1.9.7/brownie/__init__.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/_cli/
--rw-rw-r--   0 computer  (1001) computer  (1001)       19 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_cli/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     2240 2020-07-04 21:29:30.000000 eth-brownie-1.9.7/brownie/_cli/__main__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     4376 2020-04-26 17:15:32.000000 eth-brownie-1.9.7/brownie/_cli/accounts.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    14709 2020-06-20 09:37:18.000000 eth-brownie-1.9.7/brownie/_cli/analyze.py
--rw-rw-r--   0 computer  (1001) computer  (1001)      860 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_cli/bake.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     1253 2020-06-01 12:13:30.000000 eth-brownie-1.9.7/brownie/_cli/compile.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    12752 2020-05-23 16:18:42.000000 eth-brownie-1.9.7/brownie/_cli/console.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     7349 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_cli/ethpm.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     1318 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_cli/gui.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     1105 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_cli/init.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    11203 2020-05-23 13:40:27.000000 eth-brownie-1.9.7/brownie/_cli/networks.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     3966 2020-06-12 07:17:42.000000 eth-brownie-1.9.7/brownie/_cli/pm.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     2412 2020-07-03 22:58:03.000000 eth-brownie-1.9.7/brownie/_cli/run.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     2533 2020-07-05 21:09:28.000000 eth-brownie-1.9.7/brownie/_cli/test.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    10432 2020-07-05 21:28:26.000000 eth-brownie-1.9.7/brownie/_config.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/_gui/
--rwxrwxr-x   0 computer  (1001) computer  (1001)       64 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_gui/__init__.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     1270 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_gui/bases.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     1211 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_gui/console.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     7313 2020-06-12 07:17:42.000000 eth-brownie-1.9.7/brownie/_gui/opcodes.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     2260 2020-04-26 17:15:32.000000 eth-brownie-1.9.7/brownie/_gui/report.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     4669 2020-04-30 12:42:26.000000 eth-brownie-1.9.7/brownie/_gui/root.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     8643 2020-06-01 12:13:30.000000 eth-brownie-1.9.7/brownie/_gui/source.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     3496 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_gui/styles.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)      975 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_gui/tooltip.py
--rw-rw-r--   0 computer  (1001) computer  (1001)      325 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/_singleton.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/convert/
--rw-rw-r--   0 computer  (1001) computer  (1001)      215 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/convert/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    13203 2020-07-03 22:58:03.000000 eth-brownie-1.9.7/brownie/convert/datatypes.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     2354 2020-07-03 22:43:41.000000 eth-brownie-1.9.7/brownie/convert/main.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     4167 2020-05-23 17:29:28.000000 eth-brownie-1.9.7/brownie/convert/normalize.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     1527 2020-05-14 09:19:30.000000 eth-brownie-1.9.7/brownie/convert/utils.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/data/
--rw-rw-r--   0 computer  (1001) computer  (1001)     1393 2020-07-05 21:09:28.000000 eth-brownie-1.9.7/brownie/data/default-config.yaml
--rw-rw-r--   0 computer  (1001) computer  (1001)      378 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/data/ethpm-config.yaml
--rw-rw-r--   0 computer  (1001) computer  (1001)     1856 2020-07-05 17:52:14.000000 eth-brownie-1.9.7/brownie/data/network-config.yaml
--rw-rw-r--   0 computer  (1001) computer  (1001)     4984 2020-07-05 10:13:40.000000 eth-brownie-1.9.7/brownie/exceptions.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/network/
--rw-rw-r--   0 computer  (1001) computer  (1001)      431 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/network/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    20110 2020-07-05 19:54:08.000000 eth-brownie-1.9.7/brownie/network/account.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     4453 2020-06-05 18:01:40.000000 eth-brownie-1.9.7/brownie/network/alert.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    44812 2020-07-04 21:03:36.000000 eth-brownie-1.9.7/brownie/network/contract.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     8278 2020-06-04 09:01:45.000000 eth-brownie-1.9.7/brownie/network/event.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     4184 2020-06-02 12:19:17.000000 eth-brownie-1.9.7/brownie/network/main.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    15791 2020-07-04 21:48:34.000000 eth-brownie-1.9.7/brownie/network/rpc.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     5826 2020-06-12 07:17:42.000000 eth-brownie-1.9.7/brownie/network/state.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    38017 2020-07-05 19:54:08.000000 eth-brownie-1.9.7/brownie/network/transaction.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     6793 2020-06-08 11:49:06.000000 eth-brownie-1.9.7/brownie/network/web3.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.878831 eth-brownie-1.9.7/brownie/project/
--rw-rw-r--   0 computer  (1001) computer  (1001)      317 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/project/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     5192 2020-07-04 17:18:29.000000 eth-brownie-1.9.7/brownie/project/build.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/brownie/project/compiler/
--rw-rw-r--   0 computer  (1001) computer  (1001)    15636 2020-06-03 16:59:20.000000 eth-brownie-1.9.7/brownie/project/compiler/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    23875 2020-06-25 09:02:13.000000 eth-brownie-1.9.7/brownie/project/compiler/solidity.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     1619 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/project/compiler/utils.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     7482 2020-07-04 21:48:34.000000 eth-brownie-1.9.7/brownie/project/compiler/vyper.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    26058 2020-06-08 11:49:06.000000 eth-brownie-1.9.7/brownie/project/ethpm.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    32616 2020-06-20 09:37:18.000000 eth-brownie-1.9.7/brownie/project/main.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     3966 2020-06-01 12:13:30.000000 eth-brownie-1.9.7/brownie/project/scripts.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     7246 2020-06-12 07:17:42.000000 eth-brownie-1.9.7/brownie/project/sources.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/brownie/test/
--rw-rw-r--   0 computer  (1001) computer  (1001)     2299 2020-06-04 16:08:36.000000 eth-brownie-1.9.7/brownie/test/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     2998 2020-06-19 06:53:58.000000 eth-brownie-1.9.7/brownie/test/coverage.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     4486 2020-05-14 15:39:32.000000 eth-brownie-1.9.7/brownie/test/fixtures.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/brownie/test/managers/
--rw-rw-r--   0 computer  (1001) computer  (1001)      152 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/test/managers/__init__.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     9963 2020-06-08 17:09:47.000000 eth-brownie-1.9.7/brownie/test/managers/base.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     2868 2020-06-08 08:47:02.000000 eth-brownie-1.9.7/brownie/test/managers/master.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    16947 2020-07-04 21:03:36.000000 eth-brownie-1.9.7/brownie/test/managers/runner.py
--rw-rw-r--   0 computer  (1001) computer  (1001)      275 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/test/managers/utils.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    11087 2020-06-08 17:09:47.000000 eth-brownie-1.9.7/brownie/test/output.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     3861 2020-07-05 21:09:28.000000 eth-brownie-1.9.7/brownie/test/plugin.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     3452 2020-06-04 09:01:45.000000 eth-brownie-1.9.7/brownie/test/stateful.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     6698 2020-06-05 07:27:26.000000 eth-brownie-1.9.7/brownie/test/strategies.py
--rw-rw-r--   0 computer  (1001) computer  (1001)      309 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/typing.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/brownie/utils/
--rw-rw-r--   0 computer  (1001) computer  (1001)       82 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/utils/__init__.py
--rwxrwxr-x   0 computer  (1001) computer  (1001)     5239 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/utils/color.py
--rw-rw-r--   0 computer  (1001) computer  (1001)    33852 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/utils/docopt.py
--rw-rw-r--   0 computer  (1001) computer  (1001)     1227 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/brownie/utils/sql.py
-drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/eth_brownie.egg-info/
--rw-rw-r--   0 computer  (1001) computer  (1001)     6482 2020-07-05 21:29:42.000000 eth-brownie-1.9.7/eth_brownie.egg-info/PKG-INFO
--rw-rw-r--   0 computer  (1001) computer  (1001)     2134 2020-07-05 21:29:42.000000 eth-brownie-1.9.7/eth_brownie.egg-info/SOURCES.txt
--rw-rw-r--   0 computer  (1001) computer  (1001)        1 2020-07-05 21:29:42.000000 eth-brownie-1.9.7/eth_brownie.egg-info/dependency_links.txt
--rw-rw-r--   0 computer  (1001) computer  (1001)      105 2020-07-05 21:29:42.000000 eth-brownie-1.9.7/eth_brownie.egg-info/entry_points.txt
--rw-rw-r--   0 computer  (1001) computer  (1001)      472 2020-07-05 21:29:42.000000 eth-brownie-1.9.7/eth_brownie.egg-info/requires.txt
--rw-rw-r--   0 computer  (1001) computer  (1001)        8 2020-07-05 21:29:42.000000 eth-brownie-1.9.7/eth_brownie.egg-info/top_level.txt
--rw-rw-r--   0 computer  (1001) computer  (1001)      534 2020-04-24 10:30:06.000000 eth-brownie-1.9.7/pyproject.toml
--rw-rw-r--   0 computer  (1001) computer  (1001)      466 2020-07-05 21:09:28.000000 eth-brownie-1.9.7/requirements.txt
--rw-rw-r--   0 computer  (1001) computer  (1001)      890 2020-07-05 21:29:42.882831 eth-brownie-1.9.7/setup.cfg
--rw-rw-r--   0 computer  (1001) computer  (1001)     1417 2020-07-05 21:28:26.000000 eth-brownie-1.9.7/setup.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1076 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/LICENSE
+-rw-rw-r--   0 computer  (1001) computer  (1001)      149 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/MANIFEST.in
+-rw-rw-r--   0 computer  (1001) computer  (1001)     6482 2020-07-10 02:07:43.028927 eth-brownie-1.9.8/PKG-INFO
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4678 2020-07-03 22:58:03.000000 eth-brownie-1.9.8/README.md
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.020927 eth-brownie-1.9.8/brownie/
+-rw-rw-r--   0 computer  (1001) computer  (1001)      654 2020-06-12 07:17:42.000000 eth-brownie-1.9.8/brownie/__init__.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.020927 eth-brownie-1.9.8/brownie/_cli/
+-rw-rw-r--   0 computer  (1001) computer  (1001)       19 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_cli/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2240 2020-07-04 21:29:30.000000 eth-brownie-1.9.8/brownie/_cli/__main__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4376 2020-04-26 17:15:32.000000 eth-brownie-1.9.8/brownie/_cli/accounts.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    14709 2020-06-20 09:37:18.000000 eth-brownie-1.9.8/brownie/_cli/analyze.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)      860 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_cli/bake.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1253 2020-07-06 09:40:13.000000 eth-brownie-1.9.8/brownie/_cli/compile.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    12174 2020-07-08 06:12:17.000000 eth-brownie-1.9.8/brownie/_cli/console.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     7349 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_cli/ethpm.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1318 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_cli/gui.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1105 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_cli/init.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    11203 2020-05-23 13:40:27.000000 eth-brownie-1.9.8/brownie/_cli/networks.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     3966 2020-06-12 07:17:42.000000 eth-brownie-1.9.8/brownie/_cli/pm.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2412 2020-07-03 22:58:03.000000 eth-brownie-1.9.8/brownie/_cli/run.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2533 2020-07-05 21:09:28.000000 eth-brownie-1.9.8/brownie/_cli/test.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    10432 2020-07-10 02:05:42.000000 eth-brownie-1.9.8/brownie/_config.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.020927 eth-brownie-1.9.8/brownie/_gui/
+-rwxrwxr-x   0 computer  (1001) computer  (1001)       64 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_gui/__init__.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     1270 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_gui/bases.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     1211 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_gui/console.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     7313 2020-06-12 07:17:42.000000 eth-brownie-1.9.8/brownie/_gui/opcodes.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     2260 2020-04-26 17:15:32.000000 eth-brownie-1.9.8/brownie/_gui/report.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     4669 2020-04-30 12:42:26.000000 eth-brownie-1.9.8/brownie/_gui/root.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     8643 2020-06-01 12:13:30.000000 eth-brownie-1.9.8/brownie/_gui/source.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     3496 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_gui/styles.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)      975 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_gui/tooltip.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)      325 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/_singleton.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.020927 eth-brownie-1.9.8/brownie/convert/
+-rw-rw-r--   0 computer  (1001) computer  (1001)      215 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/convert/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    13203 2020-07-03 22:58:03.000000 eth-brownie-1.9.8/brownie/convert/datatypes.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2354 2020-07-03 22:43:41.000000 eth-brownie-1.9.8/brownie/convert/main.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4167 2020-05-23 17:29:28.000000 eth-brownie-1.9.8/brownie/convert/normalize.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1527 2020-05-14 09:19:30.000000 eth-brownie-1.9.8/brownie/convert/utils.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.020927 eth-brownie-1.9.8/brownie/data/
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1393 2020-07-05 21:09:28.000000 eth-brownie-1.9.8/brownie/data/default-config.yaml
+-rw-rw-r--   0 computer  (1001) computer  (1001)      378 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/data/ethpm-config.yaml
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1856 2020-07-05 17:52:14.000000 eth-brownie-1.9.8/brownie/data/network-config.yaml
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4984 2020-07-05 10:13:40.000000 eth-brownie-1.9.8/brownie/exceptions.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/brownie/network/
+-rw-rw-r--   0 computer  (1001) computer  (1001)      431 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/network/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    20110 2020-07-05 19:54:08.000000 eth-brownie-1.9.8/brownie/network/account.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4453 2020-06-05 18:01:40.000000 eth-brownie-1.9.8/brownie/network/alert.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    44917 2020-07-09 12:10:19.000000 eth-brownie-1.9.8/brownie/network/contract.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     8278 2020-06-04 09:01:45.000000 eth-brownie-1.9.8/brownie/network/event.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4184 2020-06-02 12:19:17.000000 eth-brownie-1.9.8/brownie/network/main.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    15791 2020-07-04 21:48:34.000000 eth-brownie-1.9.8/brownie/network/rpc.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     5826 2020-06-12 07:17:42.000000 eth-brownie-1.9.8/brownie/network/state.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    37627 2020-07-09 12:10:19.000000 eth-brownie-1.9.8/brownie/network/transaction.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     6793 2020-06-08 11:49:06.000000 eth-brownie-1.9.8/brownie/network/web3.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/brownie/project/
+-rw-rw-r--   0 computer  (1001) computer  (1001)      317 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/project/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     5192 2020-07-04 17:18:29.000000 eth-brownie-1.9.8/brownie/project/build.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/brownie/project/compiler/
+-rw-rw-r--   0 computer  (1001) computer  (1001)    15636 2020-06-03 16:59:20.000000 eth-brownie-1.9.8/brownie/project/compiler/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    24238 2020-07-09 20:17:25.000000 eth-brownie-1.9.8/brownie/project/compiler/solidity.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1619 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/project/compiler/utils.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     7482 2020-07-07 10:19:07.000000 eth-brownie-1.9.8/brownie/project/compiler/vyper.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    26058 2020-06-08 11:49:06.000000 eth-brownie-1.9.8/brownie/project/ethpm.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    33050 2020-07-08 07:16:47.000000 eth-brownie-1.9.8/brownie/project/main.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     3966 2020-06-01 12:13:30.000000 eth-brownie-1.9.8/brownie/project/scripts.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     7246 2020-06-12 07:17:42.000000 eth-brownie-1.9.8/brownie/project/sources.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/brownie/test/
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2299 2020-06-04 16:08:36.000000 eth-brownie-1.9.8/brownie/test/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2998 2020-06-19 06:53:58.000000 eth-brownie-1.9.8/brownie/test/coverage.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     4486 2020-05-14 15:39:32.000000 eth-brownie-1.9.8/brownie/test/fixtures.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/brownie/test/managers/
+-rw-rw-r--   0 computer  (1001) computer  (1001)      152 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/test/managers/__init__.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     9963 2020-06-08 17:09:47.000000 eth-brownie-1.9.8/brownie/test/managers/base.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2868 2020-06-08 08:47:02.000000 eth-brownie-1.9.8/brownie/test/managers/master.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    16947 2020-07-04 21:03:36.000000 eth-brownie-1.9.8/brownie/test/managers/runner.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)      275 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/test/managers/utils.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    11087 2020-06-08 17:09:47.000000 eth-brownie-1.9.8/brownie/test/output.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     3861 2020-07-09 12:09:04.000000 eth-brownie-1.9.8/brownie/test/plugin.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     3452 2020-06-04 09:01:45.000000 eth-brownie-1.9.8/brownie/test/stateful.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     6698 2020-06-05 07:27:26.000000 eth-brownie-1.9.8/brownie/test/strategies.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)      309 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/typing.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/brownie/utils/
+-rw-rw-r--   0 computer  (1001) computer  (1001)       82 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/utils/__init__.py
+-rwxrwxr-x   0 computer  (1001) computer  (1001)     6479 2020-07-09 14:24:32.000000 eth-brownie-1.9.8/brownie/utils/color.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)    33852 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/utils/docopt.py
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1227 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/brownie/utils/sql.py
+drwxrwxr-x   0 computer  (1001) computer  (1001)        0 2020-07-10 02:07:43.024927 eth-brownie-1.9.8/eth_brownie.egg-info/
+-rw-rw-r--   0 computer  (1001) computer  (1001)     6482 2020-07-10 02:07:42.000000 eth-brownie-1.9.8/eth_brownie.egg-info/PKG-INFO
+-rw-rw-r--   0 computer  (1001) computer  (1001)     2134 2020-07-10 02:07:42.000000 eth-brownie-1.9.8/eth_brownie.egg-info/SOURCES.txt
+-rw-rw-r--   0 computer  (1001) computer  (1001)        1 2020-07-10 02:07:42.000000 eth-brownie-1.9.8/eth_brownie.egg-info/dependency_links.txt
+-rw-rw-r--   0 computer  (1001) computer  (1001)      105 2020-07-10 02:07:42.000000 eth-brownie-1.9.8/eth_brownie.egg-info/entry_points.txt
+-rw-rw-r--   0 computer  (1001) computer  (1001)      503 2020-07-10 02:07:42.000000 eth-brownie-1.9.8/eth_brownie.egg-info/requires.txt
+-rw-rw-r--   0 computer  (1001) computer  (1001)        8 2020-07-10 02:07:42.000000 eth-brownie-1.9.8/eth_brownie.egg-info/top_level.txt
+-rw-rw-r--   0 computer  (1001) computer  (1001)      534 2020-04-24 10:30:06.000000 eth-brownie-1.9.8/pyproject.toml
+-rw-rw-r--   0 computer  (1001) computer  (1001)      497 2020-07-09 14:24:32.000000 eth-brownie-1.9.8/requirements.txt
+-rw-rw-r--   0 computer  (1001) computer  (1001)      914 2020-07-10 02:07:43.028927 eth-brownie-1.9.8/setup.cfg
+-rw-rw-r--   0 computer  (1001) computer  (1001)     1417 2020-07-10 02:05:42.000000 eth-brownie-1.9.8/setup.py
```

### Comparing `eth-brownie-1.9.7/LICENSE` & `eth-brownie-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/PKG-INFO` & `eth-brownie-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-brownie
-Version: 1.9.7
+Version: 1.9.8
 Summary: A Python framework for Ethereum smart contract deployment, testing and interaction.
 Home-page: https://github.com/eth-brownie/brownie
 Author: Ben Hauser
 Author-email: ben@hauser.id
 License: MIT
 Description: # Brownie
```

### Comparing `eth-brownie-1.9.7/README.md` & `eth-brownie-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/__init__.py` & `eth-brownie-1.9.8/brownie/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/__main__.py` & `eth-brownie-1.9.8/brownie/_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/accounts.py` & `eth-brownie-1.9.8/brownie/_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/analyze.py` & `eth-brownie-1.9.8/brownie/_cli/analyze.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/bake.py` & `eth-brownie-1.9.8/brownie/_cli/bake.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/compile.py` & `eth-brownie-1.9.8/brownie/_cli/compile.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/console.py` & `eth-brownie-1.9.8/brownie/_cli/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from prompt_toolkit.auto_suggest import AutoSuggest, Suggestion
 from prompt_toolkit.completion import Completer, Completion
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.lexers import PygmentsLexer
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
-from pygments import highlight
-from pygments.formatters import get_formatter_by_name
 from pygments.lexers import PythonLexer
 from pygments.styles import get_style_by_name
 
 import brownie
 from brownie import network, project
 from brownie._config import CONFIG, _get_data_folder, _update_argv_from_docopt
 from brownie.utils import color
@@ -105,28 +103,14 @@
             locals_dict["Gui"] = Gui
         except ModuleNotFoundError:
             pass
 
         if extra_locals:
             locals_dict.update(extra_locals)
 
-        # prepare lexer and formatter
-        self.lexer = PythonLexer()
-        fmt_name = "terminal"
-        try:
-            import curses
-
-            curses.setupterm()
-            if curses.tigetnum("colors") == 256:
-                fmt_name = "terminal256"
-        except Exception:
-            # if curses won't import we are probably using Windows
-            pass
-        self.formatter = get_formatter_by_name(fmt_name, style=console_settings["color_style"])
-
         # create prompt session object
         history_file = str(_get_data_folder().joinpath(".history").absolute())
         kwargs = {}
         if console_settings["show_colors"]:
             kwargs.update(
                 lexer=PygmentsLexer(PythonLexer),
                 style=style_from_pygments_cls(get_style_by_name(console_settings["color_style"])),
@@ -180,15 +164,15 @@
             if obj and isinstance(obj, dict):
                 text = color.pretty_dict(obj)
             elif obj and isinstance(obj, (tuple, list, set)):
                 text = color.pretty_sequence(obj)
         except (SyntaxError, NameError):
             pass
         if CONFIG.settings["console"]["show_colors"]:
-            text = highlight(text, self.lexer, self.formatter)
+            text = color.highlight(text)
         self.write(text)
 
     def raw_input(self, prompt=""):
         return self.prompt_session.prompt(prompt)
 
     def paste_event(self, event):
         data = event.data
```

### Comparing `eth-brownie-1.9.7/brownie/_cli/ethpm.py` & `eth-brownie-1.9.8/brownie/_cli/ethpm.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/gui.py` & `eth-brownie-1.9.8/brownie/_cli/gui.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/init.py` & `eth-brownie-1.9.8/brownie/_cli/init.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/networks.py` & `eth-brownie-1.9.8/brownie/_cli/networks.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/pm.py` & `eth-brownie-1.9.8/brownie/_cli/pm.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/run.py` & `eth-brownie-1.9.8/brownie/_cli/run.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_cli/test.py` & `eth-brownie-1.9.8/brownie/_cli/test.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_config.py` & `eth-brownie-1.9.8/brownie/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import yaml
 from hypothesis import Phase
 from hypothesis import settings as hp_settings
 from hypothesis.database import DirectoryBasedExampleDatabase
 
 from brownie._singleton import _Singleton
 
-__version__ = "1.9.7"
+__version__ = "1.9.8"
 
 BROWNIE_FOLDER = Path(__file__).parent
 DATA_FOLDER = Path.home().joinpath(".brownie")
 
 DATA_SUBFOLDERS = ("accounts", "ethpm", "packages")
 
 EVM_EQUIVALENTS = {"atlantis": "byzantium", "agharta": "petersburg"}
```

### Comparing `eth-brownie-1.9.7/brownie/_gui/bases.py` & `eth-brownie-1.9.8/brownie/_gui/bases.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/console.py` & `eth-brownie-1.9.8/brownie/_gui/console.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/opcodes.py` & `eth-brownie-1.9.8/brownie/_gui/opcodes.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/report.py` & `eth-brownie-1.9.8/brownie/_gui/report.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/root.py` & `eth-brownie-1.9.8/brownie/_gui/root.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/source.py` & `eth-brownie-1.9.8/brownie/_gui/source.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/styles.py` & `eth-brownie-1.9.8/brownie/_gui/styles.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/_gui/tooltip.py` & `eth-brownie-1.9.8/brownie/_gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/convert/datatypes.py` & `eth-brownie-1.9.8/brownie/convert/datatypes.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/convert/main.py` & `eth-brownie-1.9.8/brownie/convert/main.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/convert/normalize.py` & `eth-brownie-1.9.8/brownie/convert/normalize.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/convert/utils.py` & `eth-brownie-1.9.8/brownie/convert/utils.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/data/default-config.yaml` & `eth-brownie-1.9.8/brownie/data/default-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/data/network-config.yaml` & `eth-brownie-1.9.8/brownie/data/network-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/exceptions.py` & `eth-brownie-1.9.8/brownie/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/account.py` & `eth-brownie-1.9.8/brownie/network/account.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/alert.py` & `eth-brownie-1.9.8/brownie/network/alert.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/contract.py` & `eth-brownie-1.9.8/brownie/network/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         if CONFIG.network_type == "live":
             _add_deployment(contract)
 
         return contract
 
     def _add_from_tx(self, tx: TransactionReceiptType) -> None:
         tx._confirmed.wait()
-        if tx.status:
+        if tx.status and tx.contract_address is not None:
             try:
                 self.at(tx.contract_address, tx.sender, tx)
             except ContractNotFound:
                 # if the contract self-destructed during deployment
                 pass
 
 
@@ -641,14 +641,17 @@
                 "Some functionality will not be available.",
                 BrownieCompilerWarning,
             )
 
         if as_proxy_for is None and data["result"][0].get("Implementation"):
             as_proxy_for = _resolve_address(data["result"][0]["Implementation"])
 
+        if as_proxy_for == address:
+            as_proxy_for = None
+
         # if this is a proxy, fetch information for the implementation contract
         if as_proxy_for is not None:
             implementation_contract = Contract.from_explorer(as_proxy_for)
             abi = implementation_contract._build["abi"]
 
         if not is_verified:
             return cls.from_abi(name, address, abi, owner)
```

### Comparing `eth-brownie-1.9.7/brownie/network/event.py` & `eth-brownie-1.9.8/brownie/network/event.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/main.py` & `eth-brownie-1.9.8/brownie/network/main.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/rpc.py` & `eth-brownie-1.9.8/brownie/network/rpc.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/state.py` & `eth-brownie-1.9.8/brownie/network/state.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/network/transaction.py` & `eth-brownie-1.9.8/brownie/network/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 def trace_property(fn: Callable) -> Any:
     # attributes that are only available after querying the tranasaction trace
 
     @property  # type: ignore
     def wrapper(self: "TransactionReceipt") -> Any:
         if self.status == -1:
             return None
+        if self._trace_exc is not None:
+            raise self._trace_exc
         return fn(self)
 
     return wrapper
 
 
 def trace_inspection(fn: Callable) -> Any:
     def wrapper(self: "TransactionReceipt", *args: Any, **kwargs: Any) -> Any:
@@ -86,47 +88,14 @@
 
         events: Decoded transaction log events
         trace: Expanded stack trace from debug_traceTransaction
         return_value: Return value(s) from contract call
         revert_msg: Error string from reverted contract all
         modified_state: Boolean, did this contract write to storage?"""
 
-    __slots__ = (
-        "_call_cost",
-        "_confirmed",
-        "_events",
-        "_internal_transfers",
-        "_modified_state",
-        "_new_contracts",
-        "_raw_trace",
-        "_return_value",
-        "_revert_msg",
-        "_revert_pc",
-        "_silent",
-        "_trace",
-        "_trace_origin",
-        "block_number",
-        "contract_address",
-        "contract_name",
-        "coverage_hash",
-        "fn_name",
-        "gas_limit",
-        "gas_price",
-        "gas_used",
-        "input",
-        "logs",
-        "nonce",
-        "receiver",
-        "sender",
-        "status",
-        "txid",
-        "txindex",
-        "value",
-    )
-
     def __init__(
         self,
         txid: Union[str, bytes],
         sender: Any = None,
         silent: bool = True,
         required_confs: int = 1,
         name: str = "",
@@ -147,29 +116,41 @@
         if CONFIG.mode == "test":
             self._silent = True
         if isinstance(txid, bytes):
             txid = txid.hex()
         if not self._silent:
             print(f"Transaction sent: {color('bright blue')}{txid}{color}")
 
+        # internal attributes
+        self._trace_exc = None
         self._trace_origin = None
         self._raw_trace = None
         self._trace = None
         self._call_cost = 0
         self._events = None
         self._return_value = None
         self._revert_msg = None
         self._modified_state = None
         self._new_contracts = None
         self._internal_transfers = None
         self._confirmed = threading.Event()
 
+        # attributes that cannot be set until the tx confirms
+        self.block_number = None
+        self.contract_address: Optional[str] = None
+        self.gas_used = None
+        self.logs = None
+        self.nonce = None
+        self.txindex = None
+
+        # attributes that can be set immediately
         self.sender = sender
         self.status = -1
         self.txid = txid
+        self.contract_name = None
         self.fn_name = name
 
         if name and "." in name:
             self.contract_name, self.fn_name = name.split(".", maxsplit=1)
 
         # avoid querying the trace to get the revert string if possible
         self._revert_msg, self._revert_pc, revert_type = revert_data or (None, None, None)
@@ -189,20 +170,14 @@
     def __repr__(self) -> str:
         c = {-1: "bright yellow", 0: "bright red", 1: None}
         return f"<Transaction '{color(c[self.status])}{self.txid}{color}'>"
 
     def __hash__(self) -> int:
         return hash(self.txid)
 
-    def __getattr__(self, attr: str) -> Any:
-        if attr not in self.__slots__:
-            raise AttributeError(f"'TransactionReceipt' object has no attribute '{attr}'")
-        if self.status == -1:
-            return None
-
     @trace_property
     def events(self) -> Optional[List]:
         if not self.status:
             self._get_trace()
         return self._events
 
     @trace_property
@@ -325,15 +300,15 @@
                     f"{required_confs}{color}"
                 )
                 sys.stdout.flush()
 
         # await first confirmation
         receipt = web3.eth.waitForTransactionReceipt(self.txid, timeout=None, poll_latency=0.5)
 
-        self.block_number: Optional[int] = receipt["blockNumber"]
+        self.block_number = receipt["blockNumber"]
         # wait for more confirmations if required and handle uncle blocks
         remaining_confs = required_confs
         while remaining_confs > 0 and required_confs > 1:
             try:
                 receipt = web3.eth.getTransactionReceipt(self.txid)
                 self.block_number = receipt["blockNumber"]
             except TransactionNotFound:
@@ -440,16 +415,18 @@
             msg = f"Encountered a {type(e).__name__} while requesting "
             msg += "debug_traceTransaction. The local RPC client has likely crashed."
             if CONFIG.argv["coverage"]:
                 msg += " If the error persists, add the skip_coverage fixture to this test."
             raise RPCRequestError(msg) from None
 
         if "error" in trace:
-            self.modified_state = None
-            raise RPCRequestError(trace["error"]["message"])
+            self._modified_state = None
+            self._trace_exc = RPCRequestError(trace["error"]["message"])
+            raise self._trace_exc
+
         self._raw_trace = trace = trace["result"]["structLogs"]
         if not trace:
             self._modified_state = False
             return
 
         if isinstance(trace[0]["gas"], str):
             # handle traces where numeric values are returned as nex (Nethermind)
```

### Comparing `eth-brownie-1.9.7/brownie/network/web3.py` & `eth-brownie-1.9.8/brownie/network/web3.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/build.py` & `eth-brownie-1.9.8/brownie/project/build.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/compiler/__init__.py` & `eth-brownie-1.9.8/brownie/project/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/compiler/solidity.py` & `eth-brownie-1.9.8/brownie/project/compiler/solidity.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,14 +398,22 @@
             pass
 
         if pc_list[-1].get("value", None) == fallback_hexstr and opcodes[0] in ("JUMP", "JUMPI"):
             # track all jumps to the initial revert
             key = (pc_list[-1]["path"], pc_list[-1]["offset"])
             revert_map.setdefault(key, []).append(len(pc_list))
 
+    while opcodes and opcodes[0] not in ("INVALID", "STOP"):
+        # necessary because sometimes solidity returns an incomplete source map
+        pc_list.append({"op": opcodes.popleft(), "pc": pc})
+        pc += 1
+        if opcodes and opcodes[0][:2] == "0x":
+            pc_list[-1]["value"] = opcodes.popleft()
+            pc += int(pc_list[-1]["op"][4:])
+
     # compare revert and require statements against the map of revert jumps
     for (contract_id, fn_offset), values in revert_map.items():
         fn_node = source_nodes[contract_id].children(
             depth=2,
             include_children=False,
             required_offset=fn_offset,
             filters={"nodeType": "FunctionDefinition"},
```

### Comparing `eth-brownie-1.9.7/brownie/project/compiler/utils.py` & `eth-brownie-1.9.8/brownie/project/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/compiler/vyper.py` & `eth-brownie-1.9.8/brownie/project/compiler/vyper.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/ethpm.py` & `eth-brownie-1.9.8/brownie/project/ethpm.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/main.py` & `eth-brownie-1.9.8/brownie/project/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -863,14 +863,26 @@
         path_str: str = path.relative_to(project_path).as_posix()
         contract_sources[path_str] = source
     return contract_sources
 
 
 def _stream_download(download_url: str, target_path: str) -> None:
     response = requests.get(download_url, stream=True, headers=REQUEST_HEADERS)
+
+    if response.status_code == 404:
+        raise ConnectionError(
+            f"404 error when attempting to download from {download_url} - "
+            "are you sure this is a valid mix? https://github.com/brownie-mix"
+        )
+    if response.status_code != 200:
+        raise ConnectionError(
+            f"Received status code {response.status_code} when attempting "
+            f"to download from {download_url}"
+        )
+
     total_size = int(response.headers.get("content-length", 0))
     progress_bar = tqdm(total=total_size, unit="iB", unit_scale=True)
     content = bytes()
 
     for data in response.iter_content(1024, decode_unicode=True):
         progress_bar.update(len(data))
         content += data
```

### Comparing `eth-brownie-1.9.7/brownie/project/scripts.py` & `eth-brownie-1.9.8/brownie/project/scripts.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/project/sources.py` & `eth-brownie-1.9.8/brownie/project/sources.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/__init__.py` & `eth-brownie-1.9.8/brownie/test/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/coverage.py` & `eth-brownie-1.9.8/brownie/test/coverage.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/fixtures.py` & `eth-brownie-1.9.8/brownie/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/managers/base.py` & `eth-brownie-1.9.8/brownie/test/managers/base.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/managers/master.py` & `eth-brownie-1.9.8/brownie/test/managers/master.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/managers/runner.py` & `eth-brownie-1.9.8/brownie/test/managers/runner.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/output.py` & `eth-brownie-1.9.8/brownie/test/output.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/plugin.py` & `eth-brownie-1.9.8/brownie/test/plugin.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/stateful.py` & `eth-brownie-1.9.8/brownie/test/stateful.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/test/strategies.py` & `eth-brownie-1.9.8/brownie/test/strategies.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/utils/color.py` & `eth-brownie-1.9.8/brownie/utils/color.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,40 @@
 #!/usr/bin/python3
 
 import sys
 import traceback
 from pathlib import Path
 from typing import Dict, Optional, Sequence
 
+import pygments
+from pygments.formatters import get_formatter_by_name
+from pygments.lexers import PythonLexer
+from pygments_lexer_solidity import SolidityLexer
+from vyper.exceptions import VyperException
+
 from brownie._config import CONFIG
 
 if sys.platform == "win32":
     import colorama
 
     colorama.init()
 
+fmt_name = "terminal"
+try:
+    import curses
+
+    curses.setupterm()
+    if curses.tigetnum("colors") == 256:
+        fmt_name = "terminal256"
+except Exception:
+    # if curses won't import we are probably using Windows
+    pass
+
+formatter = get_formatter_by_name(fmt_name, style=CONFIG.settings["console"]["color_style"])
+
 
 BASE = "\x1b[0;"
 
 MODIFIERS = {"bright": "1;", "dark": "2;"}
 
 COLORS = {
     "black": "30",
@@ -102,46 +121,70 @@
         exc: Exception,
         filename: str = None,
         start: Optional[int] = None,
         stop: Optional[int] = None,
     ) -> str:
         if isinstance(exc, SyntaxError) and exc.text is not None:
             return self.format_syntaxerror(exc)
+
         tb = [i.replace("./", "") for i in traceback.format_tb(exc.__traceback__)]
         if filename and not CONFIG.argv["tb"]:
             try:
                 start = tb.index(next(i for i in tb if filename in i))
                 stop = tb.index(next(i for i in tb[::-1] if filename in i)) + 1
             except Exception:
                 pass
+
         tb = tb[start:stop]
         for i in range(len(tb)):
             info, code = tb[i].split("\n")[:2]
             info = info.replace(base_path, ".")
             info_lines = [x.strip(",") for x in info.strip().split(" ")]
             if "site-packages/" in info_lines[1]:
                 info_lines[1] = '"' + info_lines[1].split("site-packages/")[1]
             tb[i] = (
                 f"  {self('dark white')}File {self('bright magenta')}{info_lines[1]}"
                 f"{self('dark white')}, line {self('bright blue')}{info_lines[3]}"
                 f"{self('dark white')}, in {self('bright cyan')}{info_lines[5]}{self}"
             )
             if code:
                 tb[i] += f"\n{code}"
-        tb.append(f"{self('bright red')}{type(exc).__name__}{self}: {exc}")
+
+        msg = str(exc)
+        if isinstance(exc, VyperException):
+            # apply syntax highlight and remove traceback on vyper exceptions
+            msg = self.highlight(msg)
+            if not CONFIG.argv["tb"]:
+                tb.clear()
+
+        from brownie.exceptions import CompilerError
+
+        if isinstance(exc, CompilerError):
+            # apply syntax highlighting on solc exceptions
+            msg = self.highlight(msg, SolidityLexer())
+            if not CONFIG.argv["tb"]:
+                tb.clear()
+
+        tb.append(f"{self('bright red')}{type(exc).__name__}{self}: {msg}")
         return "\n".join(tb)
 
     def format_syntaxerror(self, exc: SyntaxError) -> str:
         offset = exc.offset + len(exc.text.lstrip()) - len(exc.text) + 3  # type: ignore
         exc.filename = exc.filename.replace(base_path, ".")
         return (
             f"  {self('dark white')}File \"{self('bright magenta')}{exc.filename}"
             f"{self('dark white')}\", line {self('bright blue')}{exc.lineno}"
             f"{self('dark white')},\n{self}    {exc.text.strip()}\n"
             f"{' '*offset}^\n{self('bright red')}SyntaxError{self}: {exc.msg}"
         )
 
+    def highlight(self, text, lexer=PythonLexer()):
+        """
+        Apply syntax highlighting to a string.
+        """
+        return pygments.highlight(text, lexer, formatter)
+
 
 def notify(type_, msg):
     """Prepends a message with a colored tag and outputs it to the console."""
     color = Color()
     print(f"{color(NOTIFY_COLORS[type_])}{type_}{color}: {msg}")
```

### Comparing `eth-brownie-1.9.7/brownie/utils/docopt.py` & `eth-brownie-1.9.8/brownie/utils/docopt.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/brownie/utils/sql.py` & `eth-brownie-1.9.8/brownie/utils/sql.py`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/eth_brownie.egg-info/PKG-INFO` & `eth-brownie-1.9.8/eth_brownie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-brownie
-Version: 1.9.7
+Version: 1.9.8
 Summary: A Python framework for Ethereum smart contract deployment, testing and interaction.
 Home-page: https://github.com/eth-brownie/brownie
 Author: Ben Hauser
 Author-email: ben@hauser.id
 License: MIT
 Description: # Brownie
```

### Comparing `eth-brownie-1.9.7/eth_brownie.egg-info/SOURCES.txt` & `eth-brownie-1.9.8/eth_brownie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/pyproject.toml` & `eth-brownie-1.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-brownie-1.9.7/setup.cfg` & `eth-brownie-1.9.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.7
+current_version = 1.9.8
 
 [bumpversion:file:setup.py]
 
 [bumpversion:file:brownie/_config.py]
 
 [flake8]
 exclude = tests/data/*
@@ -11,15 +11,15 @@
 ignore = E203,W503
 
 [tool:isort]
 force_grid_wrap = 0
 include_trailing_comma = True
 known_standard_library = tkinter
 known_first_party = brownie
-known_third_party = _pytest,ens,eth_abi,eth_account,eth_event,eth_hash,eth_keys,eth_utils,ethpm,hexbytes,hypothesis,mythx_models,prompt_toolkit,psutil,py,pygments,pytest,pythx,requests,semantic_version,setuptools,solcast,solcx,tqdm,vyper,web3,xdist,yaml
+known_third_party = _pytest,ens,eth_abi,eth_account,eth_event,eth_hash,eth_keys,eth_utils,ethpm,hexbytes,hypothesis,mythx_models,prompt_toolkit,psutil,py,pygments,pygments_lexer_solidity,pytest,pythx,requests,semantic_version,setuptools,solcast,solcx,tqdm,vyper,web3,xdist,yaml
 line_length = 100
 multi_line_output = 3
 use_parentheses = True
 
 [mypy]
 ignore_missing_imports = True
 follow_imports = silent
```

### Comparing `eth-brownie-1.9.7/setup.py` & `eth-brownie-1.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = list(map(str.strip, f.read().split("\n")))[:-1]
 
 setup(
     name="eth-brownie",
     packages=find_packages(),
-    version="1.9.7",  # don't change this manually, use bumpversion instead
+    version="1.9.8",  # don't change this manually, use bumpversion instead
     license="MIT",
     description="A Python framework for Ethereum smart contract deployment, testing and interaction.",  # noqa: E501
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ben Hauser",
     author_email="ben@hauser.id",
     url="https://github.com/eth-brownie/brownie",
```

