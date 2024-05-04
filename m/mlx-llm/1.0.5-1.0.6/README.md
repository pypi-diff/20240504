# Comparing `tmp/mlx_llm-1.0.5.tar.gz` & `tmp/mlx_llm-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_llm-1.0.5.tar", max compression
+gzip compressed data, was "mlx_llm-1.0.6.tar", max compression
```

## Comparing `mlx_llm-1.0.5.tar` & `mlx_llm-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     7020 2023-12-17 18:14:37.703503 mlx_llm-1.0.5/LICENSE
--rw-r--r--   0        0        0     4725 2024-04-30 12:51:36.132834 mlx_llm-1.0.5/README.md
--rw-r--r--   0        0        0     2346 2024-04-30 12:51:36.134698 mlx_llm-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-30 12:51:36.135519 mlx_llm-1.0.5/src/mlx_llm/__init__.py
--rw-r--r--   0        0        0       37 2024-04-26 13:24:58.257004 mlx_llm-1.0.5/src/mlx_llm/chat/__init__.py
--rw-r--r--   0        0        0     4097 2024-04-30 08:49:32.694862 mlx_llm-1.0.5/src/mlx_llm/chat/chat.py
--rw-r--r--   0        0        0      449 2024-04-26 13:24:58.258114 mlx_llm-1.0.5/src/mlx_llm/chat/utils.py
--rw-r--r--   0        0        0      132 2024-04-26 13:24:58.258969 mlx_llm-1.0.5/src/mlx_llm/model/__init__.py
--rw-r--r--   0        0        0      447 2024-04-30 08:49:32.695556 mlx_llm-1.0.5/src/mlx_llm/model/_config.py
--rw-r--r--   0        0        0     4742 2024-04-30 12:33:49.101839 mlx_llm-1.0.5/src/mlx_llm/model/_factory.py
--rw-r--r--   0        0        0    20811 2024-04-30 12:51:36.136081 mlx_llm-1.0.5/src/mlx_llm/model/_registry.py
--rw-r--r--   0        0        0     6428 2024-04-30 08:49:32.697930 mlx_llm-1.0.5/src/mlx_llm/model/_utils.py
--rw-r--r--   0        0        0     8795 2024-04-30 09:29:36.399989 mlx_llm-1.0.5/src/mlx_llm/model/converter.py
--rw-r--r--   0        0        0    14301 2024-04-30 08:49:32.699154 mlx_llm-1.0.5/src/mlx_llm/model/transformer.py
--rw-r--r--   0        0        0     1235 2024-04-30 12:51:36.136498 mlx_llm-1.0.5/src/mlx_llm/prompt/__init__.py
--rw-r--r--   0        0        0      287 2024-04-26 13:24:58.264679 mlx_llm-1.0.5/src/mlx_llm/prompt/_base.py
--rw-r--r--   0        0        0     1691 2024-04-30 08:49:32.699930 mlx_llm-1.0.5/src/mlx_llm/prompt/gemma.py
--rw-r--r--   0        0        0     4337 2024-04-30 12:51:36.136950 mlx_llm-1.0.5/src/mlx_llm/prompt/llama.py
--rw-r--r--   0        0        0     3083 2024-04-30 12:51:36.137351 mlx_llm-1.0.5/src/mlx_llm/prompt/mistral.py
--rw-r--r--   0        0        0     1394 2024-04-30 12:51:36.137509 mlx_llm-1.0.5/src/mlx_llm/prompt/openelm.py
--rw-r--r--   0        0        0      559 2024-04-26 13:24:58.266273 mlx_llm-1.0.5/src/mlx_llm/prompt/phi.py
--rw-r--r--   0        0        0        1 2024-04-26 13:24:58.267232 mlx_llm-1.0.5/src/mlx_llm/utils/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-26 13:24:58.267997 mlx_llm-1.0.5/src/mlx_llm/utils/hf.py
--rw-r--r--   0        0        0     4810 2024-04-26 13:24:58.268439 mlx_llm-1.0.5/src/mlx_llm/utils/session.py
--rw-r--r--   0        0        0     1261 2024-02-09 16:22:28.193671 mlx_llm-1.0.5/src/mlx_llm/utils/time.py
--rw-r--r--   0        0        0     2258 2024-04-30 09:29:35.029759 mlx_llm-1.0.5/src/mlx_llm/utils/weights.py
--rw-r--r--   0        0        0     5634 1970-01-01 00:00:00.000000 mlx_llm-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     7020 2023-12-17 18:14:37.703503 mlx_llm-1.0.6/LICENSE
+-rw-r--r--   0        0        0     4941 2024-05-04 15:39:12.337372 mlx_llm-1.0.6/README.md
+-rw-r--r--   0        0        0     2346 2024-05-04 15:39:12.338078 mlx_llm-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-04 15:39:12.338525 mlx_llm-1.0.6/src/mlx_llm/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-26 13:24:58.257004 mlx_llm-1.0.6/src/mlx_llm/chat/__init__.py
+-rw-r--r--   0        0        0     4160 2024-05-04 15:39:12.339060 mlx_llm-1.0.6/src/mlx_llm/chat/chat.py
+-rw-r--r--   0        0        0      449 2024-04-26 13:24:58.258114 mlx_llm-1.0.6/src/mlx_llm/chat/utils.py
+-rw-r--r--   0        0        0      132 2024-04-26 13:24:58.258969 mlx_llm-1.0.6/src/mlx_llm/model/__init__.py
+-rw-r--r--   0        0        0      447 2024-05-04 15:07:20.959149 mlx_llm-1.0.6/src/mlx_llm/model/_config.py
+-rw-r--r--   0        0        0     4742 2024-05-04 15:15:41.932387 mlx_llm-1.0.6/src/mlx_llm/model/_factory.py
+-rw-r--r--   0        0        0    21934 2024-05-04 15:39:12.339470 mlx_llm-1.0.6/src/mlx_llm/model/_registry.py
+-rw-r--r--   0        0        0     6428 2024-04-30 08:49:32.697930 mlx_llm-1.0.6/src/mlx_llm/model/_utils.py
+-rw-r--r--   0        0        0     8795 2024-04-30 09:29:36.399989 mlx_llm-1.0.6/src/mlx_llm/model/converter.py
+-rw-r--r--   0        0        0    14301 2024-04-30 08:49:32.699154 mlx_llm-1.0.6/src/mlx_llm/model/transformer.py
+-rw-r--r--   0        0        0     1226 2024-05-04 15:39:12.340014 mlx_llm-1.0.6/src/mlx_llm/prompt/__init__.py
+-rw-r--r--   0        0        0      287 2024-05-04 15:06:41.516089 mlx_llm-1.0.6/src/mlx_llm/prompt/_base.py
+-rw-r--r--   0        0        0     1691 2024-04-30 08:49:32.699930 mlx_llm-1.0.6/src/mlx_llm/prompt/gemma.py
+-rw-r--r--   0        0        0     2460 2024-05-04 15:39:12.340265 mlx_llm-1.0.6/src/mlx_llm/prompt/hermes.py
+-rw-r--r--   0        0        0     4337 2024-04-30 12:51:36.136950 mlx_llm-1.0.6/src/mlx_llm/prompt/llama.py
+-rw-r--r--   0        0        0     3083 2024-04-30 12:51:36.137351 mlx_llm-1.0.6/src/mlx_llm/prompt/mistral.py
+-rw-r--r--   0        0        0     1394 2024-04-30 12:51:36.137509 mlx_llm-1.0.6/src/mlx_llm/prompt/openelm.py
+-rw-r--r--   0        0        0      559 2024-04-26 13:24:58.266273 mlx_llm-1.0.6/src/mlx_llm/prompt/phi.py
+-rw-r--r--   0        0        0        1 2024-04-26 13:24:58.267232 mlx_llm-1.0.6/src/mlx_llm/utils/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-26 13:24:58.267997 mlx_llm-1.0.6/src/mlx_llm/utils/hf.py
+-rw-r--r--   0        0        0     4810 2024-05-04 15:06:58.586214 mlx_llm-1.0.6/src/mlx_llm/utils/session.py
+-rw-r--r--   0        0        0     1261 2024-02-09 16:22:28.193671 mlx_llm-1.0.6/src/mlx_llm/utils/time.py
+-rw-r--r--   0        0        0     2258 2024-04-30 09:29:35.029759 mlx_llm-1.0.6/src/mlx_llm/utils/weights.py
+-rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 mlx_llm-1.0.6/PKG-INFO
```

### Comparing `mlx_llm-1.0.5/LICENSE` & `mlx_llm-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/README.md` & `mlx_llm-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## **Models 🧠**
 
 Currently, out-of-the-box supported models are:
 
 | Family        |  Models |
 |---------------------|----------------|
 | LLaMA 2                  |     llama_2_7b_chat_hf, llama_2_7b_hf            |
-| LLaMA 3          |  llama_3_8b, llama_3_8b_instruct              |
+| LLaMA 3          |  llama_3_8b, llama_3_8b_instruct, hermes_2_pro_llama_3_8b              |
 | Phi3 |   phi_3_mini_4k_instruct, phi_3_mini_128k_instruct           |
 | Mistral |  mistral_7b_instruct_v0.2, openhermes_2.5_mistral_7b, starling_lm_7b_beta          |
 | TinyLLaMA |     tiny_llama_1.1B_chat_v1.0       |
 | Gemma |  gemma_1.1_2b_it, gemma_1.1_7b_it                    |
 | OpenELM |  openelm_270M_instruct, openelm_450M_instruct, openelm_1.1B_instruct, openelm_3B_instruct |
 
 To create a model with pre-trained weights from HuggingFace:
@@ -108,14 +108,15 @@
 from mlx_llm.model import create_model, create_tokenizer
 from mlx_llm.prompt import create_prompt
 
 model_name = "tiny_llama_1.1B_chat_v1.0"
 
 chat = LLMChat(
     model_name=model_name,
+    prompt_family="tinyllama",
     chat_setup=ChatSetup(
         system="You are Michael Scott from The Office. Your goal is to answer like hime, so be funny and inappropriate, but be brief.",
         history=[
             {"question": "What is your name?", "answer": "Michael Scott"},
             {"question": "What is your favorite episode of The Office?", "answer": "The Dinner Party"},
         ],
     ),
@@ -124,14 +125,17 @@
 
 chat.start()
 ```
 
 > [!WARNING]
 > In current release (v1.0.5) OpenELM chat-mode is broken. I am working on fixing it.
 
+> [!WARNING]
+> In current release (v1.0.5) chat mode is supported only for registered models and mode with other HF weights from HuggingFace is not supported.
+
 ### **Fine-Tuning with LoRA or QLoRA 🚀**
 ```python
 raise NotImplementedError
 ```
 
 ### **Retrieval Augmented Generation (RAG) 📚**
 ```python
```

### Comparing `mlx_llm-1.0.5/pyproject.toml` & `mlx_llm-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlx_llm"
-version = "1.0.5"
+version = "1.0.6"
 description = "Large Language Models (LLMs) applications and tools running on Apple Silicon in real-time with Apple MLX"
 authors = ["Riccardo Musmeci <riccardomusmeci92@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "mlx_llm", from = "src" },
 ]
```

### Comparing `mlx_llm-1.0.5/src/mlx_llm/chat/chat.py` & `mlx_llm-1.0.6/src/mlx_llm/chat/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,37 @@
 
 
 class LLMChat:
     """Chat with LLM class
 
     Args:
         model_name (str): model name
+        prompt_family (str): prompt family
         chat_setup (ChatSetup): chat setup
         max_tokens (int, optional): max tokens. Defaults to 1024.
         temperature (float, optional): temperature. Defaults to 0.1.
         quantized (bool, optional): quantized. Defaults to False.
         group_size (int, optional): group size. Defaults to 64.
         bits (int, optional): bits. Defaults to 8.
     """
 
     def __init__(
         self,
         model_name: str,
+        prompt_family: str,
         chat_setup: ChatSetup,
         max_tokens: int = 1024,
         temperature: float = 0.1,
         quantized: bool = False,
         group_size: int = 64,
         bits: int = 8,
     ) -> None:
         self.model = create_model(model_name)
         self.tokenizer = create_tokenizer(model_name)
-        self.prompt = create_prompt(model_name=model_name, system=chat_setup.system)
+        self.prompt = create_prompt(prompt_family, system=chat_setup.system)
         self.session = chat_setup.session()
         self.max_tokens = max_tokens
         self.temperature = temperature
 
         if quantized:
             print(f"[INFO] Quantizing model {model_name} with group_size={group_size} and bits={bits}")
             self.model = quantize(self.model, group_size=group_size, bits=bits)
```

### Comparing `mlx_llm-1.0.5/src/mlx_llm/model/_factory.py` & `mlx_llm-1.0.6/src/mlx_llm/model/_factory.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/model/_registry.py` & `mlx_llm-1.0.6/src/mlx_llm/model/_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,49 @@
         hf=HFConfig(
             repo_id="meta-llama/Meta-Llama-3-8B-Instruct",
         ),
         converter=llama_to_mlxllm,
     )
     return model, config
 
+@register_model("hermes_2_pro_llama_3_8b")
+def hermes_2_pro_llama_3_8b(
+    vocab_size: int = 128288, norm_eps: float = 1e-5, rope_theta: float = 500000.0, rope_traditional: bool = False
+) -> Tuple[Transformer, ModelConfig]:
+    """Create a Hermes 2 Pro Llama 3 8B model.
+
+    Args:
+        vocab_size (int, optional): vocab size. Defaults to 128288.
+        norm_eps (float, optional): norm epsilon. Defaults to 1e-5.
+        rope_theta (float, optional): rope theta. Defaults to 500000.0.
+        rope_traditional (bool, optional): whether to use traditional rope. Defaults to False.
+
+    Returns:
+        Tuple[Transformer, ModelConfig]: model, config
+    """
+    model = Transformer(
+        dim=4096,
+        hidden_dim=14336,
+        vocab_size=vocab_size,
+        n_layers=32,
+        n_heads=32,
+        n_kv_heads=8,
+        norm_eps=norm_eps,
+        rope_theta=rope_theta,
+        rope_traditional=rope_traditional,
+    )
+    
+    config = ModelConfig(
+        hf=HFConfig(
+            repo_id="NousResearch/Hermes-2-Pro-Llama-3-8B",
+        ),
+        converter=llama_to_mlxllm,
+    )
+    return model, config
+
 
 @register_model("phi_3_mini_4k_instruct")
 def phi3_mini_4k_instruct(
     vocab_size: int = 32064, norm_eps: float = 1e-5, rope_theta: float = 10000.0, rope_traditional: bool = False
 ) -> Tuple[Transformer, ModelConfig]:
     """Create a Phi3 Mini 4k Instruct model.
```

### Comparing `mlx_llm-1.0.5/src/mlx_llm/model/_utils.py` & `mlx_llm-1.0.6/src/mlx_llm/model/_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/model/converter.py` & `mlx_llm-1.0.6/src/mlx_llm/model/converter.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/model/transformer.py` & `mlx_llm-1.0.6/src/mlx_llm/model/transformer.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/prompt/gemma.py` & `mlx_llm-1.0.6/src/mlx_llm/prompt/gemma.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/prompt/llama.py` & `mlx_llm-1.0.6/src/mlx_llm/prompt/llama.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/prompt/mistral.py` & `mlx_llm-1.0.6/src/mlx_llm/prompt/mistral.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/prompt/openelm.py` & `mlx_llm-1.0.6/src/mlx_llm/prompt/openelm.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/prompt/phi.py` & `mlx_llm-1.0.6/src/mlx_llm/prompt/phi.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/utils/hf.py` & `mlx_llm-1.0.6/src/mlx_llm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/utils/session.py` & `mlx_llm-1.0.6/src/mlx_llm/utils/session.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/utils/time.py` & `mlx_llm-1.0.6/src/mlx_llm/utils/time.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/src/mlx_llm/utils/weights.py` & `mlx_llm-1.0.6/src/mlx_llm/utils/weights.py`

 * *Files identical despite different names*

### Comparing `mlx_llm-1.0.5/PKG-INFO` & `mlx_llm-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx_llm
-Version: 1.0.5
+Version: 1.0.6
 Summary: Large Language Models (LLMs) applications and tools running on Apple Silicon in real-time with Apple MLX
 Author: Riccardo Musmeci
 Author-email: riccardomusmeci92@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -39,15 +39,15 @@
 ## **Models 🧠**
 
 Currently, out-of-the-box supported models are:
 
 | Family        |  Models |
 |---------------------|----------------|
 | LLaMA 2                  |     llama_2_7b_chat_hf, llama_2_7b_hf            |
-| LLaMA 3          |  llama_3_8b, llama_3_8b_instruct              |
+| LLaMA 3          |  llama_3_8b, llama_3_8b_instruct, hermes_2_pro_llama_3_8b              |
 | Phi3 |   phi_3_mini_4k_instruct, phi_3_mini_128k_instruct           |
 | Mistral |  mistral_7b_instruct_v0.2, openhermes_2.5_mistral_7b, starling_lm_7b_beta          |
 | TinyLLaMA |     tiny_llama_1.1B_chat_v1.0       |
 | Gemma |  gemma_1.1_2b_it, gemma_1.1_7b_it                    |
 | OpenELM |  openelm_270M_instruct, openelm_450M_instruct, openelm_1.1B_instruct, openelm_3B_instruct |
 
 To create a model with pre-trained weights from HuggingFace:
@@ -134,14 +134,15 @@
 from mlx_llm.model import create_model, create_tokenizer
 from mlx_llm.prompt import create_prompt
 
 model_name = "tiny_llama_1.1B_chat_v1.0"
 
 chat = LLMChat(
     model_name=model_name,
+    prompt_family="tinyllama",
     chat_setup=ChatSetup(
         system="You are Michael Scott from The Office. Your goal is to answer like hime, so be funny and inappropriate, but be brief.",
         history=[
             {"question": "What is your name?", "answer": "Michael Scott"},
             {"question": "What is your favorite episode of The Office?", "answer": "The Dinner Party"},
         ],
     ),
@@ -150,14 +151,17 @@
 
 chat.start()
 ```
 
 > [!WARNING]
 > In current release (v1.0.5) OpenELM chat-mode is broken. I am working on fixing it.
 
+> [!WARNING]
+> In current release (v1.0.5) chat mode is supported only for registered models and mode with other HF weights from HuggingFace is not supported.
+
 ### **Fine-Tuning with LoRA or QLoRA 🚀**
 ```python
 raise NotImplementedError
 ```
 
 ### **Retrieval Augmented Generation (RAG) 📚**
 ```python
```

