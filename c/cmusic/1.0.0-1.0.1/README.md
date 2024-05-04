# Comparing `tmp/cmusic-1.0.0.tar.gz` & `tmp/cmusic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmusic-1.0.0.tar", max compression
+gzip compressed data, was "cmusic-1.0.1.tar", max compression
```

## Comparing `cmusic-1.0.0.tar` & `cmusic-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      846 2024-04-24 15:27:09.715496 cmusic-1.0.0/LICENSE
--rw-r--r--   0        0        0     3701 2024-05-04 00:48:49.841802 cmusic-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-27 23:05:32.082513 cmusic-1.0.0/cmusic/__init__.py
--rw-r--r--   0        0        0     3940 2024-05-04 01:16:26.452353 cmusic-1.0.0/cmusic/bg_threads.py
--rwxr-xr-x   0        0        0     5708 2024-05-04 01:16:26.466198 cmusic-1.0.0/cmusic/cmusic.py
--rw-r--r--   0        0        0     1129 2024-05-04 01:16:26.411822 cmusic-1.0.0/cmusic/constants.py
--rw-r--r--   0        0        0    19509 2024-05-04 01:16:26.702616 cmusic-1.0.0/cmusic/indexlib.py
--rw-r--r--   0        0        0    24199 2024-05-04 01:16:26.718203 cmusic-1.0.0/cmusic/main.py
--rw-r--r--   0        0        0      418 2024-05-04 01:36:05.985763 cmusic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4201 1970-01-01 00:00:00.000000 cmusic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      846 2024-04-24 15:27:09.715496 cmusic-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3764 2024-05-04 01:50:08.697910 cmusic-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-27 23:05:32.082513 cmusic-1.0.1/cmusic/__init__.py
+-rw-r--r--   0        0        0     3940 2024-05-04 01:16:26.452353 cmusic-1.0.1/cmusic/bg_threads.py
+-rwxr-xr-x   0        0        0     5726 2024-05-04 02:03:26.436978 cmusic-1.0.1/cmusic/cmusic.py
+-rw-r--r--   0        0        0     1129 2024-05-04 01:16:26.411822 cmusic-1.0.1/cmusic/constants.py
+-rw-r--r--   0        0        0    19509 2024-05-04 01:16:26.702616 cmusic-1.0.1/cmusic/indexlib.py
+-rw-r--r--   0        0        0    24199 2024-05-04 01:16:26.718203 cmusic-1.0.1/cmusic/main.py
+-rw-r--r--   0        0        0      418 2024-05-04 02:03:37.686886 cmusic-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 cmusic-1.0.1/PKG-INFO
```

### Comparing `cmusic-1.0.0/LICENSE` & `cmusic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.0/README.md` & `cmusic-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 cmusic is available on PyPI, so you can install it using pip.
 
 ```sh
 pip install cmusic
 ```
 
+(please make sure that your python scripts directory is in your PATH)
+
 or you can install it from the source code.
 
 ```sh
 git clone
 cd cmusic
 pip install .
 ```
@@ -106,15 +108,15 @@
 
 ```sh
 git clone https://github.com/kokonico/cmusic
 cd cmusic
 poetry install
 ```
 
-to install the player so you can use it in the terminal, you can use the following command.
+to install the player to use it in the terminal, you can use the following command.
 
 ```sh
 poetry run pip install .
 ```
 
 ## License
```

### Comparing `cmusic-1.0.0/cmusic/bg_threads.py` & `cmusic-1.0.1/cmusic/bg_threads.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.0/cmusic/cmusic.py` & `cmusic-1.0.1/cmusic/cmusic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 """cmusic CLI script"""
 
 import os
 
 # prevent pygame support prompt (must do before importing anything from pygame)
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
 
+import constants
+
 from objlog.LogMessages import Debug, Info, Warn, Error, Fatal
 from . import main as central
 
 MAIN = central.MAIN
 try:
     import argparse
     import subprocess
```

### Comparing `cmusic-1.0.0/cmusic/constants.py` & `cmusic-1.0.1/cmusic/constants.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.0/cmusic/indexlib.py` & `cmusic-1.0.1/cmusic/indexlib.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.0/cmusic/main.py` & `cmusic-1.0.1/cmusic/main.py`

 * *Files identical despite different names*

### Comparing `cmusic-1.0.0/PKG-INFO` & `cmusic-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmusic
-Version: 1.0.0
+Version: 1.0.1
 Summary: the CLI music player
 Author: Kokonico
 Author-email: kokonico@duck.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: inquirer (>=3.2.4,<4.0.0)
@@ -28,14 +28,16 @@
 
 cmusic is available on PyPI, so you can install it using pip.
 
 ```sh
 pip install cmusic
 ```
 
+(please make sure that your python scripts directory is in your PATH)
+
 or you can install it from the source code.
 
 ```sh
 git clone
 cd cmusic
 pip install .
 ```
@@ -122,15 +124,15 @@
 
 ```sh
 git clone https://github.com/kokonico/cmusic
 cd cmusic
 poetry install
 ```
 
-to install the player so you can use it in the terminal, you can use the following command.
+to install the player to use it in the terminal, you can use the following command.
 
 ```sh
 poetry run pip install .
 ```
 
 ## License
```

