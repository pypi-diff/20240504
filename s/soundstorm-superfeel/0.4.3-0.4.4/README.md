# Comparing `tmp/soundstorm_superfeel-0.4.3.tar.gz` & `tmp/soundstorm_superfeel-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundstorm_superfeel-0.4.3.tar", last modified: Sat May  4 09:51:24 2024, max compression
+gzip compressed data, was "soundstorm_superfeel-0.4.4.tar", last modified: Sat May  4 10:24:45 2024, max compression
```

## Comparing `soundstorm_superfeel-0.4.3.tar` & `soundstorm_superfeel-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 09:51:24.459900 soundstorm_superfeel-0.4.3/
--rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.3/LICENSE
--rw-r--r--   0 oseh       (501) staff       (20)      991 2024-05-04 09:51:24.459715 soundstorm_superfeel-0.4.3/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)     8325 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.3/README.md
--rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 09:51:24.459936 soundstorm_superfeel-0.4.3/setup.cfg
--rw-r--r--   0 oseh       (501) staff       (20)     1094 2024-05-04 09:51:17.000000 soundstorm_superfeel-0.4.3/setup.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 09:51:24.458770 soundstorm_superfeel-0.4.3/soundstorm_pytorch/
--rw-r--r--   0 oseh       (501) staff       (20)      180 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.3/soundstorm_pytorch/__init__.py
--rw-r--r--   0 oseh       (501) staff       (20)     4919 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.3/soundstorm_pytorch/attend.py
--rw-r--r--   0 oseh       (501) staff       (20)    41029 2024-05-04 09:49:37.000000 soundstorm_superfeel-0.4.3/soundstorm_pytorch/soundstorm.py
--rw-r--r--   0 oseh       (501) staff       (20)    10302 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.3/soundstorm_pytorch/trainer.py
-drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 09:51:24.459516 soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/
--rw-r--r--   0 oseh       (501) staff       (20)      991 2024-05-04 09:51:24.000000 soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/PKG-INFO
--rw-r--r--   0 oseh       (501) staff       (20)      368 2024-05-04 09:51:24.000000 soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/SOURCES.txt
--rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 09:51:24.000000 soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/dependency_links.txt
--rw-r--r--   0 oseh       (501) staff       (20)      161 2024-05-04 09:51:24.000000 soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/requires.txt
--rw-r--r--   0 oseh       (501) staff       (20)       19 2024-05-04 09:51:24.000000 soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/top_level.txt
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:24:45.464171 soundstorm_superfeel-0.4.4/
+-rw-r--r--   0 oseh       (501) staff       (20)     1066 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.4/LICENSE
+-rw-r--r--   0 oseh       (501) staff       (20)      991 2024-05-04 10:24:45.464005 soundstorm_superfeel-0.4.4/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)     8325 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.4/README.md
+-rw-r--r--   0 oseh       (501) staff       (20)       38 2024-05-04 10:24:45.464207 soundstorm_superfeel-0.4.4/setup.cfg
+-rw-r--r--   0 oseh       (501) staff       (20)     1094 2024-05-04 10:24:20.000000 soundstorm_superfeel-0.4.4/setup.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:24:45.463095 soundstorm_superfeel-0.4.4/soundstorm_superfeel/
+-rw-r--r--   0 oseh       (501) staff       (20)      180 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel/__init__.py
+-rw-r--r--   0 oseh       (501) staff       (20)     4919 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel/attend.py
+-rw-r--r--   0 oseh       (501) staff       (20)    41029 2024-05-04 09:49:37.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel/soundstorm.py
+-rw-r--r--   0 oseh       (501) staff       (20)    10302 2024-05-04 09:37:32.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel/trainer.py
+drwxr-xr-x   0 oseh       (501) staff       (20)        0 2024-05-04 10:24:45.463822 soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/
+-rw-r--r--   0 oseh       (501) staff       (20)      991 2024-05-04 10:24:45.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/PKG-INFO
+-rw-r--r--   0 oseh       (501) staff       (20)      376 2024-05-04 10:24:45.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/SOURCES.txt
+-rw-r--r--   0 oseh       (501) staff       (20)        1 2024-05-04 10:24:45.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/dependency_links.txt
+-rw-r--r--   0 oseh       (501) staff       (20)      161 2024-05-04 10:24:45.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/requires.txt
+-rw-r--r--   0 oseh       (501) staff       (20)       21 2024-05-04 10:24:45.000000 soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/top_level.txt
```

### Comparing `soundstorm_superfeel-0.4.3/LICENSE` & `soundstorm_superfeel-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soundstorm_superfeel-0.4.3/PKG-INFO` & `soundstorm_superfeel-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-superfeel
-Version: 0.4.3
+Version: 0.4.4
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/osehmathias/soundstorm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soundstorm_superfeel-0.4.3/README.md` & `soundstorm_superfeel-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `soundstorm_superfeel-0.4.3/setup.py` & `soundstorm_superfeel-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soundstorm-superfeel',
   packages = find_packages(exclude=[]),
-  version = '0.4.3',
+  version = '0.4.4',
   license='MIT',
   description = 'SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch',
   author = 'Phil Wang & Oseh Mathias',
   author_email = 'o@matmail.me',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/osehmathias/soundstorm-superfeel',
   keywords = [
```

### Comparing `soundstorm_superfeel-0.4.3/soundstorm_pytorch/attend.py` & `soundstorm_superfeel-0.4.4/soundstorm_superfeel/attend.py`

 * *Files identical despite different names*

### Comparing `soundstorm_superfeel-0.4.3/soundstorm_pytorch/soundstorm.py` & `soundstorm_superfeel-0.4.4/soundstorm_superfeel/soundstorm.py`

 * *Files identical despite different names*

### Comparing `soundstorm_superfeel-0.4.3/soundstorm_pytorch/trainer.py` & `soundstorm_superfeel-0.4.4/soundstorm_superfeel/trainer.py`

 * *Files identical despite different names*

### Comparing `soundstorm_superfeel-0.4.3/soundstorm_superfeel.egg-info/PKG-INFO` & `soundstorm_superfeel-0.4.4/soundstorm_superfeel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-superfeel
-Version: 0.4.3
+Version: 0.4.4
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/osehmathias/soundstorm-superfeel
 Author: Phil Wang & Oseh Mathias
 Author-email: o@matmail.me
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

