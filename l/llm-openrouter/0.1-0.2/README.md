# Comparing `tmp/llm-openrouter-0.1.tar.gz` & `tmp/llm_openrouter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-openrouter-0.1.tar", last modified: Mon Aug 21 07:04:22 2023, max compression
+gzip compressed data, was "llm_openrouter-0.2.tar", last modified: Fri May  3 23:58:46 2024, max compression
```

## Comparing `llm-openrouter-0.1.tar` & `llm_openrouter-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:04:22.599230 llm-openrouter-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-21 07:04:02.000000 llm-openrouter-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-21 07:04:22.599230 llm-openrouter-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-21 07:04:02.000000 llm-openrouter-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:04:22.599230 llm-openrouter-0.1/llm_openrouter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-21 07:04:22.000000 llm-openrouter-0.1/llm_openrouter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-21 07:04:22.000000 llm-openrouter-0.1/llm_openrouter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 07:04:22.000000 llm-openrouter-0.1/llm_openrouter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-21 07:04:22.000000 llm-openrouter-0.1/llm_openrouter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-21 07:04:22.000000 llm-openrouter-0.1/llm_openrouter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-21 07:04:22.000000 llm-openrouter-0.1/llm_openrouter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-21 07:04:02.000000 llm-openrouter-0.1/llm_openrouter.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-21 07:04:02.000000 llm-openrouter-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 07:04:22.599230 llm-openrouter-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:04:22.599230 llm-openrouter-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-21 07:04:02.000000 llm-openrouter-0.1/tests/test_llm_openrouter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:58:46.900744 llm_openrouter-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 23:58:31.000000 llm_openrouter-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-03 23:58:46.900744 llm_openrouter-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-03 23:58:31.000000 llm_openrouter-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:58:46.900744 llm_openrouter-0.2/llm_openrouter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-03 23:58:46.000000 llm_openrouter-0.2/llm_openrouter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-03 23:58:46.000000 llm_openrouter-0.2/llm_openrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:58:46.000000 llm_openrouter-0.2/llm_openrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 23:58:46.000000 llm_openrouter-0.2/llm_openrouter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 23:58:46.000000 llm_openrouter-0.2/llm_openrouter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 23:58:46.000000 llm_openrouter-0.2/llm_openrouter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-03 23:58:31.000000 llm_openrouter-0.2/llm_openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 23:58:31.000000 llm_openrouter-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 23:58:46.900744 llm_openrouter-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:58:46.900744 llm_openrouter-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-03 23:58:31.000000 llm_openrouter-0.2/tests/test_llm_openrouter.py
```

### Comparing `llm-openrouter-0.1/LICENSE` & `llm_openrouter-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-openrouter-0.1/PKG-INFO` & `llm_openrouter-0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: llm-openrouter
-Version: 0.1
+Version: 0.2
 Summary: LLM plugin for models hosted by OpenRouter
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-openrouter
 Project-URL: Changelog, https://github.com/simonw/llm-openrouter/releases
 Project-URL: Issues, https://github.com/simonw/llm-openrouter/issues
 Project-URL: CI, https://github.com/simonw/llm-openrouter/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: llm>=0.8
+Requires-Dist: httpx
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-httpx; extra == "test"
 
 # llm-openrouter
 
 [![PyPI](https://img.shields.io/pypi/v/llm-openrouter.svg)](https://pypi.org/project/llm-openrouter/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm-openrouter?include_prereleases&label=changelog)](https://github.com/simonw/llm-openrouter/releases)
 [![Tests](https://github.com/simonw/llm-openrouter/workflows/Test/badge.svg)](https://github.com/simonw/llm-openrouter/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm-openrouter/blob/main/LICENSE)
```

### Comparing `llm-openrouter-0.1/README.md` & `llm_openrouter-0.2/README.md`

 * *Files identical despite different names*

### Comparing `llm-openrouter-0.1/llm_openrouter.egg-info/PKG-INFO` & `llm_openrouter-0.2/llm_openrouter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: llm-openrouter
-Version: 0.1
+Version: 0.2
 Summary: LLM plugin for models hosted by OpenRouter
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-openrouter
 Project-URL: Changelog, https://github.com/simonw/llm-openrouter/releases
 Project-URL: Issues, https://github.com/simonw/llm-openrouter/issues
 Project-URL: CI, https://github.com/simonw/llm-openrouter/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: llm>=0.8
+Requires-Dist: httpx
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-httpx; extra == "test"
 
 # llm-openrouter
 
 [![PyPI](https://img.shields.io/pypi/v/llm-openrouter.svg)](https://pypi.org/project/llm-openrouter/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm-openrouter?include_prereleases&label=changelog)](https://github.com/simonw/llm-openrouter/releases)
 [![Tests](https://github.com/simonw/llm-openrouter/workflows/Test/badge.svg)](https://github.com/simonw/llm-openrouter/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm-openrouter/blob/main/LICENSE)
```

### Comparing `llm-openrouter-0.1/llm_openrouter.py` & `llm_openrouter-0.2/llm_openrouter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import llm
 from llm.default_plugins.openai_models import Chat
 from pathlib import Path
 import json
 import time
 import httpx
-import urllib3
 
 
 def get_openrouter_models():
     return fetch_cached_json(
         url="https://openrouter.ai/api/v1/models",
         path=llm.user_dir() / "openrouter_models.json",
         cache_timeout=3600,
     )["data"]
 
 
 class OpenRouterChat(Chat):
     needs_key = "openrouter"
+    key_env_var = "OPENROUTER_KEY"
 
     def __str__(self):
         return "OpenRouter: {}".format(self.model_id)
 
 
 @llm.hookimpl
 def register_models(register):
@@ -64,15 +64,15 @@
         response.raise_for_status()  # This will raise an HTTPError if the request fails
 
         # If successful, write to the file
         with open(path, "w") as file:
             json.dump(response.json(), file)
 
         return response.json()
-    except (httpx.HTTPError, urllib3.exceptions.NameResolutionError):
+    except httpx.HTTPError:
         # If there's an existing file, load it
         if path.is_file():
             with open(path, "r") as file:
                 return json.load(file)
         else:
             # If not, raise an error
             raise DownloadError(
```

### Comparing `llm-openrouter-0.1/pyproject.toml` & `llm_openrouter-0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "llm-openrouter"
-version = "0.1"
+version = "0.2"
 description = "LLM plugin for models hosted by OpenRouter"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "llm>=0.8",
+    "httpx"
 ]
 
 [project.urls]
 Homepage = "https://github.com/simonw/llm-openrouter"
 Changelog = "https://github.com/simonw/llm-openrouter/releases"
 Issues = "https://github.com/simonw/llm-openrouter/issues"
 CI = "https://github.com/simonw/llm-openrouter/actions"
```

### Comparing `llm-openrouter-0.1/tests/test_llm_openrouter.py` & `llm_openrouter-0.2/tests/test_llm_openrouter.py`

 * *Files identical despite different names*

