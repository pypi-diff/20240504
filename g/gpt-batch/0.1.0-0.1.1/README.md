# Comparing `tmp/gpt_batch-0.1.0.tar.gz` & `tmp/gpt_batch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_batch-0.1.0.tar", last modified: Sat May  4 06:12:35 2024, max compression
+gzip compressed data, was "gpt_batch-0.1.1.tar", last modified: Sat May  4 06:47:53 2024, max compression
```

## Comparing `gpt_batch-0.1.0.tar` & `gpt_batch-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 06:12:35.508986 gpt_batch-0.1.0/
--rw-rw-rw-   0        0        0      707 2024-05-04 06:12:35.507981 gpt_batch-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-05-04 05:08:42.000000 gpt_batch-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 06:12:35.490212 gpt_batch-0.1.0/gpt_batch/
--rw-rw-rw-   0        0        0       61 2024-05-04 05:29:30.000000 gpt_batch-0.1.0/gpt_batch/__init__.py
--rw-rw-rw-   0        0        0     3720 2024-05-04 05:41:12.000000 gpt_batch-0.1.0/gpt_batch/batcher.py
-drwxrwxrwx   0        0        0        0 2024-05-04 06:12:35.503474 gpt_batch-0.1.0/gpt_batch.egg-info/
--rw-rw-rw-   0        0        0      707 2024-05-04 06:12:35.000000 gpt_batch-0.1.0/gpt_batch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-04 06:12:35.000000 gpt_batch-0.1.0/gpt_batch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 06:12:35.000000 gpt_batch-0.1.0/gpt_batch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-04 06:12:35.000000 gpt_batch-0.1.0/gpt_batch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-04 06:12:35.000000 gpt_batch-0.1.0/gpt_batch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 06:12:35.508986 gpt_batch-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      473 2024-05-04 06:12:12.000000 gpt_batch-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 06:12:35.506470 gpt_batch-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-04 05:06:20.000000 gpt_batch-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1117 2024-05-04 05:40:48.000000 gpt_batch-0.1.0/tests/test_batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:53.689670 gpt_batch-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-04 06:47:53.689670 gpt_batch-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 06:47:45.000000 gpt_batch-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:53.685670 gpt_batch-0.1.1/gpt_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-04 06:47:45.000000 gpt_batch-0.1.1/gpt_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-04 06:47:45.000000 gpt_batch-0.1.1/gpt_batch/batcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:53.685670 gpt_batch-0.1.1/gpt_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-04 06:47:53.000000 gpt_batch-0.1.1/gpt_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 06:47:53.000000 gpt_batch-0.1.1/gpt_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:47:53.000000 gpt_batch-0.1.1/gpt_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 06:47:53.000000 gpt_batch-0.1.1/gpt_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 06:47:53.000000 gpt_batch-0.1.1/gpt_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:47:53.689670 gpt_batch-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-04 06:47:45.000000 gpt_batch-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:53.689670 gpt_batch-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 06:47:45.000000 gpt_batch-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-04 06:47:45.000000 gpt_batch-0.1.1/tests/test_batcher.py
```

### Comparing `gpt_batch-0.1.0/PKG-INFO` & `gpt_batch-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1
-Name: gpt_batch
-Version: 0.1.0
-Summary: A package for batch processing with OpenAI API.
-Home-page: https://github.com/fengsxy/gpt_batch
-Author: Ted Yu
-Author-email: liddlerain@gmail.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: tqdm
-
-# GPT Batcher
-
-A simple tool to batch process messages using OpenAI's GPT models.
-
-## Installation
-
-Clone this repository and run:
-
-## Usage
-
-Here's how to use the `GPTBatcher`:
-
-```python
-from gpt_batch.batcher import GPTBatcher
-
-batcher = GPTBatcher(key='your_key_here', model_name='gpt-3.5-turbo-1106')
-result = batcher.handle_list(['your', 'list', 'of', 'messages'])
-print(result)
-
+Metadata-Version: 2.1
+Name: gpt_batch
+Version: 0.1.1
+Summary: A package for batch processing with OpenAI API.
+Home-page: https://github.com/fengsxy/gpt_batch
+Author: Ted Yu
+Author-email: liddlerain@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+# GPT Batcher
+
+A simple tool to batch process messages using OpenAI's GPT models.
+
+## Installation
+
+Clone this repository and run:
+
+## Usage
+
+Here's how to use the `GPTBatcher`:
+
+```python
+from gpt_batch.batcher import GPTBatcher
+
+batcher = GPTBatcher(api_key='your_key_here', model_name='gpt-3.5-turbo-1106')
+result = batcher.handle_message_list(['your', 'list', 'of', 'messages'])
+print(result)
+
+
+
```

### Comparing `gpt_batch-0.1.0/gpt_batch/batcher.py` & `gpt_batch-0.1.1/gpt_batch/batcher.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from openai import OpenAI
-from concurrent.futures import ThreadPoolExecutor, wait
-from functools import partial
-from tqdm import tqdm
-
-class GPTBatcher:
-    def __init__(self, api_key, model_name="gpt-3.5-turbo-0125", system_prompt="",temperature=1,num_workers=64,timeout_duration=60,retry_attempts=2):
-        self.client = OpenAI(api_key=api_key)
-        self.model_name = model_name
-        self.system_prompt = system_prompt
-        self.temperature = temperature
-        self.num_workers = num_workers
-        self.timeout_duration = timeout_duration
-        self.retry_attempts = retry_attempts
-        self.miss_index =[]
-
-    def get_attitude(self, ask_text):
-        index, ask_text = ask_text
-
-        completion = self.client.chat.completions.create(
-            model=self.model_name,
-            messages=[
-                {"role": "system", "content": self.system_prompt},
-                {"role": "user", "content": ask_text}
-            ],
-            temperature=self.temperature,
-        )
-        return (index, completion.choices[0].message.content)
-
-    def process_attitude(self, message_list):
-        new_list = []
-        num_workers = self.num_workers
-        timeout_duration = self.timeout_duration
-        retry_attempts=2
-
-        executor = ThreadPoolExecutor(max_workers=num_workers)
-        message_chunks = list(self.chunk_list(message_list, num_workers))
-        for chunk in tqdm(message_chunks, desc="Processing messages"):
-            future_to_message =  {executor.submit(self.get_attitude, message): message for message in chunk}
-            for _ in range(retry_attempts):
-                done, not_done = wait(future_to_message.keys(), timeout=timeout_duration)
-                for future in not_done:
-                    future.cancel()
-                new_list.extend(future.result() for future in done if future.done())
-                if len(not_done) == 0:
-                    break
-                future_to_message = {executor.submit(self.get_attitude, (future_to_message[future], msg), temperature): future_to_message[future] for future, msg in not_done}
-        executor.shutdown(wait=False)
-        return new_list
-
-    def complete_attitude_list(self,attitude_list, max_length):
-        completed_list = []
-        current_index = 0
-        for item in attitude_list:
-            index, value = item
-            # Fill in missing indices
-            while current_index < index:
-                completed_list.append((current_index, None))
-                current_index += 1
-            # Add the current element from the list
-            completed_list.append(item)
-            current_index = index + 1
-        while current_index < max_length:
-            print("Filling in missing index", current_index)
-            self.miss_index.append(current_index)
-            completed_list.append((current_index, None))
-            current_index += 1
-        return completed_list
-
-    def chunk_list(self, lst, n):
-        """Yield successive n-sized chunks from lst."""
-        for i in range(0, len(lst), n):
-            yield lst[i:i + n]
-
-    def handle_message_list(self,message_list):
-        indexed_list = [(index, data) for index, data in enumerate(message_list)]
-        max_length = len(indexed_list)
-        attitude_list = self.process_attitude(indexed_list)
-        attitude_list.sort(key=lambda x: x[0])
-        attitude_list = self.complete_attitude_list(attitude_list, max_length)
-        attitude_list = [x[1] for x in attitude_list]
-        return attitude_list
-
-    # Add other necessary methods similar to the above, refactored to fit within this class structure.
-
+from openai import OpenAI
+from concurrent.futures import ThreadPoolExecutor, wait
+from functools import partial
+from tqdm import tqdm
+
+class GPTBatcher:
+    def __init__(self, api_key, model_name="gpt-3.5-turbo-0125", system_prompt="",temperature=1,num_workers=64,timeout_duration=60,retry_attempts=2):
+        self.client = OpenAI(api_key=api_key)
+        self.model_name = model_name
+        self.system_prompt = system_prompt
+        self.temperature = temperature
+        self.num_workers = num_workers
+        self.timeout_duration = timeout_duration
+        self.retry_attempts = retry_attempts
+        self.miss_index =[]
+
+    def get_attitude(self, ask_text):
+        index, ask_text = ask_text
+
+        completion = self.client.chat.completions.create(
+            model=self.model_name,
+            messages=[
+                {"role": "system", "content": self.system_prompt},
+                {"role": "user", "content": ask_text}
+            ],
+            temperature=self.temperature,
+        )
+        return (index, completion.choices[0].message.content)
+
+    def process_attitude(self, message_list):
+        new_list = []
+        num_workers = self.num_workers
+        timeout_duration = self.timeout_duration
+        retry_attempts=2
+
+        executor = ThreadPoolExecutor(max_workers=num_workers)
+        message_chunks = list(self.chunk_list(message_list, num_workers))
+        for chunk in tqdm(message_chunks, desc="Processing messages"):
+            future_to_message =  {executor.submit(self.get_attitude, message): message for message in chunk}
+            for _ in range(retry_attempts):
+                done, not_done = wait(future_to_message.keys(), timeout=timeout_duration)
+                for future in not_done:
+                    future.cancel()
+                new_list.extend(future.result() for future in done if future.done())
+                if len(not_done) == 0:
+                    break
+                future_to_message = {executor.submit(self.get_attitude, (future_to_message[future], msg), temperature): future_to_message[future] for future, msg in not_done}
+        executor.shutdown(wait=False)
+        return new_list
+
+    def complete_attitude_list(self,attitude_list, max_length):
+        completed_list = []
+        current_index = 0
+        for item in attitude_list:
+            index, value = item
+            # Fill in missing indices
+            while current_index < index:
+                completed_list.append((current_index, None))
+                current_index += 1
+            # Add the current element from the list
+            completed_list.append(item)
+            current_index = index + 1
+        while current_index < max_length:
+            print("Filling in missing index", current_index)
+            self.miss_index.append(current_index)
+            completed_list.append((current_index, None))
+            current_index += 1
+        return completed_list
+
+    def chunk_list(self, lst, n):
+        """Yield successive n-sized chunks from lst."""
+        for i in range(0, len(lst), n):
+            yield lst[i:i + n]
+
+    def handle_message_list(self,message_list):
+        indexed_list = [(index, data) for index, data in enumerate(message_list)]
+        max_length = len(indexed_list)
+        attitude_list = self.process_attitude(indexed_list)
+        attitude_list.sort(key=lambda x: x[0])
+        attitude_list = self.complete_attitude_list(attitude_list, max_length)
+        attitude_list = [x[1] for x in attitude_list]
+        return attitude_list
+
+    # Add other necessary methods similar to the above, refactored to fit within this class structure.
+
```

### Comparing `gpt_batch-0.1.0/gpt_batch.egg-info/PKG-INFO` & `gpt_batch-0.1.1/gpt_batch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1
-Name: gpt-batch
-Version: 0.1.0
-Summary: A package for batch processing with OpenAI API.
-Home-page: https://github.com/fengsxy/gpt_batch
-Author: Ted Yu
-Author-email: liddlerain@gmail.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: tqdm
-
-# GPT Batcher
-
-A simple tool to batch process messages using OpenAI's GPT models.
-
-## Installation
-
-Clone this repository and run:
-
-## Usage
-
-Here's how to use the `GPTBatcher`:
-
-```python
-from gpt_batch.batcher import GPTBatcher
-
-batcher = GPTBatcher(key='your_key_here', model_name='gpt-3.5-turbo-1106')
-result = batcher.handle_list(['your', 'list', 'of', 'messages'])
-print(result)
-
+Metadata-Version: 2.1
+Name: gpt-batch
+Version: 0.1.1
+Summary: A package for batch processing with OpenAI API.
+Home-page: https://github.com/fengsxy/gpt_batch
+Author: Ted Yu
+Author-email: liddlerain@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+# GPT Batcher
+
+A simple tool to batch process messages using OpenAI's GPT models.
+
+## Installation
+
+Clone this repository and run:
+
+## Usage
+
+Here's how to use the `GPTBatcher`:
+
+```python
+from gpt_batch.batcher import GPTBatcher
+
+batcher = GPTBatcher(api_key='your_key_here', model_name='gpt-3.5-turbo-1106')
+result = batcher.handle_message_list(['your', 'list', 'of', 'messages'])
+print(result)
+
+
+
```

### Comparing `gpt_batch-0.1.0/tests/test_batcher.py` & `gpt_batch-0.1.1/tests/test_batcher.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pytest
-from gpt_batch import GPTBatcher
-import os
-
-def test_handle_message_list():
-    # Initialize the GPTBatcher with hypothetical valid credentials
-    #api_key = #get from system environment
-    api_key = os.getenv('TEST_KEY')
-    if not api_key:
-        raise ValueError("API key must be set in the environment variables")
-    batcher = GPTBatcher(api_key=api_key, model_name='gpt-3.5-turbo-1106', system_prompt="Your task is to discuss privacy questions and provide persuasive answers with supporting reasons.")
-    message_list = ["I think privacy is important", "I don't think privacy is important"]
-
-    # Call the method under test
-    results = batcher.handle_message_list(message_list)
-
-    # Assertions to verify the length of the results and the structure of each item
-    assert len(results) == 2, "There should be two results, one for each message"
-    assert all(len(result) >= 2 for result in results), "Each result should be at least two elements"
-
-# Optionally, you can add a test configuration if you have specific needs
-if __name__ == "__main__":
-    pytest.main()
+import pytest
+from gpt_batch import GPTBatcher
+import os
+
+def test_handle_message_list():
+    # Initialize the GPTBatcher with hypothetical valid credentials
+    #api_key = #get from system environment
+    api_key = os.getenv('TEST_KEY')
+    if not api_key:
+        raise ValueError("API key must be set in the environment variables")
+    batcher = GPTBatcher(api_key=api_key, model_name='gpt-3.5-turbo-1106', system_prompt="Your task is to discuss privacy questions and provide persuasive answers with supporting reasons.")
+    message_list = ["I think privacy is important", "I don't think privacy is important"]
+
+    # Call the method under test
+    results = batcher.handle_message_list(message_list)
+
+    # Assertions to verify the length of the results and the structure of each item
+    assert len(results) == 2, "There should be two results, one for each message"
+    assert all(len(result) >= 2 for result in results), "Each result should be at least two elements"
+
+# Optionally, you can add a test configuration if you have specific needs
+if __name__ == "__main__":
+    pytest.main()
```

