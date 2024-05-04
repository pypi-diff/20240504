# Comparing `tmp/abstract_pandas-0.0.0.4.tar.gz` & `tmp/abstract_pandas-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.4.tar", last modified: Mon Apr 29 22:32:32 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.5.tar", last modified: Fri May  3 07:53:18 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.4.tar` & `abstract_pandas-0.0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 22:32:32.112074 abstract_pandas-0.0.0.4/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 22:32:32.112074 abstract_pandas-0.0.0.4/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.4/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-29 22:32:32.112074 abstract_pandas-0.0.0.4/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-04-29 22:32:23.000000 abstract_pandas-0.0.0.4/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 22:32:32.108075 abstract_pandas-0.0.0.4/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 22:32:32.112074 abstract_pandas-0.0.0.4/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/class_manager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    16258 2024-04-29 22:31:50.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.4/src/abstract_pandas/time_module.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 22:32:32.112074 abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 22:32:32.000000 abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      512 2024-04-29 22:32:32.000000 abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-29 22:32:32.000000 abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-04-29 22:32:32.000000 abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-04-29 22:32:32.000000 abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.5/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-05-03 07:53:00.000000 abstract_pandas-0.0.0.5/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.115340 abstract_pandas-0.0.0.5/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/class_manager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15967 2024-05-03 07:52:16.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/geo_pandas.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/geo_spec.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      290 2024-05-03 07:49:52.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/test_sol.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.5/src/abstract_pandas/time_module.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 07:53:18.119340 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      544 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-03 07:53:18.000000 abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.4/PKG-INFO` & `abstract_pandas-0.0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.4
+Version: 0.0.0.5
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.4/setup.py` & `abstract_pandas-0.0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.4',
+    version='0.0.0.5',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.5/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.5/src/abstract_pandas/excel_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 from pyexcel_ods import get_data
 import ezodf
 import tempfile,shutil,os
 from abstract_utilities import *
 from odf import text, teletype
 from odf.opendocument import load
-from .general_functions import *
+from general_functions import *
 from datetime import datetime
 from itertools import permutations
 from difflib import get_close_matches
 from datetime import datetime
 import pandas as pd
 from pyxlsb import open_workbook
 import pandas as pd
@@ -20,14 +20,16 @@
 from io import BytesIO
 # Example usage
 
 
 def safe_excel_save(df,original_file_path,index=False, engine='openpyxl'):
     with tempfile.NamedTemporaryFile(delete=False, suffix='.xlsx') as tmp:
         temp_file_name = tmp.name
+        if not isinstance(headers_js,pd.DataFrame):
+            df = pd.DataFrame(new_data = pd.DataFrame([headers_js]))
         df.to_excel(tmp.name, index=index, engine=engine)  # Save your DataFrame to the temp file
     if os.path.getsize(temp_file_name) > 0:
         shutil.move(temp_file_name, original_file_path)
     else:
         print("Temporary file is empty or wasn't written correctly. Original file is unchanged.")
     # Cleanup: Ensure the temporary file is deleted if it hasn't been moved
     if os.path.exists(temp_file_name):
@@ -177,15 +179,15 @@
             elif file_ext == '.ods':
                 return pd.read_excel(source, engine='odf', nrows=nrows)  # For .ods files
             elif file_ext in ('.xlsx', '.xls'):
                 return pd.read_excel(source, engine='openpyxl', nrows=nrows)  # For Excel files
             elif file_ext == '.tsv':  # Handle TSV files
                 return pd.read_csv(source, sep='\t', nrows=nrows)
             elif file_ext == '.xlsb':
-                return read_xlsb_to_dataframe(source,nrows=nrows)  # Custom function to handle .xlsb
+                return pd.read_excel(source, engine = 'pyxlsb',nrows=nrows) # Custom function to handle .xlsb
         except Exception as e:
             print(f"Failed to read file: {e}")
     elif isinstance(source, FileStorage):  # Check if source is a FileStorage object
         try:
             # Read the file directly from the file object, considering Excel format
             return pd.read_excel(source.stream, nrows=nrows)
         except Exception as e:
@@ -193,25 +195,15 @@
     else:
         print("Invalid source provided.")
     
     return None
 
 
 
-def read_xlsb_to_dataframe(file_path, sheet_name=1,nrows=None):
-    data = []
-    with open_workbook(file_path) as wb:
-        with wb.get_sheet(sheet_name) as sheet:
-            for row in sheet.rows():
-                headers = [cell.v for cell in row]
-                if nrows == 0:
-                    return headers
-                data.append(headers)
-    # Create a DataFrame
-    return pd.DataFrame(data)
+
 def read_excel_as_dicts(file_path):
     # Read the Excel file
     df = pd.read_excel(file_path, engine='openpyxl')
     # Convert each row to a dictionary with column headers as keys
     rows_as_dicts = df.to_dict(orient='records')
     return rows_as_dicts
```

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.5/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas/geo_pandas.py` & `abstract_pandas-0.0.0.5/src/abstract_pandas/geo_pandas.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas/geo_spec.py` & `abstract_pandas-0.0.0.5/src/abstract_pandas/geo_spec.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas/time_module.py` & `abstract_pandas-0.0.0.5/src/abstract_pandas/time_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.4
+Version: 0.0.0.5
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.4/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.5/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 src/abstract_pandas/__init__.py
 src/abstract_pandas/class_manager.py
 src/abstract_pandas/excel_gui.py
 src/abstract_pandas/excel_module.py
 src/abstract_pandas/general_functions.py
 src/abstract_pandas/geo_pandas.py
 src/abstract_pandas/geo_spec.py
+src/abstract_pandas/test_sol.py
 src/abstract_pandas/time_module.py
 src/abstract_pandas.egg-info/PKG-INFO
 src/abstract_pandas.egg-info/SOURCES.txt
 src/abstract_pandas.egg-info/dependency_links.txt
 src/abstract_pandas.egg-info/requires.txt
 src/abstract_pandas.egg-info/top_level.txt
```

