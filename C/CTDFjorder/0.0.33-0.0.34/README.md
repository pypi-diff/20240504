# Comparing `tmp/ctdfjorder-0.0.33.tar.gz` & `tmp/ctdfjorder-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.33.tar", last modified: Sat May  4 04:52:31 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.34.tar", last modified: Sat May  4 05:11:46 2024, max compression
```

## Comparing `ctdfjorder-0.0.33.tar` & `ctdfjorder-0.0.34.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59056 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 04:52:31.000000 ctdfjorder-0.0.33/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 04:52:31.441393 ctdfjorder-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:52:31.445393 ctdfjorder-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-04 04:52:26.000000 ctdfjorder-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    59056 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/setup.py
```

### Comparing `ctdfjorder-0.0.33/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.34/CTDFjorder/CTDFjorder.py`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.33/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.34/CTDFjorder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.33
+Version: 0.0.34
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.33/PKG-INFO` & `ctdfjorder-0.0.34/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.33
+Version: 0.0.34
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.33/README.md` & `ctdfjorder-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.33/setup.py` & `ctdfjorder-0.0.34/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.33",
+    version="0.0.34",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
@@ -30,12 +30,12 @@
         "tabulate>=0.9.0",
         "pyrsktools==0.1.9",
         "openpyxl>=3.1.2",
         "setuptools"
     ],
     packages=find_packages(),
     entry_points={
-        "console_scripts": [
-            "CTDFjorder-cli = CTDFjorder:main"
-        ]
+        'console_scripts': [
+            'ctdfjorder-cli=CTDFjorder.CTDFjorder:main',
+        ],
     },
-)
+)
```

