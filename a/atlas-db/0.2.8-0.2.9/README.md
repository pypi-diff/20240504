# Comparing `tmp/atlas_db-0.2.8.tar.gz` & `tmp/atlas_db-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas_db-0.2.8.tar", last modified: Sat May  4 19:30:32 2024, max compression
+gzip compressed data, was "atlas_db-0.2.9.tar", last modified: Sat May  4 19:38:54 2024, max compression
```

## Comparing `atlas_db-0.2.8.tar` & `atlas_db-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:30:32.871886 atlas_db-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 19:30:26.000000 atlas_db-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-04 19:30:32.871886 atlas_db-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-04 19:30:26.000000 atlas_db-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:30:32.867886 atlas_db-0.2.8/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 19:30:26.000000 atlas_db-0.2.8/atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 19:30:26.000000 atlas_db-0.2.8/atlas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-04 19:30:26.000000 atlas_db-0.2.8/atlas/apple_health.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-04 19:30:26.000000 atlas_db-0.2.8/atlas/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:30:32.871886 atlas_db-0.2.8/atlas_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-04 19:30:32.000000 atlas_db-0.2.8/atlas_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-04 19:30:32.000000 atlas_db-0.2.8/atlas_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:30:32.000000 atlas_db-0.2.8/atlas_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 19:30:32.000000 atlas_db-0.2.8/atlas_db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-04 19:30:32.000000 atlas_db-0.2.8/atlas_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 19:30:32.000000 atlas_db-0.2.8/atlas_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-04 19:30:26.000000 atlas_db-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:30:32.871886 atlas_db-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:30:32.867886 atlas_db-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 19:30:26.000000 atlas_db-0.2.8/tests/test_expanse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:38:54.395063 atlas_db-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 19:38:48.000000 atlas_db-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-04 19:38:54.395063 atlas_db-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-04 19:38:48.000000 atlas_db-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:38:54.391064 atlas_db-0.2.9/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 19:38:48.000000 atlas_db-0.2.9/atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 19:38:48.000000 atlas_db-0.2.9/atlas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-04 19:38:48.000000 atlas_db-0.2.9/atlas/apple_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-04 19:38:48.000000 atlas_db-0.2.9/atlas/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:38:54.395063 atlas_db-0.2.9/atlas_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-04 19:38:54.000000 atlas_db-0.2.9/atlas_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-04 19:38:54.000000 atlas_db-0.2.9/atlas_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:38:54.000000 atlas_db-0.2.9/atlas_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 19:38:54.000000 atlas_db-0.2.9/atlas_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-04 19:38:54.000000 atlas_db-0.2.9/atlas_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 19:38:54.000000 atlas_db-0.2.9/atlas_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-04 19:38:48.000000 atlas_db-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:38:54.395063 atlas_db-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:38:54.395063 atlas_db-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 19:38:48.000000 atlas_db-0.2.9/tests/test_expanse.py
```

### Comparing `atlas_db-0.2.8/LICENSE` & `atlas_db-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atlas_db-0.2.8/PKG-INFO` & `atlas_db-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-db
-Version: 0.2.8
+Version: 0.2.9
 Summary: turn apple health export.xml into parquet
 Author: Thomas Schranz
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/atlaslib/atlas
 Project-URL: Changelog, https://github.com/atlaslib/atlas/releases
 Project-URL: Issues, https://github.com/atlaslib/atlas/issues
 Project-URL: CI, https://github.com/atlaslib/atlas/actions
@@ -18,33 +18,33 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 
 <div align="center">
   <img alt="Atlas"
        height="320px"
-       src="https://github.com/tosh/expanse/assets/14825/0f766786-31c9-434e-ae65-66cf7331a27b">
+       src="https://github.com/atlaslib/atlas/assets/14825/0f766786-31c9-434e-ae65-66cf7331a27b">
 </div>
 
 # Atlas
 
 Atlas lets you explore your Apple Health data.
 
 ---
 
-[![PyPI](https://img.shields.io/pypi/v/expanse.svg)](https://pypi.org/project/expanse/)
-[![Tests](https://github.com/tosh/expanse/actions/workflows/test.yml/badge.svg)](https://github.com/tosh/expanse/actions/workflows/test.yml)
-[![Changelog](https://img.shields.io/github/v/release/tosh/expanse?include_prereleases&label=changelog)](https://github.com/tosh/expanse/releases)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tosh/expanse/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/atlas-db.svg)](https://pypi.org/project/atlas-db/)
+[![Tests](https://github.com/atlaslib/atlas/actions/workflows/test.yml/badge.svg)](https://github.com/atlaslib/atlas/actions/workflows/test.yml)
+[![Changelog](https://img.shields.io/github/v/release/atlaslib/atlas?include_prereleases&label=changelog)](https://github.com/atlaslib/atlas/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/atlaslib/atlas/blob/main/LICENSE)
 
 ## Installation
 
 Install expanse using `pip`:
 ```bash
-pip install atlaslib
+pip install atlas-db
 ```
 
 ## Explore
 
 First we create the `.parquet` file from the `export.xml` file.
 
 ```bash
```

### Comparing `atlas_db-0.2.8/README.md` & `atlas_db-0.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 
 <div align="center">
   <img alt="Atlas"
        height="320px"
-       src="https://github.com/tosh/expanse/assets/14825/0f766786-31c9-434e-ae65-66cf7331a27b">
+       src="https://github.com/atlaslib/atlas/assets/14825/0f766786-31c9-434e-ae65-66cf7331a27b">
 </div>
 
 # Atlas
 
 Atlas lets you explore your Apple Health data.
 
 ---
 
-[![PyPI](https://img.shields.io/pypi/v/expanse.svg)](https://pypi.org/project/expanse/)
-[![Tests](https://github.com/tosh/expanse/actions/workflows/test.yml/badge.svg)](https://github.com/tosh/expanse/actions/workflows/test.yml)
-[![Changelog](https://img.shields.io/github/v/release/tosh/expanse?include_prereleases&label=changelog)](https://github.com/tosh/expanse/releases)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tosh/expanse/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/atlas-db.svg)](https://pypi.org/project/atlas-db/)
+[![Tests](https://github.com/atlaslib/atlas/actions/workflows/test.yml/badge.svg)](https://github.com/atlaslib/atlas/actions/workflows/test.yml)
+[![Changelog](https://img.shields.io/github/v/release/atlaslib/atlas?include_prereleases&label=changelog)](https://github.com/atlaslib/atlas/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/atlaslib/atlas/blob/main/LICENSE)
 
 ## Installation
 
 Install expanse using `pip`:
 ```bash
-pip install atlaslib
+pip install atlas-db
 ```
 
 ## Explore
 
 First we create the `.parquet` file from the `export.xml` file.
 
 ```bash
```

### Comparing `atlas_db-0.2.8/atlas/apple_health.py` & `atlas_db-0.2.9/atlas/apple_health.py`

 * *Files identical despite different names*

### Comparing `atlas_db-0.2.8/atlas/cli.py` & `atlas_db-0.2.9/atlas/cli.py`

 * *Files identical despite different names*

### Comparing `atlas_db-0.2.8/atlas_db.egg-info/PKG-INFO` & `atlas_db-0.2.9/atlas_db.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-db
-Version: 0.2.8
+Version: 0.2.9
 Summary: turn apple health export.xml into parquet
 Author: Thomas Schranz
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/atlaslib/atlas
 Project-URL: Changelog, https://github.com/atlaslib/atlas/releases
 Project-URL: Issues, https://github.com/atlaslib/atlas/issues
 Project-URL: CI, https://github.com/atlaslib/atlas/actions
@@ -18,33 +18,33 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 
 <div align="center">
   <img alt="Atlas"
        height="320px"
-       src="https://github.com/tosh/expanse/assets/14825/0f766786-31c9-434e-ae65-66cf7331a27b">
+       src="https://github.com/atlaslib/atlas/assets/14825/0f766786-31c9-434e-ae65-66cf7331a27b">
 </div>
 
 # Atlas
 
 Atlas lets you explore your Apple Health data.
 
 ---
 
-[![PyPI](https://img.shields.io/pypi/v/expanse.svg)](https://pypi.org/project/expanse/)
-[![Tests](https://github.com/tosh/expanse/actions/workflows/test.yml/badge.svg)](https://github.com/tosh/expanse/actions/workflows/test.yml)
-[![Changelog](https://img.shields.io/github/v/release/tosh/expanse?include_prereleases&label=changelog)](https://github.com/tosh/expanse/releases)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/tosh/expanse/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/atlas-db.svg)](https://pypi.org/project/atlas-db/)
+[![Tests](https://github.com/atlaslib/atlas/actions/workflows/test.yml/badge.svg)](https://github.com/atlaslib/atlas/actions/workflows/test.yml)
+[![Changelog](https://img.shields.io/github/v/release/atlaslib/atlas?include_prereleases&label=changelog)](https://github.com/atlaslib/atlas/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/atlaslib/atlas/blob/main/LICENSE)
 
 ## Installation
 
 Install expanse using `pip`:
 ```bash
-pip install atlaslib
+pip install atlas-db
 ```
 
 ## Explore
 
 First we create the `.parquet` file from the `export.xml` file.
 
 ```bash
```

### Comparing `atlas_db-0.2.8/pyproject.toml` & `atlas_db-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atlas-db"
-version = "0.2.8"
+version = "0.2.9"
 description = "turn apple health export.xml into parquet"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Thomas Schranz"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

