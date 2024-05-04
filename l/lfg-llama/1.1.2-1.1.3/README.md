# Comparing `tmp/lfg_llama-1.1.2.tar.gz` & `tmp/lfg_llama-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.1.2.tar", last modified: Fri May  3 14:24:42 2024, max compression
+gzip compressed data, was "lfg_llama-1.1.3.tar", last modified: Fri May  3 14:28:48 2024, max compression
```

## Comparing `lfg_llama-1.1.2.tar` & `lfg_llama-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:24:42.195031 lfg_llama-1.1.2/
--rw-r--r--   0 ob907      (502) staff       (20)     1217 2024-05-03 14:24:42.194802 lfg_llama-1.1.2/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      980 2024-05-03 14:24:05.000000 lfg_llama-1.1.2/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:24:42.193287 lfg_llama-1.1.2/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.2/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2173 2024-05-03 14:13:28.000000 lfg_llama-1.1.2/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:24:42.194557 lfg_llama-1.1.2/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1217 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 14:24:42.195089 lfg_llama-1.1.2/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-03 14:24:38.000000 lfg_llama-1.1.2/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:28:48.179736 lfg_llama-1.1.3/
+-rw-r--r--   0 ob907      (502) staff       (20)     1281 2024-05-03 14:28:48.179439 lfg_llama-1.1.3/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1044 2024-05-03 14:28:10.000000 lfg_llama-1.1.3/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:28:48.178032 lfg_llama-1.1.3/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.3/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2173 2024-05-03 14:13:28.000000 lfg_llama-1.1.3/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:28:48.179199 lfg_llama-1.1.3/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1281 2024-05-03 14:28:48.000000 lfg_llama-1.1.3/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 14:28:48.000000 lfg_llama-1.1.3/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 14:28:48.000000 lfg_llama-1.1.3/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 14:28:48.000000 lfg_llama-1.1.3/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 14:28:48.000000 lfg_llama-1.1.3/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 14:28:48.000000 lfg_llama-1.1.3/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 14:28:48.179842 lfg_llama-1.1.3/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-03 14:28:45.000000 lfg_llama-1.1.3/setup.py
```

### Comparing `lfg_llama-1.1.2/PKG-INFO` & `lfg_llama-1.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.1.2
+Version: 1.1.3
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
 ![Demo](example.gif)
 
-LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. It taps into the vast knowledge of the LLAMA3 language model (via Ollama) to understand your natural language descriptions and provide you with the most relevant commands and explanations.
+LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch.
+
+## Why?
+
+Testing the llama3 model. Initially it was made using ollama locally, but changed to use groq due to not needing to have the llama3 model downloaded.
 
 ## Installation
 
 ```bash
 # install pipx
 brew install pipx
 
@@ -52,7 +56,11 @@
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.7
 pipenv install
 ```
+
+### TODO
+
+- Add a flag to choose between all the models available by GROQ
```

### Comparing `lfg_llama-1.1.2/lfg/cli.py` & `lfg_llama-1.1.3/lfg/cli.py`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.1.2/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.1.3/lfg_llama.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.1.2
+Version: 1.1.3
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
 ![Demo](example.gif)
 
-LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. It taps into the vast knowledge of the LLAMA3 language model (via Ollama) to understand your natural language descriptions and provide you with the most relevant commands and explanations.
+LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch.
+
+## Why?
+
+Testing the llama3 model. Initially it was made using ollama locally, but changed to use groq due to not needing to have the llama3 model downloaded.
 
 ## Installation
 
 ```bash
 # install pipx
 brew install pipx
 
@@ -52,7 +56,11 @@
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.7
 pipenv install
 ```
+
+### TODO
+
+- Add a flag to choose between all the models available by GROQ
```

