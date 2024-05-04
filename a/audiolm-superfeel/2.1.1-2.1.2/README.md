# Comparing `tmp/audiolm_superfeel-2.1.1.tar.gz` & `tmp/audiolm_superfeel-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm_superfeel-2.1.1.tar", last modified: Sat May  4 10:34:36 2024, max compression
+gzip compressed data, was "audiolm_superfeel-2.1.2.tar", last modified: Sat May  4 10:46:52 2024, max compression
```

## Comparing `audiolm_superfeel-2.1.1.tar` & `audiolm_superfeel-2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:34:36.837712 audiolm_superfeel-2.1.1/
--rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.1/LICENSE
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:34:36.837471 audiolm_superfeel-2.1.1/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/README.md
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:34:36.836404 audiolm_superfeel-2.1.1/audiolm_superfeel/
--rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/__init__.py
--rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/attend.py
--rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/audiolm_superfeel.py
--rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/data.py
--rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/encodec.py
--rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/hubert_kmeans.py
--rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/optimizer.py
--rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/soundstream.py
--rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/t5.py
--rw-r--r--   0 oseh       (501) staff       (20)    56350 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/trainer.py
--rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/utils.py
--rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:34:33.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/version.py
--rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.1/audiolm_superfeel/vq_wav2vec.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:34:36.837145 audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:34:36.000000 audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 10:34:36.000000 audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/SOURCES.txt
--rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:34:36.000000 audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/dependency_links.txt
--rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:34:36.000000 audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/requires.txt
--rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 10:34:36.000000 audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/top_level.txt
--rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:34:36.837757 audiolm_superfeel-2.1.1/setup.cfg
--rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.1/setup.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:46:52.078182 audiolm_superfeel-2.1.2/
+-rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/LICENSE
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:46:52.077957 audiolm_superfeel-2.1.2/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/README.md
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:46:52.076988 audiolm_superfeel-2.1.2/audiolm_superfeel/
+-rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/__init__.py
+-rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/attend.py
+-rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/audiolm_superfeel.py
+-rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/data.py
+-rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/encodec.py
+-rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/hubert_kmeans.py
+-rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/optimizer.py
+-rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/soundstream.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/t5.py
+-rw-r--r--   0 oseh       (501) staff       (20)    58571 2024-05-04 10:46:35.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/trainer.py
+-rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/utils.py
+-rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:46:48.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/version.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/vq_wav2vec.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:46:52.077724 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/SOURCES.txt
+-rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/dependency_links.txt
+-rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/requires.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/top_level.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:46:52.078223 audiolm_superfeel-2.1.2/setup.cfg
+-rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.2/setup.py
```

### Comparing `audiolm_superfeel-2.1.1/LICENSE` & `audiolm_superfeel-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/PKG-INFO` & `audiolm_superfeel-2.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.1.1
+Version: 2.1.2
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.1.1/README.md` & `audiolm_superfeel-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/__init__.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/attend.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/audiolm_superfeel.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/audiolm_superfeel.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/data.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/data.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/encodec.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/hubert_kmeans.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/optimizer.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/soundstream.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/t5.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/trainer.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -927,28 +927,42 @@
         if not exists(self.ds_fields):
             self.ds_fields = determine_types(data, DATASET_FIELD_TYPE_CONFIG)
             assert not has_duplicates(self.ds_fields), 'dataset fields must not have duplicate field names'
 
         return dict(zip(self.ds_fields, data))
 
     @contextmanager
-    def wandb_tracker(self, project, run = None, hps = None):
-        assert self.use_wandb_tracking, '`use_wandb_tracking` must be set to True on SemanticTransformerTrainer'
-
-        hps = default(hps, self.tracker_hps)
-
-        self.accelerator.init_trackers(project, config = None)
-
-        if exists(run):
-            wandb_tracker = find_first(lambda el: isinstance(el, WandBTracker), self.accelerator.trackers)
-            assert exists(wandb_tracker)
-
+    def wandb_tracker(self, project=None, run=None, hps=None):
+        # Get W&B parameters from the user if not provided
+        if not project:
+            project = input("Enter the project name for W&B: ")
+        if not run:
+            run = input("Enter the run name for this session: ")
+        if not hps:
+            learning_rate = float(input("Enter the learning rate: "))
+            batch_size = int(input("Enter the batch size: "))
+            hps = {"learning_rate": learning_rate, "batch_size": batch_size}
+
+        assert self.use_wandb_tracking, '`use_wandb_tracking` must be set to True on SoundStreamTrainer'
+
+        # Ensure W&B API key is set
+        if "WANDB_API_KEY" not in os.environ:
+            api_key = input("Enter your Weights & Biases API key: ")
+            wandb.login(key=api_key)
+
+        hps = self.default(hps, self.tracker_hps)
+        
+        self.accelerator.init_trackers(project, config=hps)
+        
+        if run:
+            wandb_tracker = next((el for el in self.accelerator.trackers if isinstance(el, WandBTracker)), None)
+            assert wandb_tracker, "WandBTracker not found."
             wandb_tracker.run.name = run
 
-        yield
+        yield wandb_tracker  # Yield the tracker for use in the with block
 
         self.accelerator.end_training()
 
     def train_step(self):
         device = self.device
 
         steps = int(self.steps.item())
@@ -1206,30 +1220,44 @@
     def print(self, msg):
         self.accelerator.print(msg)
 
     def generate(self, *args, **kwargs):
         return self.train_wrapper.generate(*args, **kwargs)
 
     @contextmanager
-    def wandb_tracker(self, project, run = None, hps = None):
-        assert self.use_wandb_tracking, '`use_wandb_tracking` must be set to True on CoarseTransformerTrainer'
-
-        hps = default(hps, self.tracker_hps)
-
-        self.accelerator.init_trackers(project, config = None)
-
-        if exists(run):
-            wandb_tracker = find_first(lambda el: isinstance(el, WandBTracker), self.accelerator.trackers)
-            assert exists(wandb_tracker)
-
+    def wandb_tracker(self, project=None, run=None, hps=None):
+        # Get W&B parameters from the user if not provided
+        if not project:
+            project = input("Enter the project name for W&B: ")
+        if not run:
+            run = input("Enter the run name for this session: ")
+        if not hps:
+            learning_rate = float(input("Enter the learning rate: "))
+            batch_size = int(input("Enter the batch size: "))
+            hps = {"learning_rate": learning_rate, "batch_size": batch_size}
+
+        assert self.use_wandb_tracking, '`use_wandb_tracking` must be set to True on SoundStreamTrainer'
+
+        # Ensure W&B API key is set
+        if "WANDB_API_KEY" not in os.environ:
+            api_key = input("Enter your Weights & Biases API key: ")
+            wandb.login(key=api_key)
+
+        hps = self.default(hps, self.tracker_hps)
+        
+        self.accelerator.init_trackers(project, config=hps)
+        
+        if run:
+            wandb_tracker = next((el for el in self.accelerator.trackers if isinstance(el, WandBTracker)), None)
+            assert wandb_tracker, "WandBTracker not found."
             wandb_tracker.run.name = run
 
-        yield
+        yield wandb_tracker  # Yield the tracker for use in the with block
 
-        self.accelerator.end_training()  
+        self.accelerator.end_training() 
 
     @property
     def device(self):
         return self.accelerator.device
 
     @property
     def is_distributed(self):
@@ -1503,30 +1531,44 @@
     def print(self, msg):
         self.accelerator.print(msg)
 
     def generate(self, *args, **kwargs):
         return self.train_wrapper.generate(*args, **kwargs)
 
     @contextmanager
-    def wandb_tracker(self, project, run = None, hps = None):
-        assert self.use_wandb_tracking, '`use_wandb_tracking` must be set to True on FineTransformerTrainer'
-
-        hps = default(hps, self.tracker_hps)
-
-        self.accelerator.init_trackers(project, config = None)
-
-        if exists(run):
-            wandb_tracker = find_first(lambda el: isinstance(el, WandBTracker), self.accelerator.trackers)
-            assert exists(wandb_tracker)
-
+    def wandb_tracker(self, project=None, run=None, hps=None):
+        # Get W&B parameters from the user if not provided
+        if not project:
+            project = input("Enter the project name for W&B: ")
+        if not run:
+            run = input("Enter the run name for this session: ")
+        if not hps:
+            learning_rate = float(input("Enter the learning rate: "))
+            batch_size = int(input("Enter the batch size: "))
+            hps = {"learning_rate": learning_rate, "batch_size": batch_size}
+
+        assert self.use_wandb_tracking, '`use_wandb_tracking` must be set to True on SoundStreamTrainer'
+
+        # Ensure W&B API key is set
+        if "WANDB_API_KEY" not in os.environ:
+            api_key = input("Enter your Weights & Biases API key: ")
+            wandb.login(key=api_key)
+
+        hps = self.default(hps, self.tracker_hps)
+        
+        self.accelerator.init_trackers(project, config=hps)
+        
+        if run:
+            wandb_tracker = next((el for el in self.accelerator.trackers if isinstance(el, WandBTracker)), None)
+            assert wandb_tracker, "WandBTracker not found."
             wandb_tracker.run.name = run
 
-        yield
+        yield wandb_tracker  # Yield the tracker for use in the with block
 
-        self.accelerator.end_training() 
+        self.accelerator.end_training()
 
     @property
     def device(self):
         return self.accelerator.device
 
     @property
     def is_distributed(self):
```

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel/vq_wav2vec.py` & `audiolm_superfeel-2.1.2/audiolm_superfeel/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/PKG-INFO` & `audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.1.1
+Version: 2.1.2
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.1.1/audiolm_superfeel.egg-info/SOURCES.txt` & `audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.1/setup.py` & `audiolm_superfeel-2.1.2/setup.py`

 * *Files identical despite different names*

