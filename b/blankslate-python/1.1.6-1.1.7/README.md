# Comparing `tmp/blankslate_python-1.1.6.tar.gz` & `tmp/blankslate_python-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankslate_python-1.1.6.tar", max compression
+gzip compressed data, was "blankslate_python-1.1.7.tar", max compression
```

## Comparing `blankslate_python-1.1.6.tar` & `blankslate_python-1.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.1.6/LICENSE
--rw-r--r--   0        0        0     2824 2024-05-04 21:11:01.839346 blankslate_python-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2245 2024-05-04 17:20:48.274142 blankslate_python-1.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.1.6/source/blankslate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.6/source/blankslate/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.1.6/source/blankslate/config/constants.py
--rw-r--r--   0        0        0      740 2024-05-04 20:47:22.274910 blankslate_python-1.1.6/source/blankslate/config/paths.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.6/source/blankslate/generation/__init__.py
--rw-r--r--   0        0        0     2539 2024-05-04 14:20:49.402998 blankslate_python-1.1.6/source/blankslate/generation/folder_generation.py
--rw-r--r--   0        0        0     7209 2024-05-04 20:59:12.550950 blankslate_python-1.1.6/source/blankslate/generation/project_generation.py
--rw-r--r--   0        0        0     1797 2024-05-04 21:08:06.168529 blankslate_python-1.1.6/source/blankslate/generation/template_rendering.py
--rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.1.6/source/blankslate/generation/templates/.gitignore.j2
--rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.1.6/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.1.6/source/blankslate/generation/templates/__init__.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.1.6/source/blankslate/generation/templates/CHANGELOG.md.j2
--rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.1.6/source/blankslate/generation/templates/command_line.py.j2
--rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.1.6/source/blankslate/generation/templates/conf.py.j2
--rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.1.6/source/blankslate/generation/templates/constants.py.j2
--rw-r--r--   0        0        0     3382 2024-05-04 20:50:51.262514 blankslate_python-1.1.6/source/blankslate/generation/templates/continuous_integration.yml.j2
--rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.1.6/source/blankslate/generation/templates/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.1.6/source/blankslate/generation/templates/extensions.json.j2
--rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.1.6/source/blankslate/generation/templates/index.rst.j2
--rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.1.6/source/blankslate/generation/templates/LICENSE.j2
--rw-r--r--   0        0        0      533 2024-05-04 16:12:42.195472 blankslate_python-1.1.6/source/blankslate/generation/templates/main.py.j2
--rw-r--r--   0        0        0      606 2024-05-04 16:17:41.564825 blankslate_python-1.1.6/source/blankslate/generation/templates/paths.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.1.6/source/blankslate/generation/templates/py.typed.j2
--rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.1.6/source/blankslate/generation/templates/pyproject.toml.j2
--rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.1.6/source/blankslate/generation/templates/README.md.j2
--rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.1.6/source/blankslate/generation/templates/release.sh.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.1.6/source/blankslate/generation/templates/requirements-dev.txt.j2
--rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.1.6/source/blankslate/generation/templates/requirements.txt.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.1.6/source/blankslate/generation/templates/requirements_dev.txt.j2
--rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.1.6/source/blankslate/generation/templates/setup_logging.py.j2
--rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.1.6/source/blankslate/generation/templates/todo_to_issue.yml.j2
--rw-r--r--   0        0        0     2791 2024-05-04 16:26:45.870722 blankslate_python-1.1.6/source/blankslate/generation/templates/tox.ini.j2
--rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.1.6/source/blankslate/generation/templates/VERSION.j2
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.6/source/blankslate/interface/__init__.py
--rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.1.6/source/blankslate/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.6/source/blankslate/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.1.6/source/blankslate/logs/setup_logging.py
--rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.1.6/source/blankslate/main.py
--rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.1.6/source/blankslate/py.typed
--rw-r--r--   0        0        0        6 2024-05-04 21:11:04.772973 blankslate_python-1.1.6/source/blankslate/VERSION
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 blankslate_python-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.1.7/LICENSE
+-rw-r--r--   0        0        0     2866 2024-05-04 21:29:06.281610 blankslate_python-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2245 2024-05-04 17:20:48.274142 blankslate_python-1.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.1.7/source/blankslate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.7/source/blankslate/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.1.7/source/blankslate/config/constants.py
+-rw-r--r--   0        0        0      620 2024-05-04 21:28:29.754011 blankslate_python-1.1.7/source/blankslate/config/paths.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.7/source/blankslate/generation/__init__.py
+-rw-r--r--   0        0        0     2539 2024-05-04 14:20:49.402998 blankslate_python-1.1.7/source/blankslate/generation/folder_generation.py
+-rw-r--r--   0        0        0     7209 2024-05-04 20:59:12.550950 blankslate_python-1.1.7/source/blankslate/generation/project_generation.py
+-rw-r--r--   0        0        0     1797 2024-05-04 21:08:06.168529 blankslate_python-1.1.7/source/blankslate/generation/template_rendering.py
+-rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.1.7/source/blankslate/generation/templates/.gitignore.j2
+-rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.1.7/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.1.7/source/blankslate/generation/templates/__init__.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.1.7/source/blankslate/generation/templates/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.1.7/source/blankslate/generation/templates/command_line.py.j2
+-rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.1.7/source/blankslate/generation/templates/conf.py.j2
+-rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.1.7/source/blankslate/generation/templates/constants.py.j2
+-rw-r--r--   0        0        0     3382 2024-05-04 20:50:51.262514 blankslate_python-1.1.7/source/blankslate/generation/templates/continuous_integration.yml.j2
+-rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.1.7/source/blankslate/generation/templates/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.1.7/source/blankslate/generation/templates/extensions.json.j2
+-rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.1.7/source/blankslate/generation/templates/index.rst.j2
+-rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.1.7/source/blankslate/generation/templates/LICENSE.j2
+-rw-r--r--   0        0        0      533 2024-05-04 16:12:42.195472 blankslate_python-1.1.7/source/blankslate/generation/templates/main.py.j2
+-rw-r--r--   0        0        0      606 2024-05-04 16:17:41.564825 blankslate_python-1.1.7/source/blankslate/generation/templates/paths.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.1.7/source/blankslate/generation/templates/py.typed.j2
+-rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.1.7/source/blankslate/generation/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.1.7/source/blankslate/generation/templates/README.md.j2
+-rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.1.7/source/blankslate/generation/templates/release.sh.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.1.7/source/blankslate/generation/templates/requirements-dev.txt.j2
+-rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.1.7/source/blankslate/generation/templates/requirements.txt.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.1.7/source/blankslate/generation/templates/requirements_dev.txt.j2
+-rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.1.7/source/blankslate/generation/templates/setup_logging.py.j2
+-rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.1.7/source/blankslate/generation/templates/todo_to_issue.yml.j2
+-rw-r--r--   0        0        0     2791 2024-05-04 16:26:45.870722 blankslate_python-1.1.7/source/blankslate/generation/templates/tox.ini.j2
+-rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.1.7/source/blankslate/generation/templates/VERSION.j2
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.7/source/blankslate/interface/__init__.py
+-rw-r--r--   0        0        0     3690 2024-05-04 21:03:09.221224 blankslate_python-1.1.7/source/blankslate/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.7/source/blankslate/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.1.7/source/blankslate/logs/setup_logging.py
+-rw-r--r--   0        0        0      752 2024-05-04 19:52:11.294674 blankslate_python-1.1.7/source/blankslate/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.1.7/source/blankslate/py.typed
+-rw-r--r--   0        0        0        6 2024-05-04 21:29:09.411369 blankslate_python-1.1.7/source/blankslate/VERSION
+-rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 blankslate_python-1.1.7/PKG-INFO
```

### Comparing `blankslate_python-1.1.6/LICENSE` & `blankslate_python-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/pyproject.toml` & `blankslate_python-1.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blankslate-python"
-version = "1.1.6"
+version = "1.1.7"
 description = "A blank slate for Python projects"
 authors = ["William Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "blankslate", from = "source"}]
 homepage = "https://github.com/unkokaeru/blankslate"
 repository = "https://github.com/unkokaeru/blankslate"
-include = ["LICENSE", "source/blankslate/py.typed", "source/blankslate/VERSION"]
+include = ["LICENSE", "source/blankslate/py.typed", "source/blankslate/VERSION", "source/blankslate/generation/templates"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 Jinja2 = "^3.0.0"
 rich = "^12.0.0"
 
 [tool.poetry.scripts]
```

### Comparing `blankslate_python-1.1.6/README.md` & `blankslate_python-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/config/constants.py` & `blankslate_python-1.1.7/source/blankslate/config/constants.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/config/paths.py` & `blankslate_python-1.1.7/source/blankslate/config/paths.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """paths.py: Contains paths for the application."""
 
-import os
+from importlib import resources
 
 
 class Paths:
     """
     Paths for the application.
 
     Notes
@@ -12,13 +12,10 @@
     This class contains paths used throughout the application.
     By storing paths in a single location, it is easier to
     manage and update them. Paths should be defined as class
     attributes and should be named in uppercase with underscores
     separating words.
     """
 
-    # Path to the root directory of the package
-    BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    SOURCE_DIR = os.path.join(BASE_DIR, "source", "blankslate")
-
     # Path to the templates directory
-    TEMPLATES_PATH = os.path.join(SOURCE_DIR, "generation", "templates")
+    with resources.path("blankslate.generation.templates", "") as templates_path:
+        TEMPLATES_PATH = templates_path
```

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/folder_generation.py` & `blankslate_python-1.1.7/source/blankslate/generation/folder_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/project_generation.py` & `blankslate_python-1.1.7/source/blankslate/generation/project_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/template_rendering.py` & `blankslate_python-1.1.7/source/blankslate/generation/template_rendering.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/.gitignore.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/.pre-commit-config.yaml.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/constants.py.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/constants.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/continuous_integration.yml.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/continuous_integration.yml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/CONTRIBUTING.md.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/index.rst.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/index.rst.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/LICENSE.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/main.py.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/main.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/paths.py.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/paths.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/pyproject.toml.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/README.md.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/release.sh.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/release.sh.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/setup_logging.py.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/setup_logging.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/generation/templates/tox.ini.j2` & `blankslate_python-1.1.7/source/blankslate/generation/templates/tox.ini.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/interface/command_line.py` & `blankslate_python-1.1.7/source/blankslate/interface/command_line.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/logs/setup_logging.py` & `blankslate_python-1.1.7/source/blankslate/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/source/blankslate/main.py` & `blankslate_python-1.1.7/source/blankslate/main.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.1.6/PKG-INFO` & `blankslate_python-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blankslate-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: A blank slate for Python projects
 Home-page: https://github.com/unkokaeru/blankslate
 License: MIT
 Author: William Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

