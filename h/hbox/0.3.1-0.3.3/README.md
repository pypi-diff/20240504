# Comparing `tmp/hbox-0.3.1.tar.gz` & `tmp/hbox-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbox-0.3.1.tar", max compression
+gzip compressed data, was "hbox-0.3.3.tar", max compression
```

## Comparing `hbox-0.3.1.tar` & `hbox-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-04 01:55:48.469025 hbox-0.3.1/LICENSE
--rw-r--r--   0        0        0     6344 2024-05-04 01:55:48.469025 hbox-0.3.1/README.md
--rw-r--r--   0        0        0     6635 2024-05-04 01:55:48.469025 hbox-0.3.1/hbox/commands.py
--rw-r--r--   0        0        0     2212 2024-05-04 01:55:48.469025 hbox-0.3.1/hbox/config.py
--rw-r--r--   0        0        0      684 2024-05-04 01:55:48.469025 hbox-0.3.1/hbox/logger.py
--rw-r--r--   0        0        0     3094 2024-05-04 01:55:48.469025 hbox-0.3.1/hbox/main.py
--rw-r--r--   0        0        0     2292 2024-05-04 01:55:48.469025 hbox-0.3.1/hbox/utils.py
--rw-r--r--   0        0        0     1944 2024-05-04 01:55:48.469025 hbox-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-04 02:06:17.694286 hbox-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6344 2024-05-04 02:06:17.694286 hbox-0.3.3/README.md
+-rw-r--r--   0        0        0     6635 2024-05-04 02:06:17.694286 hbox-0.3.3/hbox/commands.py
+-rw-r--r--   0        0        0     2212 2024-05-04 02:06:17.694286 hbox-0.3.3/hbox/config.py
+-rw-r--r--   0        0        0      684 2024-05-04 02:06:17.694286 hbox-0.3.3/hbox/logger.py
+-rw-r--r--   0        0        0     3094 2024-05-04 02:06:17.694286 hbox-0.3.3/hbox/main.py
+-rw-r--r--   0        0        0     2292 2024-05-04 02:06:17.694286 hbox-0.3.3/hbox/utils.py
+-rw-r--r--   0        0        0     1944 2024-05-04 02:06:17.694286 hbox-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.3.3/PKG-INFO
```

### Comparing `hbox-0.3.1/LICENSE` & `hbox-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/README.md` & `hbox-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/hbox/commands.py` & `hbox-0.3.3/hbox/commands.py`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/hbox/config.py` & `hbox-0.3.3/hbox/config.py`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/hbox/logger.py` & `hbox-0.3.3/hbox/logger.py`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/hbox/main.py` & `hbox-0.3.3/hbox/main.py`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/hbox/utils.py` & `hbox-0.3.3/hbox/utils.py`

 * *Files identical despite different names*

### Comparing `hbox-0.3.1/pyproject.toml` & `hbox-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hbox"
-version = "0.3.1"
+version = "0.3.3"
 description = "CLI tool that leverages container technology to manage packages."
 authors = ["Helton Carlos de Souza <heltoncarlossouza@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `hbox-0.3.1/PKG-INFO` & `hbox-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbox
-Version: 0.3.1
+Version: 0.3.3
 Summary: CLI tool that leverages container technology to manage packages.
 License: MIT
 Author: Helton Carlos de Souza
 Author-email: heltoncarlossouza@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
