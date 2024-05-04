# Comparing `tmp/ctdfjorder-0.0.34.tar.gz` & `tmp/ctdfjorder-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.34.tar", last modified: Sat May  4 05:11:46 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.35.tar", last modified: Sat May  4 05:29:10 2024, max compression
```

## Comparing `ctdfjorder-0.0.34.tar` & `ctdfjorder-0.0.35.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59056 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 05:11:46.000000 ctdfjorder-0.0.34/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:11:46.471471 ctdfjorder-0.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 05:11:42.000000 ctdfjorder-0.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:29:10.817178 ctdfjorder-0.0.35/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    59106 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/setup.py
```

### Comparing `ctdfjorder-0.0.34/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.35/CTDFjorder/CTDFjorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1391,15 +1391,17 @@
         print("Default processing completed successfully.")
 
     elif command == "defaultplotall":
         run_default(True)
         print("Default processing completed successfully.")
 
     elif command == "electron":
-        run_default(working_dir= sys.argv[2])
+        os.chdir(sys.argv[2])
+        print(sys.argv[2])
+        run_default(True, sys.argv[2])
         print("Default processing completed successfully")
 
     else:
         print(f"Unknown command: {command}")
         print("Usage: ctdfjorder <command> [arguments]")
         print("Commands:")
         print("  process <file>          Process a single RSK file")
```

### Comparing `ctdfjorder-0.0.34/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.35/CTDFjorder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.34
+Version: 0.0.35
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.34/PKG-INFO` & `ctdfjorder-0.0.35/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.34
+Version: 0.0.35
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.34/README.md` & `ctdfjorder-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.34/setup.py` & `ctdfjorder-0.0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.34",
+    version="0.0.35",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

