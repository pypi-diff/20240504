# Comparing `tmp/jklib-5.1.0.tar.gz` & `tmp/jklib-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jklib-5.1.0.tar", last modified: Sun Apr 14 20:05:29 2024, max compression
+gzip compressed data, was "jklib-5.1.1.tar", last modified: Sat May  4 16:57:54 2024, max compression
```

## Comparing `jklib-5.1.0.tar` & `jklib-5.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 20:05:21.000000 jklib-5.1.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 20:05:29.076698 jklib-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-14 20:05:21.000000 jklib-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.068698 jklib-5.1.0/jklib/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.072698 jklib-5.1.0/jklib/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.072698 jklib-5.1.0/jklib/meili/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/jklib/meili/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/jklib/std/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/jklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:05:29.076698 jklib-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-14 20:05:21.000000 jklib-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.144989 jklib-5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-04 16:57:43.000000 jklib-5.1.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 16:57:54.144989 jklib-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-04 16:57:43.000000 jklib-5.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.136989 jklib-5.1.1/jklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.140989 jklib-5.1.1/jklib/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.140989 jklib-5.1.1/jklib/meili/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.140989 jklib-5.1.1/jklib/meili/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.144989 jklib-5.1.1/jklib/std/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.144989 jklib-5.1.1/jklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:57:54.144989 jklib-5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-04 16:57:43.000000 jklib-5.1.1/setup.py
```

### Comparing `jklib-5.1.0/LICENCE.txt` & `jklib-5.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/PKG-INFO` & `jklib-5.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jklib
-Version: 5.1.0
+Version: 5.1.1
 Summary: Package with utility functions on many different subjects
 Home-page: https://github.com/Jordan-Kowal/jklib
-Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.1.0.tar.gz
+Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.1.1.tar.gz
 Author: Jordan Kowal
 Author-email: kowaljordan@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jklib-5.1.0/README.md` & `jklib-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/admin.py` & `jklib-5.1.1/jklib/dj/admin.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/decorators.py` & `jklib-5.1.1/jklib/dj/decorators.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/emails.py` & `jklib-5.1.1/jklib/dj/emails.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/exceptions.py` & `jklib-5.1.1/jklib/dj/exceptions.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/files.py` & `jklib-5.1.1/jklib/dj/files.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/images.py` & `jklib-5.1.1/jklib/dj/images.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/managers.py` & `jklib-5.1.1/jklib/dj/managers.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/models.py` & `jklib-5.1.1/jklib/dj/models.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/network.py` & `jklib-5.1.1/jklib/dj/network.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/permissions.py` & `jklib-5.1.1/jklib/dj/permissions.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/serializers.py` & `jklib-5.1.1/jklib/dj/serializers.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/test_runner.py` & `jklib-5.1.1/jklib/dj/test_runner.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/tests.py` & `jklib-5.1.1/jklib/dj/tests.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/validators.py` & `jklib-5.1.1/jklib/dj/validators.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/dj/viewsets.py` & `jklib-5.1.1/jklib/dj/viewsets.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/meili/dj/indexer.py` & `jklib-5.1.1/jklib/meili/dj/indexer.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/meili/dj/serializers.py` & `jklib-5.1.1/jklib/meili/dj/serializers.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/meili/dj/test_utils.py` & `jklib-5.1.1/jklib/meili/dj/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # Django
 from django.db.models import Model, Q
 from django.test import tag
 
 # Application
 from jklib.meili.dj.indexer import MeilisearchModelIndexer
 
-SLEEP_TIME = 0.07
 
 M = TypeVar("M", bound=Model)
 
 
 @tag("integration")
 class IndexerBaseTestMixin(Generic[M]):
     """
@@ -30,157 +29,158 @@
 
     meilisearch_client: Client
 
     indexer_class: Type[MeilisearchModelIndexer]
     item_1: M
     item_2: M
     search_attribute: str
+    sleep_time: float = 0.1
 
     def setUp(self):
         super().setUp()
         self.meilisearch_client.delete_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
 
     def tearDown(self):
         self.meilisearch_client.delete_index(self.indexer_class.index_name())
         super().tearDown()
 
     def test_index_exists(self) -> None:
         self.assertFalse(self.indexer_class.index_exists())
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         self.assertTrue(self.indexer_class.index_exists())
 
     def test_maybe_create_index(self) -> None:
         self.assertFalse(self.indexer_class.index_exists())
         self.indexer_class.maybe_create_index()
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         self.assertTrue(self.indexer_class.index_exists())
 
     def test_update_settings(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         self.indexer_class.update_settings()
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).get_settings()
         for key, value in self.indexer_class.SETTINGS.items():
             self.assertEqual(response[key], value)
 
     def test_index(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search(getattr(self.item_1, self.search_attribute))
         self.assertSearchHits(response, [])
         self.indexer_class.index(self.item_1)
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search(getattr(self.item_1, self.search_attribute))
         self.assertSearchHits(response, [self.item_1])
 
     def test_index_multiple(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [])
         self.indexer_class.index_multiple([self.item_1, self.item_2])
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [self.item_1, self.item_2])
 
     def test_index_from_query(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search(getattr(self.item_1, self.search_attribute))
         self.assertSearchHits(response, [])
         self.indexer_class.index_from_query(Q(id=self.item_1.id))
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search(getattr(self.item_1, self.search_attribute))
         self.assertSearchHits(response, [self.item_1])
 
     def test_index_all(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [])
         self.indexer_class.index_all()
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [self.item_1, self.item_2])
 
     def test_index_all_atomically(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertEqual(response["hits"], [])
         self.indexer_class.index_all_atomically()
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [self.item_1, self.item_2])
 
     def test_unindex(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         self.indexer_class.index(self.item_1)
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search(getattr(self.item_1, self.search_attribute))
         self.assertSearchHits(response, [self.item_1])
         self.indexer_class.unindex(self.item_1.id)
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search(getattr(self.item_1, self.search_attribute))
         self.assertSearchHits(response, [])
 
     def test_unindex_multiple(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         self.indexer_class.index_multiple([self.item_1, self.item_2])
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [self.item_1, self.item_2])
         self.indexer_class.unindex_multiple([self.item_1.id, self.item_2.id])
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.meilisearch_client.index(
             self.indexer_class.index_name()
         ).search("")
         self.assertSearchHits(response, [])
 
     def test_search(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
         search_value = getattr(self.item_1, self.search_attribute)
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.indexer_class.search(search_value)
         self.assertSearchHits(response, [])
         self.indexer_class.index(self.item_1)
-        sleep(SLEEP_TIME)
+        sleep(self.sleep_time)
         response = self.indexer_class.search(search_value)
         self.assertSearchHits(response, [self.item_1])
         self.assertEqual(response.get("limit"), 20)
         response = self.indexer_class.search(search_value, limit=1)
         self.assertSearchHits(response, [self.item_1])
         self.assertEqual(response.get("limit"), 1)
         response = self.indexer_class.search(search_value, only_hits=True, limit=1)
```

### Comparing `jklib-5.1.0/jklib/meili/search.py` & `jklib-5.1.1/jklib/meili/search.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/meili/types.py` & `jklib-5.1.1/jklib/meili/types.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/std/files.py` & `jklib-5.1.1/jklib/std/files.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/std/images.py` & `jklib-5.1.1/jklib/std/images.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/std/inputs.py` & `jklib-5.1.1/jklib/std/inputs.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/std/strings.py` & `jklib-5.1.1/jklib/std/strings.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib/std/transforms.py` & `jklib-5.1.1/jklib/std/transforms.py`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/jklib.egg-info/PKG-INFO` & `jklib-5.1.1/jklib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jklib
-Version: 5.1.0
+Version: 5.1.1
 Summary: Package with utility functions on many different subjects
 Home-page: https://github.com/Jordan-Kowal/jklib
-Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.1.0.tar.gz
+Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.1.1.tar.gz
 Author: Jordan Kowal
 Author-email: kowaljordan@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jklib-5.1.0/jklib.egg-info/SOURCES.txt` & `jklib-5.1.1/jklib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jklib-5.1.0/setup.py` & `jklib-5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Third-party
 from setuptools import find_packages, setup
 
 # --------------------------------------------------------------------------------
 # > Variables
 # --------------------------------------------------------------------------------
-VERSION = "5.1.0"
+VERSION = "5.1.1"
 packages = find_packages()
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 # --------------------------------------------------------------------------------
 # > Setup
 # --------------------------------------------------------------------------------
```

