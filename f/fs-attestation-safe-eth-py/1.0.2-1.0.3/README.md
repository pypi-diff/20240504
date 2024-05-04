# Comparing `tmp/fs-attestation-safe-eth-py-1.0.2.tar.gz` & `tmp/fs-attestation-safe-eth-py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs-attestation-safe-eth-py-1.0.2.tar", last modified: Thu Apr 25 06:42:29 2024, max compression
+gzip compressed data, was "fs-attestation-safe-eth-py-1.0.3.tar", last modified: Sat May  4 05:04:01 2024, max compression
```

## Comparing `fs-attestation-safe-eth-py-1.0.2.tar` & `fs-attestation-safe-eth-py-1.0.3.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.313163 fs-attestation-safe-eth-py-1.0.2/
--rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/LICENSE
--rw-r--r--   0 mohan      (501) staff       (20)       71 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/MANIFEST.in
--rw-r--r--   0 mohan      (501) staff       (20)     2234 2024-04-25 06:42:29.314472 fs-attestation-safe-eth-py-1.0.2/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)      714 2024-04-25 06:42:08.000000 fs-attestation-safe-eth-py-1.0.2/README.rst
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.163952 fs-attestation-safe-eth-py-1.0.2/docs/
--rw-r--r--   0 mohan      (501) staff       (20)      638 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/Makefile
--rw-r--r--   0 mohan      (501) staff       (20)      799 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/make.bat
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.172342 fs-attestation-safe-eth-py-1.0.2/docs/source/
--rw-r--r--   0 mohan      (501) staff       (20)     1987 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/conf.py
--rw-r--r--   0 mohan      (501) staff       (20)      978 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 mohan      (501) staff       (20)      183 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 mohan      (501) staff       (20)      177 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 mohan      (501) staff       (20)     1198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 mohan      (501) staff       (20)      936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.rst
--rw-r--r--   0 mohan      (501) staff       (20)      226 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.rst
--rw-r--r--   0 mohan      (501) staff       (20)     1852 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.safe.rst
--rw-r--r--   0 mohan      (501) staff       (20)      894 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/index.rst
--rw-r--r--   0 mohan      (501) staff       (20)       55 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/modules.rst
--rw-r--r--   0 mohan      (501) staff       (20)     8368 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/docs/source/quickstart.rst
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.175703 fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/
--rw-r--r--   0 mohan      (501) staff       (20)     2234 2024-04-25 06:42:29.000000 fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 mohan      (501) staff       (20)     7536 2024-04-25 06:42:29.000000 fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 mohan      (501) staff       (20)        1 2024-04-25 06:42:29.000000 fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 mohan      (501) staff       (20)      129 2024-04-25 06:42:29.000000 fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 mohan      (501) staff       (20)        7 2024-04-25 06:42:29.000000 fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/top_level.txt
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.176528 fs-attestation-safe-eth-py-1.0.2/gnosis/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.178000 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/
--rw-r--r--   0 mohan      (501) staff       (20)      156 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     8465 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/cow_swap_api.py
--rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/order.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.178772 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/tests/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5604 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/tests/test_cow_swap_api.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.184612 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/
--rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.188140 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)      348 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7060 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/bundler_client.py
--rw-r--r--   0 mohan      (501) staff       (20)      986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/constants.py
--rw-r--r--   0 mohan      (501) staff       (20)      208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)     4259 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/user_operation.py
--rw-r--r--   0 mohan      (501) staff       (20)     3357 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/user_operation_receipt.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.190977 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/
--rw-r--r--   0 mohan      (501) staff       (20)      878 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     9236 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 mohan      (501) staff       (20)      194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 mohan      (501) staff       (20)     4839 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/ens_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     9677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     3345 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/sourcify_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     1020 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/constants.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.191962 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/
--rw-r--r--   0 mohan      (501) staff       (20)    10273 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.231068 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/
--rw-r--r--   0 mohan      (501) staff       (20)   328664 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/CPKFactory.json
--rw-r--r--   0 mohan      (501) staff       (20)    28908 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    29485 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)    26897 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
--rw-r--r--   0 mohan      (501) staff       (20)    29068 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC1155.json
--rw-r--r--   0 mohan      (501) staff       (20)    54748 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC20.json
--rw-r--r--   0 mohan      (501) staff       (20)    89890 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC20TestToken.json
--rw-r--r--   0 mohan      (501) staff       (20)   622260 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC721.json
--rw-r--r--   0 mohan      (501) staff       (20)   983403 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
--rw-r--r--   0 mohan      (501) staff       (20)  1158944 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
--rw-r--r--   0 mohan      (501) staff       (20)  1347363 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
--rw-r--r--   0 mohan      (501) staff       (20)   119875 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    19886 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/MultiSend.json
--rw-r--r--   0 mohan      (501) staff       (20)    78793 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/PayingProxy.json
--rw-r--r--   0 mohan      (501) staff       (20)   136946 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
--rw-r--r--   0 mohan      (501) staff       (20)   288861 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
--rw-r--r--   0 mohan      (501) staff       (20)    18975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    15538 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)    32495 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
--rw-r--r--   0 mohan      (501) staff       (20)    39032 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
--rw-r--r--   0 mohan      (501) staff       (20)     1862 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
--rw-r--r--   0 mohan      (501) staff       (20)     1849 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)   121611 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Safe_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/SignMessageLib.json
--rw-r--r--   0 mohan      (501) staff       (20)     4913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7351 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/kyber_network_proxy.json
--rw-r--r--   0 mohan      (501) staff       (20)    19012 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/multicall.py
--rw-r--r--   0 mohan      (501) staff       (20)    17165 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_exchange.json
--rw-r--r--   0 mohan      (501) staff       (20)     2480 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_factory.json
--rw-r--r--   0 mohan      (501) staff       (20)     2242 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_v2_factory.json
--rw-r--r--   0 mohan      (501) staff       (20)     8293 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_v2_pair.json
--rw-r--r--   0 mohan      (501) staff       (20)    11889 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_v2_router.json
--rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/contract_base.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.234500 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     3735 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/admin.py
--rw-r--r--   0 mohan      (501) staff       (20)      269 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/filters.py
--rw-r--r--   0 mohan      (501) staff       (20)     2435 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/forms.py
--rw-r--r--   0 mohan      (501) staff       (20)     9936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/models.py
--rw-r--r--   0 mohan      (501) staff       (20)     6191 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.238214 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)      711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/models.py
--rw-r--r--   0 mohan      (501) staff       (20)     3028 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 mohan      (501) staff       (20)     8621 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 mohan      (501) staff       (20)     7877 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 mohan      (501) staff       (20)      484 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 mohan      (501) staff       (20)      320 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/validators.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.238996 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/eip712/
--rw-r--r--   0 mohan      (501) staff       (20)     5915 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    82106 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/ethereum_client.py
--rw-r--r--   0 mohan      (501) staff       (20)    35545 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/ethereum_network.py
--rw-r--r--   0 mohan      (501) staff       (20)     1332 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)    13617 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/multicall.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.244946 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/
--rw-r--r--   0 mohan      (501) staff       (20)     1093 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.252190 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    15986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    30036 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    29731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    27567 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    25872 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)      239 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)    45208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 mohan      (501) staff       (20)    36257 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)     1464 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 mohan      (501) staff       (20)     2375 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 mohan      (501) staff       (20)      161 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.253045 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/helpers/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5856 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 mohan      (501) staff       (20)     4117 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 mohan      (501) staff       (20)    32169 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 mohan      (501) staff       (20)     1677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 mohan      (501) staff       (20)     1516 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 mohan      (501) staff       (20)     7154 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.257663 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.260683 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     6695 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_bundler_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     2727 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
--rw-r--r--   0 mohan      (501) staff       (20)      671 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_user_operation.py
--rw-r--r--   0 mohan      (501) staff       (20)      947 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.265864 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)   107388 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 mohan      (501) staff       (20)     1047 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     6185 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_ens_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     1686 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     2521 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_sourcify_client.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.267075 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/eip712/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    13327 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 mohan      (501) staff       (20)     3189 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.273435 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    29208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_bundler.py
--rw-r--r--   0 mohan      (501) staff       (20)    31306 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 mohan      (501) staff       (20)    10570 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 mohan      (501) staff       (20)   792720 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 mohan      (501) staff       (20)    92795 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 mohan      (501) staff       (20)   171076 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.277132 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2706 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 mohan      (501) staff       (20)     1820 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 mohan      (501) staff       (20)     1460 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 mohan      (501) staff       (20)     2043 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 mohan      (501) staff       (20)     3544 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 mohan      (501) staff       (20)    61025 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 mohan      (501) staff       (20)     7087 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 mohan      (501) staff       (20)    21137 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 mohan      (501) staff       (20)     7287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)      390 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/typing.py
--rw-r--r--   0 mohan      (501) staff       (20)     6977 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/eth/utils.py
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/py.typed
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.293645 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/
--rw-r--r--   0 mohan      (501) staff       (20)      742 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.295374 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)      101 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5647 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/account_abstraction/safe_operation.py
--rw-r--r--   0 mohan      (501) staff       (20)    63401 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/addresses.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.298816 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/
--rw-r--r--   0 mohan      (501) staff       (20)      346 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     2471 2024-04-24 04:21:12.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/base_api.py
--rw-r--r--   0 mohan      (501) staff       (20)     2913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/relay_service_api.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.301555 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/
--rw-r--r--   0 mohan      (501) staff       (20)      103 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)    14033 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/transaction_service_api.py
--rw-r--r--   0 mohan      (501) staff       (20)     1732 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
--rw-r--r--   0 mohan      (501) staff       (20)      252 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)      105 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/enums.py
--rw-r--r--   0 mohan      (501) staff       (20)     1451 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/exceptions.py
--rw-r--r--   0 mohan      (501) staff       (20)    11459 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/multi_send.py
--rw-r--r--   0 mohan      (501) staff       (20)    10479 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/proxy_factory.py
--rw-r--r--   0 mohan      (501) staff       (20)    36823 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe.py
--rw-r--r--   0 mohan      (501) staff       (20)    11975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)     9736 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_creator.py
--rw-r--r--   0 mohan      (501) staff       (20)   121198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_deployments.py
--rw-r--r--   0 mohan      (501) staff       (20)    12587 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_signature.py
--rw-r--r--   0 mohan      (501) staff       (20)    17225 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)     4194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/serializers.py
--rw-r--r--   0 mohan      (501) staff       (20)     2000 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/signatures.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.308297 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.309079 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/account_abstraction/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/account_abstraction/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     3469 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/account_abstraction/test_safe_operation.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.309934 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/api/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     5341 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 mohan      (501) staff       (20)    20692 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 mohan      (501) staff       (20)     1398 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_addresses.py
--rw-r--r--   0 mohan      (501) staff       (20)    10515 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_multi_send.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.310940 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_proxy_factory/
--rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_proxy_factory/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     7798 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
--rw-r--r--   0 mohan      (501) staff       (20)    33486 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 mohan      (501) staff       (20)    16674 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)    18510 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 mohan      (501) staff       (20)    13004 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 mohan      (501) staff       (20)     2563 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_v1_0_0.py
--rw-r--r--   0 mohan      (501) staff       (20)     1073 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_v1_3_0.py
--rw-r--r--   0 mohan      (501) staff       (20)     3731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 mohan      (501) staff       (20)     3711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 mohan      (501) staff       (20)      287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-04-25 06:42:29.312558 fs-attestation-safe-eth-py-1.0.2/gnosis/util/
--rw-r--r--   0 mohan      (501) staff       (20)       83 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/util/__init__.py
--rw-r--r--   0 mohan      (501) staff       (20)     1003 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/util/http.py
--rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/gnosis/util/util.py
--rw-r--r--   0 mohan      (501) staff       (20)     2446 2024-04-25 06:42:29.316125 fs-attestation-safe-eth-py-1.0.2/setup.cfg
--rw-r--r--   0 mohan      (501) staff       (20)       69 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.2/setup.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.372937 fs-attestation-safe-eth-py-1.0.3/
+-rw-r--r--   0 mohan      (501) staff       (20)     1082 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/LICENSE
+-rw-r--r--   0 mohan      (501) staff       (20)       71 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/MANIFEST.in
+-rw-r--r--   0 mohan      (501) staff       (20)     2234 2024-05-04 05:04:01.373139 fs-attestation-safe-eth-py-1.0.3/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)      714 2024-04-25 06:42:08.000000 fs-attestation-safe-eth-py-1.0.3/README.rst
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.017285 fs-attestation-safe-eth-py-1.0.3/docs/
+-rw-r--r--   0 mohan      (501) staff       (20)      638 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/Makefile
+-rw-r--r--   0 mohan      (501) staff       (20)      799 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/make.bat
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.034176 fs-attestation-safe-eth-py-1.0.3/docs/source/
+-rw-r--r--   0 mohan      (501) staff       (20)     1987 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/conf.py
+-rw-r--r--   0 mohan      (501) staff       (20)      978 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      183 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      177 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 mohan      (501) staff       (20)     1198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      226 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.rst
+-rw-r--r--   0 mohan      (501) staff       (20)     1852 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.safe.rst
+-rw-r--r--   0 mohan      (501) staff       (20)      894 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/index.rst
+-rw-r--r--   0 mohan      (501) staff       (20)       55 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/modules.rst
+-rw-r--r--   0 mohan      (501) staff       (20)     8368 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/docs/source/quickstart.rst
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.037925 fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/
+-rw-r--r--   0 mohan      (501) staff       (20)     2234 2024-05-04 05:04:00.000000 fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 mohan      (501) staff       (20)     7536 2024-05-04 05:04:00.000000 fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        1 2024-05-04 05:04:00.000000 fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mohan      (501) staff       (20)      129 2024-05-04 05:04:00.000000 fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 mohan      (501) staff       (20)        7 2024-05-04 05:04:00.000000 fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/top_level.txt
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.038918 fs-attestation-safe-eth-py-1.0.3/gnosis/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.041683 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/
+-rw-r--r--   0 mohan      (501) staff       (20)      156 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8465 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/cow_swap_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2700 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/order.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.042587 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/tests/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5604 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/tests/test_cow_swap_api.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.055500 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/
+-rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.062902 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)      348 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7060 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/bundler_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)      986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/constants.py
+-rw-r--r--   0 mohan      (501) staff       (20)      208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4259 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/user_operation.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3357 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/user_operation_receipt.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.070707 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/
+-rw-r--r--   0 mohan      (501) staff       (20)      878 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9236 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)      194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4839 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/ens_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3345 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/sourcify_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1020 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/constants.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.073475 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/
+-rw-r--r--   0 mohan      (501) staff       (20)    10273 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.172397 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/
+-rw-r--r--   0 mohan      (501) staff       (20)   328664 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/CPKFactory.json
+-rw-r--r--   0 mohan      (501) staff       (20)    28908 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    29485 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)    26897 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
+-rw-r--r--   0 mohan      (501) staff       (20)    29068 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC1155.json
+-rw-r--r--   0 mohan      (501) staff       (20)    54748 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC20.json
+-rw-r--r--   0 mohan      (501) staff       (20)    89890 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC20TestToken.json
+-rw-r--r--   0 mohan      (501) staff       (20)   622260 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC721.json
+-rw-r--r--   0 mohan      (501) staff       (20)   983403 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)  1158944 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)  1347363 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)   119875 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    19886 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/MultiSend.json
+-rw-r--r--   0 mohan      (501) staff       (20)    78793 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/PayingProxy.json
+-rw-r--r--   0 mohan      (501) staff       (20)   136946 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)   288861 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)    18975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    15538 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)    32495 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)    39032 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)     1862 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
+-rw-r--r--   0 mohan      (501) staff       (20)     1849 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)   121611 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Safe_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/SignMessageLib.json
+-rw-r--r--   0 mohan      (501) staff       (20)     4913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7351 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/kyber_network_proxy.json
+-rw-r--r--   0 mohan      (501) staff       (20)    19012 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/multicall.py
+-rw-r--r--   0 mohan      (501) staff       (20)    17165 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_exchange.json
+-rw-r--r--   0 mohan      (501) staff       (20)     2480 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_factory.json
+-rw-r--r--   0 mohan      (501) staff       (20)     2242 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_v2_factory.json
+-rw-r--r--   0 mohan      (501) staff       (20)     8293 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_v2_pair.json
+-rw-r--r--   0 mohan      (501) staff       (20)    11889 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_v2_router.json
+-rw-r--r--   0 mohan      (501) staff       (20)      954 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/contract_base.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.182732 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3735 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/admin.py
+-rw-r--r--   0 mohan      (501) staff       (20)      269 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/filters.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2435 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/forms.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9936 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/models.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6191 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.188697 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)      711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3028 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 mohan      (501) staff       (20)     8621 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7877 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 mohan      (501) staff       (20)      484 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 mohan      (501) staff       (20)      320 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/validators.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.189830 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/eip712/
+-rw-r--r--   0 mohan      (501) staff       (20)     5915 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    82106 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)    35545 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1332 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)    13617 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/multicall.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.202044 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/
+-rw-r--r--   0 mohan      (501) staff       (20)     1093 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.213755 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    15986 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    30036 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    29731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    27567 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    25872 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)      239 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)    45208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 mohan      (501) staff       (20)    36257 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1464 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2375 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)      161 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.215561 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5856 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4117 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 mohan      (501) staff       (20)    32169 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1677 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1516 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7154 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1064 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.227041 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.229319 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6695 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_bundler_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2727 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)      671 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_user_operation.py
+-rw-r--r--   0 mohan      (501) staff       (20)      947 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.234660 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)   107388 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1047 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6185 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_ens_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1686 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2521 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_sourcify_client.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.235579 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/eip712/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    13327 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3189 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.244468 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    29208 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_bundler.py
+-rw-r--r--   0 mohan      (501) staff       (20)    31306 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10570 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 mohan      (501) staff       (20)   792720 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 mohan      (501) staff       (20)    92795 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 mohan      (501) staff       (20)   171076 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.255925 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2706 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1820 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1460 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2043 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3544 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 mohan      (501) staff       (20)    61025 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7087 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 mohan      (501) staff       (20)    21137 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5069 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)      390 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/typing.py
+-rw-r--r--   0 mohan      (501) staff       (20)     6977 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/eth/utils.py
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/py.typed
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.338552 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/
+-rw-r--r--   0 mohan      (501) staff       (20)      742 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.341886 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)      101 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5647 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/account_abstraction/safe_operation.py
+-rw-r--r--   0 mohan      (501) staff       (20)    63401 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/addresses.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.346485 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/
+-rw-r--r--   0 mohan      (501) staff       (20)      346 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2512 2024-05-04 05:02:30.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/base_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2913 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/relay_service_api.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.350997 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/
+-rw-r--r--   0 mohan      (501) staff       (20)      103 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)    14033 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/transaction_service_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1732 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
+-rw-r--r--   0 mohan      (501) staff       (20)      252 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)      105 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/enums.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1451 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/exceptions.py
+-rw-r--r--   0 mohan      (501) staff       (20)    11459 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/multi_send.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10479 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 mohan      (501) staff       (20)    36823 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe.py
+-rw-r--r--   0 mohan      (501) staff       (20)    11975 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)     9736 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_creator.py
+-rw-r--r--   0 mohan      (501) staff       (20)   121198 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_deployments.py
+-rw-r--r--   0 mohan      (501) staff       (20)    12587 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_signature.py
+-rw-r--r--   0 mohan      (501) staff       (20)    17225 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)     4194 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/serializers.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2000 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/signatures.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.366572 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.367921 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/account_abstraction/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/account_abstraction/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3469 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/account_abstraction/test_safe_operation.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.369019 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/api/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     5341 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 mohan      (501) staff       (20)    20692 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1398 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 mohan      (501) staff       (20)    10515 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_multi_send.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.370010 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_proxy_factory/
+-rw-r--r--   0 mohan      (501) staff       (20)        0 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_proxy_factory/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     7798 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
+-rw-r--r--   0 mohan      (501) staff       (20)    33486 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 mohan      (501) staff       (20)    16674 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)    18510 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 mohan      (501) staff       (20)    13004 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2563 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_v1_0_0.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1073 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_v1_3_0.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3731 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 mohan      (501) staff       (20)     3711 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 mohan      (501) staff       (20)      287 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 mohan      (501) staff       (20)        0 2024-05-04 05:04:01.372452 fs-attestation-safe-eth-py-1.0.3/gnosis/util/
+-rw-r--r--   0 mohan      (501) staff       (20)       83 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/util/__init__.py
+-rw-r--r--   0 mohan      (501) staff       (20)     1003 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/util/http.py
+-rw-r--r--   0 mohan      (501) staff       (20)      450 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/gnosis/util/util.py
+-rw-r--r--   0 mohan      (501) staff       (20)     2446 2024-05-04 05:04:01.373971 fs-attestation-safe-eth-py-1.0.3/setup.cfg
+-rw-r--r--   0 mohan      (501) staff       (20)       69 2024-04-23 09:43:20.000000 fs-attestation-safe-eth-py-1.0.3/setup.py
```

### Comparing `fs-attestation-safe-eth-py-1.0.2/LICENSE` & `fs-attestation-safe-eth-py-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/PKG-INFO` & `fs-attestation-safe-eth-py-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-eth-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Modified safe-eth-py library version 6.0.0b25 to be used in FailSafe Attestation Service CLI. The original safe-eth-py is available here https://pypi.org/project/safe-eth-py/
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Mohan | Team FailSafe | https://getfailsafe.com
 Author-email: mohan@ethlas.com
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `fs-attestation-safe-eth-py-1.0.2/README.rst` & `fs-attestation-safe-eth-py-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/Makefile` & `fs-attestation-safe-eth-py-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/make.bat` & `fs-attestation-safe-eth-py-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/conf.py` & `fs-attestation-safe-eth-py-1.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.clients.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.django.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.oracles.abis.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.eth.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/gnosis.safe.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/index.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/docs/source/quickstart.rst` & `fs-attestation-safe-eth-py-1.0.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/PKG-INFO` & `fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-attestation-safe-eth-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Modified safe-eth-py library version 6.0.0b25 to be used in FailSafe Attestation Service CLI. The original safe-eth-py is available here https://pypi.org/project/safe-eth-py/
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Mohan | Team FailSafe | https://getfailsafe.com
 Author-email: mohan@ethlas.com
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `fs-attestation-safe-eth-py-1.0.2/fs_attestation_safe_eth_py.egg-info/SOURCES.txt` & `fs-attestation-safe-eth-py-1.0.3/fs_attestation_safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/cow_swap_api.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/order.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/order.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/cowsap/tests/test_cow_swap_api.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/cowsap/tests/test_cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/__init__.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/bundler_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/bundler_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/constants.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/constants.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/user_operation.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/user_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/account_abstraction/user_operation_receipt.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/account_abstraction/user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/__init__.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/blockscout_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/ens_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/ens_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/etherscan_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/clients/sourcify_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/clients/sourcify_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/constants.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/__init__.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/CPKFactory.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/DelegateConstructorProxy.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC1155.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC1155.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC20.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC20TestToken.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ERC721.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ERC721.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/MultiSend.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/MultiSend.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/PayingProxy.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_0_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_1_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_3_0.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Proxy_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Proxy_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/Safe_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/Safe_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/SignMessageLib.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/SignMessageLib.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/kyber_network_proxy.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/multicall.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_exchange.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_factory.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_v2_factory.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_v2_pair.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/abis/uniswap_v2_router.json` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/abis/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/contracts/contract_base.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/contracts/contract_base.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/admin.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/forms.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/models.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/serializers.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/models.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_forms.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_models.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/django/tests/test_serializers.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/eip712/__init__.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/ethereum_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/ethereum_network.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/exceptions.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/multicall.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/__init__.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/aave_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/balancer_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/cream_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/curve_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/mooniswap_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/uniswap_v3.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/yearn_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/abis/zerion_abis.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/cowswap.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/kyber.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/oracles.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/superfluid.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/sushiswap.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/uniswap_v3.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/oracles/utils.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_bundler_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_bundler_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_user_operation.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_user_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/mocks.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_blockscout_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_ens_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_ens_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_etherscan_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/clients/test_sourcify_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/clients/test_sourcify_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/eip712/test_eip712.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/ethereum_test_case.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_bundler.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_bundler.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_internal_txs.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_log_receipts.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_trace_block.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_trace_filter.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_cowswap.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_kyber.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_superfluid.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_sushiswap.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_ethereum_client.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_multicall.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_oracles.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/test_utils.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/tests/utils.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/eth/utils.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/__init__.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/account_abstraction/safe_operation.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/account_abstraction/safe_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/addresses.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/addresses.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/base_api.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             raise EthereumNetworkNotSupported(network)
         self.http_session = prepare_http_session(10, 100)
         self.request_timeout = request_timeout
 
     @classmethod
     def from_custom_safe_tx_service_base_url(cls, ethereum_client: EthereumClient, base_url: str) -> "SafeBaseAPI":
         ethereum_network = ethereum_client.get_network()
-        return cls(ethereum_network, base_url=base_url)
+        return cls(network=ethereum_network, ethereum_client=ethereum_client, base_url=base_url)
 
     @classmethod
     def from_ethereum_client(cls, ethereum_client: EthereumClient) -> "SafeBaseAPI":
         ethereum_network = ethereum_client.get_network()
         return cls(ethereum_network, ethereum_client=ethereum_client)
 
     def _get_request(self, url: str) -> requests.Response:
```

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/relay_service_api.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/transaction_service_api.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/api/transaction_service_api/transaction_service_messages.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/api/transaction_service_api/transaction_service_messages.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/exceptions.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/multi_send.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/proxy_factory.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_create2_tx.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_creator.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_creator.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_deployments.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_deployments.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_signature.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/safe_tx.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/serializers.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/signatures.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/account_abstraction/test_safe_operation.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/account_abstraction/test_safe_operation.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/api/test_transaction_service_api.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/safe_test_case.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_addresses.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_multi_send.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_create2_tx.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_signature.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_tx.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_v1_0_0.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_safe_v1_3_0.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_safe_v1_3_0.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_serializers.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/safe/tests/test_signatures.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/gnosis/util/http.py` & `fs-attestation-safe-eth-py-1.0.3/gnosis/util/http.py`

 * *Files identical despite different names*

### Comparing `fs-attestation-safe-eth-py-1.0.2/setup.cfg` & `fs-attestation-safe-eth-py-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fs-attestation-safe-eth-py
-version = 1.0.2
+version = 1.0.3
 description = Modified safe-eth-py library version 6.0.0b25 to be used in FailSafe Attestation Service CLI. The original safe-eth-py is available here https://pypi.org/project/safe-eth-py/
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

