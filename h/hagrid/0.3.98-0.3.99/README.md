# Comparing `tmp/hagrid-0.3.98.tar.gz` & `tmp/hagrid-0.3.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.98.tar", last modified: Sat Dec 23 10:17:24 2023, max compression
+gzip compressed data, was "hagrid-0.3.99.tar", last modified: Sun Dec 24 10:20:14 2023, max compression
```

## Comparing `hagrid-0.3.98.tar` & `hagrid-0.3.99.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 10:17:24.598724 hagrid-0.3.98/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-23 10:17:24.598724 hagrid-0.3.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2023-12-23 10:15:29.000000 hagrid-0.3.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 10:17:24.598724 hagrid-0.3.98/hagrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)   143990 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    29773 2023-12-23 10:16:29.000000 hagrid-0.3.98/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    12057 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14037 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-23 10:15:49.000000 hagrid-0.3.98/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    19803 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2023-12-23 10:16:29.000000 hagrid-0.3.98/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-23 10:15:49.000000 hagrid-0.3.98/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-23 10:15:29.000000 hagrid-0.3.98/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 10:17:24.598724 hagrid-0.3.98/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-23 10:17:24.000000 hagrid-0.3.98/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-23 10:17:24.000000 hagrid-0.3.98/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 10:17:24.000000 hagrid-0.3.98/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-23 10:17:24.000000 hagrid-0.3.98/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-23 10:17:24.000000 hagrid-0.3.98/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-23 10:17:24.000000 hagrid-0.3.98/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 10:17:24.598724 hagrid-0.3.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-12-23 10:15:49.000000 hagrid-0.3.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 10:17:24.598724 hagrid-0.3.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 10:15:29.000000 hagrid-0.3.98/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 10:17:24.598724 hagrid-0.3.98/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 10:15:29.000000 hagrid-0.3.98/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2023-12-23 10:15:29.000000 hagrid-0.3.98/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 10:20:14.744310 hagrid-0.3.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-24 10:20:14.744310 hagrid-0.3.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2023-12-24 10:18:34.000000 hagrid-0.3.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 10:20:14.740310 hagrid-0.3.99/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143990 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29773 2023-12-24 10:19:21.000000 hagrid-0.3.99/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12057 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14037 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-24 10:18:44.000000 hagrid-0.3.99/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19803 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2023-12-24 10:19:21.000000 hagrid-0.3.99/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-24 10:18:44.000000 hagrid-0.3.99/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-24 10:18:34.000000 hagrid-0.3.99/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 10:20:14.744310 hagrid-0.3.99/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-24 10:20:14.000000 hagrid-0.3.99/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-24 10:20:14.000000 hagrid-0.3.99/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 10:20:14.000000 hagrid-0.3.99/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-24 10:20:14.000000 hagrid-0.3.99/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-24 10:20:14.000000 hagrid-0.3.99/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-24 10:20:14.000000 hagrid-0.3.99/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-24 10:20:14.744310 hagrid-0.3.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-12-24 10:18:44.000000 hagrid-0.3.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 10:20:14.744310 hagrid-0.3.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 10:18:34.000000 hagrid-0.3.99/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 10:20:14.744310 hagrid-0.3.99/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-24 10:18:34.000000 hagrid-0.3.99/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2023-12-24 10:18:34.000000 hagrid-0.3.99/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.98/PKG-INFO` & `hagrid-0.3.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagrid
-Version: 0.3.98
+Version: 0.3.99
 Summary: Happy Automation for Grid
 Author: Andrew Trask <andrew@openmined.org>
 Description-Content-Type: text/plain
 Requires-Dist: ascii_magic
 Requires-Dist: click>=8.1.7
 Requires-Dist: cryptography>=41.0.4
 Requires-Dist: gitpython
```

### Comparing `hagrid-0.3.98/README.md` & `hagrid-0.3.99/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/__init__.py` & `hagrid-0.3.99/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/art.py` & `hagrid-0.3.99/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/auth.py` & `hagrid-0.3.99/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/azure.py` & `hagrid-0.3.99/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/cache.py` & `hagrid-0.3.99/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/cli.py` & `hagrid-0.3.99/hagrid/cli.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/deps.py` & `hagrid-0.3.99/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/grammar.py` & `hagrid-0.3.99/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/land.py` & `hagrid-0.3.99/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/launch.py` & `hagrid-0.3.99/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/lib.py` & `hagrid-0.3.99/hagrid/lib.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/manifest_template.yml` & `hagrid-0.3.99/hagrid/manifest_template.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.98
+hagrid_version: 0.3.99
 syft_version: 0.8.4-beta.10
 dockerTag: 0.8.4-beta.10
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: c58be0f24ff03b6f46ad6679f068a3f3a9e75454
+hash: c3a50ec4ca28534460440ad99a705e632238df2d
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
     - rabbitmq/rabbitmq.conf
     - redis/redis.conf
```

### Comparing `hagrid-0.3.98/hagrid/mode.py` & `hagrid-0.3.99/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/names.py` & `hagrid-0.3.99/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/orchestra.py` & `hagrid-0.3.99/hagrid/orchestra.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/parse_template.py` & `hagrid-0.3.99/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/quickstart_ui.py` & `hagrid-0.3.99/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/rand_sec.py` & `hagrid-0.3.99/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/style.py` & `hagrid-0.3.99/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/util.py` & `hagrid-0.3.99/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/win_bootstrap.py` & `hagrid-0.3.99/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid/wizard_ui.py` & `hagrid-0.3.99/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/hagrid.egg-info/PKG-INFO` & `hagrid-0.3.99/hagrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagrid
-Version: 0.3.98
+Version: 0.3.99
 Summary: Happy Automation for Grid
 Author: Andrew Trask <andrew@openmined.org>
 Description-Content-Type: text/plain
 Requires-Dist: ascii_magic
 Requires-Dist: click>=8.1.7
 Requires-Dist: cryptography>=41.0.4
 Requires-Dist: gitpython
```

### Comparing `hagrid-0.3.98/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.99/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.98/setup.py` & `hagrid-0.3.99/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.98"
+__version__ = "0.3.99"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=8.1.7",
     "cryptography>=41.0.4",
```

### Comparing `hagrid-0.3.98/tests/hagrid/cli_test.py` & `hagrid-0.3.99/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

