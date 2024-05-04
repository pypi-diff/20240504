# Comparing `tmp/got-cli-0.0.7.tar.gz` & `tmp/got-cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "got-cli-0.0.7.tar", last modified: Sat May  4 20:12:22 2024, max compression
+gzip compressed data, was "got-cli-0.0.8.tar", last modified: Sat May  4 20:20:06 2024, max compression
```

## Comparing `got-cli-0.0.7.tar` & `got-cli-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.154304 got-cli-0.0.7/
--rw-r--r--   0 guialves   (501) staff       (20)     1066 2024-05-04 19:36:59.000000 got-cli-0.0.7/LICENSE
--rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 20:12:22.154105 got-cli-0.0.7/PKG-INFO
--rw-r--r--   0 guialves   (501) staff       (20)     2039 2024-05-04 20:11:18.000000 got-cli-0.0.7/README.md
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.152471 got-cli-0.0.7/got/
--rw-r--r--   0 guialves   (501) staff       (20)        0 2024-05-04 17:10:40.000000 got-cli-0.0.7/got/__init__.py
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.152999 got-cli-0.0.7/got/ai/
--rw-r--r--   0 guialves   (501) staff       (20)     2242 2024-05-04 19:31:02.000000 got-cli-0.0.7/got/ai/__init__.py
--rw-r--r--   0 guialves   (501) staff       (20)     1210 2024-05-04 18:10:34.000000 got-cli-0.0.7/got/ai/chatgpt.py
--rw-r--r--   0 guialves   (501) staff       (20)      545 2024-05-04 18:20:32.000000 got-cli-0.0.7/got/ai/factory.py
--rw-r--r--   0 guialves   (501) staff       (20)     1326 2024-05-04 18:17:57.000000 got-cli-0.0.7/got/ai/groq.py
--rw-r--r--   0 guialves   (501) staff       (20)     4473 2024-05-04 19:46:00.000000 got-cli-0.0.7/got/cli.py
--rw-r--r--   0 guialves   (501) staff       (20)     2104 2024-05-04 19:41:42.000000 got-cli-0.0.7/got/commit.py
--rw-r--r--   0 guialves   (501) staff       (20)     2649 2024-05-04 20:00:46.000000 got-cli-0.0.7/got/git.py
--rw-r--r--   0 guialves   (501) staff       (20)     1945 2024-05-04 16:57:28.000000 got-cli-0.0.7/got/printer.py
-drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:12:22.153781 got-cli-0.0.7/got_cli.egg-info/
--rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/PKG-INFO
--rw-r--r--   0 guialves   (501) staff       (20)      351 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/SOURCES.txt
--rw-r--r--   0 guialves   (501) staff       (20)        1 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/dependency_links.txt
--rw-r--r--   0 guialves   (501) staff       (20)       37 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/entry_points.txt
--rw-r--r--   0 guialves   (501) staff       (20)       79 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/requires.txt
--rw-r--r--   0 guialves   (501) staff       (20)        4 2024-05-04 20:12:22.000000 got-cli-0.0.7/got_cli.egg-info/top_level.txt
--rw-r--r--   0 guialves   (501) staff       (20)       38 2024-05-04 20:12:22.154489 got-cli-0.0.7/setup.cfg
--rw-r--r--   0 guialves   (501) staff       (20)      658 2024-05-04 20:12:22.000000 got-cli-0.0.7/setup.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:20:06.468699 got-cli-0.0.8/
+-rw-r--r--   0 guialves   (501) staff       (20)     1066 2024-05-04 19:36:59.000000 got-cli-0.0.8/LICENSE
+-rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 20:20:06.468481 got-cli-0.0.8/PKG-INFO
+-rw-r--r--   0 guialves   (501) staff       (20)     2035 2024-05-04 20:15:53.000000 got-cli-0.0.8/README.md
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:20:06.465340 got-cli-0.0.8/got/
+-rw-r--r--   0 guialves   (501) staff       (20)        0 2024-05-04 17:10:40.000000 got-cli-0.0.8/got/__init__.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:20:06.466366 got-cli-0.0.8/got/ai/
+-rw-r--r--   0 guialves   (501) staff       (20)     2242 2024-05-04 19:31:02.000000 got-cli-0.0.8/got/ai/__init__.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1210 2024-05-04 18:10:34.000000 got-cli-0.0.8/got/ai/chatgpt.py
+-rw-r--r--   0 guialves   (501) staff       (20)      545 2024-05-04 18:20:32.000000 got-cli-0.0.8/got/ai/factory.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1326 2024-05-04 18:17:57.000000 got-cli-0.0.8/got/ai/groq.py
+-rw-r--r--   0 guialves   (501) staff       (20)     4479 2024-05-04 20:20:02.000000 got-cli-0.0.8/got/cli.py
+-rw-r--r--   0 guialves   (501) staff       (20)     2104 2024-05-04 19:41:42.000000 got-cli-0.0.8/got/commit.py
+-rw-r--r--   0 guialves   (501) staff       (20)     2649 2024-05-04 20:00:46.000000 got-cli-0.0.8/got/git.py
+-rw-r--r--   0 guialves   (501) staff       (20)     1945 2024-05-04 16:57:28.000000 got-cli-0.0.8/got/printer.py
+drwxr-xr-x   0 guialves   (501) staff       (20)        0 2024-05-04 20:20:06.467647 got-cli-0.0.8/got_cli.egg-info/
+-rw-r--r--   0 guialves   (501) staff       (20)      293 2024-05-04 20:20:06.000000 got-cli-0.0.8/got_cli.egg-info/PKG-INFO
+-rw-r--r--   0 guialves   (501) staff       (20)      351 2024-05-04 20:20:06.000000 got-cli-0.0.8/got_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 guialves   (501) staff       (20)        1 2024-05-04 20:20:06.000000 got-cli-0.0.8/got_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       37 2024-05-04 20:20:06.000000 got-cli-0.0.8/got_cli.egg-info/entry_points.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       79 2024-05-04 20:20:06.000000 got-cli-0.0.8/got_cli.egg-info/requires.txt
+-rw-r--r--   0 guialves   (501) staff       (20)        4 2024-05-04 20:20:06.000000 got-cli-0.0.8/got_cli.egg-info/top_level.txt
+-rw-r--r--   0 guialves   (501) staff       (20)       38 2024-05-04 20:20:06.468759 got-cli-0.0.8/setup.cfg
+-rw-r--r--   0 guialves   (501) staff       (20)      658 2024-05-04 20:20:06.000000 got-cli-0.0.8/setup.py
```

### Comparing `got-cli-0.0.7/LICENSE` & `got-cli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/README.md` & `got-cli-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GOT-CLI
+# GOT
 
 GOT is a command-line tool designed to enhance your git workflow by integrating AI-driven commit message suggestions. It leverages models from both OpenAI and Groq to suggest relevant commit messages based on the changes you've made.
 
 ## Features
 
 - **AI-Driven Commit Suggestions**: Utilize models like GPT-3.5, GPT-4, and various Groq models to generate commit messages.
 - **Interactive Commit Process**: Choose commit messages from suggested options or enter manually.
```

### Comparing `got-cli-0.0.7/got/ai/__init__.py` & `got-cli-0.0.8/got/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/got/ai/chatgpt.py` & `got-cli-0.0.8/got/ai/chatgpt.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/got/ai/factory.py` & `got-cli-0.0.8/got/ai/factory.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/got/ai/groq.py` & `got-cli-0.0.8/got/ai/groq.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/got/cli.py` & `got-cli-0.0.8/got/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         if commit_message == "Abort":
             printer.print("Aborted!", "red", 1, 1)
             exit()
 
         if commit_message == "Manual":
             printer.br()
-            commit_message = prompt("Enter a commit message: ")
+            commit_message = click.prompt("Enter a commit message: ")
 
         else:
             change_commit_message = inquirer.select(
                 message=f"Would you like to edit the selected message?",
                 choices=["No", "Yes"],
             ).execute()
```

### Comparing `got-cli-0.0.7/got/commit.py` & `got-cli-0.0.8/got/commit.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/got/git.py` & `got-cli-0.0.8/got/git.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/got/printer.py` & `got-cli-0.0.8/got/printer.py`

 * *Files identical despite different names*

### Comparing `got-cli-0.0.7/setup.py` & `got-cli-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="got-cli",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     license="MIT",
     install_requires=[
         "openai==1.25.1",
         "groq==0.5.0",
         "click==8.1.3",
         "python-dotenv==1.0.1",
```

