# Comparing `tmp/webscout-1.3.9.tar.gz` & `tmp/webscout-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.3.9.tar", last modified: Fri May  3 04:56:08 2024, max compression
+gzip compressed data, was "webscout-1.4.0.tar", last modified: Fri May  3 12:07:45 2024, max compression
```

## Comparing `webscout-1.3.9.tar` & `webscout-1.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:07.630790 webscout-1.3.9/
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:05.832325 webscout-1.3.9/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:06.107872 webscout-1.3.9/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:06.339994 webscout-1.3.9/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:06.459578 webscout-1.3.9/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-26 07:30:49.000000 webscout-1.3.9/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-26 07:30:49.000000 webscout-1.3.9/LICENSE.md
--rw-rw-rw-   0        0        0    31949 2024-05-03 04:56:07.354297 webscout-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    29695 2024-05-03 03:46:18.000000 webscout-1.3.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 04:56:07.632798 webscout-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2772 2024-05-03 03:40:51.000000 webscout-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:07.103063 webscout-1.3.9/webscout/
--rw-rw-rw-   0        0        0   202197 2024-05-03 04:52:32.000000 webscout-1.3.9/webscout/AI.py
--rw-rw-rw-   0        0        0     4710 2024-05-03 04:08:13.000000 webscout-1.3.9/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33135 2024-05-03 04:26:47.000000 webscout-1.3.9/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/LLM.py
--rw-rw-rw-   0        0        0     1046 2024-05-03 03:49:13.000000 webscout-1.3.9/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/__main__.py
--rw-rw-rw-   0        0        0      939 2024-05-03 03:36:32.000000 webscout-1.3.9/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/cli.py
--rw-rw-rw-   0        0        0      378 2024-05-03 02:40:34.000000 webscout-1.3.9/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24451 2024-05-03 03:31:40.000000 webscout-1.3.9/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/models.py
--rw-rw-rw-   0        0        0    20622 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-05-03 03:38:17.000000 webscout-1.3.9/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/voice.py
--rw-rw-rw-   0        0        0    81661 2024-05-03 04:48:27.000000 webscout-1.3.9/webscout/webai.py
--rw-rw-rw-   0        0        0     3085 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-26 07:30:49.000000 webscout-1.3.9/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:56:07.333311 webscout-1.3.9/webscout.egg-info/
--rw-rw-rw-   0        0        0    31949 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-05-03 04:56:05.000000 webscout-1.3.9/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-03 04:56:03.000000 webscout-1.3.9/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:45.100725 webscout-1.4.0/
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:44.766305 webscout-1.4.0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:44.782940 webscout-1.4.0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:44.811495 webscout-1.4.0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:44.836501 webscout-1.4.0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-26 07:30:49.000000 webscout-1.4.0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-26 07:30:49.000000 webscout-1.4.0/LICENSE.md
+-rw-rw-rw-   0        0        0    32651 2024-05-03 12:07:45.091748 webscout-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    30380 2024-05-03 10:56:52.000000 webscout-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 12:07:45.101728 webscout-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2773 2024-05-03 11:14:48.000000 webscout-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:45.031223 webscout-1.4.0/webscout/
+-rw-rw-rw-   0        0        0   211764 2024-05-03 11:00:29.000000 webscout-1.4.0/webscout/AI.py
+-rw-rw-rw-   0        0        0     4710 2024-05-03 04:08:13.000000 webscout-1.4.0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33135 2024-05-03 04:26:47.000000 webscout-1.4.0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/LLM.py
+-rw-rw-rw-   0        0        0     1046 2024-05-03 03:49:13.000000 webscout-1.4.0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      939 2024-05-03 03:36:32.000000 webscout-1.4.0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/cli.py
+-rw-rw-rw-   0        0        0      378 2024-05-03 02:40:34.000000 webscout-1.4.0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24451 2024-05-03 03:31:40.000000 webscout-1.4.0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-05-03 11:13:11.000000 webscout-1.4.0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/voice.py
+-rw-rw-rw-   0        0        0    81661 2024-05-03 04:48:27.000000 webscout-1.4.0/webscout/webai.py
+-rw-rw-rw-   0        0        0     3085 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-26 07:30:49.000000 webscout-1.4.0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:07:45.084717 webscout-1.4.0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    32651 2024-05-03 12:07:43.000000 webscout-1.4.0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-05-03 12:07:44.000000 webscout-1.4.0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 12:07:43.000000 webscout-1.4.0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-03 12:07:43.000000 webscout-1.4.0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      368 2024-05-03 12:07:43.000000 webscout-1.4.0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-03 12:07:43.000000 webscout-1.4.0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.3.9/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.4.0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.4.0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/networks/filepath_converter.py` & `webscout-1.4.0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/networks/google_searcher.py` & `webscout-1.4.0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/networks/network_configs.py` & `webscout-1.4.0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.4.0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/utilsdw/enver.py` & `webscout-1.4.0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/DeepWEBS/utilsdw/logger.py` & `webscout-1.4.0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/LICENSE.md` & `webscout-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/PKG-INFO` & `webscout-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.9
+Version: 1.4.0
 Summary: Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -43,15 +43,16 @@
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
-Requires-Dist: appdirsGoogleBard1>=2.1.4
+Requires-Dist: appdirs
+Requires-Dist: GoogleBard1>=2.1.4
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 #  webscout
 <p align="center">
 
@@ -86,25 +87,25 @@
     - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
     - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
     - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
     - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
   - [usage of webscout.AI](#usage-of-webscoutai)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
-    - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
+    - [3. `You.com` - search with you.com -NOT WORKING](#3-youcom---search-with-youcom--not-working)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
-    - [`LLM`](#llm)
+    - [`LLM` --not working](#llm---not-working)
     - [`LLM` with internet](#llm-with-internet)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -548,34 +549,30 @@
 response = ph.ask(prompt)
 
 # Extract and print the message from the response
 message = ph.get_message(response)
 print(message)
 ```
 ### 2. `YepChat` - Chat with mistral 8x7b powered by yepchat
-Thanks To Divyansh Shukla for This code
 ```python
-from webscout.AI import YepChat
+from webscout.AI import YEPCHAT
 
-def main():
-    # Initialize the YepChat class with your message
-    yep_chat = YepChat(message="who is pm of india")
-    
-    # Send the request and process the response
-    response = yep_chat.send_request()
-    processed_response = yep_chat.process_response(response)
-    
-    # Print the processed response
-    print(processed_response)
+# Instantiate the YEPCHAT class with default parameters
+YEPCHAT = YEPCHAT()
+
+# Define a prompt to send to the AI
+prompt = "What is the capital of France?"
+
+# Use the 'cha' method to get a response from the AI
+r = YEPCHAT.chat(prompt)
+print(r)
 
-if __name__ == "__main__":
-    main()
 ```
 
-### 3. `You.com` - search with you.com
+### 3. `You.com` - search with you.com -NOT WORKING
 ```python
 from webscout.AI import youChat
 
 # Instantiate the youchat class
 youChat = youChat()
 
 while True:
@@ -593,23 +590,42 @@
     except Exception as e:
         print("⚠️ An error occurred:", e)
 ```
 
 ### 4. `Gemini` - search with google gemini
 
 ```python
-from webscout.AI import Gemini
+import webscout
+from webscout.AI import GEMINI
+
+# Replace with the path to your bard.google.com.cookies.json file
+COOKIE_FILE = "path/to/bard.google.com.cookies.json"
+
+# Optional: Provide proxy details if needed
+PROXIES = {
+    "http": "http://proxy_server:port",
+    "https": "https://proxy_server:port",
+}
+
+# Initialize GEMINI with cookie file and optional proxies
+gemini = GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES)
+
+# Ask a question and print the response
+response = gemini.chat("What is the meaning of life?")
+print(response)
 
-# Create an instance of the Gemini class
-gemini = Gemini()
+# Ask another question, this time streaming the response
+for chunk in gemini.chat("Tell me a story", stream=True):
+    print(chunk, end="")
 
-# Use the chat method to send a message to the Gemini assistant
-response = gemini.chat("Your message here")
+# Reset the conversation to start a new interaction
+gemini.reset()
 
-# Print the response from the Gemini assistant
+# Ask a question with the code optimizer
+response = gemini.chat("Write Python code to print 'Hello, world!'", optimizer="code")
 print(response)
 ```
 ##  usage of image generator from Webscout.AI
 ### 5. `Prodia` - make image using prodia
 ```python
 from webscout.AI import Prodia
 
@@ -633,25 +649,26 @@
     update_file=True,
     proxies={},
     history_offset=10250,
     act=None,
     model=None # You can specify a model if needed
 )
 
-# Define a prompt to send to the AI
-prompt = "Tell me about india"
-
-# Use the 'ask' method to send the prompt and receive a response
-response = ai.ask(prompt)
-
-# Extract the text from the response
-response_text = ai.get_message(response)
-
-# Print the response text
-print(response_text)
+# Start an infinite loop for continuous interaction
+while True:
+    # Define a prompt to send to the AI
+    prompt = input("Enter your prompt: ")
+    
+    # Check if the user wants to exit the loop
+    if prompt.lower() == "exit":
+        break
+    
+    # Use the 'chat' method to send the prompt and receive a response
+    r = ai.chat(prompt)
+    print(r)
 ```
 ### 7. `PERPLEXITY` - Search With PERPLEXITY
 ```python
 from webscout.AI import PERPLEXITY
 # Create an instance of the PERPLEXITY class
 perplexity = PERPLEXITY()
 
@@ -661,18 +678,20 @@
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
 from webscout.AI import OPENGPT
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
-# This example sends a simple greeting and prints the response
-prompt = "tell me about india"
-response_str = opengpt.chat(prompt)
-print(response_str)
+while True:
+    # Prompt the user for input
+    prompt = input("Enter your prompt: ")
+    # Send the prompt to the OPENGPT model and print the response
+    response_str = opengpt.chat(prompt)
+    print(response_str)
 ```
 ### 9. `KOBOLDIA` - 
 ```python
 from webscout.AI import KOBOLDAI
 
 # Instantiate the KOBOLDAI class with default parameters
 koboldai = KOBOLDAI()
@@ -707,15 +726,15 @@
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
-### `LLM`
+### `LLM` --not working
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.9 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.0 Summary: Search for
 anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc
 Also containes AI models, can transcribe yt videos, have TTS support and now
 has webai(terminal gpt and open interpeter) support Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -21,16 +21,16 @@
 curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
 asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist:
-appdirsGoogleBard1>=2.1.4 Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
+Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
+Dist: GoogleBard1>=2.1.4 Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
 == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
        _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos, have TTS support and now has webai(terminal gpt and open
  interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
    Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
      version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
@@ -52,81 +52,81 @@
   duckduckgocom-and) - [7. `translate()` - translation by DuckDuckGo.com and
     Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom) - [8.
 `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---
  suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI](#usage-of-
   webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---
   search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b powered by
     yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) - [3.
-`You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
-- search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
-image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
-[5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
-  [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
- with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
-  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka]
- (#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---
-chat-with-cohere) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) -
-  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
-   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
-version ```python3 python -m webscout --help ``` | Command | Description | |---
-----------------------------------------|--------------------------------------
- -----------------------------------------------------------------| | python -
- m webscout answers -k Text | CLI function to perform an answers search using
- Webscout. | | python -m webscout images -k Text | CLI function to perform an
-    images search using Webscout. | | python -m webscout maps -k Text | CLI
-function to perform a maps search using Webscout. | | python -m webscout news -
-  k Text | CLI function to perform a news search using Webscout. | | python -
- m webscout suggestions -k Text | CLI function to perform a suggestions search
-using Webscout. | | python -m webscout text -k Text | CLI function to perform a
-  text search using Webscout. | | python -m webscout translate -k Text | CLI
-function to perform translate using Webscout. | | python -m webscout version |
-  A command-line interface command that prints and returns the version of the
-  program. | | python -m webscout videos -k Text | CLI function to perform a
-  videos search using DuckDuckGo API. | ## CLI to use LLM ```python python -
-  m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for
-Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for
- Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg
-for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
-  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
-     Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Transcriber The
-   transcriber function in webscout is a handy tool that transcribes YouTube
- videos. Here's an example code demonstrating its usage: ```python import sys
-from webscout import transcriber def extract_transcript(video_id): """Extracts
-        the transcript from a YouTube video.""" try: transcript_list =
-   transcriber.list_transcripts(video_id) for transcript in transcript_list:
-     transcript_data_list = transcript.fetch() lang = transcript.language
-     transcript_text = "" if transcript.language_code == 'en': for line in
- transcript_data_list: start_time = line['start'] end_time = start_time + line
-   ['duration'] formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line
-  ['text']}\n" transcript_text += formatted_line return transcript_text elif
-  transcript.is_translatable: english_transcript_list = transcript.translate
-('en').fetch() for line in english_transcript_list: start_time = line['start']
-end_time = start_time + line['duration'] formatted_line = f"{start_time:.2f} -
+`You.com` - search with you.com -NOT WORKING](#3-youcom---search-with-youcom--
+ not-working) - [4. `Gemini` - search with google gemini](#4-gemini---search-
+ with-google-gemini) - [usage of image generator from Webscout.AI](#usage-of-
+image-generator-from-webscoutai) - [5. `Prodia` - make image using prodia](#5-
+prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat With BlackBox]
+   (#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With
+PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With
+OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) -
+[10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat
+with cohere](#11-cohere---chat-with-cohere) - [`LLM` --not working](#llm---not-
+working) - [`LLM` with internet](#llm-with-internet) - [`Webai` - terminal gpt
+and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
+ model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
+Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
+ Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
+ for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
+ China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
+Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
+ gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
+for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
+for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
+ xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+ To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
+tool that transcribes YouTube videos. Here's an example code demonstrating its
+       usage: ```python import sys from webscout import transcriber def
+    extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ transcript.language transcript_text = "" if transcript.language_code == 'en':
+    for line in transcript_data_list: start_time = line['start'] end_time =
+     start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
-  transcript_text print("Transcript extraction failed. Please check the video
-  URL.") except Exception as e: print(f"Error: {e}") def main(): video_url =
- input("Enter the video link: ") if video_url: video_id = video_url.split("=")
-  [1] print("Video URL:", video_url) submit = input("Press 'Enter' to get the
-   transcript or type 'exit' to quit: ") if submit == '': print("Extracting
-Transcript...") transcript = extract_transcript(video_id) print('Transcript:')
-                            print(transcript) print
+  transcript_text elif transcript.is_translatable: english_transcript_list =
+    transcript.translate('en').fetch() for line in english_transcript_list:
+      start_time = line['start'] end_time = start_time + line['duration']
+    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+  transcript_text += formatted_line return transcript_text print("Transcript
+ extraction failed. Please check the video URL.") except Exception as e: print
+  (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
+ video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
+submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '': print("Extracting Transcript...") transcript =
+   extract_transcript(video_id) print('Transcript:') print(transcript) print
 ("__________________________________________________________________________________")
    elif submit.lower() == 'exit': print("Exiting...") sys.exit() else: print
  ("Invalid input. Please try again.") if __name__ == "__main__": main() ``` ##
 DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone feature designed to
  perform advanced web searches with enhanced capabilities. It is particularly
  powerful in extracting relevant information directly from webpages and Search
 engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which
@@ -262,109 +262,116 @@
      WEBS.suggestions("fly"): print(r) ``` ## usage of webscout.AI ### 1.
    `PhindSearch` - Search using Phind.com ```python from webscout.AI import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
- by yepchat Thanks To Divyansh Shukla for This code ```python from webscout.AI
-  import YepChat def main(): # Initialize the YepChat class with your message
-yep_chat = YepChat(message="who is pm of india") # Send the request and process
-     the response response = yep_chat.send_request() processed_response =
-   yep_chat.process_response(response) # Print the processed response print
- (processed_response) if __name__ == "__main__": main() ``` ### 3. `You.com` -
-search with you.com ```python from webscout.AI import youChat # Instantiate the
-   youchat class youChat = youChat() while True: # Ask the user for a prompt
-    prompt = input("ð¡ Enter a prompt (or type 'exit' to quit): ") # Exit
- condition if prompt.lower() == 'exit': break # Generate a completion based on
-the prompt try: completion = youChat.create(prompt) print("ð¬:", completion)
-    except Exception as e: print("â ï¸ An error occurred:", e) ``` ### 4.
-`Gemini` - search with google gemini ```python from webscout.AI import Gemini #
-Create an instance of the Gemini class gemini = Gemini() # Use the chat method
-to send a message to the Gemini assistant response = gemini.chat("Your message
- here") # Print the response from the Gemini assistant print(response) ``` ##
- usage of image generator from Webscout.AI ### 5. `Prodia` - make image using
-prodia ```python from webscout.AI import Prodia # Define a prompt for the image
- generation prompt = "A beautiful sunset over the ocean" # Use the prodia_cli
- method to generate an image based on the prompt Prodia.prodia_cli(prompt) ```
-### 6. `BlackBox` - Search/chat With BlackBox ```python from webscout.AI import
-   BLACKBOXAI from rich import print ai = BLACKBOXAI( is_conversation=True,
-   max_tokens=800, timeout=30, intro=None, filepath=None, update_file=True,
-  proxies={}, history_offset=10250, act=None, model=None # You can specify a
- model if needed ) # Define a prompt to send to the AI prompt = "Tell me about
-    india" # Use the 'ask' method to send the prompt and receive a response
-response = ai.ask(prompt) # Extract the text from the response response_text =
-ai.get_message(response) # Print the response text print(response_text) ``` ###
-  7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
-PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
-   () # Example usage: prompt = "Explain the concept of recursion in simple
-terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
-- chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
-  (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
-    simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
-  ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
-with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
- AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
- response from the AI response = koboldai.ask(prompt) # Extract and print the
-   message from the response message = koboldai.get_message(response) print
-(message) ``` ### 10. `Reka` - chat with reka ```python from webscout.AI import
-  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
-      prompt = "tell me about india" response_str = a.chat(prompt) print
-     (response_str) ``` ### 11. `Cohere` - chat with cohere ```python from
-  webscout.AI import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
-  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
- (prompt) print(response_str) ``` ### `LLM` ```python from webscout.LLM import
-  LLM # Read the system message from the file with open('system.txt', 'r') as
- file: system_message = file.read() # Initialize the LLM class with the model
-     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
- system_message=system_message) while True: # Get the user input user_input =
-input("User: ") # Define the messages to be sent messages = [ {"role": "user",
-  "content": user_input} ] # Use the mistral_chat method to get the response
-response = llm.chat(messages) # Print the response print("AI: ", response) ```
-   ### `LLM` with internet ```python from __future__ import annotations from
-typing import List, Optional from webscout import LLM from webscout import WEBS
-import warnings system_message: str = ( "As AI, you possess internet access and
- are capable of executing real-time web searches based on user inputs. " "You
-shall utilize this capability to enrich conversations, offer informed insights,
-  and augment your ability to " "respond accurately and thoroughly. However,
-    refrain from stating 'You have provided a list of strings,' ensuring "
- "seamless interactions with users. Embrace a responsive demeanor, harnessing
-available online resources to address " "queries, share pertinent content, and
-   facilitate meaningful exchanges. By doing so, you create value through "
-"connection and engagement, ultimately enhancing overall user satisfaction and
-  experience. Additionally, " "continue upholding the principles of respect,
-  impartiality, and intellectual integrity throughout all interactions." ) #
-       Ignore the specific UserWarning warnings.filterwarnings("ignore",
-      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
- (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
-  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
- [str]: """ Chat function to perform a web search based on the user input and
-generate a response using the LLM model. Parameters ---------- user_input : str
-    The user input to be used for the web search webs : WEBS The web search
-   instance to be used to perform the search max_results : int, optional The
-  maximum number of search results to include in the response, by default 10
-Returns ------- Optional[str] The response generated by the LLM model, or None
-  if there is no response """ # Perform a web search based on the user input
-search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
-          safesearch="off", timelimit="y", max_results=max_results ):
- search_results.append(str(r)) # Convert each result to a string # Define the
-   messages to be sent, including the user input, search results, and system
-message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
-results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
-     response response = LLM.chat(messages) return response if __name__ ==
-  "__main__": while True: # Get the user input user_input = input("User: ") #
- Perform a web search based on the user input with WEBS() as webs: response =
-chat(user_input, webs) # Print the response if response: print("AI:", response)
-else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
- ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
-    """ Wrap the webscout default method in a try-except block to catch any
-  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
-  ( max_tokens=500, provider="cohere", temperature=0.7, top_k=40, top_p=0.95,
-model="command-r-plus", # Replace with your desired model auth=None, # Replace
-  with your auth key/value (if needed) timeout=30, disable_conversation=True,
-filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
-      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
-webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
-     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
-use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
-                        --provider "phind" --rawdog ```
+by yepchat ```python from webscout.AI import YEPCHAT # Instantiate the YEPCHAT
+class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
+the AI prompt = "What is the capital of France?" # Use the 'cha' method to get
+a response from the AI r = YEPCHAT.chat(prompt) print(r) ``` ### 3. `You.com` -
+ search with you.com -NOT WORKING ```python from webscout.AI import youChat #
+ Instantiate the youchat class youChat = youChat() while True: # Ask the user
+for a prompt prompt = input("ð¡ Enter a prompt (or type 'exit' to quit): ") #
+Exit condition if prompt.lower() == 'exit': break # Generate a completion based
+     on the prompt try: completion = youChat.create(prompt) print("ð¬:",
+ completion) except Exception as e: print("â ï¸ An error occurred:", e) ```
+  ### 4. `Gemini` - search with google gemini ```python import webscout from
+           webscout.AI import GEMINI # Replace with the path to your
+           bard.google.com.cookies.json file COOKIE_FILE = "path/to/
+   bard.google.com.cookies.json" # Optional: Provide proxy details if needed
+PROXIES = { "http": "http://proxy_server:port", "https": "https://proxy_server:
+  port", } # Initialize GEMINI with cookie file and optional proxies gemini =
+ GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES) # Ask a question and print the
+response response = gemini.chat("What is the meaning of life?") print(response)
+     # Ask another question, this time streaming the response for chunk in
+ gemini.chat("Tell me a story", stream=True): print(chunk, end="") # Reset the
+ conversation to start a new interaction gemini.reset() # Ask a question with
+ the code optimizer response = gemini.chat("Write Python code to print 'Hello,
+  world!'", optimizer="code") print(response) ``` ## usage of image generator
+   from Webscout.AI ### 5. `Prodia` - make image using prodia ```python from
+ webscout.AI import Prodia # Define a prompt for the image generation prompt =
+"A beautiful sunset over the ocean" # Use the prodia_cli method to generate an
+  image based on the prompt Prodia.prodia_cli(prompt) ``` ### 6. `BlackBox` -
+  Search/chat With BlackBox ```python from webscout.AI import BLACKBOXAI from
+   rich import print ai = BLACKBOXAI( is_conversation=True, max_tokens=800,
+     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
+history_offset=10250, act=None, model=None # You can specify a model if needed
+ ) # Start an infinite loop for continuous interaction while True: # Define a
+ prompt to send to the AI prompt = input("Enter your prompt: ") # Check if the
+user wants to exit the loop if prompt.lower() == "exit": break # Use the 'chat'
+ method to send the prompt and receive a response r = ai.chat(prompt) print(r)
+  ``` ### 7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI
+  import PERPLEXITY # Create an instance of the PERPLEXITY class perplexity =
+  PERPLEXITY() # Example usage: prompt = "Explain the concept of recursion in
+ simple terms." response = perplexity.chat(prompt) print(response) ``` ### 8.
+`OpenGPT` - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt
+  = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30) while True: #
+  Prompt the user for input prompt = input("Enter your prompt: ") # Send the
+prompt to the OPENGPT model and print the response response_str = opengpt.chat
+(prompt) print(response_str) ``` ### 9. `KOBOLDIA` - ```python from webscout.AI
+   import KOBOLDAI # Instantiate the KOBOLDAI class with default parameters
+koboldai = KOBOLDAI() # Define a prompt to send to the AI prompt = "What is the
+   capital of France?" # Use the 'ask' method to get a response from the AI
+   response = koboldai.ask(prompt) # Extract and print the message from the
+ response message = koboldai.get_message(response) print(message) ``` ### 10.
+    `Reka` - chat with reka ```python from webscout.AI import REKA a = REKA
+ (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
+ me about india" response_str = a.chat(prompt) print(response_str) ``` ### 11.
+`Cohere` - chat with cohere ```python from webscout.AI import Cohere a = Cohere
+ (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
+me about india" response_str = a.chat(prompt) print(response_str) ``` ### `LLM`
+--not working ```python from webscout.LLM import LLM # Read the system message
+from the file with open('system.txt', 'r') as file: system_message = file.read
+() # Initialize the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+ __future__ import annotations from typing import List, Optional from webscout
+  import LLM from webscout import WEBS import warnings system_message: str =
+ ( "As AI, you possess internet access and are capable of executing real-time
+  web searches based on user inputs. " "You shall utilize this capability to
+ enrich conversations, offer informed insights, and augment your ability to "
+  "respond accurately and thoroughly. However, refrain from stating 'You have
+  provided a list of strings,' ensuring " "seamless interactions with users.
+Embrace a responsive demeanor, harnessing available online resources to address
+ " "queries, share pertinent content, and facilitate meaningful exchanges. By
+  doing so, you create value through " "connection and engagement, ultimately
+ enhancing overall user satisfaction and experience. Additionally, " "continue
+ upholding the principles of respect, impartiality, and intellectual integrity
+       throughout all interactions." ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
+ Parameters ---------- user_input : str The user input to be used for the web
+  search webs : WEBS The web search instance to be used to perform the search
+max_results : int, optional The maximum number of search results to include in
+    the response, by default 10 Returns ------- Optional[str] The response
+generated by the LLM model, or None if there is no response """ # Perform a web
+    search based on the user input search_results: List[str] = [] for r in
+    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
+max_results=max_results ): search_results.append(str(r)) # Convert each result
+to a string # Define the messages to be sent, including the user input, search
+results, and system message messages = [ {"role": "user", "content": user_input
+  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
+ chat method to get the response response = LLM.chat(messages) return response
+if __name__ == "__main__": while True: # Get the user input user_input = input
+("User: ") # Perform a web search based on the user input with WEBS() as webs:
+response = chat(user_input, webs) # Print the response if response: print("AI:
+  ", response) else: print("No response") ``` ## `Webai` - terminal gpt and a
+         open interpeter ```python from webscout.webai import Main def
+ use_rawdog_with_webai(prompt): """ Wrap the webscout default method in a try-
+except block to catch any unhandled exceptions and print a helpful message. """
+  try: webai_bot = Main( max_tokens=500, provider="cohere", temperature=0.7,
+top_k=40, top_p=0.95, model="command-r-plus", # Replace with your desired model
+     auth=None, # Replace with your auth key/value (if needed) timeout=30,
+    disable_conversation=True, filepath=None, update_file=True, intro=None,
+   rawdog=True, history_offset=10250, awesome_prompt=None, proxy_path=None,
+quiet=True ) webai_response = webai_bot.default(prompt) except Exception as e:
+ print("Unexpected error:", e) if __name__ == "__main__": user_prompt = input
+("Enter your prompt: ") use_rawdog_with_webai(user_prompt) ``` ```shell python
+            -m webscout.webai webai --provider "phind" --rawdog ```
```

### Comparing `webscout-1.3.9/README.md` & `webscout-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,25 +32,25 @@
     - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
     - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
     - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
     - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
   - [usage of webscout.AI](#usage-of-webscoutai)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
-    - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
+    - [3. `You.com` - search with you.com -NOT WORKING](#3-youcom---search-with-youcom--not-working)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
-    - [`LLM`](#llm)
+    - [`LLM` --not working](#llm---not-working)
     - [`LLM` with internet](#llm-with-internet)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -494,34 +494,30 @@
 response = ph.ask(prompt)
 
 # Extract and print the message from the response
 message = ph.get_message(response)
 print(message)
 ```
 ### 2. `YepChat` - Chat with mistral 8x7b powered by yepchat
-Thanks To Divyansh Shukla for This code
 ```python
-from webscout.AI import YepChat
+from webscout.AI import YEPCHAT
 
-def main():
-    # Initialize the YepChat class with your message
-    yep_chat = YepChat(message="who is pm of india")
-    
-    # Send the request and process the response
-    response = yep_chat.send_request()
-    processed_response = yep_chat.process_response(response)
-    
-    # Print the processed response
-    print(processed_response)
+# Instantiate the YEPCHAT class with default parameters
+YEPCHAT = YEPCHAT()
+
+# Define a prompt to send to the AI
+prompt = "What is the capital of France?"
+
+# Use the 'cha' method to get a response from the AI
+r = YEPCHAT.chat(prompt)
+print(r)
 
-if __name__ == "__main__":
-    main()
 ```
 
-### 3. `You.com` - search with you.com
+### 3. `You.com` - search with you.com -NOT WORKING
 ```python
 from webscout.AI import youChat
 
 # Instantiate the youchat class
 youChat = youChat()
 
 while True:
@@ -539,23 +535,42 @@
     except Exception as e:
         print("⚠️ An error occurred:", e)
 ```
 
 ### 4. `Gemini` - search with google gemini
 
 ```python
-from webscout.AI import Gemini
+import webscout
+from webscout.AI import GEMINI
+
+# Replace with the path to your bard.google.com.cookies.json file
+COOKIE_FILE = "path/to/bard.google.com.cookies.json"
+
+# Optional: Provide proxy details if needed
+PROXIES = {
+    "http": "http://proxy_server:port",
+    "https": "https://proxy_server:port",
+}
+
+# Initialize GEMINI with cookie file and optional proxies
+gemini = GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES)
+
+# Ask a question and print the response
+response = gemini.chat("What is the meaning of life?")
+print(response)
 
-# Create an instance of the Gemini class
-gemini = Gemini()
+# Ask another question, this time streaming the response
+for chunk in gemini.chat("Tell me a story", stream=True):
+    print(chunk, end="")
 
-# Use the chat method to send a message to the Gemini assistant
-response = gemini.chat("Your message here")
+# Reset the conversation to start a new interaction
+gemini.reset()
 
-# Print the response from the Gemini assistant
+# Ask a question with the code optimizer
+response = gemini.chat("Write Python code to print 'Hello, world!'", optimizer="code")
 print(response)
 ```
 ##  usage of image generator from Webscout.AI
 ### 5. `Prodia` - make image using prodia
 ```python
 from webscout.AI import Prodia
 
@@ -579,25 +594,26 @@
     update_file=True,
     proxies={},
     history_offset=10250,
     act=None,
     model=None # You can specify a model if needed
 )
 
-# Define a prompt to send to the AI
-prompt = "Tell me about india"
-
-# Use the 'ask' method to send the prompt and receive a response
-response = ai.ask(prompt)
-
-# Extract the text from the response
-response_text = ai.get_message(response)
-
-# Print the response text
-print(response_text)
+# Start an infinite loop for continuous interaction
+while True:
+    # Define a prompt to send to the AI
+    prompt = input("Enter your prompt: ")
+    
+    # Check if the user wants to exit the loop
+    if prompt.lower() == "exit":
+        break
+    
+    # Use the 'chat' method to send the prompt and receive a response
+    r = ai.chat(prompt)
+    print(r)
 ```
 ### 7. `PERPLEXITY` - Search With PERPLEXITY
 ```python
 from webscout.AI import PERPLEXITY
 # Create an instance of the PERPLEXITY class
 perplexity = PERPLEXITY()
 
@@ -607,18 +623,20 @@
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
 from webscout.AI import OPENGPT
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
-# This example sends a simple greeting and prints the response
-prompt = "tell me about india"
-response_str = opengpt.chat(prompt)
-print(response_str)
+while True:
+    # Prompt the user for input
+    prompt = input("Enter your prompt: ")
+    # Send the prompt to the OPENGPT model and print the response
+    response_str = opengpt.chat(prompt)
+    print(response_str)
 ```
 ### 9. `KOBOLDIA` - 
 ```python
 from webscout.AI import KOBOLDAI
 
 # Instantiate the KOBOLDAI class with default parameters
 koboldai = KOBOLDAI()
@@ -653,15 +671,15 @@
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
-### `LLM`
+### `LLM` --not working
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
```

#### html2text {}

```diff
@@ -23,81 +23,81 @@
   duckduckgocom-and) - [7. `translate()` - translation by DuckDuckGo.com and
     Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom) - [8.
 `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---
  suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI](#usage-of-
   webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---
   search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b powered by
     yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) - [3.
-`You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
-- search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
-image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
-[5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
-  [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
- with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
-  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka]
- (#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---
-chat-with-cohere) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) -
-  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
-   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
-version ```python3 python -m webscout --help ``` | Command | Description | |---
-----------------------------------------|--------------------------------------
- -----------------------------------------------------------------| | python -
- m webscout answers -k Text | CLI function to perform an answers search using
- Webscout. | | python -m webscout images -k Text | CLI function to perform an
-    images search using Webscout. | | python -m webscout maps -k Text | CLI
-function to perform a maps search using Webscout. | | python -m webscout news -
-  k Text | CLI function to perform a news search using Webscout. | | python -
- m webscout suggestions -k Text | CLI function to perform a suggestions search
-using Webscout. | | python -m webscout text -k Text | CLI function to perform a
-  text search using Webscout. | | python -m webscout translate -k Text | CLI
-function to perform translate using Webscout. | | python -m webscout version |
-  A command-line interface command that prints and returns the version of the
-  program. | | python -m webscout videos -k Text | CLI function to perform a
-  videos search using DuckDuckGo API. | ## CLI to use LLM ```python python -
-  m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for
-Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for
- Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg
-for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
-  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
-     Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Transcriber The
-   transcriber function in webscout is a handy tool that transcribes YouTube
- videos. Here's an example code demonstrating its usage: ```python import sys
-from webscout import transcriber def extract_transcript(video_id): """Extracts
-        the transcript from a YouTube video.""" try: transcript_list =
-   transcriber.list_transcripts(video_id) for transcript in transcript_list:
-     transcript_data_list = transcript.fetch() lang = transcript.language
-     transcript_text = "" if transcript.language_code == 'en': for line in
- transcript_data_list: start_time = line['start'] end_time = start_time + line
-   ['duration'] formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line
-  ['text']}\n" transcript_text += formatted_line return transcript_text elif
-  transcript.is_translatable: english_transcript_list = transcript.translate
-('en').fetch() for line in english_transcript_list: start_time = line['start']
-end_time = start_time + line['duration'] formatted_line = f"{start_time:.2f} -
+`You.com` - search with you.com -NOT WORKING](#3-youcom---search-with-youcom--
+ not-working) - [4. `Gemini` - search with google gemini](#4-gemini---search-
+ with-google-gemini) - [usage of image generator from Webscout.AI](#usage-of-
+image-generator-from-webscoutai) - [5. `Prodia` - make image using prodia](#5-
+prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat With BlackBox]
+   (#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With
+PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With
+OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) -
+[10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat
+with cohere](#11-cohere---chat-with-cohere) - [`LLM` --not working](#llm---not-
+working) - [`LLM` with internet](#llm-with-internet) - [`Webai` - terminal gpt
+and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
+ model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
+Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
+ Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
+ for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
+ China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
+Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
+ gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
+for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
+for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
+ xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+ To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
+tool that transcribes YouTube videos. Here's an example code demonstrating its
+       usage: ```python import sys from webscout import transcriber def
+    extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ transcript.language transcript_text = "" if transcript.language_code == 'en':
+    for line in transcript_data_list: start_time = line['start'] end_time =
+     start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
-  transcript_text print("Transcript extraction failed. Please check the video
-  URL.") except Exception as e: print(f"Error: {e}") def main(): video_url =
- input("Enter the video link: ") if video_url: video_id = video_url.split("=")
-  [1] print("Video URL:", video_url) submit = input("Press 'Enter' to get the
-   transcript or type 'exit' to quit: ") if submit == '': print("Extracting
-Transcript...") transcript = extract_transcript(video_id) print('Transcript:')
-                            print(transcript) print
+  transcript_text elif transcript.is_translatable: english_transcript_list =
+    transcript.translate('en').fetch() for line in english_transcript_list:
+      start_time = line['start'] end_time = start_time + line['duration']
+    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+  transcript_text += formatted_line return transcript_text print("Transcript
+ extraction failed. Please check the video URL.") except Exception as e: print
+  (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
+ video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
+submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '': print("Extracting Transcript...") transcript =
+   extract_transcript(video_id) print('Transcript:') print(transcript) print
 ("__________________________________________________________________________________")
    elif submit.lower() == 'exit': print("Exiting...") sys.exit() else: print
  ("Invalid input. Please try again.") if __name__ == "__main__": main() ``` ##
 DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone feature designed to
  perform advanced web searches with enhanced capabilities. It is particularly
  powerful in extracting relevant information directly from webpages and Search
 engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which
@@ -233,109 +233,116 @@
      WEBS.suggestions("fly"): print(r) ``` ## usage of webscout.AI ### 1.
    `PhindSearch` - Search using Phind.com ```python from webscout.AI import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
- by yepchat Thanks To Divyansh Shukla for This code ```python from webscout.AI
-  import YepChat def main(): # Initialize the YepChat class with your message
-yep_chat = YepChat(message="who is pm of india") # Send the request and process
-     the response response = yep_chat.send_request() processed_response =
-   yep_chat.process_response(response) # Print the processed response print
- (processed_response) if __name__ == "__main__": main() ``` ### 3. `You.com` -
-search with you.com ```python from webscout.AI import youChat # Instantiate the
-   youchat class youChat = youChat() while True: # Ask the user for a prompt
-    prompt = input("ð¡ Enter a prompt (or type 'exit' to quit): ") # Exit
- condition if prompt.lower() == 'exit': break # Generate a completion based on
-the prompt try: completion = youChat.create(prompt) print("ð¬:", completion)
-    except Exception as e: print("â ï¸ An error occurred:", e) ``` ### 4.
-`Gemini` - search with google gemini ```python from webscout.AI import Gemini #
-Create an instance of the Gemini class gemini = Gemini() # Use the chat method
-to send a message to the Gemini assistant response = gemini.chat("Your message
- here") # Print the response from the Gemini assistant print(response) ``` ##
- usage of image generator from Webscout.AI ### 5. `Prodia` - make image using
-prodia ```python from webscout.AI import Prodia # Define a prompt for the image
- generation prompt = "A beautiful sunset over the ocean" # Use the prodia_cli
- method to generate an image based on the prompt Prodia.prodia_cli(prompt) ```
-### 6. `BlackBox` - Search/chat With BlackBox ```python from webscout.AI import
-   BLACKBOXAI from rich import print ai = BLACKBOXAI( is_conversation=True,
-   max_tokens=800, timeout=30, intro=None, filepath=None, update_file=True,
-  proxies={}, history_offset=10250, act=None, model=None # You can specify a
- model if needed ) # Define a prompt to send to the AI prompt = "Tell me about
-    india" # Use the 'ask' method to send the prompt and receive a response
-response = ai.ask(prompt) # Extract the text from the response response_text =
-ai.get_message(response) # Print the response text print(response_text) ``` ###
-  7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
-PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
-   () # Example usage: prompt = "Explain the concept of recursion in simple
-terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
-- chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
-  (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
-    simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
-  ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
-with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
- AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
- response from the AI response = koboldai.ask(prompt) # Extract and print the
-   message from the response message = koboldai.get_message(response) print
-(message) ``` ### 10. `Reka` - chat with reka ```python from webscout.AI import
-  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
-      prompt = "tell me about india" response_str = a.chat(prompt) print
-     (response_str) ``` ### 11. `Cohere` - chat with cohere ```python from
-  webscout.AI import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
-  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
- (prompt) print(response_str) ``` ### `LLM` ```python from webscout.LLM import
-  LLM # Read the system message from the file with open('system.txt', 'r') as
- file: system_message = file.read() # Initialize the LLM class with the model
-     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
- system_message=system_message) while True: # Get the user input user_input =
-input("User: ") # Define the messages to be sent messages = [ {"role": "user",
-  "content": user_input} ] # Use the mistral_chat method to get the response
-response = llm.chat(messages) # Print the response print("AI: ", response) ```
-   ### `LLM` with internet ```python from __future__ import annotations from
-typing import List, Optional from webscout import LLM from webscout import WEBS
-import warnings system_message: str = ( "As AI, you possess internet access and
- are capable of executing real-time web searches based on user inputs. " "You
-shall utilize this capability to enrich conversations, offer informed insights,
-  and augment your ability to " "respond accurately and thoroughly. However,
-    refrain from stating 'You have provided a list of strings,' ensuring "
- "seamless interactions with users. Embrace a responsive demeanor, harnessing
-available online resources to address " "queries, share pertinent content, and
-   facilitate meaningful exchanges. By doing so, you create value through "
-"connection and engagement, ultimately enhancing overall user satisfaction and
-  experience. Additionally, " "continue upholding the principles of respect,
-  impartiality, and intellectual integrity throughout all interactions." ) #
-       Ignore the specific UserWarning warnings.filterwarnings("ignore",
-      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
- (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
-  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
- [str]: """ Chat function to perform a web search based on the user input and
-generate a response using the LLM model. Parameters ---------- user_input : str
-    The user input to be used for the web search webs : WEBS The web search
-   instance to be used to perform the search max_results : int, optional The
-  maximum number of search results to include in the response, by default 10
-Returns ------- Optional[str] The response generated by the LLM model, or None
-  if there is no response """ # Perform a web search based on the user input
-search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
-          safesearch="off", timelimit="y", max_results=max_results ):
- search_results.append(str(r)) # Convert each result to a string # Define the
-   messages to be sent, including the user input, search results, and system
-message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
-results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
-     response response = LLM.chat(messages) return response if __name__ ==
-  "__main__": while True: # Get the user input user_input = input("User: ") #
- Perform a web search based on the user input with WEBS() as webs: response =
-chat(user_input, webs) # Print the response if response: print("AI:", response)
-else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
- ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
-    """ Wrap the webscout default method in a try-except block to catch any
-  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
-  ( max_tokens=500, provider="cohere", temperature=0.7, top_k=40, top_p=0.95,
-model="command-r-plus", # Replace with your desired model auth=None, # Replace
-  with your auth key/value (if needed) timeout=30, disable_conversation=True,
-filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
-      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
-webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
-     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
-use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
-                        --provider "phind" --rawdog ```
+by yepchat ```python from webscout.AI import YEPCHAT # Instantiate the YEPCHAT
+class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
+the AI prompt = "What is the capital of France?" # Use the 'cha' method to get
+a response from the AI r = YEPCHAT.chat(prompt) print(r) ``` ### 3. `You.com` -
+ search with you.com -NOT WORKING ```python from webscout.AI import youChat #
+ Instantiate the youchat class youChat = youChat() while True: # Ask the user
+for a prompt prompt = input("ð¡ Enter a prompt (or type 'exit' to quit): ") #
+Exit condition if prompt.lower() == 'exit': break # Generate a completion based
+     on the prompt try: completion = youChat.create(prompt) print("ð¬:",
+ completion) except Exception as e: print("â ï¸ An error occurred:", e) ```
+  ### 4. `Gemini` - search with google gemini ```python import webscout from
+           webscout.AI import GEMINI # Replace with the path to your
+           bard.google.com.cookies.json file COOKIE_FILE = "path/to/
+   bard.google.com.cookies.json" # Optional: Provide proxy details if needed
+PROXIES = { "http": "http://proxy_server:port", "https": "https://proxy_server:
+  port", } # Initialize GEMINI with cookie file and optional proxies gemini =
+ GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES) # Ask a question and print the
+response response = gemini.chat("What is the meaning of life?") print(response)
+     # Ask another question, this time streaming the response for chunk in
+ gemini.chat("Tell me a story", stream=True): print(chunk, end="") # Reset the
+ conversation to start a new interaction gemini.reset() # Ask a question with
+ the code optimizer response = gemini.chat("Write Python code to print 'Hello,
+  world!'", optimizer="code") print(response) ``` ## usage of image generator
+   from Webscout.AI ### 5. `Prodia` - make image using prodia ```python from
+ webscout.AI import Prodia # Define a prompt for the image generation prompt =
+"A beautiful sunset over the ocean" # Use the prodia_cli method to generate an
+  image based on the prompt Prodia.prodia_cli(prompt) ``` ### 6. `BlackBox` -
+  Search/chat With BlackBox ```python from webscout.AI import BLACKBOXAI from
+   rich import print ai = BLACKBOXAI( is_conversation=True, max_tokens=800,
+     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
+history_offset=10250, act=None, model=None # You can specify a model if needed
+ ) # Start an infinite loop for continuous interaction while True: # Define a
+ prompt to send to the AI prompt = input("Enter your prompt: ") # Check if the
+user wants to exit the loop if prompt.lower() == "exit": break # Use the 'chat'
+ method to send the prompt and receive a response r = ai.chat(prompt) print(r)
+  ``` ### 7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI
+  import PERPLEXITY # Create an instance of the PERPLEXITY class perplexity =
+  PERPLEXITY() # Example usage: prompt = "Explain the concept of recursion in
+ simple terms." response = perplexity.chat(prompt) print(response) ``` ### 8.
+`OpenGPT` - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt
+  = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30) while True: #
+  Prompt the user for input prompt = input("Enter your prompt: ") # Send the
+prompt to the OPENGPT model and print the response response_str = opengpt.chat
+(prompt) print(response_str) ``` ### 9. `KOBOLDIA` - ```python from webscout.AI
+   import KOBOLDAI # Instantiate the KOBOLDAI class with default parameters
+koboldai = KOBOLDAI() # Define a prompt to send to the AI prompt = "What is the
+   capital of France?" # Use the 'ask' method to get a response from the AI
+   response = koboldai.ask(prompt) # Extract and print the message from the
+ response message = koboldai.get_message(response) print(message) ``` ### 10.
+    `Reka` - chat with reka ```python from webscout.AI import REKA a = REKA
+ (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
+ me about india" response_str = a.chat(prompt) print(response_str) ``` ### 11.
+`Cohere` - chat with cohere ```python from webscout.AI import Cohere a = Cohere
+ (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
+me about india" response_str = a.chat(prompt) print(response_str) ``` ### `LLM`
+--not working ```python from webscout.LLM import LLM # Read the system message
+from the file with open('system.txt', 'r') as file: system_message = file.read
+() # Initialize the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+ __future__ import annotations from typing import List, Optional from webscout
+  import LLM from webscout import WEBS import warnings system_message: str =
+ ( "As AI, you possess internet access and are capable of executing real-time
+  web searches based on user inputs. " "You shall utilize this capability to
+ enrich conversations, offer informed insights, and augment your ability to "
+  "respond accurately and thoroughly. However, refrain from stating 'You have
+  provided a list of strings,' ensuring " "seamless interactions with users.
+Embrace a responsive demeanor, harnessing available online resources to address
+ " "queries, share pertinent content, and facilitate meaningful exchanges. By
+  doing so, you create value through " "connection and engagement, ultimately
+ enhancing overall user satisfaction and experience. Additionally, " "continue
+ upholding the principles of respect, impartiality, and intellectual integrity
+       throughout all interactions." ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
+ Parameters ---------- user_input : str The user input to be used for the web
+  search webs : WEBS The web search instance to be used to perform the search
+max_results : int, optional The maximum number of search results to include in
+    the response, by default 10 Returns ------- Optional[str] The response
+generated by the LLM model, or None if there is no response """ # Perform a web
+    search based on the user input search_results: List[str] = [] for r in
+    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
+max_results=max_results ): search_results.append(str(r)) # Convert each result
+to a string # Define the messages to be sent, including the user input, search
+results, and system message messages = [ {"role": "user", "content": user_input
+  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
+ chat method to get the response response = LLM.chat(messages) return response
+if __name__ == "__main__": while True: # Get the user input user_input = input
+("User: ") # Perform a web search based on the user input with WEBS() as webs:
+response = chat(user_input, webs) # Print the response if response: print("AI:
+  ", response) else: print("No response") ``` ## `Webai` - terminal gpt and a
+         open interpeter ```python from webscout.webai import Main def
+ use_rawdog_with_webai(prompt): """ Wrap the webscout default method in a try-
+except block to catch any unhandled exceptions and print a helpful message. """
+  try: webai_bot = Main( max_tokens=500, provider="cohere", temperature=0.7,
+top_k=40, top_p=0.95, model="command-r-plus", # Replace with your desired model
+     auth=None, # Replace with your auth key/value (if needed) timeout=30,
+    disable_conversation=True, filepath=None, update_file=True, intro=None,
+   rawdog=True, history_offset=10250, awesome_prompt=None, proxy_path=None,
+quiet=True ) webai_response = webai_bot.default(prompt) except Exception as e:
+ print("Unexpected error:", e) if __name__ == "__main__": user_prompt = input
+("Enter your prompt: ") use_rawdog_with_webai(user_prompt) ``` ```shell python
+            -m webscout.webai webai --provider "phind" --rawdog ```
```

### Comparing `webscout-1.3.9/setup.py` & `webscout-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.3.9", 
+    version="1.4.0", 
     description="Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -47,15 +47,15 @@
         "requests",
         "sse_starlette",
         "termcolor",
         "tiktoken",
         "tldextract",
         "orjson",
         "PyYAML",
-        "appdirs"
+        "appdirs",
         "GoogleBard1>=2.1.4"
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout-ai-phindsearch = webscout.AI:phindsearch",
             "webscout-ai-yepchat = webscout.AI:yepchat",
```

### Comparing `webscout-1.3.9/webscout/AI.py` & `webscout-1.4.0/webscout/AI.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
             proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
         """
+        self.session = requests.Session()
         self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
         self.model = model
         self.temperature = temperature
         self.presence_penalty = presence_penalty
         self.frequency_penalty = frequency_penalty
         self.top_p = top_p
@@ -4154,15 +4155,15 @@
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         temperature: float = 0.6,
         presence_penalty: int = 0,
         frequency_penalty: int = 0,
         top_p: float = 0.7,
-        model: str ="Mixtral-8x7B-Instruct-v0.1",
+        model: str = "Mixtral-8x7B-Instruct-v0.1",
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
@@ -4181,14 +4182,15 @@
             intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
             proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
         """
+        self.session = requests.Session()
         self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
         self.model = model
         self.temperature = temperature
         self.presence_penalty = presence_penalty
         self.frequency_penalty = frequency_penalty
         self.top_p = top_p
@@ -4359,14 +4361,239 @@
         """Retrieves message only from response
 
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        try:
+            if response["choices"][0].get("delta"):
+                return response["choices"][0]["delta"]["content"]
+            return response["choices"][0]["message"]["content"]
+        except KeyError:
+            return ""
+
+
+class AsyncYEPCHAT(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.6,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 0.7,
+        model: str = "Mixtral-8x7B-Instruct-v0.1",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates YEPCHAT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.6.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.7.
+            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://api.yep.com/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Accept": "*/*",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Content-Type": "application/json; charset=utf-8",
+            "Origin": "https://yep.com",
+            "Referer": "https://yep.com/",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(
+            headers=self.headers,
+            proxies=proxies,
+        )
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "cmpl-c61c1c88de4e4ad3a79134775d17ea0c",
+            "object": "chat.completion.chunk",
+            "created": 1713876886,
+            "model": "Mixtral-8x7B-Instruct-v0.1",
+            "choices": [
+                {
+                    "index": 0,
+                    "delta": {
+                        "role": null,
+                        "content": " Sure, I can help with that. Are you looking for information on how to start coding, or do you need help with a specific coding problem? We can discuss various programming languages like Python, JavaScript, Java, C++, or others. Please provide more details so I can assist you better."
+                        },
+                    "finish_reason": null
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        payload = {
+            "stream": True,
+            "max_tokens": 1280,
+            "top_p": self.top_p,
+            "temperature": self.temperature,
+            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "model": self.model,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if not response.is_success:
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase}) - {response.text}"
+                    )
+
+                message_load = ""
+                async for value in response.aiter_lines():
+                    try:
+                        resp = sanitize_stream(value)
+                        incomplete_message = await self.get_message(resp)
+                        if incomplete_message:
+                            message_load += incomplete_message
+                            resp["choices"][0]["delta"]["content"] = message_load
+                            self.last_response.update(resp)
+                            yield value if raw else resp
+                        elif raw:
+                            yield value
+                    except json.decoder.JSONDecodeError:
+                        pass
+
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
         try:
             if response["choices"][0].get("delta"):
                 return response["choices"][0]["delta"]["content"]
             return response["choices"][0]["message"]["content"]
         except KeyError:
```

### Comparing `webscout-1.3.9/webscout/AIbase.py` & `webscout-1.4.0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/AIutel.py` & `webscout-1.4.0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/DWEBS.py` & `webscout-1.4.0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/LLM.py` & `webscout-1.4.0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/__init__.py` & `webscout-1.4.0/webscout/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/async_providers.py` & `webscout-1.4.0/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/cli.py` & `webscout-1.4.0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/g4f.py` & `webscout-1.4.0/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/models.py` & `webscout-1.4.0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/transcriber.py` & `webscout-1.4.0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/utils.py` & `webscout-1.4.0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/voice.py` & `webscout-1.4.0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/webai.py` & `webscout-1.4.0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/webscout_search.py` & `webscout-1.4.0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout/webscout_search_async.py` & `webscout-1.4.0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.3.9/webscout.egg-info/PKG-INFO` & `webscout-1.4.0/webscout.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.3.9
+Version: 1.4.0
 Summary: Search for anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can transcribe yt videos, have TTS support and now has webai(terminal gpt and open interpeter) support
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -43,15 +43,16 @@
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
 Requires-Dist: orjson
 Requires-Dist: PyYAML
-Requires-Dist: appdirsGoogleBard1>=2.1.4
+Requires-Dist: appdirs
+Requires-Dist: GoogleBard1>=2.1.4
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 #  webscout
 <p align="center">
 
@@ -86,25 +87,25 @@
     - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
     - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
     - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
     - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
   - [usage of webscout.AI](#usage-of-webscoutai)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
-    - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
+    - [3. `You.com` - search with you.com -NOT WORKING](#3-youcom---search-with-youcom--not-working)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDIA` -](#9-koboldia--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
-    - [`LLM`](#llm)
+    - [`LLM` --not working](#llm---not-working)
     - [`LLM` with internet](#llm-with-internet)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -548,34 +549,30 @@
 response = ph.ask(prompt)
 
 # Extract and print the message from the response
 message = ph.get_message(response)
 print(message)
 ```
 ### 2. `YepChat` - Chat with mistral 8x7b powered by yepchat
-Thanks To Divyansh Shukla for This code
 ```python
-from webscout.AI import YepChat
+from webscout.AI import YEPCHAT
 
-def main():
-    # Initialize the YepChat class with your message
-    yep_chat = YepChat(message="who is pm of india")
-    
-    # Send the request and process the response
-    response = yep_chat.send_request()
-    processed_response = yep_chat.process_response(response)
-    
-    # Print the processed response
-    print(processed_response)
+# Instantiate the YEPCHAT class with default parameters
+YEPCHAT = YEPCHAT()
+
+# Define a prompt to send to the AI
+prompt = "What is the capital of France?"
+
+# Use the 'cha' method to get a response from the AI
+r = YEPCHAT.chat(prompt)
+print(r)
 
-if __name__ == "__main__":
-    main()
 ```
 
-### 3. `You.com` - search with you.com
+### 3. `You.com` - search with you.com -NOT WORKING
 ```python
 from webscout.AI import youChat
 
 # Instantiate the youchat class
 youChat = youChat()
 
 while True:
@@ -593,23 +590,42 @@
     except Exception as e:
         print("⚠️ An error occurred:", e)
 ```
 
 ### 4. `Gemini` - search with google gemini
 
 ```python
-from webscout.AI import Gemini
+import webscout
+from webscout.AI import GEMINI
+
+# Replace with the path to your bard.google.com.cookies.json file
+COOKIE_FILE = "path/to/bard.google.com.cookies.json"
+
+# Optional: Provide proxy details if needed
+PROXIES = {
+    "http": "http://proxy_server:port",
+    "https": "https://proxy_server:port",
+}
+
+# Initialize GEMINI with cookie file and optional proxies
+gemini = GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES)
+
+# Ask a question and print the response
+response = gemini.chat("What is the meaning of life?")
+print(response)
 
-# Create an instance of the Gemini class
-gemini = Gemini()
+# Ask another question, this time streaming the response
+for chunk in gemini.chat("Tell me a story", stream=True):
+    print(chunk, end="")
 
-# Use the chat method to send a message to the Gemini assistant
-response = gemini.chat("Your message here")
+# Reset the conversation to start a new interaction
+gemini.reset()
 
-# Print the response from the Gemini assistant
+# Ask a question with the code optimizer
+response = gemini.chat("Write Python code to print 'Hello, world!'", optimizer="code")
 print(response)
 ```
 ##  usage of image generator from Webscout.AI
 ### 5. `Prodia` - make image using prodia
 ```python
 from webscout.AI import Prodia
 
@@ -633,25 +649,26 @@
     update_file=True,
     proxies={},
     history_offset=10250,
     act=None,
     model=None # You can specify a model if needed
 )
 
-# Define a prompt to send to the AI
-prompt = "Tell me about india"
-
-# Use the 'ask' method to send the prompt and receive a response
-response = ai.ask(prompt)
-
-# Extract the text from the response
-response_text = ai.get_message(response)
-
-# Print the response text
-print(response_text)
+# Start an infinite loop for continuous interaction
+while True:
+    # Define a prompt to send to the AI
+    prompt = input("Enter your prompt: ")
+    
+    # Check if the user wants to exit the loop
+    if prompt.lower() == "exit":
+        break
+    
+    # Use the 'chat' method to send the prompt and receive a response
+    r = ai.chat(prompt)
+    print(r)
 ```
 ### 7. `PERPLEXITY` - Search With PERPLEXITY
 ```python
 from webscout.AI import PERPLEXITY
 # Create an instance of the PERPLEXITY class
 perplexity = PERPLEXITY()
 
@@ -661,18 +678,20 @@
 print(response)
 ```
 ### 8. `OpenGPT` - chat With OPENGPT
 ```python
 from webscout.AI import OPENGPT
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
-# This example sends a simple greeting and prints the response
-prompt = "tell me about india"
-response_str = opengpt.chat(prompt)
-print(response_str)
+while True:
+    # Prompt the user for input
+    prompt = input("Enter your prompt: ")
+    # Send the prompt to the OPENGPT model and print the response
+    response_str = opengpt.chat(prompt)
+    print(response_str)
 ```
 ### 9. `KOBOLDIA` - 
 ```python
 from webscout.AI import KOBOLDAI
 
 # Instantiate the KOBOLDAI class with default parameters
 koboldai = KOBOLDAI()
@@ -707,15 +726,15 @@
 a = Cohere(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
 
 prompt = "tell me about india"
 response_str = a.chat(prompt)
 print(response_str)
 ```
 
-### `LLM`
+### `LLM` --not working
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.3.9 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.0 Summary: Search for
 anything using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc
 Also containes AI models, can transcribe yt videos, have TTS support and now
 has webai(terminal gpt and open interpeter) support Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -21,16 +21,16 @@
 curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
 asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist:
-appdirsGoogleBard1>=2.1.4 Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
+Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
+Dist: GoogleBard1>=2.1.4 Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
 == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
        _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models, can
 transcribe yt videos, have TTS support and now has webai(terminal gpt and open
  interpeter) support ## Table of Contents - [webscout](#webscout) - [Table of
    Contents](#table-of-contents) - [Install](#install) - [CLI version](#cli-
      version) - [CLI to use LLM](#cli-to-use-llm) - [Regions](#regions) -
@@ -52,81 +52,81 @@
   duckduckgocom-and) - [7. `translate()` - translation by DuckDuckGo.com and
     Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom) - [8.
 `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---
  suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI](#usage-of-
   webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---
   search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b powered by
     yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) - [3.
-`You.com` - search with you.com](#3-youcom---search-with-youcom) - [4. `Gemini`
-- search with google gemini](#4-gemini---search-with-google-gemini) - [usage of
-image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai) -
-[5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia) -
-  [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-
-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-
- with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-
-  opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [10. `Reka` - chat with reka]
- (#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere](#11-cohere---
-chat-with-cohere) - [`LLM`](#llm) - [`LLM` with internet](#llm-with-internet) -
-  [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-
-   open-interpeter) ## Install ```python pip install -U webscout ``` ## CLI
-version ```python3 python -m webscout --help ``` | Command | Description | |---
-----------------------------------------|--------------------------------------
- -----------------------------------------------------------------| | python -
- m webscout answers -k Text | CLI function to perform an answers search using
- Webscout. | | python -m webscout images -k Text | CLI function to perform an
-    images search using Webscout. | | python -m webscout maps -k Text | CLI
-function to perform a maps search using Webscout. | | python -m webscout news -
-  k Text | CLI function to perform a news search using Webscout. | | python -
- m webscout suggestions -k Text | CLI function to perform a suggestions search
-using Webscout. | | python -m webscout text -k Text | CLI function to perform a
-  text search using Webscout. | | python -m webscout translate -k Text | CLI
-function to perform translate using Webscout. | | python -m webscout version |
-  A command-line interface command that prints and returns the version of the
-  program. | | python -m webscout videos -k Text | CLI function to perform a
-  videos search using DuckDuckGo API. | ## CLI to use LLM ```python python -
-  m webscout.LLM model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for
-Arabia xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for
- Austria be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg
-for Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
-  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
-     Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Transcriber The
-   transcriber function in webscout is a handy tool that transcribes YouTube
- videos. Here's an example code demonstrating its usage: ```python import sys
-from webscout import transcriber def extract_transcript(video_id): """Extracts
-        the transcript from a YouTube video.""" try: transcript_list =
-   transcriber.list_transcripts(video_id) for transcript in transcript_list:
-     transcript_data_list = transcript.fetch() lang = transcript.language
-     transcript_text = "" if transcript.language_code == 'en': for line in
- transcript_data_list: start_time = line['start'] end_time = start_time + line
-   ['duration'] formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line
-  ['text']}\n" transcript_text += formatted_line return transcript_text elif
-  transcript.is_translatable: english_transcript_list = transcript.translate
-('en').fetch() for line in english_transcript_list: start_time = line['start']
-end_time = start_time + line['duration'] formatted_line = f"{start_time:.2f} -
+`You.com` - search with you.com -NOT WORKING](#3-youcom---search-with-youcom--
+ not-working) - [4. `Gemini` - search with google gemini](#4-gemini---search-
+ with-google-gemini) - [usage of image generator from Webscout.AI](#usage-of-
+image-generator-from-webscoutai) - [5. `Prodia` - make image using prodia](#5-
+prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat With BlackBox]
+   (#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With
+PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With
+OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) -
+[10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat
+with cohere](#11-cohere---chat-with-cohere) - [`LLM` --not working](#llm---not-
+working) - [`LLM` with internet](#llm-with-internet) - [`Webai` - terminal gpt
+and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+  using DuckDuckGo API. | ## CLI to use LLM ```python python -m webscout.LLM
+ model_name ``` [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for
+Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria be-fr for
+ Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en
+ for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for
+ China co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for
+Denmark ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany
+ gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id
+for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it
+for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania
+ xl-es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+ To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
+tool that transcribes YouTube videos. Here's an example code demonstrating its
+       usage: ```python import sys from webscout import transcriber def
+    extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ transcript.language transcript_text = "" if transcript.language_code == 'en':
+    for line in transcript_data_list: start_time = line['start'] end_time =
+     start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
-  transcript_text print("Transcript extraction failed. Please check the video
-  URL.") except Exception as e: print(f"Error: {e}") def main(): video_url =
- input("Enter the video link: ") if video_url: video_id = video_url.split("=")
-  [1] print("Video URL:", video_url) submit = input("Press 'Enter' to get the
-   transcript or type 'exit' to quit: ") if submit == '': print("Extracting
-Transcript...") transcript = extract_transcript(video_id) print('Transcript:')
-                            print(transcript) print
+  transcript_text elif transcript.is_translatable: english_transcript_list =
+    transcript.translate('en').fetch() for line in english_transcript_list:
+      start_time = line['start'] end_time = start_time + line['duration']
+    formatted_line = f"{start_time:.2f} - {end_time:.2f}: {line['text']}\n"
+  transcript_text += formatted_line return transcript_text print("Transcript
+ extraction failed. Please check the video URL.") except Exception as e: print
+  (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
+ video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
+submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '': print("Extracting Transcript...") transcript =
+   extract_transcript(video_id) print('Transcript:') print(transcript) print
 ("__________________________________________________________________________________")
    elif submit.lower() == 'exit': print("Exiting...") sys.exit() else: print
  ("Invalid input. Please try again.") if __name__ == "__main__": main() ``` ##
 DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone feature designed to
  perform advanced web searches with enhanced capabilities. It is particularly
  powerful in extracting relevant information directly from webpages and Search
 engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which
@@ -262,109 +262,116 @@
      WEBS.suggestions("fly"): print(r) ``` ## usage of webscout.AI ### 1.
    `PhindSearch` - Search using Phind.com ```python from webscout.AI import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
- by yepchat Thanks To Divyansh Shukla for This code ```python from webscout.AI
-  import YepChat def main(): # Initialize the YepChat class with your message
-yep_chat = YepChat(message="who is pm of india") # Send the request and process
-     the response response = yep_chat.send_request() processed_response =
-   yep_chat.process_response(response) # Print the processed response print
- (processed_response) if __name__ == "__main__": main() ``` ### 3. `You.com` -
-search with you.com ```python from webscout.AI import youChat # Instantiate the
-   youchat class youChat = youChat() while True: # Ask the user for a prompt
-    prompt = input("ð¡ Enter a prompt (or type 'exit' to quit): ") # Exit
- condition if prompt.lower() == 'exit': break # Generate a completion based on
-the prompt try: completion = youChat.create(prompt) print("ð¬:", completion)
-    except Exception as e: print("â ï¸ An error occurred:", e) ``` ### 4.
-`Gemini` - search with google gemini ```python from webscout.AI import Gemini #
-Create an instance of the Gemini class gemini = Gemini() # Use the chat method
-to send a message to the Gemini assistant response = gemini.chat("Your message
- here") # Print the response from the Gemini assistant print(response) ``` ##
- usage of image generator from Webscout.AI ### 5. `Prodia` - make image using
-prodia ```python from webscout.AI import Prodia # Define a prompt for the image
- generation prompt = "A beautiful sunset over the ocean" # Use the prodia_cli
- method to generate an image based on the prompt Prodia.prodia_cli(prompt) ```
-### 6. `BlackBox` - Search/chat With BlackBox ```python from webscout.AI import
-   BLACKBOXAI from rich import print ai = BLACKBOXAI( is_conversation=True,
-   max_tokens=800, timeout=30, intro=None, filepath=None, update_file=True,
-  proxies={}, history_offset=10250, act=None, model=None # You can specify a
- model if needed ) # Define a prompt to send to the AI prompt = "Tell me about
-    india" # Use the 'ask' method to send the prompt and receive a response
-response = ai.ask(prompt) # Extract the text from the response response_text =
-ai.get_message(response) # Print the response text print(response_text) ``` ###
-  7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
-PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
-   () # Example usage: prompt = "Explain the concept of recursion in simple
-terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
-- chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
-  (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
-    simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
-  ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
-with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
- AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
- response from the AI response = koboldai.ask(prompt) # Extract and print the
-   message from the response message = koboldai.get_message(response) print
-(message) ``` ### 10. `Reka` - chat with reka ```python from webscout.AI import
-  REKA a = REKA(is_conversation=True, max_tokens=8000, timeout=30,api_key="")
-      prompt = "tell me about india" response_str = a.chat(prompt) print
-     (response_str) ``` ### 11. `Cohere` - chat with cohere ```python from
-  webscout.AI import Cohere a = Cohere(is_conversation=True, max_tokens=8000,
-  timeout=30,api_key="") prompt = "tell me about india" response_str = a.chat
- (prompt) print(response_str) ``` ### `LLM` ```python from webscout.LLM import
-  LLM # Read the system message from the file with open('system.txt', 'r') as
- file: system_message = file.read() # Initialize the LLM class with the model
-     name and system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
- system_message=system_message) while True: # Get the user input user_input =
-input("User: ") # Define the messages to be sent messages = [ {"role": "user",
-  "content": user_input} ] # Use the mistral_chat method to get the response
-response = llm.chat(messages) # Print the response print("AI: ", response) ```
-   ### `LLM` with internet ```python from __future__ import annotations from
-typing import List, Optional from webscout import LLM from webscout import WEBS
-import warnings system_message: str = ( "As AI, you possess internet access and
- are capable of executing real-time web searches based on user inputs. " "You
-shall utilize this capability to enrich conversations, offer informed insights,
-  and augment your ability to " "respond accurately and thoroughly. However,
-    refrain from stating 'You have provided a list of strings,' ensuring "
- "seamless interactions with users. Embrace a responsive demeanor, harnessing
-available online resources to address " "queries, share pertinent content, and
-   facilitate meaningful exchanges. By doing so, you create value through "
-"connection and engagement, ultimately enhancing overall user satisfaction and
-  experience. Additionally, " "continue upholding the principles of respect,
-  impartiality, and intellectual integrity throughout all interactions." ) #
-       Ignore the specific UserWarning warnings.filterwarnings("ignore",
-      category=UserWarning, module="curl_cffi.aio", lineno=205) LLM = LLM
- (model="meta-llama/Meta-Llama-3-70B-Instruct", system_message=system_message)
-  def chat( user_input: str, webs: WEBS, max_results: int = 10 ) -> Optional
- [str]: """ Chat function to perform a web search based on the user input and
-generate a response using the LLM model. Parameters ---------- user_input : str
-    The user input to be used for the web search webs : WEBS The web search
-   instance to be used to perform the search max_results : int, optional The
-  maximum number of search results to include in the response, by default 10
-Returns ------- Optional[str] The response generated by the LLM model, or None
-  if there is no response """ # Perform a web search based on the user input
-search_results: List[str] = [] for r in webs.text( user_input, region="wt-wt",
-          safesearch="off", timelimit="y", max_results=max_results ):
- search_results.append(str(r)) # Convert each result to a string # Define the
-   messages to be sent, including the user input, search results, and system
-message messages = [ {"role": "user", "content": user_input + "\n" + "websearch
-results are:" + "\n".join(search_results)}, ] # Use the chat method to get the
-     response response = LLM.chat(messages) return response if __name__ ==
-  "__main__": while True: # Get the user input user_input = input("User: ") #
- Perform a web search based on the user input with WEBS() as webs: response =
-chat(user_input, webs) # Print the response if response: print("AI:", response)
-else: print("No response") ``` ## `Webai` - terminal gpt and a open interpeter
- ```python from webscout.webai import Main def use_rawdog_with_webai(prompt):
-    """ Wrap the webscout default method in a try-except block to catch any
-  unhandled exceptions and print a helpful message. """ try: webai_bot = Main
-  ( max_tokens=500, provider="cohere", temperature=0.7, top_k=40, top_p=0.95,
-model="command-r-plus", # Replace with your desired model auth=None, # Replace
-  with your auth key/value (if needed) timeout=30, disable_conversation=True,
-filepath=None, update_file=True, intro=None, rawdog=True, history_offset=10250,
-      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
-webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
-     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
-use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
-                        --provider "phind" --rawdog ```
+by yepchat ```python from webscout.AI import YEPCHAT # Instantiate the YEPCHAT
+class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
+the AI prompt = "What is the capital of France?" # Use the 'cha' method to get
+a response from the AI r = YEPCHAT.chat(prompt) print(r) ``` ### 3. `You.com` -
+ search with you.com -NOT WORKING ```python from webscout.AI import youChat #
+ Instantiate the youchat class youChat = youChat() while True: # Ask the user
+for a prompt prompt = input("ð¡ Enter a prompt (or type 'exit' to quit): ") #
+Exit condition if prompt.lower() == 'exit': break # Generate a completion based
+     on the prompt try: completion = youChat.create(prompt) print("ð¬:",
+ completion) except Exception as e: print("â ï¸ An error occurred:", e) ```
+  ### 4. `Gemini` - search with google gemini ```python import webscout from
+           webscout.AI import GEMINI # Replace with the path to your
+           bard.google.com.cookies.json file COOKIE_FILE = "path/to/
+   bard.google.com.cookies.json" # Optional: Provide proxy details if needed
+PROXIES = { "http": "http://proxy_server:port", "https": "https://proxy_server:
+  port", } # Initialize GEMINI with cookie file and optional proxies gemini =
+ GEMINI(cookie_file=COOKIE_FILE, proxy=PROXIES) # Ask a question and print the
+response response = gemini.chat("What is the meaning of life?") print(response)
+     # Ask another question, this time streaming the response for chunk in
+ gemini.chat("Tell me a story", stream=True): print(chunk, end="") # Reset the
+ conversation to start a new interaction gemini.reset() # Ask a question with
+ the code optimizer response = gemini.chat("Write Python code to print 'Hello,
+  world!'", optimizer="code") print(response) ``` ## usage of image generator
+   from Webscout.AI ### 5. `Prodia` - make image using prodia ```python from
+ webscout.AI import Prodia # Define a prompt for the image generation prompt =
+"A beautiful sunset over the ocean" # Use the prodia_cli method to generate an
+  image based on the prompt Prodia.prodia_cli(prompt) ``` ### 6. `BlackBox` -
+  Search/chat With BlackBox ```python from webscout.AI import BLACKBOXAI from
+   rich import print ai = BLACKBOXAI( is_conversation=True, max_tokens=800,
+     timeout=30, intro=None, filepath=None, update_file=True, proxies={},
+history_offset=10250, act=None, model=None # You can specify a model if needed
+ ) # Start an infinite loop for continuous interaction while True: # Define a
+ prompt to send to the AI prompt = input("Enter your prompt: ") # Check if the
+user wants to exit the loop if prompt.lower() == "exit": break # Use the 'chat'
+ method to send the prompt and receive a response r = ai.chat(prompt) print(r)
+  ``` ### 7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI
+  import PERPLEXITY # Create an instance of the PERPLEXITY class perplexity =
+  PERPLEXITY() # Example usage: prompt = "Explain the concept of recursion in
+ simple terms." response = perplexity.chat(prompt) print(response) ``` ### 8.
+`OpenGPT` - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt
+  = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30) while True: #
+  Prompt the user for input prompt = input("Enter your prompt: ") # Send the
+prompt to the OPENGPT model and print the response response_str = opengpt.chat
+(prompt) print(response_str) ``` ### 9. `KOBOLDIA` - ```python from webscout.AI
+   import KOBOLDAI # Instantiate the KOBOLDAI class with default parameters
+koboldai = KOBOLDAI() # Define a prompt to send to the AI prompt = "What is the
+   capital of France?" # Use the 'ask' method to get a response from the AI
+   response = koboldai.ask(prompt) # Extract and print the message from the
+ response message = koboldai.get_message(response) print(message) ``` ### 10.
+    `Reka` - chat with reka ```python from webscout.AI import REKA a = REKA
+ (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
+ me about india" response_str = a.chat(prompt) print(response_str) ``` ### 11.
+`Cohere` - chat with cohere ```python from webscout.AI import Cohere a = Cohere
+ (is_conversation=True, max_tokens=8000, timeout=30,api_key="") prompt = "tell
+me about india" response_str = a.chat(prompt) print(response_str) ``` ### `LLM`
+--not working ```python from webscout.LLM import LLM # Read the system message
+from the file with open('system.txt', 'r') as file: system_message = file.read
+() # Initialize the LLM class with the model name and system message llm = LLM
+(model="microsoft/WizardLM-2-8x22B", system_message=system_message) while True:
+ # Get the user input user_input = input("User: ") # Define the messages to be
+     sent messages = [ {"role": "user", "content": user_input} ] # Use the
+ mistral_chat method to get the response response = llm.chat(messages) # Print
+the response print("AI: ", response) ``` ### `LLM` with internet ```python from
+ __future__ import annotations from typing import List, Optional from webscout
+  import LLM from webscout import WEBS import warnings system_message: str =
+ ( "As AI, you possess internet access and are capable of executing real-time
+  web searches based on user inputs. " "You shall utilize this capability to
+ enrich conversations, offer informed insights, and augment your ability to "
+  "respond accurately and thoroughly. However, refrain from stating 'You have
+  provided a list of strings,' ensuring " "seamless interactions with users.
+Embrace a responsive demeanor, harnessing available online resources to address
+ " "queries, share pertinent content, and facilitate meaningful exchanges. By
+  doing so, you create value through " "connection and engagement, ultimately
+ enhancing overall user satisfaction and experience. Additionally, " "continue
+ upholding the principles of respect, impartiality, and intellectual integrity
+       throughout all interactions." ) # Ignore the specific UserWarning
+warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffi.aio",
+      lineno=205) LLM = LLM(model="meta-llama/Meta-Llama-3-70B-Instruct",
+     system_message=system_message) def chat( user_input: str, webs: WEBS,
+ max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
+  search based on the user input and generate a response using the LLM model.
+ Parameters ---------- user_input : str The user input to be used for the web
+  search webs : WEBS The web search instance to be used to perform the search
+max_results : int, optional The maximum number of search results to include in
+    the response, by default 10 Returns ------- Optional[str] The response
+generated by the LLM model, or None if there is no response """ # Perform a web
+    search based on the user input search_results: List[str] = [] for r in
+    webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
+max_results=max_results ): search_results.append(str(r)) # Convert each result
+to a string # Define the messages to be sent, including the user input, search
+results, and system message messages = [ {"role": "user", "content": user_input
+  + "\n" + "websearch results are:" + "\n".join(search_results)}, ] # Use the
+ chat method to get the response response = LLM.chat(messages) return response
+if __name__ == "__main__": while True: # Get the user input user_input = input
+("User: ") # Perform a web search based on the user input with WEBS() as webs:
+response = chat(user_input, webs) # Print the response if response: print("AI:
+  ", response) else: print("No response") ``` ## `Webai` - terminal gpt and a
+         open interpeter ```python from webscout.webai import Main def
+ use_rawdog_with_webai(prompt): """ Wrap the webscout default method in a try-
+except block to catch any unhandled exceptions and print a helpful message. """
+  try: webai_bot = Main( max_tokens=500, provider="cohere", temperature=0.7,
+top_k=40, top_p=0.95, model="command-r-plus", # Replace with your desired model
+     auth=None, # Replace with your auth key/value (if needed) timeout=30,
+    disable_conversation=True, filepath=None, update_file=True, intro=None,
+   rawdog=True, history_offset=10250, awesome_prompt=None, proxy_path=None,
+quiet=True ) webai_response = webai_bot.default(prompt) except Exception as e:
+ print("Unexpected error:", e) if __name__ == "__main__": user_prompt = input
+("Enter your prompt: ") use_rawdog_with_webai(user_prompt) ``` ```shell python
+            -m webscout.webai webai --provider "phind" --rawdog ```
```

### Comparing `webscout-1.3.9/webscout.egg-info/SOURCES.txt` & `webscout-1.4.0/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

