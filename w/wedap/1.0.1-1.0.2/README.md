# Comparing `tmp/wedap-1.0.1.tar.gz` & `tmp/wedap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedap-1.0.1.tar", last modified: Wed Apr 24 17:18:08 2024, max compression
+gzip compressed data, was "wedap-1.0.2.tar", last modified: Sat May  4 00:48:07 2024, max compression
```

## Comparing `wedap-1.0.1.tar` & `wedap-1.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.118682 wedap-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-24 17:17:50.000000 wedap-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-24 17:18:08.118682 wedap-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-24 17:17:50.000000 wedap-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/mdap/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 17:17:50.000000 wedap-1.0.1/mdap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-24 17:17:50.000000 wedap-1.0.1/mdap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-04-24 17:17:50.000000 wedap-1.0.1/mdap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/md_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/mdap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/styles/default.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/mdap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/tests/make_md_pdist_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-24 17:17:51.000000 wedap-1.0.1/mdap/tests/test_md_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:18:08.118682 wedap-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-24 17:17:51.000000 wedap-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.110682 wedap-1.0.1/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/styles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wedap/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28147 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/h5_gif.py
--rw-r--r--   0 runner    (1001) docker     (127)    69160 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wedap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/styles/default.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wedap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/make_h5_pdist_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/make_h5_plot_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/test_h5_pdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-24 17:17:51.000000 wedap-1.0.1/wedap/tests/test_h5_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.118682 wedap-1.0.1/wedap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 17:18:08.000000 wedap-1.0.1/wedap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wekap/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wekap/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/data/ppf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.114682 wedap-1.0.1/wekap/error/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/error/GetAvg_CR.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/error/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:18:08.118682 wedap-1.0.1/wekap/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 17:17:51.000000 wedap-1.0.1/wekap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-04 00:47:47.000000 wedap-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-05-04 00:48:07.772097 wedap-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-04 00:47:47.000000 wedap-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.768097 wedap-1.0.2/mdap/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22751 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/md_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.768097 wedap-1.0.2/mdap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.768097 wedap-1.0.2/mdap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/tests/make_md_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-04 00:47:47.000000 wedap-1.0.2/mdap/tests/test_md_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:48:07.772097 wedap-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-04 00:47:47.000000 wedap-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.768097 wedap-1.0.2/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:47:47.000000 wedap-1.0.2/styles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.768097 wedap-1.0.2/wedap/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-04 00:47:47.000000 wedap-1.0.2/wedap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-04 00:47:47.000000 wedap-1.0.2/wedap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28147 2024-05-04 00:47:47.000000 wedap-1.0.2/wedap/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/h5_gif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69160 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31441 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.768097 wedap-1.0.2/wedap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/styles/default.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/wedap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/tests/make_h5_pdist_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/tests/make_h5_plot_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/tests/test_h5_pdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-04 00:47:48.000000 wedap-1.0.2/wedap/tests/test_h5_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/wedap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-05-04 00:48:07.000000 wedap-1.0.2/wedap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-04 00:48:07.000000 wedap-1.0.2/wedap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:48:07.000000 wedap-1.0.2/wedap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-04 00:48:07.000000 wedap-1.0.2/wedap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 00:48:07.000000 wedap-1.0.2/wedap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 00:48:07.000000 wedap-1.0.2/wedap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/wekap/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/wekap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/data/ppf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/wekap/error/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/error/GetAvg_CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/error/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:48:07.772097 wedap-1.0.2/wekap/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 00:47:48.000000 wedap-1.0.2/wekap/styles/default.mplstyle
```

### Comparing `wedap-1.0.1/LICENSE` & `wedap-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/PKG-INFO` & `wedap-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Weighted Ensemble Data Analysis and Plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
```

### Comparing `wedap-1.0.1/README.md` & `wedap-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/mdap/__main__.py` & `wedap-1.0.2/mdap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/mdap/command_line.py` & `wedap-1.0.2/mdap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/mdap/md_pdist.py` & `wedap-1.0.2/mdap/md_pdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,18 @@
             if data_item.ndim < 2:
                 data_item = data_item[:, np.newaxis]
 
             # if indexing is wrong (e.g. 1 for 1 column dataset when 0 index is needed)
             try:
                 data.append(data_item[::interval, index])
             except IndexError as e:
-                print(f"{e}: Note that by default MDAP uses the 2nd column of the input data, \
-                        which cooresponds to an X/Y/Zindex of 1. Your dataset may only have 1 column, \
-                        and in that case the X/Y/Zindex should be set to 0. Exiting...")
-                sys.exit(0)
+                message = f"{e}: Note that by default MDAP uses the 2nd column of the input data, " + \
+                          "which cooresponds to an X/Y/Zindex of 1. E.g. if your dataset only had 1 column, " + \
+                          "the X/Y/Zindex should be set to 0."
+                raise IndexError(message)
 
         # combine into a single array
         data = np.concatenate(data)
 
         return data
 
     def timeseries(self):
```

### Comparing `wedap-1.0.1/mdap/md_plot.py` & `wedap-1.0.2/mdap/md_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/mdap/tests/make_md_pdist_test_data.py` & `wedap-1.0.2/mdap/tests/make_md_pdist_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/mdap/tests/test_md_pdist.py` & `wedap-1.0.2/mdap/tests/test_md_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/setup.py` & `wedap-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('./LICENSE') as f:
     lic = f.read()
 
 packages = find_packages()
 
 setup(
     name='wedap',
-    version='1.0.1',
+    version='1.0.2',
     description='Weighted Ensemble Data Analysis and Plotting',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='Darian T. Yang',
     author_email='dty7@pitt.edu',
     install_requires=['numpy', 'matplotlib', 'h5py', 'gif', 'tqdm'],
     url='https://github.com/darianyang/wedap',
```

### Comparing `wedap-1.0.1/wedap/__main__.py` & `wedap-1.0.2/wedap/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,20 @@
     # a poor workaround for now for the weighted arg
     # this is only to make the gooey formatting look nicer in terms of the checkbox
     if args.not_weighted is True:
         args.weighted = False
     elif args.not_weighted is False:
         args.weighted = True
 
+    # default avg: when using scatter3d or hexbin3d, if Yname is provided (hence 2d and not evo),
+    # or if requesting line plot, all these conditions only if dt is wrong (default evolution)
+    if (args.plot_mode == "scatter3d" or args.plot_mode == "hexbin3d" or args.Yname is not None \
+       or args.plot_mode == "line") and args.data_type == "evolution" :
+        args.data_type = "average"
+
     #  make a gif instead of a single plot if gif_out is given
     # e.g. $ wedap -h5 wedap/data/p53.h5 -y pcoord -yi 1 -dt average --last-iter 16 
     #              --avg-plus 2 --gif-out test.gif --xlim 0 6 --ylim 0 36 --pmax 20
     if args.gif_out is not None:
         make_gif(**vars(args))
         # exit prematurely since gif making
         return
```

### Comparing `wedap-1.0.1/wedap/command_line.py` & `wedap-1.0.2/wedap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/h5_gif.py` & `wedap-1.0.2/wedap/h5_gif.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/h5_pdist.py` & `wedap-1.0.2/wedap/h5_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/h5_plot.py` & `wedap-1.0.2/wedap/h5_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/tests/make_h5_pdist_test_data.py` & `wedap-1.0.2/wedap/tests/make_h5_pdist_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/tests/make_h5_plot_test_data.py` & `wedap-1.0.2/wedap/tests/make_h5_plot_test_data.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/tests/test_h5_pdist.py` & `wedap-1.0.2/wedap/tests/test_h5_pdist.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap/tests/test_h5_plot.py` & `wedap-1.0.2/wedap/tests/test_h5_plot.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wedap.egg-info/PKG-INFO` & `wedap-1.0.2/wedap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Weighted Ensemble Data Analysis and Plotting
 Home-page: https://github.com/darianyang/wedap
 Author: Darian T. Yang
 Author-email: dty7@pitt.edu
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Darian Yang
```

### Comparing `wedap-1.0.1/wedap.egg-info/SOURCES.txt` & `wedap-1.0.2/wedap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wekap/__main__.py` & `wedap-1.0.2/wekap/__main__.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wekap/bootstrap.py` & `wedap-1.0.2/wekap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wekap/command_line.py` & `wedap-1.0.2/wekap/command_line.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wekap/error/GetAvg_CR.py` & `wedap-1.0.2/wekap/error/GetAvg_CR.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wekap/error/bootstrap.py` & `wedap-1.0.2/wekap/error/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wedap-1.0.1/wekap/kinetics.py` & `wedap-1.0.2/wekap/kinetics.py`

 * *Files identical despite different names*

