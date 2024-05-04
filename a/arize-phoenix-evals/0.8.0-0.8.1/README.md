# Comparing `tmp/arize_phoenix_evals-0.8.0.tar.gz` & `tmp/arize_phoenix_evals-0.8.1.tar.gz`

## Comparing `arize_phoenix_evals-0.8.0.tar` & `arize_phoenix_evals-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/__init__.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/classify.py
--rw-r--r--   0        0        0    30320 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/default_templates.py
--rw-r--r--   0        0        0    15930 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/evaluators.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/exceptions.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/executors.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/py.typed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/retrievals.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/templates.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/utils.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/anthropic.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/base.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/bedrock.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/litellm.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/mistralai.py
--rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/openai.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/rate_limiters.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/vertex.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/src/phoenix/evals/models/vertexai.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/LICENSE
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/__init__.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/classify.py
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/default_templates.py
+-rw-r--r--   0        0        0    15930 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/evaluators.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/exceptions.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/executors.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/py.typed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/retrievals.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/templates.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/utils.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/anthropic.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/base.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/bedrock.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/litellm.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/mistralai.py
+-rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/openai.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/rate_limiters.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertex.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertexai.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/README.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.1/PKG-INFO
```

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/__init__.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/classify.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/classify.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/default_templates.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/default_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 ************
 
 EXPLANATION:"""
 
 HALLUCINATION_PROMPT_RAILS_MAP = OrderedDict({True: "hallucinated", False: "factual"})
 HALLUCINATION_PROMPT_BASE_TEMPLATE = """
 In this task, you will be presented with a query, a reference text and an answer. The answer is
-generated to the question based on the reference text. The answer may contain false information, you
+generated to the question based on the reference text. The answer may contain false information. You
 must use the reference text to determine if the answer to the question contains false information,
-if the answer is a hallucination of facts. Your objective is to determine whether the reference text
-contains factual information and is not a hallucination. A 'hallucination' in this context refers to
+if the answer is a hallucination of facts. Your objective is to determine whether the answer text
+contains factual information and is not a hallucination. A 'hallucination' refers to
 an answer that is not based on the reference text or assumes information that is not available in
 the reference text. Your response should be a single word: either "factual" or "hallucinated", and
 it should not include any other text or characters. "hallucinated" indicates that the answer
 provides factually inaccurate information to the query based on the reference text. "factual"
 indicates that the answer to the question is correct relative to the reference text, and does not
 contain made up information. Please read the query and reference text carefully before determining
 your response.
@@ -72,18 +72,18 @@
     ************
     [END DATA]
 
     Is the answer above factual or hallucinated based on the query and reference text?
 """
 HALLUCINATION_PROMPT_TEMPLATE_WITH_EXPLANATION = """
 In this task, you will be presented with a query, a reference text and an answer. The answer is
-generated to the question based on the reference text. The answer may contain false information, you
+generated to the question based on the reference text. The answer may contain false information. You
 must use the reference text to determine if the answer to the question contains false information,
-if the answer is a hallucination of facts. Your objective is to determine whether the reference text
-contains factual information and is not a hallucination. A 'hallucination' in this context refers to
+if the answer is a hallucination of facts. Your objective is to determine whether the answer text
+contains factual information and is not a hallucination. A 'hallucination' refers to
 an answer that is not based on the reference text or assumes information that is not available in
 the reference text.
 
     [BEGIN DATA]
     ************
     [Query]: {input}
     ************
```

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/evaluators.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/evaluators.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/executors.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/executors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/generate.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/generate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/retrievals.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/retrievals.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/templates.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/utils.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/anthropic.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/base.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/base.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/bedrock.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/litellm.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/litellm.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/mistralai.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/mistralai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/openai.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/openai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/rate_limiters.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/vertex.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertex.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/src/phoenix/evals/models/vertexai.py` & `arize_phoenix_evals-0.8.1/src/phoenix/evals/models/vertexai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/LICENSE` & `arize_phoenix_evals-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/README.md` & `arize_phoenix_evals-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.0/pyproject.toml` & `arize_phoenix_evals-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-version = "0.8.0"
+version = "0.8.1"
 dependencies = [
   "pandas",
   "tqdm",
   "typing-extensions>=4.5, <5",
 ]
 
 [project.optional-dependencies]
```

### Comparing `arize_phoenix_evals-0.8.0/PKG-INFO` & `arize_phoenix_evals-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arize-phoenix-evals
-Version: 0.8.0
+Version: 0.8.1
 Summary: LLM Evaluations
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
 License: Elastic-2.0
 License-File: IP_NOTICE
```

