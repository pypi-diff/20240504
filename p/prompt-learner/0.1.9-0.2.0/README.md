# Comparing `tmp/prompt_learner-0.1.9.tar.gz` & `tmp/prompt_learner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.1.9.tar", max compression
+gzip compressed data, was "prompt_learner-0.2.0.tar", max compression
```

## Comparing `prompt_learner-0.1.9.tar` & `prompt_learner-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,38 @@
--rw-r--r--   0        0        0     2140 2024-04-16 15:23:30.960382 prompt_learner-0.1.9/README.md
--rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.1.9/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.1.9/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0      240 2024-04-11 03:34:45.465265 prompt_learner-0.1.9/prompt_learner/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2024-04-11 03:18:16.055309 prompt_learner-0.1.9/prompt_learner/adapters/__pycache__/anthropic.cpython-311.pyc
--rw-r--r--   0        0        0     1470 2024-04-11 03:12:44.449954 prompt_learner-0.1.9/prompt_learner/adapters/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.1.9/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0     1261 2024-04-11 03:18:09.033090 prompt_learner-0.1.9/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      687 2024-04-19 02:14:47.310681 prompt_learner-0.1.9/prompt_learner/adapters/llama.py
--rw-r--r--   0        0        0      597 2024-04-11 03:12:12.072973 prompt_learner-0.1.9/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.1.9/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.1.9/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-04-18 07:01:26.041471 prompt_learner-0.1.9/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.1.9/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.1.9/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.1.9/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.1.9/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.1.9/prompt_learner/optimizers/descriptors/__init__.py
--rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.1.9/prompt_learner/optimizers/descriptors/descriptor.py
--rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.1.9/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.1.9/prompt_learner/optimizers/selectors/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.1.9/prompt_learner/optimizers/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.1.9/prompt_learner/optimizers/selectors/random_sampler.py
--rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.1.9/prompt_learner/optimizers/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.1.9/prompt_learner/optimizers/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.1.9/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      592 2024-04-18 08:15:47.085207 prompt_learner-0.1.9/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1005 2024-04-18 08:13:03.030889 prompt_learner-0.1.9/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.1.9/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      614 2024-04-18 01:51:33.806026 prompt_learner-0.1.9/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-04-18 06:38:05.061557 prompt_learner-0.1.9/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.1.9/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-04-18 07:03:05.419391 prompt_learner-0.1.9/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.1.9/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     2844 2024-04-18 08:23:15.734126 prompt_learner-0.1.9/prompt_learner/templates/anthropic_template.py
--rw-r--r--   0        0        0     2836 2024-04-19 02:21:05.344251 prompt_learner-0.1.9/prompt_learner/templates/llama_template.py
--rw-r--r--   0        0        0     2636 2024-04-19 02:42:03.868175 prompt_learner-0.1.9/prompt_learner/templates/openai_template.py
--rw-r--r--   0        0        0     1570 2024-04-18 06:49:29.458366 prompt_learner-0.1.9/prompt_learner/templates/template.py
--rw-r--r--   0        0        0      459 2024-04-19 02:44:40.413277 prompt_learner-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2817 1970-01-01 00:00:00.000000 prompt_learner-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2140 2024-04-16 15:23:30.960382 prompt_learner-0.2.0/README.md
+-rw-r--r--   0        0        0     6148 2024-04-12 21:48:53.225544 prompt_learner-0.2.0/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-04-11 03:24:46.950449 prompt_learner-0.2.0/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0      394 2024-03-30 07:34:49.479472 prompt_learner-0.2.0/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0     1291 2024-04-19 04:22:30.029307 prompt_learner-0.2.0/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      720 2024-04-19 04:23:36.748602 prompt_learner-0.2.0/prompt_learner/adapters/llama.py
+-rw-r--r--   0        0        0      662 2024-04-19 04:26:50.738576 prompt_learner-0.2.0/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1295 2024-04-12 22:29:26.768011 prompt_learner-0.2.0/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-04-11 03:23:09.786151 prompt_learner-0.2.0/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-18 07:01:26.041471 prompt_learner-0.2.0/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-03-30 04:43:35.605009 prompt_learner-0.2.0/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 06:22:23.812645 prompt_learner-0.2.0/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 06:22:57.915297 prompt_learner-0.2.0/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:44:07.604053 prompt_learner-0.2.0/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:24:34.521211 prompt_learner-0.2.0/prompt_learner/optimizers/descriptors/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-03 13:24:51.204583 prompt_learner-0.2.0/prompt_learner/optimizers/descriptors/descriptor.py
+-rw-r--r--   0        0        0       34 2024-03-30 05:23:18.250890 prompt_learner-0.2.0/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       30 2024-04-11 03:24:14.614552 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-12 21:34:12.452345 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      624 2024-04-12 23:18:56.744204 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/random_sampler.py
+-rw-r--r--   0        0        0      873 2024-04-12 23:12:29.480864 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-04-11 07:42:16.046290 prompt_learner-0.2.0/prompt_learner/optimizers/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       26 2024-04-11 03:24:06.645622 prompt_learner-0.2.0/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-02 04:09:00.049153 prompt_learner-0.2.0/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1136 2024-05-02 04:10:24.786688 prompt_learner-0.2.0/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       22 2024-04-11 03:23:46.852998 prompt_learner-0.2.0/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-02 04:33:01.819102 prompt_learner-0.2.0/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-04-18 06:38:05.061557 prompt_learner-0.2.0/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-04-11 03:43:06.447386 prompt_learner-0.2.0/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-04-18 07:03:05.419391 prompt_learner-0.2.0/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-04-11 03:23:57.503062 prompt_learner-0.2.0/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2819 2024-05-03 22:21:49.890118 prompt_learner-0.2.0/prompt_learner/templates/claude_template.py
+-rw-r--r--   0        0        0     2610 2024-05-03 22:22:14.955790 prompt_learner-0.2.0/prompt_learner/templates/gpt_template.py
+-rw-r--r--   0        0        0     2824 2024-05-03 22:21:49.889834 prompt_learner-0.2.0/prompt_learner/templates/llama_template.py
+-rw-r--r--   0        0        0     1570 2024-04-18 06:49:29.458366 prompt_learner-0.2.0/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0     3373 2024-05-03 05:36:59.720092 prompt_learner-0.2.0/prompt_learner/translator/translate.py
+-rw-r--r--   0        0        0      459 2024-05-03 22:31:16.739118 prompt_learner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2817 1970-01-01 00:00:00.000000 prompt_learner-0.2.0/PKG-INFO
```

### Comparing `prompt_learner-0.1.9/README.md` & `prompt_learner-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/.DS_Store` & `prompt_learner-0.2.0/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.2.0/prompt_learner/adapters/anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from langchain_anthropic import ChatAnthropic
 from dotenv import load_dotenv
 from .adapter import Adapter
 
 
 class Anthropic(Adapter):
     """An adapter for an Anthropic language model call"""
-    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024):
+    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024, model_name: str = "claude-3-haiku-20240307"):
         super().__init__(temperature, max_tokens)
         load_dotenv()
         self.llm = ChatAnthropic(
                 anthropic_api_key=os.getenv('ANTHROPIC_API_KEY'),
-                model="claude-3-haiku-20240307",
+                model=model_name,
                 temperature=self.temperature,
                 max_tokens=self.max_tokens)
 
     def extract_xml_tag(self, data: str, tag: str) -> str:
         """Extracts the data between the XML tags."""
         open_tag = "<" + tag + ">"
         close_tag = "</" + tag + ">"
```

### Comparing `prompt_learner-0.1.9/prompt_learner/adapters/llama.py` & `prompt_learner-0.2.0/prompt_learner/adapters/llama.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from langchain_fireworks import ChatFireworks
 from dotenv import load_dotenv
 from .adapter import Adapter
 
 
 class Llama(Adapter):
     """An adapter for a llama model call using fireworks"""
-    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024):
+    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024, model_name: str = "llama-v3-70b-instruct"):
         super().__init__(temperature, max_tokens)
         load_dotenv()
         self.llm = ChatFireworks(
-            model='accounts/fireworks/models/llama-v3-70b-instruct',
+            model='accounts/fireworks/models/'+model_name,
             fireworks_api_key=os.getenv('FIREWORKS_API_KEY'),
             temperature=self.temperature,
             max_tokens=self.max_tokens)
```

### Comparing `prompt_learner-0.1.9/prompt_learner/adapters/openai.py` & `prompt_learner-0.2.0/prompt_learner/adapters/openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from langchain_openai import ChatOpenAI
 from dotenv import load_dotenv
 from .adapter import Adapter
 
 
 class OpenAI(Adapter):
     """An adapter for an OpenAI language model call"""
-    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024):
+    def __init__(self, temperature: float = 0.0, max_tokens: int = 1024, model_name: str = "gpt-3.5-turbo"):
         super().__init__(temperature, max_tokens)
         load_dotenv()
         self.llm = ChatOpenAI(
             openai_api_key=os.getenv('OPENAI_API_KEY'),
+            model=model_name,
             temperature=self.temperature,
             max_tokens=self.max_tokens)
```

### Comparing `prompt_learner-0.1.9/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.2.0/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/optimizers/selectors/diverse_sampler.py` & `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/optimizers/selectors/random_sampler.py` & `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/optimizers/selectors/selector.py` & `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/optimizers/selectors/stratified_sampler.py` & `prompt_learner-0.2.0/prompt_learner/optimizers/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/prompts/cot.py` & `prompt_learner-0.2.0/prompt_learner/prompts/cot.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,8 +7,8 @@
     """Think step by step"""
     custom_intructions: str = Field(description="""Custom intructions for Chain
                                  of Thought Prompting""",
                                  default="Think step by step.\n")
     
     def assemble_prompt(self):
         """Assemble the prompt."""
-        self.prompt = f"""{self.template.descriptor}{self.template.examples_preamble}{self.template.format_examples(self.selector.selected_examples)}{self.custom_intructions}"""
+        self.prompt = f"""{self.template.descriptor}{self.template.examples_preamble}{self.template.format_examples(self.template.task.selected_examples)}{self.custom_intructions}"""
```

### Comparing `prompt_learner-0.1.9/prompt_learner/tasks/classification.py` & `prompt_learner-0.2.0/prompt_learner/tasks/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 
 class ClassificationTask(Task):
     """Classification"""
     allowed_labels: List[str] = []
 
     def validate_example(self, example: Example):
         """Validate the example for tagging task."""
-        labels = example.label.split(',')  # Handle multiple labels
+        labels = example.label.split(',')  # Handle multiple labels #TO_DO bug
         allowed_labels_set = set(self.allowed_labels)  # Convert to set
         if not all(label.strip() in allowed_labels_set for label in labels):
             return False
         return True
```

### Comparing `prompt_learner-0.1.9/prompt_learner/tasks/tagging.py` & `prompt_learner-0.2.0/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/tasks/task.py` & `prompt_learner-0.2.0/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/prompt_learner/templates/anthropic_template.py` & `prompt_learner-0.2.0/prompt_learner/templates/llama_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""This module contains the AnthropicCompletionTemplate class"""
+"""This module contains the ClaudeTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class AnthropicCompletionTemplate(Template):
-    """This class generates a template for Anthropic completions"""
+class LlamaCompletionTemplate(Template):
+    """This class generates a template for Llama completions"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
         self.descriptor = f"""You are a helpful AI assistant.\nYou are helping a user with a {self.task_type} task.\nThe user gives you the following task description.\n<task_description>{self.task_description}</task_description>\n"""
         if self.allowed_labels:
-            self.descriptor += """You have to select from the following labels.\n<allowed_labels>{self.allowed_labels}</allowed_labels>"""
+            self.descriptor += f"""You have to select from the following labels.\n<allowed_labels>{self.allowed_labels}</allowed_labels>"""
         if self.task_type in tasks_with_labels:
             self.prediction_preamble = f"""Given the text, you have to now predict the labels from list of allowed labels - {self.allowed_labels}.\nOutput only the label(s) and close the <label> tag."""
         elif self.task_type == "SQLGeneration":
             self.prediction_preamble = """Given the text, you have to now generate a SQL query.\nOnly the SQL query is expected."""
         else:  #generic preamble for prediction
             self.prediction_preamble = """Given the text, you have to now predict."""
         self.examples_preamble = """Here are a few examples to help you understand the task better.\n"""
```

### Comparing `prompt_learner-0.1.9/prompt_learner/templates/llama_template.py` & `prompt_learner-0.2.0/prompt_learner/templates/claude_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""This module contains the AnthropicCompletionTemplate class"""
+"""This module contains the ClaudeTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class LlamaCompletionTemplate(Template):
-    """This class generates a template for Llama completions"""
+class ClaudeTemplate(Template):
+    """This class generates a template for Anthropic completions"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
         self.descriptor = f"""You are a helpful AI assistant.\nYou are helping a user with a {self.task_type} task.\nThe user gives you the following task description.\n<task_description>{self.task_description}</task_description>\n"""
         if self.allowed_labels:
-            self.descriptor += """You have to select from the following labels.\n<allowed_labels>{self.allowed_labels}</allowed_labels>"""
+            self.descriptor += f"""You have to select from the following labels.\n<allowed_labels>{self.allowed_labels}</allowed_labels>"""
         if self.task_type in tasks_with_labels:
             self.prediction_preamble = f"""Given the text, you have to now predict the labels from list of allowed labels - {self.allowed_labels}.\nOutput only the label(s) and close the <label> tag."""
         elif self.task_type == "SQLGeneration":
             self.prediction_preamble = """Given the text, you have to now generate a SQL query.\nOnly the SQL query is expected."""
         else:  #generic preamble for prediction
             self.prediction_preamble = """Given the text, you have to now predict."""
         self.examples_preamble = """Here are a few examples to help you understand the task better.\n"""
```

### Comparing `prompt_learner-0.1.9/prompt_learner/templates/openai_template.py` & `prompt_learner-0.2.0/prompt_learner/templates/gpt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""This module contains the OpenAICompletionTemplate class"""
+"""This module contains the GPTTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class OpenAICompletionTemplate(Template):
+class GPTTemplate(Template):
     """This class generates a template for OpenAI completions"""
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
         self.descriptor = f"""You are a helpful AI assistant.\nYou are helping a user with a {self.task_type} task.\nThe user gives you the following task description.\n{self.task_description}\n"""
         if self.allowed_labels:
```

### Comparing `prompt_learner-0.1.9/prompt_learner/templates/template.py` & `prompt_learner-0.2.0/prompt_learner/templates/template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.1.9/PKG-INFO` & `prompt_learner-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.3.0,<25.0.0)
 Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: langchain-anthropic (>=0.1.4,<0.2.0)
 Requires-Dist: langchain-fireworks (>=0.1.2,<0.2.0)
-Requires-Dist: langchain-openai (>=0.1.1,<0.2.0)
+Requires-Dist: langchain-openai (>=0.1.5,<0.2.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Prompt Learner
 
 [![Documentation](https://img.shields.io/badge/docs-promptlearner.attuna.xyz-blue.svg)](https://promptlearner.attuna.xyz/)
```

