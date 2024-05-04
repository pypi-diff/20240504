# Comparing `tmp/tabletalk-0.0.8.tar.gz` & `tmp/tabletalk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabletalk-0.0.8.tar", last modified: Fri Apr 19 21:23:30 2024, max compression
+gzip compressed data, was "tabletalk-0.0.9.tar", last modified: Sat May  4 03:27:35 2024, max compression
```

## Comparing `tabletalk-0.0.8.tar` & `tabletalk-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 21:23:30.004016 tabletalk-0.0.8/
--rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.8/LICENSE
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 21:23:30.003763 tabletalk-0.0.8/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.8/README.md
--rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 21:23:30.004062 tabletalk-0.0.8/setup.cfg
--rw-r--r--   0 vinceberry   (501) staff       (20)     1155 2024-04-19 21:14:48.000000 tabletalk-0.0.8/setup.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 21:23:30.002685 tabletalk-0.0.8/tabletalk/
--rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.8/tabletalk/__init__.py
--rw-r--r--   0 vinceberry   (501) staff       (20)     3944 2024-04-19 21:20:32.000000 tabletalk-0.0.8/tabletalk/talk.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 21:23:30.003534 tabletalk-0.0.8/tabletalk.egg-info/
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 21:23:29.000000 tabletalk-0.0.8/tabletalk.egg-info/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 21:23:30.000000 tabletalk-0.0.8/tabletalk.egg-info/SOURCES.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 21:23:29.000000 tabletalk-0.0.8/tabletalk.egg-info/dependency_links.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 21:23:29.000000 tabletalk-0.0.8/tabletalk.egg-info/requires.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 21:23:29.000000 tabletalk-0.0.8/tabletalk.egg-info/top_level.txt
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-05-04 03:27:35.168773 tabletalk-0.0.9/
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.9/LICENSE
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-05-04 03:27:35.168548 tabletalk-0.0.9/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.9/README.md
+-rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-05-04 03:27:35.168825 tabletalk-0.0.9/setup.cfg
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1155 2024-05-04 03:27:23.000000 tabletalk-0.0.9/setup.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-05-04 03:27:35.167505 tabletalk-0.0.9/tabletalk/
+-rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.9/tabletalk/__init__.py
+-rw-r--r--   0 vinceberry   (501) staff       (20)     2949 2024-05-04 02:55:01.000000 tabletalk-0.0.9/tabletalk/sql_prompt.py
+-rw-r--r--   0 vinceberry   (501) staff       (20)     9044 2024-05-04 03:16:27.000000 tabletalk-0.0.9/tabletalk/talk.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-05-04 03:27:35.168344 tabletalk-0.0.9/tabletalk.egg-info/
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-05-04 03:27:35.000000 tabletalk-0.0.9/tabletalk.egg-info/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)      254 2024-05-04 03:27:35.000000 tabletalk-0.0.9/tabletalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-05-04 03:27:35.000000 tabletalk-0.0.9/tabletalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-05-04 03:27:35.000000 tabletalk-0.0.9/tabletalk.egg-info/requires.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-05-04 03:27:35.000000 tabletalk-0.0.9/tabletalk.egg-info/top_level.txt
```

### Comparing `tabletalk-0.0.8/LICENSE` & `tabletalk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.8/PKG-INFO` & `tabletalk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.8
+Version: 0.0.9
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tabletalk-0.0.8/setup.py` & `tabletalk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'NL2SQL2RAG'
 LONG_DESCRIPTION = 'TableTalk allows you ask query your tabular data with natural language, then produces a generated response.'
 
 setup(
     name="tabletalk",
     version=VERSION,
     author="Vince Berry",
```

### Comparing `tabletalk-0.0.8/tabletalk.egg-info/PKG-INFO` & `tabletalk-0.0.9/tabletalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.8
+Version: 0.0.9
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

