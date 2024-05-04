# Comparing `tmp/audiolm_superfeel-2.0.8.tar.gz` & `tmp/audiolm_superfeel-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm_superfeel-2.0.8.tar", last modified: Sat May  4 10:17:20 2024, max compression
+gzip compressed data, was "audiolm_superfeel-2.0.9.tar", last modified: Sat May  4 10:22:29 2024, max compression
```

## Comparing `audiolm_superfeel-2.0.8.tar` & `audiolm_superfeel-2.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:17:20.150017 audiolm_superfeel-2.0.8/
--rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/LICENSE
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:17:20.149807 audiolm_superfeel-2.0.8/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)    21052 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/README.md
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:17:20.148836 audiolm_superfeel-2.0.8/audiolm_pytorch/
--rw-r--r--   0 oseh       (501) staff       (20)      932 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/__init__.py
--rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/attend.py
--rw-r--r--   0 oseh       (501) staff       (20)    79876 2024-05-04 10:14:52.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 oseh       (501) staff       (20)     5118 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/data.py
--rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/encodec.py
--rw-r--r--   0 oseh       (501) staff       (20)     3071 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/optimizer.py
--rw-r--r--   0 oseh       (501) staff       (20)    34449 2024-05-04 10:14:50.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/soundstream.py
--rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/t5.py
--rw-r--r--   0 oseh       (501) staff       (20)    56334 2024-05-04 10:14:55.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/trainer.py
--rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/utils.py
--rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:02:28.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/version.py
--rw-r--r--   0 oseh       (501) staff       (20)     2351 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.8/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:17:20.149564 audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/
--rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:17:20.000000 audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)      594 2024-05-04 10:17:20.000000 audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/SOURCES.txt
--rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:17:20.000000 audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/dependency_links.txt
--rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:17:20.000000 audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/requires.txt
--rw-r--r--   0 oseh       (501) staff       (20)       16 2024-05-04 10:17:20.000000 audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/top_level.txt
--rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:17:20.150056 audiolm_superfeel-2.0.8/setup.cfg
--rw-r--r--   0 oseh       (501) staff       (20)     1315 2024-05-04 10:14:23.000000 audiolm_superfeel-2.0.8/setup.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:22:29.105960 audiolm_superfeel-2.0.9/
+-rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/LICENSE
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:22:29.105803 audiolm_superfeel-2.0.9/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)    21052 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/README.md
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:22:29.104908 audiolm_superfeel-2.0.9/audiolm_superfeel/
+-rw-r--r--   0 oseh       (501) staff       (20)      932 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/__init__.py
+-rw-r--r--   0 oseh       (501) staff       (20)     4170 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/attend.py
+-rw-r--r--   0 oseh       (501) staff       (20)    79876 2024-05-04 10:14:52.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/audiolm_pytorch.py
+-rw-r--r--   0 oseh       (501) staff       (20)     5118 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/data.py
+-rw-r--r--   0 oseh       (501) staff       (20)     8077 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/encodec.py
+-rw-r--r--   0 oseh       (501) staff       (20)     3071 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/hubert_kmeans.py
+-rw-r--r--   0 oseh       (501) staff       (20)     1000 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/optimizer.py
+-rw-r--r--   0 oseh       (501) staff       (20)    34449 2024-05-04 10:14:50.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/soundstream.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2555 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/t5.py
+-rw-r--r--   0 oseh       (501) staff       (20)    56334 2024-05-04 10:14:55.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/trainer.py
+-rw-r--r--   0 oseh       (501) staff       (20)      454 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/utils.py
+-rw-r--r--   0 oseh       (501) staff       (20)       22 2024-05-04 10:22:19.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/version.py
+-rw-r--r--   0 oseh       (501) staff       (20)     2351 2024-05-04 09:54:14.000000 audiolm_superfeel-2.0.9/audiolm_superfeel/vq_wav2vec.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:22:29.105600 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/
+-rw-r--r--   0 oseh       (501) staff       (20)     1243 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)      620 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/SOURCES.txt
+-rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/dependency_links.txt
+-rw-r--r--   0 oseh       (501) staff       (20)      263 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/requires.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       18 2024-05-04 10:22:29.000000 audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/top_level.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:22:29.105997 audiolm_superfeel-2.0.9/setup.cfg
+-rw-r--r--   0 oseh       (501) staff       (20)     1317 2024-05-04 10:21:39.000000 audiolm_superfeel-2.0.9/setup.py
```

### Comparing `audiolm_superfeel-2.0.8/LICENSE` & `audiolm_superfeel-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/PKG-INFO` & `audiolm_superfeel-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.0.8
+Version: 2.0.9
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.0.8/README.md` & `audiolm_superfeel-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/__init__.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/attend.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/audiolm_pytorch.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/audiolm_pytorch.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/data.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/data.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/encodec.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/hubert_kmeans.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/optimizer.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/soundstream.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/t5.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/trainer.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_pytorch/vq_wav2vec.py` & `audiolm_superfeel-2.0.9/audiolm_superfeel/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm_superfeel-2.0.8/audiolm_superfeel.egg-info/PKG-INFO` & `audiolm_superfeel-2.0.9/audiolm_superfeel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-superfeel
-Version: 2.0.8
+Version: 2.0.9
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/osehmathias/audiolm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm_superfeel-2.0.8/setup.py` & `audiolm_superfeel-2.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-exec(open('audiolm_pytorch/version.py').read())
+exec(open('audiolm_superfeel/version.py').read())
 
 setup(
   name = 'audiolm-superfeel',
   packages = find_packages(exclude=[]),
   version = __version__,
   license='MIT',
   description = 'AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch',
```

