# Comparing `tmp/gr1336_toolbox-0.0.3.tar.gz` & `tmp/gr1336_toolbox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr1336_toolbox-0.0.3.tar", last modified: Fri May  3 03:03:42 2024, max compression
+gzip compressed data, was "gr1336_toolbox-0.0.4.tar", last modified: Fri May  3 22:01:37 2024, max compression
```

## Comparing `gr1336_toolbox-0.0.3.tar` & `gr1336_toolbox-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/gr1336_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/test_even_odd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/gr1336_toolbox/types_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 03:03:42.000000 gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:03:42.137633 gr1336_toolbox-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 03:03:37.000000 gr1336_toolbox-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:01:37.692766 gr1336_toolbox-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 22:01:37.692766 gr1336_toolbox-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:01:37.692766 gr1336_toolbox-0.0.4/gr1336_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/gr1336_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/gr1336_toolbox/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/gr1336_toolbox/misc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/gr1336_toolbox/test_even_odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/gr1336_toolbox/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/gr1336_toolbox/types_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:01:37.692766 gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 22:01:37.000000 gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 22:01:37.000000 gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:01:37.000000 gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 22:01:37.000000 gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 22:01:37.000000 gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:01:37.692766 gr1336_toolbox-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 22:01:33.000000 gr1336_toolbox-0.0.4/setup.py
```

### Comparing `gr1336_toolbox-0.0.3/LICENSE` & `gr1336_toolbox-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.3/PKG-INFO` & `gr1336_toolbox-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.3
+Version: 0.0.4
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.3/gr1336_toolbox/file_manager.py` & `gr1336_toolbox-0.0.4/gr1336_toolbox/file_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import yaml
+import shutil
 import pandas as pd
 import pyarrow as pa
 from typing import Any
 from pathlib import Path
 import pyarrow.parquet as pq
 from .types_check import _path
 
@@ -17,15 +19,15 @@
     if not _path(path):
         return []
     if not extension:
         return [x for x in Path(path).glob("*") if x.is_file()]
     return [x for x in Path(path).glob(f"*.{extension}") if x.is_file()]
 
 
-def _create(path: str | Path):
+def create_path(path: str | Path):
     Path(path).parent.mkdir(parents=True, exist_ok=True)
 
 
 def _load_parquet(content: Any):
     if not isinstance(content, dict):
         return content
     return {key: list(value) for key, value in content.items()}
@@ -35,15 +37,15 @@
     """Load a Parquet file."""
     table = pq.read_table(path).to_pandas().to_dict(orient="records")
     return [_load_parquet(x) for x in table]
 
 
 def save_parquet(path: str, data: list | dict) -> None:
     """Save a list to a Parquet file."""
-    _create(path)
+    create_path(path)
     table = pa.Table.from_pandas(pd.DataFrame(data))
     pq.write_table(table, path)
 
 
 def load_text(
     path: Path | str,
     encoding: str = "utf-8",
@@ -53,15 +55,15 @@
         return ""
     with open(path, "r", encoding=encoding) as file:
         return file.read()
 
 
 def save_text(path: Path | str, content: str, encoding: str = "utf-8") -> None:
     """Save a text file to the provided path."""
-    _create(path)
+    create_path(path)
     with open(path, "w", encoding=encoding) as file:
         file.write(content)
 
 
 def load_yaml(
     path: Path | str,
     encoding: str = "utf-8",
@@ -79,13 +81,21 @@
 def save_yaml(
     path: Path | str,
     content: list | tuple | dict,
     encoding: str = "utf-8",
     safe_dump: bool = False,
 ) -> None:
     """Save a YAML file to the provided path."""
-    _create(path)
+    create_path(path)
     with open(path, "w", encoding=encoding) as file:
         if safe_dump:
             yaml.safe_dump(content, file, encoding=encoding)
         else:
             yaml.dump(content, file, encoding=encoding)
+
+def move_to(source_path: str | Path, destination_path: str | Path):
+    assert (
+        str(source_path).strip() and Path(source_path).exists()
+    ), "Source path does not exists!"
+
+    os.makedirs(str(destination_path), exist_ok=True)
+    shutil.move(source_path, destination_path)
```

### Comparing `gr1336_toolbox-0.0.3/gr1336_toolbox/test_even_odd.py` & `gr1336_toolbox-0.0.4/gr1336_toolbox/test_even_odd.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.3/gr1336_toolbox/text_tools.py` & `gr1336_toolbox-0.0.4/gr1336_toolbox/text_tools.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.3/gr1336_toolbox.egg-info/PKG-INFO` & `gr1336_toolbox-0.0.4/gr1336_toolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.3
+Version: 0.0.4
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.3/setup.py` & `gr1336_toolbox-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    version="0.0.3",
+    version="0.0.4",
     name="gr1336_toolbox",
     description="Personal collection of reusable tools in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gr1336/gr1336_toolbox/",
     install_requires=["numpy", "pyperclip", "textblob", "pyyaml", "pyarrow"],
     author="gr1336",
```

