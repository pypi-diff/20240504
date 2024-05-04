# Comparing `tmp/cgg-0.2.7.tar.gz` & `tmp/cgg-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgg-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cgg-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cgg-0.2.7.tar` & `cgg-0.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.7/LICENSE
--rw-r--r--   0        0        0     4066 2024-04-25 00:36:15.159266 cgg-0.2.7/README.md
--rw-r--r--   0        0        0      742 2024-04-25 00:32:11.783810 cgg-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5490 2024-04-25 00:31:01.107926 cgg-0.2.7/src/cgg/__init__.py
--rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 cgg-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4066 2024-04-25 00:36:15.159266 cgg-0.2.8/README.md
+-rw-r--r--   0        0        0      742 2024-04-25 00:32:11.783810 cgg-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     5563 2024-05-04 00:44:57.266735 cgg-0.2.8/src/cgg/__init__.py
+-rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 cgg-0.2.8/PKG-INFO
```

### Comparing `cgg-0.2.7/LICENSE` & `cgg-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cgg-0.2.7/README.md` & `cgg-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cgg-0.2.7/pyproject.toml` & `cgg-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cgg-0.2.7/src/cgg/__init__.py` & `cgg-0.2.8/src/cgg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # !/usr/bin/env python3
 
-__version__="0.2.7"
+__version__="0.2.8"
 
 import argparse, json, os.path, urllib.request
 from rich.progress import Progress
-# rich (refined) ###########################################################################
+# rich (refined) #######################################################################
 def get_file_size(url):
     with urllib.request.urlopen(url) as response:
         size = int(response.headers['Content-Length'])
     return size
 def format_size(size_bytes):
     return f"{size_bytes / (1024 * 1024):.2f} MB"
 def clone_file(url):
@@ -26,27 +26,24 @@
                         break
                     file.write(chunk)
                     downloaded += len(chunk)
                     progress.update(task, completed=downloaded, description=f"Downloading {filename} [green][{format_size(downloaded)} / {format_size(file_size)}]")
         print(f"File cloned successfully and saved as '{filename}'({format_size(file_size)}) in the current directory.")
     except Exception as e:
         print(f"Error: {e}")
-# ##########################################################################################
-        
+# ######################################################################################
 def read_json_file(file_path):
     response = urllib.request.urlopen(file_path)
     data = json.loads(response.read())
     # with open(file_path, 'r') as file:
         # data = json.load(file)
     return data
-
 def extract_names(data):
     for idx, entry in enumerate(data, start=1):
         print(f'{idx}. {entry["name"]}')
-
 def handle_user_input(data):
     while True:
         user_choice = input(f"Enter your choice (1 to {len(data)}) or 'q' to quit: ")
         if user_choice.lower() == 'q':
             break
         try:
             index = int(user_choice)
@@ -54,24 +51,24 @@
                 source_url = data[index - 1]["url"]
                 clone_file(source_url)
                 break
             else:
                 print("Invalid selection. Please enter a valid number.")
         except ValueError:
             print("Invalid input. Please enter a number.")
-
+# ######################################################################################
 def __init__():
     parser = argparse.ArgumentParser(description="cgg will execute different functions based on command-line arguments")
     parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
     # Subparser session below
     subparsers = parser.add_subparsers(title="subcommands", dest="subcommand", help="choose a subcommand:")
     # Subparser for 'clone [URL]' subcommand
     clone_parser = subparsers.add_parser('clone', help='download a GGUF file/model from URL')
     clone_parser.add_argument('url', type=str, help='URL to download from (i.e., cgg clone [url])')
-    # Subparser for 'menu/cpp/c/gpp/g/s/r/us' subcommand
+    # Subparser for 'menu/cpp/c/gpp/g/s/r/us...etc.' subcommand
     subparsers.add_parser('menu', help='connector selection list:')
     subparsers.add_parser('cpp', help='cpp connector')
     subparsers.add_parser('gpp', help='gpp connector')
     subparsers.add_parser('c', help='c connector')
     subparsers.add_parser('g', help='g connector')
     subparsers.add_parser('r', help='metadata reader')
     subparsers.add_parser('s', help='sample GGUF list (internet required)')
```

### Comparing `cgg-0.2.7/PKG-INFO` & `cgg-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgg
-Version: 0.2.7
+Version: 0.2.8
 Summary: cgg is a short form of call gguf model/file; cgg is a cmd-based app built on gguf-connector, which allows users interacting with large language model (i.e., chatgpt) via a simple command without coding a long long syntax
 Author-email: calcuis <info@calcu.io>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: gguf-connector >=0.7.31
 Project-URL: Homepage, https://github.com/calcuis/cgg
 Project-URL: Issues, https://github.com/calcuis/cgg/issues
```

