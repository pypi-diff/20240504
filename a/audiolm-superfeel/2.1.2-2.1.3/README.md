# Comparing `tmp/audiolm_superfeel-2.1.2.tar.gz` & `tmp/audiolm_superfeel-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm_superfeel-2.1.2.tar", last modified: Sat May  4 10:46:52 2024, max compression
+gzip compressed data, was "audiolm_superfeel-2.1.3.tar", last modified: Sat May  4 11:00:27 2024, max compression
```

## Comparing `audiolm_superfeel-2.1.2.tar` & `audiolm_superfeel-2.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:46:52.078182 audiolm_superfeel-2.1.2/
--rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/LICENSE
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:46:52.077957 audiolm_superfeel-2.1.2/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/README.md
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:46:52.076988 audiolm_superfeel-2.1.2/audiolm_superfeel/
--rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/__init__.py
--rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/attend.py
--rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/audiolm_superfeel.py
--rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/data.py
--rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/encodec.py
--rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/hubert_kmeans.py
--rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/optimizer.py
--rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/soundstream.py
--rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/t5.py
--rw-r--r--   0 oseh       (501) staff       (20)    58571 2024-05-04 10:46:35.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/trainer.py
--rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/utils.py
--rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:46:48.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/version.py
--rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.2/audiolm_superfeel/vq_wav2vec.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:46:52.077724 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/SOURCES.txt
--rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/dependency_links.txt
--rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/requires.txt
--rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 10:46:52.000000 audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/top_level.txt
--rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:46:52.078223 audiolm_superfeel-2.1.2/setup.cfg
--rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.2/setup.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:00:27.518147 audiolm_superfeel-2.1.3/
+-rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/LICENSE
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 11:00:27.517923 audiolm_superfeel-2.1.3/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/README.md
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:00:27.516800 audiolm_superfeel-2.1.3/audiolm_superfeel/
+-rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/__init__.py
+-rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/attend.py
+-rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/audiolm_superfeel.py
+-rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/data.py
+-rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/encodec.py
+-rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/hubert_kmeans.py
+-rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/optimizer.py
+-rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/soundstream.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/t5.py
+-rw-r--r--   0 oseh       (501) staff       (20)    58790 2024-05-04 11:00:15.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/trainer.py
+-rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/utils.py
+-rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 11:00:24.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/version.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/vq_wav2vec.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:00:27.517659 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/SOURCES.txt
+-rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/dependency_links.txt
+-rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/requires.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/top_level.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 11:00:27.518196 audiolm_superfeel-2.1.3/setup.cfg
+-rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.3/setup.py
```

### Comparing `audiolm_superfeel-2.1.2/LICENSE` & `audiolm_superfeel-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/PKG-INFO` & `audiolm_superfeel-2.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.1.2
+Version: 2.1.3
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.1.2/README.md` & `audiolm_superfeel-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/__init__.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/attend.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/audiolm_superfeel.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/audiolm_superfeel.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/data.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/data.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/encodec.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/hubert_kmeans.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/optimizer.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/soundstream.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/t5.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/trainer.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 api_key = input("Enter your Weights & Biases API key: ")
 project_name = input("Enter the project name for W&B: ")
 run_name = input("Enter the run name for this session: ")
 learning_rate = float(input("Enter the learning rate: "))
 batch_size = int(input("Enter the batch size: "))
 
 wandb.login(key=api_key)
+wandb.init(project_name=project_name, run_name=run_name)
+wandb.config = {"learning_rate": learning_rate, "batch_size": batch_size}
+
 
 
 # constants
 
 DEFAULT_SAMPLE_RATE = 16000
 
 ConstantLRScheduler = partial(LambdaLR, lr_lambda = lambda step: 1.)
@@ -657,15 +660,14 @@
 
         self.discr_optim.step()
 
         for name, multiscale_discr_optim in self.multiscale_discriminator_optim_iter():
             multiscale_discr_optim.step()
 
         # build pretty printed losses
-
         losses_str = f"{steps}: soundstream total loss: {logs['loss']:.3f}, soundstream recon loss: {logs['recon_loss']:.3f}"
 
         if log_losses:
             self.log(**logs)
 
         for key, loss in logs.items():
             if not key.startswith('scale:'):
@@ -676,14 +678,15 @@
 
             if log_losses:
                 self.log(**{f"discr_loss (scale {scale_factor})": loss})
 
         # log
 
         self.print(losses_str)
+        wandb.log({"loss": f"{logs['loss']:.3f}", "step": steps})
 
         # update exponential moving averaged generator
 
         self.accelerator.wait_for_everyone()
 
         if self.is_main and self.use_ema:
             self.ema_soundstream.update()
@@ -729,15 +732,15 @@
         return logs
 
     def train(self, log_fn = noop):
 
         while self.steps < self.num_train_steps:
             logs = self.train_step()
             log_fn(logs)
-
+        wandb.finish()
         self.print('training complete')
 
 # semantic transformer trainer
 
 class SemanticTransformerTrainer(nn.Module):
     @beartype
     def __init__(
```

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel/vq_wav2vec.py` & `audiolm_superfeel-2.1.3/audiolm_superfeel/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/PKG-INFO` & `audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.1.2
+Version: 2.1.3
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.1.2/audiolm_superfeel.egg-info/SOURCES.txt` & `audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.2/setup.py` & `audiolm_superfeel-2.1.3/setup.py`

 * *Files identical despite different names*

