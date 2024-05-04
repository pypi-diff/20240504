# Comparing `tmp/lfg_llama-1.2.1.tar.gz` & `tmp/lfg_llama-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.2.1.tar", last modified: Sat May  4 07:31:39 2024, max compression
+gzip compressed data, was "lfg_llama-1.2.2.tar", last modified: Sat May  4 07:33:02 2024, max compression
```

## Comparing `lfg_llama-1.2.1.tar` & `lfg_llama-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 07:31:39.183096 lfg_llama-1.2.1/
--rw-r--r--   0 ob907      (502) staff       (20)     1334 2024-05-04 07:31:39.182895 lfg_llama-1.2.1/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1097 2024-05-04 07:25:12.000000 lfg_llama-1.2.1/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 07:31:39.181769 lfg_llama-1.2.1/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.2.1/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     3113 2024-05-04 07:31:26.000000 lfg_llama-1.2.1/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 07:31:39.182681 lfg_llama-1.2.1/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1334 2024-05-04 07:31:39.000000 lfg_llama-1.2.1/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-04 07:31:39.000000 lfg_llama-1.2.1/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-04 07:31:39.000000 lfg_llama-1.2.1/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-04 07:31:39.000000 lfg_llama-1.2.1/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-04 07:31:39.000000 lfg_llama-1.2.1/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-04 07:31:39.000000 lfg_llama-1.2.1/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-04 07:31:39.183166 lfg_llama-1.2.1/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-04 07:31:33.000000 lfg_llama-1.2.1/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 07:33:02.908182 lfg_llama-1.2.2/
+-rw-r--r--   0 ob907      (502) staff       (20)     1334 2024-05-04 07:33:02.907982 lfg_llama-1.2.2/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1097 2024-05-04 07:25:12.000000 lfg_llama-1.2.2/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 07:33:02.906747 lfg_llama-1.2.2/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.2.2/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     3098 2024-05-04 07:32:53.000000 lfg_llama-1.2.2/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 07:33:02.907776 lfg_llama-1.2.2/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1334 2024-05-04 07:33:02.000000 lfg_llama-1.2.2/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-04 07:33:02.000000 lfg_llama-1.2.2/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-04 07:33:02.000000 lfg_llama-1.2.2/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-04 07:33:02.000000 lfg_llama-1.2.2/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-04 07:33:02.000000 lfg_llama-1.2.2/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-04 07:33:02.000000 lfg_llama-1.2.2/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-04 07:33:02.908250 lfg_llama-1.2.2/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-04 07:32:58.000000 lfg_llama-1.2.2/setup.py
```

### Comparing `lfg_llama-1.2.1/PKG-INFO` & `lfg_llama-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.2.1
+Version: 1.2.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

### Comparing `lfg_llama-1.2.1/README.md` & `lfg_llama-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.2.1/lfg/cli.py` & `lfg_llama-1.2.2/lfg/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     parser.add_argument(
         "-m",
         choices=["llama38b", "llama370b", "mixtral8x7b", "gemma7b"],
         default="llama370b",
         help="Select the language model.",
     )
     args = parser.parse_args()
-    print(args)
+
     try:
         client = get_groq_client()
         send_chat_query(args.query, args.m.upper(), client)
 
         return
     except ValueError as e:
         print(f"Error: {e}")
```

### Comparing `lfg_llama-1.2.1/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.2.2/lfg_llama.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.2.1
+Version: 1.2.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

