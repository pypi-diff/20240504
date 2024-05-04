# Comparing `tmp/ctdfjorder-0.0.32.tar.gz` & `tmp/ctdfjorder-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.32.tar", last modified: Sat May  4 04:43:02 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.33.tar", last modified: Sat May  4 04:52:31 2024, max compression
```

## Comparing `ctdfjorder-0.0.32.tar` & `ctdfjorder-0.0.33.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:43:02.937118 ctdfjorder-0.0.32/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:43:02.937118 ctdfjorder-0.0.32/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59056 2024-05-04 04:42:59.000000 ctdfjorder-0.0.32/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 04:42:59.000000 ctdfjorder-0.0.32/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:43:02.937118 ctdfjorder-0.0.32/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 04:43:02.000000 ctdfjorder-0.0.32/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 04:43:02.000000 ctdfjorder-0.0.32/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:43:02.000000 ctdfjorder-0.0.32/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 04:43:02.000000 ctdfjorder-0.0.32/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 04:43:02.000000 ctdfjorder-0.0.32/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 04:43:02.000000 ctdfjorder-0.0.32/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 04:43:02.937118 ctdfjorder-0.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 04:42:59.000000 ctdfjorder-0.0.32/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:43:02.937118 ctdfjorder-0.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-04 04:42:59.000000 ctdfjorder-0.0.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    59056 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:52:31.445393 ctdfjorder-0.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/setup.py
```

### Comparing `ctdfjorder-0.0.32/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.33/CTDFjorder/CTDFjorder.py`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.32/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.33/CTDFjorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.32
+Version: 0.0.33
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.32/PKG-INFO` & `ctdfjorder-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.32
+Version: 0.0.33
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.32/README.md` & `ctdfjorder-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.32/setup.py` & `ctdfjorder-0.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.32",
+    version="0.0.33",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

