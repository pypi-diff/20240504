# Comparing `tmp/c4t-1.4.0.tar.gz` & `tmp/c4t-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4t-1.4.0.tar", last modified: Wed May  1 00:04:31 2024, max compression
+gzip compressed data, was "c4t-1.5.0.tar", last modified: Fri May  3 07:49:50 2024, max compression
```

## Comparing `c4t-1.4.0.tar` & `c4t-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.285895 c4t-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 00:04:25.000000 c4t-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-01 00:04:31.281895 c4t-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-01 00:04:25.000000 c4t-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-01 00:04:25.000000 c4t-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:04:31.285895 c4t-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-01 00:04:25.000000 c4t-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.277896 c4t-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.277896 c4t-1.4.0/src/c4t/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-01 00:04:25.000000 c4t-1.4.0/src/c4t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-01 00:04:25.000000 c4t-1.4.0/src/c4t/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.281895 c4t-1.4.0/src/c4t.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-01 00:04:31.000000 c4t-1.4.0/src/c4t.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:04:31.281895 c4t-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-01 00:04:25.000000 c4t-1.4.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:49:50.087146 c4t-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 07:49:43.000000 c4t-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-03 07:49:50.087146 c4t-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-03 07:49:43.000000 c4t-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-03 07:49:43.000000 c4t-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:49:50.087146 c4t-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-03 07:49:43.000000 c4t-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:49:50.079146 c4t-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:49:50.083146 c4t-1.5.0/src/c4t/
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-05-03 07:49:43.000000 c4t-1.5.0/src/c4t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-03 07:49:43.000000 c4t-1.5.0/src/c4t/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:49:50.083146 c4t-1.5.0/src/c4t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-03 07:49:50.000000 c4t-1.5.0/src/c4t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-03 07:49:50.000000 c4t-1.5.0/src/c4t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:49:50.000000 c4t-1.5.0/src/c4t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 07:49:50.000000 c4t-1.5.0/src/c4t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 07:49:50.000000 c4t-1.5.0/src/c4t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 07:49:50.000000 c4t-1.5.0/src/c4t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:49:50.083146 c4t-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-03 07:49:43.000000 c4t-1.5.0/tests/tests.py
```

### Comparing `c4t-1.4.0/LICENSE` & `c4t-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `c4t-1.4.0/PKG-INFO` & `c4t-1.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,17 @@
-Metadata-Version: 2.1
-Name: c4t
-Version: 1.4.0
-Summary: Install Chrome for Testing assets.
-Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
-Project-URL: Homepage, https://github.com/p4irin/c4t
-Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
-Keywords: chrome,testing,selenium,chromedriver,cft
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: wget>=3.2
-Provides-Extra: lint
-Requires-Dist: mypy>=1.9.0; extra == "lint"
-Requires-Dist: types-requests>=2.31.0.20240311; extra == "lint"
-Requires-Dist: ruff>=0.3.4; extra == "lint"
-Provides-Extra: test
-Requires-Dist: selenium>=4.12.0; extra == "test"
-Requires-Dist: pytest>=8.1.1; extra == "test"
-Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Provides-Extra: package
-Requires-Dist: build==0.10.0; extra == "package"
-Requires-Dist: twine>=4.0.2; extra == "package"
-Provides-Extra: dev
-Requires-Dist: bumpver>=2023.1126; extra == "dev"
-Requires-Dist: c4t[lint]; extra == "dev"
-Requires-Dist: c4t[test]; extra == "dev"
-Requires-Dist: c4t[package]; extra == "dev"
-
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 [![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.4.0
+# c4t: Chrome for Testing - v1.5.0
 
-Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
+Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. Currently, the version of assets installed is for _linux64_ platforms only.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 
 > ...setting up an adequate browser testing environment is notoriously difficult...
 >
@@ -156,18 +116,43 @@
 
 ### On the command line
 
 #### Display command line help
 
 ```bash
 (venv) $ c4t --help
+usage: c4t [-h] [-V] {install,path,list,switch} ...
+
+Install 'Chrome for Testing' assets.
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Show version and exit.
+
+Commands:
+  {install,path,list,switch}
+    install             Install a version of 'Chrome for Testing' assets.
+    path                Show the installation path of assets and exit.
+    list                List versions
+    switch              Switch the active version.
+
+Reference: https://github.com/GoogleChromeLabs/chrome-for-testing
 ```
 
 ```bash
 (venv) $ c4t install --help
+usage: c4t install [-h] [--version VERSION] [-l]
+
+Install a version of 'Chrome for Testing' assets.
+
+options:
+  -h, --help            show this help message and exit
+  --version VERSION     The version of 'Chrome for Testing' assets to install. The default is 'latest'
+  -l, --last-known-good-version
+                        Install a last known good version from a list
 ```
 
 #### Install the default, the latest stable version
 
 ```bash
 # By default assets are installed in ${HOME}/.c4t-assets
 # To use a different path, set the C4T_PATH_TO_ASSETS environment variable.
@@ -178,53 +163,80 @@
 
 #### Install a specific version
 
 ```bash
 (venv) $ c4t install --version 116.0.5794.0
 ```
 
-#### Show the currently active version
+#### Install a last known good version from a list
 
 ```bash
-(venv) $ c4t --active
-Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
+# Notice the list also indicates versions you already installed
+(venv) $ c4t install -l
+0 - Stable version=124.0.6367.91, revision=1274542, installed
+1 - Beta version=125.0.6422.26, revision=1287751
+2 - Dev version=126.0.6439.0, revision=1292160, installed
+3 - Canary version=126.0.6449.0, revision=1293886
+Select a version by number:
 ```
 
 #### Show installation path of assets
 
 ```bash
 (venv) $ c4t path
 Path to assets: /home/p4irin/.c4t-assets
 ```
 
+#### Show the currently active version
+
+```bash
+(venv) $ c4t list --active
+Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
+```
+
 #### Show a list of installed versions
 
 ```bash
-(venv) $ c4t list
-1 - 124.0.6367.91
-2 - 116.0.5794.0
+# Notice the active version is marked 'active'
+(venv) $ c4t list --installed
+0 - 116.0.5794.0
+1 - 124.0.6367.91, active
+2 - 125.0.6422.14
+3 - 126.0.6439.0
+```
+
+#### Show a list of last known good versions
+
+```bash
+(venv) $ c4t list --last-known-good-versions
+0 - Stable version=124.0.6367.91, revision=1274542, installed
+1 - Beta version=125.0.6422.26, revision=1287751
+2 - Dev version=126.0.6439.0, revision=1292160, installed
+3 - Canary version=126.0.6449.0, revision=1293886
 ```
 
 #### Switch active version
 
 ```bash
 (venv) $ c4t switch
-1 - 124.0.6367.91
-2 - 116.0.5794.0
-Select a version by number: 2
+0 - 116.0.5794.0
+1 - 124.0.6367.91, active
+2 - 125.0.6422.14
+3 - 126.0.6439.0
+Select a version by number: 0
 Creating symlink to chrome version 116.0.5794.0
 Creating symlink to chromedriver version 116.0.5794.0
 Active version is now: 116.0.5794.0
 ```
 
 ### Common workflow
 
 1. Install one or more versions of Chrome for testing assets
 1. Set/switch the active version
 1. Run your Selenium Webdriver tests with the active version of Chrome for testing
 
-This allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
+E.g., this allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
 
 ## Reference
 
 - [Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 - [GitHub](https://github.com/GoogleChromeLabs/chrome-for-testing)
```

### Comparing `c4t-1.4.0/README.md` & `c4t-1.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,57 @@
+Metadata-Version: 2.1
+Name: c4t
+Version: 1.5.0
+Summary: Install Chrome for Testing assets.
+Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/p4irin/c4t
+Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
+Keywords: chrome,testing,selenium,chromedriver,cft
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: wget>=3.2
+Provides-Extra: lint
+Requires-Dist: mypy>=1.9.0; extra == "lint"
+Requires-Dist: types-requests>=2.31.0.20240311; extra == "lint"
+Requires-Dist: ruff>=0.3.4; extra == "lint"
+Provides-Extra: test
+Requires-Dist: selenium>=4.12.0; extra == "test"
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: pytest-cov>=4.1.0; extra == "test"
+Provides-Extra: package
+Requires-Dist: build==0.10.0; extra == "package"
+Requires-Dist: twine>=4.0.2; extra == "package"
+Provides-Extra: dev
+Requires-Dist: bumpver>=2023.1126; extra == "dev"
+Requires-Dist: c4t[lint]; extra == "dev"
+Requires-Dist: c4t[test]; extra == "dev"
+Requires-Dist: c4t[package]; extra == "dev"
+
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 [![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.4.0
+# c4t: Chrome for Testing - v1.5.0
 
-Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
+Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. Currently, the version of assets installed is for _linux64_ platforms only.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 
 > ...setting up an adequate browser testing environment is notoriously difficult...
 >
@@ -116,18 +156,43 @@
 
 ### On the command line
 
 #### Display command line help
 
 ```bash
 (venv) $ c4t --help
+usage: c4t [-h] [-V] {install,path,list,switch} ...
+
+Install 'Chrome for Testing' assets.
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Show version and exit.
+
+Commands:
+  {install,path,list,switch}
+    install             Install a version of 'Chrome for Testing' assets.
+    path                Show the installation path of assets and exit.
+    list                List versions
+    switch              Switch the active version.
+
+Reference: https://github.com/GoogleChromeLabs/chrome-for-testing
 ```
 
 ```bash
 (venv) $ c4t install --help
+usage: c4t install [-h] [--version VERSION] [-l]
+
+Install a version of 'Chrome for Testing' assets.
+
+options:
+  -h, --help            show this help message and exit
+  --version VERSION     The version of 'Chrome for Testing' assets to install. The default is 'latest'
+  -l, --last-known-good-version
+                        Install a last known good version from a list
 ```
 
 #### Install the default, the latest stable version
 
 ```bash
 # By default assets are installed in ${HOME}/.c4t-assets
 # To use a different path, set the C4T_PATH_TO_ASSETS environment variable.
@@ -138,53 +203,80 @@
 
 #### Install a specific version
 
 ```bash
 (venv) $ c4t install --version 116.0.5794.0
 ```
 
-#### Show the currently active version
+#### Install a last known good version from a list
 
 ```bash
-(venv) $ c4t --active
-Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
+# Notice the list also indicates versions you already installed
+(venv) $ c4t install -l
+0 - Stable version=124.0.6367.91, revision=1274542, installed
+1 - Beta version=125.0.6422.26, revision=1287751
+2 - Dev version=126.0.6439.0, revision=1292160, installed
+3 - Canary version=126.0.6449.0, revision=1293886
+Select a version by number:
 ```
 
 #### Show installation path of assets
 
 ```bash
 (venv) $ c4t path
 Path to assets: /home/p4irin/.c4t-assets
 ```
 
+#### Show the currently active version
+
+```bash
+(venv) $ c4t list --active
+Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
+```
+
 #### Show a list of installed versions
 
 ```bash
-(venv) $ c4t list
-1 - 124.0.6367.91
-2 - 116.0.5794.0
+# Notice the active version is marked 'active'
+(venv) $ c4t list --installed
+0 - 116.0.5794.0
+1 - 124.0.6367.91, active
+2 - 125.0.6422.14
+3 - 126.0.6439.0
+```
+
+#### Show a list of last known good versions
+
+```bash
+(venv) $ c4t list --last-known-good-versions
+0 - Stable version=124.0.6367.91, revision=1274542, installed
+1 - Beta version=125.0.6422.26, revision=1287751
+2 - Dev version=126.0.6439.0, revision=1292160, installed
+3 - Canary version=126.0.6449.0, revision=1293886
 ```
 
 #### Switch active version
 
 ```bash
 (venv) $ c4t switch
-1 - 124.0.6367.91
-2 - 116.0.5794.0
-Select a version by number: 2
+0 - 116.0.5794.0
+1 - 124.0.6367.91, active
+2 - 125.0.6422.14
+3 - 126.0.6439.0
+Select a version by number: 0
 Creating symlink to chrome version 116.0.5794.0
 Creating symlink to chromedriver version 116.0.5794.0
 Active version is now: 116.0.5794.0
 ```
 
 ### Common workflow
 
 1. Install one or more versions of Chrome for testing assets
 1. Set/switch the active version
 1. Run your Selenium Webdriver tests with the active version of Chrome for testing
 
-This allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
+E.g., this allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
 
 ## Reference
 
 - [Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 - [GitHub](https://github.com/GoogleChromeLabs/chrome-for-testing)
```

### Comparing `c4t-1.4.0/pyproject.toml` & `c4t-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c4t"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
   { name="p4irin", email="139928764+p4irin@users.noreply.github.com" },
 ]
 description = "Install Chrome for Testing assets."
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -65,15 +65,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "1.4.0"
+current_version = "1.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `c4t-1.4.0/setup.py` & `c4t-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `c4t-1.4.0/src/c4t/__init__.py` & `c4t-1.5.0/src/c4t/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     browser.close()
     browser.quit()
 """
 
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.4.0'
+__version__ = '1.5.0'
 
 
 import requests
 import os
 import json
 import wget
 import zipfile
@@ -393,12 +393,82 @@
         )
 
         print(self._successful_installation_message.format(version=version))
 
     @property
     def path(self) -> str:
         return _path_to_assets
+
+    def installed(self, output: bool=True) -> List[str]:
+        """List installed versions"""
+
+        versions = []
+        items = [item for item in os.listdir(self.path) if os.path.isdir(f'{self.path}/{item}')]
+        items.sort()
+        for n, item in enumerate(items, start=0):
+            if os.path.isdir(f'{self.path}/{item}'):
+                if output:
+                    active = ', active' if item == self.active_version else ''
+                    print(f'{n} - {item}{active}')
+                versions.append(item)
+        return versions
+    
+    def _isinstalled(self, version: str) -> bool:
+        installed_versions = self.installed(output=False)
+        if version in installed_versions:
+            return True
+        else:
+            return False
+    
+    def switch(self) -> None:
+        """Switch the active version"""
+
+        versions = self.installed()
+
+        try:
+            selection = int(input("Select a version by number: "))
+        except ValueError:
+            selection = None
+        except IndexError:
+            selection = None
+
+        if selection is not None:
+            version = versions[selection]
+            self._create_symlink(to_binary='chrome', version=version)
+            self._create_symlink(to_binary='chromedriver', version=version)
+            print(f'Active version is now: {version}')
+
+    def last_known_good_versions(self) -> List[str]:
+        """List last known good versions"""
+
+        versions = []
+        try:
+            r = requests.get(
+                self._last_known_good_versions_json_api_endpoint
+            )
+        except requests.exceptions.RequestException as e:
+            raise SystemExit(e)
+        
+        json_response = json.loads(r.text)
+        channels = json_response['channels']
+        for n, channel in enumerate(channels, start=0):
+            version = channels[channel]['version']
+            revision = channels[channel]['revision']
+            if self._isinstalled(version):
+                installed = ', installed'
+            else:
+                installed = ''
+            print(f'{n} - {channel} version={version}, revision={revision}{installed}')
+            versions.append(version)
+        return versions
     
-    def switch(self, to_version: str) -> None:
-        self._create_symlink(to_binary='chrome', version=to_version)
-        self._create_symlink(to_binary='chromedriver', version=to_version)
-        print(f'Active version is now: {to_version}')
+    def install_last_known_good_version(self) -> None:
+        versions = self.last_known_good_versions()
+        try:
+            selection = int(input('Select a version by number: '))
+        except ValueError:
+            selection = None
+        except IndexError:
+            selection = None
+
+        if selection is not None:
+            self.install(version=versions[selection])
```

### Comparing `c4t-1.4.0/src/c4t/cli.py` & `c4t-1.5.0/src/c4t/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,13 @@
 import argparse
-import os
-import typing
 from . import Assets, __version__
 
 assets = Assets()
 
 
-def list_versions() -> list:
-    versions = []
-    items = os.listdir(assets.path)
-    for n, item in enumerate(items, start=0):
-        if os.path.isdir(f'{assets.path}/{item}'):
-            print(f'{n} - {item}')
-            versions.append(item)
-    return versions
-
-
-def select_version(versions: list) -> typing.Union[str, None]:
-    try:
-        selection = int(input("Select a version by number: ")) - 1
-        return versions[selection]
-    except ValueError:
-        return None
-    except IndexError:
-        return None
-
-
 def cli() -> None:
     parser = argparse.ArgumentParser(
         description="Install 'Chrome for Testing' assets.",
         epilog='Reference: https://github.com/GoogleChromeLabs/'
                +'chrome-for-testing'
     )
 
@@ -37,67 +15,95 @@
         '-V',
         '--version',
         action='version',
         version=f'v{__version__}',
         help='Show version and exit.'
     )
 
-    parser.add_argument(
-        '-a',
-        '--active',
-        action='store_true',
-        help="Show the currently active version of 'Chrome for Testing' assets"
-             + " installed."
-    )
     sub_parsers = parser.add_subparsers(
         title='Commands',
         dest='command'
     )
 
+    help_install = "Install a version of 'Chrome for Testing' assets."
     sp_install = sub_parsers.add_parser(
         'install',
-        help="Install a version of 'Chrome for Testing' assets."
+        description=help_install,
+        help=help_install
     )
     sp_install.add_argument(
         '--version',
         default='latest',
         help="The version of 'Chrome for Testing' assets to install. " +
              "The default is '%(default)s'"
     )
+    sp_install.add_argument(
+        '-l',
+        '--last-known-good-version',
+        action='store_true',
+        help='Install a last known good version from a list'
+    )
 
+    help_path = 'Show the installation path of assets and exit.'
     sub_parsers.add_parser(
         'path',
-        help='Show the installation path of assets and exit.'
+        description=help_path,
+        help=help_path
     )
 
-    sub_parsers.add_parser(
+    help_list = 'List versions'
+    sp_list = sub_parsers.add_parser(
         'list',
-        help='Show installed versions.'
+        description=help_list,
+        help=help_list
+    )
+    sp_list.add_argument(
+        '-a',
+        '--active',
+        action='store_true',
+        help="List the currently active version of 'Chrome for Testing' assets"
+             + " installed."
+    )
+    sp_list.add_argument(
+        '-i',
+        '--installed',
+        action='store_true',
+        help='List installed versions'
+    )
+    sp_list.add_argument(
+        '-l',
+        '--last-known-good-versions',
+        action='store_true',
+        help='List last known good versions'
     )
 
+    help_switch = 'Switch the active version.'
     sub_parsers.add_parser(
         'switch',
-        help='Switch the active version.'
+        description=help_switch,
+        help=help_switch
     )    
 
     args = parser.parse_args()
 
-    if args.active:
-        print("Active version of 'Chrome for Testing' assets installed: "
-              + f'{assets.active_version}'
-        )
-
     if args.command == 'install':
-        print(f"Installing version '{args.version}'")
-        assets.install(version=args.version)
+        if args.last_known_good_version:
+            assets.install_last_known_good_version()
+        else:
+            print(f"Installing version '{args.version}'")
+            assets.install(version=args.version)
 
     if args.command == 'path':
         print(f'Path to assets: {assets.path}')
 
     if args.command == 'list':
-        list_versions()
+        if args.installed:
+            assets.installed()
+        if args.active:
+            print("Active version of 'Chrome for Testing' assets installed: "
+                + f'{assets.active_version}'
+        )
+        if args.last_known_good_versions:
+            assets.last_known_good_versions()
 
     if args.command == 'switch':
-        versions = list_versions()
-        version = select_version(versions)
-        if version is not None:
-            assets.switch(to_version=version)
+        assets.switch()
```

### Comparing `c4t-1.4.0/src/c4t.egg-info/PKG-INFO` & `c4t-1.5.0/src/c4t.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4t
-Version: 1.4.0
+Version: 1.5.0
 Summary: Install Chrome for Testing assets.
 Author-email: p4irin <139928764+p4irin@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/p4irin/c4t
 Project-URL: Bug Tracker, https://github.com/p4irin/c4t/issues
 Keywords: chrome,testing,selenium,chromedriver,cft
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -41,17 +41,17 @@
 [![Build Status](https://dev.azure.com/p4irin/c4t/_apis/build/status%2Fp4irin.c4t?branchName=master&jobName=BuildAndTest&configuration=BuildAndTest%20Python38)](https://dev.azure.com/p4irin/c4t/_build/latest?definitionId=5&branchName=master)
 [![c4t publish](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml/badge.svg)](https://github.com/p4irin/c4t/actions/workflows/python-publish.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/c4t)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/c4t)
 ![PyPI - Format](https://img.shields.io/pypi/format/c4t)
 ![PyPI - License](https://img.shields.io/pypi/l/c4t)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-# c4t: Chrome for Testing - v1.4.0
+# c4t: Chrome for Testing - v1.5.0
 
-Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. The version of assets installed are from the stable channel and currently only for _linux64_ platforms.
+Install _Chrome for Testing_ assets. A flavor of Chrome, specifically for testing and a matching chromedriver. Currently, the version of assets installed is for _linux64_ platforms only.
 
 ## Why Chrome for Testing?
 
 Taken from [the Chrome Developers Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 
 > ...setting up an adequate browser testing environment is notoriously difficult...
 >
@@ -156,18 +156,43 @@
 
 ### On the command line
 
 #### Display command line help
 
 ```bash
 (venv) $ c4t --help
+usage: c4t [-h] [-V] {install,path,list,switch} ...
+
+Install 'Chrome for Testing' assets.
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         Show version and exit.
+
+Commands:
+  {install,path,list,switch}
+    install             Install a version of 'Chrome for Testing' assets.
+    path                Show the installation path of assets and exit.
+    list                List versions
+    switch              Switch the active version.
+
+Reference: https://github.com/GoogleChromeLabs/chrome-for-testing
 ```
 
 ```bash
 (venv) $ c4t install --help
+usage: c4t install [-h] [--version VERSION] [-l]
+
+Install a version of 'Chrome for Testing' assets.
+
+options:
+  -h, --help            show this help message and exit
+  --version VERSION     The version of 'Chrome for Testing' assets to install. The default is 'latest'
+  -l, --last-known-good-version
+                        Install a last known good version from a list
 ```
 
 #### Install the default, the latest stable version
 
 ```bash
 # By default assets are installed in ${HOME}/.c4t-assets
 # To use a different path, set the C4T_PATH_TO_ASSETS environment variable.
@@ -178,53 +203,80 @@
 
 #### Install a specific version
 
 ```bash
 (venv) $ c4t install --version 116.0.5794.0
 ```
 
-#### Show the currently active version
+#### Install a last known good version from a list
 
 ```bash
-(venv) $ c4t --active
-Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
+# Notice the list also indicates versions you already installed
+(venv) $ c4t install -l
+0 - Stable version=124.0.6367.91, revision=1274542, installed
+1 - Beta version=125.0.6422.26, revision=1287751
+2 - Dev version=126.0.6439.0, revision=1292160, installed
+3 - Canary version=126.0.6449.0, revision=1293886
+Select a version by number:
 ```
 
 #### Show installation path of assets
 
 ```bash
 (venv) $ c4t path
 Path to assets: /home/p4irin/.c4t-assets
 ```
 
+#### Show the currently active version
+
+```bash
+(venv) $ c4t list --active
+Active version of 'Chrome for Testing' assets installed: 124.0.6367.91
+```
+
 #### Show a list of installed versions
 
 ```bash
-(venv) $ c4t list
-1 - 124.0.6367.91
-2 - 116.0.5794.0
+# Notice the active version is marked 'active'
+(venv) $ c4t list --installed
+0 - 116.0.5794.0
+1 - 124.0.6367.91, active
+2 - 125.0.6422.14
+3 - 126.0.6439.0
+```
+
+#### Show a list of last known good versions
+
+```bash
+(venv) $ c4t list --last-known-good-versions
+0 - Stable version=124.0.6367.91, revision=1274542, installed
+1 - Beta version=125.0.6422.26, revision=1287751
+2 - Dev version=126.0.6439.0, revision=1292160, installed
+3 - Canary version=126.0.6449.0, revision=1293886
 ```
 
 #### Switch active version
 
 ```bash
 (venv) $ c4t switch
-1 - 124.0.6367.91
-2 - 116.0.5794.0
-Select a version by number: 2
+0 - 116.0.5794.0
+1 - 124.0.6367.91, active
+2 - 125.0.6422.14
+3 - 126.0.6439.0
+Select a version by number: 0
 Creating symlink to chrome version 116.0.5794.0
 Creating symlink to chromedriver version 116.0.5794.0
 Active version is now: 116.0.5794.0
 ```
 
 ### Common workflow
 
 1. Install one or more versions of Chrome for testing assets
 1. Set/switch the active version
 1. Run your Selenium Webdriver tests with the active version of Chrome for testing
 
-This allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
+E.g., this allows for quickly switching back to a previous version of Chrome to run your tests against in case of a regression on a recent/latest version. For example, a test failing against the latest of Chrome, did it pass consistently on the previous version or is it flaky and in need for a more robust implementation?
 
 ## Reference
 
 - [Blog](https://developer.chrome.com/blog/chrome-for-testing/)
 - [GitHub](https://github.com/GoogleChromeLabs/chrome-for-testing)
```

### Comparing `c4t-1.4.0/tests/tests.py` & `c4t-1.5.0/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 from selenium.webdriver import ChromeOptions, ChromeService, Chrome
 import c4t
 
 __author__ = 'p4irin'
 __email__ = '139928764+p4irin@users.noreply.github.com'
-__version__ = '1.4.0'
+__version__ = '1.5.0'
 
 
 class C4tTests(unittest.TestCase):
 
     class _TestData:
         specific_version_of_assets = '116.0.5794.0'
```

