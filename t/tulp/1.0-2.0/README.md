# Comparing `tmp/tulp-1.0.tar.gz` & `tmp/tulp-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulp-1.0.tar", last modified: Wed Feb 14 16:19:40 2024, max compression
+gzip compressed data, was "tulp-2.0.tar", last modified: Fri May  3 22:26:57 2024, max compression
```

## Comparing `tulp-1.0.tar` & `tulp-2.0.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-02-14 16:19:40.914121 tulp-1.0/
--rw-rw-r--   0 fede      (1000) fede      (1000)      684 2024-02-14 15:35:47.000000 tulp-1.0/LICENSE
--rw-r--r--   0 fede      (1000) fede      (1000)     8895 2024-02-14 16:19:40.914121 tulp-1.0/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)     8273 2024-02-14 16:19:30.000000 tulp-1.0/README.md
--rw-rw-r--   0 fede      (1000) fede      (1000)      899 2024-02-14 16:19:40.918121 tulp-1.0/setup.cfg
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-02-14 15:35:47.000000 tulp-1.0/setup.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-02-14 16:19:40.914121 tulp-1.0/test/
--rw-rw-r--   0 fede      (1000) fede      (1000)     2680 2024-02-14 15:35:47.000000 tulp-1.0/test/test_filterMode_advanced.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3621 2024-02-14 15:35:47.000000 tulp-1.0/test/test_filterMode_basic.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1342 2024-02-14 15:35:47.000000 tulp-1.0/test/test_requestMode.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1066 2024-02-14 15:35:47.000000 tulp-1.0/test/test_slowtest.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-02-14 16:19:40.914121 tulp-1.0/tulp/
--rw-rw-r--   0 fede      (1000) fede      (1000)     1378 2024-02-14 15:35:47.000000 tulp-1.0/tulp/TulpOutputFileWriter.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      111 2024-02-14 15:35:47.000000 tulp-1.0/tulp/__init__.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1864 2024-02-14 15:35:47.000000 tulp-1.0/tulp/createFilteringProgramPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1443 2024-02-14 15:35:47.000000 tulp-1.0/tulp/createProgramPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)      389 2024-02-14 15:35:47.000000 tulp-1.0/tulp/executePython.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     4940 2024-02-14 15:35:47.000000 tulp-1.0/tulp/filteringPrompt.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     3841 2024-02-14 15:35:47.000000 tulp-1.0/tulp/requestPrompt.py
--rwxrwxr-x   0 fede      (1000) fede      (1000)    12332 2024-02-14 16:17:10.000000 tulp-1.0/tulp/tulp.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1968 2024-02-14 15:39:58.000000 tulp-1.0/tulp/tulpargs.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1058 2024-02-14 15:39:11.000000 tulp-1.0/tulp/tulpconfig.py
--rw-rw-r--   0 fede      (1000) fede      (1000)     1722 2024-02-14 15:35:47.000000 tulp-1.0/tulp/tulplogger.py
--rw-rw-r--   0 fede      (1000) fede      (1000)       16 2024-02-14 16:00:53.000000 tulp-1.0/tulp/version.py
-drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-02-14 16:19:40.914121 tulp-1.0/tulp.egg-info/
--rw-r--r--   0 fede      (1000) fede      (1000)     8895 2024-02-14 16:19:40.000000 tulp-1.0/tulp.egg-info/PKG-INFO
--rw-rw-r--   0 fede      (1000) fede      (1000)      602 2024-02-14 16:19:40.000000 tulp-1.0/tulp.egg-info/SOURCES.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-02-14 16:19:40.000000 tulp-1.0/tulp.egg-info/dependency_links.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-02-14 16:19:40.000000 tulp-1.0/tulp.egg-info/entry_points.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)       14 2024-02-14 16:19:40.000000 tulp-1.0/tulp.egg-info/requires.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        5 2024-02-14 16:19:40.000000 tulp-1.0/tulp.egg-info/top_level.txt
--rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-02-14 15:41:21.000000 tulp-1.0/tulp.egg-info/zip-safe
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.607448 tulp-2.0/
+-rw-rw-r--   0 fede      (1000) fede      (1000)      684 2024-02-14 15:35:47.000000 tulp-2.0/LICENSE
+-rw-r--r--   0 fede      (1000) fede      (1000)    11330 2024-05-03 22:26:57.607448 tulp-2.0/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)    10567 2024-05-03 22:26:20.000000 tulp-2.0/README.md
+-rw-rw-r--   0 fede      (1000) fede      (1000)      990 2024-05-03 22:26:57.611448 tulp-2.0/setup.cfg
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-02-14 15:35:47.000000 tulp-2.0/setup.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.595448 tulp-2.0/test/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2847 2024-05-03 22:26:20.000000 tulp-2.0/test/test_filterMode_advanced.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3621 2024-02-14 15:35:47.000000 tulp-2.0/test/test_filterMode_basic.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1342 2024-02-14 15:35:47.000000 tulp-2.0/test/test_requestMode.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1066 2024-02-14 15:35:47.000000 tulp-2.0/test/test_slowtest.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.599448 tulp-2.0/tulp/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1378 2024-05-02 13:40:36.000000 tulp-2.0/tulp/TulpOutputFileWriter.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      111 2024-02-14 15:35:47.000000 tulp-2.0/tulp/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1864 2024-02-14 15:35:47.000000 tulp-2.0/tulp/createFilteringProgramPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1443 2024-02-14 15:35:47.000000 tulp-2.0/tulp/createProgramPrompt.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)      389 2024-02-14 15:35:47.000000 tulp-2.0/tulp/executePython.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     4939 2024-05-03 22:26:20.000000 tulp-2.0/tulp/filteringPrompt.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.607448 tulp-2.0/tulp/llms/
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3431 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmAnthropic.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3167 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmGemini.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3431 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmGroq.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3141 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmOllama.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2061 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/LlmOpenAI.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1616 2024-05-03 22:26:20.000000 tulp-2.0/tulp/llms/__init__.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     3678 2024-05-03 22:26:20.000000 tulp-2.0/tulp/requestPrompt.py
+-rwxrwxr-x   0 fede      (1000) fede      (1000)    11917 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulp.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     2387 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulpargs.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1381 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulpconfig.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)     1935 2024-05-03 22:26:20.000000 tulp-2.0/tulp/tulplogger.py
+-rw-rw-r--   0 fede      (1000) fede      (1000)       16 2024-05-03 22:26:20.000000 tulp-2.0/tulp/version.py
+drwxrwxr-x   0 fede      (1000) fede      (1000)        0 2024-05-03 22:26:57.607448 tulp-2.0/tulp.egg-info/
+-rw-r--r--   0 fede      (1000) fede      (1000)    11330 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/PKG-INFO
+-rw-rw-r--   0 fede      (1000) fede      (1000)      740 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/SOURCES.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/dependency_links.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       39 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/entry_points.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)       95 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/requires.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        5 2024-05-03 22:26:57.000000 tulp-2.0/tulp.egg-info/top_level.txt
+-rw-rw-r--   0 fede      (1000) fede      (1000)        1 2024-02-14 15:41:21.000000 tulp-2.0/tulp.egg-info/zip-safe
```

### Comparing `tulp-1.0/LICENSE` & `tulp-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tulp-1.0/PKG-INFO` & `tulp-2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 1.0
+Version: 2.0
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai>=1.0.0
+Requires-Dist: openai==1.25.1
+Requires-Dist: google-ai-generativelanguage==0.6.2
+Requires-Dist: anthropic==0.25.7
+Requires-Dist: groq==0.5.0
+Requires-Dist: ollama==0.1.9
 
-# TULP: TULP Understands Language Promptly
+# TULP: TULP Understands Language Promptly | v2.0 
 
-A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, backed by chatGPT.
+A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with enhanced capabilities to utilize various AI APIs including groq, ollama, anthropic, and gemini.
 
-TULP allows you to harness the power of chatGPT by piping standard input content directly to chatGPT, getting the answer back on the shell.
+TULP allows you to harness the power of multiple AI models by piping standard input content directly to these models, getting the answer back on the shell.
 
 [![tulp demo video](https://markdown-videos.deta.dev/youtube/mHAvlRXXp6I)](https://www.youtube.com/watch?v=mHAvlRXXp6I)
 
 ## Installation:
 
 ```bash
 pip install tulp
@@ -43,80 +47,127 @@
 ```
 cat examples/titanics.csv | tulp -x how many persons survived
 ```
 
 
 In both cases, TULP will write to the standard output the answers and will write any other information to the standard error. You can safely pipe the output to your file or next piping command and will still get all the information and errors on stderr.
 
-It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by chatGPT in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
+It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by the selected AI model in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
 
-By default, tulp uses **gpt-3.5-turbo**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to force the gpt-4 model**: tulp --model gpt-4 {a complex task}
+By default, tulp uses **gpt-4-0125-preview**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
 
 ### Options:
 ```
-usage: tulp [-h] [-x] [-w W] [--model {gpt-3.5-turbo,gpt-4}] [--max-chars MAX_CHARS] [-v] [-q] ...
+usage: tulp [-h] [-x] [-w W] [--model MODEL] [--max-chars MAX_CHARS] [-v] [-q] [--groq_api_key GROQ_API_KEY] [--ollama_host OLLAMA_HOST] [--anthropic_api_key ANTHROPIC_API_KEY] [--openai_api_key OPENAI_API_KEY] [--openai_baseurl OPENAI_BASEURL] [--gemini_api_key GEMINI_API_KEY] ...
 
-TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, backed by chatGPT.
+TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with support for multiple AI APIs including groq, ollama, anthropic, and gemini.
 
 positional arguments:
   request               User request, instructions written in natural language
 
 optional arguments:
   -h, --help            show this help message and exit
   -x                    Allow tulp to create a program and execute it to fulfill the task (code interpret)
   -w W                  Write the output (or the created program for execution) to the file. If the file exists, a backup will be created before overwriting it.
-  --model {gpt-3.5-turbo,gpt-4}
-                        Select the LLM model to use, currently gpt-3.5-turbo or gpt-4
+  --model MODEL         Select the AI LLM model to use, now supporting groq.*, ollama.*, claude-.*, gpt-.*, and gemini.* models
   --max-chars MAX_CHARS
                         Number of chars per message chunk per request
   -v                    Be verbose!
   -q                    Be quiet! Only print the answer and errors.
+  --groq_api_key GROQ_API_KEY
+                        GROQ cloud API KEY
+  --ollama_host OLLAMA_HOST
+                        Define custom ollama host
+  --anthropic_api_key ANTHROPIC_API_KEY
+                        Anthropic api key
+  --openai_api_key OPENAI_API_KEY
+                        OpenAI cloud API KEY
+  --openai_baseurl OPENAI_BASEURL
+                        Use it to change the server, e.g.: use http://localhost:11434/v1/ to connect to your local ollama server
+  --gemini_api_key GEMINI_API_KEY
+                        gemini cloud API KEY
 
 ```
 
-
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. 
 
 The following are the parameters that can be configured:
 - **LOG_LEVEL**: The log level of Tulp. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
-- **OPENAI_API_KEY**: The API key for OpenAI. The default value is an empty string.
-- **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 5000.
-- **MODEL**: The OpenAI model to be used by Tulp. The default value is gpt-3.5-turbo, but gpt-4 is also available.
+- **API_KEYS**: The API keys for the supported AI models (OpenAI, GROQ, Ollama, Anthropic, Gemini). The default value is an empty string for each.
+- **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 40000.
+- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4-0125-preview, but other models are also available.
 
 All these settings could be overridden by an environment variable using the prefix TULP\_ or by the different command line arguments described above. 
-As environment variables, they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_MAX_CHARS, or TULP_MODEL.
+As environment variables, they will become: TULP_LOG_LEVEL, TULP_API_KEYS, TULP_MAX_CHARS, or TULP_MODEL.
 Command line arguments will override environmental variables and the configuration file.
 
 
 Here is an example configuration file with the default values:
 ```INI
 [DEFAULT]
 LOG_LEVEL = INFO
-OPENAI_API_KEY = <<<YOUR API KEY >>>>
-MAX_CHARS = 10000
-MODEL = gpt-3.5-turbo
+${MODEL}_API_KEYS = <<<YOUR API KEYS FOR GROQ, OLLAMA, ANTHROPIC, OPENAI, GEMINI>>>
+MAX_CHARS = 40000
+MODEL = gpt-4-0125-preview
 ```
+
+
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspiration:
 
 ### Random
+#### The meaning of life for different models:
+
+```
++ tulp -q --model gpt-4-turbo tell me the meaning of life in just 3 words
+42, not known
+
+
++ tulp -q --model gpt-3.5-turbo tell me the meaning of life in just 3 words
+Live, love, learn.
+
++ tulp -q --model claude-3-opus-20240229 tell me the meaning of life in just 3 words
+Love conquers all.
+
++ tulp -q --model gemini-1.5-pro-latest tell me the meaning of life in just 3 words
+The answer is 42.
+
++ tulp -q --model groq.gemma-7b-it tell me the meaning of life in just 3 words
+The meaning of life is to find purpose and fulfillment in the present moment.
+
+
++ tulp -q --model groq.llama3-70b-8192 tell me the meaning of life in just 3 words
+Find Your Purpose
+
++ tulp -q --model groq.mixtral-8x7b-32768 tell me the meaning of life in just 3 words
+Impossible task.
+
++ tulp -q --model ollama.phi3:instruct tell me the meaning of life in just 3 words
+echo "Meaning of Life"
+```
+
 #### Create a plot directly from raw memory output printed by gdb:
 Command:
 ```bash
 cat <<EOF | tulp convert this to a python list of 2 element tuples |  tulp write a python function to scatter plot these points using matplotlib | python 
 (gdb) p *polygon._points._M_ptr._M_impl._M_start@4
 $21 = {{x = 0.441429973, y = -0.176619753}, {x = 0.476210177, y = -0.104575738}, {x = 0.674865067, y = -0.0814191923}, {x = 0.640084863, y = -0.199776307}}
 EOF
 ```
 
 Result:
 
 ![matplotlib @rela](./examples/rela_plot.png)
 
+### Grammatical and Syntax Correction of Clipboard Content in Linux (The Corrected Version Will Be in the Clipboard)
+
+```bash
+xsel -b | tulp fix my english | xsel -b
+```
 
 
 ### Typical Unix tooling replacement:
 #### Sed
 ```bash
 cat README.md | tulp replace all the occurrences of TULP for **TULP**
 ```
@@ -208,17 +259,22 @@
 ```
 
 # Why?
 
 I am a heavy user of Unix tooling (e.g: awk, jq, sed, grep, and so on), I have been using them since my early days and I used to think that I couldn't survive without them. But then, ChatGPT appeared, and I started to use more and more GPT for things that I used to use Unix tooling for. Somehow I feel the pain of cut & paste, and I was missing a way to do it faster and from within the terminal itself, so I came up with `tulp`.
 
 # Changelog
+## v2.0 | 2024-05-04
+- Added support for groq, ollama, anthropic, and gemini AI models.
+- Changed to use gpt-4-turbo model by default
+
 ## v1.0 | 2024-02-14
 - Changed to use gpt-4-0125-preview model by default
 - Updated to use openapi v1.0
 - Changes default max-chars to 40000
 
-## v07  | 2023-05-23 
+## v0.7  | 2023-05-23 
 - Adds Code Interpretation, -x option
 ## v0.6 | 2023-05-11
 - Adds all the settings as command line arguments
 
+
```

### Comparing `tulp-1.0/README.md` & `tulp-2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# TULP: TULP Understands Language Promptly
+# TULP: TULP Understands Language Promptly | v2.0 
 
-A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, backed by chatGPT.
+A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with enhanced capabilities to utilize various AI APIs including groq, ollama, anthropic, and gemini.
 
-TULP allows you to harness the power of chatGPT by piping standard input content directly to chatGPT, getting the answer back on the shell.
+TULP allows you to harness the power of multiple AI models by piping standard input content directly to these models, getting the answer back on the shell.
 
 [![tulp demo video](https://markdown-videos.deta.dev/youtube/mHAvlRXXp6I)](https://www.youtube.com/watch?v=mHAvlRXXp6I)
 
 ## Installation:
 
 ```bash
 pip install tulp
@@ -28,80 +28,127 @@
 ```
 cat examples/titanics.csv | tulp -x how many persons survived
 ```
 
 
 In both cases, TULP will write to the standard output the answers and will write any other information to the standard error. You can safely pipe the output to your file or next piping command and will still get all the information and errors on stderr.
 
-It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by chatGPT in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
+It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by the selected AI model in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
 
-By default, tulp uses **gpt-3.5-turbo**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to force the gpt-4 model**: tulp --model gpt-4 {a complex task}
+By default, tulp uses **gpt-4-0125-preview**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
 
 ### Options:
 ```
-usage: tulp [-h] [-x] [-w W] [--model {gpt-3.5-turbo,gpt-4}] [--max-chars MAX_CHARS] [-v] [-q] ...
+usage: tulp [-h] [-x] [-w W] [--model MODEL] [--max-chars MAX_CHARS] [-v] [-q] [--groq_api_key GROQ_API_KEY] [--ollama_host OLLAMA_HOST] [--anthropic_api_key ANTHROPIC_API_KEY] [--openai_api_key OPENAI_API_KEY] [--openai_baseurl OPENAI_BASEURL] [--gemini_api_key GEMINI_API_KEY] ...
 
-TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, backed by chatGPT.
+TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with support for multiple AI APIs including groq, ollama, anthropic, and gemini.
 
 positional arguments:
   request               User request, instructions written in natural language
 
 optional arguments:
   -h, --help            show this help message and exit
   -x                    Allow tulp to create a program and execute it to fulfill the task (code interpret)
   -w W                  Write the output (or the created program for execution) to the file. If the file exists, a backup will be created before overwriting it.
-  --model {gpt-3.5-turbo,gpt-4}
-                        Select the LLM model to use, currently gpt-3.5-turbo or gpt-4
+  --model MODEL         Select the AI LLM model to use, now supporting groq.*, ollama.*, claude-.*, gpt-.*, and gemini.* models
   --max-chars MAX_CHARS
                         Number of chars per message chunk per request
   -v                    Be verbose!
   -q                    Be quiet! Only print the answer and errors.
+  --groq_api_key GROQ_API_KEY
+                        GROQ cloud API KEY
+  --ollama_host OLLAMA_HOST
+                        Define custom ollama host
+  --anthropic_api_key ANTHROPIC_API_KEY
+                        Anthropic api key
+  --openai_api_key OPENAI_API_KEY
+                        OpenAI cloud API KEY
+  --openai_baseurl OPENAI_BASEURL
+                        Use it to change the server, e.g.: use http://localhost:11434/v1/ to connect to your local ollama server
+  --gemini_api_key GEMINI_API_KEY
+                        gemini cloud API KEY
 
 ```
 
-
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. 
 
 The following are the parameters that can be configured:
 - **LOG_LEVEL**: The log level of Tulp. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
-- **OPENAI_API_KEY**: The API key for OpenAI. The default value is an empty string.
-- **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 5000.
-- **MODEL**: The OpenAI model to be used by Tulp. The default value is gpt-3.5-turbo, but gpt-4 is also available.
+- **API_KEYS**: The API keys for the supported AI models (OpenAI, GROQ, Ollama, Anthropic, Gemini). The default value is an empty string for each.
+- **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 40000.
+- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4-0125-preview, but other models are also available.
 
 All these settings could be overridden by an environment variable using the prefix TULP\_ or by the different command line arguments described above. 
-As environment variables, they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_MAX_CHARS, or TULP_MODEL.
+As environment variables, they will become: TULP_LOG_LEVEL, TULP_API_KEYS, TULP_MAX_CHARS, or TULP_MODEL.
 Command line arguments will override environmental variables and the configuration file.
 
 
 Here is an example configuration file with the default values:
 ```INI
 [DEFAULT]
 LOG_LEVEL = INFO
-OPENAI_API_KEY = <<<YOUR API KEY >>>>
-MAX_CHARS = 10000
-MODEL = gpt-3.5-turbo
+${MODEL}_API_KEYS = <<<YOUR API KEYS FOR GROQ, OLLAMA, ANTHROPIC, OPENAI, GEMINI>>>
+MAX_CHARS = 40000
+MODEL = gpt-4-0125-preview
 ```
+
+
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspiration:
 
 ### Random
+#### The meaning of life for different models:
+
+```
++ tulp -q --model gpt-4-turbo tell me the meaning of life in just 3 words
+42, not known
+
+
++ tulp -q --model gpt-3.5-turbo tell me the meaning of life in just 3 words
+Live, love, learn.
+
++ tulp -q --model claude-3-opus-20240229 tell me the meaning of life in just 3 words
+Love conquers all.
+
++ tulp -q --model gemini-1.5-pro-latest tell me the meaning of life in just 3 words
+The answer is 42.
+
++ tulp -q --model groq.gemma-7b-it tell me the meaning of life in just 3 words
+The meaning of life is to find purpose and fulfillment in the present moment.
+
+
++ tulp -q --model groq.llama3-70b-8192 tell me the meaning of life in just 3 words
+Find Your Purpose
+
++ tulp -q --model groq.mixtral-8x7b-32768 tell me the meaning of life in just 3 words
+Impossible task.
+
++ tulp -q --model ollama.phi3:instruct tell me the meaning of life in just 3 words
+echo "Meaning of Life"
+```
+
 #### Create a plot directly from raw memory output printed by gdb:
 Command:
 ```bash
 cat <<EOF | tulp convert this to a python list of 2 element tuples |  tulp write a python function to scatter plot these points using matplotlib | python 
 (gdb) p *polygon._points._M_ptr._M_impl._M_start@4
 $21 = {{x = 0.441429973, y = -0.176619753}, {x = 0.476210177, y = -0.104575738}, {x = 0.674865067, y = -0.0814191923}, {x = 0.640084863, y = -0.199776307}}
 EOF
 ```
 
 Result:
 
 ![matplotlib @rela](./examples/rela_plot.png)
 
+### Grammatical and Syntax Correction of Clipboard Content in Linux (The Corrected Version Will Be in the Clipboard)
+
+```bash
+xsel -b | tulp fix my english | xsel -b
+```
 
 
 ### Typical Unix tooling replacement:
 #### Sed
 ```bash
 cat README.md | tulp replace all the occurrences of TULP for **TULP**
 ```
@@ -193,17 +240,22 @@
 ```
 
 # Why?
 
 I am a heavy user of Unix tooling (e.g: awk, jq, sed, grep, and so on), I have been using them since my early days and I used to think that I couldn't survive without them. But then, ChatGPT appeared, and I started to use more and more GPT for things that I used to use Unix tooling for. Somehow I feel the pain of cut & paste, and I was missing a way to do it faster and from within the terminal itself, so I came up with `tulp`.
 
 # Changelog
+## v2.0 | 2024-05-04
+- Added support for groq, ollama, anthropic, and gemini AI models.
+- Changed to use gpt-4-turbo model by default
+
 ## v1.0 | 2024-02-14
 - Changed to use gpt-4-0125-preview model by default
 - Updated to use openapi v1.0
 - Changes default max-chars to 40000
 
-## v07  | 2023-05-23 
+## v0.7  | 2023-05-23 
 - Adds Code Interpretation, -x option
 ## v0.6 | 2023-05-11
 - Adds all the settings as command line arguments
 
+
```

### Comparing `tulp-1.0/setup.cfg` & `tulp-2.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 [options]
 packages = find:
 python_requires = >=3.7.1
 zip_safe = True
 include_package_data = True
 install_requires = 
-	openai >= 1.0.0
+	openai==1.25.1
+	google-ai-generativelanguage == 0.6.2
+	anthropic == 0.25.7
+	groq == 0.5.0
+	ollama == 0.1.9
 
 [options.entry_points]
 console_scripts = 
 	tulp = tulp.tulp:run
 
 [options.packages.find]
 exclude =
```

### Comparing `tulp-1.0/test/test_filterMode_advanced.py` & `tulp-2.0/test/test_filterMode_advanced.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,20 +42,23 @@
     assert "PASSED" in res
 
 
 def test_filter_process_gdb_output():
     INPUT="""(gdb) p *polygon._points._M_ptr._M_impl._M_start@4
 $21 = {{x = 0.441429973, y = -0.176619753}, {x = 0.476210177, y = -0.104575738}, {x = 0.674865067, y = -0.0814191923}, {x = 0.640084863, y = -0.199776307}}
 """
-    cmd = f"echo '{INPUT}' | ./main.py 'convert this to a python list of 2 element tulpes'"
+    cmd = f"echo '{INPUT}' | ./main.py 'convert this to a python list of 2 element tulpes (x,y), just write the definition of the list'"
     result = execute(cmd)
     assert result.returncode == 0
     res = result.stdout.decode().strip()
-    POINTS="[(0.441429973, -0.176619753), (0.476210177, -0.104575738), (0.674865067, -0.0814191923), (0.640084863, -0.199776307)]"
-    assert POINTS in res
+    POINTS=eval("[(0.441429973, -0.176619753), (0.476210177, -0.104575738), (0.674865067, -0.0814191923), (0.640084863, -0.199776307)]")
+    res = res.split('=')[-1]
+    res = eval(res)
+    assert len(POINTS) == len(res)
+    assert all(p1 == p2 for p1, p2 in zip(POINTS, res)) 
 
 
 def test_filter_create_python_plot_from_points():
     POINTS="[(0.441429973, -0.176619753), (0.476210177, -0.104575738), (0.674865067, -0.0814191923), (0.640084863, -0.199776307)]"
     cmd = f"echo '{POINTS}' | ./main.py 'write a python function to scatter plot these points using matplotlib'"
     result = execute(cmd)
     res = result.stdout.decode().strip()
```

### Comparing `tulp-1.0/test/test_filterMode_basic.py` & `tulp-2.0/test/test_filterMode_basic.py`

 * *Files identical despite different names*

### Comparing `tulp-1.0/test/test_requestMode.py` & `tulp-2.0/test/test_requestMode.py`

 * *Files identical despite different names*

### Comparing `tulp-1.0/test/test_slowtest.py` & `tulp-2.0/test/test_slowtest.py`

 * *Files identical despite different names*

### Comparing `tulp-1.0/tulp/TulpOutputFileWriter.py` & `tulp-2.0/tulp/TulpOutputFileWriter.py`

 * *Files identical despite different names*

### Comparing `tulp-1.0/tulp/createFilteringProgramPrompt.py` & `tulp-2.0/tulp/createFilteringProgramPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-1.0/tulp/createProgramPrompt.py` & `tulp-2.0/tulp/createProgramPrompt.py`

 * *Files identical despite different names*

### Comparing `tulp-1.0/tulp/filteringPrompt.py` & `tulp-2.0/tulp/filteringPrompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 - Your main functionality is to process the given raw_input (from now on: the raw_input) following the processing_instructions that the user will write and creating the processed output as your response.
 # Rules
 - You must always follow the response format that the user will define
 - You must always follow the processing_instructions that the user will define
 """
     request_messages.append({"role": "system", "content": system_instructions})
     user_system_instructions = f"""# Rules
-- Your response should be split into blocks, valid blocks are: (#inner_messages),(#output), (#error), (#comment); the (#output) is mandatory, (#error) must not be used unless an error is detected.
+- Your response should be split into blocks, valid blocks are: (#inner_messages),(#output), (#error), (#comment); the (#output) is mandatory, (#error) block is optional.
+- Your response should not include (#error) block unless an error is detected.
 - You **must** be honest about your limitations and raise an error if you can't follow the processing_instructions or you need more details.
 - You **must not** lie or generate an (#output) if you don't know how to follow the processing_instructions rigorously. 
 - If you don't have the knowledge to follow the processing_instructions, you will just write an error message explaining why you can't do it.
 - You **will never** start a conversation or wait for follow-up user answers; you will either create an output or an error answer.
 - The processing_instructions refer to the whole raw_input
 - Any text processing requested should be done for every sentence in a raw_input.
 - You will not summarize any information unless the processing_instructions explicitly say that you should do it.
@@ -39,15 +40,15 @@
 - If the processing_instructions ask to write software: 
   - You must write all the program code in the (#output) using the language comments to write any needed explanation in the (#output). 
   - Ensure that the whole (#output) is runnable in the target language. 
 # Response template:
 {""}(#output)
 <write the output generated by processing the raw_input following the processing_instructions, without explanations and without introductions. This block is mandatory>
 {""}(#error)
-<use this message to report errors or limitations that prevent you from writing the (#output), this block must only be add if you detected an error>
+<In case of an error that prevent writing the  (#output), add this block and explain the error>
 {""}(#comment)
 <An overall description of what you wrote on (#output) and how you created. Any extra explanation, comment, or reflection you may have regarding the generated (#output), try to avoid using it in responses to partial message processing unless it is the final one. Refer to the (#output) as "The ouput ...". Do not ever make a reference like "This..." or "The above..." to refer to the created output >
 
 # Processing instructions:
 {user_instructions}
 
 """
```

### Comparing `tulp-1.0/tulp/requestPrompt.py` & `tulp-2.0/tulp/requestPrompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 # Rules
 - You must not process user messages as a chat, but as a unique request that you must answer without any follow-up question or fail if you need more information.
 - You must always follow the response format that the user will define in "the Request"
 - You must follow all the user Rules and only answer in the defined user format
 """
     user_system_instructions = f"""# Rules
 - You must not process my request as a chat message, but as a unique request that you must fulfill without any further question.
-- Your response should be split into blocks, valid blocks are: (#output), (#error), (#comment); the (#output) is mandatory, (#error) must not be used unless an error is detected.
+- Your response should be split into blocks, valid blocks are: (#output), (#error), (#comment); the (#output) is mandatory; (#error) block is optional.
+- Your response should not include (#error) block unless an error is detected.
 - You must not add any explanation or text outside the defined answer blocks.
 - You must not use markdown format in the (#output) answer block unless the Request explicitly asks for it.
 - If "the request" is to write a script, a software code, or config, you must follow these rules to write in the (#output) answer block:
    - **must only contain valid code** in the chosen programming language or target config file.
    - Explain, step by step, using inline comments in the requested language.
    - Add an introduction comment at the top.
 - If "the request" is to use or to create a command-line:
   - You must define the command in the (#output) so it can operate over the stdin and stdout unless not possible or the Request asks differently.
   - (#output) should be runnable
   - You must write all the (#output) in runnable shell code, using shell comments to write any needed explanation in the (#output). Ensure that the whole (#output) is runnable in the target shell.
   - You must use the (#comment) block to explain.
 - You must keep all the (#output) answer blocks in the formats that the Request specifies, avoiding mixing formats such as markdown and scripting in the same output.
-- You must not start your coding (#output) message with "```" or "```python" or "```...", just write the code without any explanation.
 - If my request asks to create some content, write the raw content without any explanation in the (#output) answer block and use the (#comment) block to write any explanation referred to the output block.
-- You must not write the (#error) block, unless there is an error to report.
+- Only write the (#error) block in case of error.
 - When possible, the (#output) block should only contain runnable code and any explaination should be written in the (#comment) block, unless the request explicitly mandates differently.
 - You must use the following response template:
 
 (#output)
 <your best answer to "the Request" bellow, without any explanations and without any introductions. This block is mandatory>
 (#error)
-<use this message to report errors or limitations that prevent you from writing the (#output), this block must only be add if you detected an error>
+<In case of an error that prevent writing the  (#output), add this block and explain the error>
 (#comment)
 < Any extra explanation, comment or reflection you may have regarding the generated (#output), refer to the (#output) as "The created ...". Do never make a reference like "This..." or "The above..." to refer to the created output.>
 - You must use my following message as the Request. The request:
 """
     request_messages = []
     request_messages.append( {"role": "system", "content": system_instructions} )
     request_messages.append( {"role": "user", "content": user_system_instructions} )
```

### Comparing `tulp-1.0/tulp/tulp.py` & `tulp-2.0/tulp/tulp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 #!/usr/bin/python3
-from openai import OpenAI
 
 import sys
 import os
 import math
 from . import tulpargs
 from . import tulplogger
 from . import tulpconfig
 from . import version
 from . import TulpOutputFileWriter
 
 
 log = tulplogger.Logger()
 config = tulpconfig.TulipConfig()
 args = tulpargs.TulpArgs().get()
-client: object  # will be defined in main
+llmclient: object  # will be defined in main
 
 # Helper functions
 
 ## cleanup_output: clenaup output, removing artifacts
 def cleanup_output(output):
-    olines = output.splitlines()
+    olines = output.strip().splitlines()
     # gpt-3.5 usually adds unneeded markdown codeblock wrappers, try to remove them
     if len(olines) > 2:
         if olines[0].startswith("```") and olines[-1] == "```":
-            log.debug("markdown codeblock wrapping detected and stripped!")
+            log.info("markdown codeblock wrapping detected and stripped!")
             return "\n".join(olines[1:-1])
     return output
 
 
 ## block_exists(blocks_dict, key):  test if a KEY exist and is not empty
 def block_exists(blocks_dict, key):
     return key in blocks_dict and len(blocks_dict[key]["content"].strip()) > 0
 
 ## VALID_BLOCKS: define the valid answer blocks  blocks
 VALID_BLOCKS=["(#output)","(#thoughts)","(#inner_message)","(#error)","(#context)","(#comment)","(#end)"]
 ## parse_response)response_text): parse a gpt response, returning a dict with each response section 
 def parse_response(response_text):
     blocks_dict={}
-    lines = response_text.splitlines()
+    lines = response_text.strip().splitlines()
     # (#end) is not specified by us, but sometimes gpt-3.5 wrote it so we just parse it so we can keep it out
 
     # parse blocks:
     parsingBlock=None
     for line in lines:
         splitted_line = line.split(" ")
         key = None
@@ -67,15 +66,15 @@
                 if config.model == "gpt-3.5-turbo": 
                     log.error("""
 Unknown error while processing: this is usually related to gpt not honoring our
 output format, please try again and try to be more specific, you can also try
 with a different model (e.g., TULP_MODEL=gpt-4 tulp ...)""")
                 else:
                     log.error("""
-Unknown error while processing: this is usually related to gpt not honoring
+Unknown error while processing: this is usually related to llm not honoring
 our output format, please try again and try to be more specific in your
 request. You can also try to enable DEBUG log to inspect the raw answer (e.g.,
 TULP_LOG_LEVEL=DEBUG tulp ...)""") 
                 log.debug(f"ERROR: Invalid answer format: =====\n {response_text} \n=====")
                 sys.exit(2)
     return blocks_dict
 
@@ -136,21 +135,19 @@
     max_retries = 5
     if (not raw_input_chunks):
         raw_input_chunks = [""]
     requestMessages = promptFactory.getMessages(user_request, raw_input_chunks[0], len(raw_input_chunks))
     while retries < max_retries:
         for req in requestMessages:
             log.debug(f"REQ: {req}")
-        log.debug(f"Sending the request to OpenAI...")
-        response = client.chat.completions.create(model=config.model,
-        messages=requestMessages,
-        temperature=0)
+        log.debug(f"Sending the request to model...")
+        response = llmclient.generate(messages)
         log.debug(f"ANS: {response}")
-        response_text = response.choices[0].message.content
-        finish_reason = response.choices[0].finish_reason
+        response_text = response["response_text"]
+        finish_reason = response["finish_reason"]
         blocks_dict = parse_response(response_text)
         if block_exists(blocks_dict,"(#comment)"):
             log.info(blocks_dict["(#comment)"]["content"])
         if block_exists(blocks_dict,"(#output)"):
             oType = ""
             generatedCode = cleanup_output(blocks_dict["(#output)"]["content"])
             log.debug(f"The generated code:\n{generatedCode}")
@@ -195,21 +192,19 @@
         finish_reason = ""
         response_text = ""
         raw_input_chunk = raw_input_chunks[i]
         if user_request:
             requestMessages = promptFactory.getMessages(user_request, raw_input_chunk , len(raw_input_chunks), i+1)
             for req in requestMessages:
                 log.debug(f"REQ: {req}")
-            log.debug(f"Sending the request to OpenAI...")
-            response = client.chat.completions.create(model=config.model,
-            messages=requestMessages,
-            temperature=0)
+            log.debug(f"Sending the request to llm...")
+            response = llmclient.generate(requestMessages)
             log.debug(f"ANS: {response}")
-            response_text += response.choices[0].message.content
-            finish_reason = response.choices[0].finish_reason
+            response_text += response["response_text"]
+            finish_reason = response["finish_reason"]
 
 
         blocks_dict = parse_response(response_text)
 
         if block_exists(blocks_dict,"(#error)"):
             log.error("Error: Couldn't process your request:")
             log.error(blocks_dict["(#error)"]["content"])
@@ -251,29 +246,24 @@
 """
 
             log.error(errorMsg)
             sys.exit(2)
 
 def run():
     log.debug(f"Running tulp v{version.VERSION} using model: {config.model}")
-    openai_key = config.openai_api_key
-    if not openai_key:
-        log.error(f'OpenAI API key not found. Please set the TULP_OPENAI_API_KEY environment variable or add it to {tulpconfig.CONFIG_FILE}')
-        log.error(f"If you don't have one, please create one at: https://platform.openai.com/account/api-keys")
-        sys.exit(1)
-
-    global client
-    client = OpenAI(api_key=openai_key)
-
 
+    global llmclient
+    from . import llms
+    llmclient = llms.getModelClient(config.model,config)
 
     # If input is available on stdin, read it
     input_text = ""
     if not sys.stdin.isatty():
-        input_text = sys.stdin.read().strip()
+        #input_text = sys.stdin.read().strip()
+        input_text = sys.stdin.buffer.read().decode('ascii', errors='ignore').strip()
 
     user_request=None
     if not args.request and not input_text:
         user_request = input("Enter your request: ").strip()
     elif args.request and not input_text:
         user_request = args.request
     elif not args.request and input_text:
```

### Comparing `tulp-1.0/tulp/tulpargs.py` & `tulp-2.0/tulp/tulpargs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 import os
 import argparse
 import re
+from . import llms
 
 CONFIG_FILE=os.path.expanduser("~/.tulp.conf")
 
-def model_type(arg_value, pat=re.compile(r"^gpt-[a-z0-9\-_\.]*$")):
-    if not pat.match(arg_value):
-        raise argparse.ArgumentTypeError("Invalid model")
-    return arg_value
+def model_type(arg_value):
+   client = llms.getModelModule(arg_value)
+   if (not client):
+       raise argparse.ArgumentTypeError("Invalid model")
+   return arg_value
 
 class TulpArgs:
     _instance = None
 
+    def loadLlmsArguments(self,parser):
+        for o in llms.getArguments():
+            parser.add_argument(f'--{o["name"]}', type=str, help=o['description'])
 
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            parser = argparse.ArgumentParser(description="""TULP Understands Language Promptly:
+            parser = argparse.ArgumentParser(description=f"""TULP Understands Language Promptly:
 A command line tool, in the best essence of POSIX tooling, that will help you
 to **process**, **filter**, and **create** data in this new Artificial
-Intelligence world, backed by chatGPT.
+Intelligence world.
 
-""")
+Tulp support different backends and models, the backend will be automatically selected for each model, currently supported models should match:
+{llms.getModelsDescription()}
+
+""",
+formatter_class=argparse.RawTextHelpFormatter
+)
             parser.add_argument('-x', action='store_true', help='Allow tulp to create a program and execute it to fulfill the task (code interpret)')
 
             parser.add_argument('-w', type=str, help='Write the output (or the created program for execution) to the file. If the file exists, a backup will be created before overwriting it.')
 
 
-            parser.add_argument('--model', type=model_type, help='Select the openai LLM model to use (default: gpt-4-0125-preview)')
+            parser.add_argument('--model', type=model_type, help='Select the openai LLM model to use (default: gpt-4-turbo)')
 
             parser.add_argument('--max-chars', type=int, help='Number of chars per message chunk per request (Default 40000)')
 
             parser.add_argument('-v', action='store_true', help='Be verbose!')
 
             parser.add_argument('-q', action='store_true', help='Be quiet! Only print the answer and errors.')
 
+            cls._instance.loadLlmsArguments(parser)
+
             parser.add_argument('request', nargs=argparse.REMAINDER, help="User request, instructions written in natural language")
 
 
 
+
             args = parser.parse_args()
             cls._instance.args = args
 
             if 'help' in args:
                 parser.print_help()
                 return
```

### Comparing `tulp-1.0/tulp/tulpconfig.py` & `tulp-2.0/tulp/tulpconfig.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import os
 import configparser
 from . import tulpargs
+from . import tulplogger
 
 CONFIG_FILE=os.path.expanduser("~/.tulp.conf")
 
 class TulipConfig:
     _instance = None
 
     def getValue(self, key, defaultValue):
         value = self.config.get("DEFAULT", key, fallback=defaultValue)
         value = os.environ.get(f"TULP_{key}", value)
         return value
 
+    def CONFIG_FILE(self):
+        return CONFIG_FILE
+    def loadLlmsArguments(self,cliargs):
+        from . import llms
+        for o in llms.getArguments():
+            setattr(self,o['name'], cliargs.__getattribute__(o["name"]) or self.getValue(o["name"].upper(),o["default"]))
+
     def __new__(cls):
 
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             args = tulpargs.TulpArgs().get()
             cls._instance.config = configparser.ConfigParser()
             cls._instance.config.read(CONFIG_FILE)
 
+
             cls._instance.log_level = (args.v and "DEBUG") or (args.q and "ERROR")  or cls._instance.getValue("LOG_LEVEL", "INFO")
-            cls._instance.openai_api_key = cls._instance.getValue("OPENAI_API_KEY",None)
+            tulplogger.setLogLevel(cls._instance.log_level)
             cls._instance.max_chars = int(args.max_chars or cls._instance.getValue("MAX_CHARS", "40000"))
-            cls._instance.model = args.model or cls._instance.getValue("MODEL", "gpt-4-0125-preview")
+            cls._instance.model = args.model or cls._instance.getValue("MODEL", "gpt-4-turbo")
+            cls._instance.loadLlmsArguments(args)
 
         return cls._instance
```

### Comparing `tulp-1.0/tulp/tulplogger.py` & `tulp-2.0/tulp/tulplogger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import os
 import sys
-from . import tulpconfig
-
-config = tulpconfig.TulipConfig()
 
 YELLOW = '\033[33m'
 ORANGE = '\033[38;5;208m'
 RED    = '\033[31m'
 BOLD   = '\033[1m'
 RESET  = '\033[0m'
 GREY   = '\033[90m'
@@ -33,32 +30,47 @@
 def print_color(text, color):
     """Prints text in the specified color"""
     if useColors:
         print(f"{color}{text}{RESET}",file=sys.stderr)
     else:
         print(text,file=sys.stderr)
 
+loglevel = 'ERROR'
+
+def setLogLevel(level):
+    global loglevel
+    loglevel = level
+
+
 class Logger:
     def __init__(self):
-        self.log_level = config.log_level
+        self.loglevel = None
+
+    def __getLevel(self):
+        global loglevel
+        return self.loglevel or loglevel
+
+    # override global loglevel
+    def setLogLevel(self,level):
+        self.loglevel = level
 
     def error(self, message):
-        if self.log_level in ['ERROR', 'WARNING', 'INFO', 'DEBUG']:
+        if self.__getLevel() in ['ERROR', 'WARNING', 'INFO', 'DEBUG']:
             print_color(f'[ERROR] {message}',RED)
 
     def warning(self, message):
-        if self.log_level in ['WARNING', 'INFO', 'DEBUG']:
+        if self.__getLevel() in ['WARNING', 'INFO', 'DEBUG']:
             print_color(f'[WARNING] {message}',ORANGE)
 
     def info(self, message):
-        if self.log_level in ['INFO', 'DEBUG']:
+        if self.__getLevel() in ['INFO', 'DEBUG']:
             print_color(f'[INFO] {message}',GREY_18)
 
     def debug(self, message):
-        if self.log_level == 'DEBUG':
+        if self.__getLevel() == 'DEBUG':
             print_color(f'[DEBUG] {message}',GREY_11)
 
 if __name__ == '__main__':
     # Example usage
     logger = Logger()
     logger.error('This is an error message')
     logger.warning('This is a warning message')
```

### Comparing `tulp-1.0/tulp.egg-info/PKG-INFO` & `tulp-2.0/tulp.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: tulp
-Version: 1.0
+Version: 2.0
 Summary: TULP: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world.
 Home-page: https://github.com/fedenunez/tulp
 Author: Federico Nuñez
 Author-email: fedenunez@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai>=1.0.0
+Requires-Dist: openai==1.25.1
+Requires-Dist: google-ai-generativelanguage==0.6.2
+Requires-Dist: anthropic==0.25.7
+Requires-Dist: groq==0.5.0
+Requires-Dist: ollama==0.1.9
 
-# TULP: TULP Understands Language Promptly
+# TULP: TULP Understands Language Promptly | v2.0 
 
-A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, backed by chatGPT.
+A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with enhanced capabilities to utilize various AI APIs including groq, ollama, anthropic, and gemini.
 
-TULP allows you to harness the power of chatGPT by piping standard input content directly to chatGPT, getting the answer back on the shell.
+TULP allows you to harness the power of multiple AI models by piping standard input content directly to these models, getting the answer back on the shell.
 
 [![tulp demo video](https://markdown-videos.deta.dev/youtube/mHAvlRXXp6I)](https://www.youtube.com/watch?v=mHAvlRXXp6I)
 
 ## Installation:
 
 ```bash
 pip install tulp
@@ -43,80 +47,127 @@
 ```
 cat examples/titanics.csv | tulp -x how many persons survived
 ```
 
 
 In both cases, TULP will write to the standard output the answers and will write any other information to the standard error. You can safely pipe the output to your file or next piping command and will still get all the information and errors on stderr.
 
-It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by chatGPT in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
+It is **important** to note that if your input is larger than 5000 characters, the input will be split into multiple chunks and processed by the selected AI model in multiple requests. In this case, the result quality will really depend on the task (e.g., will work fine for translations or grammatical corrections, it will work terribly for summarizing). Anyway, **tulp works great when the input is less than 5000 chars**.
 
-By default, tulp uses **gpt-3.5-turbo**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to force the gpt-4 model**: tulp --model gpt-4 {a complex task}
+By default, tulp uses **gpt-4-0125-preview**, because it is cheaper and **faster**, but for complex tasks, it is always a **good idea to specify the model**: tulp --model {model_name} {a complex task}
 
 ### Options:
 ```
-usage: tulp [-h] [-x] [-w W] [--model {gpt-3.5-turbo,gpt-4}] [--max-chars MAX_CHARS] [-v] [-q] ...
+usage: tulp [-h] [-x] [-w W] [--model MODEL] [--max-chars MAX_CHARS] [-v] [-q] [--groq_api_key GROQ_API_KEY] [--ollama_host OLLAMA_HOST] [--anthropic_api_key ANTHROPIC_API_KEY] [--openai_api_key OPENAI_API_KEY] [--openai_baseurl OPENAI_BASEURL] [--gemini_api_key GEMINI_API_KEY] ...
 
-TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, backed by chatGPT.
+TULP Understands Language Promptly: A command line tool, in the best essence of POSIX tooling, that will help you to **process**, **filter**, and **create** data in this new Artificial Intelligence world, now with support for multiple AI APIs including groq, ollama, anthropic, and gemini.
 
 positional arguments:
   request               User request, instructions written in natural language
 
 optional arguments:
   -h, --help            show this help message and exit
   -x                    Allow tulp to create a program and execute it to fulfill the task (code interpret)
   -w W                  Write the output (or the created program for execution) to the file. If the file exists, a backup will be created before overwriting it.
-  --model {gpt-3.5-turbo,gpt-4}
-                        Select the LLM model to use, currently gpt-3.5-turbo or gpt-4
+  --model MODEL         Select the AI LLM model to use, now supporting groq.*, ollama.*, claude-.*, gpt-.*, and gemini.* models
   --max-chars MAX_CHARS
                         Number of chars per message chunk per request
   -v                    Be verbose!
   -q                    Be quiet! Only print the answer and errors.
+  --groq_api_key GROQ_API_KEY
+                        GROQ cloud API KEY
+  --ollama_host OLLAMA_HOST
+                        Define custom ollama host
+  --anthropic_api_key ANTHROPIC_API_KEY
+                        Anthropic api key
+  --openai_api_key OPENAI_API_KEY
+                        OpenAI cloud API KEY
+  --openai_baseurl OPENAI_BASEURL
+                        Use it to change the server, e.g.: use http://localhost:11434/v1/ to connect to your local ollama server
+  --gemini_api_key GEMINI_API_KEY
+                        gemini cloud API KEY
 
 ```
 
-
 ## Configuration 
 The configuration file is located at ~/.tulp.conf. 
 
 The following are the parameters that can be configured:
 - **LOG_LEVEL**: The log level of Tulp. Valid options are DEBUG, INFO, WARNING, ERROR, and CRITICAL. The default value is INFO.
-- **OPENAI_API_KEY**: The API key for OpenAI. The default value is an empty string.
-- **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 5000.
-- **MODEL**: The OpenAI model to be used by Tulp. The default value is gpt-3.5-turbo, but gpt-4 is also available.
+- **API_KEYS**: The API keys for the supported AI models (OpenAI, GROQ, Ollama, Anthropic, Gemini). The default value is an empty string for each.
+- **MAX_CHARS**: The maximum number of characters processed in one chunk. The default value is 40000.
+- **MODEL**: The AI model to be used by Tulp. The default value is gpt-4-0125-preview, but other models are also available.
 
 All these settings could be overridden by an environment variable using the prefix TULP\_ or by the different command line arguments described above. 
-As environment variables, they will become: TULP_LOG_LEVEL, TULP_OPENAI_API_KEY, TULP_MAX_CHARS, or TULP_MODEL.
+As environment variables, they will become: TULP_LOG_LEVEL, TULP_API_KEYS, TULP_MAX_CHARS, or TULP_MODEL.
 Command line arguments will override environmental variables and the configuration file.
 
 
 Here is an example configuration file with the default values:
 ```INI
 [DEFAULT]
 LOG_LEVEL = INFO
-OPENAI_API_KEY = <<<YOUR API KEY >>>>
-MAX_CHARS = 10000
-MODEL = gpt-3.5-turbo
+${MODEL}_API_KEYS = <<<YOUR API KEYS FOR GROQ, OLLAMA, ANTHROPIC, OPENAI, GEMINI>>>
+MAX_CHARS = 40000
+MODEL = gpt-4-0125-preview
 ```
+
+
 ## Examples:
 The usage is endless, but anyway, here you have some ideas as inspiration:
 
 ### Random
+#### The meaning of life for different models:
+
+```
++ tulp -q --model gpt-4-turbo tell me the meaning of life in just 3 words
+42, not known
+
+
++ tulp -q --model gpt-3.5-turbo tell me the meaning of life in just 3 words
+Live, love, learn.
+
++ tulp -q --model claude-3-opus-20240229 tell me the meaning of life in just 3 words
+Love conquers all.
+
++ tulp -q --model gemini-1.5-pro-latest tell me the meaning of life in just 3 words
+The answer is 42.
+
++ tulp -q --model groq.gemma-7b-it tell me the meaning of life in just 3 words
+The meaning of life is to find purpose and fulfillment in the present moment.
+
+
++ tulp -q --model groq.llama3-70b-8192 tell me the meaning of life in just 3 words
+Find Your Purpose
+
++ tulp -q --model groq.mixtral-8x7b-32768 tell me the meaning of life in just 3 words
+Impossible task.
+
++ tulp -q --model ollama.phi3:instruct tell me the meaning of life in just 3 words
+echo "Meaning of Life"
+```
+
 #### Create a plot directly from raw memory output printed by gdb:
 Command:
 ```bash
 cat <<EOF | tulp convert this to a python list of 2 element tuples |  tulp write a python function to scatter plot these points using matplotlib | python 
 (gdb) p *polygon._points._M_ptr._M_impl._M_start@4
 $21 = {{x = 0.441429973, y = -0.176619753}, {x = 0.476210177, y = -0.104575738}, {x = 0.674865067, y = -0.0814191923}, {x = 0.640084863, y = -0.199776307}}
 EOF
 ```
 
 Result:
 
 ![matplotlib @rela](./examples/rela_plot.png)
 
+### Grammatical and Syntax Correction of Clipboard Content in Linux (The Corrected Version Will Be in the Clipboard)
+
+```bash
+xsel -b | tulp fix my english | xsel -b
+```
 
 
 ### Typical Unix tooling replacement:
 #### Sed
 ```bash
 cat README.md | tulp replace all the occurrences of TULP for **TULP**
 ```
@@ -208,17 +259,22 @@
 ```
 
 # Why?
 
 I am a heavy user of Unix tooling (e.g: awk, jq, sed, grep, and so on), I have been using them since my early days and I used to think that I couldn't survive without them. But then, ChatGPT appeared, and I started to use more and more GPT for things that I used to use Unix tooling for. Somehow I feel the pain of cut & paste, and I was missing a way to do it faster and from within the terminal itself, so I came up with `tulp`.
 
 # Changelog
+## v2.0 | 2024-05-04
+- Added support for groq, ollama, anthropic, and gemini AI models.
+- Changed to use gpt-4-turbo model by default
+
 ## v1.0 | 2024-02-14
 - Changed to use gpt-4-0125-preview model by default
 - Updated to use openapi v1.0
 - Changes default max-chars to 40000
 
-## v07  | 2023-05-23 
+## v0.7  | 2023-05-23 
 - Adds Code Interpretation, -x option
 ## v0.6 | 2023-05-11
 - Adds all the settings as command line arguments
 
+
```

### Comparing `tulp-1.0/tulp.egg-info/SOURCES.txt` & `tulp-2.0/tulp.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -20,8 +20,14 @@
 tulp/version.py
 tulp.egg-info/PKG-INFO
 tulp.egg-info/SOURCES.txt
 tulp.egg-info/dependency_links.txt
 tulp.egg-info/entry_points.txt
 tulp.egg-info/requires.txt
 tulp.egg-info/top_level.txt
-tulp.egg-info/zip-safe
+tulp.egg-info/zip-safe
+tulp/llms/LlmAnthropic.py
+tulp/llms/LlmGemini.py
+tulp/llms/LlmGroq.py
+tulp/llms/LlmOllama.py
+tulp/llms/LlmOpenAI.py
+tulp/llms/__init__.py
```

