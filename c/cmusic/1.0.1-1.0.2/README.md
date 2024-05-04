# Comparing `tmp/cmusic-1.0.1.tar.gz` & `tmp/cmusic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmusic-1.0.1.tar", max compression
+gzip compressed data, was "cmusic-1.0.2.tar", max compression
```

## Comparing `cmusic-1.0.1.tar` & `cmusic-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      846 2024-04-24 15:27:09.715496 cmusic-1.0.1/LICENSE
--rw-r--r--   0        0        0     3764 2024-05-04 01:50:08.697910 cmusic-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-27 23:05:32.082513 cmusic-1.0.1/cmusic/__init__.py
--rw-r--r--   0        0        0     3940 2024-05-04 01:16:26.452353 cmusic-1.0.1/cmusic/bg_threads.py
--rwxr-xr-x   0        0        0     5726 2024-05-04 02:03:26.436978 cmusic-1.0.1/cmusic/cmusic.py
--rw-r--r--   0        0        0     1129 2024-05-04 01:16:26.411822 cmusic-1.0.1/cmusic/constants.py
--rw-r--r--   0        0        0    19509 2024-05-04 01:16:26.702616 cmusic-1.0.1/cmusic/indexlib.py
--rw-r--r--   0        0        0    24199 2024-05-04 01:16:26.718203 cmusic-1.0.1/cmusic/main.py
--rw-r--r--   0        0        0      418 2024-05-04 02:03:37.686886 cmusic-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 cmusic-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      846 2024-04-24 15:27:09.715496 cmusic-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3764 2024-05-04 01:50:08.697910 cmusic-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 23:05:32.082513 cmusic-1.0.2/cmusic/__init__.py
+-rw-r--r--   0        0        0     3940 2024-05-04 01:16:26.452353 cmusic-1.0.2/cmusic/bg_threads.py
+-rwxr-xr-x   0        0        0     5726 2024-05-04 02:03:26.436978 cmusic-1.0.2/cmusic/cmusic.py
+-rw-r--r--   0        0        0     1170 2024-05-04 02:05:42.073462 cmusic-1.0.2/cmusic/constants.py
+-rw-r--r--   0        0        0    19509 2024-05-04 01:16:26.702616 cmusic-1.0.2/cmusic/indexlib.py
+-rw-r--r--   0        0        0    24199 2024-05-04 01:16:26.718203 cmusic-1.0.2/cmusic/main.py
+-rw-r--r--   0        0        0      418 2024-05-04 02:04:31.818825 cmusic-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 cmusic-1.0.2/PKG-INFO
```

### Comparing `cmusic-1.0.1/LICENSE` & `cmusic-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.1/README.md` & `cmusic-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.1/cmusic/bg_threads.py` & `cmusic-1.0.2/cmusic/bg_threads.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.1/cmusic/cmusic.py` & `cmusic-1.0.2/cmusic/cmusic.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.1/cmusic/constants.py` & `cmusic-1.0.2/cmusic/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # the path to the config file
 
 CMUSIC_DIR = os.path.join(os.path.expanduser("~"), ".cmusic")
 
 CONFIG_FILE = os.path.join(CMUSIC_DIR, "config.json")
 
 LOG_FILE = os.path.join(CMUSIC_DIR, "cmusic.log")
-MAIN = objlog.LogNode("CMUSIC", log_file=LOG_FILE)
+MAIN = objlog.LogNode("CMUSIC")
 
 DEFAULT_CONFIG = {
     "library": os.path.join(os.path.expanduser("~"), "cMusic Library"),
     "volume": 100,
 }
 
 # check if the cmusic directory exists
@@ -36,7 +36,9 @@
     MAIN.log(Info("Created crashes directory"))
 
 config = json.load(open(CONFIG_FILE))
 LIBRARY = config["library"]
 CRASH_FOLDER = os.path.join(CMUSIC_DIR, "crashes")
 
 MAIN.log(Info("Constants OK"))
+
+MAIN.set_output_file(LOG_FILE, preserve_old_messages=True)
```

### Comparing `cmusic-1.0.1/cmusic/indexlib.py` & `cmusic-1.0.2/cmusic/indexlib.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.1/cmusic/main.py` & `cmusic-1.0.2/cmusic/main.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.1/PKG-INFO` & `cmusic-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmusic
-Version: 1.0.1
+Version: 1.0.2
 Summary: the CLI music player
 Author: Kokonico
 Author-email: kokonico@duck.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: inquirer (>=3.2.4,<4.0.0)
```

