# Comparing `tmp/nbtof-0.0.6.tar.gz` & `tmp/nbtof-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbtof-0.0.6.tar", last modified: Fri May  3 07:18:23 2024, max compression
+gzip compressed data, was "nbtof-0.0.7.tar", last modified: Sat May  4 13:52:18 2024, max compression
```

## Comparing `nbtof-0.0.6.tar` & `nbtof-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 07:18:23.133345 nbtof-0.0.6/
--rw-rw-rw-   0        0        0     1084 2023-11-20 14:37:06.000000 nbtof-0.0.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-12-12 14:56:20.000000 nbtof-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3107 2024-05-03 07:18:23.132386 nbtof-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2024-01-02 04:04:03.000000 nbtof-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 07:18:23.122348 nbtof-0.0.6/nbtof/
--rw-rw-rw-   0        0        0       54 2024-05-03 07:16:39.000000 nbtof-0.0.6/nbtof/__init__.py
--rw-rw-rw-   0        0        0    11564 2024-05-03 06:03:50.000000 nbtof-0.0.6/nbtof/nbtof_base.py
--rw-rw-rw-   0        0        0     9289 2024-05-02 07:02:04.000000 nbtof-0.0.6/nbtof/nbtof_concat.py
--rw-rw-rw-   0        0        0     2777 2024-05-03 06:05:36.000000 nbtof-0.0.6/nbtof/nbtof_generate.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:18:23.130416 nbtof-0.0.6/nbtof.egg-info/
--rw-rw-rw-   0        0        0     3107 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 07:18:23.000000 nbtof-0.0.6/nbtof.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 07:18:23.133345 nbtof-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1337 2024-05-03 07:17:44.000000 nbtof-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:52:18.168233 nbtof-0.0.7/
+-rw-rw-rw-   0        0        0     1084 2023-11-20 14:37:06.000000 nbtof-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-12-12 14:56:20.000000 nbtof-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4462 2024-05-04 13:52:18.166229 nbtof-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3788 2024-05-04 09:38:02.000000 nbtof-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 13:52:18.154507 nbtof-0.0.7/nbtof/
+-rw-rw-rw-   0        0        0       54 2024-05-03 07:16:39.000000 nbtof-0.0.7/nbtof/__init__.py
+-rw-rw-rw-   0        0        0    12387 2024-05-04 13:46:23.000000 nbtof-0.0.7/nbtof/nbtof_base.py
+-rw-rw-rw-   0        0        0     9289 2024-05-02 07:02:04.000000 nbtof-0.0.7/nbtof/nbtof_concat.py
+-rw-rw-rw-   0        0        0     2777 2024-05-03 06:05:36.000000 nbtof-0.0.7/nbtof/nbtof_generate.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:52:18.162432 nbtof-0.0.7/nbtof.egg-info/
+-rw-rw-rw-   0        0        0     4462 2024-05-04 13:52:17.000000 nbtof-0.0.7/nbtof.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-04 13:52:18.000000 nbtof-0.0.7/nbtof.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 13:52:17.000000 nbtof-0.0.7/nbtof.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 13:52:17.000000 nbtof-0.0.7/nbtof.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 13:52:18.169228 nbtof-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2024-05-04 13:48:19.000000 nbtof-0.0.7/setup.py
```

### Comparing `nbtof-0.0.6/LICENSE` & `nbtof-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.6/nbtof/nbtof_base.py` & `nbtof-0.0.7/nbtof/nbtof_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import tempfile
 import os
 import subprocess
 import sys
 import copy
-import warnings
 
 def nbtof_base(
     notebook_name,
     func_name=None,
     func_file_name=None,
     ):
     """
@@ -121,14 +120,32 @@
     
         if check_num <= 0:
             if instant_list[0] == code_dict['# In[']:
                 instant_list[0]=code_dict['#@plane']
             instant_table.append(instant_list)
     table_hist_list.append(instant_table)
     
+    # organization return
+    instant_table = []
+    check_num = 0
+    for instant_list in table_hist_list[-1]:
+        if (instant_list[0] == code_dict['#@return'])*(instant_list[1][:len("#@return")] == "#@return"):
+            check_num = 1
+            instant_table.append(instant_list)
+        elif (check_num == 1)*(instant_list[0] == code_dict['#@return'])*(instant_list[1][:len("#@return")] != "#@return"):
+            check_num = 0
+            instant_table.append(instant_list)
+        elif (check_num == 0)*(instant_list[0] == code_dict['#@return'])*(instant_list[1][:len("#@return")] != "#@return"):
+            instant_list[0] = code_dict["#@plane"]
+            instant_table.append(instant_list)
+        else:
+            instant_table.append(instant_list)
+    
+    table_hist_list.append(instant_table)
+    
     # remove ignore
     instant_table = []
     for instant_list in table_hist_list[-1]:
         if (instant_list[0] != code_dict['#@ignore']):
             instant_table.append(instant_list)
     table_hist_list.append(instant_table)
```

### Comparing `nbtof-0.0.6/nbtof/nbtof_concat.py` & `nbtof-0.0.7/nbtof/nbtof_concat.py`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.6/nbtof/nbtof_generate.py` & `nbtof-0.0.7/nbtof/nbtof_generate.py`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.6/setup.py` & `nbtof-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = "nbtof: transfering notebook to function"
 NAME = 'nbtof'
 AUTHOR = 'Haruka Nodaka'
 AUTHOR_EMAIL = 'haruka.nodaka@gmail.com'
 URL = 'https://github.com/Nodaka/nbtof'
 LICENSE = 'MIT'
 DOWNLOAD_URL = 'https://github.com/Nodaka/nbtof'
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 PYTHON_REQUIRES = ">=3.9"
 
 INSTALL_REQUIRES = [
 #    'pandas',
 #    'nbconvert',
 #    'jupyter',
 ]
```

