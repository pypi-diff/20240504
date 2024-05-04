# Comparing `tmp/streamlit_analytics2-0.7.2.tar.gz` & `tmp/streamlit_analytics2-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_analytics2-0.7.2.tar", last modified: Mon Apr 15 19:14:51 2024, max compression
+gzip compressed data, was "streamlit_analytics2-0.7.3.tar", last modified: Sat May  4 06:03:36 2024, max compression
```

## Comparing `streamlit_analytics2-0.7.2.tar` & `streamlit_analytics2-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:51.003273 streamlit_analytics2-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:50.999273 streamlit_analytics2-0.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/.github/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-15 19:14:50.999273 streamlit_analytics2-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:14:51.003273 streamlit_analytics2-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:50.999273 streamlit_analytics2-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:50.999273 streamlit_analytics2-0.7.2/src/streamlit_analytics2/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2/firestore.py
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:50.999273 streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-15 19:14:50.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-15 19:14:50.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:14:50.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:14:50.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:14:50.000000 streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:14:50.999273 streamlit_analytics2-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-15 19:14:12.000000 streamlit_analytics2-0.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.724917 streamlit_analytics2-0.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/.github/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.724917 streamlit_analytics2-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.724917 streamlit_analytics2-0.7.3/src/streamlit_analytics2/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/tests/test_utils.py
```

### Comparing `streamlit_analytics2-0.7.2/.github/README.md` & `streamlit_analytics2-0.7.3/.github/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-# streamlit-analytics2 &nbsp;👀
-
+# streamlit-analytics2 👀
 [![PyPi](https://img.shields.io/pypi/v/streamlit-analytics2)](https://pypi.org/project/streamlit-analytics2/)
+[![CodeFactor](https://www.codefactor.io/repository/github/444b/streamlit-analytics2/badge)](https://www.codefactor.io/repository/github/444b/streamlit-analytics2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-analytics2)](https://pypi.org/project/streamlit-analytics2/)
+![Build Status](https://github.com/444B/streamlit-analytics2/actions/workflows/release.yml/badge.svg)
+![Coverage](https://codecov.io/gh/444B/streamlit-analytics2/branch/main/graph/badge.svg)
+
 
 **Enhanced tracking & visualization for your Streamlit apps.**
 
 `streamlit-analytics2` is a fork and extension of the original [streamlit-analytics](https://github.com/jrieke/streamlit-analytics), aimed at improving and securing the analytics functionality within Streamlit applications. With minimal setup, track user interactions and visualize analytics directly in your browser, akin to Google Analytics but tailored for Streamlit.
 
 This fork was initiated due to the inability to collaborate directly on the upstream project, which currently has several unresolved security issues and bugs. Our intention is to maintain a positive relationship with the original project and its creator, focusing on enhancing the tool's reliability and security for the community.
```

### Comparing `streamlit_analytics2-0.7.2/LICENSE` & `streamlit_analytics2-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.2/PKG-INFO` & `streamlit_analytics2-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_analytics2
-Version: 0.7.2
+Version: 0.7.3
 Summary: Track & visualize user interactions with your streamlit app.
 Author-email: 444B <contact+pypi@444b.me>
 License: MIT License
         
         Copyright (c) 2021 Johannes Rieke
         
         Copyright (c) 2024 444B
@@ -46,17 +46,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=1.31.0
 Requires-Dist: pandas
 Requires-Dist: altair
 Requires-Dist: google-cloud-firestore
 
-# streamlit-analytics2 &nbsp;👀
-
+# streamlit-analytics2 👀
 [![PyPi](https://img.shields.io/pypi/v/streamlit-analytics2)](https://pypi.org/project/streamlit-analytics2/)
+[![CodeFactor](https://www.codefactor.io/repository/github/444b/streamlit-analytics2/badge)](https://www.codefactor.io/repository/github/444b/streamlit-analytics2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-analytics2)](https://pypi.org/project/streamlit-analytics2/)
+![Build Status](https://github.com/444B/streamlit-analytics2/actions/workflows/release.yml/badge.svg)
+![Coverage](https://codecov.io/gh/444B/streamlit-analytics2/branch/main/graph/badge.svg)
+
 
 **Enhanced tracking & visualization for your Streamlit apps.**
 
 `streamlit-analytics2` is a fork and extension of the original [streamlit-analytics](https://github.com/jrieke/streamlit-analytics), aimed at improving and securing the analytics functionality within Streamlit applications. With minimal setup, track user interactions and visualize analytics directly in your browser, akin to Google Analytics but tailored for Streamlit.
 
 This fork was initiated due to the inability to collaborate directly on the upstream project, which currently has several unresolved security issues and bugs. Our intention is to maintain a positive relationship with the original project and its creator, focusing on enhancing the tool's reliability and security for the community.
```

### Comparing `streamlit_analytics2-0.7.2/pyproject.toml` & `streamlit_analytics2-0.7.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.1.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_analytics2"
-version = "0.7.2"
+version = "0.7.3"
 description = "Track & visualize user interactions with your streamlit app."
 authors = [{ name = "444B", email = "contact+pypi@444b.me" }]
 license = { file = "LICENSE" }
 readme = {file = ".github/README.md", content-type = "text/markdown"}
 keywords = ["streamlit", "analytics", "visualization", "streamlit-analytics", "streamlit-analytics2"]
 classifiers = [
     "Programming Language :: Python :: 3.9",
```

### Comparing `streamlit_analytics2-0.7.2/src/streamlit_analytics2/display.py` & `streamlit_analytics2-0.7.3/src/streamlit_analytics2/display.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.2/src/streamlit_analytics2/firestore.py` & `streamlit_analytics2-0.7.3/src/streamlit_analytics2/firestore.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.2/src/streamlit_analytics2/main.py` & `streamlit_analytics2-0.7.3/src/streamlit_analytics2/main.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.2/src/streamlit_analytics2/utils.py` & `streamlit_analytics2-0.7.3/src/streamlit_analytics2/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.2/src/streamlit_analytics2.egg-info/PKG-INFO` & `streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_analytics2
-Version: 0.7.2
+Version: 0.7.3
 Summary: Track & visualize user interactions with your streamlit app.
 Author-email: 444B <contact+pypi@444b.me>
 License: MIT License
         
         Copyright (c) 2021 Johannes Rieke
         
         Copyright (c) 2024 444B
@@ -46,17 +46,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=1.31.0
 Requires-Dist: pandas
 Requires-Dist: altair
 Requires-Dist: google-cloud-firestore
 
-# streamlit-analytics2 &nbsp;👀
-
+# streamlit-analytics2 👀
 [![PyPi](https://img.shields.io/pypi/v/streamlit-analytics2)](https://pypi.org/project/streamlit-analytics2/)
+[![CodeFactor](https://www.codefactor.io/repository/github/444b/streamlit-analytics2/badge)](https://www.codefactor.io/repository/github/444b/streamlit-analytics2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/streamlit-analytics2)](https://pypi.org/project/streamlit-analytics2/)
+![Build Status](https://github.com/444B/streamlit-analytics2/actions/workflows/release.yml/badge.svg)
+![Coverage](https://codecov.io/gh/444B/streamlit-analytics2/branch/main/graph/badge.svg)
+
 
 **Enhanced tracking & visualization for your Streamlit apps.**
 
 `streamlit-analytics2` is a fork and extension of the original [streamlit-analytics](https://github.com/jrieke/streamlit-analytics), aimed at improving and securing the analytics functionality within Streamlit applications. With minimal setup, track user interactions and visualize analytics directly in your browser, akin to Google Analytics but tailored for Streamlit.
 
 This fork was initiated due to the inability to collaborate directly on the upstream project, which currently has several unresolved security issues and bugs. Our intention is to maintain a positive relationship with the original project and its creator, focusing on enhancing the tool's reliability and security for the community.
```

### Comparing `streamlit_analytics2-0.7.2/tests/test_utils.py` & `streamlit_analytics2-0.7.3/tests/test_utils.py`

 * *Files identical despite different names*

