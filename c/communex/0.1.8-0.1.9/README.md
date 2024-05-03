# Comparing `tmp/communex-0.1.8.tar.gz` & `tmp/communex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communex-0.1.8.tar", max compression
+gzip compressed data, was "communex-0.1.9.tar", max compression
```

## Comparing `communex-0.1.8.tar` & `communex-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      909 2024-03-23 11:18:25.661457 communex-0.1.8/LICENSE
--rw-r--r--   0        0        0     4575 2024-03-24 19:18:19.153594 communex-0.1.8/README.md
--rw-r--r--   0        0        0     1385 2024-04-03 22:10:50.105212 communex-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      451 2024-03-30 15:42:14.063605 communex-0.1.8/src/communex/__init__.py
--rw-r--r--   0        0        0     1572 2024-04-03 22:10:23.093921 communex-0.1.8/src/communex/_common.py
--rw-r--r--   0        0        0      426 2024-03-23 11:18:25.662457 communex-0.1.8/src/communex/balance.py
--rw-r--r--   0        0        0       41 2024-04-02 20:20:50.841713 communex-0.1.8/src/communex/cli/__init__.py
--rw-r--r--   0        0        0       86 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/__main__.py
--rw-r--r--   0        0        0     2302 2024-04-03 22:10:23.093921 communex-0.1.8/src/communex/cli/_common.py
--rw-r--r--   0        0        0     6735 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/balance.py
--rw-r--r--   0        0        0     7590 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/key.py
--rw-r--r--   0        0        0     2406 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/misc.py
--rw-r--r--   0        0        0     6408 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/module.py
--rw-r--r--   0        0        0     5536 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/network.py
--rw-r--r--   0        0        0     1449 2024-04-03 22:10:23.093921 communex-0.1.8/src/communex/cli/root.py
--rw-r--r--   0        0        0     3546 2024-03-30 16:23:28.998483 communex-0.1.8/src/communex/cli/subnet.py
--rw-r--r--   0        0        0    91414 2024-03-30 15:44:47.719256 communex-0.1.8/src/communex/client.py
--rw-r--r--   0        0        0      297 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/__init__.py
--rw-r--r--   0        0        0     1120 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/_util.py
--rw-r--r--   0        0        0     5290 2024-03-25 19:42:20.678258 communex-0.1.8/src/communex/compat/key.py
--rw-r--r--   0        0        0     2636 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/storage.py
--rw-r--r--   0        0        0      386 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/compat/types.py
--rw-r--r--   0        0        0      262 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/errors.py
--rw-r--r--   0        0        0     1329 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/key.py
--rw-r--r--   0        0        0    12756 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/misc.py
--rw-r--r--   0        0        0      142 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/module/__init__.py
--rw-r--r--   0        0        0     1533 2024-03-23 14:58:10.559875 communex-0.1.8/src/communex/module/_ip_limiter.py
--rw-r--r--   0        0        0     2059 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/module/_signer.py
--rw-r--r--   0        0        0     2712 2024-03-25 14:07:08.730822 communex-0.1.8/src/communex/module/client.py
--rw-r--r--   0        0        0        0 2024-03-23 11:18:25.663457 communex-0.1.8/src/communex/module/example/__init__.py
--rw-r--r--   0        0        0     1562 2024-03-30 16:16:22.622958 communex-0.1.8/src/communex/module/example/gpt.py
--rw-r--r--   0        0        0      544 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/module/example/openai.py
--rw-r--r--   0        0        0     2086 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/module/module.py
--rw-r--r--   0        0        0     7676 2024-03-30 16:23:28.999483 communex-0.1.8/src/communex/module/server.py
--rw-r--r--   0        0        0      381 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/module/stuff.md
--rw-r--r--   0        0        0     2272 2024-03-30 16:12:44.684414 communex-0.1.8/src/communex/types.py
--rw-r--r--   0        0        0     1333 2024-03-23 11:18:25.664457 communex-0.1.8/src/communex/util.py
--rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 communex-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      909 2024-03-23 11:18:25.661457 communex-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4575 2024-03-24 19:18:19.153594 communex-0.1.9/README.md
+-rw-r--r--   0        0        0     1385 2024-04-04 11:40:58.489456 communex-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      451 2024-03-30 15:42:14.063605 communex-0.1.9/src/communex/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-04 11:37:33.825239 communex-0.1.9/src/communex/_common.py
+-rw-r--r--   0        0        0      426 2024-03-23 11:18:25.662457 communex-0.1.9/src/communex/balance.py
+-rw-r--r--   0        0        0       41 2024-04-02 20:20:50.841713 communex-0.1.9/src/communex/cli/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/__main__.py
+-rw-r--r--   0        0        0     2302 2024-04-03 22:10:23.093921 communex-0.1.9/src/communex/cli/_common.py
+-rw-r--r--   0        0        0     6735 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/balance.py
+-rw-r--r--   0        0        0     7590 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/key.py
+-rw-r--r--   0        0        0     2406 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/misc.py
+-rw-r--r--   0        0        0     6408 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/module.py
+-rw-r--r--   0        0        0     5536 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/network.py
+-rw-r--r--   0        0        0     1449 2024-04-03 22:10:23.093921 communex-0.1.9/src/communex/cli/root.py
+-rw-r--r--   0        0        0     3546 2024-03-30 16:23:28.998483 communex-0.1.9/src/communex/cli/subnet.py
+-rw-r--r--   0        0        0    91414 2024-03-30 15:44:47.719256 communex-0.1.9/src/communex/client.py
+-rw-r--r--   0        0        0      297 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/compat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/compat/_util.py
+-rw-r--r--   0        0        0     5290 2024-03-25 19:42:20.678258 communex-0.1.9/src/communex/compat/key.py
+-rw-r--r--   0        0        0     2636 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/compat/storage.py
+-rw-r--r--   0        0        0      386 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/compat/types.py
+-rw-r--r--   0        0        0      262 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/errors.py
+-rw-r--r--   0        0        0     1329 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/key.py
+-rw-r--r--   0        0        0    12756 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/misc.py
+-rw-r--r--   0        0        0      142 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/module/__init__.py
+-rw-r--r--   0        0        0     1533 2024-03-23 14:58:10.559875 communex-0.1.9/src/communex/module/_ip_limiter.py
+-rw-r--r--   0        0        0     2059 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/module/_signer.py
+-rw-r--r--   0        0        0     2712 2024-03-25 14:07:08.730822 communex-0.1.9/src/communex/module/client.py
+-rw-r--r--   0        0        0        0 2024-03-23 11:18:25.663457 communex-0.1.9/src/communex/module/example/__init__.py
+-rw-r--r--   0        0        0     1562 2024-03-30 16:16:22.622958 communex-0.1.9/src/communex/module/example/gpt.py
+-rw-r--r--   0        0        0      544 2024-03-23 11:18:25.664457 communex-0.1.9/src/communex/module/example/openai.py
+-rw-r--r--   0        0        0     2086 2024-03-23 11:18:25.664457 communex-0.1.9/src/communex/module/module.py
+-rw-r--r--   0        0        0     7676 2024-03-30 16:23:28.999483 communex-0.1.9/src/communex/module/server.py
+-rw-r--r--   0        0        0      381 2024-03-23 11:18:25.664457 communex-0.1.9/src/communex/module/stuff.md
+-rw-r--r--   0        0        0     2272 2024-03-30 16:12:44.684414 communex-0.1.9/src/communex/types.py
+-rw-r--r--   0        0        0     1333 2024-03-23 11:18:25.664457 communex-0.1.9/src/communex/util.py
+-rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 communex-0.1.9/PKG-INFO
```

### Comparing `communex-0.1.8/LICENSE` & `communex-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/README.md` & `communex-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/pyproject.toml` & `communex-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "communex"
-version = "0.1.8"
+version = "0.1.9"
 description = "A library for Commune network focused on simplicity"
 authors = ["agicommies <info@agicommies.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 comx = "communex.cli:app"
```

### Comparing `communex-0.1.8/src/communex/_common.py` & `communex-0.1.9/src/communex/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 def get_node_url(comx_settings: ComxSettings | None = None) -> str:
     comx_settings = comx_settings or ComxSettings()
     match get_use_testnet():
         case True:
             node_url = random.choice(comx_settings.TESTNET_NODE_URLS)
         case False:
             node_url = random.choice(comx_settings.NODE_URLS)
-    node_url = random.choice(comx_settings.NODE_URLS)
     print(f"Using node: {node_url}")
     return node_url
 
 
 def make_client():
     """
     Create a client to the Commune network.
```

### Comparing `communex-0.1.8/src/communex/cli/_common.py` & `communex-0.1.9/src/communex/cli/_common.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/balance.py` & `communex-0.1.9/src/communex/cli/balance.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/key.py` & `communex-0.1.9/src/communex/cli/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/misc.py` & `communex-0.1.9/src/communex/cli/misc.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/module.py` & `communex-0.1.9/src/communex/cli/module.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/network.py` & `communex-0.1.9/src/communex/cli/network.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/root.py` & `communex-0.1.9/src/communex/cli/root.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/cli/subnet.py` & `communex-0.1.9/src/communex/cli/subnet.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/client.py` & `communex-0.1.9/src/communex/client.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/compat/_util.py` & `communex-0.1.9/src/communex/compat/_util.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/compat/key.py` & `communex-0.1.9/src/communex/compat/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/compat/storage.py` & `communex-0.1.9/src/communex/compat/storage.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/key.py` & `communex-0.1.9/src/communex/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/misc.py` & `communex-0.1.9/src/communex/misc.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/_ip_limiter.py` & `communex-0.1.9/src/communex/module/_ip_limiter.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/_signer.py` & `communex-0.1.9/src/communex/module/_signer.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/client.py` & `communex-0.1.9/src/communex/module/client.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/example/gpt.py` & `communex-0.1.9/src/communex/module/example/gpt.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/example/openai.py` & `communex-0.1.9/src/communex/module/example/openai.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/module.py` & `communex-0.1.9/src/communex/module/module.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/module/server.py` & `communex-0.1.9/src/communex/module/server.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/types.py` & `communex-0.1.9/src/communex/types.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/src/communex/util.py` & `communex-0.1.9/src/communex/util.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.8/PKG-INFO` & `communex-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communex
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for Commune network focused on simplicity
 License: MIT
 Author: agicommies
 Author-email: info@agicommies.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

