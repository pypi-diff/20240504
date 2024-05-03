# Comparing `tmp/martian_adapters-4.2.0.tar.gz` & `tmp/martian_adapters-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-4.2.0.tar", max compression
+gzip compressed data, was "martian_adapters-4.2.1.tar", max compression
```

## Comparing `martian_adapters-4.2.0.tar` & `martian_adapters-4.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35149 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/LICENSE
--rw-r--r--   0        0        0     3452 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/README.md
--rw-r--r--   0        0        0      725 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     3347 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2386 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0     3419 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5816 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     5812 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3429 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0      942 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9225 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4102 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2412 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2384 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1836 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2450 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2604 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    10017 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/rate_limiter.py
--rw-r--r--   0        0        0      335 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/requirements.txt
--rw-r--r--   0        0        0     6903 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-03 19:23:19.515366 martian_adapters-4.2.0/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1170 2024-05-03 19:23:19.519366 martian_adapters-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 martian_adapters-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/LICENSE
+-rw-r--r--   0        0        0     3452 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/README.md
+-rw-r--r--   0        0        0      725 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     3347 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2386 2024-05-03 19:56:26.462288 martian_adapters-4.2.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0     3419 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5816 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     5812 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3429 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0      942 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9225 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4102 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2412 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2587 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1836 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2450 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2604 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    10017 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      335 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/requirements.txt
+-rw-r--r--   0        0        0     6903 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1170 2024-05-03 19:56:26.466288 martian_adapters-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 martian_adapters-4.2.1/PKG-INFO
```

### Comparing `martian_adapters-4.2.0/LICENSE` & `martian_adapters-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/README.md` & `martian_adapters-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/__init__.py` & `martian_adapters-4.2.1/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-4.2.1/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/adapter_factory.py` & `martian_adapters-4.2.1/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-4.2.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/__init__.py` & `martian_adapters-4.2.1/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,20 @@
     FireworksModel(
         name="mistral-7b-instruct-4k",
         cost=Cost(prompt=0.20e-6, completion=0.20e-6),
         context_length=32_768,
         vendor_name="accounts/fireworks/models",
     ),
     FireworksModel(
+        name="mistral-7b-instruct-v0p2",
+        cost=Cost(prompt=0.20e-6, completion=0.20e-6),
+        context_length=32_768,
+        vendor_name="accounts/fireworks/models",
+    ),
+    FireworksModel(
         name="mixtral-8x22b-instruct",
         cost=Cost(prompt=0.90e-6, completion=0.90e-6),
         context_length=65_536,
         vendor_name="accounts/fireworks/models",
     ),
     FireworksModel(
         name="mixtral-8x7b-instruct",
```

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-4.2.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/rate_limiter.py` & `martian_adapters-4.2.1/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/types.py` & `martian_adapters-4.2.1/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/utils/general_utils.py` & `martian_adapters-4.2.1/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/utils/network_utils.py` & `martian_adapters-4.2.1/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/adapters/utils/openai_client_factory.py` & `martian_adapters-4.2.1/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.2.0/pyproject.toml` & `martian_adapters-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "4.2.0"
+version = "4.2.1"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-4.2.0/PKG-INFO` & `martian_adapters-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 4.2.0
+Version: 4.2.1
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
```

