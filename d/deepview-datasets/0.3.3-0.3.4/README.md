# Comparing `tmp/deepview_datasets-0.3.3.tar.gz` & `tmp/deepview_datasets-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepview_datasets-0.3.3.tar", last modified: Fri May  3 20:08:40 2024, max compression
+gzip compressed data, was "deepview_datasets-0.3.4.tar", last modified: Sat May  4 01:05:03 2024, max compression
```

## Comparing `deepview_datasets-0.3.3.tar` & `deepview_datasets-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34675 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/generators/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/generators/detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/readers/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/readers/pascal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.585801 deepview_datasets-0.3.3/deepview/datasets/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/writers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/deepview/datasets/writers/polars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/deepview_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 20:08:40.000000 deepview_datasets-0.3.3/deepview_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-03 20:08:36.000000 deepview_datasets-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:08:40.589801 deepview_datasets-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.395910 deepview_datasets-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34675 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-05-04 01:05:03.391910 deepview_datasets-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.387910 deepview_datasets-0.3.4/deepview/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.387910 deepview_datasets-0.3.4/deepview/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.391910 deepview_datasets-0.3.4/deepview/datasets/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/generators/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/generators/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.391910 deepview_datasets-0.3.4/deepview/datasets/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/readers/pascal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.391910 deepview_datasets-0.3.4/deepview/datasets/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/writers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/deepview/datasets/writers/polars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 01:05:03.391910 deepview_datasets-0.3.4/deepview_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41536 2024-05-04 01:05:03.000000 deepview_datasets-0.3.4/deepview_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-04 01:05:03.000000 deepview_datasets-0.3.4/deepview_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 01:05:03.000000 deepview_datasets-0.3.4/deepview_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-04 01:05:03.000000 deepview_datasets-0.3.4/deepview_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 01:05:03.000000 deepview_datasets-0.3.4/deepview_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-04 01:04:58.000000 deepview_datasets-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 01:05:03.395910 deepview_datasets-0.3.4/setup.cfg
```

### Comparing `deepview_datasets-0.3.3/LICENSE` & `deepview_datasets-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/PKG-INFO` & `deepview_datasets-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepview-datasets
-Version: 0.3.3
+Version: 0.3.4
 Summary: DeepView Datasets
 Author-email: Au-Zone Technologies <info@au-zone.com>
 License:    DUAL-LICENSED UNDER AGPL-3.0 OR DEEPVIEW AI MIDDLEWARE COMMERCIAL LICENSE
              CONTACT AU-ZONE TECHNOLOGIES <INFO@AU-ZONE.COM> FOR LICENSING DETAILS
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `deepview_datasets-0.3.3/README.md` & `deepview_datasets-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview/datasets/generators/core.py` & `deepview_datasets-0.3.4/deepview/datasets/generators/core.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview/datasets/generators/detection.py` & `deepview_datasets-0.3.4/deepview/datasets/generators/detection.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview/datasets/readers/arrow.py` & `deepview_datasets-0.3.4/deepview/datasets/readers/arrow.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview/datasets/readers/core.py` & `deepview_datasets-0.3.4/deepview/datasets/readers/core.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview/datasets/readers/darknet.py` & `deepview_datasets-0.3.4/deepview/datasets/readers/darknet.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                         self.annotations.append(ann_path)
                         ann_file = ann_path
                     else:
                         ann_file = None
                 else:
                     ann_file = join(annotations, image_name + '.txt')
                     if exists(ann_file):
-                        self.annotations.append(ann_path)
+                        self.annotations.append(ann_file)
                     else:
                         ann_file = None
                 
                 self.__storage__.append([image, ann_file])
                 self.__size__ += 1
         else:
             loop = tqdm(
```

### Comparing `deepview_datasets-0.3.3/deepview/datasets/writers/core.py` & `deepview_datasets-0.3.4/deepview/datasets/writers/core.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview/datasets/writers/polars.py` & `deepview_datasets-0.3.4/deepview/datasets/writers/polars.py`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/deepview_datasets.egg-info/PKG-INFO` & `deepview_datasets-0.3.4/deepview_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepview-datasets
-Version: 0.3.3
+Version: 0.3.4
 Summary: DeepView Datasets
 Author-email: Au-Zone Technologies <info@au-zone.com>
 License:    DUAL-LICENSED UNDER AGPL-3.0 OR DEEPVIEW AI MIDDLEWARE COMMERCIAL LICENSE
              CONTACT AU-ZONE TECHNOLOGIES <INFO@AU-ZONE.COM> FOR LICENSING DETAILS
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `deepview_datasets-0.3.3/deepview_datasets.egg-info/SOURCES.txt` & `deepview_datasets-0.3.4/deepview_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepview_datasets-0.3.3/pyproject.toml` & `deepview_datasets-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deepview-datasets"
-version = "0.3.3"
+version = "0.3.4"
 description = "DeepView Datasets"
 readme = "README.md"
 authors = [{ name = "Au-Zone Technologies", email = "info@au-zone.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

