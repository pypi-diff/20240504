# Comparing `tmp/manabase_solver-0.1.1.tar.gz` & `tmp/manabase_solver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manabase_solver-0.1.1.tar", last modified: Fri May  3 19:57:12 2024, max compression
+gzip compressed data, was "manabase_solver-0.1.2.tar", last modified: Fri May  3 23:43:11 2024, max compression
```

## Comparing `manabase_solver-0.1.1.tar` & `manabase_solver-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 19:57:12.138412 manabase_solver-0.1.1/
--rw-r--r--   0 bakert     (501) wheel        (0)     1075 2024-03-30 23:26:22.000000 manabase_solver-0.1.1/LICENSE
--rw-r--r--   0 bakert     (501) wheel        (0)     3090 2024-05-03 19:57:12.138213 manabase_solver-0.1.1/PKG-INFO
--rw-r--r--   0 bakert     (501) wheel        (0)     1124 2024-05-03 19:53:53.000000 manabase_solver-0.1.1/README.md
--rw-r--r--   0 bakert     (501) wheel        (0)      819 2024-05-03 19:56:32.000000 manabase_solver-0.1.1/pyproject.toml
--rw-r--r--   0 bakert     (501) wheel        (0)       38 2024-05-03 19:57:12.138451 manabase_solver-0.1.1/setup.cfg
-drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 19:57:12.134923 manabase_solver-0.1.1/src/
-drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 19:57:12.137315 manabase_solver-0.1.1/src/manabase_solver/
--rw-r--r--   0 bakert     (501) wheel        (0)      165 2024-05-03 19:37:23.000000 manabase_solver-0.1.1/src/manabase_solver/__init__.py
--rw-r--r--   0 bakert     (501) wheel        (0)     7811 2024-05-03 19:42:38.000000 manabase_solver-0.1.1/src/manabase_solver/lands.py
--rw-r--r--   0 bakert     (501) wheel        (0)    45565 2024-05-03 18:27:34.000000 manabase_solver-0.1.1/src/manabase_solver/manabase_solver.py
--rw-r--r--   0 bakert     (501) wheel        (0)    11431 2024-05-03 19:37:23.000000 manabase_solver-0.1.1/src/manabase_solver/manabase_solver_test.py
--rw-r--r--   0 bakert     (501) wheel        (0)        0 2024-05-03 18:02:21.000000 manabase_solver-0.1.1/src/manabase_solver/py.typed
--rw-r--r--   0 bakert     (501) wheel        (0)     2253 2024-04-10 00:28:57.000000 manabase_solver-0.1.1/src/manabase_solver/remembering_model.py
--rw-r--r--   0 bakert     (501) wheel        (0)      325 2024-05-03 18:26:10.000000 manabase_solver-0.1.1/src/manabase_solver/remembering_model_test.py
-drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 19:57:12.138015 manabase_solver-0.1.1/src/manabase_solver.egg-info/
--rw-r--r--   0 bakert     (501) wheel        (0)     3090 2024-05-03 19:57:12.000000 manabase_solver-0.1.1/src/manabase_solver.egg-info/PKG-INFO
--rw-r--r--   0 bakert     (501) wheel        (0)      464 2024-05-03 19:57:12.000000 manabase_solver-0.1.1/src/manabase_solver.egg-info/SOURCES.txt
--rw-r--r--   0 bakert     (501) wheel        (0)        1 2024-05-03 19:57:12.000000 manabase_solver-0.1.1/src/manabase_solver.egg-info/dependency_links.txt
--rw-r--r--   0 bakert     (501) wheel        (0)       16 2024-05-03 19:57:12.000000 manabase_solver-0.1.1/src/manabase_solver.egg-info/top_level.txt
+drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 23:43:11.136670 manabase_solver-0.1.2/
+-rw-r--r--   0 bakert     (501) wheel        (0)      124 2024-05-03 18:31:17.000000 manabase_solver-0.1.2/.gitignore
+-rw-r--r--   0 bakert     (501) wheel        (0)     1075 2024-03-30 23:26:22.000000 manabase_solver-0.1.2/LICENSE
+-rw-r--r--   0 bakert     (501) wheel        (0)      409 2024-04-10 06:09:38.000000 manabase_solver-0.1.2/Makefile
+-rw-r--r--   0 bakert     (501) wheel        (0)     3167 2024-05-03 23:43:11.136480 manabase_solver-0.1.2/PKG-INFO
+-rw-r--r--   0 bakert     (501) wheel        (0)     1124 2024-05-03 19:53:53.000000 manabase_solver-0.1.2/README.md
+-rw-r--r--   0 bakert     (501) wheel        (0)      918 2024-05-03 23:42:22.000000 manabase_solver-0.1.2/pyproject.toml
+-rw-r--r--   0 bakert     (501) wheel        (0)       49 2024-05-03 19:01:35.000000 manabase_solver-0.1.2/requirements-dev.txt
+-rw-r--r--   0 bakert     (501) wheel        (0)       32 2024-04-09 21:12:37.000000 manabase_solver-0.1.2/requirements.txt
+drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 23:43:11.133503 manabase_solver-0.1.2/scripts/
+-rw-r--r--   0 bakert     (501) wheel        (0)     6461 2024-05-03 19:42:38.000000 manabase_solver-0.1.2/scripts/scratch.py
+-rw-r--r--   0 bakert     (501) wheel        (0)       38 2024-05-03 23:43:11.136712 manabase_solver-0.1.2/setup.cfg
+drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 23:43:11.131947 manabase_solver-0.1.2/src/
+drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 23:43:11.135459 manabase_solver-0.1.2/src/manabase_solver/
+-rw-r--r--   0 bakert     (501) wheel        (0)      165 2024-05-03 19:37:23.000000 manabase_solver-0.1.2/src/manabase_solver/__init__.py
+-rw-r--r--   0 bakert     (501) wheel        (0)     7811 2024-05-03 19:42:38.000000 manabase_solver-0.1.2/src/manabase_solver/lands.py
+-rw-r--r--   0 bakert     (501) wheel        (0)    45565 2024-05-03 21:09:29.000000 manabase_solver-0.1.2/src/manabase_solver/manabase_solver.py
+-rw-r--r--   0 bakert     (501) wheel        (0)    11431 2024-05-03 19:37:23.000000 manabase_solver-0.1.2/src/manabase_solver/manabase_solver_test.py
+-rw-r--r--   0 bakert     (501) wheel        (0)        0 2024-05-03 18:02:21.000000 manabase_solver-0.1.2/src/manabase_solver/py.typed
+-rw-r--r--   0 bakert     (501) wheel        (0)     2253 2024-04-10 00:28:57.000000 manabase_solver-0.1.2/src/manabase_solver/remembering_model.py
+-rw-r--r--   0 bakert     (501) wheel        (0)      325 2024-05-03 18:26:10.000000 manabase_solver-0.1.2/src/manabase_solver/remembering_model_test.py
+drwxr-xr-x   0 bakert     (501) wheel        (0)        0 2024-05-03 23:43:11.136266 manabase_solver-0.1.2/src/manabase_solver.egg-info/
+-rw-r--r--   0 bakert     (501) wheel        (0)     3167 2024-05-03 23:43:11.000000 manabase_solver-0.1.2/src/manabase_solver.egg-info/PKG-INFO
+-rw-r--r--   0 bakert     (501) wheel        (0)      583 2024-05-03 23:43:11.000000 manabase_solver-0.1.2/src/manabase_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 bakert     (501) wheel        (0)        1 2024-05-03 23:43:11.000000 manabase_solver-0.1.2/src/manabase_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 bakert     (501) wheel        (0)       32 2024-05-03 23:43:11.000000 manabase_solver-0.1.2/src/manabase_solver.egg-info/requires.txt
+-rw-r--r--   0 bakert     (501) wheel        (0)       16 2024-05-03 23:43:11.000000 manabase_solver-0.1.2/src/manabase_solver.egg-info/top_level.txt
```

### Comparing `manabase_solver-0.1.1/LICENSE` & `manabase_solver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `manabase_solver-0.1.1/PKG-INFO` & `manabase_solver-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manabase-solver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Magic: the Gathering manabase solver
 Author-email: Thomas David Baker <bakert@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Thomas David Baker
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: more_itertools
+Requires-Dist: multiset
+Requires-Dist: ortools
 
 # manabase-solver
 
 Magic the Gathering manabase solver
 
 ## Usage
```

### Comparing `manabase_solver-0.1.1/README.md` & `manabase_solver-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `manabase_solver-0.1.1/pyproject.toml` & `manabase_solver-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "manabase-solver"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Thomas David Baker", email = "bakert@gmail.com"},
 ]
 description = "Magic: the Gathering manabase solver"
 readme = "README.md"
 requires-python = ">=3.12"
 license = {file = "LICENSE"}
@@ -16,12 +16,16 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Games/Entertainment",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.12",
 ]
+dynamic = ["dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/bakert/manabase-solver"
 Repository = "https://github.com/bakert/manabase-solver"
 Issues = "https://github.com/bakert/manabase-solver/issues"
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `manabase_solver-0.1.1/src/manabase_solver/lands.py` & `manabase_solver-0.1.2/src/manabase_solver/lands.py`

 * *Files identical despite different names*

### Comparing `manabase_solver-0.1.1/src/manabase_solver/manabase_solver.py` & `manabase_solver-0.1.2/src/manabase_solver/manabase_solver.py`

 * *Files identical despite different names*

### Comparing `manabase_solver-0.1.1/src/manabase_solver/manabase_solver_test.py` & `manabase_solver-0.1.2/src/manabase_solver/manabase_solver_test.py`

 * *Files identical despite different names*

### Comparing `manabase_solver-0.1.1/src/manabase_solver/remembering_model.py` & `manabase_solver-0.1.2/src/manabase_solver/remembering_model.py`

 * *Files identical despite different names*

### Comparing `manabase_solver-0.1.1/src/manabase_solver.egg-info/PKG-INFO` & `manabase_solver-0.1.2/src/manabase_solver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manabase-solver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Magic: the Gathering manabase solver
 Author-email: Thomas David Baker <bakert@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Thomas David Baker
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: more_itertools
+Requires-Dist: multiset
+Requires-Dist: ortools
 
 # manabase-solver
 
 Magic the Gathering manabase solver
 
 ## Usage
```

