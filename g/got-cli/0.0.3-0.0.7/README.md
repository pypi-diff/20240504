# Comparing `tmp/got-cli-0.0.3.tar.gz` & `tmp/got-cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "got-cli-0.0.3.tar", last modified: Sat May  4 19:50:05 2024, max compression
+gzip compressed data, was "got-cli-0.0.7.tar", last modified: Sat May  4 20:12:22 2024, max compression
```

## Comparing `got-cli-0.0.3.tar` & `got-cli-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 19:50:05.557220 got-cli-0.0.3/
--rw-r--r--   0 guialves   (501) staff       (20)     1066 2024-05-04 19:36:59.000000 got-cli-0.0.3/LICENSE
--rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 19:50:05.557087 got-cli-0.0.3/PKG-INFO
--rw-r--r--   0 guialves   (501) staff       (20)     1548 2024-05-04 19:46:44.000000 got-cli-0.0.3/README.md
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 19:50:05.554857 got-cli-0.0.3/got/
--rw-r--r--   0 guialves   (501) staff       (20)        0 2024-05-04 17:10:40.000000 got-cli-0.0.3/got/__init__.py
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 19:50:05.555972 got-cli-0.0.3/got/ai/
--rw-r--r--   0 guialves   (501) staff       (20)     2242 2024-05-04 19:31:02.000000 got-cli-0.0.3/got/ai/__init__.py
--rw-r--r--   0 guialves   (501) staff       (20)     1210 2024-05-04 18:10:34.000000 got-cli-0.0.3/got/ai/chatgpt.py
--rw-r--r--   0 guialves   (501) staff       (20)      545 2024-05-04 18:20:32.000000 got-cli-0.0.3/got/ai/factory.py
--rw-r--r--   0 guialves   (501) staff       (20)     1326 2024-05-04 18:17:57.000000 got-cli-0.0.3/got/ai/groq.py
--rw-r--r--   0 guialves   (501) staff       (20)     4473 2024-05-04 19:46:00.000000 got-cli-0.0.3/got/cli.py
--rw-r--r--   0 guialves   (501) staff       (20)     2104 2024-05-04 19:41:42.000000 got-cli-0.0.3/got/commit.py
--rw-r--r--   0 guialves   (501) staff       (20)     2649 2024-05-04 19:13:35.000000 got-cli-0.0.3/got/git.py
--rw-r--r--   0 guialves   (501) staff       (20)     1945 2024-05-04 16:57:28.000000 got-cli-0.0.3/got/printer.py
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 19:50:05.556908 got-cli-0.0.3/got_cli.egg-info/
--rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 19:50:05.000000 got-cli-0.0.3/got_cli.egg-info/PKG-INFO
--rw-r--r--   0 guialves   (501) staff       (20)      351 2024-05-04 19:50:05.000000 got-cli-0.0.3/got_cli.egg-info/SOURCES.txt
--rw-r--r--   0 guialves   (501) staff       (20)        1 2024-05-04 19:50:05.000000 got-cli-0.0.3/got_cli.egg-info/dependency_links.txt
--rw-r--r--   0 guialves   (501) staff       (20)       37 2024-05-04 19:50:05.000000 got-cli-0.0.3/got_cli.egg-info/entry_points.txt
--rw-r--r--   0 guialves   (501) staff       (20)       79 2024-05-04 19:50:05.000000 got-cli-0.0.3/got_cli.egg-info/requires.txt
--rw-r--r--   0 guialves   (501) staff       (20)        4 2024-05-04 19:50:05.000000 got-cli-0.0.3/got_cli.egg-info/top_level.txt
--rw-r--r--   0 guialves   (501) staff       (20)       38 2024-05-04 19:50:05.557279 got-cli-0.0.3/setup.cfg
--rw-r--r--   0 guialves   (501) staff       (20)      658 2024-05-04 19:50:05.000000 got-cli-0.0.3/setup.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.154304 got-cli-0.0.7/
+-rw-r--r--   0 guialves   (501) staff       (20)     1066 2024-05-04 19:36:59.000000 got-cli-0.0.7/LICENSE
+-rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 20:12:22.154105 got-cli-0.0.7/PKG-INFO
+-rw-r--r--   0 guialves   (501) staff       (20)     2039 2024-05-04 20:11:18.000000 got-cli-0.0.7/README.md
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.152471 got-cli-0.0.7/got/
+-rw-r--r--   0 guialves   (501) staff       (20)        0 2024-05-04 17:10:40.000000 got-cli-0.0.7/got/__init__.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.152999 got-cli-0.0.7/got/ai/
+-rw-r--r--   0 guialves   (501) staff       (20)     2242 2024-05-04 19:31:02.000000 got-cli-0.0.7/got/ai/__init__.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1210 2024-05-04 18:10:34.000000 got-cli-0.0.7/got/ai/chatgpt.py
+-rw-r--r--   0 guialves   (501) staff       (20)      545 2024-05-04 18:20:32.000000 got-cli-0.0.7/got/ai/factory.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1326 2024-05-04 18:17:57.000000 got-cli-0.0.7/got/ai/groq.py
+-rw-r--r--   0 guialves   (501) staff       (20)     4473 2024-05-04 19:46:00.000000 got-cli-0.0.7/got/cli.py
+-rw-r--r--   0 guialves   (501) staff       (20)     2104 2024-05-04 19:41:42.000000 got-cli-0.0.7/got/commit.py
+-rw-r--r--   0 guialves   (501) staff       (20)     2649 2024-05-04 20:00:46.000000 got-cli-0.0.7/got/git.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1945 2024-05-04 16:57:28.000000 got-cli-0.0.7/got/printer.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.153781 got-cli-0.0.7/got_cli.egg-info/
+-rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/PKG-INFO
+-rw-r--r--   0 guialves   (501) staff       (20)      351 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 guialves   (501) staff       (20)        1 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       37 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/entry_points.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       79 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/requires.txt
+-rw-r--r--   0 guialves   (501) staff       (20)        4 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/top_level.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       38 2024-05-04 20:12:22.154489 got-cli-0.0.7/setup.cfg
+-rw-r--r--   0 guialves   (501) staff       (20)      658 2024-05-04 20:12:22.000000 got-cli-0.0.7/setup.py
```

### Comparing `got-cli-0.0.3/LICENSE` & `got-cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/README.md` & `got-cli-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-# GOT - Git Operations Tool
+# GOT-CLI
 
 GOT is a command-line tool designed to enhance your git workflow by integrating AI-driven commit message suggestions. It leverages models from both OpenAI and Groq to suggest relevant commit messages based on the changes you've made.
 
 ## Features
 
 - **AI-Driven Commit Suggestions**: Utilize models like GPT-3.5, GPT-4, and various Groq models to generate commit messages.
 - **Interactive Commit Process**: Choose commit messages from suggested options or enter manually.
 - **Commit and Push**: Option to automatically add, commit, and push changes to a remote repository.
 
 ## Installation
 
-Clone the repository and install the required packages:
+Install from pip
 
 ```bash
-git clone https://github.com/GuiPimenta-Dev/got
-cd got
-pip install -r requirements.txt
+pip install got-cli
+```
+
+## API Tokens
+
+GOT leverages powerful AI models from OpenAI's [Chat GPT](https://platform.openai.com/docs/guides/text-generation) and [GROQ Cloud](https://console.groq.com/playground). To enable these features, you must configure API tokens as environment variables.
+
+Before using the CLI, set up your environment variables based on the model you intend to use. These tokens will authenticate your requests to the respective services.
+
+```
+# Set the OpenAI Chat GPT API token
+export CHAT_GPT_TOKEN=<Your_Chat_GPT_API_Token>
+
+# Set the GROQ API key
+export GROQ_API_KEY=<Your_GROQ_API_Key>
 ```
 
 ## Usage
 
 ### Committing Changes
 
 To commit changes with AI-generated messages:
@@ -28,19 +40,19 @@
 got commit -a -p
 ```
 
 Options:
 
 - `-a`: Automatically stage all changes before committing.
 - `-p`: Push changes to the remote repository after committing.
-- `-m`: Specify the language model to use for generating commit messages.
+- `-m`: Specify the language model to use for generating commit messages (Default: gpt-4-turbo).
 
 ### Modifying Prompts
 
-To modify the prompts and examples used by the tool:
+To modify the prompts and examples used by the cli:
 
 ```bash
 got prompt --set-example
 ```
 
 Options:
```

### Comparing `got-cli-0.0.3/got/ai/__init__.py` & `got-cli-0.0.7/got/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/ai/chatgpt.py` & `got-cli-0.0.7/got/ai/chatgpt.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/ai/factory.py` & `got-cli-0.0.7/got/ai/factory.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/ai/groq.py` & `got-cli-0.0.7/got/ai/groq.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/cli.py` & `got-cli-0.0.7/got/cli.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/commit.py` & `got-cli-0.0.7/got/commit.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/git.py` & `got-cli-0.0.7/got/git.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/got/printer.py` & `got-cli-0.0.7/got/printer.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.3/setup.py` & `got-cli-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="got-cli",
-    version="0.0.3",
+    version="0.0.7",
     packages=find_packages(),
     license="MIT",
     install_requires=[
         "openai==1.25.1",
         "groq==0.5.0",
         "click==8.1.3",
         "python-dotenv==1.0.1",
```

