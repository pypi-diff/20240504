# Comparing `tmp/nmk-0.9.1.tar.gz` & `tmp/nmk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-0.9.1.tar", last modified: Sat Jan 21 15:20:37 2023, max compression
+gzip compressed data, was "nmk-0.9.2.tar", last modified: Thu Nov 23 08:44:46 2023, max compression
```

## Comparing `nmk-0.9.1.tar` & `nmk-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:37.079771 nmk-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-21 15:20:15.000000 nmk-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-21 15:20:37.083771 nmk-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-21 15:20:35.000000 nmk-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-21 15:20:37.083771 nmk-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-21 15:20:35.000000 nmk-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:37.075771 nmk-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:37.079771 nmk-0.9.1/src/nmk/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:37.079771 nmk-0.9.1/src/nmk/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/model.yml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:37.079771 nmk-0.9.1/src/nmk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/tests/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-01-21 15:20:15.000000 nmk-0.9.1/src/nmk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 15:20:37.079771 nmk-0.9.1/src/nmk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-21 15:20:37.000000 nmk-0.9.1/src/nmk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-21 15:20:37.000000 nmk-0.9.1/src/nmk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 15:20:37.000000 nmk-0.9.1/src/nmk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-21 15:20:37.000000 nmk-0.9.1/src/nmk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-21 15:20:37.000000 nmk-0.9.1/src/nmk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-21 15:20:37.000000 nmk-0.9.1/src/nmk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:46.175554 nmk-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-23 08:44:24.000000 nmk-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-11-23 08:44:46.175554 nmk-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-11-23 08:44:44.000000 nmk-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-23 08:44:46.175554 nmk-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-23 08:44:44.000000 nmk-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:46.171554 nmk-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:46.171554 nmk-0.9.2/src/nmk/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:46.175554 nmk-0.9.2/src/nmk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/model.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:46.175554 nmk-0.9.2/src/nmk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/tests/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2023-11-23 08:44:24.000000 nmk-0.9.2/src/nmk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 08:44:46.175554 nmk-0.9.2/src/nmk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-11-23 08:44:46.000000 nmk-0.9.2/src/nmk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-23 08:44:46.000000 nmk-0.9.2/src/nmk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 08:44:46.000000 nmk-0.9.2/src/nmk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-23 08:44:46.000000 nmk-0.9.2/src/nmk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-23 08:44:46.000000 nmk-0.9.2/src/nmk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-23 08:44:46.000000 nmk-0.9.2/src/nmk.egg-info/top_level.txt
```

### Comparing `nmk-0.9.1/LICENSE` & `nmk-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/PKG-INFO` & `nmk-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nmk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Next-gen make-like build system
 Home-page: https://github.com/dynod/nmk
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk - next-gen make-like build system
         
         <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk)](https://github.com/dynod/nmk/blob/main/LICENSE)
+        [![License: MPL](https://img.shields.io/github/license/dynod/nmk?color=green)](https://github.com/dynod/nmk/blob/main/LICENSE)
         [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk/actions?query=branch%3Amain)
         [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue)
         [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
         [![PyPI](https://img.shields.io/pypi/v/nmk)](https://pypi.org/project/nmk/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
         [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk)](https://app.codecov.io/gh/dynod/nmk)
```

### Comparing `nmk-0.9.1/README.md` & `nmk-0.9.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # nmk - next-gen make-like build system
 
 <!-- NMK-BADGES-BEGIN -->
-[![License: MPL](https://img.shields.io/github/license/dynod/nmk)](https://github.com/dynod/nmk/blob/main/LICENSE)
+[![License: MPL](https://img.shields.io/github/license/dynod/nmk?color=green)](https://github.com/dynod/nmk/blob/main/LICENSE)
 [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk/actions?query=branch%3Amain)
 [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue)
 [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/nmk)](https://pypi.org/project/nmk/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
 [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk)](https://app.codecov.io/gh/dynod/nmk)
```

### Comparing `nmk-0.9.1/setup.cfg` & `nmk-0.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 ignore = E203,E501,B902,W503
 jobs = auto
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk
-version = 0.9.1
+author = The dynod project
+maintainer = The dynod project
+version = 0.9.2
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
-author = The dynod project
-maintainer = The dynod project
 url = https://github.com/dynod/nmk
 description = Next-gen make-like build system
 
 [options]
 package_dir = =src
 packages = find:
 install_requires =
```

### Comparing `nmk-0.9.1/src/nmk/__main__.py` & `nmk-0.9.2/src/nmk/__main__.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/build.py` & `nmk-0.9.2/src/nmk/build.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/completion.py` & `nmk-0.9.2/src/nmk/completion.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/logs.py` & `nmk-0.9.2/src/nmk/logs.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/builder.py` & `nmk-0.9.2/src/nmk/model/builder.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/cache.py` & `nmk-0.9.2/src/nmk/model/cache.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/config.py` & `nmk-0.9.2/src/nmk/model/config.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/files.py` & `nmk-0.9.2/src/nmk/model/files.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/loader.py` & `nmk-0.9.2/src/nmk/model/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             NmkRootConfig.BASE_DIR: "",  # Useless while directly referenced (must identify current project file parent dir)
             NmkRootConfig.ROOT_DIR: root,
             NmkRootConfig.ROOT_NMK_DIR: self.root_nmk_dir,
             NmkRootConfig.CACHE_DIR: self.repo_cache,
             NmkRootConfig.PROJECT_DIR: "",  # Will be updated as soon as initial project is loaded
             NmkRootConfig.PROJECT_NMK_DIR: "",  # Will be updated as soon as initial project is loaded
             NmkRootConfig.PROJECT_FILES: [],  # Will be updated as soon as files are loaded
-            NmkRootConfig.ENV: {k: v for k, v in os.environ.items()},
+            NmkRootConfig.ENV: dict(os.environ),
         }.items():
             self.model.add_config(name, None, value)
 
         # Init recursive files loading loop
         NmkModelFile(self.model.args.project, self.repo_cache, self.model, [])
 
         # Refresh project files list
```

### Comparing `nmk-0.9.1/src/nmk/model/model.py` & `nmk-0.9.2/src/nmk/model/model.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/model.yml` & `nmk-0.9.2/src/nmk/model/model.yml`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/resolver.py` & `nmk-0.9.2/src/nmk/model/resolver.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/model/task.py` & `nmk-0.9.2/src/nmk/model/task.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/parser.py` & `nmk-0.9.2/src/nmk/parser.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/tests/tester.py` & `nmk-0.9.2/src/nmk/tests/tester.py`

 * *Files identical despite different names*

### Comparing `nmk-0.9.1/src/nmk/utils.py` & `nmk-0.9.2/src/nmk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def run_with_logs(args: List[str], logger=NmkLogger, check: bool = True, cwd: Path = None) -> subprocess.CompletedProcess:
     """
     Execute subprocess, and logs output/error streams + error code
     """
     logger.debug(f"Running command: {args}")
-    cp = subprocess.run(args, check=False, capture_output=True, text=True, encoding="utf-8", cwd=cwd)
+    cp = subprocess.run(args, check=False, capture_output=True, text=True, encoding="utf-8", errors="ignore", cwd=cwd)
     logger.debug(f">> rc: {cp.returncode}")
     logger.debug(">> stderr:")
     list(map(logger.debug, cp.stderr.splitlines(keepends=False)))
     logger.debug(">> stdout:")
     list(map(logger.debug, cp.stdout.splitlines(keepends=False)))
     assert not check or cp.returncode == 0, (
         f"command returned {cp.returncode}" + (f"\n{cp.stdout}" if len(cp.stdout) else "") + (f"\n{cp.stderr}" if len(cp.stderr) else "")
```

### Comparing `nmk-0.9.1/src/nmk.egg-info/PKG-INFO` & `nmk-0.9.2/src/nmk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nmk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Next-gen make-like build system
 Home-page: https://github.com/dynod/nmk
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk - next-gen make-like build system
         
         <!-- NMK-BADGES-BEGIN -->
-        [![License: MPL](https://img.shields.io/github/license/dynod/nmk)](https://github.com/dynod/nmk/blob/main/LICENSE)
+        [![License: MPL](https://img.shields.io/github/license/dynod/nmk?color=green)](https://github.com/dynod/nmk/blob/main/LICENSE)
         [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk/actions?query=branch%3Amain)
         [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue)
         [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
         [![PyPI](https://img.shields.io/pypi/v/nmk)](https://pypi.org/project/nmk/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
         [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk)](https://app.codecov.io/gh/dynod/nmk)
```

### Comparing `nmk-0.9.1/src/nmk.egg-info/SOURCES.txt` & `nmk-0.9.2/src/nmk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

