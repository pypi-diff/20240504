# Comparing `tmp/STAIR-tools-1.1.8.tar.gz` & `tmp/STAIR-tools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.1.8.tar", last modified: Sun Apr 28 03:58:16 2024, max compression
+gzip compressed data, was "STAIR-tools-1.1.9.tar", last modified: Sun Apr 28 04:04:36 2024, max compression
```

## Comparing `STAIR-tools-1.1.8.tar` & `STAIR-tools-1.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 03:58:16.512546 STAIR-tools-1.1.8/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-28 03:58:16.512355 STAIR-tools-1.1.8/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.8/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 03:58:16.507203 STAIR-tools-1.1.8/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.8/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 03:58:16.507490 STAIR-tools-1.1.8/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.8/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.8/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18517 2024-04-26 11:02:07.000000 STAIR-tools-1.1.8/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 03:58:16.509983 STAIR-tools-1.1.8/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.8/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.8/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3891 2024-04-25 06:09:45.000000 STAIR-tools-1.1.8/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.8/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.8/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.8/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.8/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12324 2024-04-25 02:44:23.000000 STAIR-tools-1.1.8/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14202 2024-04-25 02:44:36.000000 STAIR-tools-1.1.8/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 03:58:16.511570 STAIR-tools-1.1.8/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.8/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.1.8/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.1.8/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.1.8/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.1.8/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.1.8/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.8/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 03:58:16.512165 STAIR-tools-1.1.8/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-28 03:58:16.000000 STAIR-tools-1.1.8/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-04-28 03:58:16.000000 STAIR-tools-1.1.8/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-28 03:58:16.000000 STAIR-tools-1.1.8/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-28 03:58:16.000000 STAIR-tools-1.1.8/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-28 03:58:16.512600 STAIR-tools-1.1.8/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      429 2024-04-28 03:58:12.000000 STAIR-tools-1.1.8/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.173136 STAIR-tools-1.1.9/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-28 04:04:36.172929 STAIR-tools-1.1.9/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.1.9/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.167302 STAIR-tools-1.1.9/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.1.9/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.167669 STAIR-tools-1.1.9/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.9/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.9/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18517 2024-04-26 11:02:07.000000 STAIR-tools-1.1.9/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.170111 STAIR-tools-1.1.9/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.1.9/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3013 2023-12-23 11:23:11.000000 STAIR-tools-1.1.9/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3891 2024-04-25 06:09:45.000000 STAIR-tools-1.1.9/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12324 2024-04-25 02:44:23.000000 STAIR-tools-1.1.9/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14202 2024-04-25 02:44:36.000000 STAIR-tools-1.1.9/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.172025 STAIR-tools-1.1.9/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.1.9/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.1.9/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.1.9/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-04-28 04:04:36.172719 STAIR-tools-1.1.9/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      173 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-04-28 04:04:36.000000 STAIR-tools-1.1.9/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-04-28 04:04:36.173186 STAIR-tools-1.1.9/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      426 2024-04-28 04:04:25.000000 STAIR-tools-1.1.9/setup.py
```

### Comparing `STAIR-tools-1.1.8/README.md` & `STAIR-tools-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/ABA_annotation.py` & `STAIR-tools-1.1.9/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/emb_alignment.py` & `STAIR-tools-1.1.9/STAIR/emb_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.1.9/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.1.9/STAIR/embedding/dataset_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/embedding/loss.py` & `STAIR-tools-1.1.9/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/embedding/module_ae.py` & `STAIR-tools-1.1.9/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.1.9/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.1.9/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/loc_alignment.py` & `STAIR-tools-1.1.9/STAIR/loc_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/loc_prediction.py` & `STAIR-tools-1.1.9/STAIR/loc_prediction.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/location/align_fine.py` & `STAIR-tools-1.1.9/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/location/align_init.py` & `STAIR-tools-1.1.9/STAIR/location/align_init.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/location/edge_detection.py` & `STAIR-tools-1.1.9/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/location/edge_detection1.py` & `STAIR-tools-1.1.9/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/location/transformation.py` & `STAIR-tools-1.1.9/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR/utils.py` & `STAIR-tools-1.1.9/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.1.8/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.1.9/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

