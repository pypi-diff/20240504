# Comparing `tmp/meta-reid-3.9.24.tar.gz` & `tmp/meta-reid-3.9.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-reid-3.9.24.tar", last modified: Sat Oct  7 08:37:42 2023, max compression
+gzip compressed data, was "dist/meta-reid-3.9.25.tar", last modified: Sat May  4 14:47:39 2024, max compression
```

## Comparing `meta-reid-3.9.24.tar` & `meta-reid-3.9.25.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-10-07 08:37:42.000000 meta-reid-3.9.24/
--rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-10-07 08:37:42.000000 meta-reid-3.9.24/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-03-13 10:34:15.000000 meta-reid-3.9.24/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      277 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      499 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       69 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-10-07 08:37:42.000000 meta-reid-3.9.24/meta_reid.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-10-07 08:37:42.000000 meta-reid-3.9.24/metareid/
--rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-03-14 03:19:31.000000 meta-reid-3.9.24/metareid/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-10-07 08:37:42.000000 meta-reid-3.9.24/metareid/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       83 2023-03-14 03:19:10.000000 meta-reid-3.9.24/metareid/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-03-20 06:12:28.000000 meta-reid-3.9.24/metareid/app/onnx_to_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6026 2023-10-07 08:07:44.000000 meta-reid-3.9.24/metareid/app/reid_inference_trt.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-10-07 08:37:42.000000 meta-reid-3.9.24/metareid/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)       60 2023-03-20 06:14:45.000000 meta-reid-3.9.24/metareid/model_zoo/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4789 2023-04-11 04:01:10.000000 meta-reid-3.9.24/metareid/model_zoo/trt_engine.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    12524 2023-06-12 03:26:09.000000 meta-reid-3.9.24/metareid/model_zoo/trt_export.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-10-07 08:37:42.000000 meta-reid-3.9.24/metareid/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       50 2023-03-20 06:14:05.000000 meta-reid-3.9.24/metareid/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      608 2023-03-20 01:47:13.000000 meta-reid-3.9.24/metareid/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-reid-3.9.24/metareid/utils/image_batch.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-10-07 08:37:42.000000 meta-reid-3.9.24/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      712 2023-10-07 08:37:22.000000 meta-reid-3.9.24/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2024-05-04 14:47:39.000000 meta-reid-3.9.25/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      277 2024-05-04 14:47:39.000000 meta-reid-3.9.25/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-03-13 10:34:15.000000 meta-reid-3.9.25/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      277 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      499 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       59 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2024-05-04 14:47:39.000000 meta-reid-3.9.25/meta_reid.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2024-05-04 14:47:39.000000 meta-reid-3.9.25/metareid/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-03-14 03:19:31.000000 meta-reid-3.9.25/metareid/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2024-05-04 14:47:39.000000 meta-reid-3.9.25/metareid/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       83 2023-03-14 03:19:10.000000 meta-reid-3.9.25/metareid/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-03-20 06:12:28.000000 meta-reid-3.9.25/metareid/app/onnx_to_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6510 2024-05-04 14:33:47.000000 meta-reid-3.9.25/metareid/app/reid_inference_trt.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2024-05-04 14:47:39.000000 meta-reid-3.9.25/metareid/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       60 2023-03-20 06:14:45.000000 meta-reid-3.9.25/metareid/model_zoo/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4789 2023-04-11 04:01:10.000000 meta-reid-3.9.25/metareid/model_zoo/trt_engine.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    12524 2023-06-12 03:26:09.000000 meta-reid-3.9.25/metareid/model_zoo/trt_export.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2024-05-04 14:47:39.000000 meta-reid-3.9.25/metareid/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       50 2023-03-20 06:14:05.000000 meta-reid-3.9.25/metareid/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      608 2023-03-20 01:47:13.000000 meta-reid-3.9.25/metareid/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-reid-3.9.25/metareid/utils/image_batch.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2024-05-04 14:47:39.000000 meta-reid-3.9.25/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      696 2024-05-04 14:42:05.000000 meta-reid-3.9.25/setup.py
```

### Comparing `meta-reid-3.9.24/metareid/app/onnx_to_trt.py` & `meta-reid-3.9.25/metareid/app/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.9.24/metareid/app/reid_inference_trt.py` & `meta-reid-3.9.25/metareid/app/reid_inference_trt.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,18 +90,22 @@
         if len(self.query_names) > idx:
             self.query_files = self.query_files[idx + 1:]
             self.query_names = self.query_names[idx + 1:]
             self.query_features = self.query_features[idx + 1:]
             self.query_images = self.query_images[idx + 1:]
 
     def save_features(self):
-        np.save(self.query_file_path, self.query_files)
-        np.save(self.query_name_path, self.query_names)
-        np.save(self.query_feature_path, self.query_features)
-        np.save(self.query_image_path, self.query_images)
+        np.save(self.query_image_path.replace('.npy', '.npy.tmp'), self.query_images)
+        os.replace(self.query_image_path.replace('.npy', '.npy.tmp'), self.query_image_path)
+        np.save(self.query_file_path.replace('.npy', '.npy.tmp'), self.query_files)
+        os.replace(self.query_file_path.replace('.npy', '.npy.tmp'), self.query_file_path)
+        np.save(self.query_name_path.replace('.npy', '.npy.tmp'), self.query_names)
+        os.replace(self.query_name_path.replace('.npy', '.npy.tmp'), self.query_name_path)
+        np.save(self.query_feature_path.replace('.npy', '.npy.tmp'), self.query_features)
+        os.replace(self.query_feature_path.replace('.npy', '.npy.tmp'), self.query_feature_path)
 
     def save_folder(self, img_dir):
         query_name = img_dir.split('/')[-1]
         img_files = list_files(img_dir, "*.jpg")
         for img_file in tqdm.tqdm(img_files):
             query_image = cv2.imread(img_file)[:, :, ::-1]
             query_feature = self.predict(query_image)
```

### Comparing `meta-reid-3.9.24/metareid/model_zoo/trt_engine.py` & `meta-reid-3.9.25/metareid/model_zoo/trt_engine.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.9.24/metareid/model_zoo/trt_export.py` & `meta-reid-3.9.25/metareid/model_zoo/trt_export.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.9.24/metareid/utils/general.py` & `meta-reid-3.9.25/metareid/utils/general.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.9.24/metareid/utils/image_batch.py` & `meta-reid-3.9.25/metareid/utils/image_batch.py`

 * *Files identical despite different names*

### Comparing `meta-reid-3.9.24/setup.py` & `meta-reid-3.9.25/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,17 @@
     'opencv-python',
     'setuptools',
     'tensorrt',
     'pycuda',
     'numpy',
     'pillow',
     'tqdm',
-    'faiss-gpu'
 ]
 
-__version__ = 'V3.09.24'
+__version__ = 'V3.09.25'
 
 setup(
     name='meta-reid',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

