# Comparing `tmp/dataset_iterator-0.4.2.tar.gz` & `tmp/dataset_iterator-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.4.2.tar", last modified: Mon Apr 29 15:50:22 2024, max compression
+gzip compressed data, was "dataset_iterator-0.4.3.tar", last modified: Fri May  3 22:15:51 2024, max compression
```

## Comparing `dataset_iterator-0.4.2.tar` & `dataset_iterator-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/dataset_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/concat_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/dataset_iterator/datasetIO/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/group_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/h5pyIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/memoryIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/hard_sample_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/image_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/index_array_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    58005 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/multichannel_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/ordered_enqueuer_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/tile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/tracking_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/dataset_iterator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/dataset_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 15:50:22.000000 dataset_iterator-0.4.2/dataset_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:50:22.924105 dataset_iterator-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-29 15:50:19.000000 dataset_iterator-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.444933 dataset_iterator-0.4.3/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58005 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/ordered_enqueuer_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/setup.py
```

### Comparing `dataset_iterator-0.4.2/LICENSE.txt` & `dataset_iterator-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/PKG-INFO` & `dataset_iterator-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.2
+Version: 0.4.3
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.2/dataset_iterator-0.4.2.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.3/dataset_iterator-0.4.3.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.2/README.md` & `dataset_iterator-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/__init__.py` & `dataset_iterator-0.4.3/dataset_iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.4.3/dataset_iterator/concat_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/memoryIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/memoryIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/hard_sample_mining.py` & `dataset_iterator-0.4.3/dataset_iterator/hard_sample_mining.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import numpy as np
 import tensorflow as tf
 from .index_array_iterator import IndexArrayIterator, INCOMPLETE_LAST_BATCH_MODE
 from dataset_iterator.ordered_enqueuer_cf import OrderedEnqueuerCF
 import threading
 
 class HardSampleMiningCallback(tf.keras.callbacks.Callback):
-    def __init__(self, iterator, target_iterator, predict_fun, metrics_fun, period:int=10, start_epoch:int=0, skip_first:bool=False, start_from_epoch:int=0, enrich_factor:float=10., quantile_max:float=0.99, quantile_min:float=None, disable_channel_postprocessing:bool=False, workers=None, verbose:int=1):
+    def __init__(self, iterator, target_iterator, predict_fun, metrics_fun, period:int=10, start_epoch:int=0, start_from_epoch:int=0, enrich_factor:float=10., quantile_max:float=0.99, quantile_min:float=None, disable_channel_postprocessing:bool=False, workers=None, verbose:int=1):
         super().__init__()
         self.period = period
         self.start_epoch = start_epoch
         self.start_from_epoch = start_from_epoch
-        self.skip_first = skip_first
         self.iterator = iterator
         self.target_iterator = target_iterator
         self.predict_fun = predict_fun
         self.metrics_fun = metrics_fun
         self.enrich_factor = enrich_factor
         self.quantile_max = quantile_max
         self.quantile_min = quantile_min
@@ -28,47 +27,51 @@
         self.n_metrics = 0
         self.data_aug_param = self.iterator.disable_random_transforms(True, self.disable_channel_postprocessing)
         simple_iterator = SimpleIterator(self.iterator)
         self.batch_size = self.iterator.get_batch_size()
         self.n_batches = len(simple_iterator)
         self.enq = OrderedEnqueuerCF(simple_iterator, single_epoch=True, shuffle=False)
         self.wait_for_me = threading.Event()
+        self.wait_for_me.set()
 
     def close(self):
         self.enq.stop()
         if self.data_aug_param is not None:
             self.iterator.enable_random_transforms(self.data_aug_param)
         self.iterator.close()
 
+    def need_compute(self, epoch):
+        return epoch + 1 + self.start_epoch >= self.start_from_epoch and (self.period == 1 or (epoch + 1 + self.start_epoch - self.start_from_epoch) % self.period == 0)
+
     def on_epoch_begin(self, epoch, logs=None):
-        if self.proba_per_metric is not None:
-            self.wait_for_me.clear() # will block
+        if self.proba_per_metric is not None or self.need_compute(epoch):
+            self.wait_for_me.clear()  # will lock
 
     def on_epoch_end(self, epoch, logs=None):
-        if self.period == 1 or (epoch + 1 + self.start_epoch) % self.period == 0:
-            if (epoch > 0 or not self.skip_first) and epoch + 1 + self.start_epoch >= self.start_from_epoch:
+        if self.need_compute(epoch):
+            if self.target_iterator is not self.iterator:
                 self.target_iterator.close()
                 self.iterator.open()
-                metrics = self.compute_metrics()
+            metrics = self.compute_metrics()
+            if self.target_iterator is not self.iterator:
                 self.iterator.close()
                 self.target_iterator.open()
-                first = self.proba_per_metric is None
-                self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
-                self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
-                if first and self.n_metrics > self.period:
-                    warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
+            first = self.proba_per_metric is None
+            self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
+            self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
+            if first and self.n_metrics > self.period:
+                warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
         if self.proba_per_metric is not None:
             if len(self.proba_per_metric.shape) == 2:
                 self.metric_idx = (self.metric_idx + 1) % self.n_metrics
                 proba = self.proba_per_metric[self.metric_idx]
             else:
                 proba = self.proba_per_metric
-            # set probability to iterator in case of multiprocessing iwth OrderedEnqueeur this will be taken into account only a next epoch has iterator has already been sent to processes at this stage
             self.target_iterator.set_index_probability(proba)
-            self.wait_for_me.set() # release block
+            self.wait_for_me.set()  # release lock
 
     def on_train_end(self, logs=None):
         self.close()
 
     def compute_metrics(self):
         workers = os.cpu_count() if self.workers is None else self.workers
         self.enq.start(workers=workers, max_queue_size=max(2, min(self.n_batches, workers)))
```

### Comparing `dataset_iterator-0.4.2/dataset_iterator/helpers.py` & `dataset_iterator-0.4.3/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.4.3/dataset_iterator/image_data_generator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.4.3/dataset_iterator/index_array_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.4.3/dataset_iterator/multichannel_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/ordered_enqueuer_cf.py` & `dataset_iterator-0.4.3/dataset_iterator/ordered_enqueuer_cf.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/pre_processing.py` & `dataset_iterator-0.4.3/dataset_iterator/pre_processing.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/shared_memory.py` & `dataset_iterator-0.4.3/dataset_iterator/shared_memory.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/tile_utils.py` & `dataset_iterator-0.4.3/dataset_iterator/tile_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.4.3/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator/utils.py` & `dataset_iterator-0.4.3/dataset_iterator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.4.3/dataset_iterator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.2
+Version: 0.4.3
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.2/dataset_iterator-0.4.2.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.3/dataset_iterator-0.4.3.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.2/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.4.3/dataset_iterator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.2/setup.py` & `dataset_iterator-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.4.2",
+    version="0.4.3",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.2/dataset_iterator-0.4.2.tar.gz',
+    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.3/dataset_iterator-0.4.3.tar.gz',
     keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

