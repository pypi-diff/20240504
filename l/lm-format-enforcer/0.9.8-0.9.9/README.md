# Comparing `tmp/lm_format_enforcer-0.9.8.tar.gz` & `tmp/lm_format_enforcer-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_format_enforcer-0.9.8.tar", max compression
+gzip compressed data, was "lm_format_enforcer-0.9.9.tar", max compression
```

## Comparing `lm_format_enforcer-0.9.8.tar` & `lm_format_enforcer-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/LICENSE
--rw-r--r--   0        0        0    12804 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/README.md
--rw-r--r--   0        0        0      850 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/__init__.py
--rw-r--r--   0        0        0     3893 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/analyzer.py
--rw-r--r--   0        0        0     6702 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/characterlevelparser.py
--rw-r--r--   0        0        0      341 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/consts.py
--rw-r--r--   0        0        0      104 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/external/__init__.py
--rw-r--r--   0        0        0    10566 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/external/jsonschemaobject.py
--rw-r--r--   0        0        0     7044 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/external/jsonschemaobjectutil.py
--rw-r--r--   0        0        0        0 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/__init__.py
--rw-r--r--   0        0        0     2595 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/exllamav2.py
--rw-r--r--   0        0        0     2820 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/haystackv1.py
--rw-r--r--   0        0        0     3518 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/haystackv2.py
--rw-r--r--   0        0        0     3572 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/llamacpp.py
--rw-r--r--   0        0        0     6769 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/transformers.py
--rw-r--r--   0        0        0     3538 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/trtllm.py
--rw-r--r--   0        0        0     2645 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/integrations/vllm.py
--rw-r--r--   0        0        0    30336 2024-04-20 06:58:47.841975 lm_format_enforcer-0.9.8/lmformatenforcer/jsonschemaparser.py
--rw-r--r--   0        0        0     3926 2024-04-20 06:58:47.845975 lm_format_enforcer-0.9.8/lmformatenforcer/regexparser.py
--rw-r--r--   0        0        0    10083 2024-04-20 06:58:47.845975 lm_format_enforcer-0.9.8/lmformatenforcer/tokenenforcer.py
--rw-r--r--   0        0        0     6813 2024-04-20 06:58:47.845975 lm_format_enforcer-0.9.8/lmformatenforcer/tokenizerprefixtree.py
--rw-r--r--   0        0        0     2664 2024-04-20 06:58:47.845975 lm_format_enforcer-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    14137 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/LICENSE
+-rw-r--r--   0        0        0    14030 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/README.md
+-rw-r--r--   0        0        0      850 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/__init__.py
+-rw-r--r--   0        0        0     3893 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/analyzer.py
+-rw-r--r--   0        0        0     6702 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/characterlevelparser.py
+-rw-r--r--   0        0        0      341 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/consts.py
+-rw-r--r--   0        0        0      104 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/external/__init__.py
+-rw-r--r--   0        0        0    10566 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/external/jsonschemaobject.py
+-rw-r--r--   0        0        0     7044 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/external/jsonschemaobjectutil.py
+-rw-r--r--   0        0        0        0 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/__init__.py
+-rw-r--r--   0        0        0     2595 2024-04-24 18:26:31.729806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/exllamav2.py
+-rw-r--r--   0        0        0     2820 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/haystackv1.py
+-rw-r--r--   0        0        0     3518 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/haystackv2.py
+-rw-r--r--   0        0        0     3572 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/llamacpp.py
+-rw-r--r--   0        0        0     6769 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/transformers.py
+-rw-r--r--   0        0        0     3538 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/trtllm.py
+-rw-r--r--   0        0        0     2645 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/integrations/vllm.py
+-rw-r--r--   0        0        0    30336 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/jsonschemaparser.py
+-rw-r--r--   0        0        0     3926 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/regexparser.py
+-rw-r--r--   0        0        0    10083 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/tokenenforcer.py
+-rw-r--r--   0        0        0     6813 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/lmformatenforcer/tokenizerprefixtree.py
+-rw-r--r--   0        0        0     2664 2024-04-24 18:26:31.733806 lm_format_enforcer-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    15363 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.9/PKG-INFO
```

### Comparing `lm_format_enforcer-0.9.8/LICENSE` & `lm_format_enforcer-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/README.md` & `lm_format_enforcer-0.9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,38 @@
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 You can also [view the notebook in GitHub](https://github.com/noamgat/lm-format-enforcer/blob/main/samples/colab_llama2_enforcer.ipynb).
 
 For the different ways to integrate with huggingface transformers, see the [unit tests](https://github.com/noamgat/lm-format-enforcer/blob/main/tests/test_transformerenforcer.py).
 
+## vLLM Server Integration
+
+LM Format Enforcer is integrated into the [vLLM](https://github.com/vllm-project/vllm) inference server. vLLM includes an [OpenAI compatible server](https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html) with added capabilities that allow using LM Format Enforcer without writing custom inference code.
+
+Use LM Format Enforcer with the vLLM OpenAI Server either by adding this [vLLM command line parameter](https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html#command-line-arguments-for-the-server):
+
+```--guided-decoding-backend lm-format-enforcer```
+
+Or on a per-request basis, by adding the `guided_decoding_backend` [extra parameter](https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html#extra-parameters-for-chat-api) to the request:
+
+```
+completion = client.chat.completions.create(
+  model="mistralai/Mistral-7B-Instruct-v0.2",
+  messages=[
+    {"role": "user", "content": "Classify this sentiment: vLLM is wonderful!"}
+  ],
+  extra_body={
+    "guided_choice": ["positive", "negative"],
+    "guided_decoding_backend": "lm-format-enforcer"
+  }
+)
+```
+Json schema and regex decoding also supported via `guided_json` and `guided_regex` parameters.
+
 ## How does it work?
 
 The library works by combining a character level parser and a tokenizer prefix tree into a smart token filtering mechanism.
 
 ![An example of the character level parser and tokenizer prefix tree in a certain timestep](https://raw.githubusercontent.com/noamgat/lm-format-enforcer/main/docs/Trees.drawio.svg?sanitize=true)
 
 ### Character Level Parser
```

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/__init__.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/__init__.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/analyzer.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/analyzer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/characterlevelparser.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/characterlevelparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/external/jsonschemaobject.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/external/jsonschemaobject.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/external/jsonschemaobjectutil.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/external/jsonschemaobjectutil.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/exllamav2.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/exllamav2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/haystackv1.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/haystackv1.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/haystackv2.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/haystackv2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/llamacpp.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/llamacpp.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/transformers.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/trtllm.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/trtllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/integrations/vllm.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/integrations/vllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/jsonschemaparser.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/jsonschemaparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/regexparser.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/regexparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/tokenenforcer.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/tokenenforcer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/lmformatenforcer/tokenizerprefixtree.py` & `lm_format_enforcer-0.9.9/lmformatenforcer/tokenizerprefixtree.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.8/pyproject.toml` & `lm_format_enforcer-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lm-format-enforcer"
-version = "0.9.8"
+version = "0.9.9"
 description = "Enforce the output format (JSON Schema, Regex etc) of a language model"
 authors = ["Noam Gat <noamgat@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noamgat/lm-format-enforcer"
 repository = "https://github.com/noamgat/lm-format-enforcer"
 documentation = "https://github.com/noamgat/lm-format-enforcer"
```

### Comparing `lm_format_enforcer-0.9.8/PKG-INFO` & `lm_format_enforcer-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-format-enforcer
-Version: 0.9.8
+Version: 0.9.9
 Summary: Enforce the output format (JSON Schema, Regex etc) of a language model
 Home-page: https://github.com/noamgat/lm-format-enforcer
 License: MIT
 Author: Noam Gat
 Author-email: noamgat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -121,14 +121,38 @@
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 You can also [view the notebook in GitHub](https://github.com/noamgat/lm-format-enforcer/blob/main/samples/colab_llama2_enforcer.ipynb).
 
 For the different ways to integrate with huggingface transformers, see the [unit tests](https://github.com/noamgat/lm-format-enforcer/blob/main/tests/test_transformerenforcer.py).
 
+## vLLM Server Integration
+
+LM Format Enforcer is integrated into the [vLLM](https://github.com/vllm-project/vllm) inference server. vLLM includes an [OpenAI compatible server](https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html) with added capabilities that allow using LM Format Enforcer without writing custom inference code.
+
+Use LM Format Enforcer with the vLLM OpenAI Server either by adding this [vLLM command line parameter](https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html#command-line-arguments-for-the-server):
+
+```--guided-decoding-backend lm-format-enforcer```
+
+Or on a per-request basis, by adding the `guided_decoding_backend` [extra parameter](https://docs.vllm.ai/en/latest/serving/openai_compatible_server.html#extra-parameters-for-chat-api) to the request:
+
+```
+completion = client.chat.completions.create(
+  model="mistralai/Mistral-7B-Instruct-v0.2",
+  messages=[
+    {"role": "user", "content": "Classify this sentiment: vLLM is wonderful!"}
+  ],
+  extra_body={
+    "guided_choice": ["positive", "negative"],
+    "guided_decoding_backend": "lm-format-enforcer"
+  }
+)
+```
+Json schema and regex decoding also supported via `guided_json` and `guided_regex` parameters.
+
 ## How does it work?
 
 The library works by combining a character level parser and a tokenizer prefix tree into a smart token filtering mechanism.
 
 ![An example of the character level parser and tokenizer prefix tree in a certain timestep](https://raw.githubusercontent.com/noamgat/lm-format-enforcer/main/docs/Trees.drawio.svg?sanitize=true)
 
 ### Character Level Parser
```

