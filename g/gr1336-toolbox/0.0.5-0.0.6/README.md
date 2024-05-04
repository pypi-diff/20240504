# Comparing `tmp/gr1336_toolbox-0.0.5.tar.gz` & `tmp/gr1336_toolbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr1336_toolbox-0.0.5.tar", last modified: Sat May  4 01:49:12 2024, max compression
+gzip compressed data, was "gr1336_toolbox-0.0.6.tar", last modified: Sat May  4 02:16:06 2024, max compression
```

## Comparing `gr1336_toolbox-0.0.5.tar` & `gr1336_toolbox-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:49:12.505492 gr1336_toolbox-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 01:49:12.505492 gr1336_toolbox-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:49:12.501492 gr1336_toolbox-0.0.5/gr1336_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/gr1336_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/gr1336_toolbox/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/gr1336_toolbox/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/gr1336_toolbox/test_even_odd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/gr1336_toolbox/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/gr1336_toolbox/types_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:49:12.505492 gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 01:49:12.000000 gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 01:49:12.000000 gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:49:12.000000 gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 01:49:12.000000 gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 01:49:12.000000 gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:49:12.505492 gr1336_toolbox-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-04 01:49:08.000000 gr1336_toolbox-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/gr1336_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/misc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/test_even_odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/gr1336_toolbox/types_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 02:16:06.000000 gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 02:16:06.298386 gr1336_toolbox-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-04 02:15:58.000000 gr1336_toolbox-0.0.6/setup.py
```

### Comparing `gr1336_toolbox-0.0.5/LICENSE` & `gr1336_toolbox-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.5/PKG-INFO` & `gr1336_toolbox-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox/__init__.py` & `gr1336_toolbox-0.0.6/gr1336_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox/file_manager.py` & `gr1336_toolbox-0.0.6/gr1336_toolbox/file_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,31 +12,23 @@
 def get_dirs(path: str | Path) -> list[Path]:
     if not _path(path):
         return []
     return [x for x in Path(path).glob("*") if x.is_dir()]
 
 
 def get_files(
-    path: str | Path, extensions: str | list[str] | tuple[str, ...] | None = None
+    path: str | Path, extensions: str | None = None
 ) -> list[Path]:
 
     if not _path(path):
         return []
     if not extensions:
         return [x for x in Path(path).glob("*") if x.is_file()]
     if _str(path):
         return [x for x in Path(path).glob(f"*.{extensions}") if x.is_file()]
-    elif _array(extensions):
-        results = []
-        for y in extensions:
-            if y[0] == ".":
-                y = y[1:]
-            _t = [x for x in Path(path).glob(f"*.{y}") if x.is_file()]
-            results.extend(_t)
-        return results
     return []
 
 
 def create_path(path: str | Path):
     Path(path).parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox/misc_tools.py` & `gr1336_toolbox-0.0.6/gr1336_toolbox/misc_tools.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox/test_even_odd.py` & `gr1336_toolbox-0.0.6/gr1336_toolbox/test_even_odd.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox/text_tools.py` & `gr1336_toolbox-0.0.6/gr1336_toolbox/text_tools.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox/types_check.py` & `gr1336_toolbox-0.0.6/gr1336_toolbox/types_check.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.5/gr1336_toolbox.egg-info/PKG-INFO` & `gr1336_toolbox-0.0.6/gr1336_toolbox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.5/setup.py` & `gr1336_toolbox-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    version="0.0.5",
+    version="0.0.6",
     name="gr1336_toolbox",
     description="Personal collection of reusable tools in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gr1336/gr1336_toolbox/",
     install_requires=["numpy", "pyperclip", "textblob", "pyyaml", "pyarrow"],
     author="gr1336",
```

