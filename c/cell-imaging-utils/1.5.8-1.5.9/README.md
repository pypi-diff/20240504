# Comparing `tmp/cell_imaging_utils-1.5.8.tar.gz` & `tmp/cell_imaging_utils-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cell_imaging_utils-1.5.8.tar", last modified: Sat Nov 13 15:57:46 2021, max compression
+gzip compressed data, was "dist\cell_imaging_utils-1.5.9.tar", last modified: Wed Dec 22 11:49:21 2021, max compression
```

## Comparing `cell_imaging_utils-1.5.8.tar` & `cell_imaging_utils-1.5.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.701760 cell_imaging_utils-1.5.8/
--rw-rw-rw-   0        0        0     1093 2021-05-05 13:23:19.000000 cell_imaging_utils-1.5.8/LICENSE
--rw-rw-rw-   0        0        0      915 2021-11-13 15:57:46.699767 cell_imaging_utils-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      429 2021-05-05 13:28:23.000000 cell_imaging_utils-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.649899 cell_imaging_utils-1.5.8/cell_imaging_utils/
--rw-rw-rw-   0        0        0      411 2021-05-08 11:15:13.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.675832 cell_imaging_utils-1.5.8/cell_imaging_utils/data_structures/
--rw-rw-rw-   0        0        0      320 2021-05-05 13:24:25.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/data_structures/__init__.py
--rw-rw-rw-   0        0        0      327 2021-05-07 19:00:06.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/data_structures/singleton.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.677824 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/
--rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/__init__.py
--rw-rw-rw-   0        0        0      848 2021-11-09 13:12:05.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/datasetes_metadata_abstract.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.681814 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/dict/
--rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/dict/__init__.py
--rw-rw-rw-   0        0        0      709 2021-05-08 11:15:22.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_abstract_dict.py
--rw-rw-rw-   0        0        0      746 2021-06-02 08:24:27.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_pickle.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.686857 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/table/
--rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/table/__init__.py
--rw-rw-rw-   0        0        0     2445 2021-11-09 09:52:59.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_abstract_table.py
--rw-rw-rw-   0        0        0      773 2021-05-08 14:24:01.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_csv.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.689794 cell_imaging_utils-1.5.8/cell_imaging_utils/image/
--rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/image/__init__.py
--rw-rw-rw-   0        0        0     4528 2021-11-13 15:56:38.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/image/image_utils.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.692786 cell_imaging_utils-1.5.8/cell_imaging_utils/plots/
--rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/plots/__init__.py
--rw-rw-rw-   0        0        0      790 2021-07-06 19:47:54.000000 cell_imaging_utils-1.5.8/cell_imaging_utils/plots/plot_utils.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.672840 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/
--rw-rw-rw-   0        0        0      915 2021-11-13 15:57:46.000000 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2021-11-13 15:57:46.000000 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-13 15:57:46.000000 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-05-05 13:27:06.000000 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      136 2021-11-13 15:57:46.000000 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2021-11-13 15:57:46.000000 cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-13 15:57:46.701861 cell_imaging_utils-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1020 2021-11-13 15:57:45.000000 cell_imaging_utils-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-13 15:57:46.698778 cell_imaging_utils-1.5.8/tests/
--rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1511 2021-05-08 14:08:19.000000 cell_imaging_utils-1.5.8/tests/test_datasets_metadata.py
--rw-rw-rw-   0        0        0     1373 2021-05-08 17:47:57.000000 cell_imaging_utils-1.5.8/tests/test_image_utils.py
--rw-rw-rw-   0        0        0     2103 2021-07-07 12:49:55.000000 cell_imaging_utils-1.5.8/tests/test_plot_utils.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.662987 cell_imaging_utils-1.5.9/
+-rw-rw-rw-   0        0        0     1093 2021-05-05 13:23:19.000000 cell_imaging_utils-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0      915 2021-12-22 11:49:21.661989 cell_imaging_utils-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2021-05-05 13:28:23.000000 cell_imaging_utils-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.508010 cell_imaging_utils-1.5.9/cell_imaging_utils/
+-rw-rw-rw-   0        0        0      411 2021-05-08 11:15:13.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.563807 cell_imaging_utils-1.5.9/cell_imaging_utils/data_structures/
+-rw-rw-rw-   0        0        0      320 2021-05-05 13:24:25.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      327 2021-05-07 19:00:06.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/data_structures/singleton.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.573780 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/
+-rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/__init__.py
+-rw-rw-rw-   0        0        0      848 2021-11-09 13:12:05.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/datasetes_metadata_abstract.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.592709 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/dict/
+-rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/dict/__init__.py
+-rw-rw-rw-   0        0        0      709 2021-05-08 11:15:22.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_abstract_dict.py
+-rw-rw-rw-   0        0        0      746 2021-06-02 08:24:27.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_pickle.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.612656 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/table/
+-rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/table/__init__.py
+-rw-rw-rw-   0        0        0     2445 2021-11-09 09:52:59.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_abstract_table.py
+-rw-rw-rw-   0        0        0      773 2021-05-08 14:24:01.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_csv.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.623064 cell_imaging_utils-1.5.9/cell_imaging_utils/image/
+-rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/image/__init__.py
+-rw-rw-rw-   0        0        0     4866 2021-12-22 09:02:13.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/image/image_utils.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.631039 cell_imaging_utils-1.5.9/cell_imaging_utils/plots/
+-rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/plots/__init__.py
+-rw-rw-rw-   0        0        0      790 2021-07-06 19:47:54.000000 cell_imaging_utils-1.5.9/cell_imaging_utils/plots/plot_utils.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.541865 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/
+-rw-rw-rw-   0        0        0      915 2021-12-22 11:49:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2021-12-22 11:49:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-22 11:49:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-05-05 13:27:06.000000 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      136 2021-12-22 11:49:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2021-12-22 11:49:21.000000 cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-12-22 11:49:21.662987 cell_imaging_utils-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2021-12-22 11:49:20.000000 cell_imaging_utils-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-22 11:49:21.660994 cell_imaging_utils-1.5.9/tests/
+-rw-rw-rw-   0        0        0        0 2021-04-28 21:53:21.000000 cell_imaging_utils-1.5.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1511 2021-05-08 14:08:19.000000 cell_imaging_utils-1.5.9/tests/test_datasets_metadata.py
+-rw-rw-rw-   0        0        0     1373 2021-05-08 17:47:57.000000 cell_imaging_utils-1.5.9/tests/test_image_utils.py
+-rw-rw-rw-   0        0        0     2103 2021-07-07 12:49:55.000000 cell_imaging_utils-1.5.9/tests/test_plot_utils.py
```

### Comparing `cell_imaging_utils-1.5.8/LICENSE` & `cell_imaging_utils-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/PKG-INFO` & `cell_imaging_utils-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell_imaging_utils
-Version: 1.5.8
+Version: 1.5.9
 Summary: UNKNOWN
 Home-page: https://github.com/lionben89/BGU_cell_imaging_utils
 Author: Lion Ben Nedava
 Author-email: lionben89@gmail.com
 License: MIT
 Description: # BGU-cell-imaging-utils
```

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/datasetes_metadata_abstract.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/datasetes_metadata_abstract.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_abstract_dict.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_abstract_dict.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_pickle.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/dict/datasetes_metadata_pickle.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_abstract_table.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_abstract_table.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_csv.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/datasets_metadata/table/datasetes_metadata_csv.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/image/image_utils.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/image/image_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,17 +108,24 @@
             
         if (x_pad >= 0):        
             scaled_a = np.pad(scaled_a,((0,0),(0,0),(0,0),(x_pad//2, x_pad//2 + x_pad%2)),mode = 'constant')
         else:
             scaled_a = scaled_a[:,:,:,abs(x_pad//2):scaled_a.shape[3]+(x_pad//2 + x_pad%2)]                        
         return scaled_a
     
-    # @staticmethod
-    # def clean_by_slice(image_ndarray:np.ndarray, leave_percentage:float)->np.ndarray:
-    #     sum_values
+    @staticmethod
+    def slice_image(image_ndarray:np.ndarray, x_idx:tuple,y_idx:tuple,z_idx:tuple)->np.ndarray:
+        n_dim = len(image_ndarray.shape)
+        slices = [slice(None)] * n_dim
+        slices[n_dim - 3] = slice(x_idx[0], x_idx[1])
+        slices[n_dim - 2] = slice(y_idx[0], y_idx[1])
+        slices[n_dim - 1] = slice(z_idx[0], z_idx[1])
+        slices = tuple(slices)
+        sliced_image = image_ndarray[slices]
+        return sliced_image
     
     """
     mask_image gets image and mask_template it masks the image according to the template and duplicate it accordingly
     """
     @staticmethod
     def mask_image(image_ndarray,mask_template_ndarray) -> np.ndarray:
         mask_ndarray = mask_template_ndarray
```

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils/plots/plot_utils.py` & `cell_imaging_utils-1.5.9/cell_imaging_utils/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/PKG-INFO` & `cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-imaging-utils
-Version: 1.5.8
+Version: 1.5.9
 Summary: UNKNOWN
 Home-page: https://github.com/lionben89/BGU_cell_imaging_utils
 Author: Lion Ben Nedava
 Author-email: lionben89@gmail.com
 License: MIT
 Description: # BGU-cell-imaging-utils
```

### Comparing `cell_imaging_utils-1.5.8/cell_imaging_utils.egg-info/SOURCES.txt` & `cell_imaging_utils-1.5.9/cell_imaging_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/setup.py` & `cell_imaging_utils-1.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = '1.5.8'
+__version__ = '1.5.9'
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 requirements = [
     "matplotlib",
     "numpy",
```

### Comparing `cell_imaging_utils-1.5.8/tests/test_datasets_metadata.py` & `cell_imaging_utils-1.5.9/tests/test_datasets_metadata.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/tests/test_image_utils.py` & `cell_imaging_utils-1.5.9/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `cell_imaging_utils-1.5.8/tests/test_plot_utils.py` & `cell_imaging_utils-1.5.9/tests/test_plot_utils.py`

 * *Files identical despite different names*

