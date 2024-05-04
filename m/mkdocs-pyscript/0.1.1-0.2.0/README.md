# Comparing `tmp/mkdocs-pyscript-0.1.1.tar.gz` & `tmp/mkdocs_pyscript-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-pyscript-0.1.1.tar", last modified: Tue Nov  7 00:24:18 2023, max compression
+gzip compressed data, was "mkdocs_pyscript-0.2.0.tar", last modified: Sat May  4 16:58:21 2024, max compression
```

## Comparing `mkdocs-pyscript-0.1.1.tar` & `mkdocs_pyscript-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.736099 mkdocs-pyscript-0.1.1/
--rw-rw-r--   0 jglass    (1000) jglass    (1000)    11541 2023-10-29 14:13:37.000000 mkdocs-pyscript-0.1.1/LICENSE
--rw-rw-r--   0 jglass    (1000) jglass    (1000)       75 2023-10-29 14:13:37.000000 mkdocs-pyscript-0.1.1/MANIFEST.in
--rw-r--r--   0 jglass    (1000) jglass    (1000)     4520 2023-11-07 00:24:18.736099 mkdocs-pyscript-0.1.1/PKG-INFO
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     3715 2023-11-07 00:16:53.000000 mkdocs-pyscript-0.1.1/README.md
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.728099 mkdocs-pyscript-0.1.1/mkdocs_pyscript/
--rw-rw-r--   0 jglass    (1000) jglass    (1000)      204 2023-10-29 14:13:37.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript/__init__.py
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.728099 mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.732099 mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/css/
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     1973 2023-11-07 00:24:13.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/css/pyrepl.css
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.732099 mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/js/
--rw-rw-r--   0 jglass    (1000) jglass    (1000)   856170 2023-11-07 00:24:13.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/js/makeblocks.js
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     1288 2023-11-07 00:24:13.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/js/mini-coi.js
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     7193 2023-11-07 00:22:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript/plugin.py
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     1188 2023-11-07 00:16:53.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript/prePostExtension.py
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.732099 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/
--rw-r--r--   0 jglass    (1000) jglass    (1000)     4520 2023-11-07 00:24:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/PKG-INFO
--rw-rw-r--   0 jglass    (1000) jglass    (1000)      570 2023-11-07 00:24:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/SOURCES.txt
--rw-rw-r--   0 jglass    (1000) jglass    (1000)        1 2023-11-07 00:24:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/dependency_links.txt
--rw-rw-r--   0 jglass    (1000) jglass    (1000)       65 2023-11-07 00:24:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/entry_points.txt
--rw-rw-r--   0 jglass    (1000) jglass    (1000)       34 2023-11-07 00:24:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/requires.txt
--rw-rw-r--   0 jglass    (1000) jglass    (1000)       22 2023-11-07 00:24:18.000000 mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/top_level.txt
--rw-rw-r--   0 jglass    (1000) jglass    (1000)       38 2023-11-07 00:24:18.736099 mkdocs-pyscript-0.1.1/setup.cfg
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     1404 2023-11-07 00:23:47.000000 mkdocs-pyscript-0.1.1/setup.py
-drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2023-11-07 00:24:18.736099 mkdocs-pyscript-0.1.1/tests/
--rw-rw-r--   0 jglass    (1000) jglass    (1000)        0 2023-10-29 14:13:37.000000 mkdocs-pyscript-0.1.1/tests/__init__.py
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     4330 2023-10-29 15:47:56.000000 mkdocs-pyscript-0.1.1/tests/conftest.py
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     2137 2023-11-07 00:16:53.000000 mkdocs-pyscript-0.1.1/tests/support.py
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     2599 2023-11-07 00:16:53.000000 mkdocs-pyscript-0.1.1/tests/test_dynamic.py
--rw-rw-r--   0 jglass    (1000) jglass    (1000)     2265 2023-11-07 00:16:53.000000 mkdocs-pyscript-0.1.1/tests/test_static.py
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)    11541 2024-04-21 20:55:12.000000 mkdocs_pyscript-0.2.0/LICENSE
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)       75 2024-04-21 20:55:12.000000 mkdocs_pyscript-0.2.0/MANIFEST.in
+-rw-r--r--   0 jglass    (1000) jglass    (1000)     4890 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/PKG-INFO
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     4035 2024-05-04 16:55:11.000000 mkdocs_pyscript-0.2.0/README.md
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.046785 mkdocs_pyscript-0.2.0/mkdocs_pyscript/
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)      204 2024-04-21 20:55:12.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript/__init__.py
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.046785 mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/css/
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     1973 2024-05-04 16:58:17.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/css/pyrepl.css
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/js/
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     1306 2024-05-04 16:58:17.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/js/makeblocks.js
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     1288 2024-05-04 16:58:17.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/js/mini-coi.js
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     6073 2024-05-04 16:55:11.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript/plugin.py
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/
+-rw-r--r--   0 jglass    (1000) jglass    (1000)     4890 2024-05-04 16:58:21.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/PKG-INFO
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)      534 2024-05-04 16:58:21.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/SOURCES.txt
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)        1 2024-05-04 16:58:21.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/dependency_links.txt
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)       65 2024-05-04 16:58:21.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/entry_points.txt
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)       34 2024-05-04 16:58:21.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/requires.txt
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)       22 2024-05-04 16:58:21.000000 mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/top_level.txt
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)       38 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/setup.cfg
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     1463 2024-05-04 16:58:01.000000 mkdocs_pyscript-0.2.0/setup.py
+drwxrwxr-x   0 jglass    (1000) jglass    (1000)        0 2024-05-04 16:58:21.050785 mkdocs_pyscript-0.2.0/tests/
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)        0 2024-04-21 20:55:12.000000 mkdocs_pyscript-0.2.0/tests/__init__.py
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     4330 2024-04-21 20:55:12.000000 mkdocs_pyscript-0.2.0/tests/conftest.py
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     2137 2024-04-21 20:55:12.000000 mkdocs_pyscript-0.2.0/tests/support.py
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     3131 2024-05-04 16:55:11.000000 mkdocs_pyscript-0.2.0/tests/test_dynamic.py
+-rw-rw-r--   0 jglass    (1000) jglass    (1000)     1891 2024-05-04 16:55:11.000000 mkdocs_pyscript-0.2.0/tests/test_static.py
```

### Comparing `mkdocs-pyscript-0.1.1/LICENSE` & `mkdocs_pyscript-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-pyscript-0.1.1/PKG-INFO` & `mkdocs_pyscript-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: mkdocs-pyscript
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add PyScript to your mkdocs site
 Home-page: https://github.com/jeffersglass/mkdocs-pyscript
 Author: Jeff Glass
-Author-email: mail@jeff.glass
+Author-email: glass.jeffrey@gmail.com
 License: APACHE
 Keywords: mkdocs,pyscript
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.4.0
 Requires-Dist: beautifulsoup4>=4.1
 
 # mkdocs-pyscript
@@ -43,71 +44,80 @@
 
 ## Usage
 
 With this plugin enabled, all Python [fenced code blocks](https://www.mkdocs.org/user-guide/writing-your-docs/#fenced-code-blocks) (type `py` or `python` or any other label that maps to `lang-python`) will have an added LOAD button in the lower-right corrner. When clicked, the code block will be transformed into an editable code snippet (using [codemirror](https://codemirror.net/)). When the user clicks on the green "run" arrow in the lower right corner, or pressed SHIFT+ENTER when focused, will run the inner Python code using PyScript.
 
 The included code is run in a [Web Worker](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers), so as not to block the main thread. Each snippet is run in a separate web worker; variables, objects, and names are not shared between executions of the same cell.
 
-### `pre` and `post` code
+### Environments
 
-Some demo code snippets may require setup and/or teardown code to properly function, which don't necessarily need to be displayed to the user. To run a chunk of Python code before any code the user runs in a particular code editor, add the `.py-pre` class to a fenced code block immediately before the user-visible code block, using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin. To run a chunk of code after a user runs a particular code editor add the `.py-post` class to a fenced code block immediately after the user-visible code block:
+Documentation may benefit from some executable code blocks being isolated from others to create distinct examples. Add the `env` attribute to a fenced code block, using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin, to create an editor for the [PyScript Environment](https://docs.pyscript.net/2024.4.2/user-guide/editor/), e.g. a specific copy of the interpreter isolated from other evnironments.
 
 ````
-```{.py .py-pre}
-print("This is some pre-code")
+```{.py env="one"}
+x = 1
 ```
 
-```py
-print("This is the main tag")
-# Only this code will be displayed in the code editor
+```{.py env="one"}
+print(x) # Shares an interpreter with the first block
 ```
 
-```{.py .py-post}
-print("This is some post code")
+```{.py env="two"}
+print(x) # Error: 'x' is not defined (in this interpreter)
+```
+````
+
+### `setup` code
+
+Some demo code snippets may require setup code to properly function, which don't necessarily need to be displayed to the user. To run a chunk of Python code before any code the user runs in a particular code editor, add the `setup` attribute to a fenced code block with a specific [environment](#Environments), using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin.
+
+````
+```{.py setup env="three"}
+print("This is some setup code")
+```
+
+```{.py env="three"}
+print("This is the main tag")
 ```
 ````
 
 ## Configuration
 
 `mkdocs-pyscript` supports  options that can be set in `mkdocs.yaml` to control the behavior of the plugin
 
 ### `pyscript_version`
 
-The `pyscript_version` property of the plugin controls the version of PyScript that is loaded. If not specified, the current default version is `snapshots/2023.09.1.RC2`.
+The `pyscript_version` property of the plugin controls the version of PyScript that is loaded. If not specified, the current default version is `releases/2024.4.2`.
 
 
 To support both pre-release snapshots and released versions of PyScript, the provided value is inserted into the following string:
 
 ```py
 SCRIPT = f'https://pyscript.net/{pyscript_version}/core.js'
 ```
 
 That is, to load a specific release or snapshot, use:
 ```yaml
 #Load a release
 plugins:
     - mkdocs-pyscript:
-        pyscript_version: "releases/2023.11.1"
+        pyscript_version: "releases/2024.2.1"
 
 #Load a snapshot
 plugins:
     - mkdocs-pyscript:
         pyscript_version: "snapshots/2023.11.1.RC3"
 
-#Load the most recent (unstable) build:
-plugins:
-    - mkdocs-pyscript:
-        pyscript_version: "unstable"
 ```
 
 ### `selective`
 
 By default, `mkdocs-pyscript` turns *all* blocks with type `py` or `python` into exectuable code snippets. To cause only selected blocks to be transformed:
 
-  1. Set the `selective` property to `true`:
+  1. Set the `selective` property to `true` in your configuration:
 ```yaml
 plugins:
     - mkdocs-pyscript:
         selective: true
 ```
   2. Specify `.pyscript` as an additional class for the codeblocks that you want to be runnable:
```

### Comparing `mkdocs-pyscript-0.1.1/README.md` & `mkdocs_pyscript-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,71 +18,80 @@
 
 ## Usage
 
 With this plugin enabled, all Python [fenced code blocks](https://www.mkdocs.org/user-guide/writing-your-docs/#fenced-code-blocks) (type `py` or `python` or any other label that maps to `lang-python`) will have an added LOAD button in the lower-right corrner. When clicked, the code block will be transformed into an editable code snippet (using [codemirror](https://codemirror.net/)). When the user clicks on the green "run" arrow in the lower right corner, or pressed SHIFT+ENTER when focused, will run the inner Python code using PyScript.
 
 The included code is run in a [Web Worker](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers), so as not to block the main thread. Each snippet is run in a separate web worker; variables, objects, and names are not shared between executions of the same cell.
 
-### `pre` and `post` code
+### Environments
 
-Some demo code snippets may require setup and/or teardown code to properly function, which don't necessarily need to be displayed to the user. To run a chunk of Python code before any code the user runs in a particular code editor, add the `.py-pre` class to a fenced code block immediately before the user-visible code block, using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin. To run a chunk of code after a user runs a particular code editor add the `.py-post` class to a fenced code block immediately after the user-visible code block:
+Documentation may benefit from some executable code blocks being isolated from others to create distinct examples. Add the `env` attribute to a fenced code block, using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin, to create an editor for the [PyScript Environment](https://docs.pyscript.net/2024.4.2/user-guide/editor/), e.g. a specific copy of the interpreter isolated from other evnironments.
 
 ````
-```{.py .py-pre}
-print("This is some pre-code")
+```{.py env="one"}
+x = 1
 ```
 
-```py
-print("This is the main tag")
-# Only this code will be displayed in the code editor
+```{.py env="one"}
+print(x) # Shares an interpreter with the first block
 ```
 
-```{.py .py-post}
-print("This is some post code")
+```{.py env="two"}
+print(x) # Error: 'x' is not defined (in this interpreter)
+```
+````
+
+### `setup` code
+
+Some demo code snippets may require setup code to properly function, which don't necessarily need to be displayed to the user. To run a chunk of Python code before any code the user runs in a particular code editor, add the `setup` attribute to a fenced code block with a specific [environment](#Environments), using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin.
+
+````
+```{.py setup env="three"}
+print("This is some setup code")
+```
+
+```{.py env="three"}
+print("This is the main tag")
 ```
 ````
 
 ## Configuration
 
 `mkdocs-pyscript` supports  options that can be set in `mkdocs.yaml` to control the behavior of the plugin
 
 ### `pyscript_version`
 
-The `pyscript_version` property of the plugin controls the version of PyScript that is loaded. If not specified, the current default version is `snapshots/2023.09.1.RC2`.
+The `pyscript_version` property of the plugin controls the version of PyScript that is loaded. If not specified, the current default version is `releases/2024.4.2`.
 
 
 To support both pre-release snapshots and released versions of PyScript, the provided value is inserted into the following string:
 
 ```py
 SCRIPT = f'https://pyscript.net/{pyscript_version}/core.js'
 ```
 
 That is, to load a specific release or snapshot, use:
 ```yaml
 #Load a release
 plugins:
     - mkdocs-pyscript:
-        pyscript_version: "releases/2023.11.1"
+        pyscript_version: "releases/2024.2.1"
 
 #Load a snapshot
 plugins:
     - mkdocs-pyscript:
         pyscript_version: "snapshots/2023.11.1.RC3"
 
-#Load the most recent (unstable) build:
-plugins:
-    - mkdocs-pyscript:
-        pyscript_version: "unstable"
 ```
 
 ### `selective`
 
 By default, `mkdocs-pyscript` turns *all* blocks with type `py` or `python` into exectuable code snippets. To cause only selected blocks to be transformed:
 
-  1. Set the `selective` property to `true`:
+  1. Set the `selective` property to `true` in your configuration:
 ```yaml
 plugins:
     - mkdocs-pyscript:
         selective: true
 ```
   2. Specify `.pyscript` as an additional class for the codeblocks that you want to be runnable:
```

### Comparing `mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/css/pyrepl.css` & `mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/css/pyrepl.css`

 * *Files identical despite different names*

### Comparing `mkdocs-pyscript-0.1.1/mkdocs_pyscript/dist/js/mini-coi.js` & `mkdocs_pyscript-0.2.0/mkdocs_pyscript/dist/js/mini-coi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-pyscript-0.1.1/mkdocs_pyscript/plugin.py` & `mkdocs_pyscript-0.2.0/mkdocs_pyscript/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from bs4 import BeautifulSoup, Tag
 from mkdocs.config import config_options, config_options, base
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin, get_plugin_logger
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 
-DEFAULT_VERSION = "snapshots/2023.11.1.RC3"
+DEFAULT_VERSION = "releases/2024.4.2"
 SCRIPT = 'https://pyscript.net/{version}/core.js'
-LANG_TAGS = ['language-python', 'language-py']
+CSS = 'https://pyscript.net/{version}/core.css'
 
 from . import glr_path_static
 
 @dataclass
 class Script():
     path: str
     type: str = None
@@ -46,127 +46,107 @@
         for file in os.listdir(glr_path_static("dist/js")):
             if file.endswith(".js"):
                 config["extra_javascript"].append(file)
 
 
         # Set version
         self.SCRIPT_LINK = SCRIPT.format(version=self.config.pyscript_version)
+        self.CSS_LINK = CSS.format(version=self.config.pyscript_version)
 
         # Disable navigation.instant
         if 'features' in config['theme'] and 'navigation.instant' in config['theme']['features']:
             self.logger.warning("mkdocs-pyscript is not compatible with navigation.instant; instant navigation will be disabled.")
             config['theme']['features'].remove('navigation.instant')
 
         if 'attr_list' not in config['markdown_extensions']: config['markdown_extensions'].append('attr_list')
-
-        # Inject pre-post Markdown plugin
-        #config['markdown_extensions'].append(PrePostExtension())
         
         return config
     
-    def scriptize(self, soup: BeautifulSoup, block: Tag, *, script_type="unmanaged-pyscript-mkdocs", label=None,):
+    def scriptize(self, soup: BeautifulSoup, block: Tag, *, script_type="unmanaged-pyscript-mkdocs", label=None, attrs: dict = None):
         #Remove linenumber links:
         lineno_links = block.find_all('a')
         for a in lineno_links:
             if 'href' in a.attrs and "codelineno" in a['href']: a.extract()
 
         script = soup.new_tag("script")
         script['type'] = script_type
-        script['id'] = label
+        if label: script['id'] = label
+        for k, v in attrs.items():
+            script.attrs[k] = v
         script.string = block.text
         return script
 
 
     def on_page_content(self, html: str, *, page: Page, config: MkDocsConfig, files: Files) -> Union[str, None]:
-        print(f" Processing {page}")
         soup = BeautifulSoup(html, features="html.parser")
 
         tag_names = ['code', 'div']
 
         # Get all potential codeblocks in order:
-        code_blocks: List[Tag] = []
-        tag = soup.find(name=tag_names)
-        if tag:
-            code_blocks.append(tag)
-            while tag:= tag.find_next(name=tag_names):
-                # Only include "top level" code tags
-                if not any((tag in existing_tag.descendants) for existing_tag in code_blocks): code_blocks.append(tag)
+        #code_blocks: List[Tag] = []
+        #tag = soup.find(name=tag_names)
+        #if tag:
+        #    code_blocks.append(tag)
+        #    while tag:= tag.find_next(name=tag_names):
+        #        # Only include "top level" code tags
+        #        if not any((tag in existing_tag.descendants) for existing_tag in code_blocks): code_blocks.append(tag)
+
+        code_blocks: list[Tag] = soup.find_all(name=tag_names)
 
         # exit early if no codeblocks on page
         if not code_blocks: return html
 
-        # When we process a 'py-pre' tag, we'll turn it into a comment and extract it from the document,
-        # only saving the most recent one seen. Then, when we process an actual code tag, we'll inject 
-        # that py-pre tag before it with a matching ID
-
-        # Similarly, when we see an actual code tag, we'll save a reference to it; when we process a 'py-post'
-        # tag, we'll inject it after the most recent code tag with a matching ID
-        last_seen_pre_tag = None
-        last_seen_primary_tag = None
-        primary_block_index = -1
-
         # Process all blocks
         for block in code_blocks:
+            print(block.attrs)
             try:
                 #Classless blocks cannot be handled
                 classes = block.attrs['class']
             except KeyError:
                 continue
 
-             # Move classes from exterior pre/post to py-wrapper
+
+            # Move classes from exterior pre/post to py-wrapper
             if block.parent.name == 'pre' and 'class' in block.parent.attrs:
                 block.attrs['class'].extend(block.parent.attrs['class'])
+                
+            if (self.config.selective and 'pyscript' in classes) or \
+                    ((not self.config.selective) and ('language-python' in classes or 'language-py' in classes or 'pyscript' in classes)):
+            
 
-            if 'py-pre' in classes:
-                if last_seen_pre_tag:
-                    self.logger.warning("Multiple py-pre tags encountered with no primary tag between them")
-                last_seen_pre_tag = block.extract()
-
-            elif 'py-post' in classes:
-                block.extract()
-                if last_seen_primary_tag:
-                    last_seen_primary_tag.insert_before(self.scriptize(soup, block, script_type="py-post", label=f"py-post-{primary_block_index}"))
-                    last_seen_primary_tag = None
-                else: self.logger.warning('Encountered py-post tag with no valid primary tag preceding it')
-
-            elif (self.config.selective and 'pyscript' in classes) or \
-                    ((not self.config.selective) and any(c.lower() == lang for c in classes for lang in LANG_TAGS)):
                 #Wrap codeblock in a new div
                 div = soup.new_tag('div')
                 div['class'] = "py-wrapper"
-                div['style'] = "position:relative"
-                div['id'] = f"py-main-{(primary_block_index := primary_block_index + 1)}"
+                div['style'] = "position:relative;"
+                if 'setup' in block.attrs:
+                    div['style'] += 'display: none;'
+                #div['id'] = f"py-main-{(primary_block_index := primary_block_index + 1)}"
 
                 block.wrap(div) # Wrap codeblock with div
-                last_seen_primary_tag = block
 
-                #Inject a pre-tag if necessary
-                if last_seen_pre_tag:
-                    block.insert_before(self.scriptize(soup, last_seen_pre_tag, script_type="py-pre", label=f"py-pre-{primary_block_index}"))
-                    last_seen_pre_tag = None                    
+                if 'setup' in block.attrs:
+                    env = block.attrs['env'] if 'env' in block.attrs else ""
+                    block.replace_with(self.scriptize(soup, block, script_type='py-editor', attrs={'setup': '', 'env' : env}))
+                    print('Replacing with script')
             
         return str(soup)
     
     def on_post_page(self, output: str, *, page: Page, config: MkDocsConfig) -> Union[str, None]:
         soup = BeautifulSoup(output, features="html.parser")
         codeblocks = soup.find_all(attrs={"class": "py-wrapper" },)
         if (len(codeblocks)):
             # Add importmap
-            imp_map = soup.new_tag("script")
-            imp_map['type'] = "importmap"
-            imp_map.string = f"""
-            {{
-                "imports": {{ 
-                    "@pyscript/core": "{self.SCRIPT_LINK}"
-                }}
-            }}
-            """
-            #soup.head.append(imp_map)
-            soup.head.contents[0].insert_before(imp_map)
-
-            # PyScript is imported in makeblocks.js via the import map
+            script_tag = soup.new_tag("script")
+            script_tag['type'] = "module"
+            script_tag['src'] = self.SCRIPT_LINK
+            soup.head.append(script_tag)
+
+            css = soup.new_tag('link')
+            css['rel'] = 'stylesheet'
+            css['href'] = self.CSS_LINK
+            soup.head.append(css)
 
             # Make makeblock script a module
             makeblocks = [s for s in soup.find_all("script") if 'src' in s.attrs and "makeblocks" in s['src']][0]
             makeblocks['type'] = "module"
         return str(soup)
```

### Comparing `mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/PKG-INFO` & `mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: mkdocs-pyscript
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add PyScript to your mkdocs site
 Home-page: https://github.com/jeffersglass/mkdocs-pyscript
 Author: Jeff Glass
-Author-email: mail@jeff.glass
+Author-email: glass.jeffrey@gmail.com
 License: APACHE
 Keywords: mkdocs,pyscript
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.4.0
 Requires-Dist: beautifulsoup4>=4.1
 
 # mkdocs-pyscript
@@ -43,71 +44,80 @@
 
 ## Usage
 
 With this plugin enabled, all Python [fenced code blocks](https://www.mkdocs.org/user-guide/writing-your-docs/#fenced-code-blocks) (type `py` or `python` or any other label that maps to `lang-python`) will have an added LOAD button in the lower-right corrner. When clicked, the code block will be transformed into an editable code snippet (using [codemirror](https://codemirror.net/)). When the user clicks on the green "run" arrow in the lower right corner, or pressed SHIFT+ENTER when focused, will run the inner Python code using PyScript.
 
 The included code is run in a [Web Worker](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers), so as not to block the main thread. Each snippet is run in a separate web worker; variables, objects, and names are not shared between executions of the same cell.
 
-### `pre` and `post` code
+### Environments
 
-Some demo code snippets may require setup and/or teardown code to properly function, which don't necessarily need to be displayed to the user. To run a chunk of Python code before any code the user runs in a particular code editor, add the `.py-pre` class to a fenced code block immediately before the user-visible code block, using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin. To run a chunk of code after a user runs a particular code editor add the `.py-post` class to a fenced code block immediately after the user-visible code block:
+Documentation may benefit from some executable code blocks being isolated from others to create distinct examples. Add the `env` attribute to a fenced code block, using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin, to create an editor for the [PyScript Environment](https://docs.pyscript.net/2024.4.2/user-guide/editor/), e.g. a specific copy of the interpreter isolated from other evnironments.
 
 ````
-```{.py .py-pre}
-print("This is some pre-code")
+```{.py env="one"}
+x = 1
 ```
 
-```py
-print("This is the main tag")
-# Only this code will be displayed in the code editor
+```{.py env="one"}
+print(x) # Shares an interpreter with the first block
 ```
 
-```{.py .py-post}
-print("This is some post code")
+```{.py env="two"}
+print(x) # Error: 'x' is not defined (in this interpreter)
+```
+````
+
+### `setup` code
+
+Some demo code snippets may require setup code to properly function, which don't necessarily need to be displayed to the user. To run a chunk of Python code before any code the user runs in a particular code editor, add the `setup` attribute to a fenced code block with a specific [environment](#Environments), using the style of the [attr_list](https://python-markdown.github.io/extensions/attr_list/) markdown plugin.
+
+````
+```{.py setup env="three"}
+print("This is some setup code")
+```
+
+```{.py env="three"}
+print("This is the main tag")
 ```
 ````
 
 ## Configuration
 
 `mkdocs-pyscript` supports  options that can be set in `mkdocs.yaml` to control the behavior of the plugin
 
 ### `pyscript_version`
 
-The `pyscript_version` property of the plugin controls the version of PyScript that is loaded. If not specified, the current default version is `snapshots/2023.09.1.RC2`.
+The `pyscript_version` property of the plugin controls the version of PyScript that is loaded. If not specified, the current default version is `releases/2024.4.2`.
 
 
 To support both pre-release snapshots and released versions of PyScript, the provided value is inserted into the following string:
 
 ```py
 SCRIPT = f'https://pyscript.net/{pyscript_version}/core.js'
 ```
 
 That is, to load a specific release or snapshot, use:
 ```yaml
 #Load a release
 plugins:
     - mkdocs-pyscript:
-        pyscript_version: "releases/2023.11.1"
+        pyscript_version: "releases/2024.2.1"
 
 #Load a snapshot
 plugins:
     - mkdocs-pyscript:
         pyscript_version: "snapshots/2023.11.1.RC3"
 
-#Load the most recent (unstable) build:
-plugins:
-    - mkdocs-pyscript:
-        pyscript_version: "unstable"
 ```
 
 ### `selective`
 
 By default, `mkdocs-pyscript` turns *all* blocks with type `py` or `python` into exectuable code snippets. To cause only selected blocks to be transformed:
 
-  1. Set the `selective` property to `true`:
+  1. Set the `selective` property to `true` in your configuration:
 ```yaml
 plugins:
     - mkdocs-pyscript:
         selective: true
 ```
   2. Specify `.pyscript` as an additional class for the codeblocks that you want to be runnable:
```

### Comparing `mkdocs-pyscript-0.1.1/mkdocs_pyscript.egg-info/SOURCES.txt` & `mkdocs_pyscript-0.2.0/mkdocs_pyscript.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 mkdocs_pyscript/__init__.py
 mkdocs_pyscript/plugin.py
-mkdocs_pyscript/prePostExtension.py
 mkdocs_pyscript.egg-info/PKG-INFO
 mkdocs_pyscript.egg-info/SOURCES.txt
 mkdocs_pyscript.egg-info/dependency_links.txt
 mkdocs_pyscript.egg-info/entry_points.txt
 mkdocs_pyscript.egg-info/requires.txt
 mkdocs_pyscript.egg-info/top_level.txt
 mkdocs_pyscript/dist/css/pyrepl.css
```

### Comparing `mkdocs-pyscript-0.1.1/setup.py` & `mkdocs_pyscript-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mkdocs-pyscript',
-    version='0.1.1',
+    version='0.2.0',
     description='Add PyScript to your mkdocs site',
     long_description= long_description,
     long_description_content_type='text/markdown',
     keywords=['mkdocs', 'pyscript'],
     url='https://github.com/jeffersglass/mkdocs-pyscript',
     author='Jeff Glass',
-    author_email='mail@jeff.glass',
+    author_email='glass.jeffrey@gmail.com',
     license='APACHE',
     python_requires='>=3.8',
     install_requires=[
         'mkdocs>=1.4.0',
         'beautifulsoup4>=4.1',
     ],
     classifiers=[
@@ -27,14 +27,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     packages=find_packages(),
     entry_points={
         'mkdocs.plugins': [
             'mkdocs-pyscript = mkdocs_pyscript.plugin:Plugin'
         ]
     },
```

### Comparing `mkdocs-pyscript-0.1.1/tests/conftest.py` & `mkdocs_pyscript-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocs-pyscript-0.1.1/tests/support.py` & `mkdocs_pyscript-0.2.0/tests/support.py`

 * *Files identical despite different names*

### Comparing `mkdocs-pyscript-0.1.1/tests/test_static.py` & `mkdocs_pyscript-0.2.0/tests/test_static.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,14 @@
         self.build_site('basic')
         with open(self._index_file, "r") as f:
             soup = bs4.BeautifulSoup(f, features="html.parser")
 
         head = soup.find("head")
         scripts: Iterable[bs4.element.Tag] = soup.find_all("script")
       
-        # check that importmap exists
-        assert any(('type' in script.attrs and script['type'] == "importmap") for script in scripts)
-
         # check that additional script tags exist
         assert any(('src' in script.attrs and "makeblocks.js" in script['src']) for script in scripts)
         assert any(('src' in script.attrs and "mini-coi.js" in script['src']) for script in scripts) 
 
     def test_code_blocks(self):
         self.build_site("basic")
         with open(self._index_file, "r") as f:
@@ -32,33 +29,27 @@
         # Make sure all three fences are convered to codeblocks
         assert len(wrappers) == 3
         for wrapper in wrappers:
             codeblock = wrapper.code
         
         #TODO Check contents of codeblocks
             
-    def test_pre_post(self):
+    def test_setup(self):
         self.build_site("prepost")
         with open(self._index_file, "r") as f:
             soup = bs4.BeautifulSoup(f, features="html.parser")
 
         body = soup.find('body')
         wrappers: Iterable[bs4.element.Tag] = body.find_all(class_ = 'py-wrapper')
 
         # Make sure all one one codeblock is emitted are convered to codeblocks
-        assert len(wrappers) == 1
+        assert len(wrappers) == 2
         for wrapper in wrappers:
             codeblock = wrapper.code
 
-        pre_tags = soup.find_all('script', attrs={"type": "py-pre"})
+        pre_tags = soup.find_all('script', attrs={"type": "py-editor", "setup": ""})
         assert len(pre_tags) == 1
-        assert pre_tags[0].text.strip() == 'print("This is some pre-code")'
-
-        post_tags = soup.find_all('script', attrs={"type": "py-post"}) 
-        assert len(post_tags) == 1
-        assert post_tags[0].text.strip() == 'print("This is some post code")'
-
-        #TODO check contents of code block, pre and post tags
+        assert pre_tags[0].text.strip() == 'print("This is some setup code")'
```

