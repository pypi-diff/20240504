# Comparing `tmp/sibila-0.4.1.tar.gz` & `tmp/sibila-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sibila-0.4.1.tar", last modified: Mon Apr 29 17:49:51 2024, max compression
+gzip compressed data, was "sibila-0.4.2.tar", last modified: Sat May  4 18:37:55 2024, max compression
```

## Comparing `sibila-0.4.1.tar` & `sibila-0.4.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.330298 sibila-0.4.1/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.1/LICENSE
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-04-29 17:49:51.330298 sibila-0.4.1/PKG-INFO
--rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3487 2024-04-29 17:34:57.000000 sibila-0.4.1/README.md
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1629 2024-04-29 16:44:20.000000 sibila-0.4.1/pyproject.toml
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-04-29 17:49:51.330298 sibila-0.4.1/setup.cfg
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.326298 sibila-0.4.1/sibila/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1312 2024-04-26 15:56:50.000000 sibila-0.4.1/sibila/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14965 2024-04-29 14:31:30.000000 sibila-0.4.1/sibila/anthropic.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.1/sibila/cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.1/sibila/context.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    10272 2024-04-27 10:05:28.000000 sibila-0.4.1/sibila/gen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.1/sibila/json_grammar.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    24981 2024-04-27 09:42:38.000000 sibila-0.4.1/sibila/json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    23826 2024-04-26 15:02:47.000000 sibila-0.4.1/sibila/llamacpp.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    16238 2024-04-29 14:31:34.000000 sibila-0.4.1/sibila/mistral.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    74638 2024-04-27 10:40:15.000000 sibila-0.4.1/sibila/model.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    47729 2024-04-29 16:00:26.000000 sibila-0.4.1/sibila/models.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.1/sibila/multigen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2489 2024-04-29 14:30:36.000000 sibila-0.4.1/sibila/null.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    21545 2024-04-27 10:52:11.000000 sibila-0.4.1/sibila/openai.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.326298 sibila-0.4.1/sibila/res/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.1/sibila/res/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14777 2024-04-27 19:34:06.000000 sibila-0.4.1/sibila/res/base_formats.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1869 2024-04-27 17:03:26.000000 sibila-0.4.1/sibila/res/base_models.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    15043 2024-04-27 10:51:43.000000 sibila-0.4.1/sibila/schema_format_openai.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.1/sibila/text_splitter.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20235 2024-04-26 15:07:47.000000 sibila-0.4.1/sibila/thread.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.1/sibila/tools.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1245 2024-04-29 15:26:33.000000 sibila-0.4.1/sibila/utils.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.330298 sibila-0.4.1/sibila.egg-info/
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/PKG-INFO
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1167 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/SOURCES.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/dependency_links.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/entry_points.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      144 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/requires.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-04-29 17:49:51.000000 sibila-0.4.1/sibila.egg-info/top_level.txt
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-04-29 17:49:51.330298 sibila-0.4.1/tests/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4037 2024-04-29 16:15:42.000000 sibila-0.4.1/tests/test_anthropic_claude-3-haiku.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    11685 2024-04-29 16:05:39.000000 sibila-0.4.1/tests/test_cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4515 2024-04-29 16:05:46.000000 sibila-0.4.1/tests/test_common_llamacpp.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8266 2024-04-29 15:07:11.000000 sibila-0.4.1/tests/test_common_llamacpp_examples.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     3780 2024-04-27 19:04:48.000000 sibila-0.4.1/tests/test_common_remote.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     7624 2024-04-27 20:12:25.000000 sibila-0.4.1/tests/test_common_remote_examples.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20543 2024-04-26 18:26:18.000000 sibila-0.4.1/tests/test_examples_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4369 2024-04-26 10:26:46.000000 sibila-0.4.1/tests/test_fireworks_mixtral.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.1/tests/test_formats.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.4.1/tests/test_json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1664 2024-04-27 17:53:16.000000 sibila-0.4.1/tests/test_llamacpp_models_dir.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     7957 2024-04-26 10:32:15.000000 sibila-0.4.1/tests/test_llamacpp_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4090 2024-04-26 10:27:01.000000 sibila-0.4.1/tests/test_mixtral_mistral_small.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4613 2024-04-04 18:27:52.000000 sibila-0.4.1/tests/test_null_extract.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4099 2024-04-29 16:16:00.000000 sibila-0.4.1/tests/test_openai_gpt35.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4086 2024-04-29 16:15:54.000000 sibila-0.4.1/tests/test_openai_gpt4.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4338 2024-04-26 10:27:29.000000 sibila-0.4.1/tests/test_together_mixtral.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.353221 sibila-0.4.2/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.2/LICENSE
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-05-04 18:37:55.353221 sibila-0.4.2/PKG-INFO
+-rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3487 2024-04-29 17:34:57.000000 sibila-0.4.2/README.md
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1629 2024-05-04 10:29:39.000000 sibila-0.4.2/pyproject.toml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-05-04 18:37:55.353221 sibila-0.4.2/setup.cfg
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.349221 sibila-0.4.2/sibila/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1312 2024-05-04 10:16:01.000000 sibila-0.4.2/sibila/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14965 2024-05-01 14:34:46.000000 sibila-0.4.2/sibila/anthropic.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.2/sibila/cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.2/sibila/context.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    10272 2024-04-27 10:05:28.000000 sibila-0.4.2/sibila/gen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.2/sibila/json_grammar.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    24981 2024-04-27 09:42:38.000000 sibila-0.4.2/sibila/json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    23826 2024-05-01 14:34:53.000000 sibila-0.4.2/sibila/llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    16238 2024-05-01 14:34:55.000000 sibila-0.4.2/sibila/mistral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    74668 2024-05-04 17:30:39.000000 sibila-0.4.2/sibila/model.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    48077 2024-05-01 10:56:43.000000 sibila-0.4.2/sibila/models.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.2/sibila/multigen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2489 2024-04-29 14:30:36.000000 sibila-0.4.2/sibila/null.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    21545 2024-05-01 14:35:09.000000 sibila-0.4.2/sibila/openai.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.349221 sibila-0.4.2/sibila/res/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.2/sibila/res/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14777 2024-04-27 19:34:06.000000 sibila-0.4.2/sibila/res/base_formats.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1996 2024-05-04 17:37:24.000000 sibila-0.4.2/sibila/res/base_models.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    15043 2024-05-01 14:35:37.000000 sibila-0.4.2/sibila/schema_format_openai.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.2/sibila/text_splitter.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20235 2024-04-26 15:07:47.000000 sibila-0.4.2/sibila/thread.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.2/sibila/tools.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1245 2024-04-29 15:26:33.000000 sibila-0.4.2/sibila/utils.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.353221 sibila-0.4.2/sibila.egg-info/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/PKG-INFO
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1167 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/SOURCES.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/dependency_links.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/entry_points.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      144 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/requires.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/top_level.txt
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.353221 sibila-0.4.2/tests/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4037 2024-04-29 16:15:42.000000 sibila-0.4.2/tests/test_anthropic_claude-3-haiku.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    11685 2024-04-29 16:05:39.000000 sibila-0.4.2/tests/test_cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4515 2024-04-29 16:05:46.000000 sibila-0.4.2/tests/test_common_llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8266 2024-04-29 15:07:11.000000 sibila-0.4.2/tests/test_common_llamacpp_examples.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     3780 2024-04-27 19:04:48.000000 sibila-0.4.2/tests/test_common_remote.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7624 2024-04-27 20:12:25.000000 sibila-0.4.2/tests/test_common_remote_examples.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20543 2024-04-26 18:26:18.000000 sibila-0.4.2/tests/test_examples_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4369 2024-04-26 10:26:46.000000 sibila-0.4.2/tests/test_fireworks_mixtral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.2/tests/test_formats.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.4.2/tests/test_json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1664 2024-04-27 17:53:16.000000 sibila-0.4.2/tests/test_llamacpp_models_dir.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7957 2024-04-26 10:32:15.000000 sibila-0.4.2/tests/test_llamacpp_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4090 2024-04-26 10:27:01.000000 sibila-0.4.2/tests/test_mixtral_mistral_small.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4613 2024-04-04 18:27:52.000000 sibila-0.4.2/tests/test_null_extract.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4099 2024-04-29 16:16:00.000000 sibila-0.4.2/tests/test_openai_gpt35.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4086 2024-04-29 16:15:54.000000 sibila-0.4.2/tests/test_openai_gpt4.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4338 2024-04-26 10:27:29.000000 sibila-0.4.2/tests/test_together_mixtral.py
```

### Comparing `sibila-0.4.1/LICENSE` & `sibila-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/PKG-INFO` & `sibila-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.4.1
+Version: 0.4.2
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
```

### Comparing `sibila-0.4.1/README.md` & `sibila-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/pyproject.toml` & `sibila-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/__init__.py` & `sibila-0.4.2/sibila/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Structured data from local or remote LLM models."""
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 __all__ = [
     "Models",
     "Model", "TextModel", "MessagesModel", "Tokenizer",
     "GenConf", "GenRes", "GenError", "GenOut",
     "AnthropicModel",
     "FireworksModel",
```

### Comparing `sibila-0.4.1/sibila/anthropic.py` & `sibila-0.4.2/sibila/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,18 +428,18 @@
         """Model description."""
         return f"AnthropicModel: {self._model_name}"
 
 
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
-        Ex. anthropic 0.25.6
+        Ex. anthropic-0.25.6
         """
         try:
             import anthropic
             ver = anthropic.__version__
         except Exception:
             raise ImportError("Please install anthropic API by running: pip install anthropic")
             
-        return f"anthropic {ver}"
+        return f"anthropic-{ver}"
```

### Comparing `sibila-0.4.1/sibila/cli.py` & `sibila-0.4.2/sibila/cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/context.py` & `sibila-0.4.2/sibila/context.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/gen.py` & `sibila-0.4.2/sibila/gen.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/json_grammar.py` & `sibila-0.4.2/sibila/json_grammar.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/json_schema.py` & `sibila-0.4.2/sibila/json_schema.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/llamacpp.py` & `sibila-0.4.2/sibila/llamacpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,23 +343,23 @@
         """Model description."""
         return f"{type(self).__name__}: {self._model_path} - '{self._llama._model.desc()}'"
 
         
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
-        Ex. llama-cpp-python 0.2.44
+        Ex. llama-cpp-python-0.2.44
         """
         try:        
             import llama_cpp
             ver = llama_cpp.__version__
         except Exception:
             raise ImportError("Please install llama-cpp-python by running: pip install llama-cpp-python")
             
-        return f"llama-cpp-python {ver}"
+        return f"llama-cpp-python-{ver}"
 
 
 
 
 
     @property
     def n_embd(self) -> int:
```

### Comparing `sibila-0.4.1/sibila/mistral.py` & `sibila-0.4.2/sibila/mistral.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,16 +473,16 @@
         """Model description."""
         return f"MistralModel: {self._model_name}"
 
 
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
-        Ex. mistralai 0.1.8
+        Ex. mistralai-0.1.8
         """
         try:
             ver = MistralClient()._version
         except Exception:
             raise ImportError("Please install mistralai by running: pip install mistralai")
             
-        return f"mistralai {ver}"
+        return f"mistralai-{ver}"
```

### Comparing `sibila-0.4.1/sibila/model.py` & `sibila-0.4.2/sibila/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1548,15 +1548,15 @@
     def resolve_genconf_max_tokens(self,
                                    input_token_len: int,
                                    genconf: GenConf) -> int:
         """Resolve genconf.max_tokens to a definitive value, depending on input, ctx_len and max_tokens_limit"""
         
         avail_output_tokens = self.calc_max_max_tokens(input_token_len)
         if avail_output_tokens <= 0:
-            raise ValueError(f"""Input token length ({input_token_len}) doesn't fit available ctx_len ({self.ctx_len})""")
+            raise ValueError(f"""Input token length ({input_token_len}) doesn't fit available ctx_len ({self.ctx_len}) or max_tokens_limit ({self.max_tokens_limit})""")
 
         # calc maximum possible output
         resolved_max_tokens = genconf.resolve_max_tokens(self.ctx_len, self.max_tokens_limit)
 
         # ensure avail_output_tokens fits resolved_max_tokens
         max_tokens = min(resolved_max_tokens, avail_output_tokens)
         return max_tokens
@@ -1597,25 +1597,25 @@
                f"genconf={self.genconf}"
                
 
     @classmethod
     @abstractmethod
     def provider_version(cls) -> str:
         """Provider library version: provider x.y.z
-        Ex. llama-cpp-python 0.2.44
+        Ex. llama-cpp-python-0.2.44
         """
         ...
 
     @classmethod
     def version(cls) -> str:
         """Sibila version + provider version
-        Ex: sibila='0.2.3' provider='llama-cpp-python 0.2.44'        
+        Ex: sibila=0.2.3 provider=llama-cpp-python-0.2.44
         """        
         from .__init__ import __version__ as version  # type: ignore[import-not-found]
-        return f"sibila='{version}' provider='{cls.provider_version()}'"
+        return f"sibila={version} provider={cls.provider_version()}"
         
 
 
     def __str__(self):
         return self.desc_info()
```

### Comparing `sibila-0.4.1/sibila/models.py` & `sibila-0.4.2/sibila/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,22 +329,27 @@
     def create(cls,
                res_name: str,
 
                # common to all providers
                genconf: Optional[GenConf] = None,
                ctx_len: Optional[int] = None,
 
+               *,
+               # debug/testing
+               resolved_create_args: Optional[dict] = None,
+
                # model-specific overriding:
                **over_args: Union[Any]) -> Model:
         """Create a model.
 
         Args:
             res_name: Resource name in the format: provider:model_name, for example "llamacpp:openchat".
             genconf: Optional model generation configuration. Overrides set_genconf() value and any directory defaults. Defaults to None.
             ctx_len: Maximum context length to be used. Overrides directory defaults. Defaults to None.
+            resolved_create_args: Pass an empty dict to be filled by this method with the resolved args used in model creation. Defaults to None.
             over_args: Model-specific creation args, which will override default args set in model directory.
 
         Returns:
             Model: the initialized model.
         """
                
         try:
@@ -362,14 +367,17 @@
         elif "genconf" in args and isinstance(args["genconf"], dict):
             # transform dict into a GenConf instance:
             args["genconf"] = GenConf.from_dict(args["genconf"])
 
         if ctx_len is not None:
             args["ctx_len"] = ctx_len
 
+        if resolved_create_args is not None:
+            resolved_create_args.update(args)
+
 
         logger.debug(f"Resolved '{res_name}' to '{provider}:{name}' with args: {args}")
 
 
         model: Model
         if provider == "anthropic":
```

### Comparing `sibila-0.4.1/sibila/multigen.py` & `sibila-0.4.2/sibila/multigen.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/null.py` & `sibila-0.4.2/sibila/null.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/openai.py` & `sibila-0.4.2/sibila/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,23 +543,23 @@
         """Model description."""
         return f"{type(self).__name__}: '{self._model_name}'"
 
 
     @classmethod
     def provider_version(_) -> str:
         """Provider library version: provider x.y.z
-        Ex. openai 1.3.6
+        Ex. openai-1.3.6
         """
         try:        
             import openai
             ver = openai.__version__
         except Exception:
             raise ImportError("Please install openai by running: pip install openai")
             
-        return f"openai {ver}"
+        return f"openai-{ver}"
```

### Comparing `sibila-0.4.1/sibila/res/base_formats.json` & `sibila-0.4.2/sibila/res/base_formats.json`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/res/base_models.json` & `sibila-0.4.2/sibila/res/base_models.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9847056878306878%*

 * *Differences: {"'openai'": "{'_default': {'ctx_len': 8192, 'max_tokens_limit': 4096}, 'gpt-4-0125-preview': "*

 * *             "{delete: ['max_tokens_limit']}, 'gpt-4-1106-preview': {delete: "*

 * *             "['max_tokens_limit']}, 'gpt-4-0613': {'max_tokens_limit': None}, 'gpt-4-0314': "*

 * *             "{'max_tokens_limit': None}, 'gpt-4-32k-0613': {'max_tokens_limit': None}, "*

 * *             "'gpt-4-32k-0314': {'max_tokens_limit': None}, 'gpt-3.5-turbo-0125': {delete: "*

 * *             "['max_tokens_limit']}, 'gpt-3.5-turbo-1106':  […]*

```diff
@@ -21,61 +21,65 @@
         "_default": {
             "ctx_len": 32768,
             "token_estimation_factor": 0.4
         }
     },
     "openai": {
         "_default": {
-            "ctx_len": 4096,
+            "ctx_len": 8192,
+            "max_tokens_limit": 4096,
             "overhead_per_msg": 3,
             "token_estimation_factor": 0.4
         },
-        "gpt-3": "gpt-3.5-turbo-1106",
-        "gpt-3.5": "gpt-3.5-turbo-1106",
+        "gpt-3": "gpt-3.5-turbo-0125",
+        "gpt-3.5": "gpt-3.5-turbo-0125",
         "gpt-3.5-turbo": "gpt-3.5-turbo-0125",
         "gpt-3.5-turbo-0125": {
-            "ctx_len": 16385,
-            "max_tokens_limit": 4096
+            "ctx_len": 16385
         },
         "gpt-3.5-turbo-0301": {
             "ctx_len": 4096,
+            "max_tokens_limit": null,
             "overhead_per_msg": 4
         },
         "gpt-3.5-turbo-0613": {
-            "ctx_len": 4096
+            "ctx_len": 4096,
+            "max_tokens_limit": null
         },
         "gpt-3.5-turbo-1106": {
-            "ctx_len": 16385,
-            "max_tokens_limit": 4096
+            "ctx_len": 16385
         },
         "gpt-3.5-turbo-16k": "gpt-3.5-turbo-16k-0613",
         "gpt-3.5-turbo-16k-0613": {
-            "ctx_len": 16385
+            "ctx_len": 16385,
+            "max_tokens_limit": null
         },
         "gpt-4": "gpt-4-1106-preview",
         "gpt-4-0125-preview": {
-            "ctx_len": 128000,
-            "max_tokens_limit": 4096
+            "ctx_len": 128000
         },
         "gpt-4-0314": {
-            "ctx_len": 8192
+            "ctx_len": 8192,
+            "max_tokens_limit": null
         },
         "gpt-4-0613": {
-            "ctx_len": 8192
+            "ctx_len": 8192,
+            "max_tokens_limit": null
         },
         "gpt-4-1106-preview": {
-            "ctx_len": 128000,
-            "max_tokens_limit": 4096
+            "ctx_len": 128000
         },
         "gpt-4-32k": "gpt-4-32k-0613",
         "gpt-4-32k-0314": {
-            "ctx_len": 32768
+            "ctx_len": 32768,
+            "max_tokens_limit": null
         },
         "gpt-4-32k-0613": {
-            "ctx_len": 32768
+            "ctx_len": 32768,
+            "max_tokens_limit": null
         },
         "gpt-4-turbo": "gpt-4-turbo-2024-04-09",
         "gpt-4-turbo-2024-04-09": {
             "ctx_len": 128000
         },
         "gpt-4-turbo-preview": "gpt-4-0125-preview"
     },
```

### Comparing `sibila-0.4.1/sibila/schema_format_openai.py` & `sibila-0.4.2/sibila/schema_format_openai.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/text_splitter.py` & `sibila-0.4.2/sibila/text_splitter.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/thread.py` & `sibila-0.4.2/sibila/thread.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/tools.py` & `sibila-0.4.2/sibila/tools.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila/utils.py` & `sibila-0.4.2/sibila/utils.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/sibila.egg-info/PKG-INFO` & `sibila-0.4.2/sibila.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.4.1
+Version: 0.4.2
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
```

### Comparing `sibila-0.4.1/sibila.egg-info/SOURCES.txt` & `sibila-0.4.2/sibila.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_anthropic_claude-3-haiku.py` & `sibila-0.4.2/tests/test_anthropic_claude-3-haiku.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_cli.py` & `sibila-0.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_common_llamacpp.py` & `sibila-0.4.2/tests/test_common_llamacpp.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_common_llamacpp_examples.py` & `sibila-0.4.2/tests/test_common_llamacpp_examples.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_common_remote.py` & `sibila-0.4.2/tests/test_common_remote.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_common_remote_examples.py` & `sibila-0.4.2/tests/test_common_remote_examples.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_examples_tinyllama.py` & `sibila-0.4.2/tests/test_examples_tinyllama.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_fireworks_mixtral.py` & `sibila-0.4.2/tests/test_fireworks_mixtral.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_formats.py` & `sibila-0.4.2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_json_schema.py` & `sibila-0.4.2/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_llamacpp_models_dir.py` & `sibila-0.4.2/tests/test_llamacpp_models_dir.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_llamacpp_tinyllama.py` & `sibila-0.4.2/tests/test_llamacpp_tinyllama.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_mixtral_mistral_small.py` & `sibila-0.4.2/tests/test_mixtral_mistral_small.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_null_extract.py` & `sibila-0.4.2/tests/test_null_extract.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_openai_gpt35.py` & `sibila-0.4.2/tests/test_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_openai_gpt4.py` & `sibila-0.4.2/tests/test_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.1/tests/test_together_mixtral.py` & `sibila-0.4.2/tests/test_together_mixtral.py`

 * *Files identical despite different names*

