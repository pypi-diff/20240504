# Comparing `tmp/SimplerLLM-0.2.0.tar.gz` & `tmp/simplerllm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimplerLLM-0.2.0.tar", last modified: Sat Apr 13 10:55:59 2024, max compression
+gzip compressed data, was "simplerllm-0.2.1.tar", last modified: Sat May  4 19:39:55 2024, max compression
```

## Comparing `SimplerLLM-0.2.0.tar` & `simplerllm-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.821885 SimplerLLM-0.2.0/
--rw-rw-rw-   0        0        0     6134 2024-04-13 10:55:59.820885 SimplerLLM-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.792885 SimplerLLM-0.2.0/SimplerLLM/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.799885 SimplerLLM-0.2.0/SimplerLLM/image/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/image/__init__.py
--rw-rw-rw-   0        0        0     1194 2024-03-20 13:27:59.000000 SimplerLLM-0.2.0/SimplerLLM/image/img_helper_funcs.py
--rw-rw-rw-   0        0        0     1996 2024-03-20 13:14:02.000000 SimplerLLM-0.2.0/SimplerLLM/image/stability_ai.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.804885 SimplerLLM-0.2.0/SimplerLLM/language/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/language/__init__.py
--rw-rw-rw-   0        0        0     8767 2024-04-13 08:48:06.000000 SimplerLLM-0.2.0/SimplerLLM/language/embeddings.py
--rw-rw-rw-   0        0        0     6422 2024-04-13 08:35:22.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm.py
--rw-rw-rw-   0        0        0     2607 2024-03-25 13:07:09.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_addons.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.809885 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     5361 2024-04-13 08:36:07.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/anthropic_llm.py
--rw-rw-rw-   0        0        0     8566 2024-04-13 08:35:54.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/gemini_llm.py
--rw-rw-rw-   0        0        0      184 2024-03-29 14:59:41.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/llm_response_models.py
--rw-rw-rw-   0        0        0     6581 2024-04-13 08:40:58.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/openai_llm.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.811885 SimplerLLM-0.2.0/SimplerLLM/prompts/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/prompts/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/prompts/prompt_builder.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.819885 SimplerLLM-0.2.0/SimplerLLM/tools/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/tools/__init__.py
--rw-rw-rw-   0        0        0      915 2024-03-19 15:25:28.000000 SimplerLLM-0.2.0/SimplerLLM/tools/file_loader.py
--rw-rw-rw-   0        0        0     6006 2024-03-19 15:25:27.000000 SimplerLLM-0.2.0/SimplerLLM/tools/generic_loader.py
--rw-rw-rw-   0        0        0     5414 2024-04-12 17:40:03.000000 SimplerLLM-0.2.0/SimplerLLM/tools/json_helpers.py
--rw-rw-rw-   0        0        0     4988 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/tools/rapid_api.py
--rw-rw-rw-   0        0        0     7138 2024-03-26 11:09:21.000000 SimplerLLM-0.2.0/SimplerLLM/tools/serp.py
--rw-rw-rw-   0        0        0     8646 2024-04-13 08:48:36.000000 SimplerLLM-0.2.0/SimplerLLM/tools/text_chunker.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.796885 SimplerLLM-0.2.0/SimplerLLM.egg-info/
--rw-rw-rw-   0        0        0     6134 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      982 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.820885 SimplerLLM-0.2.0/my_tests/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/my_tests/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-13 10:55:59.821885 SimplerLLM-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1371 2024-04-13 08:21:31.000000 SimplerLLM-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.042584 simplerllm-0.2.1/
+-rw-rw-rw-   0        0        0     6963 2024-05-04 19:39:55.040074 simplerllm-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:54.977519 simplerllm-0.2.1/SimplerLLM/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/image/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/image/__init__.py
+-rw-rw-rw-   0        0        0     1227 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/image/img_helper_funcs.py
+-rw-rw-rw-   0        0        0     2080 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/image/stability_ai.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/language/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/__init__.py
+-rw-rw-rw-   0        0        0     1851 2024-05-04 14:03:11.000000 simplerllm-0.2.1/SimplerLLM/language/embeddings.py
+-rw-rw-rw-   0        0        0     6422 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm.py
+-rw-rw-rw-   0        0        0     2922 2024-05-01 19:46:15.000000 simplerllm-0.2.1/SimplerLLM/language/llm_addons.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/language/llm_providers/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     5361 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/anthropic_llm.py
+-rw-rw-rw-   0        0        0     8566 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/gemini_llm.py
+-rw-rw-rw-   0        0        0      341 2024-05-01 19:22:49.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/llm_response_models.py
+-rw-rw-rw-   0        0        0     7871 2024-05-04 14:03:09.000000 simplerllm-0.2.1/SimplerLLM/language/llm_providers/openai_llm.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.024354 simplerllm-0.2.1/SimplerLLM/prompts/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3132 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/prompts/prompt_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.040074 simplerllm-0.2.1/SimplerLLM/tools/
+-rw-rw-rw-   0        0        0        0 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/file_loader.py
+-rw-rw-rw-   0        0        0     6006 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/generic_loader.py
+-rw-rw-rw-   0        0        0     6064 2024-05-01 19:40:59.000000 simplerllm-0.2.1/SimplerLLM/tools/json_helpers.py
+-rw-rw-rw-   0        0        0     4988 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/rapid_api.py
+-rw-rw-rw-   0        0        0     7138 2024-04-16 12:35:00.000000 simplerllm-0.2.1/SimplerLLM/tools/serp.py
+-rw-rw-rw-   0        0        0     8693 2024-05-04 19:16:42.000000 simplerllm-0.2.1/SimplerLLM/tools/text_chunker.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:39:55.040074 simplerllm-0.2.1/SimplerLLM.egg-info/
+-rw-rw-rw-   0        0        0     6963 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 19:39:54.000000 simplerllm-0.2.1/SimplerLLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:39:55.042584 simplerllm-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1473 2024-05-04 13:44:30.000000 simplerllm-0.2.1/setup.py
```

### Comparing `SimplerLLM-0.2.0/PKG-INFO` & `simplerllm-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 Metadata-Version: 2.1
 Name: SimplerLLM
-Version: 0.2.0
+Version: 0.2.1
 Summary: An easy-to-use Library for interacting with language models.
 Home-page: https://github.com/hassancs91/SimplerLLM
 Author: Hasan Aboul Hasan
 Author-email: hasan@learnwithhasan.com
 Keywords: text generation,openai,LLM,RAG
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp==3.9.4
+Requires-Dist: duckduckgo_search==5.3.0
+Requires-Dist: newspaper3k==0.2.8
+Requires-Dist: numpy==1.26.4
+Requires-Dist: openai==1.25.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: PyPDF2==3.0.1
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: python_docx==1.1.0
+Requires-Dist: pytube==15.0.0
+Requires-Dist: Requests==2.31.0
+Requires-Dist: youtube_transcript_api==0.6.2
 
 # ⚪ SimplerLLM (Beta)
 
 ⚡ Your Easy Pass to Advanced AI ⚡
 
+
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Join the Discord chat!](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/HUrtZXyp3j)
+
+
+
 
 ## 🤔 What is SimplerLLM?
 
 SimplerLLM is an open-source Python library designed to simplify interactions with Large Language Models (LLMs) for researchers and beginners. It offers a unified interface for different LLM providers and a suite of tools to enhance language model capabilities and make it Super easy for anyone to develop AI-powered tools and apps.
 
 ## Easy Installation
 
@@ -167,14 +186,18 @@
 
 This function splits the text into chunks based on sentences.
 
 ### chunk_by_paragraphs
 
 This function splits text into chunks based on paragraphs.
 
+### chunk_by_semantics
+
+This functions splits text into chunks based on semantics.
+
 Example
 
 ```python
 from SimplerLLM.tools import text_chunker as chunker
 
 blog_url = "https://www.semrush.com/blog/digital-marketing/"
 blog_post = loader.load_content(blog_url)
@@ -193,7 +216,11 @@
 - Interacting With Local LLMs
 - Prompt Optimization
 - Response Evaluation
 - GPT Trainer
 - Document Chunker
 - Advanced Document Loader
 - Integration With More Providers
+- Simple RAG With SimplerVectors
+- Integration with Vector Databases
+- Agent Builder
+- LLM Server
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/image/img_helper_funcs.py` & `simplerllm-0.2.1/SimplerLLM/image/img_helper_funcs.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import base64
-import os
-
-
-def save_image_from_base64(
-    base64_str: str, file_path: str = None, image_type: str = "png"
-):
-    """
-    Saves an image from a base64 encoded string to a file.
-    If file_path is not provided, the image is saved in the current working directory.
-
-    :param base64_str: The base64 encoded string of the image.
-    :param file_path: The path (including file name) where the image will be saved.
-                      If None, saves in the current working directory with a default name.
-    :param image_type: The image type/format (e.g., 'png', 'jpg'). Default is 'png'.
-    """
-    # Decode the base64 string
-    image_data = base64.b64decode(base64_str)
-
-    # Set the default file path if not provided
-    if file_path is None:
-        file_path = os.path.join(os.getcwd(), f"default_image.{image_type}")
-
-    # Ensure the directory exists
-    os.makedirs(os.path.dirname(file_path), exist_ok=True)
-
-    # Append the file extension if not present
-    if not file_path.lower().endswith(f".{image_type.lower()}"):
-        file_path += f".{image_type}"
-
-    # Write the image data to a file
-    with open(file_path, "wb") as file:
-        file.write(image_data)
+import base64
+import os
+
+
+def save_image_from_base64(
+    base64_str: str, file_path: str = None, image_type: str = "png"
+):
+    """
+    Saves an image from a base64 encoded string to a file.
+    If file_path is not provided, the image is saved in the current working directory.
+
+    :param base64_str: The base64 encoded string of the image.
+    :param file_path: The path (including file name) where the image will be saved.
+                      If None, saves in the current working directory with a default name.
+    :param image_type: The image type/format (e.g., 'png', 'jpg'). Default is 'png'.
+    """
+    # Decode the base64 string
+    image_data = base64.b64decode(base64_str)
+
+    # Set the default file path if not provided
+    if file_path is None:
+        file_path = os.path.join(os.getcwd(), f"default_image.{image_type}")
+
+    # Ensure the directory exists
+    os.makedirs(os.path.dirname(file_path), exist_ok=True)
+
+    # Append the file extension if not present
+    if not file_path.lower().endswith(f".{image_type.lower()}"):
+        file_path += f".{image_type}"
+
+    # Write the image data to a file
+    with open(file_path, "wb") as file:
+        file.write(image_data)
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/image/stability_ai.py` & `simplerllm-0.2.1/SimplerLLM/image/stability_ai.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from pydantic import BaseModel
-import base64
-import requests
-from typing import List
-import os
-import requests
-from dotenv import load_dotenv
-
-# Load environment variables
-load_dotenv()
-
-# Constants
-STABILITY_API_KEY = os.getenv("STABILITY_API_KEY")
-
-
-class ImageData(BaseModel):
-    base64_str: str
-    size_kb: float
-    width: int
-    height: int
-
-
-class ImageList(BaseModel):
-    images: List[ImageData]
-
-
-def generate_images(
-    model_name: str,
-    prompt: str,
-    negative_prompt: str = "",
-    width: int = 512,
-    height: int = 512,
-    samples: int = 1,
-    steps: int = 30,
-    cfg_scale: int = 7,
-    seed: int = 0,
-    style_preset: str = None,
-) -> ImageList:
-
-    engine_id = model_name
-    api_host = "https://api.stability.ai"
-    api_key = STABILITY_API_KEY
-
-    if api_key is None:
-        raise Exception("Missing Stability API key.")
-
-    response = requests.post(
-        f"{api_host}/v1/generation/{engine_id}/text-to-image",
-        headers={
-            "Content-Type": "application/json",
-            "Accept": "application/json",
-            "Authorization": f"Bearer {api_key}",
-        },
-        json={
-            "text_prompts": [{"text": prompt}],
-            "negative_prompt": negative_prompt,
-            "cfg_scale": cfg_scale,
-            "height": height,
-            "width": width,
-            "samples": samples,
-            "steps": steps,
-            "seed": seed,
-            "style_preset": style_preset,
-        },
-    )
-
-    if response.status_code != 200:
-        raise Exception("Non-200 response: " + str(response.text))
-
-    data = response.json()
-
-    images_data = []
-    for image in data["artifacts"]:
-        base64_str = image["base64"]
-        decoded_image = base64.b64decode(base64_str)
-        size_kb = len(decoded_image) / 1024
-
-        images_data.append(
-            ImageData(
-                base64_str=base64_str, size_kb=size_kb, width=width, height=height
-            )
-        )
-
-    return ImageList(images=images_data)
+from pydantic import BaseModel
+import base64
+import requests
+from typing import List
+import os
+import requests
+from dotenv import load_dotenv
+
+# Load environment variables
+load_dotenv()
+
+# Constants
+STABILITY_API_KEY = os.getenv("STABILITY_API_KEY")
+
+
+class ImageData(BaseModel):
+    base64_str: str
+    size_kb: float
+    width: int
+    height: int
+
+
+class ImageList(BaseModel):
+    images: List[ImageData]
+
+
+def generate_images(
+    model_name: str,
+    prompt: str,
+    negative_prompt: str = "",
+    width: int = 512,
+    height: int = 512,
+    samples: int = 1,
+    steps: int = 30,
+    cfg_scale: int = 7,
+    seed: int = 0,
+    style_preset: str = None,
+) -> ImageList:
+
+    engine_id = model_name
+    api_host = "https://api.stability.ai"
+    api_key = STABILITY_API_KEY
+
+    if api_key is None:
+        raise Exception("Missing Stability API key.")
+
+    response = requests.post(
+        f"{api_host}/v1/generation/{engine_id}/text-to-image",
+        headers={
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+            "Authorization": f"Bearer {api_key}",
+        },
+        json={
+            "text_prompts": [{"text": prompt}],
+            "negative_prompt": negative_prompt,
+            "cfg_scale": cfg_scale,
+            "height": height,
+            "width": width,
+            "samples": samples,
+            "steps": steps,
+            "seed": seed,
+            "style_preset": style_preset,
+        },
+    )
+
+    if response.status_code != 200:
+        raise Exception("Non-200 response: " + str(response.text))
+
+    data = response.json()
+
+    images_data = []
+    for image in data["artifacts"]:
+        base64_str = image["base64"]
+        decoded_image = base64.b64decode(base64_str)
+        size_kb = len(decoded_image) / 1024
+
+        images_data.append(
+            ImageData(
+                base64_str=base64_str, size_kb=size_kb, width=width, height=height
+            )
+        )
+
+    return ImageList(images=images_data)
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/language/llm.py` & `simplerllm-0.2.1/SimplerLLM/language/llm.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/language/llm_addons.py` & `simplerllm-0.2.1/SimplerLLM/language/llm_addons.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,33 +13,41 @@
 
 def generate_basic_pydantic_json_model(
     model_class: Type[BaseModel],
     prompt: str,
     llm_instance: LLM,
     max_retries: int = 3,
     initial_delay: float = 1.0,
+    custom_prompt_suffix: str = None,
 ) -> BaseModel:
     """
     Generates a model instance based on a given prompt, retrying on validation errors.
 
     :param model_class: The Pydantic model class to be used for validation and conversion.
     :param prompt: The fully formatted prompt including the topic.
     :param llm_instance: Instance of a large language model.
     :param max_retries: Maximum number of retries on validation errors.
     :param initial_delay: Initial delay in seconds before the first retry.
+    :param custom_prompt_suffix: Optional string to customize or override the generated prompt extension.
+
     :return: Tuple containing either (model instance, None) or (None, error message).
     """
     for attempt in range(max_retries + 1):
         try:
             json_model = generate_json_example_from_pydantic(model_class)
-            optimized_prompt = (
-                prompt
-                + f"\n\n.The response should me a structured JSON format that matches the following JSON: {json_model}"
-            )
-            ai_response = llm_instance.generate_text(optimized_prompt)
+
+            if custom_prompt_suffix is not None:
+                optimized_prompt = custom_prompt_suffix
+            else:
+                optimized_prompt = (
+                    prompt
+                    + f"\n\nThe response should be in a structured JSON format that matches the following JSON: {json_model}"
+                )
+        
+            ai_response = llm_instance.generate_response(prompt=optimized_prompt)
 
             if ai_response:
                 json_object = extract_json_from_text(ai_response)
 
                 validated, errors = validate_json_with_pydantic_model(
                     model_class, json_object
                 )
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/anthropic_llm.py` & `simplerllm-0.2.1/SimplerLLM/language/llm_providers/anthropic_llm.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/gemini_llm.py` & `simplerllm-0.2.1/SimplerLLM/language/llm_providers/gemini_llm.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/openai_llm.py` & `simplerllm-0.2.1/SimplerLLM/language/llm_providers/openai_llm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # add streaming
 from openai import AsyncOpenAI
 from openai import OpenAI
 from dotenv import load_dotenv
 import asyncio
 import os
 import time
-from .llm_response_models import LLMFullResponse
+from .llm_response_models import LLMFullResponse,LLMEmbeddingsResponse
 
 # Load environment variables
 load_dotenv()
 
 # Constants
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY", "")
 MAX_RETRIES = int(os.getenv("MAX_RETRIES", 3))
@@ -147,53 +147,89 @@
                 print(error_msg)
                 return None
 
 
 def generate_embeddings(
     model_name,
     user_input=None,
+    full_response = False
 ):
-
+    
     if not user_input:
         raise ValueError("user_input must be provided.")
+    
+    start_time = time.time() if full_response else None
+    for attempt in range(MAX_RETRIES):
+        try:
+            
+            response = openai_client.embeddings.create(
+                model= model_name,
+                input=user_input
+            )
+            generate_embeddings = response.data
+
+            if full_response:
+                end_time = time.time()
+                process_time = end_time - start_time
+                return LLMEmbeddingsResponse(
+                    generated_embedding=generate_embeddings,
+                    model=model_name,
+                    process_time=process_time,
+                    llm_provider_response=response,
+                )
+            return generate_embeddings
+
+        except Exception as e:
+            if attempt < MAX_RETRIES - 1:
+                time.sleep(RETRY_DELAY * (2**attempt))
+            else:
+                error_msg = f"Failed after {MAX_RETRIES} attempts"
+                if full_response:
+                    end_time = time.time()
+                    process_time = end_time - start_time
+                    error_msg += f" and {process_time} seconds"
+                error_msg += f" due to: {e}"
+                print(error_msg)
+                return None
 
-    # Prepare messages based on input type
-    if prompt:
-        messages = [
-            {"role": "system", "content": system_prompt},
-            {"role": "user", "content": prompt},
-        ]
 
+async def generate_embeddings_async(
+    model_name,
+    user_input=None,
+    full_response = False
+):
+    
+    if not user_input:
+        raise ValueError("user_input must be provided.")
+    
+    start_time = time.time() if full_response else None
     for attempt in range(MAX_RETRIES):
         try:
-            completion = openai_client.chat.completions.create(
+            result = await async_openai_client.embeddings.create(
                 model=model_name,
-                messages=messages,
-                temperature=temperature,
-                max_tokens=max_tokens,
-                top_p=top_p,
+                input=user_input,
             )
-            generated_text = completion.choices[0].message.content
+            generate_embeddings = result.data
 
             if full_response:
                 end_time = time.time()
                 process_time = end_time - start_time
-                return LLMFullResponse(
-                    generated_text=generated_text,
+                return LLMEmbeddingsResponse(
+                    generated_embedding=generate_embeddings,
                     model=model_name,
                     process_time=process_time,
-                    llm_provider_response=completion,
+                    llm_provider_response=result,
                 )
-            return generated_text
+            return generate_embeddings
 
         except Exception as e:
             if attempt < MAX_RETRIES - 1:
-                time.sleep(RETRY_DELAY * (2**attempt))
+                await asyncio.sleep(RETRY_DELAY * (2**attempt))
             else:
                 error_msg = f"Failed after {MAX_RETRIES} attempts"
                 if full_response:
                     end_time = time.time()
                     process_time = end_time - start_time
                     error_msg += f" and {process_time} seconds"
                 error_msg += f" due to: {e}"
                 print(error_msg)
-                return None
+                return None
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/prompts/prompt_builder.py` & `simplerllm-0.2.1/SimplerLLM/prompts/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/tools/file_loader.py` & `simplerllm-0.2.1/SimplerLLM/tools/file_loader.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import csv
-import os
-from pydantic import BaseModel
-from typing import Optional, List
-
-
-class CSVDocument(BaseModel):
-    file_size: Optional[int] = None
-    row_count: int
-    column_count: int
-    total_fields: int
-    content: List[List[str]]  # This represents the CSV data as a list of rows
-    title: Optional[str] = None
-    url_or_path: Optional[str] = None
-
-
-def read_csv_file(file_path: str) -> CSVDocument:
-    with open(file_path, "r", encoding="utf-8") as file:
-        reader = csv.reader(file)
-        rows = list(reader)
-
-    file_size = os.path.getsize(file_path)
-    row_count = len(rows)
-    column_count = len(rows[0]) if rows else 0
-    total_fields = sum(len(row) for row in rows)
-
-    return CSVDocument(
-        file_size=file_size,
-        row_count=row_count,
-        column_count=column_count,
-        total_fields=total_fields,
-        content=rows,
-        url_or_path=file_path,
-    )
+import csv
+import os
+from pydantic import BaseModel
+from typing import Optional, List
+
+
+class CSVDocument(BaseModel):
+    file_size: Optional[int] = None
+    row_count: int
+    column_count: int
+    total_fields: int
+    content: List[List[str]]  # This represents the CSV data as a list of rows
+    title: Optional[str] = None
+    url_or_path: Optional[str] = None
+
+
+def read_csv_file(file_path: str) -> CSVDocument:
+    with open(file_path, "r", encoding="utf-8") as file:
+        reader = csv.reader(file)
+        rows = list(reader)
+
+    file_size = os.path.getsize(file_path)
+    row_count = len(rows)
+    column_count = len(rows[0]) if rows else 0
+    total_fields = sum(len(row) for row in rows)
+
+    return CSVDocument(
+        file_size=file_size,
+        row_count=row_count,
+        column_count=column_count,
+        total_fields=total_fields,
+        content=rows,
+        url_or_path=file_path,
+    )
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/tools/generic_loader.py` & `simplerllm-0.2.1/SimplerLLM/tools/generic_loader.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/tools/json_helpers.py` & `simplerllm-0.2.1/SimplerLLM/tools/json_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import json
 from pydantic import BaseModel, ValidationError
 from typing import get_type_hints
 from pydantic import BaseModel
-from typing import List, get_type_hints, Type
+from typing import Type, get_type_hints, List, get_origin, get_args
+
 
 
 def convert_pydantic_to_json(model_instance):
     """
     Converts a Pydantic model instance to a JSON string.
 
     Args:
@@ -15,16 +16,18 @@
 
     Returns:
         str: A JSON string representation of the model.
     """
     return model_instance.model_dump_json()
 
 
+    
+
 def extract_json_from_text(text_response):
-    pattern = r"\{.*?\}"
+    pattern = r'\{.*?\}'
     matches = re.finditer(pattern, text_response, re.DOTALL)
     json_objects = []
 
     for match in matches:
         json_str = __json_extend_search(text_response, match.span())
         try:
             json_obj = json.loads(json_str)
@@ -35,21 +38,21 @@
     return json_objects if json_objects else None
 
 
 def __json_extend_search(text, span):
     start, end = span
     nest_count = 1  # Starts with 1 since we know '{' is at the start position
     for i in range(end, len(text)):
-        if text[i] == "{":
+        if text[i] == '{':
             nest_count += 1
-        elif text[i] == "}":
+        elif text[i] == '}':
             nest_count -= 1
             if nest_count == 0:
-                return text[start : i + 1]
-    return text[start:end]
+                return text[start:i+1]
+    return text[start:end] 
 
 
 @DeprecationWarning
 def __extract_json_from_text_deprecated(text_response):
     # This pattern matches a string that starts with '{' and ends with '}'
     pattern = r"\{[^{}]*\}"
 
@@ -135,31 +138,39 @@
     except ValidationError as e:
         print("Validation error:", e)
         return None
 
 
 # Define a function to provide example values based on type
 def example_value_for_type(field_type: Type):
-    if field_type == str:
-        return "example_string"
-    elif field_type == int:
-        return 0
-    elif field_type == float:
-        return 0.0
-    elif field_type == bool:
-        return True
-    elif field_type == List[str]:
-        return ["generated text 1", "generated text 2"]
-    elif field_type == List[int]:
-        return [1, 2, 3]
-    else:
-        return "Unsupported type"
-
+    origin = get_origin(field_type)
+    if origin is None:  # Not a generic type
+        if issubclass(field_type, BaseModel):  # Check if it's a custom Pydantic model
+            # Generate an example using all fields of the model
+            example_data = {field_name: example_value_for_type(field_type)
+                            for field_name, field_type in get_type_hints(field_type).items()}
+            return field_type(**example_data)
+        elif field_type == str:
+            return "example_string"
+        elif field_type == int:
+            return 0
+        elif field_type == float:
+            return 0.0
+        elif field_type == bool:
+            return True
+        else:
+            return "Unsupported type"
+    elif origin == list:  # It's a List
+        args = get_args(field_type)
+        if not args:
+            return []  # No type specified for elements, return empty list
+        element_type = args[0]
+        # Create a list with 3 elements of the specified type
+        return [example_value_for_type(element_type) for _ in range(3)]
 
-# Function to generate a JSON example for any Pydantic model
 def generate_json_example_from_pydantic(model_class: Type[BaseModel]) -> str:
     example_data = {}
     for field_name, field_type in get_type_hints(model_class).items():
         example_data[field_name] = example_value_for_type(field_type)
 
     model_instance = model_class(**example_data)
-    return model_instance.json()
+    return model_instance.json()
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM/tools/rapid_api.py` & `simplerllm-0.2.1/SimplerLLM/tools/rapid_api.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/tools/serp.py` & `simplerllm-0.2.1/SimplerLLM/tools/serp.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.2.0/SimplerLLM/tools/text_chunker.py` & `simplerllm-0.2.1/SimplerLLM/tools/text_chunker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,228 +1,224 @@
-from pydantic import BaseModel, Field
-from typing import List
-import re
-
-import openai
-import numpy as np
-
-# from sklearn.metrics.pairwise import cosine_similarity
-
-
-class ChunkInfo(BaseModel):
-    text: str
-    num_characters: int = Field(description="Number of characters in the chunk")
-    num_words: int = Field(description="Number of words in the chunk")
-
-
-class TextChunks(BaseModel):
-    num_chunks: int = Field(description="Total number of chunks")
-    chunks: List[ChunkInfo]
-
-
-def chunk_by_max_chunk_size(
-    text: str, max_chunk_size: int, preserve_sentence_structure: bool = False
-) -> TextChunks:
-    """
-    Split the given text into chunks based on the maximum chunk size trying to reserve sentence endings if preserve_sentence_structure is enabled
-
-    Parameters:
-    - text (str): The input text to be split into chunks.
-    - max_chunk_size (int): The maximum size of each chunk.
-    - preserve_sentence_structure: Whether to consider preserving the sentence structure when splitting the text.
-
-    Returns:
-    - TextChunks: An object containing the total number of chunks and a list of ChunkInfo objects.
-    - num_chunks (int): The total number of chunks.
-    - chunks (List[ChunkInfo]): A list of ChunkInfo objects, each representing a chunk of the text.
-        - chunk (str): The chunk of text.
-        - num_characters (int): The number of characters in the chunk.
-        - num_words (int): The number of words in the chunk.
-    """
-
-    if preserve_sentence_structure:
-        sentences = re.split(r"(?<=[.!?]) +", text)
-    else:
-        sentences = [
-            text[i : i + max_chunk_size] for i in range(0, len(text), max_chunk_size)
-        ]
-
-    chunks = []
-    current_chunk = ""
-
-    for sentence in sentences:
-        if preserve_sentence_structure:
-            if len(current_chunk) + len(sentence) <= max_chunk_size:
-                current_chunk += " " + sentence if current_chunk else sentence
-            else:
-                if current_chunk:
-                    chunks.append(current_chunk)
-                    current_chunk = sentence
-                else:
-                    # If the current chunk is empty and the sentence is longer than the max size,
-                    # accept this sentence as a single chunk even if it exceeds the max size.
-                    chunks.append(sentence)
-                    sentence = ""
-        else:
-            chunks.append(sentence)
-
-    if current_chunk.strip():
-        chunks.append(current_chunk.strip())
-
-    chunk_infos = [
-        ChunkInfo(text=chunk, num_characters=len(chunk), num_words=len(chunk.split()))
-        for chunk in chunks
-    ]
-
-    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
-
-
-def chunk_by_sentences(text: str) -> TextChunks:
-    # Regular expression for splitting by sentence
-    sentences = re.split(r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|\!)\s", text)
-
-    chunk_infos = []
-    for sentence in sentences:
-        sentence = sentence.strip()
-        if sentence:  # This condition filters out empty or whitespace-only sentences
-            chunk_info = ChunkInfo(
-                text=sentence,
-                num_characters=len(sentence),
-                num_words=len(sentence.split()),
-            )
-            chunk_infos.append(chunk_info)
-
-    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
-
-
-def chunk_by_paragraphs(text: str) -> TextChunks:
-    # Splitting the text into paragraphs
-    paragraphs = re.split(r"(?<=\n)(?=[A-Z0-9])", text)
-
-    chunk_infos = [
-        ChunkInfo(
-            text=paragraph.strip(),
-            num_characters=len(paragraph.strip()),
-            num_words=len(paragraph.strip().split()),
-        )
-        for paragraph in paragraphs
-        if paragraph.strip()  # This condition filters out empty or whitespace-only paragraphs
-    ]
-
-    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
-
-
-# def chunk_by_semantics(text: str, threshold_percentage=95) -> TextChunks:
-
-#     # Split the input text into individual sentences.
-#     single_sentences_list = _split_sentences(text)
-
-#     # Combine adjacent sentences to form a context window around each sentence.
-#     combined_sentences = _combine_sentences(single_sentences_list)
-
-#     # Convert the combined sentences into vector representations using a neural network model.
-#     embeddings = convert_to_vector(combined_sentences)
-
-#     # Calculate the cosine distances between consecutive combined sentence embeddings to measure similarity.
-#     distances = _calculate_cosine_distances(embeddings)
-
-#     # Determine the threshold distance for identifying breakpoints based on the 80th percentile of all distances.
-#     breakpoint_percentile_threshold = threshold_percentage
-#     breakpoint_distance_threshold = np.percentile(
-#         distances, breakpoint_percentile_threshold
-#     )
-
-#     # Find all indices where the distance exceeds the calculated threshold, indicating a potential chunk breakpoint.
-#     indices_above_thresh = [
-#         i
-#         for i, distance in enumerate(distances)
-#         if distance > breakpoint_distance_threshold
-#     ]
-
-#     # Initialize the list of chunks and a variable to track the start of the next chunk.
-#     chunks = []
-#     start_index = 0
-
-#     # Loop through the identified breakpoints and create chunks accordingly.
-#     for index in indices_above_thresh:
-#         chunk = " ".join(single_sentences_list[start_index : index + 1])
-#         chunks.append(chunk)
-#         start_index = index + 1
-
-#     # If there are any sentences left after the last breakpoint, add them as the final chunk.
-#     if start_index < len(single_sentences_list):
-#         chunk = " ".join(single_sentences_list[start_index:])
-#         chunks.append(chunk)
-
-#     chunk_infos = [
-#         ChunkInfo(
-#             text=chunk.strip(),
-#             num_characters=len(chunk.strip()),
-#             num_words=len(chunk.strip().split()),
-#         )
-#         for chunk in chunks
-#         if chunk.strip()  # This condition filters out empty or whitespace-only paragraphs
-#     ]
-
-#     # Return the list of text chunks.
-#     return TextChunks(num_chunks=len(chunks), chunks=chunk_infos)
-
-
-# def _split_sentences(text):
-#     # Use regular expressions to split the text into sentences based on punctuation followed by whitespace.
-#     sentences = re.split(r"(?<=[.?!])\s+", text)
-#     return sentences
-
-
-# def _combine_sentences(sentences):
-#     # Create a buffer by combining each sentence with its previous and next sentence to provide a wider context.
-#     combined_sentences = []
-#     for i in range(len(sentences)):
-#         combined_sentence = sentences[i]
-#         if i > 0:
-#             combined_sentence = sentences[i - 1] + " " + combined_sentence
-#         if i < len(sentences) - 1:
-#             combined_sentence += " " + sentences[i + 1]
-#         combined_sentences.append(combined_sentence)
-#     return combined_sentences
-
-
-# def convert_to_vector(texts):
-#     # Try to generate embeddings for a list of texts using a pre-trained model and handle any exceptions.
-#     try:
-#         response = openai.embeddings.create(input=texts, model="text-embedding-3-small")
-#         embeddings = np.array([item.embedding for item in response.data])
-#         return embeddings
-#     except Exception as e:
-#         print("An error occurred:", e)
-#         return np.array([])  # Return an empty array in case of an error
-
-
-# def calculate_cosine_similarities_manual(embeddings):
-#     # Manually calculate the cosine similarities between consecutive embeddings.
-#     similarities = []
-#     for i in range(len(embeddings) - 1):
-#         vec1 = embeddings[i].flatten()
-#         vec2 = embeddings[i + 1].flatten()
-#         dot_product = np.dot(vec1, vec2)
-#         norm_vec1 = np.linalg.norm(vec1)
-#         norm_vec2 = np.linalg.norm(vec2)
-
-#         if norm_vec1 == 0 or norm_vec2 == 0:
-#             # If either vector is zero, similarity is undefined (could also return 0)
-#             similarity = float("nan")
-#         else:
-#             similarity = dot_product / (norm_vec1 * norm_vec2)
-#         similarities.append(similarity)
-#     return similarities
-
-
-# def _calculate_cosine_distances(embeddings):
-#     # Calculate the cosine distance (1 - cosine similarity) between consecutive embeddings.
-#     distances = []
-#     for i in range(len(embeddings) - 1):
-#         similarity = calculate_cosine_similarities_manual(
-#             [embeddings[i]], [embeddings[i + 1]]
-#         )[0][0]
-#         distance = 1 - similarity
-#         distances.append(distance)
-#     return distances
+from pydantic import BaseModel, Field
+from typing import List
+import re
+
+import openai
+import numpy as np
+
+from SimplerLLM.language.llm import LLM as llm_genetation_instance
+from SimplerLLM.language.embeddings import LLM as llm_embeddings_instance
+
+# from sklearn.metrics.pairwise import cosine_similarity
+
+
+class ChunkInfo(BaseModel):
+    text: str
+    num_characters: int = Field(description="Number of characters in the chunk")
+    num_words: int = Field(description="Number of words in the chunk")
+
+
+class TextChunks(BaseModel):
+    num_chunks: int = Field(description="Total number of chunks")
+    chunks: List[ChunkInfo]
+
+
+def chunk_by_max_chunk_size(
+    text: str, max_chunk_size: int, preserve_sentence_structure: bool = False
+) -> TextChunks:
+    """
+    Split the given text into chunks based on the maximum chunk size trying to reserve sentence endings if preserve_sentence_structure is enabled
+
+    Parameters:
+    - text (str): The input text to be split into chunks.
+    - max_chunk_size (int): The maximum size of each chunk.
+    - preserve_sentence_structure: Whether to consider preserving the sentence structure when splitting the text.
+
+    Returns:
+    - TextChunks: An object containing the total number of chunks and a list of ChunkInfo objects.
+    - num_chunks (int): The total number of chunks.
+    - chunks (List[ChunkInfo]): A list of ChunkInfo objects, each representing a chunk of the text.
+        - chunk (str): The chunk of text.
+        - num_characters (int): The number of characters in the chunk.
+        - num_words (int): The number of words in the chunk.
+    """
+
+    if preserve_sentence_structure:
+        sentences = re.split(r"(?<=[.!?]) +", text)
+    else:
+        sentences = [
+            text[i : i + max_chunk_size] for i in range(0, len(text), max_chunk_size)
+        ]
+
+    chunks = []
+    current_chunk = ""
+
+    for sentence in sentences:
+        if preserve_sentence_structure:
+            if len(current_chunk) + len(sentence) <= max_chunk_size:
+                current_chunk += " " + sentence if current_chunk else sentence
+            else:
+                if current_chunk:
+                    chunks.append(current_chunk)
+                    current_chunk = sentence
+                else:
+                    # If the current chunk is empty and the sentence is longer than the max size,
+                    # accept this sentence as a single chunk even if it exceeds the max size.
+                    chunks.append(sentence)
+                    sentence = ""
+        else:
+            chunks.append(sentence)
+
+    if current_chunk.strip():
+        chunks.append(current_chunk.strip())
+
+    chunk_infos = [
+        ChunkInfo(text=chunk, num_characters=len(chunk), num_words=len(chunk.split()))
+        for chunk in chunks
+    ]
+
+    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
+
+
+def chunk_by_sentences(text: str) -> TextChunks:
+    # Regular expression for splitting by sentence
+    sentences = re.split(r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|\!)\s", text)
+
+    chunk_infos = []
+    for sentence in sentences:
+        sentence = sentence.strip()
+        if sentence:  # This condition filters out empty or whitespace-only sentences
+            chunk_info = ChunkInfo(
+                text=sentence,
+                num_characters=len(sentence),
+                num_words=len(sentence.split()),
+            )
+            chunk_infos.append(chunk_info)
+
+    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
+
+
+def chunk_by_paragraphs(text: str) -> TextChunks:
+    # Splitting the text into paragraphs
+    paragraphs = re.split(r"(?<=\n)(?=[A-Z0-9])", text)
+
+    chunk_infos = [
+        ChunkInfo(
+            text=paragraph.strip(),
+            num_characters=len(paragraph.strip()),
+            num_words=len(paragraph.strip().split()),
+        )
+        for paragraph in paragraphs
+        if paragraph.strip()  # This condition filters out empty or whitespace-only paragraphs
+    ]
+
+    return TextChunks(num_chunks=len(chunk_infos), chunks=chunk_infos)
+
+
+def chunk_by_semantics(text: str,  llm_embeddings_instance: llm_embeddings_instance, threshold_percentage=90) -> TextChunks:
+
+    # Split the input text into individual sentences.
+    single_sentences_list = __split_sentences(text)
+
+    # Combine adjacent sentences to form a context window around each sentence.
+    combined_sentences = __combine_sentences(single_sentences_list)
+
+    # Convert the combined sentences into vector representations using a neural network model.
+    embeddings = __convert_to_vector(combined_sentences,llm_embeddings_instance=llm_embeddings_instance)
+
+    # Calculate the cosine distances between consecutive combined sentence embeddings to measure similarity.
+    distances = __calculate_cosine_similarities(embeddings)
+
+    # Determine the threshold distance for identifying breakpoints based on the 80th percentile of all distances.
+    breakpoint_percentile_threshold = threshold_percentage
+    breakpoint_distance_threshold = np.percentile(
+        distances, breakpoint_percentile_threshold
+    )
+
+    # Find all indices where the distance exceeds the calculated threshold, indicating a potential chunk breakpoint.
+    indices_above_thresh = [
+        i
+        for i, distance in enumerate(distances)
+        if distance > breakpoint_distance_threshold
+    ]
+
+    # Initialize the list of chunks and a variable to track the start of the next chunk.
+    chunks = []
+    start_index = 0
+
+    # Loop through the identified breakpoints and create chunks accordingly.
+    for index in indices_above_thresh:
+        chunk = " ".join(single_sentences_list[start_index : index + 1])
+        chunks.append(chunk)
+        start_index = index + 1
+
+    # If there are any sentences left after the last breakpoint, add them as the final chunk.
+    if start_index < len(single_sentences_list):
+        chunk = " ".join(single_sentences_list[start_index:])
+        chunks.append(chunk)
+
+    chunk_infos = [
+        ChunkInfo(
+            text=chunk.strip(),
+            num_characters=len(chunk.strip()),
+            num_words=len(chunk.strip().split()),
+        )
+        for chunk in chunks
+        if chunk.strip()  # This condition filters out empty or whitespace-only paragraphs
+    ]
+
+    # Return the list of text chunks.
+    return TextChunks(num_chunks=len(chunks), chunks=chunk_infos)
+
+
+
+
+def __split_sentences(text):
+    # Use regular expressions to split the text into sentences based on punctuation followed by whitespace.
+    sentences = re.split(r"(?<=[.?!])\s+", text)
+    return sentences
+
+
+
+
+def __combine_sentences(sentences):
+    # Create a buffer by combining each sentence with its previous and next sentence to provide a wider context.
+    combined_sentences = []
+    for i in range(len(sentences)):
+        combined_sentence = sentences[i]
+        if i > 0:
+            combined_sentence = sentences[i - 1] + " " + combined_sentence
+        if i < len(sentences) - 1:
+            combined_sentence += " " + sentences[i + 1]
+        combined_sentences.append(combined_sentence)
+    return combined_sentences
+
+def __convert_to_vector(combined_sentences_list, llm_embeddings_instance: llm_embeddings_instance):
+    # Try to generate embeddings for a list of texts using a pre-trained model and handle any exceptions.
+    try:
+        response = llm_embeddings_instance.generate_embeddings(combined_sentences_list)
+        #response = openai.embeddings.create(input=combined_sentences_list, model="text-embedding-3-small")
+        embeddings = np.array([item.embedding for item in response])
+        return embeddings
+    except Exception as e:
+        print("An error occurred:", e)
+        return np.array([])  # Return an empty array in case of an error
+
+def __calculate_cosine_similarities(embeddings):
+    # Manually calculate the cosine similarities between consecutive embeddings.
+    similarities = []
+    for i in range(len(embeddings) - 1):
+        vec1 = embeddings[i].flatten()
+        vec2 = embeddings[i + 1].flatten()
+        dot_product = np.dot(vec1, vec2)
+        norm_vec1 = np.linalg.norm(vec1)
+        norm_vec2 = np.linalg.norm(vec2)
+
+        if norm_vec1 == 0 or norm_vec2 == 0:
+            # If either vector is zero, similarity is undefined (could also return 0)
+            similarity = float("nan")
+        else:
+            similarity = dot_product / (norm_vec1 * norm_vec2)
+        similarities.append(similarity)
+    return similarities
+
+
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM.egg-info/PKG-INFO` & `simplerllm-0.2.1/SimplerLLM.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 Metadata-Version: 2.1
 Name: SimplerLLM
-Version: 0.2.0
+Version: 0.2.1
 Summary: An easy-to-use Library for interacting with language models.
 Home-page: https://github.com/hassancs91/SimplerLLM
 Author: Hasan Aboul Hasan
 Author-email: hasan@learnwithhasan.com
 Keywords: text generation,openai,LLM,RAG
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp==3.9.4
+Requires-Dist: duckduckgo_search==5.3.0
+Requires-Dist: newspaper3k==0.2.8
+Requires-Dist: numpy==1.26.4
+Requires-Dist: openai==1.25.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: PyPDF2==3.0.1
+Requires-Dist: python-dotenv==1.0.1
+Requires-Dist: python_docx==1.1.0
+Requires-Dist: pytube==15.0.0
+Requires-Dist: Requests==2.31.0
+Requires-Dist: youtube_transcript_api==0.6.2
 
 # ⚪ SimplerLLM (Beta)
 
 ⚡ Your Easy Pass to Advanced AI ⚡
 
+
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Join the Discord chat!](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/HUrtZXyp3j)
+
+
+
 
 ## 🤔 What is SimplerLLM?
 
 SimplerLLM is an open-source Python library designed to simplify interactions with Large Language Models (LLMs) for researchers and beginners. It offers a unified interface for different LLM providers and a suite of tools to enhance language model capabilities and make it Super easy for anyone to develop AI-powered tools and apps.
 
 ## Easy Installation
 
@@ -167,14 +186,18 @@
 
 This function splits the text into chunks based on sentences.
 
 ### chunk_by_paragraphs
 
 This function splits text into chunks based on paragraphs.
 
+### chunk_by_semantics
+
+This functions splits text into chunks based on semantics.
+
 Example
 
 ```python
 from SimplerLLM.tools import text_chunker as chunker
 
 blog_url = "https://www.semrush.com/blog/digital-marketing/"
 blog_post = loader.load_content(blog_url)
@@ -193,7 +216,11 @@
 - Interacting With Local LLMs
 - Prompt Optimization
 - Response Evaluation
 - GPT Trainer
 - Document Chunker
 - Advanced Document Loader
 - Integration With More Providers
+- Simple RAG With SimplerVectors
+- Integration with Vector Databases
+- Agent Builder
+- LLM Server
```

### Comparing `SimplerLLM-0.2.0/SimplerLLM.egg-info/SOURCES.txt` & `simplerllm-0.2.1/SimplerLLM.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 SimplerLLM/prompts/prompt_builder.py
 SimplerLLM/tools/__init__.py
 SimplerLLM/tools/file_loader.py
 SimplerLLM/tools/generic_loader.py
 SimplerLLM/tools/json_helpers.py
 SimplerLLM/tools/rapid_api.py
 SimplerLLM/tools/serp.py
-SimplerLLM/tools/text_chunker.py
-my_tests/__init__.py
+SimplerLLM/tools/text_chunker.py
```

### Comparing `SimplerLLM-0.2.0/setup.py` & `simplerllm-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the long description from the README file
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SimplerLLM",
-    version="0.2.0",
+    version="0.2.1",
     author="Hasan Aboul Hasan",
     author_email="hasan@learnwithhasan.com",
     description="An easy-to-use Library for interacting with language models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hassancs91/SimplerLLM",
     packages=find_packages(),
@@ -27,11 +27,13 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     # Add additional fields as necessary
 )
```

