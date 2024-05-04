# Comparing `tmp/npc_lims-0.1.98.tar.gz` & `tmp/npc_lims-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_lims-0.1.98.tar", last modified: Wed Jan 10 19:27:22 2024, max compression
+gzip compressed data, was "npc_lims-0.1.99.tar", last modified: Thu Jan 11 21:27:32 2024, max compression
```

## Comparing `npc_lims-0.1.98.tar` & `npc_lims-0.1.99.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.374812 npc_lims-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-10 19:24:25.000000 npc_lims-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-01-10 19:27:22.374812 npc_lims-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-01-10 19:24:25.000000 npc_lims-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-01-10 19:27:19.000000 npc_lims-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 19:27:22.374812 npc_lims-0.1.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.366811 npc_lims-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.370812 npc_lims-0.1.98/src/npc_lims/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.370812 npc_lims-0.1.98/src/npc_lims/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.370812 npc_lims-0.1.98/src/npc_lims/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17343 2024-01-10 19:27:15.000000 npc_lims-0.1.98/src/npc_lims/metadata/codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/metadata/nwb.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/metadata/spreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/metadata/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.370812 npc_lims-0.1.98/src/npc_lims/paths/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/paths/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/paths/codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)    15757 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/paths/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.374812 npc_lims-0.1.98/src/npc_lims/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/scripts/regenerate_all_nwbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-10 19:27:15.000000 npc_lims-0.1.98/src/npc_lims/scripts/run_video_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/scripts/update_session_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.374812 npc_lims-0.1.98/src/npc_lims/status/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/status/behavior_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16050 2024-01-10 19:24:25.000000 npc_lims-0.1.98/src/npc_lims/status/tracked_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.374812 npc_lims-0.1.98/src/npc_lims.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-01-10 19:27:22.000000 npc_lims-0.1.98/src/npc_lims.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-10 19:27:22.000000 npc_lims-0.1.98/src/npc_lims.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 19:27:22.000000 npc_lims-0.1.98/src/npc_lims.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-10 19:27:22.000000 npc_lims-0.1.98/src/npc_lims.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-10 19:27:22.000000 npc_lims-0.1.98/src/npc_lims.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-10 19:27:22.000000 npc_lims-0.1.98/src/npc_lims.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:27:22.374812 npc_lims-0.1.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-10 19:24:25.000000 npc_lims-0.1.98/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-01-11 21:24:32.000000 npc_lims-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-01-11 21:27:32.744356 npc_lims-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-01-11 21:24:32.000000 npc_lims-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-01-11 21:27:29.000000 npc_lims-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 21:27:32.744356 npc_lims-0.1.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.740355 npc_lims-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.740355 npc_lims-0.1.99/src/npc_lims/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.740355 npc_lims-0.1.99/src/npc_lims/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/src/npc_lims/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17343 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/metadata/codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/metadata/nwb.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/metadata/spreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/metadata/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/src/npc_lims/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-01-11 21:27:25.000000 npc_lims-0.1.99/src/npc_lims/paths/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/paths/codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15757 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/paths/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/src/npc_lims/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/scripts/regenerate_all_nwbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/scripts/run_video_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/scripts/update_session_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/src/npc_lims/status/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/status/behavior_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16050 2024-01-11 21:24:32.000000 npc_lims-0.1.99/src/npc_lims/status/tracked_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/src/npc_lims.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-01-11 21:27:32.000000 npc_lims-0.1.99/src/npc_lims.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-01-11 21:27:32.000000 npc_lims-0.1.99/src/npc_lims.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 21:27:32.000000 npc_lims-0.1.99/src/npc_lims.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-11 21:27:32.000000 npc_lims-0.1.99/src/npc_lims.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-11 21:27:32.000000 npc_lims-0.1.99/src/npc_lims.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-11 21:27:32.000000 npc_lims-0.1.99/src/npc_lims.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:27:32.744356 npc_lims-0.1.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-11 21:24:32.000000 npc_lims-0.1.99/tests/test_core.py
```

### Comparing `npc_lims-0.1.98/LICENSE` & `npc_lims-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/PKG-INFO` & `npc_lims-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc_lims
-Version: 0.1.98
+Version: 0.1.99
 Summary: Tools to fetch and update paths, metadata and state for Mindscope Neuropixels sessions, in the cloud.
 Author-email: Arjun Sridhar <arjun.sridhar@alleninstitute.org>, Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_lims
 Project-URL: Issues, https://github.com/AllenInstitute/npc_lims/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -24,14 +24,15 @@
 Requires-Dist: s3fs>=2023.6.0
 Requires-Dist: pydbhub-bjh>=0.0.8
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: pyopenssl>=23.2.0
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: packaging>=23.2
+Requires-Dist: boto3==1.28.17
 
 # npc_lims
 
 **n**euro**p**ixels **c**loud **l**ab **i**nformation **m**anagement **s**ystem
 Tools to fetch and update paths, metadata and state for Mindscope Neuropixels sessions, in the cloud.
 
 [![PyPI](https://img.shields.io/pypi/v/npc-lims.svg?label=PyPI&color=blue)](https://pypi.org/project/npc-lims/)
```

### Comparing `npc_lims-0.1.98/README.md` & `npc_lims-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/pyproject.toml` & `npc_lims-0.1.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "npc_lims"
-version = "0.1.98"
+version = "0.1.99"
 description = "Tools to fetch and update paths, metadata and state for Mindscope Neuropixels sessions, in the cloud."
 authors = [
     { name = "Arjun Sridhar", email = "arjun.sridhar@alleninstitute.org" },
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "typing-extensions>=4.7.1",
@@ -15,14 +15,15 @@
     "s3fs>=2023.6.0",
     "pydbhub-bjh>=0.0.8",
     "pyyaml>=6.0.1",
     "python-dotenv>=1.0.0",
     "pyopenssl>=23.2.0",
     "openpyxl>=3.1.2",
     "packaging>=23.2",
+    "boto3==1.28.17",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -54,14 +55,15 @@
     "ruff>=0.0.282",
     "mypy>=1.4.1",
     "pytest-cov>=4.1.0",
     "black>=23.7.0",
     "parver>=0.3",
     "git-changelog>=2.3",
     "types-PyYAML>=6.0.12.12",
+    "types-requests>=2.31.0.6",
 ]
 docs = [
     "markdown-callouts>=0.3",
     "markdown-exec>=1.7",
     "mkdocs>=1.5",
     "mkdocs-coverage>=1.0",
     "mkdocs-gen-files>=0.5",
```

### Comparing `npc_lims-0.1.98/src/npc_lims/metadata/codeocean.py` & `npc_lims-0.1.99/src/npc_lims/metadata/codeocean.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/metadata/nwb.sql` & `npc_lims-0.1.99/src/npc_lims/metadata/nwb.sql`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/metadata/spreadsheets.py` & `npc_lims-0.1.99/src/npc_lims/metadata/spreadsheets.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/metadata/types.py` & `npc_lims-0.1.99/src/npc_lims/metadata/types.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/paths/cache.py` & `npc_lims-0.1.99/src/npc_lims/paths/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import typing
 from typing import Literal
 
 import npc_session
 import packaging.version
+import requests
 import upath
 from typing_extensions import TypeAlias
 
 from npc_lims.paths.s3 import S3_SCRATCH_ROOT
 
 CACHE_ROOT = S3_SCRATCH_ROOT / "session-caches"
 
@@ -51,22 +52,25 @@
         raise ValueError(
             f"Unknown NWB component {nwb_component!r} - must be one of {NWBComponentStr}"
         )
     return ext
 
 
 def get_current_cache_version() -> str:
-    """
+    """The current version of npc_sessions, formatted as a string starting with
+    'v'.
+
     >>> (get_cache_path(nwb_component="units", session_id="366122_2023-12-31", version="v0.0.0").parent / 'test.txt').touch()
     >>> v = get_current_cache_version()
     >>> assert v >= 'v0.0.0'
     """
     if not (version_dirs := sorted(CACHE_ROOT.glob("v*"))):
         raise FileNotFoundError(f"No cache versions found in {CACHE_ROOT}")
-    return version_dirs[-1].name
+    npc_sessions_info = requests.get("https://pypi.org/pypi/npc_sessions/json").json()
+    return _parse_version(npc_sessions_info["info"]["version"])
 
 
 def _parse_version(version: str) -> str:
     """
     >>> _parse_version("0.0.0")
     'v0.0.0'
     >>> _parse_version("v0.0.0")
```

### Comparing `npc_lims-0.1.98/src/npc_lims/paths/codeocean.py` & `npc_lims-0.1.99/src/npc_lims/paths/codeocean.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/paths/s3.py` & `npc_lims-0.1.99/src/npc_lims/paths/s3.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/scripts/regenerate_all_nwbs.py` & `npc_lims-0.1.99/src/npc_lims/scripts/regenerate_all_nwbs.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/scripts/update_session_status.py` & `npc_lims-0.1.99/src/npc_lims/scripts/update_session_status.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/status/behavior_sessions.py` & `npc_lims-0.1.99/src/npc_lims/status/behavior_sessions.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims/status/tracked_sessions.py` & `npc_lims-0.1.99/src/npc_lims/status/tracked_sessions.py`

 * *Files identical despite different names*

### Comparing `npc_lims-0.1.98/src/npc_lims.egg-info/PKG-INFO` & `npc_lims-0.1.99/src/npc_lims.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc_lims
-Version: 0.1.98
+Version: 0.1.99
 Summary: Tools to fetch and update paths, metadata and state for Mindscope Neuropixels sessions, in the cloud.
 Author-email: Arjun Sridhar <arjun.sridhar@alleninstitute.org>, Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_lims
 Project-URL: Issues, https://github.com/AllenInstitute/npc_lims/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -24,14 +24,15 @@
 Requires-Dist: s3fs>=2023.6.0
 Requires-Dist: pydbhub-bjh>=0.0.8
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: pyopenssl>=23.2.0
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: packaging>=23.2
+Requires-Dist: boto3==1.28.17
 
 # npc_lims
 
 **n**euro**p**ixels **c**loud **l**ab **i**nformation **m**anagement **s**ystem
 Tools to fetch and update paths, metadata and state for Mindscope Neuropixels sessions, in the cloud.
 
 [![PyPI](https://img.shields.io/pypi/v/npc-lims.svg?label=PyPI&color=blue)](https://pypi.org/project/npc-lims/)
```

### Comparing `npc_lims-0.1.98/src/npc_lims.egg-info/SOURCES.txt` & `npc_lims-0.1.99/src/npc_lims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

