# Comparing `tmp/ctdfjorder-0.0.36.tar.gz` & `tmp/ctdfjorder-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.36.tar", last modified: Sat May  4 05:35:44 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.37.tar", last modified: Sat May  4 06:49:02 2024, max compression
```

## Comparing `ctdfjorder-0.0.36.tar` & `ctdfjorder-0.0.37.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59049 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 05:35:44.000000 ctdfjorder-0.0.36/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:35:44.744379 ctdfjorder-0.0.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 05:35:40.000000 ctdfjorder-0.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    59116 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 06:49:02.000000 ctdfjorder-0.0.37/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:49:02.321112 ctdfjorder-0.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 06:48:55.000000 ctdfjorder-0.0.37/setup.py
```

### Comparing `ctdfjorder-0.0.36/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.37/CTDFjorder/CTDFjorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
     """
     _ctd_array = pandas.DataFrame()
     _rsk = None
     _filename = None
     _calculator = None
     _cwd = None
+    _cached_master_sheet = None
     master_sheet_path = "FjordPhyto MASTER SHEET.xlsx"
     _NO_SAMPLES_ERROR = "No samples in file."
     _NO_LOCATION_ERROR = "No location could be found."
     _DENSITY_CALCULATION_ERROR = "Could not calculate density on this dataset."
     _SALINITYABS_CALCULATION_ERROR = "Could not calculate density on this dataset."
     _DATA_CLEANING_ERROR = "No data remains after data cleaning, reverting to previous CTD"
     _REMOVE_NEGATIVES_ERROR = "No data remains after removing non-positive samples."
@@ -628,16 +629,21 @@
                 target_hour, target_minute = [int(target_time.split(':')[0]), int(target_time.split(':')[1])]
                 try:
                     df_hour, df_minute = [int(df_time_str.split(':')[0]), int(df_time_str.split(':')[1])]
                 except:
                     return None
                 return abs((target_hour * 60 + target_minute) - (df_hour * 60 + df_minute))
 
-            # Load the master sheet
-            master_df = pd.read_excel(master_sheet_path)
+            # Check if the master sheet is already cached
+            if CTD._cached_master_sheet is None:
+                # Load the master sheet and cache it
+                CTD._cached_master_sheet = pd.read_excel(master_sheet_path)
+
+            # Use the cached master sheet data
+            master_df = CTD._cached_master_sheet
             # Get date and time components from the filename
             year, month, day, time = get_date_from_string(filename)
             if year is None:
                 return
             # Calculate absolute differences for each row in 'master_df'
             master_df['date_difference'] = master_df.apply(date_difference, args=(year, month, day), axis=1)
             master_df['time_difference'] = master_df['time_local'].apply(lambda x: time_difference(time, x))
@@ -1248,15 +1254,15 @@
 
     def __init__(self, filename, message=" Unknown, check to make sure your mastersheet is in your current directory."):
         self.filename = filename
         self.message = message
         super().__init__(self.message)
 
 
-def run_default(plot=False, working_dir = None):
+def run_default(plot=False):
     _reset_file_environment()
     CTD.master_sheet_path = os.path.join(_get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
     rsk_files_list = get_rsk_filenames_in_dir(_get_cwd())
     for file in rsk_files_list:
         try:
             my_data = CTD(file)
             my_data.add_filename_to_table()
@@ -1388,28 +1394,21 @@
         run_default()
         print("Default processing completed successfully.")
 
     elif command == "defaultplotall":
         run_default(True)
         print("Default processing completed successfully.")
 
-    elif command == "electron":
-        os.chdir(sys.argv[2])
-        print(sys.argv[2])
-        run_default(True, sys.argv[2])
-        print("Default processing completed successfully")
-
     else:
         print(f"Unknown command: {command}")
         print("Usage: ctdfjorder <command> [arguments]")
         print("Commands:")
         print("  process <file>          Process a single RSK file")
         print("  merge                   Merge all RSK files in the current folder")
         print("  default                 Run the default processing pipeline")
         print("  defaultplotall          Run the default processing pipeline and create plots")
         print("CWD:")
         print(_get_cwd())
         sys.exit(1)
 
-
-if __name__ == "main":
+if __name__ == "__main__":
     main()
```

### Comparing `ctdfjorder-0.0.36/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.37/CTDFjorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.36
+Version: 0.0.37
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.36/PKG-INFO` & `ctdfjorder-0.0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.36
+Version: 0.0.37
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.36/README.md` & `ctdfjorder-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.36/setup.py` & `ctdfjorder-0.0.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.36",
+    version="0.0.37",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

