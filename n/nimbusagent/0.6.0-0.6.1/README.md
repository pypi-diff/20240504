# Comparing `tmp/nimbusagent-0.6.0.tar.gz` & `tmp/nimbusagent-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbusagent-0.6.0.tar", last modified: Sat Apr 20 10:59:27 2024, max compression
+gzip compressed data, was "nimbusagent-0.6.1.tar", last modified: Sat May  4 14:32:48 2024, max compression
```

## Comparing `nimbusagent-0.6.0.tar` & `nimbusagent-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.919646 nimbusagent-0.6.0/
--rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.6.0/.gitignore
--rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.6.0/LICENSE.txt
--rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.6.0/MANIFEST.in
--rw-r--r--   0 Lee        (501) staff       (20)    10527 2024-04-20 10:59:27.918787 nimbusagent-0.6.0/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     7992 2024-04-16 23:09:24.000000 nimbusagent-0.6.0/README.md
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.829045 nimbusagent-0.6.0/bin/
--rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.6.0/bin/build.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.6.0/bin/publish-pypi.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.6.0/bin/run_tests.sh
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.845623 nimbusagent-0.6.0/examples/
--rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/completion_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/examples/completion_agent_function_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/completion_agent_history_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/streaming_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/examples/streaming_agent_function_example.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.851482 nimbusagent-0.6.0/examples/streaming_cli_chatbot/
--rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.6.0/examples/streaming_cli_chatbot/simple_spinner.py
--rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.852094 nimbusagent-0.6.0/nimbusagent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/__init__.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.870413 nimbusagent-0.6.0/nimbusagent/agent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/agent/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    14119 2024-04-20 10:50:08.000000 nimbusagent-0.6.0/nimbusagent/agent/base.py
--rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.6.0/nimbusagent/agent/completion.py
--rw-r--r--   0 Lee        (501) staff       (20)    12853 2024-04-16 22:49:59.000000 nimbusagent-0.6.0/nimbusagent/agent/streaming.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.884684 nimbusagent-0.6.0/nimbusagent/functions/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/functions/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    18224 2024-04-20 10:54:04.000000 nimbusagent-0.6.0/nimbusagent/functions/handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/functions/parser.py
--rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/nimbusagent/functions/responses.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.888450 nimbusagent-0.6.0/nimbusagent/memory/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/memory/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/memory/base.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.893131 nimbusagent-0.6.0/nimbusagent/utils/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/nimbusagent/utils/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.6.0/nimbusagent/utils/helper.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.918128 nimbusagent-0.6.0/nimbusagent.egg-info/
--rw-r--r--   0 Lee        (501) staff       (20)    10527 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/SOURCES.txt
--rw-r--r--   0 Lee        (501) staff       (20)        1 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/dependency_links.txt
--rw-r--r--   0 Lee        (501) staff       (20)       60 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/requires.txt
--rw-r--r--   0 Lee        (501) staff       (20)       12 2024-04-20 10:59:27.000000 nimbusagent-0.6.0/nimbusagent.egg-info/top_level.txt
--rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-04-20 10:54:04.000000 nimbusagent-0.6.0/pyproject.toml
--rw-r--r--   0 Lee        (501) staff       (20)       38 2024-04-20 10:59:27.919729 nimbusagent-0.6.0/setup.cfg
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-20 10:59:27.917451 nimbusagent-0.6.0/tests/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.6.0/tests/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     1962 2024-04-17 11:36:39.000000 nimbusagent-0.6.0/tests/test_nimbusagent_agent_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/tests/test_nimbusagent_functions_handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/tests/test_nimbusagent_functions_parser.py
--rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.6.0/tests/test_nimbusagent_functions_response.py
--rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.6.0/tests/test_nimbusagent_memory_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.6.0/tests/test_nimbusagent_utils.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.140842 nimbusagent-0.6.1/
+-rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.6.1/.gitignore
+-rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.6.1/LICENSE.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.6.1/MANIFEST.in
+-rw-r--r--   0 Lee        (501) staff       (20)    10816 2024-05-04 14:32:48.139629 nimbusagent-0.6.1/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     8281 2024-04-20 11:03:27.000000 nimbusagent-0.6.1/README.md
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.032114 nimbusagent-0.6.1/bin/
+-rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.6.1/bin/build.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.6.1/bin/publish-pypi.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.6.1/bin/run_tests.sh
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.050495 nimbusagent-0.6.1/examples/
+-rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/examples/completion_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.6.1/examples/completion_agent_function_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/examples/completion_agent_history_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/examples/streaming_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.6.1/examples/streaming_agent_function_example.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.059185 nimbusagent-0.6.1/examples/streaming_cli_chatbot/
+-rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.6.1/examples/streaming_cli_chatbot/simple_spinner.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.059639 nimbusagent-0.6.1/nimbusagent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/__init__.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.077779 nimbusagent-0.6.1/nimbusagent/agent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/agent/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    14406 2024-05-04 13:39:48.000000 nimbusagent-0.6.1/nimbusagent/agent/base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.6.1/nimbusagent/agent/completion.py
+-rw-r--r--   0 Lee        (501) staff       (20)    12853 2024-04-16 22:49:59.000000 nimbusagent-0.6.1/nimbusagent/agent/streaming.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.093216 nimbusagent-0.6.1/nimbusagent/functions/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/functions/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    18712 2024-05-03 23:04:50.000000 nimbusagent-0.6.1/nimbusagent/functions/handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/functions/parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.6.1/nimbusagent/functions/responses.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.098231 nimbusagent-0.6.1/nimbusagent/memory/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/memory/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/memory/base.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.105245 nimbusagent-0.6.1/nimbusagent/utils/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/nimbusagent/utils/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.6.1/nimbusagent/utils/helper.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.138242 nimbusagent-0.6.1/nimbusagent.egg-info/
+-rw-r--r--   0 Lee        (501) staff       (20)    10816 2024-05-04 14:32:47.000000 nimbusagent-0.6.1/nimbusagent.egg-info/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-05-04 14:32:48.000000 nimbusagent-0.6.1/nimbusagent.egg-info/SOURCES.txt
+-rw-r--r--   0 Lee        (501) staff       (20)        1 2024-05-04 14:32:47.000000 nimbusagent-0.6.1/nimbusagent.egg-info/dependency_links.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       60 2024-05-04 14:32:47.000000 nimbusagent-0.6.1/nimbusagent.egg-info/requires.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       12 2024-05-04 14:32:47.000000 nimbusagent-0.6.1/nimbusagent.egg-info/top_level.txt
+-rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-05-04 14:32:11.000000 nimbusagent-0.6.1/pyproject.toml
+-rw-r--r--   0 Lee        (501) staff       (20)       38 2024-05-04 14:32:48.140934 nimbusagent-0.6.1/setup.cfg
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-05-04 14:32:48.134838 nimbusagent-0.6.1/tests/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.6.1/tests/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1962 2024-04-17 11:36:39.000000 nimbusagent-0.6.1/tests/test_nimbusagent_agent_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.6.1/tests/test_nimbusagent_functions_handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/tests/test_nimbusagent_functions_parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.6.1/tests/test_nimbusagent_functions_response.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.6.1/tests/test_nimbusagent_memory_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.6.1/tests/test_nimbusagent_utils.py
```

### Comparing `nimbusagent-0.6.0/.gitignore` & `nimbusagent-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/LICENSE.txt` & `nimbusagent-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/PKG-INFO` & `nimbusagent-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.6.0
+Version: 0.6.1
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -165,37 +165,44 @@
 
 #### `functions_embeddings_model`
 
 - **Description**: The name of the OpenAI model to use for generating embeddings for the functions.
 - **Type**: `str`
 - **Default**: `'text-embedding-ada-002'`
 
+#### `functions_k_closest`
+
+- **Description**: The number of closest functions to consider when handling a query.
+- **Type**: `int`
+- **Default**: `3`
+
+#### `functions_min_similarity`
+
+- **Description**: The minimum similarity score for a function to be considered when handling a query.
+- **Type**: `float`
+- **Default**: `0.5`
+
 #### `functions_always_use`
 
 - **Description**: Functions that should always be used by the agent.
 - **Type**: `Optional[List[str]]`
 - **Default**: `None`
 
 #### `functions_pattern_groups`
 
 - **Description**: Pattern groups for matching functions to user queries.
 - **Type**: `Optional[List[dict]]`
 - **Default**: `None`
 
-#### `functions_k_closest`
-
-- **Description**: The number of closest functions to consider when handling a query.
-- **Type**: `int`
-- **Default**: `3`
+#### `functions_pattern_mode`
 
-#### `functions_min_similarity`
-
-- **Description**: The minimum similarity score for a function to be considered when handling a query.
-- **Type**: `float`
-- **Default**: `0.5`
+- **Description**: The mode for matching functions to user queries. Options are `all` to check all patterns, `first` to
+  use only the functions within the first group that has a matching pattern
+- **Type**: `Literal['all', 'first']`
+- **Default**: `'all'`
 
 #### `function_max_tokens`
 
 - **Description**: The maximum number of tokens to allow towards function definitions. This is useful for preventing
   using a large number of tokens from function definitions, thus lowering costs and preventing AI errors. Set to 0 for
   unlimited token usage
 - **Type**: `int`
```

### Comparing `nimbusagent-0.6.0/README.md` & `nimbusagent-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -112,37 +112,44 @@
 
 #### `functions_embeddings_model`
 
 - **Description**: The name of the OpenAI model to use for generating embeddings for the functions.
 - **Type**: `str`
 - **Default**: `'text-embedding-ada-002'`
 
+#### `functions_k_closest`
+
+- **Description**: The number of closest functions to consider when handling a query.
+- **Type**: `int`
+- **Default**: `3`
+
+#### `functions_min_similarity`
+
+- **Description**: The minimum similarity score for a function to be considered when handling a query.
+- **Type**: `float`
+- **Default**: `0.5`
+
 #### `functions_always_use`
 
 - **Description**: Functions that should always be used by the agent.
 - **Type**: `Optional[List[str]]`
 - **Default**: `None`
 
 #### `functions_pattern_groups`
 
 - **Description**: Pattern groups for matching functions to user queries.
 - **Type**: `Optional[List[dict]]`
 - **Default**: `None`
 
-#### `functions_k_closest`
-
-- **Description**: The number of closest functions to consider when handling a query.
-- **Type**: `int`
-- **Default**: `3`
+#### `functions_pattern_mode`
 
-#### `functions_min_similarity`
-
-- **Description**: The minimum similarity score for a function to be considered when handling a query.
-- **Type**: `float`
-- **Default**: `0.5`
+- **Description**: The mode for matching functions to user queries. Options are `all` to check all patterns, `first` to
+  use only the functions within the first group that has a matching pattern
+- **Type**: `Literal['all', 'first']`
+- **Default**: `'all'`
 
 #### `function_max_tokens`
 
 - **Description**: The maximum number of tokens to allow towards function definitions. This is useful for preventing
   using a large number of tokens from function definitions, thus lowering costs and preventing AI errors. Set to 0 for
   unlimited token usage
 - **Type**: `int`
```

### Comparing `nimbusagent-0.6.0/examples/completion_agent_function_example.py` & `nimbusagent-0.6.1/examples/completion_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/examples/streaming_agent_function_example.py` & `nimbusagent-0.6.1/examples/streaming_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/examples/streaming_cli_chatbot/simple_spinner.py` & `nimbusagent-0.6.1/examples/streaming_cli_chatbot/simple_spinner.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py` & `nimbusagent-0.6.1/examples/streaming_cli_chatbot/streaming_cli_chatbot.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent/agent/base.py` & `nimbusagent-0.6.1/nimbusagent/agent/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 class BaseAgent:
     def __init__(
             self,
             openai_api_key: str = None,
             model_name: str = DEFAULT_MODEL_NAME,
             secondary_model_name: str = DEFAULT_SECONDARY_MODEL_NAME,
             temperature: float = DEFAULT_TEMP,
-            max_tokens: int = 500,
+            max_tokens: int = 1000,
 
             functions: Optional[list] = None,
             functions_embeddings: Optional[List[dict]] = None,
             functions_embeddings_model: str = FUNCTIONS_EMBEDDING_MODEL,
+            function_embeddings_fetcher: Optional[callable] = None,
             functions_always_use: Optional[List[str]] = None,
             functions_pattern_groups: Optional[List[dict]] = None,
-            function_pattern_mode: Literal['all','first'] = 'all',
+            function_pattern_mode: Literal['all', 'first'] = 'all',
             functions_k_closest: int = 3,
             function_min_similarity: float = 0.5,
 
             function_max_tokens: int = 2000,
             use_tool_calls: bool = True,
 
             system_message: str = SYS_MSG,
@@ -129,14 +130,15 @@
             self.chat_history.set_chat_history(message_history)
 
         self.function_handler = self._init_function_handler(
             functions=functions,
             functions_embeddings=functions_embeddings,
             functions_embeddings_model=functions_embeddings_model,
             functions_k_closest=functions_k_closest,
+            function_embeddings_fetcher=function_embeddings_fetcher,
             functions_always_use=functions_always_use,
             functions_pattern_groups=functions_pattern_groups,
             function_pattern_mode=function_pattern_mode,
             function_max_tokens=function_max_tokens,
             function_min_similarity=function_min_similarity)
         self.use_tool_calls = use_tool_calls
 
@@ -147,18 +149,19 @@
         self.system_message = {"role": "system", "content": message}
 
     def _init_function_handler(self,
                                functions: Optional[List],
                                functions_embeddings: Optional[List],
                                functions_embeddings_model: str = FUNCTIONS_EMBEDDING_MODEL,
                                functions_k_closest: int = 3,
+                               function_embeddings_fetcher: Optional[callable] = None,
                                function_min_similarity: float = 0.5,
                                functions_always_use: Optional[List[str]] = None,
                                functions_pattern_groups: Optional[List[dict]] = None,
-                               function_pattern_mode: Literal['all','first'] = 'all',
+                               function_pattern_mode: Literal['all', 'first'] = 'all',
                                function_max_tokens: int = 0) -> FunctionHandler:
         """Initializes the function handler.
         Returns a FunctionHandler instance.
 
         :param functions: The list of functions to use
         :param functions_embeddings: The list of function embeddings to use
         :param functions_k_closest: The number of closest functions to use
@@ -167,14 +170,15 @@
         :return: A FunctionHandler instance
          """
 
         return FunctionHandler(
             functions=functions,
             embeddings=functions_embeddings,
             embeddings_model=functions_embeddings_model,
+            embeddings_fetcher=function_embeddings_fetcher,
             k_nearest=functions_k_closest,
             min_similarity=function_min_similarity,
             always_use=functions_always_use,
             pattern_groups=functions_pattern_groups,
             pattern_mode=function_pattern_mode,
             calling_function_start_callback=self.calling_function_start_callback,
             calling_function_stop_callback=self.calling_function_stop_callback,
```

### Comparing `nimbusagent-0.6.0/nimbusagent/agent/completion.py` & `nimbusagent-0.6.1/nimbusagent/agent/completion.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent/agent/streaming.py` & `nimbusagent-0.6.1/nimbusagent/agent/streaming.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent/functions/handler.py` & `nimbusagent-0.6.1/nimbusagent/functions/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import tiktoken
 from openai.types.chat import ChatCompletionToolParam
 
 from nimbusagent.functions import parser
 from nimbusagent.functions.responses import FuncResponse, DictFuncResponse
 from nimbusagent.memory.base import AgentMemory
-from nimbusagent.utils.helper import find_similar_embedding_list, combine_lists_unique, FUNCTIONS_EMBEDDING_MODEL
+from nimbusagent.utils.helper import combine_lists_unique, FUNCTIONS_EMBEDDING_MODEL, find_similar_embedding_list
 
 
 @dataclass
 class FunctionInfo:
     """
     Class that stores information about a function.
     """
@@ -53,28 +53,30 @@
     chat_history: AgentMemory = None
     processed_functions = None
     max_tokens = 0
 
     def __init__(self, functions: list = None,
                  embeddings: list = None,
                  embeddings_model: str = FUNCTIONS_EMBEDDING_MODEL,
+                 embeddings_fetcher: Callable = None,
                  k_nearest: int = 3,
                  min_similarity: float = 0.5,
                  always_use: list = None,
                  pattern_groups: list = None,
                  pattern_mode: Literal['all', 'first'] = 'all',
                  calling_function_start_callback: callable = None,
                  calling_function_stop_callback: callable = None,
                  chat_history: AgentMemory = None,
                  max_tokens: int = 0
                  ):
 
         self.embeddings = embeddings
         self.embeddings_model = embeddings_model
         self.k_nearest = k_nearest
+        self.embeddings_fetcher = embeddings_fetcher
         self.min_similarity = min_similarity
         self.always_use = always_use
         self.pattern_groups = pattern_groups
         self.pattern_mode = pattern_mode
         self.chat_history = chat_history
         self.encoding = tiktoken.get_encoding("cl100k_base")
         self.max_tokens = max_tokens
@@ -193,47 +195,54 @@
         Get the functions to use based on the query and history.
         :param query:  The query to use.
         :param history:  The history to use. A list of dictionaries with 'role' and 'content' fields.
         """
         if not self.orig_functions:
             return None
 
-        if not self.pattern_groups and not self.embeddings:
+        if not self.pattern_groups and not self.embeddings and not self.always_use:
             actual_function_names = self.orig_functions.keys()
 
         else:
             # Step 1: Initialize with 'always_use' functions
-            actual_function_names = self.always_use if self.always_use else []
-            # print("actual_function_names: ", actual_function_names)
+            if self.always_use:
+                actual_function_names = self.always_use
+            else:
+                actual_function_names = []
+
+            if self.embeddings_fetcher:
+                found_functions = self.embeddings_fetcher(query, history)
+                if found_functions:
+                    actual_function_names = combine_lists_unique(actual_function_names, found_functions)
+            else:
+                # step 2: Add functions based on pattern groups on query
+                query_group_functions = self._get_group_function(query)
+                if query_group_functions:
+                    actual_function_names = combine_lists_unique(actual_function_names, query_group_functions)
+
+                # step 3: Add functions based on embeddings
+                recent_history_and_query = [message['content'] for message in history[-2:]] + [query]
+                recent_history_and_query_str = " ".join(recent_history_and_query)
+
+                if self.embeddings:
+                    similar_functions = find_similar_embedding_list(recent_history_and_query_str,
+                                                                    function_embeddings=self.embeddings,
+                                                                    embeddings_model=self.embeddings_model,
+                                                                    k_nearest_neighbors=self.k_nearest)
+                    similar_function_names = [d['name'] for d in similar_functions]
+                    if similar_function_names:
+                        actual_function_names = combine_lists_unique(actual_function_names, similar_function_names)
+
+                    # step 4: Add functions based on pattern groups on history
+                    query_group_functions = self._get_group_function(recent_history_and_query_str)
+                    if query_group_functions:
+                        actual_function_names = combine_lists_unique(actual_function_names, query_group_functions)
 
-            # step 2: Add functions based on pattern groups on query
-            query_group_functions = self._get_group_function(query)
-            if query_group_functions:
-                actual_function_names = combine_lists_unique(actual_function_names, query_group_functions)
-
-            # step 3: Add functions based on embeddings
-            recent_history_and_query = [message['content'] for message in history[-2:]] + [query]
-            recent_history_and_query_str = " ".join(recent_history_and_query)
-
-            if self.embeddings:
-                similar_functions = find_similar_embedding_list(recent_history_and_query_str,
-                                                                function_embeddings=self.embeddings,
-                                                                embeddings_model=self.embeddings_model,
-                                                                k_nearest_neighbors=self.k_nearest)
-                similar_function_names = [d['name'] for d in similar_functions]
-                if similar_function_names:
-                    actual_function_names = combine_lists_unique(actual_function_names, similar_function_names)
-
-            # step 4: Add functions based on pattern groups on history
-            query_group_functions = self._get_group_function(recent_history_and_query_str)
-            if query_group_functions:
-                actual_function_names = combine_lists_unique(actual_function_names, query_group_functions)
-
-            logging.info(f"Actual Functions Names to use: {actual_function_names}")
-            # step 5: step through functions and get the function info, adding up to max_tokens
+        logging.info(f"Actual Functions Names to use: {actual_function_names}")
+        # step 5: step through functions and get the function info, adding up to max_tokens
 
         processed_functions = []
         token_count = 0
         for func_name in actual_function_names:
             func_info = self._get_function_info(func_name)
             if func_info:
                 processed_functions.append(func_info)
```

### Comparing `nimbusagent-0.6.0/nimbusagent/functions/parser.py` & `nimbusagent-0.6.1/nimbusagent/functions/parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent/functions/responses.py` & `nimbusagent-0.6.1/nimbusagent/functions/responses.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent/memory/base.py` & `nimbusagent-0.6.1/nimbusagent/memory/base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent/utils/helper.py` & `nimbusagent-0.6.1/nimbusagent/utils/helper.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/nimbusagent.egg-info/PKG-INFO` & `nimbusagent-0.6.1/nimbusagent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.6.0
+Version: 0.6.1
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -165,37 +165,44 @@
 
 #### `functions_embeddings_model`
 
 - **Description**: The name of the OpenAI model to use for generating embeddings for the functions.
 - **Type**: `str`
 - **Default**: `'text-embedding-ada-002'`
 
+#### `functions_k_closest`
+
+- **Description**: The number of closest functions to consider when handling a query.
+- **Type**: `int`
+- **Default**: `3`
+
+#### `functions_min_similarity`
+
+- **Description**: The minimum similarity score for a function to be considered when handling a query.
+- **Type**: `float`
+- **Default**: `0.5`
+
 #### `functions_always_use`
 
 - **Description**: Functions that should always be used by the agent.
 - **Type**: `Optional[List[str]]`
 - **Default**: `None`
 
 #### `functions_pattern_groups`
 
 - **Description**: Pattern groups for matching functions to user queries.
 - **Type**: `Optional[List[dict]]`
 - **Default**: `None`
 
-#### `functions_k_closest`
-
-- **Description**: The number of closest functions to consider when handling a query.
-- **Type**: `int`
-- **Default**: `3`
+#### `functions_pattern_mode`
 
-#### `functions_min_similarity`
-
-- **Description**: The minimum similarity score for a function to be considered when handling a query.
-- **Type**: `float`
-- **Default**: `0.5`
+- **Description**: The mode for matching functions to user queries. Options are `all` to check all patterns, `first` to
+  use only the functions within the first group that has a matching pattern
+- **Type**: `Literal['all', 'first']`
+- **Default**: `'all'`
 
 #### `function_max_tokens`
 
 - **Description**: The maximum number of tokens to allow towards function definitions. This is useful for preventing
   using a large number of tokens from function definitions, thus lowering costs and preventing AI errors. Set to 0 for
   unlimited token usage
 - **Type**: `int`
```

### Comparing `nimbusagent-0.6.0/nimbusagent.egg-info/SOURCES.txt` & `nimbusagent-0.6.1/nimbusagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/pyproject.toml` & `nimbusagent-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nimbusagent"
-version = "0.6.0"
+version = "0.6.1"
 description = "An OpenAI agent with basic memory, functions, and moderation support"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 keywords = [
     "openai",
     "gpt3",
     "gpt3.5",
```

### Comparing `nimbusagent-0.6.0/tests/test_nimbusagent_agent_base.py` & `nimbusagent-0.6.1/tests/test_nimbusagent_agent_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/tests/test_nimbusagent_functions_handler.py` & `nimbusagent-0.6.1/tests/test_nimbusagent_functions_handler.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/tests/test_nimbusagent_functions_parser.py` & `nimbusagent-0.6.1/tests/test_nimbusagent_functions_parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/tests/test_nimbusagent_functions_response.py` & `nimbusagent-0.6.1/tests/test_nimbusagent_functions_response.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/tests/test_nimbusagent_memory_base.py` & `nimbusagent-0.6.1/tests/test_nimbusagent_memory_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.6.0/tests/test_nimbusagent_utils.py` & `nimbusagent-0.6.1/tests/test_nimbusagent_utils.py`

 * *Files identical despite different names*

