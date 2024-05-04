# Comparing `tmp/soundstorm-pytorch-0.4.2.tar.gz` & `tmp/soundstorm_pytorch-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundstorm-pytorch-0.4.2.tar", last modified: Tue Feb 27 21:57:25 2024, max compression
+gzip compressed data, was "soundstorm_pytorch-0.4.3.tar", last modified: Sat May  4 13:15:33 2024, max compression
```

## Comparing `soundstorm-pytorch-0.4.2.tar` & `soundstorm_pytorch-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:57:25.792781 soundstorm-pytorch-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-27 21:57:25.792781 soundstorm-pytorch-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 21:57:25.792781 soundstorm-pytorch-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:57:25.792781 soundstorm-pytorch-0.4.2/soundstorm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch/soundstorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-02-27 21:57:17.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:57:25.792781 soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-27 21:57:25.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-27 21:57:25.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 21:57:25.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-27 21:57:25.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-27 21:57:25.000000 soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:15:33.168712 soundstorm_pytorch-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-04 13:15:33.168712 soundstorm_pytorch-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 13:15:33.168712 soundstorm_pytorch-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:15:33.168712 soundstorm_pytorch-0.4.3/soundstorm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41029 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch/soundstorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-04 13:15:28.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 13:15:33.168712 soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-04 13:15:33.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-04 13:15:33.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 13:15:33.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-04 13:15:33.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 13:15:33.000000 soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/top_level.txt
```

### Comparing `soundstorm-pytorch-0.4.2/LICENSE` & `soundstorm_pytorch-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.4.2/PKG-INFO` & `soundstorm_pytorch-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.4.2
+Version: 0.4.3
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soundstorm-pytorch-0.4.2/README.md` & `soundstorm_pytorch-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.4.2/setup.py` & `soundstorm_pytorch-0.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soundstorm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.2',
+  version = '0.4.3',
   license='MIT',
   description = 'SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/soundstorm-pytorch',
   keywords = [
```

### Comparing `soundstorm-pytorch-0.4.2/soundstorm_pytorch/attend.py` & `soundstorm_pytorch-0.4.3/soundstorm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.4.2/soundstorm_pytorch/soundstorm.py` & `soundstorm_pytorch-0.4.3/soundstorm_pytorch/soundstorm.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import torch.nn.functional as F
 
 from einops import rearrange, reduce, repeat, unpack, pack
 from einops.layers.torch import Rearrange, EinMix
 
 from beartype import beartype
 from beartype.door import is_bearable
-from beartype.typing import Union, Dict, Optional, List, Optional
+from beartype.typing import Union, Dict, Optional, List, Optional, Any
 
 from soundstorm_pytorch.attend import Attend
 
 from spear_tts_pytorch import TextToSemantic
 
 from audiolm_pytorch import SoundStream
 from audiolm_pytorch import HubertWithKmeans, FairseqVQWav2Vec
@@ -490,15 +490,15 @@
 
     @beartype
     def __init__(
         self,
         *,
         codebook_size,
         num_quantizers,
-        conformer: Union[Conformer, Dict[str, any]],
+        conformer: Union[Conformer, Dict[str, Any]],
         grouped_quantizers = 1
     ):
         super().__init__()
         self.conformer = conformer
 
         if isinstance(conformer, dict):
             self.conformer = Conformer(**self.conformer)
```

### Comparing `soundstorm-pytorch-0.4.2/soundstorm_pytorch/trainer.py` & `soundstorm_pytorch-0.4.3/soundstorm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.4.2/soundstorm_pytorch.egg-info/PKG-INFO` & `soundstorm_pytorch-0.4.3/soundstorm_pytorch.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.4.2
+Version: 0.4.3
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

