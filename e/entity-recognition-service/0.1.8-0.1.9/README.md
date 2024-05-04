# Comparing `tmp/entity_recognition_service-0.1.8.tar.gz` & `tmp/entity_recognition_service-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity_recognition_service-0.1.8.tar", last modified: Mon Apr 22 21:07:08 2024, max compression
+gzip compressed data, was "entity_recognition_service-0.1.9.tar", last modified: Mon Apr 22 21:29:41 2024, max compression
```

## Comparing `entity_recognition_service-0.1.8.tar` & `entity_recognition_service-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:07:08.875769 entity_recognition_service-0.1.8/
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1053 2024-04-22 16:19:44.000000 entity_recognition_service-0.1.8/LICENSE
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3895 2024-04-22 21:07:08.875516 entity_recognition_service-0.1.8/PKG-INFO
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     2643 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.8/README.md
-drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:07:08.871610 entity_recognition_service-0.1.8/entity_recognition_service/
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1862 2024-04-22 20:22:39.000000 entity_recognition_service-0.1.8/entity_recognition_service/EntityRecognizer.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.8/entity_recognition_service/__init__.py
-drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:07:08.872670 entity_recognition_service-0.1.8/entity_recognition_service/data/
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)    31581 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.8/entity_recognition_service/data/tech_entities.json
-drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:07:08.873957 entity_recognition_service-0.1.8/entity_recognition_service/functions/
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.8/entity_recognition_service/functions/__init__.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     2831 2024-04-22 20:57:30.000000 entity_recognition_service-0.1.8/entity_recognition_service/functions/entity_extraction.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     5236 2024-04-22 20:22:53.000000 entity_recognition_service-0.1.8/entity_recognition_service/functions/recommendation_generation.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1271 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.8/entity_recognition_service/functions/topic_classification.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1556 2024-04-22 20:56:49.000000 entity_recognition_service-0.1.8/entity_recognition_service/models.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3089 2024-04-22 20:22:23.000000 entity_recognition_service-0.1.8/entity_recognition_service/utils.py
-drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:07:08.875016 entity_recognition_service-0.1.8/entity_recognition_service.egg-info/
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3895 2024-04-22 21:07:08.000000 entity_recognition_service-0.1.8/entity_recognition_service.egg-info/PKG-INFO
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)      806 2024-04-22 21:07:08.000000 entity_recognition_service-0.1.8/entity_recognition_service.egg-info/SOURCES.txt
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)        1 2024-04-22 21:07:08.000000 entity_recognition_service-0.1.8/entity_recognition_service.egg-info/dependency_links.txt
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)      192 2024-04-22 21:07:08.000000 entity_recognition_service-0.1.8/entity_recognition_service.egg-info/requires.txt
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)       27 2024-04-22 21:07:08.000000 entity_recognition_service-0.1.8/entity_recognition_service.egg-info/top_level.txt
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)      832 2024-04-22 14:18:07.000000 entity_recognition_service-0.1.8/pyproject.toml
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)       38 2024-04-22 21:07:08.875818 entity_recognition_service-0.1.8/setup.cfg
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1676 2024-04-22 21:06:49.000000 entity_recognition_service-0.1.8/setup.py
-drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:07:08.874505 entity_recognition_service-0.1.8/tests/
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3005 2024-04-22 19:49:24.000000 entity_recognition_service-0.1.8/tests/test_entity_extraction.py
--rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1707 2024-04-22 19:49:24.000000 entity_recognition_service-0.1.8/tests/test_recommendation_generation.py
+drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:29:41.253080 entity_recognition_service-0.1.9/
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1053 2024-04-22 16:19:44.000000 entity_recognition_service-0.1.9/LICENSE
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3895 2024-04-22 21:29:41.252780 entity_recognition_service-0.1.9/PKG-INFO
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     2643 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.9/README.md
+drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:29:41.249455 entity_recognition_service-0.1.9/entity_recognition_service/
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1817 2024-04-22 21:26:29.000000 entity_recognition_service-0.1.9/entity_recognition_service/EntityRecognizer.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)       47 2024-04-22 21:26:54.000000 entity_recognition_service-0.1.9/entity_recognition_service/__init__.py
+drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:29:41.250366 entity_recognition_service-0.1.9/entity_recognition_service/data/
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)    31581 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.9/entity_recognition_service/data/tech_entities.json
+drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:29:41.251460 entity_recognition_service-0.1.9/entity_recognition_service/functions/
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.9/entity_recognition_service/functions/__init__.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     2831 2024-04-22 20:57:30.000000 entity_recognition_service-0.1.9/entity_recognition_service/functions/entity_extraction.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     5236 2024-04-22 20:22:53.000000 entity_recognition_service-0.1.9/entity_recognition_service/functions/recommendation_generation.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1271 2024-04-22 19:48:55.000000 entity_recognition_service-0.1.9/entity_recognition_service/functions/topic_classification.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1556 2024-04-22 21:26:14.000000 entity_recognition_service-0.1.9/entity_recognition_service/models.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3265 2024-04-22 21:27:16.000000 entity_recognition_service-0.1.9/entity_recognition_service/utils.py
+drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:29:41.252233 entity_recognition_service-0.1.9/entity_recognition_service.egg-info/
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3895 2024-04-22 21:29:41.000000 entity_recognition_service-0.1.9/entity_recognition_service.egg-info/PKG-INFO
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)      806 2024-04-22 21:29:41.000000 entity_recognition_service-0.1.9/entity_recognition_service.egg-info/SOURCES.txt
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)        1 2024-04-22 21:29:41.000000 entity_recognition_service-0.1.9/entity_recognition_service.egg-info/dependency_links.txt
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)      192 2024-04-22 21:29:41.000000 entity_recognition_service-0.1.9/entity_recognition_service.egg-info/requires.txt
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)       27 2024-04-22 21:29:41.000000 entity_recognition_service-0.1.9/entity_recognition_service.egg-info/top_level.txt
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)      832 2024-04-22 14:18:07.000000 entity_recognition_service-0.1.9/pyproject.toml
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)       38 2024-04-22 21:29:41.253136 entity_recognition_service-0.1.9/setup.cfg
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1676 2024-04-22 21:29:35.000000 entity_recognition_service-0.1.9/setup.py
+drwxr-xr-x   0 cesaraugustogoncalves   (501) staff       (20)        0 2024-04-22 21:29:41.251873 entity_recognition_service-0.1.9/tests/
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     3005 2024-04-22 19:49:24.000000 entity_recognition_service-0.1.9/tests/test_entity_extraction.py
+-rw-r--r--   0 cesaraugustogoncalves   (501) staff       (20)     1707 2024-04-22 19:49:24.000000 entity_recognition_service-0.1.9/tests/test_recommendation_generation.py
```

### Comparing `entity_recognition_service-0.1.8/LICENSE` & `entity_recognition_service-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/PKG-INFO` & `entity_recognition_service-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-recognition-service
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for technology entity recognition and recommendation
 Home-page: https://github.com/cgoncalves94/entity-recognition
 Author: Cesar Goncalves
 Author-email: goncalves.cesaraugusto94@gmail.com
 License: MIT
 Keywords: entity recognition,recommendation,technology
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `entity_recognition_service-0.1.8/README.md` & `entity_recognition_service-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/EntityRecognizer.py` & `entity_recognition_service-0.1.9/entity_recognition_service/EntityRecognizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from entity_recognition_service.functions.topic_classification import classify_text
 from entity_recognition_service.models import load_bertopic_model
 from entity_recognition_service.utils import load_json_file
 
 
 class EntityRecognizer:
     def __init__(self):
-        self.tech_entities = asyncio.run(load_json_file("entity_recognition_service/data/tech_entities.json"))
+        self.tech_entities = load_json_file("tech_entities.json")
         self.matcher = initialize_matcher_with_patterns(self.tech_entities)
         self.topic_model = asyncio.run(load_bertopic_model("MaartenGr/BERTopic_Wikipedia"))
         self.topic_info = self.topic_model.get_topic_info()
         self.topic_name_mapping = dict(zip(self.topic_info["Topic"], self.topic_info["Name"]))
 
     def process_text(self, text):
         extracted_entities = extract_tech_entities(text, self.tech_entities, self.matcher)
```

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/data/tech_entities.json` & `entity_recognition_service-0.1.9/entity_recognition_service/data/tech_entities.json`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/functions/entity_extraction.py` & `entity_recognition_service-0.1.9/entity_recognition_service/functions/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/functions/recommendation_generation.py` & `entity_recognition_service-0.1.9/entity_recognition_service/functions/recommendation_generation.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/functions/topic_classification.py` & `entity_recognition_service-0.1.9/entity_recognition_service/functions/topic_classification.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/models.py` & `entity_recognition_service-0.1.9/entity_recognition_service/models.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service/utils.py` & `entity_recognition_service-0.1.9/entity_recognition_service/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import asyncio
 import json
-import os
+from importlib import resources  
 
-import aiofiles
+from requests import JSONDecodeError
 import torch
 import torch.nn.functional as F
 from scipy.spatial.distance import cosine
 
 from entity_recognition_service.models import load_embeddings_model
 
 tokenizer, model = asyncio.run(load_embeddings_model())
 
-async def load_json_file(file_path):
-    # Detailed explanation of the function's purpose
+def load_json_file(file_name):
     """
-    Load a JSON file from the given file path.
+    Load a JSON file from the installed package resources.
 
     Args:
-        file_path (str): The path to the JSON file.
+        file_name (str): The filename of the JSON file to load from the 'data' directory within the package.
 
     Returns:
         dict: The contents of the JSON file as a dictionary.
 
     Raises:
-        FileNotFoundError: If the file does not exist.
-
+        FileNotFoundError: If the file does not exist within the package resources.
     """
-    # Check if the file exists at the given path
-    if os.path.exists(file_path):
-        async with aiofiles.open(file_path, mode="r") as file:
-            # Load the JSON content from the file and return it as a dictionary
-            return json.loads(await file.read())
-    else:
-        # Raise an error if the file does not exist
-        raise FileNotFoundError(f"File not found: {file_path}")
+    package_path = 'entity_recognition_service.data'  # Define the package path to the resources
+
+    try:
+      # Open the resource file within the context manager
+      with resources.open_text(package_path, file_name) as file:
+        return json.load(file)
+    except FileNotFoundError:
+      raise FileNotFoundError(f"File not found: {file_name} in package resources.")
+    except JSONDecodeError as e:
+      raise JSONDecodeError(f"An error occurred while loading {file_name}: {str(e)}")
 
 
 def mean_pooling(model_output, attention_mask):
     """
     Apply mean pooling to get the sentence embedding
 
     Parameters:
```

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service.egg-info/PKG-INFO` & `entity_recognition_service-0.1.9/entity_recognition_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-recognition-service
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for technology entity recognition and recommendation
 Home-page: https://github.com/cgoncalves94/entity-recognition
 Author: Cesar Goncalves
 Author-email: goncalves.cesaraugusto94@gmail.com
 License: MIT
 Keywords: entity recognition,recommendation,technology
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `entity_recognition_service-0.1.8/entity_recognition_service.egg-info/SOURCES.txt` & `entity_recognition_service-0.1.9/entity_recognition_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/pyproject.toml` & `entity_recognition_service-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/setup.py` & `entity_recognition_service-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="entity-recognition-service",
     keywords="entity recognition, recommendation, technology",
     license="MIT",
-    version="0.1.8",
+    version="0.1.9",
     author="Cesar Goncalves",
     author_email="goncalves.cesaraugusto94@gmail.com",
     description="A library for technology entity recognition and recommendation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cgoncalves94/entity-recognition",
     packages=find_packages(include=['entity_recognition_service']),
```

### Comparing `entity_recognition_service-0.1.8/tests/test_entity_extraction.py` & `entity_recognition_service-0.1.9/tests/test_entity_extraction.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_service-0.1.8/tests/test_recommendation_generation.py` & `entity_recognition_service-0.1.9/tests/test_recommendation_generation.py`

 * *Files identical despite different names*

