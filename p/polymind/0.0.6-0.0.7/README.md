# Comparing `tmp/polymind-0.0.6.tar.gz` & `tmp/polymind-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymind-0.0.6.tar", last modified: Fri Mar  1 02:12:56 2024, max compression
+gzip compressed data, was "polymind-0.0.7.tar", last modified: Fri Mar  1 02:45:01 2024, max compression
```

## Comparing `polymind-0.0.6.tar` & `polymind-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:12:56.928917 polymind-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-01 02:12:47.000000 polymind-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-01 02:12:56.928917 polymind-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-01 02:12:47.000000 polymind-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:12:56.928917 polymind-0.0.6/polymind/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-01 02:12:47.000000 polymind-0.0.6/polymind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-01 02:12:47.000000 polymind-0.0.6/polymind/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:12:56.928917 polymind-0.0.6/polymind.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-01 02:12:56.000000 polymind-0.0.6/polymind.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-01 02:12:56.000000 polymind-0.0.6/polymind.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 02:12:56.000000 polymind-0.0.6/polymind.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-01 02:12:56.000000 polymind-0.0.6/polymind.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 02:12:56.000000 polymind-0.0.6/polymind.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-01 02:12:47.000000 polymind-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 02:12:56.928917 polymind-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-01 02:12:47.000000 polymind-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:45:01.820162 polymind-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-01 02:44:48.000000 polymind-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-01 02:45:01.820162 polymind-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-01 02:44:48.000000 polymind-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:45:01.816162 polymind-0.0.7/polymind/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-01 02:44:48.000000 polymind-0.0.7/polymind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-01 02:44:48.000000 polymind-0.0.7/polymind/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:45:01.820162 polymind-0.0.7/polymind.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-01 02:45:01.000000 polymind-0.0.7/polymind.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-01 02:45:01.000000 polymind-0.0.7/polymind.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 02:45:01.000000 polymind-0.0.7/polymind.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 02:45:01.000000 polymind-0.0.7/polymind.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-01 02:44:48.000000 polymind-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 02:45:01.820162 polymind-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-01 02:44:48.000000 polymind-0.0.7/setup.py
```

### Comparing `polymind-0.0.6/LICENSE` & `polymind-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polymind-0.0.6/PKG-INFO` & `polymind-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: polymind
-Version: 0.0.6
-Summary: PolyMind is a cutting-edge multi-agent framework focused on leveraging collective intelligence
+Version: 0.0.7
+Summary:      PolyMind is a cutting-edge multi-agent framework focused on leveraging collective intelligence     to solve complex problems.     
 Home-page: https://github.com/small-thinking/polymind
 Author: Small Thinking
 Author-email: yjiang@small-thinking.org
 License: MIT
 Keywords: multi-agent,collective intelligence,problem solving,polymind
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PolyMind (群策) 
 
 ![PolyMind Logo](images/polymind-logo.png)
 
@@ -37,7 +38,9 @@
 
 To get started with PolyMind, clone the repository and follow the installation instructions:
 
 ```bash
 git clone https://github.com/your-username/polymind.git
 cd polymind
 ```
+
+
```

### Comparing `polymind-0.0.6/README.md` & `polymind-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `polymind-0.0.6/polymind.egg-info/PKG-INFO` & `polymind-0.0.7/polymind.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: polymind
-Version: 0.0.6
-Summary: PolyMind is a cutting-edge multi-agent framework focused on leveraging collective intelligence
+Version: 0.0.7
+Summary:      PolyMind is a cutting-edge multi-agent framework focused on leveraging collective intelligence     to solve complex problems.     
 Home-page: https://github.com/small-thinking/polymind
 Author: Small Thinking
 Author-email: yjiang@small-thinking.org
 License: MIT
 Keywords: multi-agent,collective intelligence,problem solving,polymind
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PolyMind (群策) 
 
 ![PolyMind Logo](images/polymind-logo.png)
 
@@ -37,7 +38,9 @@
 
 To get started with PolyMind, clone the repository and follow the installation instructions:
 
 ```bash
 git clone https://github.com/your-username/polymind.git
 cd polymind
 ```
+
+
```

### Comparing `polymind-0.0.6/pyproject.toml` & `polymind-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = "0.1.0"
 description = "PolyMind is a customizable collaborative multi-agent framework for collective intelligence and distributed problem solving."
 authors = ["Yx Jiang <2237303+yxjiang@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.10.13"
+python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 isort = "^5.13.2"
 flake8 = "^7.0.0"
 
 [build-system]
```

### Comparing `polymind-0.0.6/setup.py` & `polymind-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     requirements = f.read().splitlines()
 
 repo = Path(__file__).resolve().parent
 long_description = (repo / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="polymind",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     install_requires=requirements,
     author="Small Thinking",
     author_email="yjiang@small-thinking.org",
     description="""
     PolyMind is a cutting-edge multi-agent framework focused on leveraging collective intelligence
     to solve complex problems.
     """,
     long_description=long_description,
     license="MIT",
-    python_requires=">=3.10",
+    python_requires=">=3.9",
     keywords="multi-agent, collective intelligence, problem solving, polymind",
     long_description_content_type="text/markdown",
     url="https://github.com/small-thinking/polymind",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

