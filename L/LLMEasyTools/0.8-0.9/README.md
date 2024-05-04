# Comparing `tmp/LLMEasyTools-0.8.tar.gz` & `tmp/LLMEasyTools-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLMEasyTools-0.8.tar", last modified: Mon Apr 22 20:23:00 2024, max compression
+gzip compressed data, was "LLMEasyTools-0.9.tar", last modified: Mon Apr 22 20:39:31 2024, max compression
```

## Comparing `LLMEasyTools-0.8.tar` & `LLMEasyTools-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:23:00.447450 LLMEasyTools-0.8/
--rw-rw-r--   0 zby       (1000) zby       (1000)    11357 2024-03-03 11:08:50.000000 LLMEasyTools-0.8/LICENSE
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:23:00.447450 LLMEasyTools-0.8/LLMEasyTools.egg-info/
--rw-r--r--   0 zby       (1000) zby       (1000)    16954 2024-04-22 20:23:00.000000 LLMEasyTools-0.8/LLMEasyTools.egg-info/PKG-INFO
--rw-rw-r--   0 zby       (1000) zby       (1000)      454 2024-04-22 20:23:00.000000 LLMEasyTools-0.8/LLMEasyTools.egg-info/SOURCES.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)        1 2024-04-22 20:23:00.000000 LLMEasyTools-0.8/LLMEasyTools.egg-info/dependency_links.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-04-22 20:23:00.000000 LLMEasyTools-0.8/LLMEasyTools.egg-info/requires.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       15 2024-04-22 20:23:00.000000 LLMEasyTools-0.8/LLMEasyTools.egg-info/top_level.txt
--rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-03-03 11:08:50.000000 LLMEasyTools-0.8/MANIFEST.in
--rw-r--r--   0 zby       (1000) zby       (1000)    16954 2024-04-22 20:23:00.447450 LLMEasyTools-0.8/PKG-INFO
--rw-rw-r--   0 zby       (1000) zby       (1000)     3153 2024-04-21 17:27:50.000000 LLMEasyTools-0.8/README.md
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:23:00.443450 LLMEasyTools-0.8/examples/
--rw-rw-r--   0 zby       (1000) zby       (1000)     1336 2024-04-20 07:38:54.000000 LLMEasyTools-0.8/examples/extract_user_details.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     3331 2024-04-20 07:38:54.000000 LLMEasyTools-0.8/examples/stateful_search.py
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:23:00.447450 LLMEasyTools-0.8/llm_easy_tools/
--rw-rw-r--   0 zby       (1000) zby       (1000)      120 2024-04-20 09:54:59.000000 LLMEasyTools-0.8/llm_easy_tools/__init__.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     4822 2024-04-20 07:38:54.000000 LLMEasyTools-0.8/llm_easy_tools/schema_generator.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     9860 2024-04-22 20:18:09.000000 LLMEasyTools-0.8/llm_easy_tools/tool_box.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     1098 2024-04-22 20:21:34.000000 LLMEasyTools-0.8/pyproject.toml
--rw-rw-r--   0 zby       (1000) zby       (1000)       38 2024-04-22 20:23:00.447450 LLMEasyTools-0.8/setup.cfg
-drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:23:00.447450 LLMEasyTools-0.8/tests/
--rw-rw-r--   0 zby       (1000) zby       (1000)      737 2024-04-20 07:38:54.000000 LLMEasyTools-0.8/tests/message_construction.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     4982 2024-04-20 07:38:54.000000 LLMEasyTools-0.8/tests/schema_generator_test.py
--rw-rw-r--   0 zby       (1000) zby       (1000)     8018 2024-04-21 20:56:56.000000 LLMEasyTools-0.8/tests/tools_test.py
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:39:31.921335 LLMEasyTools-0.9/
+-rw-rw-r--   0 zby       (1000) zby       (1000)    11357 2024-03-03 11:08:50.000000 LLMEasyTools-0.9/LICENSE
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:39:31.917335 LLMEasyTools-0.9/LLMEasyTools.egg-info/
+-rw-r--r--   0 zby       (1000) zby       (1000)    16954 2024-04-22 20:39:31.000000 LLMEasyTools-0.9/LLMEasyTools.egg-info/PKG-INFO
+-rw-rw-r--   0 zby       (1000) zby       (1000)      454 2024-04-22 20:39:31.000000 LLMEasyTools-0.9/LLMEasyTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)        1 2024-04-22 20:39:31.000000 LLMEasyTools-0.9/LLMEasyTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-04-22 20:39:31.000000 LLMEasyTools-0.9/LLMEasyTools.egg-info/requires.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       15 2024-04-22 20:39:31.000000 LLMEasyTools-0.9/LLMEasyTools.egg-info/top_level.txt
+-rw-rw-r--   0 zby       (1000) zby       (1000)       67 2024-03-03 11:08:50.000000 LLMEasyTools-0.9/MANIFEST.in
+-rw-r--r--   0 zby       (1000) zby       (1000)    16954 2024-04-22 20:39:31.917335 LLMEasyTools-0.9/PKG-INFO
+-rw-rw-r--   0 zby       (1000) zby       (1000)     3153 2024-04-21 17:27:50.000000 LLMEasyTools-0.9/README.md
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:39:31.917335 LLMEasyTools-0.9/examples/
+-rw-rw-r--   0 zby       (1000) zby       (1000)     1336 2024-04-20 07:38:54.000000 LLMEasyTools-0.9/examples/extract_user_details.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     3331 2024-04-20 07:38:54.000000 LLMEasyTools-0.9/examples/stateful_search.py
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:39:31.917335 LLMEasyTools-0.9/llm_easy_tools/
+-rw-rw-r--   0 zby       (1000) zby       (1000)      120 2024-04-20 09:54:59.000000 LLMEasyTools-0.9/llm_easy_tools/__init__.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     4822 2024-04-20 07:38:54.000000 LLMEasyTools-0.9/llm_easy_tools/schema_generator.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     9851 2024-04-22 20:30:10.000000 LLMEasyTools-0.9/llm_easy_tools/tool_box.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     1098 2024-04-22 20:37:12.000000 LLMEasyTools-0.9/pyproject.toml
+-rw-rw-r--   0 zby       (1000) zby       (1000)       38 2024-04-22 20:39:31.921335 LLMEasyTools-0.9/setup.cfg
+drwxrwxr-x   0 zby       (1000) zby       (1000)        0 2024-04-22 20:39:31.917335 LLMEasyTools-0.9/tests/
+-rw-rw-r--   0 zby       (1000) zby       (1000)      737 2024-04-20 07:38:54.000000 LLMEasyTools-0.9/tests/message_construction.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     4982 2024-04-20 07:38:54.000000 LLMEasyTools-0.9/tests/schema_generator_test.py
+-rw-rw-r--   0 zby       (1000) zby       (1000)     8232 2024-04-22 20:37:46.000000 LLMEasyTools-0.9/tests/tools_test.py
```

### Comparing `LLMEasyTools-0.8/LICENSE` & `LLMEasyTools-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/LLMEasyTools.egg-info/PKG-INFO` & `LLMEasyTools-0.9/LLMEasyTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMEasyTools
-Version: 0.8
+Version: 0.9
 Summary: OpenAI tools and functions with no fuss.
 Author: Natalia Borovskikh
 Author-email: Zbigniew Łukasiak <zzbbyy@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `LLMEasyTools-0.8/PKG-INFO` & `LLMEasyTools-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMEasyTools
-Version: 0.8
+Version: 0.9
 Summary: OpenAI tools and functions with no fuss.
 Author: Natalia Borovskikh
 Author-email: Zbigniew Łukasiak <zzbbyy@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `LLMEasyTools-0.8/README.md` & `LLMEasyTools-0.9/README.md`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/examples/extract_user_details.py` & `LLMEasyTools-0.9/examples/extract_user_details.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/examples/stateful_search.py` & `LLMEasyTools-0.9/examples/stateful_search.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/llm_easy_tools/schema_generator.py` & `LLMEasyTools-0.9/llm_easy_tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/llm_easy_tools/tool_box.py` & `LLMEasyTools-0.9/llm_easy_tools/tool_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     def to_message(self):
         if self.output is not None:
             content = self.output
         elif self.model is not None:
             content = f"{self.name} created"
         elif self.error is not None:
             content = f"{self.error}"
-        return ChatCompletionMessage(
-            role="tool",
-            tool_call_id=self.tool_call_id,
-            name=self.name,
-            content=content,
-        )
+        return {
+            "role": "tool",
+            "tool_call_id": self.tool_call_id,
+            "name": self.name,
+            "content": content,
+        }
 
 class ToolBox:
     def __init__(self,
                  fix_json_args: bool = True,
                  case_insensitive: bool = False,
                  insert_prefix_name: bool = True,
                  ):
```

### Comparing `LLMEasyTools-0.8/pyproject.toml` & `LLMEasyTools-0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LLMEasyTools"
-version = "0.08"
+version = "0.09"
 authors = [{ name = "Zbigniew Łukasiak", email = "zzbbyy@gmail.com" }, { name = "Natalia Borovskikh" }]
 description = "OpenAI tools and functions with no fuss."
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `LLMEasyTools-0.8/tests/message_construction.py` & `LLMEasyTools-0.9/tests/message_construction.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/tests/schema_generator_test.py` & `LLMEasyTools-0.9/tests/schema_generator_test.py`

 * *Files identical despite different names*

### Comparing `LLMEasyTools-0.8/tests/tools_test.py` & `LLMEasyTools-0.9/tests/tools_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,19 @@
     toolbox = ToolBox()
     toolbox.register_model(UserDetail)
     original_user = UserDetail(name="John", age=21)
     response = mk_chat_with_tool_call("UserDetail", original_user.model_dump())
     results = toolbox.process_response(response)
     assert len(results) == 1
     assert results[0].model == original_user
+    message = results[0].to_message()
+    assert message['role'] == 'tool'
+    assert message['tool_call_id'] == 'A'
+    assert message['name'] == 'UserDetail'
+    assert message['content'] == 'UserDetail created'
 
 
 # Define the test cases
 def test_register_tool():
     class Tool(BaseModel):
         name: str
```

