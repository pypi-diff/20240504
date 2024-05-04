# Comparing `tmp/audiolm_superfeel-2.1.3.tar.gz` & `tmp/audiolm_superfeel-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm_superfeel-2.1.3.tar", last modified: Sat May  4 11:00:27 2024, max compression
+gzip compressed data, was "audiolm_superfeel-2.1.5.tar", last modified: Sat May  4 11:05:56 2024, max compression
```

## Comparing `audiolm_superfeel-2.1.3.tar` & `audiolm_superfeel-2.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:00:27.518147 audiolm_superfeel-2.1.3/
--rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/LICENSE
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 11:00:27.517923 audiolm_superfeel-2.1.3/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/README.md
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:00:27.516800 audiolm_superfeel-2.1.3/audiolm_superfeel/
--rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/__init__.py
--rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/attend.py
--rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/audiolm_superfeel.py
--rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/data.py
--rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/encodec.py
--rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/hubert_kmeans.py
--rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/optimizer.py
--rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/soundstream.py
--rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/t5.py
--rw-r--r--   0 oseh       (501) staff       (20)    58790 2024-05-04 11:00:15.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/trainer.py
--rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/utils.py
--rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 11:00:24.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/version.py
--rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.3/audiolm_superfeel/vq_wav2vec.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:00:27.517659 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/SOURCES.txt
--rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/dependency_links.txt
--rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/requires.txt
--rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 11:00:27.000000 audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/top_level.txt
--rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 11:00:27.518196 audiolm_superfeel-2.1.3/setup.cfg
--rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.3/setup.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:05:56.038076 audiolm_superfeel-2.1.5/
+-rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.5/LICENSE
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 11:05:56.037885 audiolm_superfeel-2.1.5/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)    21070 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/README.md
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:05:56.036970 audiolm_superfeel-2.1.5/audiolm_superfeel/
+-rw-r--r--   0 oseh       (501) staff       (20)      958 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/__init__.py
+-rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/attend.py
+-rw-r--r--   0 oseh       (501) staff       (20)    79892 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/audiolm_superfeel.py
+-rw-r--r--   0 oseh       (501) staff       (20)     5120 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/data.py
+-rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/encodec.py
+-rw-r--r--   0 oseh       (501) staff       (20)     3073 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/hubert_kmeans.py
+-rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/optimizer.py
+-rw-r--r--   0 oseh       (501) staff       (20)    34453 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/soundstream.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/t5.py
+-rw-r--r--   0 oseh       (501) staff       (20)    58781 2024-05-04 11:05:06.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/trainer.py
+-rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/utils.py
+-rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 11:05:18.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/version.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2353 2024-05-04 10:29:55.000000 audiolm_superfeel-2.1.5/audiolm_superfeel/vq_wav2vec.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 11:05:56.037663 audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 11:05:56.000000 audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)      622 2024-05-04 11:05:56.000000 audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/SOURCES.txt
+-rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 11:05:56.000000 audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/dependency_links.txt
+-rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 11:05:56.000000 audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/requires.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 11:05:56.000000 audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/top_level.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 11:05:56.038114 audiolm_superfeel-2.1.5/setup.cfg
+-rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.1.5/setup.py
```

### Comparing `audiolm_superfeel-2.1.3/LICENSE` & `audiolm_superfeel-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/PKG-INFO` & `audiolm_superfeel-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.1.3
+Version: 2.1.5
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.1.3/README.md` & `audiolm_superfeel-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/__init__.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/attend.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/audiolm_superfeel.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/audiolm_superfeel.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/data.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/data.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/encodec.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/hubert_kmeans.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/optimizer.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/soundstream.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/t5.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/trainer.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 api_key = input("Enter your Weights & Biases API key: ")
 project_name = input("Enter the project name for W&B: ")
 run_name = input("Enter the run name for this session: ")
 learning_rate = float(input("Enter the learning rate: "))
 batch_size = int(input("Enter the batch size: "))
 
 wandb.login(key=api_key)
-wandb.init(project_name=project_name, run_name=run_name)
+wandb.init(project=project_name, name=run_name)
 wandb.config = {"learning_rate": learning_rate, "batch_size": batch_size}
 
 
 
 # constants
 
 DEFAULT_SAMPLE_RATE = 16000
```

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel/vq_wav2vec.py` & `audiolm_superfeel-2.1.5/audiolm_superfeel/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/PKG-INFO` & `audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.1.3
+Version: 2.1.5
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.1.3/audiolm_superfeel.egg-info/SOURCES.txt` & `audiolm_superfeel-2.1.5/audiolm_superfeel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.1.3/setup.py` & `audiolm_superfeel-2.1.5/setup.py`

 * *Files identical despite different names*

