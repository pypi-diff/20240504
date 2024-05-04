# Comparing `tmp/magentic-0.9.0.tar.gz` & `tmp/magentic-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magentic-0.9.0.tar", max compression
+gzip compressed data, was "magentic-0.9.1.tar", max compression
```

## Comparing `magentic-0.9.0.tar` & `magentic-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-11-06 05:08:40.483947 magentic-0.9.0/LICENSE
--rw-r--r--   0        0        0    15121 2023-11-06 05:08:40.483947 magentic-0.9.0/README.md
--rw-r--r--   0        0        0     2250 2023-11-06 05:08:40.487947 magentic-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      684 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/__init__.py
--rw-r--r--   0        0        0     1116 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/backend.py
--rw-r--r--   0        0        0     4238 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat.py
--rw-r--r--   0        0        0        0 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat_model/__init__.py
--rw-r--r--   0        0        0     3816 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat_model/base.py
--rw-r--r--   0        0        0     9083 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat_model/function_schema.py
--rw-r--r--   0        0        0    13036 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat_model/litellm_chat_model.py
--rw-r--r--   0        0        0     2895 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat_model/message.py
--rw-r--r--   0        0        0    15295 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chat_model/openai_chat_model.py
--rw-r--r--   0        0        0     6796 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/chatprompt.py
--rw-r--r--   0        0        0     1478 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/function_call.py
--rw-r--r--   0        0        0     3164 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/prompt_chain.py
--rw-r--r--   0        0        0     5644 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/prompt_function.py
--rw-r--r--   0        0        0       61 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/py.typed
--rw-r--r--   0        0        0      637 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/settings.py
--rw-r--r--   0        0        0     4532 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/streaming.py
--rw-r--r--   0        0        0     2165 2023-11-06 05:08:40.487947 magentic-0.9.0/src/magentic/typing.py
--rw-r--r--   0        0        0    15891 1970-01-01 00:00:00.000000 magentic-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-11-07 05:04:45.362364 magentic-0.9.1/LICENSE
+-rw-r--r--   0        0        0    15121 2023-11-07 05:04:45.362364 magentic-0.9.1/README.md
+-rw-r--r--   0        0        0     2255 2023-11-07 05:04:45.366364 magentic-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      684 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/__init__.py
+-rw-r--r--   0        0        0     1116 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/backend.py
+-rw-r--r--   0        0        0     4238 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat.py
+-rw-r--r--   0        0        0        0 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat_model/__init__.py
+-rw-r--r--   0        0        0     3816 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat_model/base.py
+-rw-r--r--   0        0        0     9083 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat_model/function_schema.py
+-rw-r--r--   0        0        0    13036 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat_model/litellm_chat_model.py
+-rw-r--r--   0        0        0     2895 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat_model/message.py
+-rw-r--r--   0        0        0    15295 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chat_model/openai_chat_model.py
+-rw-r--r--   0        0        0     6796 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/chatprompt.py
+-rw-r--r--   0        0        0     1478 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/function_call.py
+-rw-r--r--   0        0        0     3164 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/prompt_chain.py
+-rw-r--r--   0        0        0     5644 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/prompt_function.py
+-rw-r--r--   0        0        0       61 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/py.typed
+-rw-r--r--   0        0        0      637 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/settings.py
+-rw-r--r--   0        0        0     4532 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/streaming.py
+-rw-r--r--   0        0        0     2165 2023-11-07 05:04:45.366364 magentic-0.9.1/src/magentic/typing.py
+-rw-r--r--   0        0        0    15896 1970-01-01 00:00:00.000000 magentic-0.9.1/PKG-INFO
```

### Comparing `magentic-0.9.0/LICENSE` & `magentic-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/README.md` & `magentic-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/pyproject.toml` & `magentic-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 module = [
     "litellm",
 ]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "magentic"
-version = "0.9.0"
+version = "0.9.1"
 description = "Seamlessly integrate LLMs as Python functions"
 license = "MIT"
 authors = ["Jack Collins"]
 readme = "README.md"
 repository = "https://github.com/jackmpcollins/magentic"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 litellm = {version = ">=0.8.4", optional = true}
-openai = ">=0.27"
+openai = ">=0.27,<1.0"
 pydantic = ">=2.0.0"
 pydantic-settings = ">=2.0.0"
 
 [tool.poetry.extras]
 litellm = ["litellm"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `magentic-0.9.0/src/magentic/__init__.py` & `magentic-0.9.1/src/magentic/__init__.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/backend.py` & `magentic-0.9.1/src/magentic/backend.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chat.py` & `magentic-0.9.1/src/magentic/chat.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chat_model/base.py` & `magentic-0.9.1/src/magentic/chat_model/base.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chat_model/function_schema.py` & `magentic-0.9.1/src/magentic/chat_model/function_schema.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chat_model/litellm_chat_model.py` & `magentic-0.9.1/src/magentic/chat_model/litellm_chat_model.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chat_model/message.py` & `magentic-0.9.1/src/magentic/chat_model/message.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chat_model/openai_chat_model.py` & `magentic-0.9.1/src/magentic/chat_model/openai_chat_model.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/chatprompt.py` & `magentic-0.9.1/src/magentic/chatprompt.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/function_call.py` & `magentic-0.9.1/src/magentic/function_call.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/prompt_chain.py` & `magentic-0.9.1/src/magentic/prompt_chain.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/prompt_function.py` & `magentic-0.9.1/src/magentic/prompt_function.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/settings.py` & `magentic-0.9.1/src/magentic/settings.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/streaming.py` & `magentic-0.9.1/src/magentic/streaming.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/src/magentic/typing.py` & `magentic-0.9.1/src/magentic/typing.py`

 * *Files identical despite different names*

### Comparing `magentic-0.9.0/PKG-INFO` & `magentic-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: magentic
-Version: 0.9.0
+Version: 0.9.1
 Summary: Seamlessly integrate LLMs as Python functions
 Home-page: https://github.com/jackmpcollins/magentic
 License: MIT
 Author: Jack Collins
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: litellm
 Requires-Dist: litellm (>=0.8.4) ; extra == "litellm"
-Requires-Dist: openai (>=0.27)
+Requires-Dist: openai (>=0.27,<1.0)
 Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: pydantic-settings (>=2.0.0)
 Project-URL: Repository, https://github.com/jackmpcollins/magentic
 Description-Content-Type: text/markdown
 
 # magentic
```

