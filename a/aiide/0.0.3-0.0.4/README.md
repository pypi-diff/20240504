# Comparing `tmp/aiide-0.0.3.tar.gz` & `tmp/aiide-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiide-0.0.3.tar", max compression
+gzip compressed data, was "aiide-0.0.4.tar", max compression
```

## Comparing `aiide-0.0.3.tar` & `aiide-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-30 21:07:58.276939 aiide-0.0.3/LICENSE
--rw-r--r--   0        0        0     7020 2024-04-30 23:02:50.395209 aiide-0.0.3/README.md
--rw-r--r--   0        0        0       69 2024-04-30 23:06:31.258846 aiide-0.0.3/aiide/__init__.py
--rw-r--r--   0        0        0     8773 2024-04-30 22:57:06.380972 aiide-0.0.3/aiide/_aiide.py
--rw-r--r--   0        0        0      716 2024-04-30 17:44:07.018305 aiide-0.0.3/aiide/_utils.py
--rw-r--r--   0        0        0       27 2024-04-30 17:41:28.404617 aiide-0.0.3/aiide/tools/__init__.py
--rw-r--r--   0        0        0     6557 2024-04-30 18:01:53.387520 aiide-0.0.3/aiide/tools/_definitions.py
--rw-r--r--   0        0        0      288 2024-04-30 23:06:12.115676 aiide-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7438 1970-01-01 00:00:00.000000 aiide-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 01:38:36.118230 aiide-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7957 2024-05-04 01:38:36.118230 aiide-0.0.4/README.md
+-rw-r--r--   0        0        0       69 2024-05-04 01:38:36.118230 aiide-0.0.4/aiide/__init__.py
+-rw-r--r--   0        0        0     8773 2024-05-04 01:38:36.118230 aiide-0.0.4/aiide/_aiide.py
+-rw-r--r--   0        0        0      716 2024-05-04 01:38:36.118230 aiide-0.0.4/aiide/_utils.py
+-rw-r--r--   0        0        0       27 2024-05-04 01:38:36.118230 aiide-0.0.4/aiide/tools/__init__.py
+-rw-r--r--   0        0        0     6557 2024-05-04 01:38:36.118230 aiide-0.0.4/aiide/tools/_definitions.py
+-rw-r--r--   0        0        0      445 2024-05-04 01:38:36.122230 aiide-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8590 1970-01-01 00:00:00.000000 aiide-0.0.4/PKG-INFO
```

### Comparing `aiide-0.0.3/LICENSE` & `aiide-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiide-0.0.3/README.md` & `aiide-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 <div align="center"><picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/figures/logo_dark.svg">
-  <img alt="aiide" src="docs/figures/logo.svg" width=200">
+  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Anilturaga/aiide/blob/main/docs/figures/logo_dark.svg?raw=True">
+  <img alt="aiide" src="https://github.com/Anilturaga/aiide/blob/main/docs/figures/logo.svg?raw=True" width=200">
 </picture></div>
 <br/>
 
 
-**`aiide`** facilitates the creation of reinforcement learning (RL)-type environments for large language models (LLMs). It allows you to define and manage live data structures (components) that collectively form the environment (ENV). The LLM can interact with and modify these components by using user provided tools. After each action, along with the tool response, aiide adds the latest snapshot/state of all ENV components and removes all older ENV snapshots from the LLM's memory.
+**[`aiide`](https://github.com/Anilturaga/aiide)** facilitates the creation of reinforcement learning (RL)-type environments for large language models (LLMs). It allows you to define and manage live data structures (components) that collectively form the environment (ENV). The LLM can interact with and modify these components by using user provided tools. After each action, along with the tool response, aiide adds the latest snapshot/state of all ENV components and removes all older ENV snapshots from the LLM's memory.
 
 <div align="center"><picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/figures/aiide_overview.png">
-  <img alt="guidance" src="docs/figures/aiide_overview.png" width=700">
+  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Anilturaga/aiide/blob/main/docs/figures/aiide_overview.png?raw=true">
+  <img alt="AIIDE Overview" src="https://github.com/Anilturaga/aiide/blob/main/docs/figures/aiide_overview.png?raw=true" width=500">
+</picture></div>
+<br/>
+ENV states are made available to the LLM in the following way:
+<div align="center"><picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/figures/aiide_memory_logic.png">
+  <img alt="AIIDE Memory updates" src="https://github.com/Anilturaga/aiide/blob/main/docs/figures/aiide_memory_logic.png?raw=true" width=700">
 </picture></div>
 <br/>
 
 ### Tutorial
 Let's build a simple form filling agent. We have a pandas dataframe with field names and we want the LLM to ask the user for answers to a couple of questions at a time and populate the said dataframe.
 
 Here
 * The environment is the dataframe
 * We need a single tool that enables the LLM to add or edit values for any of the fields
 * _The library will automatically provide the latest snapshot of the dataframe to the LLM.(aiide will automatically remove older snapshots of the dataframe from the LLM memory to avoid confusing it and saving tokens)_
 
 0. Install the package<br/>
-`pip install aiide`
+```bash
+pip install aiide
+```
 
 1. Let's start with defining a simple chat agent
 
 ```python
 # Import the AIIDE class
 from aiide import AIIDE
 # Import helper classes for defining functions for the LLM
@@ -75,20 +83,24 @@
                 ]
             )
         
         # Main function of the tool is called when the tool is invoked by the agent
         def main(self, field_name,value):
             # let's set the value in the master dataframe
             self.parent.df.loc[self.parent.df['Field'] == field_name, 'Value'] = value
+            # Update the ENV
+            self.parent.ENV[0] = self.parent.df.to_markdown(index=False)
             # response to the agent
             return "Added value '"+str(value) + " to Field '"+field_name+"'"
 
 ```
 > `TOOL_DEF` is a helper proxy for the JSON-SCHEMA of OpenAI function calling. You can directly add the json or even use your own pydantic model's `model_json()`. `TOOL_DEF` and associated `tools.*` would make the code less verbose and have the advantage of intellisense.
 
+Checkout <br/>**[aiide's tool use tutorial](https://github.com/Anilturaga/aiide/blob/main/docs/tool_definitions.md)**
+
 3. That's it. We can now start using the agent
 
 `chat` is the function you invoke to start streaming agent response
 ```python
 # create the agent instance
 agent = FormFillingAgent()
 while True:
@@ -129,14 +141,16 @@
 
         def main(self, field_name,value):
             if self.user_consent == False:
                 return "User has rejected the insert, please try again"
 
             # let's set the value in the master dataframe
             self.parent.df.loc[self.parent.df['Field'] == field_name, 'Value'] = value
+            # Update the ENV
+            self.parent.ENV[0] = self.parent.df.to_markdown(index=False)
             # response to the agent
             return "Added value '"+str(value) + " to Field '"+field_name+"'"
 
 agent = FormFillingAgent()
 while True:
     user_query = input("User: ")
     for each in agent.chat(user_query, tools=["add_or_modify_form_values"]):
@@ -154,20 +168,7 @@
         if each["type"] == "tool_response":
             print("TOOL RESPONSE",each["tool_response"])
 
 ```
 
 5. Bonus!
 You can use completions and stop sequences in the `chat` function's arguments to implement prompting techniques such as ReAct, CoT etc!
-
-
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `aiide-0.0.3/aiide/_aiide.py` & `aiide-0.0.4/aiide/_aiide.py`

 * *Files identical despite different names*

### Comparing `aiide-0.0.3/aiide/_utils.py` & `aiide-0.0.4/aiide/_utils.py`

 * *Files identical despite different names*

### Comparing `aiide-0.0.3/aiide/tools/_definitions.py` & `aiide-0.0.4/aiide/tools/_definitions.py`

 * *Files identical despite different names*

### Comparing `aiide-0.0.3/PKG-INFO` & `aiide-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 Metadata-Version: 2.1
 Name: aiide
-Version: 0.0.3
+Version: 0.0.4
 Summary: Live components for your LLM
+Home-page: https://github.com/Anilturaga/aiide
+License: Apache-2.0
+Keywords: llm,rl,openai
 Author: Anilturaga
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.24.0,<2.0.0)
+Project-URL: Repository, https://github.com/Anilturaga/aiide
 Description-Content-Type: text/markdown
 
 <div align="center"><picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/figures/logo_dark.svg">
-  <img alt="aiide" src="docs/figures/logo.svg" width=200">
+  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Anilturaga/aiide/blob/main/docs/figures/logo_dark.svg?raw=True">
+  <img alt="aiide" src="https://github.com/Anilturaga/aiide/blob/main/docs/figures/logo.svg?raw=True" width=200">
 </picture></div>
 <br/>
 
 
-**`aiide`** facilitates the creation of reinforcement learning (RL)-type environments for large language models (LLMs). It allows you to define and manage live data structures (components) that collectively form the environment (ENV). The LLM can interact with and modify these components by using user provided tools. After each action, along with the tool response, aiide adds the latest snapshot/state of all ENV components and removes all older ENV snapshots from the LLM's memory.
+**[`aiide`](https://github.com/Anilturaga/aiide)** facilitates the creation of reinforcement learning (RL)-type environments for large language models (LLMs). It allows you to define and manage live data structures (components) that collectively form the environment (ENV). The LLM can interact with and modify these components by using user provided tools. After each action, along with the tool response, aiide adds the latest snapshot/state of all ENV components and removes all older ENV snapshots from the LLM's memory.
 
 <div align="center"><picture>
-  <source media="(prefers-color-scheme: dark)" srcset="docs/figures/aiide_overview.png">
-  <img alt="guidance" src="docs/figures/aiide_overview.png" width=700">
+  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Anilturaga/aiide/blob/main/docs/figures/aiide_overview.png?raw=true">
+  <img alt="AIIDE Overview" src="https://github.com/Anilturaga/aiide/blob/main/docs/figures/aiide_overview.png?raw=true" width=500">
+</picture></div>
+<br/>
+ENV states are made available to the LLM in the following way:
+<div align="center"><picture>
+  <source media="(prefers-color-scheme: dark)" srcset="docs/figures/aiide_memory_logic.png">
+  <img alt="AIIDE Memory updates" src="https://github.com/Anilturaga/aiide/blob/main/docs/figures/aiide_memory_logic.png?raw=true" width=700">
 </picture></div>
 <br/>
 
 ### Tutorial
 Let's build a simple form filling agent. We have a pandas dataframe with field names and we want the LLM to ask the user for answers to a couple of questions at a time and populate the said dataframe.
 
 Here
 * The environment is the dataframe
 * We need a single tool that enables the LLM to add or edit values for any of the fields
 * _The library will automatically provide the latest snapshot of the dataframe to the LLM.(aiide will automatically remove older snapshots of the dataframe from the LLM memory to avoid confusing it and saving tokens)_
 
 0. Install the package<br/>
-`pip install aiide`
+```bash
+pip install aiide
+```
 
 1. Let's start with defining a simple chat agent
 
 ```python
 # Import the AIIDE class
 from aiide import AIIDE
 # Import helper classes for defining functions for the LLM
@@ -88,20 +101,24 @@
                 ]
             )
         
         # Main function of the tool is called when the tool is invoked by the agent
         def main(self, field_name,value):
             # let's set the value in the master dataframe
             self.parent.df.loc[self.parent.df['Field'] == field_name, 'Value'] = value
+            # Update the ENV
+            self.parent.ENV[0] = self.parent.df.to_markdown(index=False)
             # response to the agent
             return "Added value '"+str(value) + " to Field '"+field_name+"'"
 
 ```
 > `TOOL_DEF` is a helper proxy for the JSON-SCHEMA of OpenAI function calling. You can directly add the json or even use your own pydantic model's `model_json()`. `TOOL_DEF` and associated `tools.*` would make the code less verbose and have the advantage of intellisense.
 
+Checkout <br/>**[aiide's tool use tutorial](https://github.com/Anilturaga/aiide/blob/main/docs/tool_definitions.md)**
+
 3. That's it. We can now start using the agent
 
 `chat` is the function you invoke to start streaming agent response
 ```python
 # create the agent instance
 agent = FormFillingAgent()
 while True:
@@ -142,14 +159,16 @@
 
         def main(self, field_name,value):
             if self.user_consent == False:
                 return "User has rejected the insert, please try again"
 
             # let's set the value in the master dataframe
             self.parent.df.loc[self.parent.df['Field'] == field_name, 'Value'] = value
+            # Update the ENV
+            self.parent.ENV[0] = self.parent.df.to_markdown(index=False)
             # response to the agent
             return "Added value '"+str(value) + " to Field '"+field_name+"'"
 
 agent = FormFillingAgent()
 while True:
     user_query = input("User: ")
     for each in agent.chat(user_query, tools=["add_or_modify_form_values"]):
@@ -168,20 +187,7 @@
             print("TOOL RESPONSE",each["tool_response"])
 
 ```
 
 5. Bonus!
 You can use completions and stop sequences in the `chat` function's arguments to implement prompting techniques such as ReAct, CoT etc!
 
-
-
-
-
-
-
-
-
-
-
-
-
-
```

