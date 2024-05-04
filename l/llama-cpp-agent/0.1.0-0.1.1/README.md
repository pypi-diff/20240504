# Comparing `tmp/llama_cpp_agent-0.1.0.tar.gz` & `tmp/llama_cpp_agent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.1.0.tar", last modified: Wed May  1 06:47:33 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.1.1.tar", last modified: Sat May  4 20:32:47 2024, max compression
```

## Comparing `llama_cpp_agent-0.1.0.tar` & `llama_cpp_agent-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.017607 llama_cpp_agent-0.1.0/
--rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    28305 2024-05-01 06:47:33.016606 llama_cpp_agent-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    27272 2024-05-01 06:47:04.000000 llama_cpp_agent-0.1.0/ReadMe.md
--rw-rw-rw-   0        0        0      974 2024-05-01 06:47:04.000000 llama_cpp_agent-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 06:47:33.017607 llama_cpp_agent-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:32.992569 llama_cpp_agent-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.001568 llama_cpp_agent-0.1.0/src/llama_cpp_agent/
--rw-rw-rw-   0        0        0        0 2024-01-04 14:13:41.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.009095 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/
--rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/__init__.py
--rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-rw-rw-   0        0        0     1636 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-rw-rw-   0        0        0     3830 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-rw-rw-   0        0        0    28527 2024-04-20 23:23:24.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/function_calling.py
--rw-rw-rw-   0        0        0    19266 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/function_calling_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.010097 llama_cpp_agent-0.1.0/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-rw-rw-   0        0        0    70688 2024-05-01 06:07:15.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-rw-rw-   0        0        0    47983 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/llm_agent.py
--rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/llm_prompt_template.py
--rw-rw-rw-   0        0        0     6022 2024-05-01 05:39:37.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/llm_settings.py
--rw-rw-rw-   0        0        0    21298 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/messages_formatter.py
--rw-rw-rw-   0        0        0     4314 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/output_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.013606 llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/
--rw-rw-rw-   0        0        0        0 2024-01-08 13:25:58.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/__init__.py
--rw-rw-rw-   0        0        0     7170 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
--rw-rw-rw-   0        0        0    11586 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
--rw-rw-rw-   0        0        0     6947 2024-04-29 05:14:58.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/openai_endpoint_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.014606 llama_cpp_agent-0.1.0/src/llama_cpp_agent/rag/
--rw-rw-rw-   0        0        0        0 2024-04-23 09:48:26.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/rag/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-rw-rw-   0        0        0     3895 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/rag/text_utils.py
--rw-rw-rw-   0        0        0    11104 2024-04-16 22:20:07.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent/structured_output_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:47:33.015607 llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/
--rw-rw-rw-   0        0        0    28305 2024-05-01 06:47:32.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1495 2024-05-01 06:47:32.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 06:47:32.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2024-05-01 06:47:32.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-01 06:47:32.000000 llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.792888 llama_cpp_agent-0.1.1/
+-rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    40131 2024-05-04 20:32:47.791878 llama_cpp_agent-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    39098 2024-05-04 20:30:46.000000 llama_cpp_agent-0.1.1/ReadMe.md
+-rw-rw-rw-   0        0        0      974 2024-05-04 20:30:46.000000 llama_cpp_agent-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:32:47.792888 llama_cpp_agent-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.757235 llama_cpp_agent-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.772072 llama_cpp_agent-0.1.1/src/llama_cpp_agent/
+-rw-rw-rw-   0        0        0        0 2024-01-04 14:13:41.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.782308 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/
+-rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-rw-rw-   0        0        0     1636 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-rw-rw-   0        0        0     3830 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-rw-rw-   0        0        0    13628 2024-05-04 20:30:46.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/chain.py
+-rw-rw-rw-   0        0        0    28885 2024-05-02 02:40:58.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/function_calling.py
+-rw-rw-rw-   0        0        0    19192 2024-05-04 02:23:57.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/function_calling_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.783306 llama_cpp_agent-0.1.1/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-rw-rw-   0        0        0    70837 2024-05-04 15:49:16.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-rw-rw-   0        0        0    13492 2024-05-02 06:20:18.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/hermes_2_pro_agent.py
+-rw-rw-rw-   0        0        0    47987 2024-05-03 23:42:05.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/llm_agent.py
+-rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/llm_prompt_template.py
+-rw-rw-rw-   0        0        0     6022 2024-05-01 05:39:37.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/llm_settings.py
+-rw-rw-rw-   0        0        0     8502 2024-05-03 23:16:22.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/messages.py
+-rw-rw-rw-   0        0        0    21298 2024-05-02 01:51:26.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/messages_formatter.py
+-rw-rw-rw-   0        0        0     4314 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/output_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.787304 llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/
+-rw-rw-rw-   0        0        0        0 2024-01-08 13:25:58.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/__init__.py
+-rw-rw-rw-   0        0        0     7135 2024-05-02 02:40:58.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
+-rw-rw-rw-   0        0        0    11586 2024-05-01 11:46:56.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
+-rw-rw-rw-   0        0        0     6912 2024-05-02 02:40:58.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/openai_endpoint_provider.py
+-rw-rw-rw-   0        0        0     9672 2024-05-03 23:16:22.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/provider_base.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.789739 llama_cpp_agent-0.1.1/src/llama_cpp_agent/rag/
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:48:26.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/rag/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-rw-rw-   0        0        0     3895 2024-05-01 04:36:07.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/rag/text_utils.py
+-rw-rw-rw-   0        0        0    11104 2024-04-16 22:20:07.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent/structured_output_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:32:47.790749 llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/
+-rw-rw-rw-   0        0        0    40131 2024-05-04 20:32:47.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1645 2024-05-04 20:32:47.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:32:47.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2024-05-04 20:32:47.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-04 20:32:47.000000 llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.1.0/LICENSE` & `llama_cpp_agent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/PKG-INFO` & `llama_cpp_agent-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.1.0
+Version: 0.1.1
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,27 +21,28 @@
 Requires-Dist: numpy; extra == "agent-memory"
 Requires-Dist: scipy; extra == "agent-memory"
 Provides-Extra: rag
 Requires-Dist: ragatouille; extra == "rag"
 
 # llama-cpp-agent
 
-<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/5daba580ceb1baf9266a0ed47b5b1daba6a9a122/logo/logo-without-bg.png" alt="llama-cpp-agent logo" width="400"/>
+<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
 ## Introduction
 The llama-cpp-agent framework is a tool designed for easy interaction with Large Language Models (LLMs). Allowing users to chat with LLM models, execute structured function calls, get structured output (objects) and do retrieval augmented generation.
 
 It provides a simple yet robust interface and supports llama-cpp-python and OpenAI endpoints with GBNF grammar support (like the llama-cpp-python server) and the llama.cpp backend server.
 It works by generating a formal GGML-BNF grammar of the user defined structures and functions, which is then used by llama.cpp to generate text valid to that grammar. In contrast to most GBNF grammar generators it also supports nested objects, dictionaries, enums and lists of them.
 
 ## Key Features
 - **Simple Chat Interface**: Engage in seamless conversations with LLMs.
 - **Structured Output**: Get structured output (objects) from LLMs.
 - **Single and Parallel Function Calling**: Let the LLM execute functions.
 - **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Supports processing of text in agent chains with tools. Supports Conversational, Sequential and Mapping Chains.
 - **Flexibility**: Suited for various applications from casual chatting to specific function executions.
 
 ## Installation
 The llama-cpp-agent framework can be installed using pip:
 ```shell
 pip install llama-cpp-agent
 ```
@@ -434,14 +435,205 @@
 
 ```
 Example output
 ```text
  BARS (Bridgman-Anvil High Pressure Reactor System) apparatus is a type of diamond-producing press used in the HPHT (High Pressure High Temperature) method for synthetic diamond growth. It consists of a ceramic cylindrical "synthesis capsule" placed in a cube of pressure-transmitting material, which is pressed by inner anvils and outer anvils. The whole assembly is locked in a disc-type barrel filled with oil, which pressurizes upon heating, and the oil pressure is transferred to the central cell. The BARS apparatus is claimed to be the most compact, efficient, and economical press design for diamond synthesis.
 ```
 
+### Sequential Chain Example
+This example demonstrates how to create a complete product launch campaign with help of a sequential chain.
+```python
+# Example: Product Launch Campaign (Product Description, USP, Target Audience, Marketing Channels, Ad Copy, Landing Page, Email Campaign, Social Media Posts, Press Release, and Performance Metrics)
+from llama_cpp_agent.chain import AgentChainElement, AgentChain
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.messages_formatter import MessagesFormatterType
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
+
+model = LlamaCppEndpointSettings(completions_endpoint_url="http://127.0.0.1:8080/completion")
+
+agent = LlamaCppAgent(
+    model,
+    debug_output=True,
+    system_prompt="",
+    predefined_messages_formatter_type=MessagesFormatterType.MIXTRAL
+)
+
+product_description = AgentChainElement(
+    output_identifier="out_0",
+    system_prompt="You are a product description writer",
+    prompt="Write a detailed product description for {product_name}, including its features and benefits."
+)
+
+product_usp = AgentChainElement(
+    output_identifier="out_1",
+    system_prompt="You are a unique selling proposition (USP) creator",
+    prompt="Create a compelling USP for {product_name} based on the following product description:\n--\n{out_0}"
+)
+
+target_audience = AgentChainElement(
+    output_identifier="out_2",
+    system_prompt="You are a target audience identifier",
+    prompt="Identify the target audience for {product_name} based on the following product description and USP:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}"
+)
+
+marketing_channels = AgentChainElement(
+    output_identifier="out_3",
+    system_prompt="You are a marketing channel strategist",
+    prompt="Suggest the most effective marketing channels to promote {product_name} based on the following target audience:\n--\n{out_2}"
+)
+
+ad_copy = AgentChainElement(
+    output_identifier="out_4",
+    system_prompt="You are an advertising copywriter",
+    prompt="Write engaging ad copy for {product_name} based on the following product description, USP, and target audience:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}"
+)
+
+landing_page = AgentChainElement(
+    output_identifier="out_5",
+    system_prompt="You are a landing page designer",
+    prompt="Create a high-converting landing page structure for {product_name} based on the following product description, USP, target audience, and ad copy:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nAd Copy:\n{out_4}"
+)
+
+email_campaign = AgentChainElement(
+    output_identifier="out_6",
+    system_prompt="You are an email marketing specialist",
+    prompt="Develop an email campaign for {product_name} based on the following product description, USP, target audience, and landing page structure:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nLanding Page Structure:\n{out_5}"
+)
+
+social_media_posts = AgentChainElement(
+    output_identifier="out_7",
+    system_prompt="You are a social media content creator",
+    prompt="Create a series of engaging social media posts for {product_name} based on the following product description, USP, target audience, and ad copy:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nAd Copy:\n{out_4}"
+)
+
+press_release = AgentChainElement(
+    output_identifier="out_8",
+    system_prompt="You are a press release writer",
+    prompt="Write a compelling press release announcing the launch of {product_name} based on the following product description, USP, and target audience:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}"
+)
+
+performance_metrics = AgentChainElement(
+    output_identifier="out_9",
+    system_prompt="You are a marketing performance analyst",
+    prompt="Identify the key performance metrics to track the success of the {product_name} launch campaign based on the following marketing channels, ad copy, landing page, email campaign, social media posts, and press release:\n--\nMarketing Channels:\n{out_3}\nAd Copy:\n{out_4}\nLanding Page Structure:\n{out_5}\nEmail Campaign:\n{out_6}\nSocial Media Posts:\n{out_7}\nPress Release:\n{out_8}"
+)
+
+chain = [product_description, product_usp, target_audience, marketing_channels, ad_copy, landing_page, email_campaign, social_media_posts, press_release, performance_metrics]
+agent_chain = AgentChain(agent, chain)
+agent_chain.run_chain(additional_fields={"product_name": "Smart Fitness Tracker"})
+
+
+```
+
+### Mapping Chain Example
+This example demonstrates how to create a mapping chain to summarize 3 articles into one summary.
+```python
+from llama_cpp_agent.chain import AgentChainElement, MapChain
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.messages_formatter import MessagesFormatterType
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
+
+model = LlamaCppEndpointSettings(completions_endpoint_url="http://127.0.0.1:8080/completion")
+
+agent = LlamaCppAgent(
+    model,
+    debug_output=True,
+    system_prompt="",
+    predefined_messages_formatter_type=MessagesFormatterType.MIXTRAL
+)
+
+summary_chain = AgentChainElement("out_0", system_prompt="You are an advanced AI agent for summarizing articles", prompt="Summarize this article into bullet points:\n{item}")
+
+combine_chain = AgentChainElement("out_1", system_prompt="You are an advanced AI agent that summarizes text", prompt="Please combine the bullet points of different summaries below, into one summary as bullet points:\n{map_output}")
+
+map_chain = MapChain(agent, [summary_chain], [combine_chain])
+
+
+article_list = [
+    """### 1. Quantum Computing: The Next Frontier in Computational Power
+
+**Introduction**
+Quantum computing represents a revolutionary approach to information processing, leveraging the principles of quantum mechanics to solve problems that are intractable for classical computers. This article explores the fundamental concepts of quantum computing, its potential applications, and the challenges it faces.
+
+**Quantum Mechanics and Computing**
+Quantum computers use quantum bits, or qubits, which can exist in multiple states simultaneously, thanks to superposition. This capability, combined with entanglement—where the state of one qubit can depend on the state of another, no matter the distance between them—allows quantum computers to process a vast number of possibilities concurrently.
+
+**Quantum Algorithms**
+Several algorithms have been developed for quantum computers that show significant speed-ups over their classical counterparts. Shor’s Algorithm, for instance, can factorize large integers exponentially faster than the best-known classical algorithms, which has profound implications for cryptography. Grover's Algorithm offers a quadratic speedup for unstructured search problems.
+
+**Applications**
+Quantum computing has potential applications across various fields:
+- **Cryptography**: Secure communication through quantum key distribution.
+- **Drug Discovery**: Modeling molecular interactions at quantum levels to predict drug efficacy and side effects.
+- **Optimization Problems**: Enhancing solutions in logistics, finance, and materials science.
+
+**Challenges**
+Despite its potential, quantum computing faces several hurdles:
+- **Qubit Coherence**: Maintaining the state of qubits for sufficient time is challenging due to decoherence.
+- **Error Rates**: Quantum gates are prone to errors significantly higher than conventional binary computing gates.
+- **Scalability**: Building machines with enough qubits to be useful for complex problems is currently beyond our reach.
+
+**Conclusion**
+Quantum computing is still in its infancy, but it holds the promise of massive computational power. The coming decades are likely to see significant advancements in this field as researchers overcome its current limitations.""",
+    """### 2. Machine Learning: Transforming Data into Insights
+
+**Introduction**
+Machine Learning (ML) is a branch of artificial intelligence that focuses on building applications that can learn from data and improve their accuracy over time without being explicitly programmed. This article delves into the types of ML, key algorithms, applications, and future prospects.
+
+**Types of Machine Learning**
+- **Supervised Learning**: Models predict outputs based on input data, and learning is guided by comparing actual and predicted outputs.
+- **Unsupervised Learning**: Algorithms identify patterns in data without reference to known or labeled outcomes.
+- **Reinforcement Learning**: Models learn to make sequences of decisions by receiving rewards or penalties.
+
+**Key Algorithms**
+- **Linear Regression** and **Logistic Regression** for predictive modeling.
+- **Decision Trees** and **Random Forests** for classification and regression tasks.
+- **Neural Networks**: Used in deep learning for complex pattern recognition, such as in image and speech recognition.
+
+**Applications**
+- **Healthcare**: From diagnosing diseases to personalized medicine.
+- **Finance**: For credit scoring, algorithmic trading, and risk assessment.
+- **Retail**: Enhancing customer experience through personalized recommendations.
+
+**Challenges and Future Prospects**
+The field of ML is not without challenges, including data privacy concerns, the need for large labeled datasets, and the risk of creating biased models. However, ongoing research in areas like unsupervised learning, transfer learning, and the development of more robust models promises to mitigate these issues.
+
+**Conclusion**
+Machine learning continues to be a dynamic field of research and application, with the potential to impact numerous sectors profoundly.""",
+    """### 3. Blockchain Technology: Decentralizing Trust
+
+**Introduction**
+Blockchain technology is best known as the backbone of cryptocurrencies like Bitcoin, but its applications extend far beyond. This article outlines the technology’s fundamentals, applications beyond finance, and the challenges it faces.
+
+**Blockchain Basics**
+A blockchain is a decentralized ledger of all transactions across a network. Each transaction is added to a "block" and linked to the previous block, forming a "chain." This structure, combined with cryptographic techniques, makes it secure and immutable.
+
+**Key Features**
+- **Decentralization**: No single point of control or failure.
+- **Transparency**: Changes to the public blockchain are viewable by all parties creating transparency.
+- **Immutability**: Once a transaction is recorded, it cannot be altered, increasing trust.
+
+**Applications**
+- **Supply Chain Management**: Enhancing transparency and traceability.
+- **Healthcare**: Secure sharing of medical records.
+- **Smart Contracts**: Automatically executing contracts when conditions are met.
+
+**Challenges**
+- **Scalability**: Current blockchain solutions, like Bitcoin, have limitations on transaction speed and volume.
+- **Regulatory Issues**: Balancing the need for regulation with the ethos of decentralization.
+- **Energy Consumption**: The energy requirement for "mining" transactions, particularly in networks like Bitcoin, is substantial.
+
+**Conclusion**
+Blockchain technology holds great promise for creating a more transparent and efficient world, but significant challenges must be addressed to realize its full potential."""
+]
+
+
+map_chain.run_map_chain(items_to_map=article_list)
+```
+
 ### Knowledge Graph Creation Example
 This example, based on an example of the Instructor library for OpenAI,
 demonstrates how to create a knowledge graph using the llama-cpp-agent framework.
 ```python
 import json
 from typing import List
```

### Comparing `llama_cpp_agent-0.1.0/ReadMe.md` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,48 @@
+Metadata-Version: 2.1
+Name: llama-cpp-agent
+Version: 0.1.1
+Summary: A framework for building LLM based AI agents with llama.cpp.
+Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
+Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
+Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: llama-cpp-python>=0.2.60
+Requires-Dist: pydantic>=2.5.3
+Requires-Dist: requests>=2.31.0
+Requires-Dist: docstring_parser
+Provides-Extra: agent-memory
+Requires-Dist: chromadb; extra == "agent-memory"
+Requires-Dist: SQLAlchemy; extra == "agent-memory"
+Requires-Dist: numpy; extra == "agent-memory"
+Requires-Dist: scipy; extra == "agent-memory"
+Provides-Extra: rag
+Requires-Dist: ragatouille; extra == "rag"
+
 # llama-cpp-agent
 
-<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/5daba580ceb1baf9266a0ed47b5b1daba6a9a122/logo/logo-without-bg.png" alt="llama-cpp-agent logo" width="400"/>
+<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
 ## Introduction
 The llama-cpp-agent framework is a tool designed for easy interaction with Large Language Models (LLMs). Allowing users to chat with LLM models, execute structured function calls, get structured output (objects) and do retrieval augmented generation.
 
 It provides a simple yet robust interface and supports llama-cpp-python and OpenAI endpoints with GBNF grammar support (like the llama-cpp-python server) and the llama.cpp backend server.
 It works by generating a formal GGML-BNF grammar of the user defined structures and functions, which is then used by llama.cpp to generate text valid to that grammar. In contrast to most GBNF grammar generators it also supports nested objects, dictionaries, enums and lists of them.
 
 ## Key Features
 - **Simple Chat Interface**: Engage in seamless conversations with LLMs.
 - **Structured Output**: Get structured output (objects) from LLMs.
 - **Single and Parallel Function Calling**: Let the LLM execute functions.
 - **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Supports processing of text in agent chains with tools. Supports Conversational, Sequential and Mapping Chains.
 - **Flexibility**: Suited for various applications from casual chatting to specific function executions.
 
 ## Installation
 The llama-cpp-agent framework can be installed using pip:
 ```shell
 pip install llama-cpp-agent
 ```
@@ -409,14 +435,205 @@
 
 ```
 Example output
 ```text
  BARS (Bridgman-Anvil High Pressure Reactor System) apparatus is a type of diamond-producing press used in the HPHT (High Pressure High Temperature) method for synthetic diamond growth. It consists of a ceramic cylindrical "synthesis capsule" placed in a cube of pressure-transmitting material, which is pressed by inner anvils and outer anvils. The whole assembly is locked in a disc-type barrel filled with oil, which pressurizes upon heating, and the oil pressure is transferred to the central cell. The BARS apparatus is claimed to be the most compact, efficient, and economical press design for diamond synthesis.
 ```
 
+### Sequential Chain Example
+This example demonstrates how to create a complete product launch campaign with help of a sequential chain.
+```python
+# Example: Product Launch Campaign (Product Description, USP, Target Audience, Marketing Channels, Ad Copy, Landing Page, Email Campaign, Social Media Posts, Press Release, and Performance Metrics)
+from llama_cpp_agent.chain import AgentChainElement, AgentChain
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.messages_formatter import MessagesFormatterType
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
+
+model = LlamaCppEndpointSettings(completions_endpoint_url="http://127.0.0.1:8080/completion")
+
+agent = LlamaCppAgent(
+    model,
+    debug_output=True,
+    system_prompt="",
+    predefined_messages_formatter_type=MessagesFormatterType.MIXTRAL
+)
+
+product_description = AgentChainElement(
+    output_identifier="out_0",
+    system_prompt="You are a product description writer",
+    prompt="Write a detailed product description for {product_name}, including its features and benefits."
+)
+
+product_usp = AgentChainElement(
+    output_identifier="out_1",
+    system_prompt="You are a unique selling proposition (USP) creator",
+    prompt="Create a compelling USP for {product_name} based on the following product description:\n--\n{out_0}"
+)
+
+target_audience = AgentChainElement(
+    output_identifier="out_2",
+    system_prompt="You are a target audience identifier",
+    prompt="Identify the target audience for {product_name} based on the following product description and USP:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}"
+)
+
+marketing_channels = AgentChainElement(
+    output_identifier="out_3",
+    system_prompt="You are a marketing channel strategist",
+    prompt="Suggest the most effective marketing channels to promote {product_name} based on the following target audience:\n--\n{out_2}"
+)
+
+ad_copy = AgentChainElement(
+    output_identifier="out_4",
+    system_prompt="You are an advertising copywriter",
+    prompt="Write engaging ad copy for {product_name} based on the following product description, USP, and target audience:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}"
+)
+
+landing_page = AgentChainElement(
+    output_identifier="out_5",
+    system_prompt="You are a landing page designer",
+    prompt="Create a high-converting landing page structure for {product_name} based on the following product description, USP, target audience, and ad copy:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nAd Copy:\n{out_4}"
+)
+
+email_campaign = AgentChainElement(
+    output_identifier="out_6",
+    system_prompt="You are an email marketing specialist",
+    prompt="Develop an email campaign for {product_name} based on the following product description, USP, target audience, and landing page structure:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nLanding Page Structure:\n{out_5}"
+)
+
+social_media_posts = AgentChainElement(
+    output_identifier="out_7",
+    system_prompt="You are a social media content creator",
+    prompt="Create a series of engaging social media posts for {product_name} based on the following product description, USP, target audience, and ad copy:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nAd Copy:\n{out_4}"
+)
+
+press_release = AgentChainElement(
+    output_identifier="out_8",
+    system_prompt="You are a press release writer",
+    prompt="Write a compelling press release announcing the launch of {product_name} based on the following product description, USP, and target audience:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}"
+)
+
+performance_metrics = AgentChainElement(
+    output_identifier="out_9",
+    system_prompt="You are a marketing performance analyst",
+    prompt="Identify the key performance metrics to track the success of the {product_name} launch campaign based on the following marketing channels, ad copy, landing page, email campaign, social media posts, and press release:\n--\nMarketing Channels:\n{out_3}\nAd Copy:\n{out_4}\nLanding Page Structure:\n{out_5}\nEmail Campaign:\n{out_6}\nSocial Media Posts:\n{out_7}\nPress Release:\n{out_8}"
+)
+
+chain = [product_description, product_usp, target_audience, marketing_channels, ad_copy, landing_page, email_campaign, social_media_posts, press_release, performance_metrics]
+agent_chain = AgentChain(agent, chain)
+agent_chain.run_chain(additional_fields={"product_name": "Smart Fitness Tracker"})
+
+
+```
+
+### Mapping Chain Example
+This example demonstrates how to create a mapping chain to summarize 3 articles into one summary.
+```python
+from llama_cpp_agent.chain import AgentChainElement, MapChain
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.messages_formatter import MessagesFormatterType
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
+
+model = LlamaCppEndpointSettings(completions_endpoint_url="http://127.0.0.1:8080/completion")
+
+agent = LlamaCppAgent(
+    model,
+    debug_output=True,
+    system_prompt="",
+    predefined_messages_formatter_type=MessagesFormatterType.MIXTRAL
+)
+
+summary_chain = AgentChainElement("out_0", system_prompt="You are an advanced AI agent for summarizing articles", prompt="Summarize this article into bullet points:\n{item}")
+
+combine_chain = AgentChainElement("out_1", system_prompt="You are an advanced AI agent that summarizes text", prompt="Please combine the bullet points of different summaries below, into one summary as bullet points:\n{map_output}")
+
+map_chain = MapChain(agent, [summary_chain], [combine_chain])
+
+
+article_list = [
+    """### 1. Quantum Computing: The Next Frontier in Computational Power
+
+**Introduction**
+Quantum computing represents a revolutionary approach to information processing, leveraging the principles of quantum mechanics to solve problems that are intractable for classical computers. This article explores the fundamental concepts of quantum computing, its potential applications, and the challenges it faces.
+
+**Quantum Mechanics and Computing**
+Quantum computers use quantum bits, or qubits, which can exist in multiple states simultaneously, thanks to superposition. This capability, combined with entanglement—where the state of one qubit can depend on the state of another, no matter the distance between them—allows quantum computers to process a vast number of possibilities concurrently.
+
+**Quantum Algorithms**
+Several algorithms have been developed for quantum computers that show significant speed-ups over their classical counterparts. Shor’s Algorithm, for instance, can factorize large integers exponentially faster than the best-known classical algorithms, which has profound implications for cryptography. Grover's Algorithm offers a quadratic speedup for unstructured search problems.
+
+**Applications**
+Quantum computing has potential applications across various fields:
+- **Cryptography**: Secure communication through quantum key distribution.
+- **Drug Discovery**: Modeling molecular interactions at quantum levels to predict drug efficacy and side effects.
+- **Optimization Problems**: Enhancing solutions in logistics, finance, and materials science.
+
+**Challenges**
+Despite its potential, quantum computing faces several hurdles:
+- **Qubit Coherence**: Maintaining the state of qubits for sufficient time is challenging due to decoherence.
+- **Error Rates**: Quantum gates are prone to errors significantly higher than conventional binary computing gates.
+- **Scalability**: Building machines with enough qubits to be useful for complex problems is currently beyond our reach.
+
+**Conclusion**
+Quantum computing is still in its infancy, but it holds the promise of massive computational power. The coming decades are likely to see significant advancements in this field as researchers overcome its current limitations.""",
+    """### 2. Machine Learning: Transforming Data into Insights
+
+**Introduction**
+Machine Learning (ML) is a branch of artificial intelligence that focuses on building applications that can learn from data and improve their accuracy over time without being explicitly programmed. This article delves into the types of ML, key algorithms, applications, and future prospects.
+
+**Types of Machine Learning**
+- **Supervised Learning**: Models predict outputs based on input data, and learning is guided by comparing actual and predicted outputs.
+- **Unsupervised Learning**: Algorithms identify patterns in data without reference to known or labeled outcomes.
+- **Reinforcement Learning**: Models learn to make sequences of decisions by receiving rewards or penalties.
+
+**Key Algorithms**
+- **Linear Regression** and **Logistic Regression** for predictive modeling.
+- **Decision Trees** and **Random Forests** for classification and regression tasks.
+- **Neural Networks**: Used in deep learning for complex pattern recognition, such as in image and speech recognition.
+
+**Applications**
+- **Healthcare**: From diagnosing diseases to personalized medicine.
+- **Finance**: For credit scoring, algorithmic trading, and risk assessment.
+- **Retail**: Enhancing customer experience through personalized recommendations.
+
+**Challenges and Future Prospects**
+The field of ML is not without challenges, including data privacy concerns, the need for large labeled datasets, and the risk of creating biased models. However, ongoing research in areas like unsupervised learning, transfer learning, and the development of more robust models promises to mitigate these issues.
+
+**Conclusion**
+Machine learning continues to be a dynamic field of research and application, with the potential to impact numerous sectors profoundly.""",
+    """### 3. Blockchain Technology: Decentralizing Trust
+
+**Introduction**
+Blockchain technology is best known as the backbone of cryptocurrencies like Bitcoin, but its applications extend far beyond. This article outlines the technology’s fundamentals, applications beyond finance, and the challenges it faces.
+
+**Blockchain Basics**
+A blockchain is a decentralized ledger of all transactions across a network. Each transaction is added to a "block" and linked to the previous block, forming a "chain." This structure, combined with cryptographic techniques, makes it secure and immutable.
+
+**Key Features**
+- **Decentralization**: No single point of control or failure.
+- **Transparency**: Changes to the public blockchain are viewable by all parties creating transparency.
+- **Immutability**: Once a transaction is recorded, it cannot be altered, increasing trust.
+
+**Applications**
+- **Supply Chain Management**: Enhancing transparency and traceability.
+- **Healthcare**: Secure sharing of medical records.
+- **Smart Contracts**: Automatically executing contracts when conditions are met.
+
+**Challenges**
+- **Scalability**: Current blockchain solutions, like Bitcoin, have limitations on transaction speed and volume.
+- **Regulatory Issues**: Balancing the need for regulation with the ethos of decentralization.
+- **Energy Consumption**: The energy requirement for "mining" transactions, particularly in networks like Bitcoin, is substantial.
+
+**Conclusion**
+Blockchain technology holds great promise for creating a more transparent and efficient world, but significant challenges must be addressed to realize its full potential."""
+]
+
+
+map_chain.run_map_chain(items_to_map=article_list)
+```
+
 ### Knowledge Graph Creation Example
 This example, based on an example of the Instructor library for OpenAI,
 demonstrates how to create a knowledge graph using the llama-cpp-agent framework.
 ```python
 import json
 from typing import List
```

### Comparing `llama_cpp_agent-0.1.0/pyproject.toml` & `llama_cpp_agent-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.1.0"
+version = "0.1.1"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/function_calling.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/function_calling.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,18 @@
             function=Function(
                 name=root["function"]["name"],
                 description=root["function"]["description"],
                 parameters=root["function"]["parameters"],
             )
         )
 
+    def to_openai_tool(self):
+        root = pydantic_model_to_openai_function_definition(self.model)
+        return root
+
     def __call__(self, *args, **kwargs):
         """
         Calls the Pydantic model with the provided keyword arguments.
 
         Returns:
             BaseModel: An instance of the Pydantic model.
         """
@@ -242,14 +246,15 @@
         add_request_heartbeat=True,
         tool_root="function",
         tool_rule_content="arguments",
         model_prefix="function",
         fields_prefix="parameters",
         inner_thoughts_field_name="thoughts_and_reasoning",
         request_heartbeat_field_name="request_heartbeat",
+        add_tool_root_content_to_all_results=True
     ):
         """
         Initialize the LlamaCppFunctionToolRegistry.
 
         Args:
             allow_parallel_function_calling (bool): Flag indicating whether to allow parallel function calling.
             add_inner_thoughts (bool): Flag indicating whether to add inner thoughts to the GBNF grammar.
@@ -274,14 +279,15 @@
         self.gbnf_grammar = None
         self.allow_parallel_function_calling = allow_parallel_function_calling
         self.add_inner_thoughts = add_inner_thoughts
         self.allow_inner_thoughts_only = allow_inner_thoughts_only
         self.add_request_heartbeat = add_request_heartbeat
         self.inner_thoughts_field_name = inner_thoughts_field_name
         self.request_heartbeat_field_name = request_heartbeat_field_name
+        self.add_tool_root_content_to_all_results = add_tool_root_content_to_all_results
 
     def register_function_tool(self, function_tool: LlamaCppFunctionTool):
         """
         Register a function tool in the registry.
 
         Args:
             function_tool (LlamaCppFunctionTool): The function tool to register.
@@ -445,15 +451,15 @@
                 function_tool = self.function_tools[function_call[self.tool_root]]
         try:
             if self.tool_root in function_call:
                 cls = function_tool.model
                 call_parameters = function_call[self.tool_rule_content]
                 call = cls(**call_parameters)
                 output = call.run(**function_tool.additional_parameters)
-                if function_tool.add_params_to_result:
+                if function_tool.add_params_to_result or self.add_tool_root_content_to_all_results:
                     if self.add_request_heartbeat:
                         return [
                             {
                                 "function": function_tool.model.__name__,
                                 "params": call_parameters,
                                 "return_value": output,
                                 "request_heartbeat": function_call["request_heartbeat"]
@@ -509,15 +515,15 @@
                 if self.tool_root in function_call:
                     function_tool = self.function_tools[function_call[self.tool_root]]
                     try:
                         cls = function_tool.model
                         call_parameters = function_call[self.tool_rule_content]
                         call = cls(**call_parameters)
                         output = call.run(**function_tool.additional_parameters)
-                        if function_tool.add_params_to_result:
+                        if function_tool.add_params_to_result or self.add_tool_root_content_to_all_results:
                             if self.add_request_heartbeat:
                                 result.append(
                                     {
                                         "function": function_tool.model.__name__,
                                         "params": call_parameters,
                                         "return_value": output,
                                         "request_heartbeat": function_call[
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/function_calling_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         self.without_grammar_mode_function = []
         self.prompt_suffix = ""
         if system_prompt is not None:
             self.system_prompt = system_prompt
         else:
             # You can also request to return control back to you after a function call is executed by setting the 'return_control' flag in a function call object.
             self.system_prompt = (
-                """You are Funky, an AI assistant that calls functions to perform tasks. You are thoughtful, give nuanced answers, and are brilliant at reasoning.
+                """You are Funky, an AI assistant that calls functions to perform tasks.
 
 To call functions, you respond with a JSON object containing three fields:
 "thoughts_and_reasoning": Your thoughts and reasoning behind the function call.
 "function": The name of the function you want to call.
 "parameters": The arguments required for the function.
 
 After performing a function call, you will receive a response containing the return values of the function calls.
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1594,16 +1594,16 @@
     dynamic_model = create_model(f"{func.__name__}", **dynamic_fields)  # type: ignore[call-overload]
     if add_inner_thoughts:
         dynamic_model.model_fields[
             inner_thoughts_field_name
         ].description = "Deep inner monologue private to you only."
     for name, param_doc in param_docs:
         dynamic_model.model_fields[name].description = param_doc.description
-
-    dynamic_model.__doc__ = docstring.short_description
+        
+    dynamic_model.__doc__ = (docstring.short_description if docstring.short_description is not None else "") + "\n" + (docstring.long_description if docstring.long_description is not None else "")
 
     def run_method_wrapper(self):
         func_args = {name: getattr(self, name) for name, _ in dynamic_fields.items()}
         return func(**func_args)
 
     # Adding the wrapped function as a 'run' method
     setattr(dynamic_model, "run", run_method_wrapper)
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/llm_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def __init__(
         self,
         model: Union[
             Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings
         ],
         name: str = "llamacpp_agent",
-        system_prompt: str = "You are helpful assistant.",
+        system_prompt: str = "You are a helpful assistant.",
         predefined_messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
         custom_messages_formatter: MessagesFormatter = None,
         debug_output: bool = False,
         function_tool_registry: LlamaCppFunctionToolRegistry = None,
     ):
         """
         Initializes a new LlamaCppAgent object.
@@ -391,14 +391,15 @@
         return "Error: No model loaded!"
 
     def get_chat_response(
         self,
         message: str = None,
         role: Literal["system", "user", "assistant", "function"] = "user",
         response_role: Literal["user", "assistant"] | None = None,
+
         system_prompt: str = None,
         prompt_suffix: str = None,
         add_message_to_chat_history: bool = True,
         add_response_to_chat_history: bool = True,
         grammar: str = None,
         function_tool_registry: LlamaCppFunctionToolRegistry = None,
         do_not_use_grammar: bool = False,
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/llm_settings.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/llm_settings.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/messages_formatter.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     stream: bool = True
     use_default_badwordsids: bool = False
     dynatemp_range: float = 0
     mirostat: Optional[int] = None
     mirostat_tau: float = 0
     mirostat_eta: float = 0
     genkey: Optional[str] = None
-    grammar: Optional[str] = None
     grammar_retain_state: bool = False
     memory: Optional[str] = None
     trim_stop: bool = False
     logit_bias: Optional[dict] = field(default_factory=dict)
 
     def save(self, file_path: str):
         """
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/providers/openai_endpoint_provider.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/providers/openai_endpoint_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     seed: Optional[int] = None
     top_k: int = 40
     repeat_penalty: float = 1.1
     logit_bias_type: Optional[Literal["input_ids", "tokens"]] = None
     mirostat_mode: int = 0
     mirostat_tau: float = 5.0
     mirostat_eta: float = 0.1
-    grammar: Optional[str] = None
 
     def save(self, file_path: str):
         """
         Save the settings to a file.
 
         Args:
             file_path (str): The path to the file.
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/rag/text_utils.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/rag/text_utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.1.1/ReadMe.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,23 @@
-Metadata-Version: 2.1
-Name: llama-cpp-agent
-Version: 0.1.0
-Summary: A framework for building LLM based AI agents with llama.cpp.
-Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
-Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
-Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: llama-cpp-python>=0.2.60
-Requires-Dist: pydantic>=2.5.3
-Requires-Dist: requests>=2.31.0
-Requires-Dist: docstring_parser
-Provides-Extra: agent-memory
-Requires-Dist: chromadb; extra == "agent-memory"
-Requires-Dist: SQLAlchemy; extra == "agent-memory"
-Requires-Dist: numpy; extra == "agent-memory"
-Requires-Dist: scipy; extra == "agent-memory"
-Provides-Extra: rag
-Requires-Dist: ragatouille; extra == "rag"
-
 # llama-cpp-agent
 
-<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/5daba580ceb1baf9266a0ed47b5b1daba6a9a122/logo/logo-without-bg.png" alt="llama-cpp-agent logo" width="400"/>
+<img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
 ## Introduction
 The llama-cpp-agent framework is a tool designed for easy interaction with Large Language Models (LLMs). Allowing users to chat with LLM models, execute structured function calls, get structured output (objects) and do retrieval augmented generation.
 
 It provides a simple yet robust interface and supports llama-cpp-python and OpenAI endpoints with GBNF grammar support (like the llama-cpp-python server) and the llama.cpp backend server.
 It works by generating a formal GGML-BNF grammar of the user defined structures and functions, which is then used by llama.cpp to generate text valid to that grammar. In contrast to most GBNF grammar generators it also supports nested objects, dictionaries, enums and lists of them.
 
 ## Key Features
 - **Simple Chat Interface**: Engage in seamless conversations with LLMs.
 - **Structured Output**: Get structured output (objects) from LLMs.
 - **Single and Parallel Function Calling**: Let the LLM execute functions.
 - **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Supports processing of text in agent chains with tools. Supports Conversational, Sequential and Mapping Chains.
 - **Flexibility**: Suited for various applications from casual chatting to specific function executions.
 
 ## Installation
 The llama-cpp-agent framework can be installed using pip:
 ```shell
 pip install llama-cpp-agent
 ```
@@ -434,14 +410,205 @@
 
 ```
 Example output
 ```text
  BARS (Bridgman-Anvil High Pressure Reactor System) apparatus is a type of diamond-producing press used in the HPHT (High Pressure High Temperature) method for synthetic diamond growth. It consists of a ceramic cylindrical "synthesis capsule" placed in a cube of pressure-transmitting material, which is pressed by inner anvils and outer anvils. The whole assembly is locked in a disc-type barrel filled with oil, which pressurizes upon heating, and the oil pressure is transferred to the central cell. The BARS apparatus is claimed to be the most compact, efficient, and economical press design for diamond synthesis.
 ```
 
+### Sequential Chain Example
+This example demonstrates how to create a complete product launch campaign with help of a sequential chain.
+```python
+# Example: Product Launch Campaign (Product Description, USP, Target Audience, Marketing Channels, Ad Copy, Landing Page, Email Campaign, Social Media Posts, Press Release, and Performance Metrics)
+from llama_cpp_agent.chain import AgentChainElement, AgentChain
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.messages_formatter import MessagesFormatterType
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
+
+model = LlamaCppEndpointSettings(completions_endpoint_url="http://127.0.0.1:8080/completion")
+
+agent = LlamaCppAgent(
+    model,
+    debug_output=True,
+    system_prompt="",
+    predefined_messages_formatter_type=MessagesFormatterType.MIXTRAL
+)
+
+product_description = AgentChainElement(
+    output_identifier="out_0",
+    system_prompt="You are a product description writer",
+    prompt="Write a detailed product description for {product_name}, including its features and benefits."
+)
+
+product_usp = AgentChainElement(
+    output_identifier="out_1",
+    system_prompt="You are a unique selling proposition (USP) creator",
+    prompt="Create a compelling USP for {product_name} based on the following product description:\n--\n{out_0}"
+)
+
+target_audience = AgentChainElement(
+    output_identifier="out_2",
+    system_prompt="You are a target audience identifier",
+    prompt="Identify the target audience for {product_name} based on the following product description and USP:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}"
+)
+
+marketing_channels = AgentChainElement(
+    output_identifier="out_3",
+    system_prompt="You are a marketing channel strategist",
+    prompt="Suggest the most effective marketing channels to promote {product_name} based on the following target audience:\n--\n{out_2}"
+)
+
+ad_copy = AgentChainElement(
+    output_identifier="out_4",
+    system_prompt="You are an advertising copywriter",
+    prompt="Write engaging ad copy for {product_name} based on the following product description, USP, and target audience:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}"
+)
+
+landing_page = AgentChainElement(
+    output_identifier="out_5",
+    system_prompt="You are a landing page designer",
+    prompt="Create a high-converting landing page structure for {product_name} based on the following product description, USP, target audience, and ad copy:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nAd Copy:\n{out_4}"
+)
+
+email_campaign = AgentChainElement(
+    output_identifier="out_6",
+    system_prompt="You are an email marketing specialist",
+    prompt="Develop an email campaign for {product_name} based on the following product description, USP, target audience, and landing page structure:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nLanding Page Structure:\n{out_5}"
+)
+
+social_media_posts = AgentChainElement(
+    output_identifier="out_7",
+    system_prompt="You are a social media content creator",
+    prompt="Create a series of engaging social media posts for {product_name} based on the following product description, USP, target audience, and ad copy:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}\nAd Copy:\n{out_4}"
+)
+
+press_release = AgentChainElement(
+    output_identifier="out_8",
+    system_prompt="You are a press release writer",
+    prompt="Write a compelling press release announcing the launch of {product_name} based on the following product description, USP, and target audience:\n--\nProduct Description:\n{out_0}\nUSP:\n{out_1}\nTarget Audience:\n{out_2}"
+)
+
+performance_metrics = AgentChainElement(
+    output_identifier="out_9",
+    system_prompt="You are a marketing performance analyst",
+    prompt="Identify the key performance metrics to track the success of the {product_name} launch campaign based on the following marketing channels, ad copy, landing page, email campaign, social media posts, and press release:\n--\nMarketing Channels:\n{out_3}\nAd Copy:\n{out_4}\nLanding Page Structure:\n{out_5}\nEmail Campaign:\n{out_6}\nSocial Media Posts:\n{out_7}\nPress Release:\n{out_8}"
+)
+
+chain = [product_description, product_usp, target_audience, marketing_channels, ad_copy, landing_page, email_campaign, social_media_posts, press_release, performance_metrics]
+agent_chain = AgentChain(agent, chain)
+agent_chain.run_chain(additional_fields={"product_name": "Smart Fitness Tracker"})
+
+
+```
+
+### Mapping Chain Example
+This example demonstrates how to create a mapping chain to summarize 3 articles into one summary.
+```python
+from llama_cpp_agent.chain import AgentChainElement, MapChain
+from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.messages_formatter import MessagesFormatterType
+from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
+
+model = LlamaCppEndpointSettings(completions_endpoint_url="http://127.0.0.1:8080/completion")
+
+agent = LlamaCppAgent(
+    model,
+    debug_output=True,
+    system_prompt="",
+    predefined_messages_formatter_type=MessagesFormatterType.MIXTRAL
+)
+
+summary_chain = AgentChainElement("out_0", system_prompt="You are an advanced AI agent for summarizing articles", prompt="Summarize this article into bullet points:\n{item}")
+
+combine_chain = AgentChainElement("out_1", system_prompt="You are an advanced AI agent that summarizes text", prompt="Please combine the bullet points of different summaries below, into one summary as bullet points:\n{map_output}")
+
+map_chain = MapChain(agent, [summary_chain], [combine_chain])
+
+
+article_list = [
+    """### 1. Quantum Computing: The Next Frontier in Computational Power
+
+**Introduction**
+Quantum computing represents a revolutionary approach to information processing, leveraging the principles of quantum mechanics to solve problems that are intractable for classical computers. This article explores the fundamental concepts of quantum computing, its potential applications, and the challenges it faces.
+
+**Quantum Mechanics and Computing**
+Quantum computers use quantum bits, or qubits, which can exist in multiple states simultaneously, thanks to superposition. This capability, combined with entanglement—where the state of one qubit can depend on the state of another, no matter the distance between them—allows quantum computers to process a vast number of possibilities concurrently.
+
+**Quantum Algorithms**
+Several algorithms have been developed for quantum computers that show significant speed-ups over their classical counterparts. Shor’s Algorithm, for instance, can factorize large integers exponentially faster than the best-known classical algorithms, which has profound implications for cryptography. Grover's Algorithm offers a quadratic speedup for unstructured search problems.
+
+**Applications**
+Quantum computing has potential applications across various fields:
+- **Cryptography**: Secure communication through quantum key distribution.
+- **Drug Discovery**: Modeling molecular interactions at quantum levels to predict drug efficacy and side effects.
+- **Optimization Problems**: Enhancing solutions in logistics, finance, and materials science.
+
+**Challenges**
+Despite its potential, quantum computing faces several hurdles:
+- **Qubit Coherence**: Maintaining the state of qubits for sufficient time is challenging due to decoherence.
+- **Error Rates**: Quantum gates are prone to errors significantly higher than conventional binary computing gates.
+- **Scalability**: Building machines with enough qubits to be useful for complex problems is currently beyond our reach.
+
+**Conclusion**
+Quantum computing is still in its infancy, but it holds the promise of massive computational power. The coming decades are likely to see significant advancements in this field as researchers overcome its current limitations.""",
+    """### 2. Machine Learning: Transforming Data into Insights
+
+**Introduction**
+Machine Learning (ML) is a branch of artificial intelligence that focuses on building applications that can learn from data and improve their accuracy over time without being explicitly programmed. This article delves into the types of ML, key algorithms, applications, and future prospects.
+
+**Types of Machine Learning**
+- **Supervised Learning**: Models predict outputs based on input data, and learning is guided by comparing actual and predicted outputs.
+- **Unsupervised Learning**: Algorithms identify patterns in data without reference to known or labeled outcomes.
+- **Reinforcement Learning**: Models learn to make sequences of decisions by receiving rewards or penalties.
+
+**Key Algorithms**
+- **Linear Regression** and **Logistic Regression** for predictive modeling.
+- **Decision Trees** and **Random Forests** for classification and regression tasks.
+- **Neural Networks**: Used in deep learning for complex pattern recognition, such as in image and speech recognition.
+
+**Applications**
+- **Healthcare**: From diagnosing diseases to personalized medicine.
+- **Finance**: For credit scoring, algorithmic trading, and risk assessment.
+- **Retail**: Enhancing customer experience through personalized recommendations.
+
+**Challenges and Future Prospects**
+The field of ML is not without challenges, including data privacy concerns, the need for large labeled datasets, and the risk of creating biased models. However, ongoing research in areas like unsupervised learning, transfer learning, and the development of more robust models promises to mitigate these issues.
+
+**Conclusion**
+Machine learning continues to be a dynamic field of research and application, with the potential to impact numerous sectors profoundly.""",
+    """### 3. Blockchain Technology: Decentralizing Trust
+
+**Introduction**
+Blockchain technology is best known as the backbone of cryptocurrencies like Bitcoin, but its applications extend far beyond. This article outlines the technology’s fundamentals, applications beyond finance, and the challenges it faces.
+
+**Blockchain Basics**
+A blockchain is a decentralized ledger of all transactions across a network. Each transaction is added to a "block" and linked to the previous block, forming a "chain." This structure, combined with cryptographic techniques, makes it secure and immutable.
+
+**Key Features**
+- **Decentralization**: No single point of control or failure.
+- **Transparency**: Changes to the public blockchain are viewable by all parties creating transparency.
+- **Immutability**: Once a transaction is recorded, it cannot be altered, increasing trust.
+
+**Applications**
+- **Supply Chain Management**: Enhancing transparency and traceability.
+- **Healthcare**: Secure sharing of medical records.
+- **Smart Contracts**: Automatically executing contracts when conditions are met.
+
+**Challenges**
+- **Scalability**: Current blockchain solutions, like Bitcoin, have limitations on transaction speed and volume.
+- **Regulatory Issues**: Balancing the need for regulation with the ethos of decentralization.
+- **Energy Consumption**: The energy requirement for "mining" transactions, particularly in networks like Bitcoin, is substantial.
+
+**Conclusion**
+Blockchain technology holds great promise for creating a more transparent and efficient world, but significant challenges must be addressed to realize its full potential."""
+]
+
+
+map_chain.run_map_chain(items_to_map=article_list)
+```
+
 ### Knowledge Graph Creation Example
 This example, based on an example of the Instructor library for OpenAI,
 demonstrates how to create a knowledge graph using the llama-cpp-agent framework.
 ```python
 import json
 from typing import List
```

### Comparing `llama_cpp_agent-0.1.0/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.1.1/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 LICENSE
 ReadMe.md
 pyproject.toml
 src/llama_cpp_agent/__init__.py
+src/llama_cpp_agent/chain.py
 src/llama_cpp_agent/function_calling.py
 src/llama_cpp_agent/function_calling_agent.py
+src/llama_cpp_agent/hermes_2_pro_agent.py
 src/llama_cpp_agent/llm_agent.py
 src/llama_cpp_agent/llm_prompt_template.py
 src/llama_cpp_agent/llm_settings.py
+src/llama_cpp_agent/messages.py
 src/llama_cpp_agent/messages_formatter.py
 src/llama_cpp_agent/mixtral_8x22b_agent.py
 src/llama_cpp_agent/output_parser.py
 src/llama_cpp_agent/structured_output_agent.py
 src/llama_cpp_agent.egg-info/PKG-INFO
 src/llama_cpp_agent.egg-info/SOURCES.txt
 src/llama_cpp_agent.egg-info/dependency_links.txt
@@ -25,10 +28,11 @@
 src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
 src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
 src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
 src/llama_cpp_agent/providers/__init__.py
 src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
 src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
 src/llama_cpp_agent/providers/openai_endpoint_provider.py
+src/llama_cpp_agent/providers/provider_base.py
 src/llama_cpp_agent/rag/__init__.py
 src/llama_cpp_agent/rag/rag_colbert_reranker.py
 src/llama_cpp_agent/rag/text_utils.py
```

