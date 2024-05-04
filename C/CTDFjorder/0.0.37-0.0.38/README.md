# Comparing `tmp/ctdfjorder-0.0.37.tar.gz` & `tmp/ctdfjorder-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.37.tar", last modified: Sat May  4 06:49:02 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.38.tar", last modified: Sat May  4 07:02:00 2024, max compression
```

## Comparing `ctdfjorder-0.0.37.tar` & `ctdfjorder-0.0.38.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59116 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:02:00.462280 ctdfjorder-0.0.38/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:02:00.462280 ctdfjorder-0.0.38/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    59123 2024-05-04 07:01:56.000000 ctdfjorder-0.0.38/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 07:01:56.000000 ctdfjorder-0.0.38/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:02:00.462280 ctdfjorder-0.0.38/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 07:02:00.000000 ctdfjorder-0.0.38/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 07:02:00.000000 ctdfjorder-0.0.38/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:02:00.000000 ctdfjorder-0.0.38/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 07:02:00.000000 ctdfjorder-0.0.38/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 07:02:00.000000 ctdfjorder-0.0.38/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 07:02:00.000000 ctdfjorder-0.0.38/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 07:02:00.462280 ctdfjorder-0.0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 07:01:56.000000 ctdfjorder-0.0.38/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:02:00.462280 ctdfjorder-0.0.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 07:01:56.000000 ctdfjorder-0.0.38/setup.py
```

### Comparing `ctdfjorder-0.0.37/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.38/CTDFjorder/CTDFjorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,15 +635,15 @@
 
             # Check if the master sheet is already cached
             if CTD._cached_master_sheet is None:
                 # Load the master sheet and cache it
                 CTD._cached_master_sheet = pd.read_excel(master_sheet_path)
 
             # Use the cached master sheet data
-            master_df = CTD._cached_master_sheet
+            master_df = CTD._cached_master_sheet.copy()
             # Get date and time components from the filename
             year, month, day, time = get_date_from_string(filename)
             if year is None:
                 return
             # Calculate absolute differences for each row in 'master_df'
             master_df['date_difference'] = master_df.apply(date_difference, args=(year, month, day), axis=1)
             master_df['time_difference'] = master_df['time_local'].apply(lambda x: time_difference(time, x))
```

### Comparing `ctdfjorder-0.0.37/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.38/CTDFjorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.37
+Version: 0.0.38
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.37/PKG-INFO` & `ctdfjorder-0.0.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.37
+Version: 0.0.38
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.37/README.md` & `ctdfjorder-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.37/setup.py` & `ctdfjorder-0.0.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.37",
+    version="0.0.38",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

