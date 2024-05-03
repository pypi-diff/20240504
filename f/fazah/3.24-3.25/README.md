# Comparing `tmp/fazah-3.24.tar.gz` & `tmp/fazah-3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazah-3.24.tar", last modified: Fri May  3 20:31:33 2024, max compression
+gzip compressed data, was "fazah-3.25.tar", last modified: Fri May  3 21:21:26 2024, max compression
```

## Comparing `fazah-3.24.tar` & `fazah-3.25.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:31:33.324625 fazah-3.24/
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:31:33.323007 fazah-3.24/Fazah/
--rw-r--r--   0 aidenlang   (502) staff       (20)       51 2024-05-03 20:30:04.000000 fazah-3.24/Fazah/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1222 2024-05-03 20:23:26.000000 fazah-3.24/Fazah/fazah.py
--rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 20:31:33.324437 fazah-3.24/PKG-INFO
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:31:33.324258 fazah-3.24/fazah.egg-info/
--rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 20:31:33.000000 fazah-3.24/fazah.egg-info/PKG-INFO
--rw-r--r--   0 aidenlang   (502) staff       (20)      227 2024-05-03 20:31:33.000000 fazah-3.24/fazah.egg-info/SOURCES.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 20:31:33.000000 fazah-3.24/fazah.egg-info/dependency_links.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       27 2024-05-03 20:31:33.000000 fazah-3.24/fazah.egg-info/requires.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        6 2024-05-03 20:31:33.000000 fazah-3.24/fazah.egg-info/top_level.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 20:31:33.324664 fazah-3.24/setup.cfg
--rw-r--r--   0 aidenlang   (502) staff       (20)      496 2024-05-03 20:31:03.000000 fazah-3.24/setup.py
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:31:33.323978 fazah-3.24/tests/
--rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.24/tests/test.openai.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.24/tests/test_gemini.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 21:21:26.057250 fazah-3.25/
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 21:21:26.055667 fazah-3.25/Fazah/
+-rw-r--r--   0 aidenlang   (502) staff       (20)       28 2024-05-03 21:20:42.000000 fazah-3.25/Fazah/__init__.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1222 2024-05-03 20:23:26.000000 fazah-3.25/Fazah/fazah.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 21:21:26.057068 fazah-3.25/PKG-INFO
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 21:21:26.056863 fazah-3.25/fazah.egg-info/
+-rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 21:21:26.000000 fazah-3.25/fazah.egg-info/PKG-INFO
+-rw-r--r--   0 aidenlang   (502) staff       (20)      227 2024-05-03 21:21:26.000000 fazah-3.25/fazah.egg-info/SOURCES.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 21:21:26.000000 fazah-3.25/fazah.egg-info/dependency_links.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       27 2024-05-03 21:21:26.000000 fazah-3.25/fazah.egg-info/requires.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        6 2024-05-03 21:21:26.000000 fazah-3.25/fazah.egg-info/top_level.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 21:21:26.057289 fazah-3.25/setup.cfg
+-rw-r--r--   0 aidenlang   (502) staff       (20)      496 2024-05-03 21:21:21.000000 fazah-3.25/setup.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 21:21:26.056594 fazah-3.25/tests/
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.25/tests/test.openai.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.25/tests/test_gemini.py
```

### Comparing `fazah-3.24/Fazah/fazah.py` & `fazah-3.25/Fazah/fazah.py`

 * *Files identical despite different names*

### Comparing `fazah-3.24/tests/test.openai.py` & `fazah-3.25/tests/test.openai.py`

 * *Files identical despite different names*

### Comparing `fazah-3.24/tests/test_gemini.py` & `fazah-3.25/tests/test_gemini.py`

 * *Files identical despite different names*

