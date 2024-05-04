# Comparing `tmp/scrapegraphai-0.8.0.tar.gz` & `tmp/scrapegraphai-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.8.0.tar", max compression
+gzip compressed data, was "scrapegraphai-0.8.0b1.tar", max compression
```

## Comparing `scrapegraphai-0.8.0.tar` & `scrapegraphai-0.8.0b1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1065 2024-05-03 20:26:37.021079 scrapegraphai-0.8.0/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-03 20:26:37.021079 scrapegraphai-0.8.0/README.md
--rw-r--r--   0        0        0     1736 2024-05-03 20:26:55.849120 scrapegraphai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      449 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    10586 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3594 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3738 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1959 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      342 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      463 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      736 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6987 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6431 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6987 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6987 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     6639 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4303 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-03 20:26:37.049079 scrapegraphai-0.8.0/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1605 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-03 20:26:37.053079 scrapegraphai-0.8.0/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12084 1970-01-01 00:00:00.000000 scrapegraphai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-03 20:26:06.320970 scrapegraphai-0.8.0b1/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-03 20:26:06.320970 scrapegraphai-0.8.0b1/README.md
+-rw-r--r--   0        0        0     1738 2024-05-03 20:26:31.453039 scrapegraphai-0.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      449 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    10586 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3594 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3880 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3650 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3749 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4575 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1959 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      342 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-03 20:26:06.348970 scrapegraphai-0.8.0b1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      463 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      736 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7932 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3716 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6431 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6987 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     6639 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4303 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5605 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3707 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6261 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1605 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-03 20:26:06.352970 scrapegraphai-0.8.0b1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12086 1970-01-01 00:00:00.000000 scrapegraphai-0.8.0b1/PKG-INFO
```

### Comparing `scrapegraphai-0.8.0/LICENSE` & `scrapegraphai-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/README.md` & `scrapegraphai-0.8.0b1/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/pyproject.toml` & `scrapegraphai-0.8.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.8.0"
+version = "0.8.0b1"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.8.0/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.8.0b1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.8.0b1/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.8.0b1/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.8.0b1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.8.0b1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.8.0b1/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.8.0b1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.8.0b1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.8.0b1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/remover.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.8.0b1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.8.0/PKG-INFO` & `scrapegraphai-0.8.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.8.0
+Version: 0.8.0b1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

