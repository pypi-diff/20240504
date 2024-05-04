# Comparing `tmp/torahcodes-1.0.8.tar.gz` & `tmp/torahcodes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jan 23 18:03:25 2023, from Unix
+gzip compressed data, last modified: Mon Jan 23 18:07:22 2023, from Unix
```

## Comparing `torahcodes-1.0.8.tar` & `torahcodes-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
 drwxr-xr-x   0 citrix    (1000) citrix    (1000)        0 2023-01-18 02:22:12.000000 torahcodes-1.0.8/
--rw-r--r--   0 citrix    (1000) citrix    (1000)     7002 2023-01-23 18:03:10.000000 torahcodes-1.0.8/PKG-INFO
+-rw-r--r--   0 citrix    (1000) citrix    (1000)     7002 2023-01-23 18:06:46.000000 torahcodes-1.0.8/PKG-INFO
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     6211 2023-01-18 01:42:28.000000 torahcodes-1.0.8/README.md
 -rw-r--r--   0 citrix    (1000) citrix    (1000)       38 2023-01-18 02:22:12.000000 torahcodes-1.0.8/setup.cfg
--rw-r--r--   0 citrix    (1000) citrix    (1000)     1627 2023-01-23 18:03:23.000000 torahcodes-1.0.8/setup.py
+-rw-r--r--   0 citrix    (1000) citrix    (1000)     1627 2023-01-23 18:07:04.000000 torahcodes-1.0.8/setup.py
 drwxr-xr-x   0 citrix    (1000) citrix    (1000)        0 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes/
 -rw-r--r--   0 citrix    (1000) citrix    (1000)   712520 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/D.py
--rwxr-xr-x   0 citrix    (1000) citrix    (1000)    12781 2023-01-18 02:05:44.000000 torahcodes-1.0.8/torahcodes/TBC.py
+-rwxr-xr-x   0 citrix    (1000) citrix    (1000)    12857 2023-01-23 18:06:24.000000 torahcodes-1.0.8/torahcodes/TBC.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)        0 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/__init__.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)    13495 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/baphomet.py
 drwxr-xr-x   0 citrix    (1000) citrix    (1000)        0 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes/modules/
 -rwxr-xr-x   0 citrix    (1000) citrix    (1000)      229 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/modules/__init__.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     5732 2023-01-18 02:06:14.000000 torahcodes-1.0.8/torahcodes/modules/conversions.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     3050 2023-01-18 02:06:04.000000 torahcodes-1.0.8/torahcodes/modules/query.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     3379 2023-01-18 02:18:59.000000 torahcodes-1.0.8/torahcodes/modules/shemhemaphoresh.py
@@ -31,15 +31,15 @@
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     3681 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/resources/func/mod_8DataObjectsCreate.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)      773 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/resources/func/mod_99WriteOutputToCSVFile_WordsAndGematriaValues.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     5318 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/resources/func/mod_9GetNumberValues.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     1005 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/resources/func/thread.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     5108 2023-01-18 02:07:06.000000 torahcodes-1.0.8/torahcodes/resources/func/torah.py
 -rw-r--r--   0 citrix    (1000) citrix    (1000)    11667 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/resources/func/utils.py
 drwxr-xr-x   0 citrix    (1000) citrix    (1000)        0 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes.egg-info/
--rw-r--r--   0 citrix    (1000) citrix    (1000)     7002 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes.egg-info/PKG-INFO
+-rw-r--r--   0 citrix    (1000) citrix    (1000)     7002 2023-01-23 18:07:18.000000 torahcodes-1.0.8/torahcodes.egg-info/PKG-INFO
 -rw-r--r--   0 citrix    (1000) citrix    (1000)     1369 2023-01-23 17:37:48.000000 torahcodes-1.0.8/torahcodes.egg-info/SOURCES.txt
 -rw-r--r--   0 citrix    (1000) citrix    (1000)        1 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes.egg-info/dependency_links.txt
 -rw-r--r--   0 citrix    (1000) citrix    (1000)       48 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes.egg-info/entry_points.txt
 -rw-r--r--   0 citrix    (1000) citrix    (1000)       65 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes.egg-info/requires.txt
 -rw-r--r--   0 citrix    (1000) citrix    (1000)       82 2023-01-18 02:22:12.000000 torahcodes-1.0.8/torahcodes.egg-info/top_level.txt
 -rw-r--r--   0 citrix    (1000) citrix    (1000)   221721 2023-01-17 23:58:46.000000 torahcodes-1.0.8/torahcodes/resources/data/text_13jeremiah.json
 drwxr-xr-x   0 citrix    (1000) citrix    (1000)        0 2023-01-18 02:19:13.000000 torahcodes-1.0.8/torahcodes/modules/__pycache__/
```

### torahcodes-1.0.8/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torahcodes
-Version: 1.0.8
+Version: 1.0.9
 Summary: An understandable multilanguaje and multithreading bible codes . Study the Torah as never before Bible Codes python library . An understandable multilanguaje and multithreading bible codes . Study the Torah as never before
 Home-page: 
 Author: torahcodes
 Author-email: 
 Project-URL: Source, https://github.com/pedroelbanquero/torahcodespython
 Keywords: torahcodes
 Classifier: Development Status :: 5 - Production/Stable
```

### torahcodes-1.0.8/setup.py

```diff
@@ -8,15 +8,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='torahcodes',
-    version='1.0.8',
+    version='1.0.9',
     author='torahcodes',
     include_package_data=True,
     author_email='',
     description='An understandable multilanguaje and multithreading bible codes . Study the Torah as never before Bible Codes python library . An understandable multilanguaje and multithreading bible codes . Study the Torah as never before',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
```

### torahcodes-1.0.8/torahcodes/TBC.py

```diff
@@ -11,15 +11,16 @@
 	import os
 	import traceback
 	import argparse
 	import pathlib
 	import time
 	import signal
 	import sys
-
+	import readline
+	readline.parse_and_bind('"\e[A": history-search-backward')
 	#import lib.nc as nc
 	# MODULE IMPORT
 	from torahcodes.modules import *
 	#from active_modules import *
 except KeyboardInterrupt:
 	print(GREEN + "\n[I] Shutting down..." + END)
 	raise SystemExit
```

### torahcodes-1.0.8/torahcodes.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torahcodes
-Version: 1.0.7
+Version: 1.0.9
 Summary: An understandable multilanguaje and multithreading bible codes . Study the Torah as never before Bible Codes python library . An understandable multilanguaje and multithreading bible codes . Study the Torah as never before
 Home-page: 
 Author: torahcodes
 Author-email: 
 Project-URL: Source, https://github.com/pedroelbanquero/torahcodespython
 Keywords: torahcodes
 Classifier: Development Status :: 5 - Production/Stable
```

