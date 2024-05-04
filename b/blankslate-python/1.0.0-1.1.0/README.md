# Comparing `tmp/blankslate_python-1.0.0.tar.gz` & `tmp/blankslate_python-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blankslate_python-1.0.0.tar", max compression
+gzip compressed data, was "blankslate_python-1.1.0.tar", max compression
```

## Comparing `blankslate_python-1.0.0.tar` & `blankslate_python-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.0.0/LICENSE
--rw-r--r--   0        0        0     2755 2024-05-04 17:19:22.055122 blankslate_python-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2153 2024-05-04 17:01:17.344949 blankslate_python-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.0.0/source/blankslate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.0.0/source/blankslate/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.0.0/source/blankslate/config/constants.py
--rw-r--r--   0        0        0      606 2024-05-02 13:16:44.071602 blankslate_python-1.0.0/source/blankslate/config/paths.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.0.0/source/blankslate/generation/__init__.py
--rw-r--r--   0        0        0     2539 2024-05-04 14:20:49.402998 blankslate_python-1.0.0/source/blankslate/generation/folder_generation.py
--rw-r--r--   0        0        0     7209 2024-05-04 17:07:22.287238 blankslate_python-1.0.0/source/blankslate/generation/project_generation.py
--rw-r--r--   0        0        0     1769 2024-05-04 14:26:55.624330 blankslate_python-1.0.0/source/blankslate/generation/template_rendering.py
--rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.0.0/source/blankslate/generation/templates/.gitignore.j2
--rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.0.0/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.0.0/source/blankslate/generation/templates/__init__.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.0.0/source/blankslate/generation/templates/CHANGELOG.md.j2
--rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.0.0/source/blankslate/generation/templates/command_line.py.j2
--rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.0.0/source/blankslate/generation/templates/conf.py.j2
--rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.0.0/source/blankslate/generation/templates/constants.py.j2
--rw-r--r--   0        0        0     3212 2024-05-04 16:21:06.197919 blankslate_python-1.0.0/source/blankslate/generation/templates/continuous_integration.yml.j2
--rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.0.0/source/blankslate/generation/templates/CONTRIBUTING.md.j2
--rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.0.0/source/blankslate/generation/templates/extensions.json.j2
--rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.0.0/source/blankslate/generation/templates/index.rst.j2
--rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.0.0/source/blankslate/generation/templates/LICENSE.j2
--rw-r--r--   0        0        0      533 2024-05-04 16:12:42.195472 blankslate_python-1.0.0/source/blankslate/generation/templates/main.py.j2
--rw-r--r--   0        0        0      606 2024-05-04 16:17:41.564825 blankslate_python-1.0.0/source/blankslate/generation/templates/paths.py.j2
--rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.0.0/source/blankslate/generation/templates/py.typed.j2
--rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.0.0/source/blankslate/generation/templates/pyproject.toml.j2
--rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.0.0/source/blankslate/generation/templates/README.md.j2
--rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.0.0/source/blankslate/generation/templates/release.sh.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.0.0/source/blankslate/generation/templates/requirements-dev.txt.j2
--rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.0.0/source/blankslate/generation/templates/requirements.txt.j2
--rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.0.0/source/blankslate/generation/templates/requirements_dev.txt.j2
--rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.0.0/source/blankslate/generation/templates/setup_logging.py.j2
--rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.0.0/source/blankslate/generation/templates/todo_to_issue.yml.j2
--rw-r--r--   0        0        0     2791 2024-05-04 16:26:45.870722 blankslate_python-1.0.0/source/blankslate/generation/templates/tox.ini.j2
--rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.0.0/source/blankslate/generation/templates/VERSION.j2
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.0.0/source/blankslate/interface/__init__.py
--rw-r--r--   0        0        0     3565 2024-05-04 14:22:25.345335 blankslate_python-1.0.0/source/blankslate/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.0.0/source/blankslate/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.0.0/source/blankslate/logs/setup_logging.py
--rw-r--r--   0        0        0      895 2024-05-04 16:34:03.692150 blankslate_python-1.0.0/source/blankslate/main.py
--rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.0.0/source/blankslate/py.typed
--rw-r--r--   0        0        0        6 2024-05-04 17:15:09.708675 blankslate_python-1.0.0/source/blankslate/VERSION
--rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 blankslate_python-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-02 10:19:51.904181 blankslate_python-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2755 2024-05-04 17:23:55.631259 blankslate_python-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2245 2024-05-04 17:20:48.274142 blankslate_python-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 10:44:42.812685 blankslate_python-1.1.0/source/blankslate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.0/source/blankslate/config/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-02 11:13:24.933968 blankslate_python-1.1.0/source/blankslate/config/constants.py
+-rw-r--r--   0        0        0      606 2024-05-02 13:16:44.071602 blankslate_python-1.1.0/source/blankslate/config/paths.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.0/source/blankslate/generation/__init__.py
+-rw-r--r--   0        0        0     2539 2024-05-04 14:20:49.402998 blankslate_python-1.1.0/source/blankslate/generation/folder_generation.py
+-rw-r--r--   0        0        0     7209 2024-05-04 17:07:22.287238 blankslate_python-1.1.0/source/blankslate/generation/project_generation.py
+-rw-r--r--   0        0        0     1769 2024-05-04 14:26:55.624330 blankslate_python-1.1.0/source/blankslate/generation/template_rendering.py
+-rw-r--r--   0        0        0     3237 2024-05-04 16:12:56.451075 blankslate_python-1.1.0/source/blankslate/generation/templates/.gitignore.j2
+-rw-r--r--   0        0        0     1063 2024-05-04 16:23:15.585858 blankslate_python-1.1.0/source/blankslate/generation/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-25 00:35:55.069192 blankslate_python-1.1.0/source/blankslate/generation/templates/__init__.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:23:28.152760 blankslate_python-1.1.0/source/blankslate/generation/templates/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      317 2024-05-04 16:12:34.560332 blankslate_python-1.1.0/source/blankslate/generation/templates/command_line.py.j2
+-rw-r--r--   0        0        0      264 2024-05-04 16:24:45.758933 blankslate_python-1.1.0/source/blankslate/generation/templates/conf.py.j2
+-rw-r--r--   0        0        0      603 2024-05-04 16:17:49.390745 blankslate_python-1.1.0/source/blankslate/generation/templates/constants.py.j2
+-rw-r--r--   0        0        0     3212 2024-05-04 16:21:06.197919 blankslate_python-1.1.0/source/blankslate/generation/templates/continuous_integration.yml.j2
+-rw-r--r--   0        0        0     3292 2024-05-04 17:06:59.156818 blankslate_python-1.1.0/source/blankslate/generation/templates/CONTRIBUTING.md.j2
+-rw-r--r--   0        0        0       84 2024-05-04 16:21:59.690182 blankslate_python-1.1.0/source/blankslate/generation/templates/extensions.json.j2
+-rw-r--r--   0        0        0     1702 2024-05-04 17:14:07.452271 blankslate_python-1.1.0/source/blankslate/generation/templates/index.rst.j2
+-rw-r--r--   0        0        0     1112 2024-04-24 16:37:27.384880 blankslate_python-1.1.0/source/blankslate/generation/templates/LICENSE.j2
+-rw-r--r--   0        0        0      533 2024-05-04 16:12:42.195472 blankslate_python-1.1.0/source/blankslate/generation/templates/main.py.j2
+-rw-r--r--   0        0        0      606 2024-05-04 16:17:41.564825 blankslate_python-1.1.0/source/blankslate/generation/templates/paths.py.j2
+-rw-r--r--   0        0        0        0 2024-05-04 16:22:44.594900 blankslate_python-1.1.0/source/blankslate/generation/templates/py.typed.j2
+-rw-r--r--   0        0        0     2854 2024-05-04 16:15:25.176062 blankslate_python-1.1.0/source/blankslate/generation/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0     1134 2024-05-04 17:05:19.122602 blankslate_python-1.1.0/source/blankslate/generation/templates/README.md.j2
+-rw-r--r--   0        0        0     1330 2024-05-04 16:22:21.707040 blankslate_python-1.1.0/source/blankslate/generation/templates/release.sh.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:25:54.086216 blankslate_python-1.1.0/source/blankslate/generation/templates/requirements-dev.txt.j2
+-rw-r--r--   0        0        0       28 2024-05-04 16:16:50.883961 blankslate_python-1.1.0/source/blankslate/generation/templates/requirements.txt.j2
+-rw-r--r--   0        0        0      297 2024-05-04 16:16:41.782308 blankslate_python-1.1.0/source/blankslate/generation/templates/requirements_dev.txt.j2
+-rw-r--r--   0        0        0     1879 2024-05-04 16:17:23.522577 blankslate_python-1.1.0/source/blankslate/generation/templates/setup_logging.py.j2
+-rw-r--r--   0        0        0      261 2024-05-04 16:21:46.396690 blankslate_python-1.1.0/source/blankslate/generation/templates/todo_to_issue.yml.j2
+-rw-r--r--   0        0        0     2791 2024-05-04 16:26:45.870722 blankslate_python-1.1.0/source/blankslate/generation/templates/tox.ini.j2
+-rw-r--r--   0        0        0        5 2024-05-02 09:28:19.986550 blankslate_python-1.1.0/source/blankslate/generation/templates/VERSION.j2
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.0/source/blankslate/interface/__init__.py
+-rw-r--r--   0        0        0     3565 2024-05-04 14:22:25.345335 blankslate_python-1.1.0/source/blankslate/interface/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-24 23:05:13.473582 blankslate_python-1.1.0/source/blankslate/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-04 14:22:34.495627 blankslate_python-1.1.0/source/blankslate/logs/setup_logging.py
+-rw-r--r--   0        0        0      895 2024-05-04 16:34:03.692150 blankslate_python-1.1.0/source/blankslate/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:03:08.486123 blankslate_python-1.1.0/source/blankslate/py.typed
+-rw-r--r--   0        0        0        6 2024-05-04 17:23:58.644627 blankslate_python-1.1.0/source/blankslate/VERSION
+-rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 blankslate_python-1.1.0/PKG-INFO
```

### Comparing `blankslate_python-1.0.0/LICENSE` & `blankslate_python-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/pyproject.toml` & `blankslate_python-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "blankslate-python"
-version = "1.0.0"
+version = "1.1.0"
 description = "A blank slate for Python projects"
 authors = ["William Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "blankslate", from = "source"}]
 homepage = "https://github.com/unkokaeru/blankslate"
 repository = "https://github.com/unkokaeru/blankslate"
```

### Comparing `blankslate_python-1.0.0/README.md` & `blankslate_python-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 Blankslate automates the creation of Python projects, ensuring that every detail adheres to the best practices of Python development. It leverages GitHub Actions, NumPy docstrings, and a well-organised directory structure to deliver a ready-to-deploy project scaffold.
 
 ## Installation
 
 To install Blankslate, simply run:
 
 ```bash
-pip install blankslate
+pip install blankslate-python
 ```
 
 ## Getting Started
 
 After installation, you can create a new project by executing:
 
 ```bash
-blankslate
+blankslate-python
 ```
 
 Follow the prompts to specify your project details. Blankslate will create the project in your designated directory. You can then push this project to GitHub and start programming in the `source/PROJECT_NAME/` directory.
 
 ## Features
 
 - **Automatic Project Structure Creation**: Sets up a GitHub-ready Python project with best practices.
-- **Semantic Versioning**: Use the script `./scripts/release.sh VERSION_NUMBER` to auto-version and generate a changelog. Ensure `VERSION_NUMBER` follows [semantic versioning](https://semver.org).
+- **Semantic Versioning**: Use the script `./scripts/release.sh VERSION_NUMBER` to auto-version and generate a changelog. Ensure `VERSION_NUMBER` follows [semantic versioning](https://semver.org). Note that this will automatically build and publish the project to PyPi, too.
 - **Commit Style**: Commits should follow the [Angular commit style](https://gist.github.com/brianclements/841ea7bffdb01346392c#commit-message-header).
 - **Documentation**: Automatically generates and pushes documentation to GitHub pages. Make sure your GitHub repository is configured under `Settings -> Pages`.
 - **TODO to GitHub Issues**: Converts `# TODO` comments in your Python code into GitHub issues. Configure this in `Settings -> Actions (General) -> Workflow permissions` and enable "Read and write permissions".
 
 ## Extensions
 
 Enhance your Blankslate experience with the [Blankslate Extension Pack](https://marketplace.visualstudio.com/items?itemName=unkokaeru.blankslate-extension-pack) for [VS Code](https://code.visualstudio.com/download).
```

### Comparing `blankslate_python-1.0.0/source/blankslate/config/constants.py` & `blankslate_python-1.1.0/source/blankslate/config/constants.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/config/paths.py` & `blankslate_python-1.1.0/source/blankslate/config/paths.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/folder_generation.py` & `blankslate_python-1.1.0/source/blankslate/generation/folder_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/project_generation.py` & `blankslate_python-1.1.0/source/blankslate/generation/project_generation.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/template_rendering.py` & `blankslate_python-1.1.0/source/blankslate/generation/template_rendering.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/.gitignore.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/.pre-commit-config.yaml.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/constants.py.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/constants.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/continuous_integration.yml.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/continuous_integration.yml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/CONTRIBUTING.md.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/CONTRIBUTING.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/index.rst.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/index.rst.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/LICENSE.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/main.py.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/main.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/paths.py.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/paths.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/pyproject.toml.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/README.md.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/release.sh.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/release.sh.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/setup_logging.py.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/setup_logging.py.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/generation/templates/tox.ini.j2` & `blankslate_python-1.1.0/source/blankslate/generation/templates/tox.ini.j2`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/interface/command_line.py` & `blankslate_python-1.1.0/source/blankslate/interface/command_line.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/logs/setup_logging.py` & `blankslate_python-1.1.0/source/blankslate/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/source/blankslate/main.py` & `blankslate_python-1.1.0/source/blankslate/main.py`

 * *Files identical despite different names*

### Comparing `blankslate_python-1.0.0/PKG-INFO` & `blankslate_python-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blankslate-python
-Version: 1.0.0
+Version: 1.1.0
 Summary: A blank slate for Python projects
 Home-page: https://github.com/unkokaeru/blankslate
 License: MIT
 Author: William Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -33,31 +33,31 @@
 Blankslate automates the creation of Python projects, ensuring that every detail adheres to the best practices of Python development. It leverages GitHub Actions, NumPy docstrings, and a well-organised directory structure to deliver a ready-to-deploy project scaffold.
 
 ## Installation
 
 To install Blankslate, simply run:
 
 ```bash
-pip install blankslate
+pip install blankslate-python
 ```
 
 ## Getting Started
 
 After installation, you can create a new project by executing:
 
 ```bash
-blankslate
+blankslate-python
 ```
 
 Follow the prompts to specify your project details. Blankslate will create the project in your designated directory. You can then push this project to GitHub and start programming in the `source/PROJECT_NAME/` directory.
 
 ## Features
 
 - **Automatic Project Structure Creation**: Sets up a GitHub-ready Python project with best practices.
-- **Semantic Versioning**: Use the script `./scripts/release.sh VERSION_NUMBER` to auto-version and generate a changelog. Ensure `VERSION_NUMBER` follows [semantic versioning](https://semver.org).
+- **Semantic Versioning**: Use the script `./scripts/release.sh VERSION_NUMBER` to auto-version and generate a changelog. Ensure `VERSION_NUMBER` follows [semantic versioning](https://semver.org). Note that this will automatically build and publish the project to PyPi, too.
 - **Commit Style**: Commits should follow the [Angular commit style](https://gist.github.com/brianclements/841ea7bffdb01346392c#commit-message-header).
 - **Documentation**: Automatically generates and pushes documentation to GitHub pages. Make sure your GitHub repository is configured under `Settings -> Pages`.
 - **TODO to GitHub Issues**: Converts `# TODO` comments in your Python code into GitHub issues. Configure this in `Settings -> Actions (General) -> Workflow permissions` and enable "Read and write permissions".
 
 ## Extensions
 
 Enhance your Blankslate experience with the [Blankslate Extension Pack](https://marketplace.visualstudio.com/items?itemName=unkokaeru.blankslate-extension-pack) for [VS Code](https://code.visualstudio.com/download).
```

