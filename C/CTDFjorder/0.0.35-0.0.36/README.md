# Comparing `tmp/ctdfjorder-0.0.35.tar.gz` & `tmp/ctdfjorder-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.35.tar", last modified: Sat May  4 05:29:10 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.36.tar", last modified: Sat May  4 05:35:44 2024, max compression
```

## Comparing `ctdfjorder-0.0.35.tar` & `ctdfjorder-0.0.36.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:29:10.817178 ctdfjorder-0.0.35/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59106 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 05:29:10.000000 ctdfjorder-0.0.35/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:29:10.821178 ctdfjorder-0.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 05:29:01.000000 ctdfjorder-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    59049 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/setup.py
```

### Comparing `ctdfjorder-0.0.35/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.36/CTDFjorder/CTDFjorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1250,16 +1250,14 @@
         self.filename = filename
         self.message = message
         super().__init__(self.message)
 
 
 def run_default(plot=False, working_dir = None):
     _reset_file_environment()
-    if working_dir:
-        os.chdir(f'[{working_dir}]')
     CTD.master_sheet_path = os.path.join(_get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
     rsk_files_list = get_rsk_filenames_in_dir(_get_cwd())
     for file in rsk_files_list:
         try:
             my_data = CTD(file)
             my_data.add_filename_to_table()
             my_data.save_to_csv("output.csv")
```

### Comparing `ctdfjorder-0.0.35/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.36/CTDFjorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.35
+Version: 0.0.36
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.35/PKG-INFO` & `ctdfjorder-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.35
+Version: 0.0.36
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.35/README.md` & `ctdfjorder-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.35/setup.py` & `ctdfjorder-0.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.35",
+    version="0.0.36",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

