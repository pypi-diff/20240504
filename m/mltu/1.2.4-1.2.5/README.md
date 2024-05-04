# Comparing `tmp/mltu-1.2.4.tar.gz` & `tmp/mltu-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltu-1.2.4.tar", last modified: Thu Mar 21 11:09:33 2024, max compression
+gzip compressed data, was "mltu-1.2.5.tar", last modified: Sat May  4 19:09:26 2024, max compression
```

## Comparing `mltu-1.2.4.tar` & `mltu-1.2.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.621377 mltu-1.2.4/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1062 2022-12-01 14:15:30.000000 mltu-1.2.4/LICENSE
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       24 2023-03-21 13:22:41.000000 mltu-1.2.4/MANIFEST.in
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3245 2024-03-21 11:09:33.621377 mltu-1.2.4/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2512 2024-03-18 08:04:35.000000 mltu-1.2.4/README.md
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.613377 mltu-1.2.4/mltu/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      144 2024-03-19 10:19:41.000000 mltu-1.2.4/mltu/__init__.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.613377 mltu-1.2.4/mltu/annotations/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-22 13:58:16.000000 mltu-1.2.4/mltu/annotations/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1806 2023-09-26 14:11:47.000000 mltu-1.2.4/mltu/annotations/audio.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10388 2024-03-19 09:10:04.000000 mltu-1.2.4/mltu/annotations/detections.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8026 2023-05-24 08:34:12.000000 mltu-1.2.4/mltu/annotations/images.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    40903 2024-03-21 10:40:46.000000 mltu-1.2.4/mltu/augmentors.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1349 2023-06-06 09:38:02.000000 mltu-1.2.4/mltu/configs.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    11402 2024-03-12 10:19:55.000000 mltu-1.2.4/mltu/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2995 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/inferenceModel.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10062 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/preprocessors.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.617377 mltu-1.2.4/mltu/tensorflow/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-06-06 09:38:02.000000 mltu-1.2.4/mltu/tensorflow/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6111 2023-10-17 14:37:49.000000 mltu-1.2.4/mltu/tensorflow/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      224 2023-03-21 13:22:41.000000 mltu-1.2.4/mltu/tensorflow/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     7266 2023-05-24 08:34:12.000000 mltu-1.2.4/mltu/tensorflow/layers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      897 2023-05-24 08:34:12.000000 mltu-1.2.4/mltu/tensorflow/losses.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    12935 2024-03-19 15:33:18.000000 mltu-1.2.4/mltu/tensorflow/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3443 2023-05-24 08:34:12.000000 mltu-1.2.4/mltu/tensorflow/model_utils.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.617377 mltu-1.2.4/mltu/tensorflow/transformer/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-08-29 10:56:53.000000 mltu-1.2.4/mltu/tensorflow/transformer/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     4797 2023-08-29 10:56:53.000000 mltu-1.2.4/mltu/tensorflow/transformer/attention.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2572 2023-09-26 14:11:47.000000 mltu-1.2.4/mltu/tensorflow/transformer/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    15448 2023-09-26 14:11:47.000000 mltu-1.2.4/mltu/tensorflow/transformer/layers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     6295 2023-09-26 14:11:47.000000 mltu-1.2.4/mltu/tensorflow/transformer/utils.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     9532 2023-08-29 10:56:53.000000 mltu-1.2.4/mltu/tokenizers.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.617377 mltu-1.2.4/mltu/torch/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.2.4/mltu/torch/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    20456 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/callbacks.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    10940 2024-03-12 10:19:55.000000 mltu-1.2.4/mltu/torch/dataProvider.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3885 2024-03-12 10:19:55.000000 mltu-1.2.4/mltu/torch/handlers.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1371 2023-09-26 14:11:47.000000 mltu-1.2.4/mltu/torch/losses.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     5228 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    15515 2024-03-15 11:25:28.000000 mltu-1.2.4/mltu/torch/model.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.621377 mltu-1.2.4/mltu/torch/yolo/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3173 2024-03-18 09:53:19.000000 mltu-1.2.4/mltu/torch/yolo/annotation.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.621377 mltu-1.2.4/mltu/torch/yolo/detectors/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/detectors/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2357 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/detectors/detector.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3503 2024-03-18 08:04:35.000000 mltu-1.2.4/mltu/torch/yolo/detectors/onnx_detector.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2524 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/detectors/torch_detector.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     4970 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/loss.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     8276 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/metrics.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2116 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/optimizer.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1045 2024-03-12 10:19:55.000000 mltu-1.2.4/mltu/torch/yolo/preprocessors.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     2956 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/pruning_utils.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    11467 2024-03-05 12:15:57.000000 mltu-1.2.4/mltu/torch/yolo/train.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     4670 2024-03-21 11:08:13.000000 mltu-1.2.4/mltu/torch/yolo/train_yolo.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)    15091 2024-03-21 10:41:07.000000 mltu-1.2.4/mltu/transformers.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.621377 mltu-1.2.4/mltu/utils/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2023-03-21 13:22:41.000000 mltu-1.2.4/mltu/utils/__init__.py
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     4282 2023-09-26 14:11:47.000000 mltu-1.2.4/mltu/utils/text_utils.py
-drwxr-xr-x   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        0 2024-03-21 11:09:33.621377 mltu-1.2.4/mltu.egg-info/
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     3245 2024-03-21 11:09:33.000000 mltu-1.2.4/mltu.egg-info/PKG-INFO
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1491 2024-03-21 11:09:33.000000 mltu-1.2.4/mltu.egg-info/SOURCES.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        1 2024-03-21 11:09:33.000000 mltu-1.2.4/mltu.egg-info/dependency_links.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      124 2024-03-21 11:09:33.000000 mltu-1.2.4/mltu.egg-info/requires.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)        5 2024-03-21 11:09:33.000000 mltu-1.2.4/mltu.egg-info/top_level.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)      135 2024-03-15 14:50:45.000000 mltu-1.2.4/requirements.txt
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)       38 2024-03-21 11:09:33.621377 mltu-1.2.4/setup.cfg
--rw-r--r--   0 rokbal@sf.lan  (2615) sf-developers@sf.lan  (2010)     1625 2024-01-02 08:07:09.000000 mltu-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.704490 mltu-1.2.5/
+-rw-rw-rw-   0        0        0     1083 2022-11-19 15:23:48.000000 mltu-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-01-05 13:30:48.000000 mltu-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3439 2024-05-04 19:09:26.703490 mltu-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2681 2024-05-04 19:08:56.000000 mltu-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.678490 mltu-1.2.5/mltu/
+-rw-rw-rw-   0        0        0      148 2024-05-04 19:08:56.000000 mltu-1.2.5/mltu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.684490 mltu-1.2.5/mltu/annotations/
+-rw-rw-rw-   0        0        0        0 2023-03-21 12:48:19.000000 mltu-1.2.5/mltu/annotations/__init__.py
+-rw-rw-rw-   0        0        0     1872 2023-09-28 17:02:22.000000 mltu-1.2.5/mltu/annotations/audio.py
+-rw-rw-rw-   0        0        0    10687 2024-03-21 14:11:37.000000 mltu-1.2.5/mltu/annotations/detections.py
+-rw-rw-rw-   0        0        0     8319 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/annotations/images.py
+-rw-rw-rw-   0        0        0    42051 2024-05-04 19:08:56.000000 mltu-1.2.5/mltu/augmentors.py
+-rw-rw-rw-   0        0        0     1391 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/configs.py
+-rw-rw-rw-   0        0        0    11819 2024-05-04 19:08:56.000000 mltu-1.2.5/mltu/dataProvider.py
+-rw-rw-rw-   0        0        0     3075 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/inferenceModel.py
+-rw-rw-rw-   0        0        0    10341 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/preprocessors.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.688490 mltu-1.2.5/mltu/tensorflow/
+-rw-rw-rw-   0        0        0        0 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0     6278 2024-01-02 08:49:27.000000 mltu-1.2.5/mltu/tensorflow/callbacks.py
+-rw-rw-rw-   0        0        0      231 2023-03-06 09:04:00.000000 mltu-1.2.5/mltu/tensorflow/dataProvider.py
+-rw-rw-rw-   0        0        0     7449 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tensorflow/layers.py
+-rw-rw-rw-   0        0        0      918 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tensorflow/losses.py
+-rw-rw-rw-   0        0        0    13198 2024-03-21 14:11:37.000000 mltu-1.2.5/mltu/tensorflow/metrics.py
+-rw-rw-rw-   0        0        0     3537 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tensorflow/model_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.690490 mltu-1.2.5/mltu/tensorflow/transformer/
+-rw-rw-rw-   0        0        0        0 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tensorflow/transformer/__init__.py
+-rw-rw-rw-   0        0        0     4917 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tensorflow/transformer/attention.py
+-rw-rw-rw-   0        0        0     2631 2023-09-28 17:02:22.000000 mltu-1.2.5/mltu/tensorflow/transformer/callbacks.py
+-rw-rw-rw-   0        0        0    15844 2023-09-28 17:02:22.000000 mltu-1.2.5/mltu/tensorflow/transformer/layers.py
+-rw-rw-rw-   0        0        0     6456 2023-09-28 17:02:22.000000 mltu-1.2.5/mltu/tensorflow/transformer/utils.py
+-rw-rw-rw-   0        0        0     9778 2023-09-06 14:40:23.000000 mltu-1.2.5/mltu/tokenizers.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.694490 mltu-1.2.5/mltu/torch/
+-rw-rw-rw-   0        0        0        0 2023-03-06 13:22:39.000000 mltu-1.2.5/mltu/torch/__init__.py
+-rw-rw-rw-   0        0        0    20999 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/callbacks.py
+-rw-rw-rw-   0        0        0    11234 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/dataProvider.py
+-rw-rw-rw-   0        0        0     3987 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/handlers.py
+-rw-rw-rw-   0        0        0     1408 2023-09-28 17:02:22.000000 mltu-1.2.5/mltu/torch/losses.py
+-rw-rw-rw-   0        0        0     5394 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/metrics.py
+-rw-rw-rw-   0        0        0    15942 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.698490 mltu-1.2.5/mltu/torch/yolo/
+-rw-rw-rw-   0        0        0        0 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-03-21 14:11:37.000000 mltu-1.2.5/mltu/torch/yolo/annotation.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.700490 mltu-1.2.5/mltu/torch/yolo/detectors/
+-rw-rw-rw-   0        0        0        0 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/detectors/__init__.py
+-rw-rw-rw-   0        0        0     2414 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/detectors/detector.py
+-rw-rw-rw-   0        0        0     3586 2024-03-17 18:07:54.000000 mltu-1.2.5/mltu/torch/yolo/detectors/onnx_detector.py
+-rw-rw-rw-   0        0        0     2592 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/detectors/torch_detector.py
+-rw-rw-rw-   0        0        0     5080 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/loss.py
+-rw-rw-rw-   0        0        0     8477 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/metrics.py
+-rw-rw-rw-   0        0        0     2166 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/optimizer.py
+-rw-rw-rw-   0        0        0     1172 2024-05-04 19:08:56.000000 mltu-1.2.5/mltu/torch/yolo/preprocessors.py
+-rw-rw-rw-   0        0        0     3025 2024-03-15 12:29:04.000000 mltu-1.2.5/mltu/torch/yolo/pruning_utils.py
+-rw-rw-rw-   0        0        0    15492 2024-03-21 14:11:37.000000 mltu-1.2.5/mltu/transformers.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.701490 mltu-1.2.5/mltu/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-02 11:34:41.000000 mltu-1.2.5/mltu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4404 2023-09-28 17:02:22.000000 mltu-1.2.5/mltu/utils/text_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.703490 mltu-1.2.5/mltu.egg-info/
+-rw-rw-rw-   0        0        0     3439 2024-05-04 19:09:26.000000 mltu-1.2.5/mltu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1494 2024-05-04 19:09:26.000000 mltu-1.2.5/mltu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:09:26.000000 mltu-1.2.5/mltu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-05-04 19:09:26.000000 mltu-1.2.5/mltu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-04 19:09:26.000000 mltu-1.2.5/mltu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2024-03-15 12:29:04.000000 mltu-1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:09:26.704490 mltu-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2024-01-02 08:49:27.000000 mltu-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:09:26.702490 mltu-1.2.5/tests/
+-rw-rw-rw-   0        0        0     2105 2023-09-06 14:40:23.000000 mltu-1.2.5/tests/test_tensorflow_metrics.py
+-rw-rw-rw-   0        0        0     3505 2023-09-06 14:40:23.000000 mltu-1.2.5/tests/test_text_utils.py
```

### Comparing `mltu-1.2.4/PKG-INFO` & `mltu-1.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1
-Name: mltu
-Version: 1.2.4
-Summary: Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch
-Home-page: https://pylessons.com/
-Author: PyLessons
-Author-email: pythonlessons0@gmail.com
-Project-URL: Source, https://github.com/pythonlessons/mltu/
-Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyYAML>=6.0
-Requires-Dist: tqdm
-Requires-Dist: qqdm==0.0.7
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: Pillow>=9.4.0
-Requires-Dist: onnxruntime>=1.15.0
-Requires-Dist: matplotlib
-Provides-Extra: gpu
-Requires-Dist: onnxruntime-gpu; extra == "gpu"
-
-# MLTU - Machine Learning Training Utilities
-Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
-<p align="center">
-  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
-</p>
-
-# Installation:
-To use MLTU in your own project, you can install it from PyPI:
-```bash
-pip install mltu
-```
-When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
-```bash
-pip install mltu==0.1.3
-```
-Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
-
-# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
-1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
-2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
-3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
-4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
-5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
-6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
-7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
-8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
-9. [Transformer training with TensorFlow for Translation task](https://pylessons.com/transformers-training), code in ```Tutorials\09_translation_transformer``` folder;
-10. [Speech Recognition in Python | finetune wav2vec2 model for a custom ASR model](https://youtu.be/h6ooEGzjkj0), code in ```Tutorials\10_wav2vec2_torch``` folder;
-11. [YOLOv8: Real-Time Object Detection Simplified](https://youtu.be/vegL__weCxY), code in ```Tutorials\11_Yolov8``` folder;
+Metadata-Version: 2.1
+Name: mltu
+Version: 1.2.5
+Summary: Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch
+Home-page: https://pylessons.com/
+Author: PyLessons
+Author-email: pythonlessons0@gmail.com
+Project-URL: Source, https://github.com/pythonlessons/mltu/
+Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: tqdm
+Requires-Dist: qqdm==0.0.7
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: Pillow>=9.4.0
+Requires-Dist: onnxruntime>=1.15.0
+Requires-Dist: matplotlib
+Provides-Extra: gpu
+Requires-Dist: onnxruntime-gpu; extra == "gpu"
+
+# MLTU - Machine Learning Training Utilities
+Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
+<p align="center">
+  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
+</p>
+
+# Installation:
+To use MLTU in your own project, you can install it from PyPI:
+```bash
+pip install mltu
+```
+When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
+```bash
+pip install mltu==0.1.3
+```
+Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
+
+# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
+1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
+2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
+3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
+4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
+5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
+6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
+7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
+8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
+9. [Transformer training with TensorFlow for Translation task](https://pylessons.com/transformers-training), code in ```Tutorials\09_translation_transformer``` folder;
+10. [Speech Recognition in Python | finetune wav2vec2 model for a custom ASR model](https://youtu.be/h6ooEGzjkj0), code in ```Tutorials\10_wav2vec2_torch``` folder;
+11. [YOLOv8: Real-Time Object Detection Simplified](https://youtu.be/vegL__weCxY), code in ```Tutorials\11_Yolov8``` folder;
+12. [YOLOv8: Customizing Object Detector training](https://youtu.be/ysYiV1CbCyY), code in ```Tutorials\11_Yolov8\train_yolov8.py``` folder;
```

### Comparing `mltu-1.2.4/README.md` & `mltu-1.2.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# MLTU - Machine Learning Training Utilities
-Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
-<p align="center">
-  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
-</p>
-
-# Installation:
-To use MLTU in your own project, you can install it from PyPI:
-```bash
-pip install mltu
-```
-When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
-```bash
-pip install mltu==0.1.3
-```
-Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
-
-# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
-1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
-2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
-3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
-4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
-5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
-6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
-7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
-8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
-9. [Transformer training with TensorFlow for Translation task](https://pylessons.com/transformers-training), code in ```Tutorials\09_translation_transformer``` folder;
-10. [Speech Recognition in Python | finetune wav2vec2 model for a custom ASR model](https://youtu.be/h6ooEGzjkj0), code in ```Tutorials\10_wav2vec2_torch``` folder;
-11. [YOLOv8: Real-Time Object Detection Simplified](https://youtu.be/vegL__weCxY), code in ```Tutorials\11_Yolov8``` folder;
+# MLTU - Machine Learning Training Utilities
+Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
+<p align="center">
+  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
+</p>
+
+# Installation:
+To use MLTU in your own project, you can install it from PyPI:
+```bash
+pip install mltu
+```
+When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
+```bash
+pip install mltu==0.1.3
+```
+Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
+
+# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
+1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
+2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
+3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
+4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
+5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
+6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
+7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
+8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
+9. [Transformer training with TensorFlow for Translation task](https://pylessons.com/transformers-training), code in ```Tutorials\09_translation_transformer``` folder;
+10. [Speech Recognition in Python | finetune wav2vec2 model for a custom ASR model](https://youtu.be/h6ooEGzjkj0), code in ```Tutorials\10_wav2vec2_torch``` folder;
+11. [YOLOv8: Real-Time Object Detection Simplified](https://youtu.be/vegL__weCxY), code in ```Tutorials\11_Yolov8``` folder;
+12. [YOLOv8: Customizing Object Detector training](https://youtu.be/ysYiV1CbCyY), code in ```Tutorials\11_Yolov8\train_yolov8.py``` folder;
```

### Comparing `mltu-1.2.4/mltu/annotations/detections.py` & `mltu-1.2.5/mltu/annotations/detections.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-import cv2
-import typing
-import numpy as np
-from enum import Enum
-
-
-class BboxType(Enum):
-    XYWH = 1 # x center, y center, width, height
-    XYXY = 2 # left, top, right, bottom
-    LTWH = 3 # left, top, width, height
-
-
-class Detection:
-    """ Object to hold the information of a detection for simple manipulation and visualization
-    """
-    def __init__(
-            self, 
-            bbox, 
-            label: str, 
-            labels: dict={},
-            bbox_type: BboxType=BboxType.XYWH,
-            confidence: float=0.0, 
-            image_path: str="", 
-            width: int=None, 
-            height: int=None,
-            relative: bool=False
-        ):
-        """
-        Args:
-            bbox (list or np.ndarray): Bounding box coordinates
-            label (str): Label of the detection
-            labels (dict, optional): Dictionary of labels. Defaults to {}.
-            bbox_type (BboxType, optional): Type of the bounding box coordinates. Defaults to BboxType.XYWH.
-            confidence (float, optional): Confidence score of the detection. Defaults to 0.0.
-            image_path (str, optional): Path to the image. Defaults to "".
-            width (int, optional): Width of the image. Defaults to None.
-            height (int, optional): Height of the image. Defaults to None.
-            relative (bool, optional): Whether the bounding box coordinates are relative to the image size. Defaults to False.
-        """
-        self.bbox = np.array(bbox)
-        self.label = label
-        self.labels = labels
-        self.bbox_type = bbox_type
-        self.confidence = confidence
-        self.image_path = image_path
-        self.width = width
-        self.height = height
-        self.relative = relative
-
-        self.augmented = False
-
-        self._xywh = None
-        self._xyxy = None
-
-        self.validate()
-
-    @property
-    def labelId(self) -> int:
-        return self.label2id(self.label)
-
-    def label2id(self, label: str) -> int:
-        labelId = {v: k for k, v in self.labels.items()}.get(label, None)
-        if labelId is None:
-            raise ValueError(f"label {label} not found in labels")
-        
-        return labelId
-    
-    @property
-    def xywh(self):
-        return self._xywh
-    
-    @xywh.setter
-    def xywh(self, xywh: np.ndarray):
-        if (xywh[:2] + xywh[2:] / 2 > 1).any():
-            # fix the bbox to be in range [0, 1]
-            self._xywh = self.xyxy2xywh(self.xywh2xyxy(xywh))
-        else:
-            self._xywh = xywh.clip(0, 1)
-
-        self._xyxy = self.xywh2xyxy(self._xywh)
-
-    @property
-    def xyxy(self):
-        return self._xyxy
-    
-    @property
-    def xyxy_abs(self):
-        return (self.xyxy * np.array([self.width, self.height, self.width, self.height])).astype(int)
-
-    @staticmethod
-    def xywh2xyxy(xywh: np.ndarray):
-        """ Convert bounding box from x, y, width, height to x1, y1, x2, y2
-        """
-        x, y, w, h = xywh
-        x, y = x - w / 2, y - h / 2
-        return np.array([x, y, x+w, y+h]).clip(0, 1)
-    
-    @staticmethod
-    def xyxy2xywh(xyxy: np.ndarray):
-        """ Convert bounding box from x1, y1, x2, y2 to x, y, width, height
-        """
-        x, y, x2, y2 = xyxy
-        w, h = x2 - x, y2 - y
-        return np.array([x + w / 2, y + h / 2, w, h]).clip(0, 1)
-    
-    @staticmethod
-    def ltwh2xywh(ltwh: np.ndarray):
-        """ Convert bounding box from left, top, width, height to x, y, width, height
-        """
-        l, t, w, h = ltwh
-        return np.array([l + w / 2, t + h / 2, w, h]).clip(0, 1)
-    
-    def validate(self):
-        """ Validate the bounding box coordinates
-        """
-        assert self.bbox_type in BboxType, f"bbox_type must be one of {BboxType}"
-        if not self.relative:
-            if self.width is None or self.height is None:
-                raise ValueError("width and height must be provided when relative is False")
-            
-            if not (np.array(self.bbox) > 1.0).any():
-                raise ValueError("bbox coordinates must be in range [0, np.inf] when relative is False")
-            
-            bbox = np.array(self.bbox) / np.array([self.width, self.height, self.width, self.height])
-
-        else:
-            bbox = self.bbox
-
-        if self.bbox_type.name == "XYWH":
-            self.xywh = bbox
-
-        elif self.bbox_type.name == "XYXY":
-            self.xywh = self.xyxy2xywh(bbox)
-
-        elif self.bbox_type.name == "LTWH":
-            self.xywh = self.ltwh2xywh(bbox)
-
-        else:
-            raise ValueError(f"bbox_type {self.bbox_type} not supported")
-        
-    def flip(self, direction: int):
-        new_xywh = self.xywh
-        if direction == 0: # mirror
-            new_xywh[0] = 1 - new_xywh[0]
-
-        elif direction == 1: # vertical
-            new_xywh[1] = 1 - new_xywh[1]
-
-        self.xywh = new_xywh
-        
-        self.augmented = True
-
-    def dot(self, rotMat: np.ndarray, width: int, height: int):
-        """ Apply transformation matrix to detection
-
-        Args:
-            matrix (np.ndarray): Transformation matrix
-            width (int): Width of the image
-            height (int): Height of the image
-
-        Returns:
-            Object with transformed coordinates
-        """
-        # get the four corners of the bounding box
-        bb = np.array(self.xyxy) * np.array([self.width, self.height, self.width, self.height])
-        bb = np.array(((bb[0],bb[1]),(bb[2],bb[1]),(bb[2],bb[3]),(bb[0],bb[3])))
-
-        bb_rotated = np.vstack((bb.T, np.array((1,1,1,1)))) #Convert the array to [x,y,1] format to dot it with the rotMat
-        bb_rotated = np.dot(rotMat, bb_rotated).T #Perform Dot product and get back the points in shape of (4,2)
-
-        # get the new coordinates of the bounding box
-        x_min = min(bb_rotated[:, 0])
-        y_min = min(bb_rotated[:, 1])
-        x_max = max(bb_rotated[:, 0])
-        y_max = max(bb_rotated[:, 1])
-
-        new_x = (x_min + x_max) / 2
-        new_y = (y_min + y_max) / 2
-        new_w = x_max - x_min
-        new_h = y_max - y_min
-
-        # Normalize to the new width and height
-        new_x /= width
-        new_y /= height
-        new_w /= width
-        new_h /= height
-
-        self.xywh = np.array([new_x, new_y, new_w, new_h])
-
-        self.width = width
-        self.height = height
-        self.augmented = True
-        
-        return self
-
-    def applyToFrame(self, frame: np.ndarray, color: tuple=(0, 255, 0), thickness: int=2, **kwargs) -> np.ndarray:
-        """ Draw the bounding box on the image
-        """
-        # Get the coordinates of the bounding box
-        x, y, x2, y2 = (self.xyxy * np.array([self.width, self.height, self.width, self.height])).astype(np.int32)
-
-        # Draw the bounding box on the image
-        frame = cv2.rectangle(frame.copy(), (x, y), (x2, y2), color, thickness, **kwargs)
-
-        label = f"{self.label}: {self.confidence:.2f}" if self.confidence > 0 else self.label
-
-        # Calculate the dimensions of the label text
-        (label_width, label_height), _ = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.5, 1)
-
-        label_y = y - 10 if y - 10 > label_height else y + 10
-
-        # Draw a filled rectangle as the background for the label text
-        cv2.rectangle(
-            frame, (x, label_y - label_height), (x + label_width, label_y + label_height), color, cv2.FILLED
-        )
-
-        cv2.putText(frame, label, (x, label_y), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 0), 1, cv2.LINE_AA)
-
-        return frame
-
-    def json(self):
-        return {
-            "xywh": self.xywh.tolist(),
-            "label": self.label,
-            "confidence": self.confidence,
-            "image_path": self.image_path,
-            "width": self.width,
-            "height": self.height
-        }
-    
-
-class Detections:
-    """ Object to hold the information of multiple detections for simple manipulation and visualization"""
-    def __init__(
-            self, 
-            labels: dict,
-            width: int,
-            height: int,
-            detections: typing.Iterable[Detection] = [],
-            image_path: str = "",
-            color_palette: list=[]
-        ) -> None:
-        """ Initialize the Detections object
-
-        Args:
-            labels (dict): Dictionary of labels
-            width (int): Width of the image
-            height (int): Height of the image
-            detections (typing.Iterable[Detection], optional): List of detections. Defaults to [].
-            image_path (str, optional): Path to the image. Defaults to "".
-            color_palette (list, optional): List of colors to use for the bounding boxes. Defaults to [].
-        """
-        self.labels = labels
-        self.width = width
-        self.height = height
-        self.detections = detections
-        self.image_path = image_path
-        self.color_palette = color_palette
-
-        self.validate()
-
-    def label2id(self, label: str) -> int:
-        labelId = {v: k for k, v in self.labels.items()}.get(label, None)
-        if labelId is None:
-            raise ValueError(f"label {label} not found in labels")
-        
-        return labelId
-
-    def validate(self):
-        for detection in self.detections:
-            if not isinstance(detection, Detection):
-                raise TypeError(f"detections must be iterable of Detection, not {type(detection)}")
-            
-            detection.width = self.width
-            detection.height = self.height
-            detection.labels = self.labels
-            detection.image_path = self.image_path
-
-        if isinstance(self.labels, list):
-            self.labels = {i: label for i, label in enumerate(self.labels)}
-
-        if not self.labels:
-            self.labels = {k: v for k, v in enumerate(sorted(set([detection.label for detection in self.detections])))}
-
-    def applyToFrame(self, image: np.ndarray, **kwargs: dict) -> np.ndarray:
-        """ Draw the detections on the image """
-        for detection in self.detections:
-            color = self.color_palette[detection.labelId] if len(self.color_palette) == len(self.labels) else (0, 255, 0)
-            image = detection.applyToFrame(image, color=color, **kwargs)
-        
-        return image
-
-    def __iter__(self):
-        return iter(self.detections)
-
-    def __len__(self):
-        return len(self.detections)
-
-    def __getitem__(self, index: int):
+import cv2
+import typing
+import numpy as np
+from enum import Enum
+
+
+class BboxType(Enum):
+    XYWH = 1 # x center, y center, width, height
+    XYXY = 2 # left, top, right, bottom
+    LTWH = 3 # left, top, width, height
+
+
+class Detection:
+    """ Object to hold the information of a detection for simple manipulation and visualization
+    """
+    def __init__(
+            self, 
+            bbox, 
+            label: str, 
+            labels: dict={},
+            bbox_type: BboxType=BboxType.XYWH,
+            confidence: float=0.0, 
+            image_path: str="", 
+            width: int=None, 
+            height: int=None,
+            relative: bool=False
+        ):
+        """
+        Args:
+            bbox (list or np.ndarray): Bounding box coordinates
+            label (str): Label of the detection
+            labels (dict, optional): Dictionary of labels. Defaults to {}.
+            bbox_type (BboxType, optional): Type of the bounding box coordinates. Defaults to BboxType.XYWH.
+            confidence (float, optional): Confidence score of the detection. Defaults to 0.0.
+            image_path (str, optional): Path to the image. Defaults to "".
+            width (int, optional): Width of the image. Defaults to None.
+            height (int, optional): Height of the image. Defaults to None.
+            relative (bool, optional): Whether the bounding box coordinates are relative to the image size. Defaults to False.
+        """
+        self.bbox = np.array(bbox)
+        self.label = label
+        self.labels = labels
+        self.bbox_type = bbox_type
+        self.confidence = confidence
+        self.image_path = image_path
+        self.width = width
+        self.height = height
+        self.relative = relative
+
+        self.augmented = False
+
+        self._xywh = None
+        self._xyxy = None
+
+        self.validate()
+
+    @property
+    def labelId(self) -> int:
+        return self.label2id(self.label)
+
+    def label2id(self, label: str) -> int:
+        labelId = {v: k for k, v in self.labels.items()}.get(label, None)
+        if labelId is None:
+            raise ValueError(f"label {label} not found in labels")
+        
+        return labelId
+    
+    @property
+    def xywh(self):
+        return self._xywh
+    
+    @xywh.setter
+    def xywh(self, xywh: np.ndarray):
+        if (xywh[:2] + xywh[2:] / 2 > 1).any():
+            # fix the bbox to be in range [0, 1]
+            self._xywh = self.xyxy2xywh(self.xywh2xyxy(xywh))
+        else:
+            self._xywh = xywh.clip(0, 1)
+
+        self._xyxy = self.xywh2xyxy(self._xywh)
+
+    @property
+    def xyxy(self):
+        return self._xyxy
+    
+    @property
+    def xyxy_abs(self):
+        return (self.xyxy * np.array([self.width, self.height, self.width, self.height])).astype(int)
+
+    @staticmethod
+    def xywh2xyxy(xywh: np.ndarray):
+        """ Convert bounding box from x, y, width, height to x1, y1, x2, y2
+        """
+        x, y, w, h = xywh
+        x, y = x - w / 2, y - h / 2
+        return np.array([x, y, x+w, y+h]).clip(0, 1)
+    
+    @staticmethod
+    def xyxy2xywh(xyxy: np.ndarray):
+        """ Convert bounding box from x1, y1, x2, y2 to x, y, width, height
+        """
+        x, y, x2, y2 = xyxy
+        w, h = x2 - x, y2 - y
+        return np.array([x + w / 2, y + h / 2, w, h]).clip(0, 1)
+    
+    @staticmethod
+    def ltwh2xywh(ltwh: np.ndarray):
+        """ Convert bounding box from left, top, width, height to x, y, width, height
+        """
+        l, t, w, h = ltwh
+        return np.array([l + w / 2, t + h / 2, w, h]).clip(0, 1)
+    
+    def validate(self):
+        """ Validate the bounding box coordinates
+        """
+        assert self.bbox_type in BboxType, f"bbox_type must be one of {BboxType}"
+        if not self.relative:
+            if self.width is None or self.height is None:
+                raise ValueError("width and height must be provided when relative is False")
+            
+            if not (np.array(self.bbox) > 1.0).any():
+                raise ValueError("bbox coordinates must be in range [0, np.inf] when relative is False")
+            
+            bbox = np.array(self.bbox) / np.array([self.width, self.height, self.width, self.height])
+
+        else:
+            bbox = self.bbox
+
+        if self.bbox_type.name == "XYWH":
+            self.xywh = bbox
+
+        elif self.bbox_type.name == "XYXY":
+            self.xywh = self.xyxy2xywh(bbox)
+
+        elif self.bbox_type.name == "LTWH":
+            self.xywh = self.ltwh2xywh(bbox)
+
+        else:
+            raise ValueError(f"bbox_type {self.bbox_type} not supported")
+        
+    def flip(self, direction: int):
+        new_xywh = self.xywh
+        if direction == 0: # mirror
+            new_xywh[0] = 1 - new_xywh[0]
+
+        elif direction == 1: # vertical
+            new_xywh[1] = 1 - new_xywh[1]
+
+        self.xywh = new_xywh
+        
+        self.augmented = True
+
+    def dot(self, rotMat: np.ndarray, width: int, height: int):
+        """ Apply transformation matrix to detection
+
+        Args:
+            matrix (np.ndarray): Transformation matrix
+            width (int): Width of the image
+            height (int): Height of the image
+
+        Returns:
+            Object with transformed coordinates
+        """
+        # get the four corners of the bounding box
+        bb = np.array(self.xyxy) * np.array([self.width, self.height, self.width, self.height])
+        bb = np.array(((bb[0],bb[1]),(bb[2],bb[1]),(bb[2],bb[3]),(bb[0],bb[3])))
+
+        bb_rotated = np.vstack((bb.T, np.array((1,1,1,1)))) #Convert the array to [x,y,1] format to dot it with the rotMat
+        bb_rotated = np.dot(rotMat, bb_rotated).T #Perform Dot product and get back the points in shape of (4,2)
+
+        # get the new coordinates of the bounding box
+        x_min = min(bb_rotated[:, 0])
+        y_min = min(bb_rotated[:, 1])
+        x_max = max(bb_rotated[:, 0])
+        y_max = max(bb_rotated[:, 1])
+
+        new_x = (x_min + x_max) / 2
+        new_y = (y_min + y_max) / 2
+        new_w = x_max - x_min
+        new_h = y_max - y_min
+
+        # Normalize to the new width and height
+        new_x /= width
+        new_y /= height
+        new_w /= width
+        new_h /= height
+
+        self.xywh = np.array([new_x, new_y, new_w, new_h])
+
+        self.width = width
+        self.height = height
+        self.augmented = True
+        
+        return self
+
+    def applyToFrame(self, frame: np.ndarray, color: tuple=(0, 255, 0), thickness: int=2, **kwargs) -> np.ndarray:
+        """ Draw the bounding box on the image
+        """
+        # Get the coordinates of the bounding box
+        x, y, x2, y2 = (self.xyxy * np.array([self.width, self.height, self.width, self.height])).astype(np.int32)
+
+        # Draw the bounding box on the image
+        frame = cv2.rectangle(frame.copy(), (x, y), (x2, y2), color, thickness, **kwargs)
+
+        label = f"{self.label}: {self.confidence:.2f}" if self.confidence > 0 else self.label
+
+        # Calculate the dimensions of the label text
+        (label_width, label_height), _ = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.5, 1)
+
+        label_y = y - 10 if y - 10 > label_height else y + 10
+
+        # Draw a filled rectangle as the background for the label text
+        cv2.rectangle(
+            frame, (x, label_y - label_height), (x + label_width, label_y + label_height), color, cv2.FILLED
+        )
+
+        cv2.putText(frame, label, (x, label_y), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 0), 1, cv2.LINE_AA)
+
+        return frame
+
+    def json(self):
+        return {
+            "xywh": self.xywh.tolist(),
+            "label": self.label,
+            "confidence": self.confidence,
+            "image_path": self.image_path,
+            "width": self.width,
+            "height": self.height
+        }
+    
+
+class Detections:
+    """ Object to hold the information of multiple detections for simple manipulation and visualization"""
+    def __init__(
+            self, 
+            labels: dict,
+            width: int,
+            height: int,
+            detections: typing.Iterable[Detection] = [],
+            image_path: str = "",
+            color_palette: list=[]
+        ) -> None:
+        """ Initialize the Detections object
+
+        Args:
+            labels (dict): Dictionary of labels
+            width (int): Width of the image
+            height (int): Height of the image
+            detections (typing.Iterable[Detection], optional): List of detections. Defaults to [].
+            image_path (str, optional): Path to the image. Defaults to "".
+            color_palette (list, optional): List of colors to use for the bounding boxes. Defaults to [].
+        """
+        self.labels = labels
+        self.width = width
+        self.height = height
+        self.detections = detections
+        self.image_path = image_path
+        self.color_palette = color_palette
+
+        self.validate()
+
+    def label2id(self, label: str) -> int:
+        labelId = {v: k for k, v in self.labels.items()}.get(label, None)
+        if labelId is None:
+            raise ValueError(f"label {label} not found in labels")
+        
+        return labelId
+
+    def validate(self):
+        for detection in self.detections:
+            if not isinstance(detection, Detection):
+                raise TypeError(f"detections must be iterable of Detection, not {type(detection)}")
+            
+            detection.width = self.width
+            detection.height = self.height
+            detection.labels = self.labels
+            detection.image_path = self.image_path
+
+        if isinstance(self.labels, list):
+            self.labels = {i: label for i, label in enumerate(self.labels)}
+
+        if not self.labels:
+            self.labels = {k: v for k, v in enumerate(sorted(set([detection.label for detection in self.detections])))}
+
+    def applyToFrame(self, image: np.ndarray, **kwargs: dict) -> np.ndarray:
+        """ Draw the detections on the image """
+        for detection in self.detections:
+            color = self.color_palette[detection.labelId] if len(self.color_palette) == len(self.labels) else (0, 255, 0)
+            image = detection.applyToFrame(image, color=color, **kwargs)
+        
+        return image
+
+    def __iter__(self):
+        return iter(self.detections)
+
+    def __len__(self):
+        return len(self.detections)
+
+    def __getitem__(self, index: int):
         return self.detections[index]
```

### Comparing `mltu-1.2.4/mltu/augmentors.py` & `mltu-1.2.5/mltu/augmentors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1043 +1,1045 @@
-import cv2
-import typing
-import numpy as np
-import importlib
-import logging
-
-from . import Image
-from mltu.annotations.audio import Audio
-from mltu.annotations.detections import Detections, Detection, BboxType
-
-""" 
-Implemented image augmentors:
-- RandomBrightness
-- RandomRotate
-- RandomErodeDilate
-- RandomSharpen
-- RandomGaussianBlur
-- RandomSaltAndPepper
-- RandomMirror
-- RandomFlip
-- RandomDropBlock
-- RandomMosaic
-- RandomZoom
-- RandomColorMode
-- RandomElasticTransform
-
-Implemented audio augmentors:
-- RandomAudioNoise
-- RandomAudioPitchShift
-- RandomAudioTimeStretch
-"""
-
-def randomness_decorator(func):
-    """ Decorator for randomness """
-    def wrapper(self, data: typing.Union[Image, Audio], annotation: typing.Any) -> typing.Tuple[typing.Union[Image, Audio], typing.Any]:
-        """ Decorator for randomness and type checking
-
-        Args:
-            data (typing.Union[Image, Audio]): Image or Audio object to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            data (typing.Union[Image, Audio]): Adjusted image or audio
-            annotation (typing.Any): Adjusted annotation
-        """
-        # check if image is Image object
-        if not isinstance(data, (Image, Audio)):
-            self.logger.error(f"data must be Image or Audio object, not {type(data)}, skipping augmentor")
-            # TODO instead of error convert image into Image object
-            # TODO instead of error convert audio into Audio object
-            return data, annotation
-
-        if np.random.rand() > self._random_chance:
-            return data, annotation
-
-        # return result of function
-        return func(self, data, annotation)
-
-    return wrapper
-
-
-class Augmentor:
-    """ Object that should be inherited by all augmentors
-
-    Args:
-        random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
-        log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
-    """
-    def __init__(self, random_chance: float=0.5, log_level: int = logging.INFO, augment_annotation: bool = False) -> None:
-        self._random_chance = random_chance
-        self._log_level = log_level
-        self._augment_annotation = augment_annotation
-
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(logging.INFO)
-
-        assert 0 <= self._random_chance <= 1.0, "random chance must be between 0.0 and 1.0"
-
-    def augment(self, data: typing.Union[Image, Audio]):
-        """ Augment data """
-        raise NotImplementedError
-
-    @randomness_decorator
-    def __call__(self, data: typing.Union[Image, Audio], annotation: typing.Any) -> typing.Tuple[typing.Union[Image, Audio], typing.Any]:
-        """ Randomly add noise to audio
-
-        Args:
-            data (typing.Union[Image, Audio]): Image or Audio object to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            data (typing.Union[Image, Audio]): Adjusted image or audio
-            annotation (typing.Any): Adjusted annotation if necessary
-        """
-        data = self.augment(data)
-
-        if self._augment_annotation and isinstance(annotation, np.ndarray):
-            annotation = self.augment(annotation)
-
-        return data, annotation
-
-
-class RandomBrightness(Augmentor):
-    """ Randomly adjust image brightness """
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        delta: int = 100,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = False
-        ) -> None:
-        """ Randomly adjust image brightness
-
-        Args:
-            random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
-            delta (int, optional): Integer value for brightness adjustment. Defaults to 100.
-            log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool, optional): If True, the annotation will be adjusted as well. Defaults to False.
-        """
-        super(RandomBrightness, self).__init__(random_chance, log_level, augment_annotation)
-
-        assert 0 <= delta <= 255.0, "Delta must be between 0.0 and 255.0"
-
-        self._delta = delta
-
-    def augment(self, image: Image, value: float) -> Image:
-        """ Augment image brightness """
-        hsv = np.array(image.HSV(), dtype = np.float32)
-
-        hsv[:, :, 1] = hsv[:, :, 1] * value
-        hsv[:, :, 2] = hsv[:, :, 2] * value
-
-        hsv = np.uint8(np.clip(hsv, 0, 255))
-
-        img = cv2.cvtColor(hsv, cv2.COLOR_HSV2BGR)
-
-        image.update(img)
-
-        return image
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly adjust image brightness
-
-        Args:
-            image (Image): Image to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Adjusted image
-            annotation (typing.Any): Adjusted annotation if necessary
-        """
-        value = 1 + np.random.uniform(-self._delta, self._delta) / 255
-
-        image = self.augment(image, value)
-
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = self.augment(annotation, value)
-
-        return image, annotation
-
-
-class RandomRotate(Augmentor):
-    """ Randomly rotate image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        angle: typing.Union[int, typing.List]=30, 
-        borderValue: typing.Tuple[int, int, int]=None,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = True
-        ) -> None:
-        """ Randomly rotate image 
-
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            angle (int, list): Integer value or list of integer values for image rotation
-            borderValue (tuple): Tuple of 3 integers, setting border color for image rotation
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): If True, the annotation will be adjusted as well. Defaults to True.
-        """
-        super(RandomRotate, self).__init__(random_chance, log_level, augment_annotation)
-
-        self._angle = angle
-        self._borderValue = borderValue
-
-    @staticmethod
-    def rotate_image(image: np.ndarray, angle: typing.Union[float, int], borderValue: tuple=(0,0,0), return_rotation_matrix: bool=False) -> np.ndarray:
-        # grab the dimensions of the image and then determine the centre
-        height, width = image.shape[:2]
-        center_x, center_y = (width // 2, height // 2)
-
-        # grab the rotation matrix (applying the negative of the
-        # angle to rotate clockwise), then grab the sine and cosine
-        # (i.e., the rotation components of the matrix)
-        M = cv2.getRotationMatrix2D((center_x, center_y), angle, 1.0)
-        cos = np.abs(M[0, 0])
-        sin = np.abs(M[0, 1])
-
-        # compute the new bounding dimensions of the image
-        nW = int((height * sin) + (width * cos))
-        nH = int((height * cos) + (width * sin))
-
-        # adjust the rotation matrix to take into account translation
-        M[0, 2] += (nW / 2) - center_x
-        M[1, 2] += (nH / 2) - center_y
-
-        # perform the actual rotation and return the image
-        img = cv2.warpAffine(image, M, (nW, nH), borderValue=borderValue)
-
-        if return_rotation_matrix:
-            return img, M
-        
-        return img
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly rotate image
-
-        Args:
-            image (Image): Image to be adjusted
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Adjusted image
-            annotation (typing.Any): Adjusted annotation
-        """
-        # check if angle is list of angles or a single angle value
-        if isinstance(self._angle, list):
-            angle = float(np.random.choice(self._angle))
-        else:
-            angle = float(np.random.uniform(-self._angle, self._angle))
-
-        # generate random border color
-        borderValue = np.random.randint(0, 255, 3) if self._borderValue is None else self._borderValue
-        borderValue = [int(v) for v in borderValue]
-
-        img, rotMat = self.rotate_image(image.numpy(), angle, borderValue, return_rotation_matrix=True)
-
-        if self._augment_annotation:
-            if isinstance(annotation, Image):
-                # perform the actual rotation and return the annotation image
-                annotation_image = self.rotate_image(annotation.numpy(), angle, borderValue=(0, 0, 0))
-                annotation.update(annotation_image)
-            elif isinstance(annotation, Detections):
-                height, width = img.shape[:2]
-                for detection in annotation:
-                    detection.dot(rotMat, width, height)
-
-        image.update(img)
-
-        return image, annotation
-
-
-class RandomErodeDilate(Augmentor):
-    """ Randomly erode and dilate image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        kernel_size: typing.Tuple[int, int]=(1, 1), 
-        log_level: int = logging.INFO,
-        augment_annotation: bool = False,
-        ) -> None:
-        """ Randomly erode and dilate image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            kernel_size (tuple): Tuple of 2 integers, setting kernel size for erosion and dilation
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Boolean value to determine if annotation should be adjusted. Defaults to False.
-        """
-        super(RandomErodeDilate, self).__init__(random_chance, log_level, augment_annotation)
-        self._kernel_size = kernel_size
-        self.kernel = np.ones(self._kernel_size, np.uint8)
-
-    def augment(self, image: Image) -> Image:
-        if np.random.rand() <= 0.5:
-            img = cv2.erode(image.numpy(), self.kernel, iterations=1)
-        else:
-            img = cv2.dilate(image.numpy(), self.kernel, iterations=1)
-
-        image.update(img)
-
-        return image
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly erode and dilate image
-
-        Args:
-            image (Image): Image to be eroded and dilated
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Eroded and dilated image
-            annotation (typing.Any): Adjusted annotation if necessary
-        """
-        image = self.augment(image)
-
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = self.augment(annotation)
-
-        return image, annotation
-
-
-class RandomSharpen(Augmentor):
-    """ Randomly sharpen image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        alpha: float = 0.25,
-        lightness_range: typing.Tuple = (0.75, 2.0),
-        kernel: np.ndarray = None,
-        kernel_anchor: np.ndarray = None,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = False,
-        ) -> None:
-        """ Randomly sharpen image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            alpha (float): Float between 0.0 and 1.0 setting bounds for random probability
-            lightness_range (tuple): Tuple of 2 floats, setting bounds for random lightness change
-            kernel (np.ndarray): Numpy array of kernel for image convolution
-            kernel_anchor (np.ndarray): Numpy array of kernel anchor for image convolution
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Boolean to determine if annotation should be augmented. Defaults to False.
-        """
-        super(RandomSharpen, self).__init__(random_chance, log_level, augment_annotation)
-
-        self._alpha_range = (alpha, 1.0)
-        self._ligtness_range = lightness_range
-        self._lightness_anchor = 8
-
-        self._kernel = np.array([[-1, -1, -1], [-1,  1, -1], [-1, -1, -1]], dtype=np.float32) if kernel is None else kernel
-        self._kernel_anchor = np.array([[0, 0, 0], [0, 1, 0], [0, 0, 0]], dtype=np.float32) if kernel_anchor is None else kernel_anchor
-
-        assert 0 <= alpha <= 1.0, "Alpha must be between 0.0 and 1.0"
-
-    def augment(self, image: Image) -> Image:
-        lightness = np.random.uniform(*self._ligtness_range)
-        alpha = np.random.uniform(*self._alpha_range)
-
-        kernel = self._kernel_anchor  * (self._lightness_anchor + lightness) + self._kernel
-        kernel -= self._kernel_anchor
-        kernel = (1 - alpha) * self._kernel_anchor + alpha * kernel
-
-        # Apply sharpening to each channel
-        r, g, b = cv2.split(image.numpy())
-        r_sharp = cv2.filter2D(r, -1, kernel)
-        g_sharp = cv2.filter2D(g, -1, kernel)
-        b_sharp = cv2.filter2D(b, -1, kernel)
-
-        # Merge the sharpened channels back into the original image
-        image.update(cv2.merge([r_sharp, g_sharp, b_sharp]))
-
-        return image
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly sharpen image
-
-        Args:
-            image (Image): Image to be sharpened
-            annotation (typing.Any): Annotation to be adjusted
-
-        Returns:
-            image (Image): Sharpened image
-            annotation (typing.Any): Adjusted annotation if necessary
-        """
-        image = self.augment(image)
-
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = self.augment(annotation)
-
-        return image, annotation
-    
-
-class RandomGaussianBlur(Augmentor):
-    """ Randomly erode and dilate image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        sigma: typing.Union[int, float] = 1.5,
-        augment_annotation: bool = False,
-        ) -> None:
-        """ Randomly erode and dilate image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            sigma (int, float): maximum sigma value for Gaussian blur. Defaults to 1.5.
-        """
-        super(RandomGaussianBlur, self).__init__(random_chance, log_level, augment_annotation)
-        self.sigma = sigma
-
-    def augment(self, image: Image) -> Image:
-        sigma = np.random.uniform(0, self.sigma)
-        img = cv2.GaussianBlur(image.numpy(), (0, 0), sigma)
-
-        image.update(img)
-
-        return image
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly blurs an image with a Gaussian filter
-
-        Args:
-            image (Image): Image to be blurred
-            annotation (typing.Any): Annotation to be blurred
-
-        Returns:
-            image (Image): Blurred image
-            annotation (typing.Any): Blurred annotation if necessary
-        """
-        image = self.augment(image)
-
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = self.augment(annotation)
-
-        return image, annotation
-    
-
-class RandomSaltAndPepper(Augmentor):
-    """ Randomly add Salt and Pepper noise to image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        salt_vs_pepper: float = 0.5,
-        amount: float = 0.1,
-        augment_annotation: bool = False,
-        ) -> None:
-        """ Randomly add Salt and Pepper noise to image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            salt_vs_pepper (float): ratio of salt vs pepper. Defaults to 0.5.
-            amount (float): proportion of the image to be salted and peppered. Defaults to 0.1.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-        """
-        super(RandomSaltAndPepper, self).__init__(random_chance, log_level, augment_annotation)
-        self.salt_vs_pepper = salt_vs_pepper
-        self.amount = amount
-        
-        assert 0 <= salt_vs_pepper <= 1.0, "salt_vs_pepper must be between 0.0 and 1.0"
-        assert 0 <= amount <= 1.0, "amount must be between 0.0 and 1.0"
-
-    def augment(self, image: Image) -> Image:
-        img = image.numpy()
-        height, width, channels = img.shape
-
-        # Salt mode
-        num_salt = int(self.amount * height * width * self.salt_vs_pepper)
-        row_coords = np.random.randint(0, height, size=num_salt)
-        col_coords = np.random.randint(0, width, size=num_salt)
-        img[row_coords, col_coords, :] = [255, 255, channels]
-
-        # Pepper mode
-        num_pepper = int(self.amount * height * width * (1.0 - self.salt_vs_pepper))
-        row_coords = np.random.randint(0, height, size=num_pepper)
-        col_coords = np.random.randint(0, width, size=num_pepper)
-        img[row_coords, col_coords, :] = [0, 0, channels]
-
-        image.update(img)
-
-        return image
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly add salt and pepper noise to an image
-
-        Args:
-            image (Image): Image to be noised
-            annotation (typing.Any): Annotation to be noised
-
-        Returns:
-            image (Image): Noised image
-            annotation (typing.Any): Noised annotation if necessary
-        """
-        image = self.augment(image)
-
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = self.augment(annotation)
-
-        return image, annotation
-    
-
-class RandomMirror(Augmentor):
-    """ Randomly mirror image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = True,
-        ) -> None:
-        """ Randomly mirror image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to True.
-        """
-        super(RandomMirror, self).__init__(random_chance, log_level, augment_annotation)
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly mirror an image
-
-        Args:
-            image (Image): Image to be mirrored
-            annotation (typing.Any): Annotation to be mirrored
-
-        Returns:
-            image (Image): Mirrored image
-            annotation (typing.Any): Mirrored annotation if necessary
-        """
-        image = image.flip(0)
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = annotation.flip(0)
-
-        elif isinstance(annotation, Detections):
-            for detection in annotation:
-                detection.flip(0)
-
-        return image, annotation
-    
-
-class RandomFlip(Augmentor):
-    """ Randomly flip image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = True,
-        ) -> None:
-        """ Randomly mirror image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to True.
-        """
-        super(RandomFlip, self).__init__(random_chance, log_level, augment_annotation)
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly mirror an image
-
-        Args:
-            image (Image): Image to be flipped
-            annotation (typing.Any): Annotation to be flipped
-
-        Returns:
-            image (Image): Flipped image
-            annotation (typing.Any): Flipped annotation if necessary
-        """
-        image = image.flip(1)
-        if self._augment_annotation and isinstance(annotation, Image):
-            annotation = annotation.flip(1)
-
-        elif isinstance(annotation, Detections):
-            for detection in annotation:
-                detection.flip(1)
-
-        return image, annotation
-    
-
-class RandomDropBlock(Augmentor):
-    """ Randomly drop block from image"""
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = False,
-        block_size_percentage: float = 0.05,
-        keep_prob: float = 0.7,
-        ) -> None:
-        """ Randomly drop block from image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-            block_size_percentage (float): drop block size percentage relative to image size. Defaults to 0.05.
-            keep_prob (float): Probability of keeping the block. Defaults to 0.7.
-        """
-        super(RandomDropBlock, self).__init__(random_chance, log_level, augment_annotation)
-        self.block_size_percentage = block_size_percentage
-        self.keep_prob = keep_prob
-
-    @staticmethod
-    def dropblock(image, block_percent=0.05, keep_prob=0.7):
-        height, width = image.shape[:2]
-        block_size = int(min(height, width) * block_percent)
-        mask = np.ones((height, width), dtype=bool)
-
-        for i in range(0, height - block_size + 1, block_size):
-            for j in range(0, width - block_size + 1, block_size):
-                if np.random.rand() > keep_prob:
-                    mask[i:i+block_size, j:j+block_size] = False
-
-        dropped_image = image * mask[..., np.newaxis]
-        return dropped_image
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly drop block from image
-
-        Args:
-            image (Image): Image to be dropped
-            annotation (typing.Any): Annotation to be dropped
-
-        Returns:
-            image (Image): Dropped image
-            annotation (typing.Any): Dropped annotation if necessary
-        """
-        img = self.dropblock(image.numpy(), self.block_size_percentage, self.keep_prob)
-        image.update(img)
-
-        return image, annotation
-    
-
-class RandomMosaic(Augmentor):
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = True,
-        target_size: typing.Tuple[int, int] = None,
-        ) -> None:
-        """ Randomly merge 4 images into one mosaic image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-            target_size (tuple): Tuple of 2 integers, setting target size for mosaic image. Defaults to None.
-        """
-        super(RandomMosaic, self).__init__(random_chance, log_level, augment_annotation)
-        self.target_size = target_size
-        self.images = []
-        self.annotations = []
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ R
-
-        Args:
-            image (Image): Image to be used for mosaic
-            annotation (typing.Any): Annotation to be used for mosaic
-
-        Returns:
-            image (Image): Mosaic image
-            annotation (typing.Any): Mosaic annotation if necessary
-        """
-        if not isinstance(annotation, Detections):
-            self.logger.error(f"annotation must be Detections object, not {type(annotation)}, skipping augmentor")
-            return image, annotation
-
-        self.images.append(image.numpy())
-        self.annotations.append(annotation)
-
-        if len(self.images) >= 4:
-            # merge images and annotations into one image and annotation
-            if self.target_size is None:
-                # pick smalles target size and resize all images to that size
-                target_size = (min([img.shape[0] for img in self.images]), min([img.shape[1] for img in self.images]))
-            else:
-                target_size = self.target_size
-
-            images = [cv2.resize(img, target_size) for img in self.images[:4]]
-            detections = []
-            new_img = np.concatenate([
-                np.concatenate(images[:2], axis=1), 
-                np.concatenate(images[2:4], axis=1)
-            ], axis=0)
-            
-            height, width = new_img.shape[:2]
-            for index, annotation in enumerate(self.annotations[:4]):
-                if isinstance(annotation, Detections):
-                    for detection in annotation:
-                        xywh = np.array(detection.xywh) / 2
-
-                        if index in [1, 3]:
-                            xywh[0] = xywh[0] + 0.5
-
-                        if index in [2, 3]:
-                            xywh[1] = xywh[1] + 0.5
-
-                        new_detection = Detection(
-                            xywh, 
-                            label=detection.label, 
-                            labels=detection.labels,
-                            confidence=detection.confidence, 
-                            image_path=detection.image_path, 
-                            width=width, 
-                            height=height,
-                            relative=True
-                        )
-                        detections.append(new_detection)
-
-            new_detections = Detections(
-                labels=annotation.labels,
-                width=width,
-                height=height,
-                detections=detections
-            )
-                    
-            image.update(new_img)
-
-            self.images = self.images[4:]
-            self.annotations = self.annotations[4:]
-
-            return image, new_detections
-
-        return image, annotation
-
-
-class RandomZoom(Augmentor):
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = True,
-        object_crop_percentage: float = 0.5,
-        ) -> None:
-        """ Randomly zoom into an image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-            object_crop_percentage (float): Percentage of the object allowed to be cropped. Defaults to 0.5.
-        """
-        super(RandomZoom, self).__init__(random_chance, log_level, augment_annotation)
-        self.object_crop_percentage = object_crop_percentage
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly zoom an image
-
-        Args:
-            image (Image): Image to be used for zoom
-            annotation (typing.Any): Annotation to be used for zoom
-
-        Returns:
-            image (Image): Zoomed image
-            annotation (typing.Any): Zoomed annotation if necessary
-        """
-        if isinstance(annotation, Detections) and self._augment_annotation:
-
-            dets = np.array([detection.xyxy for detection in annotation])
-            min_left = np.min(dets[:, 0])
-            min_top = np.min(dets[:, 1])
-            max_right = np.max(dets[:, 2])
-            max_bottom = np.max(dets[:, 3])
-
-            # Calculate the size of the object
-            object_width = max_right - min_left
-            object_height = max_bottom - min_top
-
-            crop_xmin = np.random.uniform(0, min_left + 0.25 * object_width * self.object_crop_percentage)
-            crop_ymin = np.random.uniform(0, min_top + 0.25 * object_height * self.object_crop_percentage)
-            crop_xmax = np.random.uniform(max_right - 0.25 * object_width * self.object_crop_percentage, 1)
-            crop_ymax = np.random.uniform(max_bottom - 0.25 * object_height * self.object_crop_percentage, 1)
-
-            crop_min_max = np.array([crop_xmin, crop_ymin, crop_xmax, crop_ymax])
-            new_xyxy = (crop_min_max * np.array([image.width, image.height, image.width, image.height])).astype(int)
-            new_image = image.numpy()[new_xyxy[1]:new_xyxy[3], new_xyxy[0]:new_xyxy[2]]
-            image.update(new_image)
-
-            crop_min_ratio = np.array([crop_xmin, crop_ymin, crop_xmin, crop_ymin])
-            crop_max_ratio = np.array([crop_xmax, crop_ymax, crop_xmax, crop_ymax])
-            new_dets = (dets - crop_min_ratio) / (crop_max_ratio - crop_min_ratio)
-
-            detections = []
-            for detection, new_det in zip(annotation, new_dets):
-                new_detection = Detection(
-                    new_det,
-                    label=detection.label, 
-                    labels=detection.labels,
-                    confidence=detection.confidence, 
-                    image_path=detection.image_path, 
-                    width=image.width, 
-                    height=image.height,
-                    relative=True,
-                    bbox_type = BboxType.XYXY
-                )
-
-                detections.append(new_detection)
-
-            annotation = Detections(
-                labels=annotation.labels,
-                width=image.width,
-                height=image.height,
-                detections=detections
-            )
-
-        return image, annotation
-    
-
-class RandomColorMode(Augmentor):
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        log_level: int = logging.INFO,
-        augment_annotation: bool = False,
-        ) -> None:
-        """ Randomly change color mode of an image
-        
-        Args:
-            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-        """
-        super(RandomColorMode, self).__init__(random_chance, log_level, augment_annotation)
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly change color mode of an image
-
-        Args:
-            image (Image): Image to be used for color mode change
-            annotation (typing.Any): Annotation to be used for color mode change
-
-        Returns:
-            image (Image): Color mode changed image
-            annotation (typing.Any): Color mode changed annotation if necessary
-        """
-        color_mode = np.random.choice([cv2.COLOR_BGR2GRAY, cv2.COLOR_BGR2HSV, cv2.COLOR_BGR2LAB, cv2.COLOR_BGR2YCrCb, cv2.COLOR_BGR2RGB])
-        new_image = cv2.cvtColor(image.numpy(), color_mode)
-        if color_mode == cv2.COLOR_BGR2GRAY:
-            new_image = cv2.cvtColor(new_image, cv2.COLOR_GRAY2BGR)
-        image.update(new_image)
-
-        return image, annotation
-    
-
-class RandomElasticTransform(Augmentor):
-    """ Randomly apply elastic transform to an image
-    
-    Attributes:
-        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-        alpha_range (tuple): Tuple of 2 floats, setting bounds for random alpha value. Defaults to (0, 0.1).
-        sigma_range (tuple): Tuple of 2 floats, setting bounds for random sigma value. Defaults to (0.01, 0.02).
-        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-    """
-    def __init__(
-        self, 
-        random_chance: float = 0.5,
-        alpha_range: tuple = (0, 0.1),
-        sigma_range: tuple = (0.01, 0.02),
-        log_level: int = logging.INFO,
-        augment_annotation: bool = True,
-        ) -> None:
-        super(RandomElasticTransform, self).__init__(random_chance, log_level, augment_annotation)
-        self.alpha_range = alpha_range
-        self.sigma_range = sigma_range
-
-    @staticmethod
-    def elastic_transform(image: np.ndarray, alpha: float, sigma: float) -> typing.Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """ Apply elastic transform to an image
-
-        Args:
-            image (np.ndarray): Image to be used for elastic transform
-            alpha (float): Alpha value for elastic transform
-            sigma (float): Sigma value for elastic transform
-
-        Returns:
-            remap_fn (np.ndarray): Elastic transformed image
-            dx (np.ndarray): X-axis displacement
-            dy (np.ndarray): Y-axis displacement
-        """
-        height, width, channels = image.shape
-        dx = np.random.rand(height, width).astype(np.float32) * 2 - 1
-        dy = np.random.rand(height, width).astype(np.float32) * 2 - 1
-
-        cv2.GaussianBlur(dx, (0, 0), sigma, dst=dx)
-        cv2.GaussianBlur(dy, (0, 0), sigma, dst=dy)
-
-        dx *= alpha
-        dy *= alpha
-
-        x, y = np.meshgrid(np.arange(width), np.arange(height))
-
-        map_x = np.float32(x + dx)
-        map_y = np.float32(y + dy)
-
-        remap_fn = cv2.remap(image, map_x, map_y, interpolation=cv2.INTER_LINEAR, borderMode=cv2.BORDER_REFLECT)
-
-        return remap_fn, dx, dy
-
-    @randomness_decorator
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Randomly apply elastic transform to an image
-
-        Args:
-            image (Image): Image to be used for elastic transform
-            annotation (typing.Any): Annotation to be used for elastic transform
-
-        Returns:
-            image (Image): Elastic transformed image
-            annotation (typing.Any): Elastic transformed annotation if necessary
-        """
-        alpha = image.width * np.random.uniform(*self.alpha_range)
-        sigma = image.width * np.random.uniform(*self.sigma_range)
-        new_image, dx, dy = self.elastic_transform(image.numpy(), alpha, sigma)
-        image.update(new_image)
-
-        if isinstance(annotation, Detections) and self._augment_annotation:
-            detections = []
-            for detection in annotation:
-                x_min, y_min, x_max, y_max = detection.xyxy_abs
-                new_x_min = min(max(0, x_min + dx[y_min, x_min]), image.width - 1)
-                new_y_min = min(max(0, y_min + dy[y_min, x_min]), image.height - 1)
-                new_x_max = min(max(0, x_max + dx[y_max, x_max]), image.width - 1)
-                new_y_max = min(max(0, y_max + dy[y_max, x_max]), image.height - 1)
-                detections.append(
-                    Detection(
-                        [new_x_min, new_y_min, new_x_max, new_y_max],
-                        label=detection.label, 
-                        labels=detection.labels,
-                        confidence=detection.confidence, 
-                        image_path=detection.image_path, 
-                        width=image.width, 
-                        height=image.height,
-                        relative=False,
-                        bbox_type = BboxType.XYXY
-                    )
-                )
-            
-            annotation = Detections(
-                labels=annotation.labels,
-                width=image.width,
-                height=image.height,
-                detections=detections
-            )
-
-        return image, annotation
-
-
-class RandomAudioNoise(Augmentor):
-    """ Randomly add noise to audio
-
-    Attributes:
-        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-        max_noise_ratio (float): Maximum noise ratio to be added to audio. Defaults to 0.1.
-    """
-    def __init__(
-            self, 
-            random_chance: float = 0.5,
-            log_level: int = logging.INFO,
-            augment_annotation: bool = False,
-            max_noise_ratio: float = 0.1,
-        ) -> None:
-        super(RandomAudioNoise, self).__init__(random_chance, log_level, augment_annotation)
-        self.max_noise_ratio = max_noise_ratio
-
-    def augment(self, audio: Audio) -> Audio:
-        noise = np.random.uniform(-1, 1, len(audio))
-        noise_ratio = np.random.uniform(0, self.max_noise_ratio)
-        audio_noisy = audio + noise_ratio * noise
-
-        return audio_noisy
-    
-
-class RandomAudioPitchShift(Augmentor):
-    """ Randomly add noise to audio
-
-    Attributes:
-        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-        max_n_steps (int): Maximum number of steps to shift audio. Defaults to 5.
-    """
-    def __init__(
-            self, 
-            random_chance: float = 0.5,
-            log_level: int = logging.INFO,
-            augment_annotation: bool = False,
-            max_n_steps: int = 5,
-        ) -> None:
-        super(RandomAudioPitchShift, self).__init__(random_chance, log_level, augment_annotation)
-        self.max_n_steps = max_n_steps
-
-        # import librosa using importlib
-        try:
-            self.librosa = importlib.import_module('librosa')
-            print("librosa version:", self.librosa.__version__)
-        except ImportError:
-            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
-
-    def augment(self, audio: Audio) -> Audio:
-        random_n_steps = np.random.randint(-self.max_n_steps, self.max_n_steps)
-        # changing default res_type "kaiser_best" to "linear" for speed and memory efficiency
-        shift_audio = self.librosa.effects.pitch_shift(
-            audio.numpy(), sr=audio.sample_rate, n_steps=random_n_steps, res_type="linear"
-            )
-        audio.audio = shift_audio
-
-        return audio
-    
-
-class RandomAudioTimeStretch(Augmentor):
-    """ Randomly add noise to audio
-
-    Attributes:
-        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
-        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
-        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
-        min_rate (float): Minimum rate to stretch audio. Defaults to 0.8.
-        max_rate (float): Maximum rate to stretch audio. Defaults to 1.2.
-    """
-    def __init__(
-            self, 
-            random_chance: float = 0.5,
-            log_level: int = logging.INFO,
-            augment_annotation: bool = False,
-            min_rate: float = 0.8,
-            max_rate: float = 1.2
-        ) -> None:
-        super(RandomAudioTimeStretch, self).__init__(random_chance, log_level, augment_annotation)
-        self.min_rate = min_rate
-        self.max_rate = max_rate
-
-        try:
-            librosa.__version__
-        except ImportError:
-            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
-
-    def augment(self, audio: Audio) -> Audio:
-        random_rate = np.random.uniform(self.min_rate, self.max_rate)
-        stretch_audio = librosa.effects.time_stretch(audio.numpy(), rate=random_rate)
-        audio.audio = stretch_audio
-
+import cv2
+import typing
+import numpy as np
+import importlib
+import logging
+
+from . import Image
+from mltu.annotations.audio import Audio
+from mltu.annotations.detections import Detections, Detection, BboxType
+
+""" 
+Implemented image augmentors:
+- RandomBrightness
+- RandomRotate
+- RandomErodeDilate
+- RandomSharpen
+- RandomGaussianBlur
+- RandomSaltAndPepper
+- RandomMirror
+- RandomFlip
+- RandomDropBlock
+- RandomMosaic
+- RandomZoom
+- RandomColorMode
+- RandomElasticTransform
+
+Implemented audio augmentors:
+- RandomAudioNoise
+- RandomAudioPitchShift
+- RandomAudioTimeStretch
+"""
+
+def randomness_decorator(func):
+    """ Decorator for randomness """
+    def wrapper(self, data: typing.Union[Image, Audio], annotation: typing.Any) -> typing.Tuple[typing.Union[Image, Audio], typing.Any]:
+        """ Decorator for randomness and type checking
+
+        Args:
+            data (typing.Union[Image, Audio]): Image or Audio object to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            data (typing.Union[Image, Audio]): Adjusted image or audio
+            annotation (typing.Any): Adjusted annotation
+        """
+        # check if image is Image object
+        if not isinstance(data, (Image, Audio)):
+            self.logger.error(f"data must be Image or Audio object, not {type(data)}, skipping augmentor")
+            # TODO instead of error convert image into Image object
+            # TODO instead of error convert audio into Audio object
+            return data, annotation
+
+        if np.random.rand() > self._random_chance:
+            return data, annotation
+
+        # return result of function
+        return func(self, data, annotation)
+
+    return wrapper
+
+
+class Augmentor:
+    """ Object that should be inherited by all augmentors
+
+    Args:
+        random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
+        log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
+    """
+    def __init__(self, random_chance: float=0.5, log_level: int = logging.INFO, augment_annotation: bool = False) -> None:
+        self._random_chance = random_chance
+        self._log_level = log_level
+        self._augment_annotation = augment_annotation
+
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(logging.INFO)
+
+        assert 0 <= self._random_chance <= 1.0, "random chance must be between 0.0 and 1.0"
+
+    def augment(self, data: typing.Union[Image, Audio]):
+        """ Augment data """
+        raise NotImplementedError
+
+    @randomness_decorator
+    def __call__(self, data: typing.Union[Image, Audio], annotation: typing.Any) -> typing.Tuple[typing.Union[Image, Audio], typing.Any]:
+        """ Randomly add noise to audio
+
+        Args:
+            data (typing.Union[Image, Audio]): Image or Audio object to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            data (typing.Union[Image, Audio]): Adjusted image or audio
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        data = self.augment(data)
+
+        if self._augment_annotation and isinstance(annotation, np.ndarray):
+            annotation = self.augment(annotation)
+
+        return data, annotation
+
+
+class RandomBrightness(Augmentor):
+    """ Randomly adjust image brightness """
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        delta: int = 100,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = False
+        ) -> None:
+        """ Randomly adjust image brightness
+
+        Args:
+            random_chance (float, optional): Chance of applying the augmentor. Where 0.0 is never and 1.0 is always. Defaults to 0.5.
+            delta (int, optional): Integer value for brightness adjustment. Defaults to 100.
+            log_level (int, optional): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool, optional): If True, the annotation will be adjusted as well. Defaults to False.
+        """
+        super(RandomBrightness, self).__init__(random_chance, log_level, augment_annotation)
+
+        assert 0 <= delta <= 255.0, "Delta must be between 0.0 and 255.0"
+
+        self._delta = delta
+
+    def augment(self, image: Image, value: float) -> Image:
+        """ Augment image brightness """
+        hsv = np.array(image.HSV(), dtype = np.float32)
+
+        hsv[:, :, 1] = hsv[:, :, 1] * value
+        hsv[:, :, 2] = hsv[:, :, 2] * value
+
+        hsv = np.uint8(np.clip(hsv, 0, 255))
+
+        img = cv2.cvtColor(hsv, cv2.COLOR_HSV2BGR)
+
+        image.update(img)
+
+        return image
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly adjust image brightness
+
+        Args:
+            image (Image): Image to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Adjusted image
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        value = 1 + np.random.uniform(-self._delta, self._delta) / 255
+
+        image = self.augment(image, value)
+
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = self.augment(annotation, value)
+
+        return image, annotation
+
+
+class RandomRotate(Augmentor):
+    """ Randomly rotate image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        angle: typing.Union[int, typing.List]=30, 
+        borderValue: typing.Tuple[int, int, int]=None,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = True
+        ) -> None:
+        """ Randomly rotate image 
+
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            angle (int, list): Integer value or list of integer values for image rotation
+            borderValue (tuple): Tuple of 3 integers, setting border color for image rotation
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): If True, the annotation will be adjusted as well. Defaults to True.
+        """
+        super(RandomRotate, self).__init__(random_chance, log_level, augment_annotation)
+
+        self._angle = angle
+        self._borderValue = borderValue
+
+    @staticmethod
+    def rotate_image(image: np.ndarray, angle: typing.Union[float, int], borderValue: tuple=(0,0,0), return_rotation_matrix: bool=False) -> np.ndarray:
+        # grab the dimensions of the image and then determine the centre
+        height, width = image.shape[:2]
+        center_x, center_y = (width // 2, height // 2)
+
+        # grab the rotation matrix (applying the negative of the
+        # angle to rotate clockwise), then grab the sine and cosine
+        # (i.e., the rotation components of the matrix)
+        M = cv2.getRotationMatrix2D((center_x, center_y), angle, 1.0)
+        cos = np.abs(M[0, 0])
+        sin = np.abs(M[0, 1])
+
+        # compute the new bounding dimensions of the image
+        nW = int((height * sin) + (width * cos))
+        nH = int((height * cos) + (width * sin))
+
+        # adjust the rotation matrix to take into account translation
+        M[0, 2] += (nW / 2) - center_x
+        M[1, 2] += (nH / 2) - center_y
+
+        # perform the actual rotation and return the image
+        img = cv2.warpAffine(image, M, (nW, nH), borderValue=borderValue)
+
+        if return_rotation_matrix:
+            return img, M
+        
+        return img
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly rotate image
+
+        Args:
+            image (Image): Image to be adjusted
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Adjusted image
+            annotation (typing.Any): Adjusted annotation
+        """
+        # check if angle is list of angles or a single angle value
+        if isinstance(self._angle, list):
+            angle = float(np.random.choice(self._angle))
+        else:
+            angle = float(np.random.uniform(-self._angle, self._angle))
+
+        # generate random border color
+        borderValue = np.random.randint(0, 255, 3) if self._borderValue is None else self._borderValue
+        borderValue = [int(v) for v in borderValue]
+
+        img, rotMat = self.rotate_image(image.numpy(), angle, borderValue, return_rotation_matrix=True)
+
+        if self._augment_annotation:
+            if isinstance(annotation, Image):
+                # perform the actual rotation and return the annotation image
+                annotation_image = self.rotate_image(annotation.numpy(), angle, borderValue=(0, 0, 0))
+                annotation.update(annotation_image)
+            elif isinstance(annotation, Detections):
+                height, width = img.shape[:2]
+                for detection in annotation:
+                    detection.dot(rotMat, width, height)
+
+        image.update(img)
+
+        return image, annotation
+
+
+class RandomErodeDilate(Augmentor):
+    """ Randomly erode and dilate image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        kernel_size: typing.Tuple[int, int]=(1, 1), 
+        log_level: int = logging.INFO,
+        augment_annotation: bool = False,
+        ) -> None:
+        """ Randomly erode and dilate image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            kernel_size (tuple): Tuple of 2 integers, setting kernel size for erosion and dilation
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Boolean value to determine if annotation should be adjusted. Defaults to False.
+        """
+        super(RandomErodeDilate, self).__init__(random_chance, log_level, augment_annotation)
+        self._kernel_size = kernel_size
+        self.kernel = np.ones(self._kernel_size, np.uint8)
+
+    def augment(self, image: Image) -> Image:
+        if np.random.rand() <= 0.5:
+            img = cv2.erode(image.numpy(), self.kernel, iterations=1)
+        else:
+            img = cv2.dilate(image.numpy(), self.kernel, iterations=1)
+
+        image.update(img)
+
+        return image
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly erode and dilate image
+
+        Args:
+            image (Image): Image to be eroded and dilated
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Eroded and dilated image
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        image = self.augment(image)
+
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = self.augment(annotation)
+
+        return image, annotation
+
+
+class RandomSharpen(Augmentor):
+    """ Randomly sharpen image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        alpha: float = 0.25,
+        lightness_range: typing.Tuple = (0.75, 2.0),
+        kernel: np.ndarray = None,
+        kernel_anchor: np.ndarray = None,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = False,
+        ) -> None:
+        """ Randomly sharpen image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            alpha (float): Float between 0.0 and 1.0 setting bounds for random probability
+            lightness_range (tuple): Tuple of 2 floats, setting bounds for random lightness change
+            kernel (np.ndarray): Numpy array of kernel for image convolution
+            kernel_anchor (np.ndarray): Numpy array of kernel anchor for image convolution
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Boolean to determine if annotation should be augmented. Defaults to False.
+        """
+        super(RandomSharpen, self).__init__(random_chance, log_level, augment_annotation)
+
+        self._alpha_range = (alpha, 1.0)
+        self._ligtness_range = lightness_range
+        self._lightness_anchor = 8
+
+        self._kernel = np.array([[-1, -1, -1], [-1,  1, -1], [-1, -1, -1]], dtype=np.float32) if kernel is None else kernel
+        self._kernel_anchor = np.array([[0, 0, 0], [0, 1, 0], [0, 0, 0]], dtype=np.float32) if kernel_anchor is None else kernel_anchor
+
+        assert 0 <= alpha <= 1.0, "Alpha must be between 0.0 and 1.0"
+
+    def augment(self, image: Image) -> Image:
+        lightness = np.random.uniform(*self._ligtness_range)
+        alpha = np.random.uniform(*self._alpha_range)
+
+        kernel = self._kernel_anchor  * (self._lightness_anchor + lightness) + self._kernel
+        kernel -= self._kernel_anchor
+        kernel = (1 - alpha) * self._kernel_anchor + alpha * kernel
+
+        # Apply sharpening to each channel
+        r, g, b = cv2.split(image.numpy())
+        r_sharp = cv2.filter2D(r, -1, kernel)
+        g_sharp = cv2.filter2D(g, -1, kernel)
+        b_sharp = cv2.filter2D(b, -1, kernel)
+
+        # Merge the sharpened channels back into the original image
+        image.update(cv2.merge([r_sharp, g_sharp, b_sharp]))
+
+        return image
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly sharpen image
+
+        Args:
+            image (Image): Image to be sharpened
+            annotation (typing.Any): Annotation to be adjusted
+
+        Returns:
+            image (Image): Sharpened image
+            annotation (typing.Any): Adjusted annotation if necessary
+        """
+        image = self.augment(image)
+
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = self.augment(annotation)
+
+        return image, annotation
+    
+
+class RandomGaussianBlur(Augmentor):
+    """ Randomly erode and dilate image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        sigma: typing.Union[int, float] = 1.5,
+        augment_annotation: bool = False,
+        ) -> None:
+        """ Randomly erode and dilate image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            sigma (int, float): maximum sigma value for Gaussian blur. Defaults to 1.5.
+        """
+        super(RandomGaussianBlur, self).__init__(random_chance, log_level, augment_annotation)
+        self.sigma = sigma
+
+    def augment(self, image: Image) -> Image:
+        sigma = np.random.uniform(0, self.sigma)
+        img = cv2.GaussianBlur(image.numpy(), (0, 0), sigma)
+
+        image.update(img)
+
+        return image
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly blurs an image with a Gaussian filter
+
+        Args:
+            image (Image): Image to be blurred
+            annotation (typing.Any): Annotation to be blurred
+
+        Returns:
+            image (Image): Blurred image
+            annotation (typing.Any): Blurred annotation if necessary
+        """
+        image = self.augment(image)
+
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = self.augment(annotation)
+
+        return image, annotation
+    
+
+class RandomSaltAndPepper(Augmentor):
+    """ Randomly add Salt and Pepper noise to image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        salt_vs_pepper: float = 0.5,
+        amount: float = 0.1,
+        augment_annotation: bool = False,
+        ) -> None:
+        """ Randomly add Salt and Pepper noise to image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            salt_vs_pepper (float): ratio of salt vs pepper. Defaults to 0.5.
+            amount (float): proportion of the image to be salted and peppered. Defaults to 0.1.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+        """
+        super(RandomSaltAndPepper, self).__init__(random_chance, log_level, augment_annotation)
+        self.salt_vs_pepper = salt_vs_pepper
+        self.amount = amount
+        
+        assert 0 <= salt_vs_pepper <= 1.0, "salt_vs_pepper must be between 0.0 and 1.0"
+        assert 0 <= amount <= 1.0, "amount must be between 0.0 and 1.0"
+
+    def augment(self, image: Image) -> Image:
+        img = image.numpy()
+        height, width, channels = img.shape
+
+        # Salt mode
+        num_salt = int(self.amount * height * width * self.salt_vs_pepper)
+        row_coords = np.random.randint(0, height, size=num_salt)
+        col_coords = np.random.randint(0, width, size=num_salt)
+        img[row_coords, col_coords, :] = [255, 255, channels]
+
+        # Pepper mode
+        num_pepper = int(self.amount * height * width * (1.0 - self.salt_vs_pepper))
+        row_coords = np.random.randint(0, height, size=num_pepper)
+        col_coords = np.random.randint(0, width, size=num_pepper)
+        img[row_coords, col_coords, :] = [0, 0, channels]
+
+        image.update(img)
+
+        return image
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly add salt and pepper noise to an image
+
+        Args:
+            image (Image): Image to be noised
+            annotation (typing.Any): Annotation to be noised
+
+        Returns:
+            image (Image): Noised image
+            annotation (typing.Any): Noised annotation if necessary
+        """
+        image = self.augment(image)
+
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = self.augment(annotation)
+
+        return image, annotation
+    
+
+class RandomMirror(Augmentor):
+    """ Randomly mirror image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = True,
+        ) -> None:
+        """ Randomly mirror image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to True.
+        """
+        super(RandomMirror, self).__init__(random_chance, log_level, augment_annotation)
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly mirror an image
+
+        Args:
+            image (Image): Image to be mirrored
+            annotation (typing.Any): Annotation to be mirrored
+
+        Returns:
+            image (Image): Mirrored image
+            annotation (typing.Any): Mirrored annotation if necessary
+        """
+        image = image.flip(0)
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = annotation.flip(0)
+
+        elif isinstance(annotation, Detections):
+            for detection in annotation:
+                detection.flip(0)
+
+        return image, annotation
+    
+
+class RandomFlip(Augmentor):
+    """ Randomly flip image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = True,
+        ) -> None:
+        """ Randomly mirror image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to True.
+        """
+        super(RandomFlip, self).__init__(random_chance, log_level, augment_annotation)
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly mirror an image
+
+        Args:
+            image (Image): Image to be flipped
+            annotation (typing.Any): Annotation to be flipped
+
+        Returns:
+            image (Image): Flipped image
+            annotation (typing.Any): Flipped annotation if necessary
+        """
+        image = image.flip(1)
+        if self._augment_annotation and isinstance(annotation, Image):
+            annotation = annotation.flip(1)
+
+        elif isinstance(annotation, Detections):
+            for detection in annotation:
+                detection.flip(1)
+
+        return image, annotation
+    
+
+class RandomDropBlock(Augmentor):
+    """ Randomly drop block from image"""
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = False,
+        block_size_percentage: float = 0.05,
+        keep_prob: float = 0.7,
+        ) -> None:
+        """ Randomly drop block from image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+            block_size_percentage (float): drop block size percentage relative to image size. Defaults to 0.05.
+            keep_prob (float): Probability of keeping the block. Defaults to 0.7.
+        """
+        super(RandomDropBlock, self).__init__(random_chance, log_level, augment_annotation)
+        self.block_size_percentage = block_size_percentage
+        self.keep_prob = keep_prob
+
+    @staticmethod
+    def dropblock(image, block_percent=0.05, keep_prob=0.7):
+        height, width = image.shape[:2]
+        block_size = int(min(height, width) * block_percent)
+        mask = np.ones((height, width), dtype=bool)
+
+        for i in range(0, height - block_size + 1, block_size):
+            for j in range(0, width - block_size + 1, block_size):
+                if np.random.rand() > keep_prob:
+                    mask[i:i+block_size, j:j+block_size] = False
+
+        dropped_image = image * mask[..., np.newaxis]
+        return dropped_image
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly drop block from image
+
+        Args:
+            image (Image): Image to be dropped
+            annotation (typing.Any): Annotation to be dropped
+
+        Returns:
+            image (Image): Dropped image
+            annotation (typing.Any): Dropped annotation if necessary
+        """
+        img = self.dropblock(image.numpy(), self.block_size_percentage, self.keep_prob)
+        image.update(img)
+
+        return image, annotation
+    
+
+class RandomMosaic(Augmentor):
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = True,
+        target_size: typing.Tuple[int, int] = None,
+        ) -> None:
+        """ Randomly merge 4 images into one mosaic image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+            target_size (tuple): Tuple of 2 integers, setting target size for mosaic image. Defaults to None.
+        """
+        super(RandomMosaic, self).__init__(random_chance, log_level, augment_annotation)
+        self.target_size = target_size
+        self.images = []
+        self.annotations = []
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ R
+
+        Args:
+            image (Image): Image to be used for mosaic
+            annotation (typing.Any): Annotation to be used for mosaic
+
+        Returns:
+            image (Image): Mosaic image
+            annotation (typing.Any): Mosaic annotation if necessary
+        """
+        if not isinstance(annotation, Detections):
+            self.logger.error(f"annotation must be Detections object, not {type(annotation)}, skipping augmentor")
+            return image, annotation
+
+        self.images.append(image.numpy())
+        self.annotations.append(annotation)
+
+        if len(self.images) >= 4:
+            # merge images and annotations into one image and annotation
+            if self.target_size is None:
+                # pick smalles target size and resize all images to that size
+                target_size = (min([img.shape[0] for img in self.images]), min([img.shape[1] for img in self.images]))
+            else:
+                target_size = self.target_size
+
+            images = [cv2.resize(img, target_size) for img in self.images[:4]]
+            detections = []
+            new_img = np.concatenate([
+                np.concatenate(images[:2], axis=1), 
+                np.concatenate(images[2:4], axis=1)
+            ], axis=0)
+            
+            height, width = new_img.shape[:2]
+            for index, annotation in enumerate(self.annotations[:4]):
+                if isinstance(annotation, Detections):
+                    for detection in annotation:
+                        xywh = np.array(detection.xywh) / 2
+
+                        if index in [1, 3]:
+                            xywh[0] = xywh[0] + 0.5
+
+                        if index in [2, 3]:
+                            xywh[1] = xywh[1] + 0.5
+
+                        new_detection = Detection(
+                            xywh, 
+                            label=detection.label, 
+                            labels=detection.labels,
+                            confidence=detection.confidence, 
+                            image_path=detection.image_path, 
+                            width=width, 
+                            height=height,
+                            relative=True
+                        )
+                        detections.append(new_detection)
+
+            new_detections = Detections(
+                labels=annotation.labels,
+                width=width,
+                height=height,
+                detections=detections
+            )
+                    
+            image.update(new_img)
+
+            self.images = self.images[4:]
+            self.annotations = self.annotations[4:]
+
+            return image, new_detections
+
+        return image, annotation
+
+
+class RandomZoom(Augmentor):
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = True,
+        object_crop_percentage: float = 0.5,
+        ) -> None:
+        """ Randomly zoom into an image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+            object_crop_percentage (float): Percentage of the object allowed to be cropped. Defaults to 0.5.
+        """
+        super(RandomZoom, self).__init__(random_chance, log_level, augment_annotation)
+        self.object_crop_percentage = object_crop_percentage
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly zoom an image
+
+        Args:
+            image (Image): Image to be used for zoom
+            annotation (typing.Any): Annotation to be used for zoom
+
+        Returns:
+            image (Image): Zoomed image
+            annotation (typing.Any): Zoomed annotation if necessary
+        """
+        if isinstance(annotation, Detections) and self._augment_annotation:
+
+            dets = np.array([detection.xyxy for detection in annotation])
+            min_left = np.min(dets[:, 0])
+            min_top = np.min(dets[:, 1])
+            max_right = np.max(dets[:, 2])
+            max_bottom = np.max(dets[:, 3])
+
+            # Calculate the size of the object
+            object_width = max_right - min_left
+            object_height = max_bottom - min_top
+
+            crop_xmin = np.random.uniform(0, min_left + 0.25 * object_width * self.object_crop_percentage)
+            crop_ymin = np.random.uniform(0, min_top + 0.25 * object_height * self.object_crop_percentage)
+            crop_xmax = np.random.uniform(max_right - 0.25 * object_width * self.object_crop_percentage, 1)
+            crop_ymax = np.random.uniform(max_bottom - 0.25 * object_height * self.object_crop_percentage, 1)
+
+            crop_min_max = np.array([crop_xmin, crop_ymin, crop_xmax, crop_ymax])
+            new_xyxy = (crop_min_max * np.array([image.width, image.height, image.width, image.height])).astype(int)
+            new_image = image.numpy()[new_xyxy[1]:new_xyxy[3], new_xyxy[0]:new_xyxy[2]]
+            image.update(new_image)
+
+            crop_min_ratio = np.array([crop_xmin, crop_ymin, crop_xmin, crop_ymin])
+            crop_max_ratio = np.array([crop_xmax, crop_ymax, crop_xmax, crop_ymax])
+            new_dets = (dets - crop_min_ratio) / (crop_max_ratio - crop_min_ratio)
+
+            detections = []
+            for detection, new_det in zip(annotation, new_dets):
+                new_detection = Detection(
+                    new_det,
+                    label=detection.label, 
+                    labels=detection.labels,
+                    confidence=detection.confidence, 
+                    image_path=detection.image_path, 
+                    width=image.width, 
+                    height=image.height,
+                    relative=True,
+                    bbox_type = BboxType.XYXY
+                )
+
+                detections.append(new_detection)
+
+            annotation = Detections(
+                labels=annotation.labels,
+                width=image.width,
+                height=image.height,
+                detections=detections
+            )
+
+        return image, annotation
+    
+
+class RandomColorMode(Augmentor):
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        log_level: int = logging.INFO,
+        augment_annotation: bool = False,
+        ) -> None:
+        """ Randomly change color mode of an image
+        
+        Args:
+            random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+            log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+            augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+        """
+        super(RandomColorMode, self).__init__(random_chance, log_level, augment_annotation)
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly change color mode of an image
+
+        Args:
+            image (Image): Image to be used for color mode change
+            annotation (typing.Any): Annotation to be used for color mode change
+
+        Returns:
+            image (Image): Color mode changed image
+            annotation (typing.Any): Color mode changed annotation if necessary
+        """
+        color_mode = np.random.choice([cv2.COLOR_BGR2GRAY, cv2.COLOR_BGR2HSV, cv2.COLOR_BGR2LAB, cv2.COLOR_BGR2YCrCb, cv2.COLOR_BGR2RGB])
+        new_image = cv2.cvtColor(image.numpy(), color_mode)
+        if color_mode == cv2.COLOR_BGR2GRAY:
+            new_image = cv2.cvtColor(new_image, cv2.COLOR_GRAY2BGR)
+        image.update(new_image)
+
+        return image, annotation
+    
+
+class RandomElasticTransform(Augmentor):
+    """ Randomly apply elastic transform to an image
+    
+    Attributes:
+        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+        alpha_range (tuple): Tuple of 2 floats, setting bounds for random alpha value. Defaults to (0, 0.1).
+        sigma_range (tuple): Tuple of 2 floats, setting bounds for random sigma value. Defaults to (0.01, 0.02).
+        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+    """
+    def __init__(
+        self, 
+        random_chance: float = 0.5,
+        alpha_range: tuple = (0, 0.1),
+        sigma_range: tuple = (0.01, 0.02),
+        log_level: int = logging.INFO,
+        augment_annotation: bool = True,
+        ) -> None:
+        super(RandomElasticTransform, self).__init__(random_chance, log_level, augment_annotation)
+        self.alpha_range = alpha_range
+        self.sigma_range = sigma_range
+
+    @staticmethod
+    def elastic_transform(image: np.ndarray, alpha: float, sigma: float) -> typing.Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """ Apply elastic transform to an image
+
+        Args:
+            image (np.ndarray): Image to be used for elastic transform
+            alpha (float): Alpha value for elastic transform
+            sigma (float): Sigma value for elastic transform
+
+        Returns:
+            remap_fn (np.ndarray): Elastic transformed image
+            dx (np.ndarray): X-axis displacement
+            dy (np.ndarray): Y-axis displacement
+        """
+        height, width, channels = image.shape
+        dx = np.random.rand(height, width).astype(np.float32) * 2 - 1
+        dy = np.random.rand(height, width).astype(np.float32) * 2 - 1
+
+        cv2.GaussianBlur(dx, (0, 0), sigma, dst=dx)
+        cv2.GaussianBlur(dy, (0, 0), sigma, dst=dy)
+
+        dx *= alpha
+        dy *= alpha
+
+        x, y = np.meshgrid(np.arange(width), np.arange(height))
+
+        map_x = np.float32(x + dx)
+        map_y = np.float32(y + dy)
+
+        remap_fn = cv2.remap(image, map_x, map_y, interpolation=cv2.INTER_LINEAR, borderMode=cv2.BORDER_REFLECT)
+
+        return remap_fn, dx, dy
+
+    @randomness_decorator
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Randomly apply elastic transform to an image
+
+        Args:
+            image (Image): Image to be used for elastic transform
+            annotation (typing.Any): Annotation to be used for elastic transform
+
+        Returns:
+            image (Image): Elastic transformed image
+            annotation (typing.Any): Elastic transformed annotation if necessary
+        """
+        alpha = image.width * np.random.uniform(*self.alpha_range)
+        sigma = image.width * np.random.uniform(*self.sigma_range)
+        new_image, dx, dy = self.elastic_transform(image.numpy(), alpha, sigma)
+        image.update(new_image)
+
+        if isinstance(annotation, Detections) and self._augment_annotation:
+            detections = []
+            for detection in annotation:
+                x_min, y_min, x_max, y_max = detection.xyxy_abs
+                x_max = min(x_max, dx.shape[1] - 1)
+                y_max = min(y_max, dy.shape[0] - 1)
+                new_x_min = min(max(0, x_min + dx[y_min, x_min]), image.width - 1)
+                new_y_min = min(max(0, y_min + dy[y_min, x_min]), image.height - 1)
+                new_x_max = min(max(0, x_max + dx[y_max, x_max]), image.width - 1)
+                new_y_max = min(max(0, y_max + dy[y_max, x_max]), image.height - 1)
+                detections.append(
+                    Detection(
+                        [new_x_min, new_y_min, new_x_max, new_y_max],
+                        label=detection.label, 
+                        labels=detection.labels,
+                        confidence=detection.confidence, 
+                        image_path=detection.image_path, 
+                        width=image.width, 
+                        height=image.height,
+                        relative=False,
+                        bbox_type = BboxType.XYXY
+                    )
+                )
+            
+            annotation = Detections(
+                labels=annotation.labels,
+                width=image.width,
+                height=image.height,
+                detections=detections
+            )
+
+        return image, annotation
+
+
+class RandomAudioNoise(Augmentor):
+    """ Randomly add noise to audio
+
+    Attributes:
+        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+        max_noise_ratio (float): Maximum noise ratio to be added to audio. Defaults to 0.1.
+    """
+    def __init__(
+            self, 
+            random_chance: float = 0.5,
+            log_level: int = logging.INFO,
+            augment_annotation: bool = False,
+            max_noise_ratio: float = 0.1,
+        ) -> None:
+        super(RandomAudioNoise, self).__init__(random_chance, log_level, augment_annotation)
+        self.max_noise_ratio = max_noise_ratio
+
+    def augment(self, audio: Audio) -> Audio:
+        noise = np.random.uniform(-1, 1, len(audio))
+        noise_ratio = np.random.uniform(0, self.max_noise_ratio)
+        audio_noisy = audio + noise_ratio * noise
+
+        return audio_noisy
+    
+
+class RandomAudioPitchShift(Augmentor):
+    """ Randomly add noise to audio
+
+    Attributes:
+        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+        max_n_steps (int): Maximum number of steps to shift audio. Defaults to 5.
+    """
+    def __init__(
+            self, 
+            random_chance: float = 0.5,
+            log_level: int = logging.INFO,
+            augment_annotation: bool = False,
+            max_n_steps: int = 5,
+        ) -> None:
+        super(RandomAudioPitchShift, self).__init__(random_chance, log_level, augment_annotation)
+        self.max_n_steps = max_n_steps
+
+        # import librosa using importlib
+        try:
+            self.librosa = importlib.import_module('librosa')
+            print("librosa version:", self.librosa.__version__)
+        except ImportError:
+            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
+
+    def augment(self, audio: Audio) -> Audio:
+        random_n_steps = np.random.randint(-self.max_n_steps, self.max_n_steps)
+        # changing default res_type "kaiser_best" to "linear" for speed and memory efficiency
+        shift_audio = self.librosa.effects.pitch_shift(
+            audio.numpy(), sr=audio.sample_rate, n_steps=random_n_steps, res_type="linear"
+            )
+        audio.audio = shift_audio
+
+        return audio
+    
+
+class RandomAudioTimeStretch(Augmentor):
+    """ Randomly add noise to audio
+
+    Attributes:
+        random_chance (float): Float between 0.0 and 1.0 setting bounds for random probability. Defaults to 0.5.
+        log_level (int): Log level for the augmentor. Defaults to logging.INFO.
+        augment_annotation (bool): Whether to augment the annotation. Defaults to False.
+        min_rate (float): Minimum rate to stretch audio. Defaults to 0.8.
+        max_rate (float): Maximum rate to stretch audio. Defaults to 1.2.
+    """
+    def __init__(
+            self, 
+            random_chance: float = 0.5,
+            log_level: int = logging.INFO,
+            augment_annotation: bool = False,
+            min_rate: float = 0.8,
+            max_rate: float = 1.2
+        ) -> None:
+        super(RandomAudioTimeStretch, self).__init__(random_chance, log_level, augment_annotation)
+        self.min_rate = min_rate
+        self.max_rate = max_rate
+
+        try:
+            librosa.__version__
+        except ImportError:
+            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
+
+    def augment(self, audio: Audio) -> Audio:
+        random_rate = np.random.uniform(self.min_rate, self.max_rate)
+        stretch_audio = librosa.effects.time_stretch(audio.numpy(), rate=random_rate)
+        audio.audio = stretch_audio
+
         return audio
```

### Comparing `mltu-1.2.4/mltu/configs.py` & `mltu-1.2.5/mltu/configs.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-import yaml
-
-
-class BaseModelConfigs:
-    def __init__(self):
-        self.model_path = None
-
-    def serialize(self):
-        class_attributes = {key: value
-                            for (key, value)
-                            in type(self).__dict__.items()
-                            if key not in ['__module__', '__init__', '__doc__', '__annotations__']}
-        instance_attributes = self.__dict__
-
-        # first init with class attributes then apply instance attributes overwriting any existing duplicate attributes
-        all_attributes = class_attributes.copy()
-        all_attributes.update(instance_attributes)
-
-        return all_attributes
-
-    def save(self, name: str = "configs.yaml"):
-        if self.model_path is None:
-            raise Exception("Model path is not specified")
-
-        # create directory if not exist
-        if not os.path.exists(self.model_path):
-            os.makedirs(self.model_path)
-
-        with open(os.path.join(self.model_path, name), "w") as f:
-            yaml.dump(self.serialize(), f)
-
-    @staticmethod
-    def load(configs_path: str):
-        with open(configs_path, "r") as f:
-            configs = yaml.load(f, Loader=yaml.FullLoader)
-
-        config = BaseModelConfigs()
-        for key, value in configs.items():
-            setattr(config, key, value)
-
-        return config
+import os
+import yaml
+
+
+class BaseModelConfigs:
+    def __init__(self):
+        self.model_path = None
+
+    def serialize(self):
+        class_attributes = {key: value
+                            for (key, value)
+                            in type(self).__dict__.items()
+                            if key not in ['__module__', '__init__', '__doc__', '__annotations__']}
+        instance_attributes = self.__dict__
+
+        # first init with class attributes then apply instance attributes overwriting any existing duplicate attributes
+        all_attributes = class_attributes.copy()
+        all_attributes.update(instance_attributes)
+
+        return all_attributes
+
+    def save(self, name: str = "configs.yaml"):
+        if self.model_path is None:
+            raise Exception("Model path is not specified")
+
+        # create directory if not exist
+        if not os.path.exists(self.model_path):
+            os.makedirs(self.model_path)
+
+        with open(os.path.join(self.model_path, name), "w") as f:
+            yaml.dump(self.serialize(), f)
+
+    @staticmethod
+    def load(configs_path: str):
+        with open(configs_path, "r") as f:
+            configs = yaml.load(f, Loader=yaml.FullLoader)
+
+        config = BaseModelConfigs()
+        for key, value in configs.items():
+            setattr(config, key, value)
+
+        return config
```

### Comparing `mltu-1.2.4/mltu/inferenceModel.py` & `mltu-1.2.5/mltu/inferenceModel.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import os
-import time
-import typing
-import numpy as np
-import onnxruntime as ort
-from collections import deque
-
-class FpsWrapper:
-    """ Decorator to calculate the frames per second of a function
-    """
-    def __init__(self, func: typing.Callable):
-        self.func = func
-        self.fps_list = deque([], maxlen=100)
-
-    def __call__(self, *args, **kwargs):
-        start = time.time()
-        results = self.func(self.instance, *args, **kwargs)
-        self.fps_list.append(1 / (time.time() - start))
-        self.instance.fps = np.mean(self.fps_list)
-        return results
-
-    def __get__(self, instance, owner):
-        self.instance = instance
-        return self.__call__.__get__(instance, owner)
-
-
-class OnnxInferenceModel:
-    """ Base class for all inference models that use onnxruntime 
-
-    Attributes:
-        model_path (str, optional): Path to the model folder. Defaults to "".
-        force_cpu (bool, optional): Force the model to run on CPU or GPU. Defaults to GPU.
-        default_model_name (str, optional): Default model name. Defaults to "model.onnx".
-    """
-    def __init__(
-        self, 
-        model_path: str = "",
-        force_cpu: bool = False,
-        default_model_name: str = "model.onnx",
-        *args, **kwargs
-        ):
-        self.model_path = model_path.replace("\\", "/")
-        self.force_cpu = force_cpu
-        self.default_model_name = default_model_name
-
-        # check if model path is a directory with os path
-        if os.path.isdir(self.model_path):
-            self.model_path = os.path.join(self.model_path, self.default_model_name)
-
-        if not os.path.exists(self.model_path):
-            raise Exception(f"Model path ({self.model_path}) does not exist")
-
-        providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if ort.get_device() == "GPU" and not force_cpu else ["CPUExecutionProvider"]
-
-        self.model = ort.InferenceSession(self.model_path, providers=providers)
-
-        self.metadata = {}
-        if self.model.get_modelmeta().custom_metadata_map:
-            # add metadata to self object
-            for key, value in self.model.get_modelmeta().custom_metadata_map.items():
-                try:
-                    new_value = eval(value) # in case the value is a list or dict
-                except:
-                    new_value = value
-                self.metadata[key] = new_value
-                
-        # Update providers priority to only CPUExecutionProvider
-        if self.force_cpu:
-            self.model.set_providers(["CPUExecutionProvider"])
-
-        self.input_shapes = [meta.shape for meta in self.model.get_inputs()]
-        self.input_names = [meta.name for meta in self.model._inputs_meta]
-        self.output_names = [meta.name for meta in self.model._outputs_meta]
-
-    def predict(self, data: np.ndarray, *args, **kwargs):
-        raise NotImplementedError
-
-    @FpsWrapper
-    def __call__(self, data: np.ndarray):
-        results = self.predict(data)
+import os
+import time
+import typing
+import numpy as np
+import onnxruntime as ort
+from collections import deque
+
+class FpsWrapper:
+    """ Decorator to calculate the frames per second of a function
+    """
+    def __init__(self, func: typing.Callable):
+        self.func = func
+        self.fps_list = deque([], maxlen=100)
+
+    def __call__(self, *args, **kwargs):
+        start = time.time()
+        results = self.func(self.instance, *args, **kwargs)
+        self.fps_list.append(1 / (time.time() - start))
+        self.instance.fps = np.mean(self.fps_list)
+        return results
+
+    def __get__(self, instance, owner):
+        self.instance = instance
+        return self.__call__.__get__(instance, owner)
+
+
+class OnnxInferenceModel:
+    """ Base class for all inference models that use onnxruntime 
+
+    Attributes:
+        model_path (str, optional): Path to the model folder. Defaults to "".
+        force_cpu (bool, optional): Force the model to run on CPU or GPU. Defaults to GPU.
+        default_model_name (str, optional): Default model name. Defaults to "model.onnx".
+    """
+    def __init__(
+        self, 
+        model_path: str = "",
+        force_cpu: bool = False,
+        default_model_name: str = "model.onnx",
+        *args, **kwargs
+        ):
+        self.model_path = model_path.replace("\\", "/")
+        self.force_cpu = force_cpu
+        self.default_model_name = default_model_name
+
+        # check if model path is a directory with os path
+        if os.path.isdir(self.model_path):
+            self.model_path = os.path.join(self.model_path, self.default_model_name)
+
+        if not os.path.exists(self.model_path):
+            raise Exception(f"Model path ({self.model_path}) does not exist")
+
+        providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if ort.get_device() == "GPU" and not force_cpu else ["CPUExecutionProvider"]
+
+        self.model = ort.InferenceSession(self.model_path, providers=providers)
+
+        self.metadata = {}
+        if self.model.get_modelmeta().custom_metadata_map:
+            # add metadata to self object
+            for key, value in self.model.get_modelmeta().custom_metadata_map.items():
+                try:
+                    new_value = eval(value) # in case the value is a list or dict
+                except:
+                    new_value = value
+                self.metadata[key] = new_value
+                
+        # Update providers priority to only CPUExecutionProvider
+        if self.force_cpu:
+            self.model.set_providers(["CPUExecutionProvider"])
+
+        self.input_shapes = [meta.shape for meta in self.model.get_inputs()]
+        self.input_names = [meta.name for meta in self.model._inputs_meta]
+        self.output_names = [meta.name for meta in self.model._outputs_meta]
+
+    def predict(self, data: np.ndarray, *args, **kwargs):
+        raise NotImplementedError
+
+    @FpsWrapper
+    def __call__(self, data: np.ndarray):
+        results = self.predict(data)
         return results
```

### Comparing `mltu-1.2.4/mltu/preprocessors.py` & `mltu-1.2.5/mltu/preprocessors.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-import os
-import typing
-import importlib
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib
-import logging
-
-from . import Image
-from mltu.annotations.audio import Audio
-
-""" Implemented Preprocessors:
-- ImageReader - Read image from path and return image and label
-- AudioReader - Read audio from path and return audio and label
-- WavReader - Read wav file with librosa and return spectrogram and label
-- ImageCropper - Crop image to (width, height)
-"""
-
-class ImageReader:
-    """Read image from path and return image and label"""
-    def __init__(self, image_class: Image, log_level: int = logging.INFO, ) -> None:
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(log_level)
-        self._image_class = image_class
-
-    def __call__(self, image_path: typing.Union[str, np.ndarray], label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Read image from path and return image and label
-        
-        Args:
-            image_path (typing.Union[str, np.ndarray]): Path to image or numpy array
-            label (Any): Label of image
-
-        Returns:
-            Image: Image object
-            Any: Label of image
-        """
-        if isinstance(image_path, str):
-            if not os.path.exists(image_path):
-                raise FileNotFoundError(f"Image {image_path} not found.")
-        elif isinstance(image_path, np.ndarray):
-            pass
-        else:
-            raise TypeError(f"Image {image_path} is not a string or numpy array.")
-
-        image = self._image_class(image=image_path)
-
-        if not image.init_successful:
-            image = None
-            self.logger.warning(f"Image {image_path} could not be read, returning None.")
-
-        return image, label
-
-def import_librosa(object) -> None:
-    """Import librosa using importlib"""
-    try:
-        version = object.librosa.__version__
-    except:
-        version = "librosa version not found"
-        try:
-            object.librosa = importlib.import_module('librosa')
-            print("librosa version:", object.librosa.__version__)
-        except:
-            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
-
-class AudioReader:
-    """ Read audio from path and return audio and label
-
-    Attributes:
-        sample_rate (int): Sample rate. Defaults to None.
-        log_level (int): Log level. Defaults to logging.INFO.
-    """
-    def __init__(
-            self, 
-            sample_rate = None,
-            log_level: int = logging.INFO, 
-        ) -> None:
-        self.sample_rate = sample_rate
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(log_level)
-
-        # import librosa using importlib
-        try:
-            self.librosa = importlib.import_module('librosa')
-            print("librosa version:", self.librosa.__version__)
-        except ImportError:
-            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
-
-    def __call__(self, audio_path: str, label: typing.Any) -> typing.Tuple[np.ndarray, typing.Any]:
-        """ Read audio from path and return audio and label
-        
-        Args:
-            audio_path (str): Path to audio
-            label (Any): Label of audio
-
-        Returns:
-            Audio: Audio object
-            Any: Label of audio
-        """
-        if isinstance(audio_path, str):
-            if not os.path.exists(audio_path):
-                raise FileNotFoundError(f"Audio {audio_path} not found.")
-        else:
-            raise TypeError(f"Audio {audio_path} is not a string.")
-
-        audio = Audio(audio_path, sample_rate=self.sample_rate, library=self.librosa)
-
-        if not audio.init_successful:
-            audio = None
-            self.logger.warning(f"Audio {audio_path} could not be read, returning None.")
-
-        return audio, label
-    
-class WavReader:
-    """Read wav file with librosa and return audio and label
-    
-    Attributes:
-        frame_length (int): Length of the frames in samples.
-        frame_step (int): Step size between frames in samples.
-        fft_length (int): Number of FFT components.
-    """
-
-    def __init__(
-            self,
-            frame_length: int = 256,
-            frame_step: int = 160,
-            fft_length: int = 384,
-            *args, **kwargs
-    ) -> None:
-        self.frame_length = frame_length
-        self.frame_step = frame_step
-        self.fft_length = fft_length
-
-        matplotlib.interactive(False)
-        # import librosa using importlib
-        import_librosa(self)
-        
-    @staticmethod
-    def get_spectrogram(wav_path: str, frame_length: int, frame_step: int, fft_length: int) -> np.ndarray:
-        """Compute the spectrogram of a WAV file
-
-        Args:
-            wav_path (str): Path to the WAV file.
-            frame_length (int): Length of the frames in samples.
-            frame_step (int): Step size between frames in samples.
-            fft_length (int): Number of FFT components.
-
-        Returns:
-            np.ndarray: Spectrogram of the WAV file.
-        """
-        import_librosa(WavReader)
-
-        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
-        audio, orig_sr = WavReader.librosa.load(wav_path) 
-
-        # Compute the Short Time Fourier Transform (STFT) of the audio data and store it in the variable 'spectrogram'
-        # The STFT is computed with a hop length of 'frame_step' samples, a window length of 'frame_length' samples, and 'fft_length' FFT components.
-        # The resulting spectrogram is also transposed for convenience
-        spectrogram = WavReader.librosa.stft(audio, hop_length=frame_step, win_length=frame_length, n_fft=fft_length).T
-
-        # Take the absolute value of the spectrogram to obtain the magnitude spectrum
-        spectrogram = np.abs(spectrogram)
-
-        # Take the square root of the magnitude spectrum to obtain the log spectrogram
-        spectrogram = np.power(spectrogram, 0.5)
-
-        # Normalize the spectrogram by subtracting the mean and dividing by the standard deviation.
-        # A small value of 1e-10 is added to the denominator to prevent division by zero.
-        spectrogram = (spectrogram - np.mean(spectrogram)) / (np.std(spectrogram) + 1e-10)
-
-        return spectrogram
-
-    @staticmethod
-    def plot_raw_audio(wav_path: str, title: str = None, sr: int = 16000) -> None:
-        """Plot the raw audio of a WAV file
-
-        Args:
-            wav_path (str): Path to the WAV file.
-            sr (int, optional): Sample rate of the WAV file. Defaults to 16000.
-            title (str, optional): Title
-        """
-        import_librosa(WavReader)
-        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
-        audio, orig_sr = WavReader.librosa.load(wav_path, sr=sr)
-
-        duration = len(audio) / orig_sr
-
-        time = np.linspace(0, duration, num=len(audio))
-
-        plt.figure(figsize=(15, 5))
-        plt.plot(time, audio)
-        plt.title(title) if title else plt.title("Audio Plot")
-        plt.ylabel("signal wave")
-        plt.xlabel("time (s)")
-        plt.tight_layout()
-        plt.show()
-
-    @staticmethod
-    def plot_spectrogram(spectrogram: np.ndarray, title:str = "", transpose: bool = True, invert: bool = True) -> None:
-        """Plot the spectrogram of a WAV file
-
-        Args:
-            spectrogram (np.ndarray): Spectrogram of the WAV file.
-            title (str, optional): Title of the plot. Defaults to None.
-            transpose (bool, optional): Transpose the spectrogram. Defaults to True.
-            invert (bool, optional): Invert the spectrogram. Defaults to True.
-        """
-        if transpose:
-            spectrogram = spectrogram.T
-        
-        if invert:
-            spectrogram = spectrogram[::-1]
-
-        plt.figure(figsize=(15, 5))
-        plt.imshow(spectrogram, aspect="auto", origin="lower")
-        plt.title(f"Spectrogram: {title}")
-        plt.xlabel("Time")
-        plt.ylabel("Frequency")
-        plt.colorbar()
-        plt.tight_layout()
-        plt.show()
-
-    def __call__(self, audio_path: str, label: typing.Any):
-        """
-        Extract the spectrogram and label of a WAV file.
-
-        Args:
-            audio_path (str): Path to the WAV file.
-            label (typing.Any): Label of the WAV file.
-
-        Returns:
-            Tuple[np.ndarray, typing.Any]: Spectrogram of the WAV file and its label.
-        """
-        return self.get_spectrogram(audio_path, self.frame_length, self.frame_step, self.fft_length), label
-
-
-class ImageCropper:
-    """Crop image to (width, height)
-
-    Attributes:
-        width (int): Width of image
-        height (int): Height of image
-        wifth_offset (int): Offset for width
-        height_offset (int): Offset for height
-    """
-    def __init__(
-            self,
-            width: int,
-            height: int,
-            width_offset: int = 0,
-            height_offset: int = 0,
-            log_level: int = logging.INFO
-    ) -> None:
-        super().__init__()
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(log_level)
-
-        self._width = width
-        self._height = height
-        self._width_offset = width_offset
-        self._height_offset = height_offset
-
-    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        image_numpy = image.numpy()
-
-        source_width, source_height = image_numpy.shape[:2][::-1]
-
-        if source_width >= self._width:
-            image_numpy = image_numpy[:, self._width_offset:self._width + self._width_offset]
-        else:
-            raise Exception("unexpected")
-
-        if source_height >= self._height:
-            image_numpy = image_numpy[self._height_offset:self._height + self._height_offset, :]
-        else:
-            raise Exception("unexpected")
-
-        image.update(image_numpy)
-
-        return image, label
+import os
+import typing
+import importlib
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib
+import logging
+
+from . import Image
+from mltu.annotations.audio import Audio
+
+""" Implemented Preprocessors:
+- ImageReader - Read image from path and return image and label
+- AudioReader - Read audio from path and return audio and label
+- WavReader - Read wav file with librosa and return spectrogram and label
+- ImageCropper - Crop image to (width, height)
+"""
+
+class ImageReader:
+    """Read image from path and return image and label"""
+    def __init__(self, image_class: Image, log_level: int = logging.INFO, ) -> None:
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(log_level)
+        self._image_class = image_class
+
+    def __call__(self, image_path: typing.Union[str, np.ndarray], label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Read image from path and return image and label
+        
+        Args:
+            image_path (typing.Union[str, np.ndarray]): Path to image or numpy array
+            label (Any): Label of image
+
+        Returns:
+            Image: Image object
+            Any: Label of image
+        """
+        if isinstance(image_path, str):
+            if not os.path.exists(image_path):
+                raise FileNotFoundError(f"Image {image_path} not found.")
+        elif isinstance(image_path, np.ndarray):
+            pass
+        else:
+            raise TypeError(f"Image {image_path} is not a string or numpy array.")
+
+        image = self._image_class(image=image_path)
+
+        if not image.init_successful:
+            image = None
+            self.logger.warning(f"Image {image_path} could not be read, returning None.")
+
+        return image, label
+
+def import_librosa(object) -> None:
+    """Import librosa using importlib"""
+    try:
+        version = object.librosa.__version__
+    except:
+        version = "librosa version not found"
+        try:
+            object.librosa = importlib.import_module('librosa')
+            print("librosa version:", object.librosa.__version__)
+        except:
+            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
+
+class AudioReader:
+    """ Read audio from path and return audio and label
+
+    Attributes:
+        sample_rate (int): Sample rate. Defaults to None.
+        log_level (int): Log level. Defaults to logging.INFO.
+    """
+    def __init__(
+            self, 
+            sample_rate = None,
+            log_level: int = logging.INFO, 
+        ) -> None:
+        self.sample_rate = sample_rate
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(log_level)
+
+        # import librosa using importlib
+        try:
+            self.librosa = importlib.import_module('librosa')
+            print("librosa version:", self.librosa.__version__)
+        except ImportError:
+            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
+
+    def __call__(self, audio_path: str, label: typing.Any) -> typing.Tuple[np.ndarray, typing.Any]:
+        """ Read audio from path and return audio and label
+        
+        Args:
+            audio_path (str): Path to audio
+            label (Any): Label of audio
+
+        Returns:
+            Audio: Audio object
+            Any: Label of audio
+        """
+        if isinstance(audio_path, str):
+            if not os.path.exists(audio_path):
+                raise FileNotFoundError(f"Audio {audio_path} not found.")
+        else:
+            raise TypeError(f"Audio {audio_path} is not a string.")
+
+        audio = Audio(audio_path, sample_rate=self.sample_rate, library=self.librosa)
+
+        if not audio.init_successful:
+            audio = None
+            self.logger.warning(f"Audio {audio_path} could not be read, returning None.")
+
+        return audio, label
+    
+class WavReader:
+    """Read wav file with librosa and return audio and label
+    
+    Attributes:
+        frame_length (int): Length of the frames in samples.
+        frame_step (int): Step size between frames in samples.
+        fft_length (int): Number of FFT components.
+    """
+
+    def __init__(
+            self,
+            frame_length: int = 256,
+            frame_step: int = 160,
+            fft_length: int = 384,
+            *args, **kwargs
+    ) -> None:
+        self.frame_length = frame_length
+        self.frame_step = frame_step
+        self.fft_length = fft_length
+
+        matplotlib.interactive(False)
+        # import librosa using importlib
+        import_librosa(self)
+        
+    @staticmethod
+    def get_spectrogram(wav_path: str, frame_length: int, frame_step: int, fft_length: int) -> np.ndarray:
+        """Compute the spectrogram of a WAV file
+
+        Args:
+            wav_path (str): Path to the WAV file.
+            frame_length (int): Length of the frames in samples.
+            frame_step (int): Step size between frames in samples.
+            fft_length (int): Number of FFT components.
+
+        Returns:
+            np.ndarray: Spectrogram of the WAV file.
+        """
+        import_librosa(WavReader)
+
+        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
+        audio, orig_sr = WavReader.librosa.load(wav_path) 
+
+        # Compute the Short Time Fourier Transform (STFT) of the audio data and store it in the variable 'spectrogram'
+        # The STFT is computed with a hop length of 'frame_step' samples, a window length of 'frame_length' samples, and 'fft_length' FFT components.
+        # The resulting spectrogram is also transposed for convenience
+        spectrogram = WavReader.librosa.stft(audio, hop_length=frame_step, win_length=frame_length, n_fft=fft_length).T
+
+        # Take the absolute value of the spectrogram to obtain the magnitude spectrum
+        spectrogram = np.abs(spectrogram)
+
+        # Take the square root of the magnitude spectrum to obtain the log spectrogram
+        spectrogram = np.power(spectrogram, 0.5)
+
+        # Normalize the spectrogram by subtracting the mean and dividing by the standard deviation.
+        # A small value of 1e-10 is added to the denominator to prevent division by zero.
+        spectrogram = (spectrogram - np.mean(spectrogram)) / (np.std(spectrogram) + 1e-10)
+
+        return spectrogram
+
+    @staticmethod
+    def plot_raw_audio(wav_path: str, title: str = None, sr: int = 16000) -> None:
+        """Plot the raw audio of a WAV file
+
+        Args:
+            wav_path (str): Path to the WAV file.
+            sr (int, optional): Sample rate of the WAV file. Defaults to 16000.
+            title (str, optional): Title
+        """
+        import_librosa(WavReader)
+        # Load the wav file and store the audio data in the variable 'audio' and the sample rate in 'orig_sr'
+        audio, orig_sr = WavReader.librosa.load(wav_path, sr=sr)
+
+        duration = len(audio) / orig_sr
+
+        time = np.linspace(0, duration, num=len(audio))
+
+        plt.figure(figsize=(15, 5))
+        plt.plot(time, audio)
+        plt.title(title) if title else plt.title("Audio Plot")
+        plt.ylabel("signal wave")
+        plt.xlabel("time (s)")
+        plt.tight_layout()
+        plt.show()
+
+    @staticmethod
+    def plot_spectrogram(spectrogram: np.ndarray, title:str = "", transpose: bool = True, invert: bool = True) -> None:
+        """Plot the spectrogram of a WAV file
+
+        Args:
+            spectrogram (np.ndarray): Spectrogram of the WAV file.
+            title (str, optional): Title of the plot. Defaults to None.
+            transpose (bool, optional): Transpose the spectrogram. Defaults to True.
+            invert (bool, optional): Invert the spectrogram. Defaults to True.
+        """
+        if transpose:
+            spectrogram = spectrogram.T
+        
+        if invert:
+            spectrogram = spectrogram[::-1]
+
+        plt.figure(figsize=(15, 5))
+        plt.imshow(spectrogram, aspect="auto", origin="lower")
+        plt.title(f"Spectrogram: {title}")
+        plt.xlabel("Time")
+        plt.ylabel("Frequency")
+        plt.colorbar()
+        plt.tight_layout()
+        plt.show()
+
+    def __call__(self, audio_path: str, label: typing.Any):
+        """
+        Extract the spectrogram and label of a WAV file.
+
+        Args:
+            audio_path (str): Path to the WAV file.
+            label (typing.Any): Label of the WAV file.
+
+        Returns:
+            Tuple[np.ndarray, typing.Any]: Spectrogram of the WAV file and its label.
+        """
+        return self.get_spectrogram(audio_path, self.frame_length, self.frame_step, self.fft_length), label
+
+
+class ImageCropper:
+    """Crop image to (width, height)
+
+    Attributes:
+        width (int): Width of image
+        height (int): Height of image
+        wifth_offset (int): Offset for width
+        height_offset (int): Offset for height
+    """
+    def __init__(
+            self,
+            width: int,
+            height: int,
+            width_offset: int = 0,
+            height_offset: int = 0,
+            log_level: int = logging.INFO
+    ) -> None:
+        super().__init__()
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(log_level)
+
+        self._width = width
+        self._height = height
+        self._width_offset = width_offset
+        self._height_offset = height_offset
+
+    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        image_numpy = image.numpy()
+
+        source_width, source_height = image_numpy.shape[:2][::-1]
+
+        if source_width >= self._width:
+            image_numpy = image_numpy[:, self._width_offset:self._width + self._width_offset]
+        else:
+            raise Exception("unexpected")
+
+        if source_height >= self._height:
+            image_numpy = image_numpy[self._height_offset:self._height + self._height_offset, :]
+        else:
+            raise Exception("unexpected")
+
+        image.update(image_numpy)
+
+        return image, label
```

### Comparing `mltu-1.2.4/mltu/tensorflow/callbacks.py` & `mltu-1.2.5/mltu/tensorflow/callbacks.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-import os
-import tensorflow as tf
-from keras.callbacks import Callback
-
-import logging
-
-class Model2onnx(Callback):
-    """ Converts the model to onnx format after training is finished. """
-    def __init__(
-        self, 
-        saved_model_path: str, 
-        metadata: dict=None,
-        save_on_epoch_end: bool=False,
-        ) -> None:
-        """ Converts the model to onnx format after training is finished.
-        Args:
-            saved_model_path (str): Path to the saved .h5 model.
-            metadata (dict, optional): Dictionary containing metadata to be added to the onnx model. Defaults to None.
-            save_on_epoch_end (bool, optional): Save the onnx model on every epoch end. Defaults to False.
-        """
-        super().__init__()
-        self.saved_model_path = saved_model_path
-        self.metadata = metadata
-        self.save_on_epoch_end = save_on_epoch_end
-
-        try:
-            import tf2onnx
-        except:
-            raise ImportError("tf2onnx is not installed. Please install it using 'pip install tf2onnx'")
-        
-        try:
-            import onnx
-        except:
-            raise ImportError("onnx is not installed. Please install it using 'pip install onnx'")
-
-    @staticmethod
-    def model2onnx(model: tf.keras.Model, onnx_model_path: str):
-        try:
-            import tf2onnx
-
-            # convert the model to onnx format
-            tf2onnx.convert.from_keras(model, output_path=onnx_model_path)
-
-        except Exception as e:
-            print(e)
-
-    @staticmethod
-    def include_metadata(onnx_model_path: str, metadata: dict=None):
-        try:
-            if metadata and isinstance(metadata, dict):
-
-                import onnx
-                # Load the ONNX model
-                onnx_model = onnx.load(onnx_model_path)
-
-                # Add the metadata dictionary to the model's metadata_props attribute
-                for key, value in metadata.items():
-                    meta = onnx_model.metadata_props.add()
-                    meta.key = key
-                    meta.value = str(value)
-
-                # Save the modified ONNX model
-                onnx.save(onnx_model, onnx_model_path)
-
-        except Exception as e:
-            print(e)  
-
-    def on_epoch_end(self, epoch: int, logs: dict=None):
-        """ Converts the model to onnx format on every epoch end. """
-        if self.save_on_epoch_end:
-            self.on_train_end(logs=logs)
-
-    def on_train_end(self, logs=None):
-        """ Converts the model to onnx format after training is finished. """
-        self.model.load_weights(self.saved_model_path)
-        onnx_model_path = self.saved_model_path.replace(".h5", ".onnx")
-        self.model2onnx(self.model, onnx_model_path)
-        self.include_metadata(onnx_model_path, self.metadata)
-
-
-class TrainLogger(Callback):
-    """Logs training metrics to a file.
-    
-    Args:
-        log_path (str): Path to the directory where the log file will be saved.
-        log_file (str, optional): Name of the log file. Defaults to 'logs.log'.
-        logLevel (int, optional): Logging level. Defaults to logging.INFO.
-    """
-    def __init__(self, log_path: str, log_file: str="logs.log", logLevel=logging.INFO, console_output=False) -> None:
-        super().__init__()
-        self.log_path = log_path
-        self.log_file = log_file
-
-        if not os.path.exists(log_path):
-            os.mkdir(log_path)
-
-        self.logger = logging.getLogger()
-        self.logger.setLevel(logLevel)
-
-        self.formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-
-        self.file_handler = logging.FileHandler(os.path.join(self.log_path, self.log_file))
-        self.file_handler.setLevel(logLevel)
-        self.file_handler.setFormatter(self.formatter)
-
-        if not console_output:
-            self.logger.handlers[:] = []
-
-        self.logger.addHandler(self.file_handler)
-
-    def on_epoch_end(self, epoch: int, logs: dict=None):
-        epoch_message = f"Epoch {epoch}; "
-        logs_message = "; ".join([f"{key}: {value}" for key, value in logs.items()])
-        self.logger.info(epoch_message + logs_message)
-
-
-class WarmupCosineDecay(Callback):
-    """ Cosine decay learning rate scheduler with warmup
-
-    Args:
-        lr_after_warmup (float): Learning rate after warmup
-        final_lr (float): Final learning rate
-        warmup_epochs (int): Number of warmup epochs
-        decay_epochs (int): Number of decay epochs
-        initial_lr (float, optional): Initial learning rate. Defaults to 0.0.
-        verbose (bool, optional): Whether to print learning rate. Defaults to False.
-    """
-    def __init__(
-            self, 
-            lr_after_warmup: float, 
-            final_lr: float, 
-            warmup_epochs: int, 
-            decay_epochs: int, 
-            initial_lr: float=0.0, 
-            verbose=False
-        ) -> None:
-        super(WarmupCosineDecay, self).__init__()
-        self.lr_after_warmup = lr_after_warmup
-        self.final_lr = final_lr
-        self.warmup_epochs = warmup_epochs
-        self.decay_epochs = decay_epochs
-        self.initial_lr = initial_lr
-        self.verbose = verbose
-
-    def on_epoch_begin(self, epoch: int, logs: dict=None):
-        """ Adjust learning rate at the beginning of each epoch """
-
-        if epoch >= self.warmup_epochs + self.decay_epochs:
-            return logs
-
-        if epoch < self.warmup_epochs:
-            lr = self.initial_lr + (self.lr_after_warmup - self.initial_lr) * (epoch + 1) / self.warmup_epochs
-        else:
-            progress = (epoch - self.warmup_epochs) / self.decay_epochs
-            lr = self.final_lr + 0.5 * (self.lr_after_warmup - self.final_lr) * (1 + tf.cos(tf.constant(progress) * 3.14159))
-
-        tf.keras.backend.set_value(self.model.optimizer.lr, lr)
-        
-        if self.verbose:
-            print(f"Epoch {epoch + 1} - Learning Rate: {lr}")
-    
-    def on_epoch_end(self, epoch: int, logs: dict=None):
-        logs = logs or {}
-        
-        # Log the learning rate value
-        logs["lr"] = self.model.optimizer.lr
-        
+import os
+import tensorflow as tf
+from keras.callbacks import Callback
+
+import logging
+
+class Model2onnx(Callback):
+    """ Converts the model to onnx format after training is finished. """
+    def __init__(
+        self, 
+        saved_model_path: str, 
+        metadata: dict=None,
+        save_on_epoch_end: bool=False,
+        ) -> None:
+        """ Converts the model to onnx format after training is finished.
+        Args:
+            saved_model_path (str): Path to the saved .h5 model.
+            metadata (dict, optional): Dictionary containing metadata to be added to the onnx model. Defaults to None.
+            save_on_epoch_end (bool, optional): Save the onnx model on every epoch end. Defaults to False.
+        """
+        super().__init__()
+        self.saved_model_path = saved_model_path
+        self.metadata = metadata
+        self.save_on_epoch_end = save_on_epoch_end
+
+        try:
+            import tf2onnx
+        except:
+            raise ImportError("tf2onnx is not installed. Please install it using 'pip install tf2onnx'")
+        
+        try:
+            import onnx
+        except:
+            raise ImportError("onnx is not installed. Please install it using 'pip install onnx'")
+
+    @staticmethod
+    def model2onnx(model: tf.keras.Model, onnx_model_path: str):
+        try:
+            import tf2onnx
+
+            # convert the model to onnx format
+            tf2onnx.convert.from_keras(model, output_path=onnx_model_path)
+
+        except Exception as e:
+            print(e)
+
+    @staticmethod
+    def include_metadata(onnx_model_path: str, metadata: dict=None):
+        try:
+            if metadata and isinstance(metadata, dict):
+
+                import onnx
+                # Load the ONNX model
+                onnx_model = onnx.load(onnx_model_path)
+
+                # Add the metadata dictionary to the model's metadata_props attribute
+                for key, value in metadata.items():
+                    meta = onnx_model.metadata_props.add()
+                    meta.key = key
+                    meta.value = str(value)
+
+                # Save the modified ONNX model
+                onnx.save(onnx_model, onnx_model_path)
+
+        except Exception as e:
+            print(e)  
+
+    def on_epoch_end(self, epoch: int, logs: dict=None):
+        """ Converts the model to onnx format on every epoch end. """
+        if self.save_on_epoch_end:
+            self.on_train_end(logs=logs)
+
+    def on_train_end(self, logs=None):
+        """ Converts the model to onnx format after training is finished. """
+        self.model.load_weights(self.saved_model_path)
+        onnx_model_path = self.saved_model_path.replace(".h5", ".onnx")
+        self.model2onnx(self.model, onnx_model_path)
+        self.include_metadata(onnx_model_path, self.metadata)
+
+
+class TrainLogger(Callback):
+    """Logs training metrics to a file.
+    
+    Args:
+        log_path (str): Path to the directory where the log file will be saved.
+        log_file (str, optional): Name of the log file. Defaults to 'logs.log'.
+        logLevel (int, optional): Logging level. Defaults to logging.INFO.
+    """
+    def __init__(self, log_path: str, log_file: str="logs.log", logLevel=logging.INFO, console_output=False) -> None:
+        super().__init__()
+        self.log_path = log_path
+        self.log_file = log_file
+
+        if not os.path.exists(log_path):
+            os.mkdir(log_path)
+
+        self.logger = logging.getLogger()
+        self.logger.setLevel(logLevel)
+
+        self.formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+
+        self.file_handler = logging.FileHandler(os.path.join(self.log_path, self.log_file))
+        self.file_handler.setLevel(logLevel)
+        self.file_handler.setFormatter(self.formatter)
+
+        if not console_output:
+            self.logger.handlers[:] = []
+
+        self.logger.addHandler(self.file_handler)
+
+    def on_epoch_end(self, epoch: int, logs: dict=None):
+        epoch_message = f"Epoch {epoch}; "
+        logs_message = "; ".join([f"{key}: {value}" for key, value in logs.items()])
+        self.logger.info(epoch_message + logs_message)
+
+
+class WarmupCosineDecay(Callback):
+    """ Cosine decay learning rate scheduler with warmup
+
+    Args:
+        lr_after_warmup (float): Learning rate after warmup
+        final_lr (float): Final learning rate
+        warmup_epochs (int): Number of warmup epochs
+        decay_epochs (int): Number of decay epochs
+        initial_lr (float, optional): Initial learning rate. Defaults to 0.0.
+        verbose (bool, optional): Whether to print learning rate. Defaults to False.
+    """
+    def __init__(
+            self, 
+            lr_after_warmup: float, 
+            final_lr: float, 
+            warmup_epochs: int, 
+            decay_epochs: int, 
+            initial_lr: float=0.0, 
+            verbose=False
+        ) -> None:
+        super(WarmupCosineDecay, self).__init__()
+        self.lr_after_warmup = lr_after_warmup
+        self.final_lr = final_lr
+        self.warmup_epochs = warmup_epochs
+        self.decay_epochs = decay_epochs
+        self.initial_lr = initial_lr
+        self.verbose = verbose
+
+    def on_epoch_begin(self, epoch: int, logs: dict=None):
+        """ Adjust learning rate at the beginning of each epoch """
+
+        if epoch >= self.warmup_epochs + self.decay_epochs:
+            return logs
+
+        if epoch < self.warmup_epochs:
+            lr = self.initial_lr + (self.lr_after_warmup - self.initial_lr) * (epoch + 1) / self.warmup_epochs
+        else:
+            progress = (epoch - self.warmup_epochs) / self.decay_epochs
+            lr = self.final_lr + 0.5 * (self.lr_after_warmup - self.final_lr) * (1 + tf.cos(tf.constant(progress) * 3.14159))
+
+        tf.keras.backend.set_value(self.model.optimizer.lr, lr)
+        
+        if self.verbose:
+            print(f"Epoch {epoch + 1} - Learning Rate: {lr}")
+    
+    def on_epoch_end(self, epoch: int, logs: dict=None):
+        logs = logs or {}
+        
+        # Log the learning rate value
+        logs["lr"] = self.model.optimizer.lr
+        
         return logs
```

### Comparing `mltu-1.2.4/mltu/tensorflow/layers.py` & `mltu-1.2.5/mltu/tensorflow/layers.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-import tensorflow as tf
-from keras import layers
-from keras import backend as K
-
-class SelfAttention(layers.Layer):
-    """  A self-attention layer for convolutional neural networks.
-    
-    This layer takes as input a tensor of shape (batch_size, height, width, channels)
-    and applies self-attention to the channels dimension.
-
-    Args:
-        num_heads (int): The number of attention heads to use. Defaults to 8.
-        wrapper (tf.keras.layers.Wrapper): A wrapper layer to apply to the convolutional layers.
-
-    Raises:
-        TypeError: If `wrapper` is provided and is not a subclass of `tf.keras.layers.Wrapper`.
-    """
-    def __init__(self, num_heads: int = 8, wrapper: tf.keras.layers.Wrapper = None):
-        super(SelfAttention, self).__init__()
-        self.num_heads = num_heads
-        self.wrapper = wrapper
-
-        if wrapper and not issubclass(wrapper, tf.keras.layers.Wrapper):
-            raise TypeError("wrapper must be a class derived from tf.keras.layers.Wrapper")
-
-    def get_config(self) -> dict:
-        config = super().get_config()
-        config.update({
-            "num_heads": self.num_heads,
-        })
-        return config
-
-    def build(self, input_shape):
-        _, h, w, c = input_shape
-        self.query_conv = self._conv(filters=c // self.num_heads)
-        self.key_conv = self._conv(filters=c // self.num_heads)
-        self.value_conv = self._conv(filters=c)
-        self.gamma = self.add_weight("gamma", shape=[1], initializer=tf.zeros_initializer(), trainable=True)
-
-    def _conv(self, filters: int) -> tf.keras.layers.Layer:
-        """ Helper function to create a convolutional layer with the given number of filters.
-
-        Args:
-            filters (int): The number of filters to use.
-
-        Returns:
-            tf.keras.layers.Layer: The created convolutional layer.
-        """
-        conv = layers.Conv2D(filters=filters, kernel_size=1, strides=1, padding="same")
-        if self.wrapper:
-            conv = self.wrapper(conv)
-
-        return conv
-
-    def call(self, inputs: tf.Tensor) -> tf.Tensor:
-        """ Apply the self-attention mechanism to the input tensor.
-
-        Args:
-            inputs (tf.Tensor): The input tensor of shape (batch_size, height, width, channels).
-
-        Returns:
-            tf.Tensor: The output tensor after the self-attention mechanism is applied.
-        """
-        _, h, w, c = inputs.shape
-        q = self.query_conv(inputs)
-        k = self.key_conv(inputs)
-        v = self.value_conv(inputs)
-
-        q_reshaped = tf.reshape(q, [-1, h * w, c // self.num_heads])
-        k_reshaped = tf.reshape(k, [-1, h * w, c // self.num_heads])
-        v_reshaped = tf.reshape(v, [-1, h * w, c])
-
-        # Compute the attention scores by taking the dot product of the query and key tensors.
-        attention_scores = tf.matmul(q_reshaped, k_reshaped, transpose_b=True)
-
-        # Scale the attention scores by the square root of the number of channels.
-        attention_scores = attention_scores / tf.sqrt(tf.cast(c // self.num_heads, dtype=tf.float32))
-
-        # Apply a softmax function to the attention scores to obtain the attention weights.
-        attention_weights = tf.nn.softmax(attention_scores, axis=-1)
-
-        # Apply the attention weights to the value tensor to obtain the attention output.
-        attention_output = tf.matmul(attention_weights, v_reshaped)
-
-        # Reshape the attended value tensor to the original input tensor shape.
-        attention_output = tf.reshape(attention_output, [-1, h, w, c])
-
-        # Apply the gamma parameter to the attended value tensor and add it to the output tensor.
-        attention_output = self.gamma * attention_output + inputs
-
-        return attention_output
-    
-    
-class SpectralNormalization(tf.keras.layers.Wrapper):
-    """Spectral Normalization Wrapper. !!! This is not working yet !!!"""
-    def __init__(self, layer, power_iterations=1, eps=1e-12, **kwargs):
-        super(SpectralNormalization, self).__init__(layer, **kwargs)
-
-        if power_iterations <= 0:
-            raise ValueError(
-                "`power_iterations` should be greater than zero, got "
-                "`power_iterations={}`".format(power_iterations)
-            )
-        self.power_iterations = power_iterations
-        self.eps = eps
-        if not isinstance(layer, tf.keras.layers.Layer):
-            raise ValueError(
-                "Please initialize `TimeDistributed` layer with a "
-                "`Layer` instance. You passed: {input}".format(input=layer))
-
-    def build(self, input_shape):
-        if not self.layer.built:
-            self.layer.build(input_shape)
-
-        self.w = self.layer.kernel
-        self.w_shape = self.w.shape.as_list()
-
-        # self.v = self.add_weight(shape=(1, self.w_shape[0] * self.w_shape[1] * self.w_shape[2]),
-        #                          initializer=tf.initializers.TruncatedNormal(stddev=0.02),
-        #                          trainable=False,
-        #                          name="sn_v",
-        #                          dtype=tf.float32)
-
-        self.u = self.add_weight(shape=(1, self.w_shape[-1]),
-                                 initializer=tf.initializers.TruncatedNormal(stddev=0.02),
-                                 trainable=False,
-                                 name="sn_u",
-                                 dtype=tf.float32)
-
-        super(SpectralNormalization, self).build()
-
-    def l2normalize(self, v, eps=1e-12):
-        return v / (tf.reduce_sum(v ** 2) ** 0.5 + eps)
-    
-    def power_iteration(self, W, u, rounds=1):
-        _u = u
-
-        for _ in range(rounds):
-            # v_ = tf.matmul(_u, tf.transpose(W))
-            # v_hat = self.l2normalize(v_)
-            _v = self.l2normalize(K.dot(_u, K.transpose(W)), eps=self.eps)
-
-            # u_ = tf.matmul(v_hat, W)
-            # u_hat = self.l2normalize(u_)
-            _u = self.l2normalize(K.dot(_v, W), eps=self.eps)
-
-        return _u, _v
-
-    def call(self, inputs, training=None):
-        if training is None:
-            training = tf.keras.backend.learning_phase()
-
-        if training:
-            self.update_weights()
-            output = self.layer(inputs)
-            self.restore_weights()  # Restore weights because of this formula "W = W - alpha * W_SN`"
-            return output
-
-        return self.layer(inputs)
-    
-    def update_weights(self):
-        w_reshaped = tf.reshape(self.w, [-1, self.w_shape[-1]])
-        
-        # u_hat = self.u
-        # v_hat = self.v  # init v vector
-
-        u_hat, v_hat = self.power_iteration(w_reshaped, self.u, self.power_iterations)
-        # v_ = tf.matmul(u_hat, tf.transpose(w_reshaped))
-        # # v_hat = v_ / (tf.reduce_sum(v_**2)**0.5 + self.eps)
-        # v_hat = self.l2normalize(v_, self.eps)
-
-        # u_ = tf.matmul(v_hat, w_reshaped)
-        # # u_hat = u_ / (tf.reduce_sum(u_**2)**0.5 + self.eps)
-        # u_hat = self.l2normalize(u_, self.eps)
-
-        # sigma = tf.matmul(tf.matmul(v_hat, w_reshaped), tf.transpose(u_hat))
-        sigma=K.dot(K.dot(v_hat, w_reshaped), K.transpose(u_hat))
-        self.u.assign(u_hat)
-        # self.v.assign(v_hat)
-
-        self.layer.kernel.assign(self.w / sigma)
-
-    def restore_weights(self):
+import tensorflow as tf
+from keras import layers
+from keras import backend as K
+
+class SelfAttention(layers.Layer):
+    """  A self-attention layer for convolutional neural networks.
+    
+    This layer takes as input a tensor of shape (batch_size, height, width, channels)
+    and applies self-attention to the channels dimension.
+
+    Args:
+        num_heads (int): The number of attention heads to use. Defaults to 8.
+        wrapper (tf.keras.layers.Wrapper): A wrapper layer to apply to the convolutional layers.
+
+    Raises:
+        TypeError: If `wrapper` is provided and is not a subclass of `tf.keras.layers.Wrapper`.
+    """
+    def __init__(self, num_heads: int = 8, wrapper: tf.keras.layers.Wrapper = None):
+        super(SelfAttention, self).__init__()
+        self.num_heads = num_heads
+        self.wrapper = wrapper
+
+        if wrapper and not issubclass(wrapper, tf.keras.layers.Wrapper):
+            raise TypeError("wrapper must be a class derived from tf.keras.layers.Wrapper")
+
+    def get_config(self) -> dict:
+        config = super().get_config()
+        config.update({
+            "num_heads": self.num_heads,
+        })
+        return config
+
+    def build(self, input_shape):
+        _, h, w, c = input_shape
+        self.query_conv = self._conv(filters=c // self.num_heads)
+        self.key_conv = self._conv(filters=c // self.num_heads)
+        self.value_conv = self._conv(filters=c)
+        self.gamma = self.add_weight("gamma", shape=[1], initializer=tf.zeros_initializer(), trainable=True)
+
+    def _conv(self, filters: int) -> tf.keras.layers.Layer:
+        """ Helper function to create a convolutional layer with the given number of filters.
+
+        Args:
+            filters (int): The number of filters to use.
+
+        Returns:
+            tf.keras.layers.Layer: The created convolutional layer.
+        """
+        conv = layers.Conv2D(filters=filters, kernel_size=1, strides=1, padding="same")
+        if self.wrapper:
+            conv = self.wrapper(conv)
+
+        return conv
+
+    def call(self, inputs: tf.Tensor) -> tf.Tensor:
+        """ Apply the self-attention mechanism to the input tensor.
+
+        Args:
+            inputs (tf.Tensor): The input tensor of shape (batch_size, height, width, channels).
+
+        Returns:
+            tf.Tensor: The output tensor after the self-attention mechanism is applied.
+        """
+        _, h, w, c = inputs.shape
+        q = self.query_conv(inputs)
+        k = self.key_conv(inputs)
+        v = self.value_conv(inputs)
+
+        q_reshaped = tf.reshape(q, [-1, h * w, c // self.num_heads])
+        k_reshaped = tf.reshape(k, [-1, h * w, c // self.num_heads])
+        v_reshaped = tf.reshape(v, [-1, h * w, c])
+
+        # Compute the attention scores by taking the dot product of the query and key tensors.
+        attention_scores = tf.matmul(q_reshaped, k_reshaped, transpose_b=True)
+
+        # Scale the attention scores by the square root of the number of channels.
+        attention_scores = attention_scores / tf.sqrt(tf.cast(c // self.num_heads, dtype=tf.float32))
+
+        # Apply a softmax function to the attention scores to obtain the attention weights.
+        attention_weights = tf.nn.softmax(attention_scores, axis=-1)
+
+        # Apply the attention weights to the value tensor to obtain the attention output.
+        attention_output = tf.matmul(attention_weights, v_reshaped)
+
+        # Reshape the attended value tensor to the original input tensor shape.
+        attention_output = tf.reshape(attention_output, [-1, h, w, c])
+
+        # Apply the gamma parameter to the attended value tensor and add it to the output tensor.
+        attention_output = self.gamma * attention_output + inputs
+
+        return attention_output
+    
+    
+class SpectralNormalization(tf.keras.layers.Wrapper):
+    """Spectral Normalization Wrapper. !!! This is not working yet !!!"""
+    def __init__(self, layer, power_iterations=1, eps=1e-12, **kwargs):
+        super(SpectralNormalization, self).__init__(layer, **kwargs)
+
+        if power_iterations <= 0:
+            raise ValueError(
+                "`power_iterations` should be greater than zero, got "
+                "`power_iterations={}`".format(power_iterations)
+            )
+        self.power_iterations = power_iterations
+        self.eps = eps
+        if not isinstance(layer, tf.keras.layers.Layer):
+            raise ValueError(
+                "Please initialize `TimeDistributed` layer with a "
+                "`Layer` instance. You passed: {input}".format(input=layer))
+
+    def build(self, input_shape):
+        if not self.layer.built:
+            self.layer.build(input_shape)
+
+        self.w = self.layer.kernel
+        self.w_shape = self.w.shape.as_list()
+
+        # self.v = self.add_weight(shape=(1, self.w_shape[0] * self.w_shape[1] * self.w_shape[2]),
+        #                          initializer=tf.initializers.TruncatedNormal(stddev=0.02),
+        #                          trainable=False,
+        #                          name="sn_v",
+        #                          dtype=tf.float32)
+
+        self.u = self.add_weight(shape=(1, self.w_shape[-1]),
+                                 initializer=tf.initializers.TruncatedNormal(stddev=0.02),
+                                 trainable=False,
+                                 name="sn_u",
+                                 dtype=tf.float32)
+
+        super(SpectralNormalization, self).build()
+
+    def l2normalize(self, v, eps=1e-12):
+        return v / (tf.reduce_sum(v ** 2) ** 0.5 + eps)
+    
+    def power_iteration(self, W, u, rounds=1):
+        _u = u
+
+        for _ in range(rounds):
+            # v_ = tf.matmul(_u, tf.transpose(W))
+            # v_hat = self.l2normalize(v_)
+            _v = self.l2normalize(K.dot(_u, K.transpose(W)), eps=self.eps)
+
+            # u_ = tf.matmul(v_hat, W)
+            # u_hat = self.l2normalize(u_)
+            _u = self.l2normalize(K.dot(_v, W), eps=self.eps)
+
+        return _u, _v
+
+    def call(self, inputs, training=None):
+        if training is None:
+            training = tf.keras.backend.learning_phase()
+
+        if training:
+            self.update_weights()
+            output = self.layer(inputs)
+            self.restore_weights()  # Restore weights because of this formula "W = W - alpha * W_SN`"
+            return output
+
+        return self.layer(inputs)
+    
+    def update_weights(self):
+        w_reshaped = tf.reshape(self.w, [-1, self.w_shape[-1]])
+        
+        # u_hat = self.u
+        # v_hat = self.v  # init v vector
+
+        u_hat, v_hat = self.power_iteration(w_reshaped, self.u, self.power_iterations)
+        # v_ = tf.matmul(u_hat, tf.transpose(w_reshaped))
+        # # v_hat = v_ / (tf.reduce_sum(v_**2)**0.5 + self.eps)
+        # v_hat = self.l2normalize(v_, self.eps)
+
+        # u_ = tf.matmul(v_hat, w_reshaped)
+        # # u_hat = u_ / (tf.reduce_sum(u_**2)**0.5 + self.eps)
+        # u_hat = self.l2normalize(u_, self.eps)
+
+        # sigma = tf.matmul(tf.matmul(v_hat, w_reshaped), tf.transpose(u_hat))
+        sigma=K.dot(K.dot(v_hat, w_reshaped), K.transpose(u_hat))
+        self.u.assign(u_hat)
+        # self.v.assign(v_hat)
+
+        self.layer.kernel.assign(self.w / sigma)
+
+    def restore_weights(self):
         self.layer.kernel.assign(self.w)
```

### Comparing `mltu-1.2.4/mltu/tensorflow/metrics.py` & `mltu-1.2.5/mltu/tensorflow/metrics.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-import tensorflow as tf
-from keras.metrics import Metric
-
-class CWERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Character Error Rate (CER).
-    
-    Args:
-        padding_token: An integer representing the padding token in the input data.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, padding_token, name="CWER", **kwargs):
-        # Initialize the base Metric class
-        super(CWERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
-        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        # Store the padding token as an attribute
-        self.padding_token = padding_token
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """Updates the state variables of the metric.
-
-        Args:
-            y_true: A tensor of true labels with shape (batch_size, sequence_length).
-            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
-            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
-        """
-        # Get the input shape and length
-        input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
-
-        # Decode the predicted labels using greedy decoding
-        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
-
-        # Convert the dense decode tensor to a sparse tensor
-        predicted_labels_sparse = tf.keras.backend.ctc_label_dense_to_sparse(decode_predicted[0], input_length)
-        
-        # Convert the dense true labels tensor to a sparse tensor and cast to int64
-        true_labels_sparse = tf.cast(tf.keras.backend.ctc_label_dense_to_sparse(y_true, input_length), "int64")
-
-        # Retain only the non-padding elements in the predicted labels tensor
-        predicted_labels_sparse = tf.sparse.retain(predicted_labels_sparse, tf.not_equal(predicted_labels_sparse.values, -1))
-        
-        # Retain only the non-padding elements in the true labels tensor
-        true_labels_sparse = tf.sparse.retain(true_labels_sparse, tf.not_equal(true_labels_sparse.values, self.padding_token))
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = tf.edit_distance(predicted_labels_sparse, true_labels_sparse, normalize=True)
-
-        # Add the sum of the distance tensor to the cer_accumulator variable
-        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
-        
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(input_shape[0])
-
-        # Calculate the number of wrong words in batch and add to wer_accumulator variable
-        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(tf.not_equal(distance, 0), tf.float32)))
-
-    def result(self):
-        """Computes and returns the metric result.
-
-        Returns:
-            A dictionary containing the CER and WER.
-        """
-        return {
-                "CER": tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32)),
-                "WER": tf.math.divide_no_nan(self.wer_accumulator, tf.cast(self.batch_counter, tf.float32))
-        }
-
-class CERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Character Error Rate (CER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, vocabulary, name="CER", **kwargs):
-        # Initialize the base Metric class
-        super(CERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        # Store the vocabulary as an attribute
-        self.vocabulary = tf.constant(list(vocabulary))
-
-    @staticmethod
-    def get_cer(pred_decoded, y_true, vocab, padding=-1):
-        """ Calculates the character error rate (CER) between the predicted labels and true labels for a batch of input data.
-
-        Args:
-            pred_decoded (tf.Tensor): The predicted labels, with dtype=tf.int32, usually output from tf.keras.backend.ctc_decode
-            y_true (tf.Tensor): The true labels, with dtype=tf.int32
-            vocab (tf.Tensor): The vocabulary tensor, with dtype=tf.string
-            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
-
-        Returns:
-            tf.Tensor: The CER between the predicted labels and true labels
-        """
-        # Keep only valid indices in the predicted labels tensor, replacing invalid indices with padding token
-        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
-        valid_pred_indices = tf.less(pred_decoded, vocab_length)
-        valid_pred = tf.where(valid_pred_indices, pred_decoded, padding)
-
-        # Keep only valid indices in the true labels tensor, replacing invalid indices with padding token
-        y_true = tf.cast(y_true, tf.int64)
-        valid_true_indices = tf.less(y_true, vocab_length)
-        valid_true = tf.where(valid_true_indices, y_true, padding)
-
-        # Convert the valid predicted labels tensor to a sparse tensor
-        sparse_pred = tf.RaggedTensor.from_tensor(valid_pred, padding=padding).to_sparse()
-
-        # Convert the valid true labels tensor to a sparse tensor
-        sparse_true = tf.RaggedTensor.from_tensor(valid_true, padding=padding).to_sparse()
-
-        # Calculate the normalized edit distance between the sparse predicted labels tensor and sparse true labels tensor
-        distance = tf.edit_distance(sparse_pred, sparse_true, normalize=True)
-
-        return distance
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """Updates the state variables of the metric.
-
-        Args:
-            y_true: A tensor of true labels with shape (batch_size, sequence_length).
-            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
-            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
-        """
-        # Get the input shape and length
-        input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
-
-        # Decode the predicted labels using greedy decoding
-        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = self.get_cer(decode_predicted[0], y_true, self.vocabulary)
-
-        # Add the sum of the distance tensor to the cer_accumulator variable
-        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
-        
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(input_shape[0])
-
-    def result(self):
-        """ Computes and returns the metric result.
-
-        Returns:
-            A TensorFlow float representing the CER (character error rate).
-        """
-        return tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32))
-
-
-class WERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Word Error Rate (WER).
-    
-    Attributes:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, vocabulary: str, name="WER", **kwargs):
-        # Initialize the base Metric class
-        super(WERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        # Store the vocabulary as an attribute
-        self.vocabulary = tf.constant(list(vocabulary))
-
-    @staticmethod
-    def preprocess_dense(dense_input: tf.Tensor, vocab: tf.Tensor, padding=-1, separator="") -> tf.SparseTensor:
-        """ Preprocess the dense input tensor to a sparse tensor with given vocabulary
-        
-        Args:
-            dense_input (tf.Tensor): The dense input tensor, dtype=tf.int32
-            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
-            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
-
-        Returns:
-            tf.SparseTensor: The sparse tensor with given vocabulary
-        """
-        # Keep only the valid indices of the dense input tensor
-        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
-        dense_input = tf.cast(dense_input, tf.int64)
-        valid_indices = tf.less(dense_input, vocab_length)
-        valid_input = tf.where(valid_indices, dense_input, padding)
-
-        # Convert the valid input tensor to a ragged tensor with padding
-        input_ragged = tf.RaggedTensor.from_tensor(valid_input, padding=padding)
-
-        # Use the vocabulary tensor to get the strings corresponding to the indices in the ragged tensor
-        input_binary_chars = tf.gather(vocab, input_ragged)
-
-        # Join the binary character tensor along the sequence axis to get the input strings
-        input_strings = tf.strings.reduce_join(input_binary_chars, axis=1, separator=separator)
-
-        # Convert the input strings tensor to a sparse tensor
-        input_sparse_string = tf.strings.split(input_strings, sep=" ").to_sparse()
-
-        return input_sparse_string
-
-    @staticmethod
-    def get_wer(pred_decoded, y_true, vocab, padding=-1, separator=""):
-        """ Calculate the normalized WER distance between the predicted labels and true labels tensors
-
-        Args:
-            pred_decoded (tf.Tensor): The predicted labels tensor, dtype=tf.int32. Usually output from tf.keras.backend.ctc_decode
-            y_true (tf.Tensor): The true labels tensor, dtype=tf.int32
-            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
-
-        Returns:
-            tf.Tensor: The normalized WER distance between the predicted labels and true labels tensors
-        """
-        pred_sparse = WERMetric.preprocess_dense(pred_decoded, vocab, padding=padding, separator=separator)
-        true_sparse = WERMetric.preprocess_dense(y_true, vocab, padding=padding, separator=separator)
-
-        distance = tf.edit_distance(pred_sparse, true_sparse, normalize=True)
-
-        # test with numerical labels not string
-        # true_sparse = tf.RaggedTensor.from_tensor(y_true, padding=-1).to_sparse()
-
-        # replace 23 with -1
-        # pred_decoded2 = tf.where(tf.equal(pred_decoded, 23), -1, pred_decoded)
-        # pred_decoded2_sparse = tf.RaggedTensor.from_tensor(pred_decoded2, padding=-1).to_sparse()
-
-        # distance = tf.edit_distance(pred_decoded2_sparse, true_sparse, normalize=True)
-
-        return distance
-
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """
-        """
-        # Get the input shape and length
-        input_shape = tf.keras.backend.shape(y_pred)
-        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
-
-        # Decode the predicted labels using greedy decoding
-        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = self.get_wer(decode_predicted[0], y_true, self.vocabulary)
-
-        # Calculate the number of wrong words in batch and add to wer_accumulator variable
-        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(distance, tf.float32)))
-
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(input_shape[0])
-
-    def result(self):
-        """Computes and returns the metric result.
-
-        Returns:
-            A TensorFlow float representing the WER (Word Error Rate).
-        """
+import tensorflow as tf
+from keras.metrics import Metric
+
+class CWERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Character Error Rate (CER).
+    
+    Args:
+        padding_token: An integer representing the padding token in the input data.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, padding_token, name="CWER", **kwargs):
+        # Initialize the base Metric class
+        super(CWERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
+        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        # Store the padding token as an attribute
+        self.padding_token = padding_token
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """Updates the state variables of the metric.
+
+        Args:
+            y_true: A tensor of true labels with shape (batch_size, sequence_length).
+            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
+            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
+        """
+        # Get the input shape and length
+        input_shape = tf.keras.backend.shape(y_pred)
+        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
+
+        # Decode the predicted labels using greedy decoding
+        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
+
+        # Convert the dense decode tensor to a sparse tensor
+        predicted_labels_sparse = tf.keras.backend.ctc_label_dense_to_sparse(decode_predicted[0], input_length)
+        
+        # Convert the dense true labels tensor to a sparse tensor and cast to int64
+        true_labels_sparse = tf.cast(tf.keras.backend.ctc_label_dense_to_sparse(y_true, input_length), "int64")
+
+        # Retain only the non-padding elements in the predicted labels tensor
+        predicted_labels_sparse = tf.sparse.retain(predicted_labels_sparse, tf.not_equal(predicted_labels_sparse.values, -1))
+        
+        # Retain only the non-padding elements in the true labels tensor
+        true_labels_sparse = tf.sparse.retain(true_labels_sparse, tf.not_equal(true_labels_sparse.values, self.padding_token))
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = tf.edit_distance(predicted_labels_sparse, true_labels_sparse, normalize=True)
+
+        # Add the sum of the distance tensor to the cer_accumulator variable
+        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
+        
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(input_shape[0])
+
+        # Calculate the number of wrong words in batch and add to wer_accumulator variable
+        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(tf.not_equal(distance, 0), tf.float32)))
+
+    def result(self):
+        """Computes and returns the metric result.
+
+        Returns:
+            A dictionary containing the CER and WER.
+        """
+        return {
+                "CER": tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32)),
+                "WER": tf.math.divide_no_nan(self.wer_accumulator, tf.cast(self.batch_counter, tf.float32))
+        }
+
+class CERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Character Error Rate (CER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, vocabulary, name="CER", **kwargs):
+        # Initialize the base Metric class
+        super(CERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        # Store the vocabulary as an attribute
+        self.vocabulary = tf.constant(list(vocabulary))
+
+    @staticmethod
+    def get_cer(pred_decoded, y_true, vocab, padding=-1):
+        """ Calculates the character error rate (CER) between the predicted labels and true labels for a batch of input data.
+
+        Args:
+            pred_decoded (tf.Tensor): The predicted labels, with dtype=tf.int32, usually output from tf.keras.backend.ctc_decode
+            y_true (tf.Tensor): The true labels, with dtype=tf.int32
+            vocab (tf.Tensor): The vocabulary tensor, with dtype=tf.string
+            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
+
+        Returns:
+            tf.Tensor: The CER between the predicted labels and true labels
+        """
+        # Keep only valid indices in the predicted labels tensor, replacing invalid indices with padding token
+        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
+        valid_pred_indices = tf.less(pred_decoded, vocab_length)
+        valid_pred = tf.where(valid_pred_indices, pred_decoded, padding)
+
+        # Keep only valid indices in the true labels tensor, replacing invalid indices with padding token
+        y_true = tf.cast(y_true, tf.int64)
+        valid_true_indices = tf.less(y_true, vocab_length)
+        valid_true = tf.where(valid_true_indices, y_true, padding)
+
+        # Convert the valid predicted labels tensor to a sparse tensor
+        sparse_pred = tf.RaggedTensor.from_tensor(valid_pred, padding=padding).to_sparse()
+
+        # Convert the valid true labels tensor to a sparse tensor
+        sparse_true = tf.RaggedTensor.from_tensor(valid_true, padding=padding).to_sparse()
+
+        # Calculate the normalized edit distance between the sparse predicted labels tensor and sparse true labels tensor
+        distance = tf.edit_distance(sparse_pred, sparse_true, normalize=True)
+
+        return distance
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """Updates the state variables of the metric.
+
+        Args:
+            y_true: A tensor of true labels with shape (batch_size, sequence_length).
+            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
+            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
+        """
+        # Get the input shape and length
+        input_shape = tf.keras.backend.shape(y_pred)
+        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
+
+        # Decode the predicted labels using greedy decoding
+        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = self.get_cer(decode_predicted[0], y_true, self.vocabulary)
+
+        # Add the sum of the distance tensor to the cer_accumulator variable
+        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
+        
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(input_shape[0])
+
+    def result(self):
+        """ Computes and returns the metric result.
+
+        Returns:
+            A TensorFlow float representing the CER (character error rate).
+        """
+        return tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32))
+
+
+class WERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Word Error Rate (WER).
+    
+    Attributes:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, vocabulary: str, name="WER", **kwargs):
+        # Initialize the base Metric class
+        super(WERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.wer_accumulator = tf.Variable(0.0, name="wer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        # Store the vocabulary as an attribute
+        self.vocabulary = tf.constant(list(vocabulary))
+
+    @staticmethod
+    def preprocess_dense(dense_input: tf.Tensor, vocab: tf.Tensor, padding=-1, separator="") -> tf.SparseTensor:
+        """ Preprocess the dense input tensor to a sparse tensor with given vocabulary
+        
+        Args:
+            dense_input (tf.Tensor): The dense input tensor, dtype=tf.int32
+            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
+            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
+
+        Returns:
+            tf.SparseTensor: The sparse tensor with given vocabulary
+        """
+        # Keep only the valid indices of the dense input tensor
+        vocab_length = tf.cast(tf.shape(vocab)[0], tf.int64)
+        dense_input = tf.cast(dense_input, tf.int64)
+        valid_indices = tf.less(dense_input, vocab_length)
+        valid_input = tf.where(valid_indices, dense_input, padding)
+
+        # Convert the valid input tensor to a ragged tensor with padding
+        input_ragged = tf.RaggedTensor.from_tensor(valid_input, padding=padding)
+
+        # Use the vocabulary tensor to get the strings corresponding to the indices in the ragged tensor
+        input_binary_chars = tf.gather(vocab, input_ragged)
+
+        # Join the binary character tensor along the sequence axis to get the input strings
+        input_strings = tf.strings.reduce_join(input_binary_chars, axis=1, separator=separator)
+
+        # Convert the input strings tensor to a sparse tensor
+        input_sparse_string = tf.strings.split(input_strings, sep=" ").to_sparse()
+
+        return input_sparse_string
+
+    @staticmethod
+    def get_wer(pred_decoded, y_true, vocab, padding=-1, separator=""):
+        """ Calculate the normalized WER distance between the predicted labels and true labels tensors
+
+        Args:
+            pred_decoded (tf.Tensor): The predicted labels tensor, dtype=tf.int32. Usually output from tf.keras.backend.ctc_decode
+            y_true (tf.Tensor): The true labels tensor, dtype=tf.int32
+            vocab (tf.Tensor): The vocabulary tensor, dtype=tf.string
+
+        Returns:
+            tf.Tensor: The normalized WER distance between the predicted labels and true labels tensors
+        """
+        pred_sparse = WERMetric.preprocess_dense(pred_decoded, vocab, padding=padding, separator=separator)
+        true_sparse = WERMetric.preprocess_dense(y_true, vocab, padding=padding, separator=separator)
+
+        distance = tf.edit_distance(pred_sparse, true_sparse, normalize=True)
+
+        # test with numerical labels not string
+        # true_sparse = tf.RaggedTensor.from_tensor(y_true, padding=-1).to_sparse()
+
+        # replace 23 with -1
+        # pred_decoded2 = tf.where(tf.equal(pred_decoded, 23), -1, pred_decoded)
+        # pred_decoded2_sparse = tf.RaggedTensor.from_tensor(pred_decoded2, padding=-1).to_sparse()
+
+        # distance = tf.edit_distance(pred_decoded2_sparse, true_sparse, normalize=True)
+
+        return distance
+
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """
+        """
+        # Get the input shape and length
+        input_shape = tf.keras.backend.shape(y_pred)
+        input_length = tf.ones(shape=input_shape[0], dtype="int32") * tf.cast(input_shape[1], "int32")
+
+        # Decode the predicted labels using greedy decoding
+        decode_predicted, log = tf.keras.backend.ctc_decode(y_pred, input_length, greedy=True)
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = self.get_wer(decode_predicted[0], y_true, self.vocabulary)
+
+        # Calculate the number of wrong words in batch and add to wer_accumulator variable
+        self.wer_accumulator.assign_add(tf.reduce_sum(tf.cast(distance, tf.float32)))
+
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(input_shape[0])
+
+    def result(self):
+        """Computes and returns the metric result.
+
+        Returns:
+            A TensorFlow float representing the WER (Word Error Rate).
+        """
         return tf.math.divide_no_nan(self.wer_accumulator, tf.cast(self.batch_counter, tf.float32))
```

### Comparing `mltu-1.2.4/mltu/tensorflow/model_utils.py` & `mltu-1.2.5/mltu/tensorflow/model_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import typing
-import tensorflow as tf
-from tensorflow import keras
-from keras import layers
-from keras.models import Model
-
-class CustomModel(Model):
-    """ Custom TensorFlow model for debugging training process purposes
-    """
-    def train_step(self, train_data):
-        # Unpack the data. Its structure depends on your model and
-        # on what you pass to `fit()`.
-        inputs, targets = train_data
-        with tf.GradientTape() as tape:
-            results = self(inputs, training=True)
-            loss = self.compiled_loss(targets, results, regularization_losses=self.losses)
-            gradients = tape.gradient(loss, self.trainable_weights)
-
-        # Applying the gradients on the model using the specified optimizer
-        self.optimizer.apply_gradients(zip(gradients, self.trainable_weights))
-
-        # Update the metrics.
-        # Metrics are configured in `compile()`.
-        self.compiled_metrics.update_state(targets, results)
-
-        return {m.name: m.result() for m in self.metrics}
-
-    def test_step(self, test_data):
-        inputs, targets = test_data
-        # Get prediction from model
-        results = self(inputs, training=False)
-
-        # Update the loss
-        self.compiled_loss(targets, results, regularization_losses=self.losses)
-
-        # Update the metrics
-        self.compiled_metrics.update_state(targets, results)
-
-        # Return a dict mapping metric names to current value.
-        # Note that it will include the loss (tracked in self.metrics).
-        return {m.name: m.result() for m in self.metrics}
-
-
-def activation_layer(layer, activation: str="relu", alpha: float=0.1) -> tf.Tensor:
-    """ Activation layer wrapper for LeakyReLU and ReLU activation functions
-    Args:
-        layer: tf.Tensor
-        activation: str, activation function name (default: 'relu')
-        alpha: float (LeakyReLU activation function parameter)
-    Returns:
-        tf.Tensor
-    """
-    if activation == "relu":
-        layer = layers.ReLU()(layer)
-    elif activation == "leaky_relu":
-        layer = layers.LeakyReLU(alpha=alpha)(layer)
-
-    return layer
-
-
-def residual_block(
-        x: tf.Tensor,
-        filter_num: int,
-        strides: typing.Union[int, list] = 2,
-        kernel_size: typing.Union[int, list] = 3,
-        skip_conv: bool = True,
-        padding: str = "same",
-        kernel_initializer: str = "he_uniform",
-        activation: str = "relu",
-        dropout: float = 0.2):
-    # Create skip connection tensor
-    x_skip = x
-
-    # Perform 1-st convolution
-    x = layers.Conv2D(filter_num, kernel_size, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x)
-    x = layers.BatchNormalization()(x)
-    x = activation_layer(x, activation=activation)
-
-    # Perform 2-nd convoluti
-    x = layers.Conv2D(filter_num, kernel_size, padding = padding, kernel_initializer=kernel_initializer)(x)
-    x = layers.BatchNormalization()(x)
-
-    # Perform 3-rd convolution if skip_conv is True, matchin the number of filters and the shape of the skip connection tensor
-    if skip_conv:
-        x_skip = layers.Conv2D(filter_num, 1, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x_skip)
-
-    # Add x and skip connection and apply activation function
-    x = layers.Add()([x, x_skip])     
-    x = activation_layer(x, activation=activation)
-
-    # Apply dropout
-    if dropout:
-        x = layers.Dropout(dropout)(x)
-
+import typing
+import tensorflow as tf
+from tensorflow import keras
+from keras import layers
+from keras.models import Model
+
+class CustomModel(Model):
+    """ Custom TensorFlow model for debugging training process purposes
+    """
+    def train_step(self, train_data):
+        # Unpack the data. Its structure depends on your model and
+        # on what you pass to `fit()`.
+        inputs, targets = train_data
+        with tf.GradientTape() as tape:
+            results = self(inputs, training=True)
+            loss = self.compiled_loss(targets, results, regularization_losses=self.losses)
+            gradients = tape.gradient(loss, self.trainable_weights)
+
+        # Applying the gradients on the model using the specified optimizer
+        self.optimizer.apply_gradients(zip(gradients, self.trainable_weights))
+
+        # Update the metrics.
+        # Metrics are configured in `compile()`.
+        self.compiled_metrics.update_state(targets, results)
+
+        return {m.name: m.result() for m in self.metrics}
+
+    def test_step(self, test_data):
+        inputs, targets = test_data
+        # Get prediction from model
+        results = self(inputs, training=False)
+
+        # Update the loss
+        self.compiled_loss(targets, results, regularization_losses=self.losses)
+
+        # Update the metrics
+        self.compiled_metrics.update_state(targets, results)
+
+        # Return a dict mapping metric names to current value.
+        # Note that it will include the loss (tracked in self.metrics).
+        return {m.name: m.result() for m in self.metrics}
+
+
+def activation_layer(layer, activation: str="relu", alpha: float=0.1) -> tf.Tensor:
+    """ Activation layer wrapper for LeakyReLU and ReLU activation functions
+    Args:
+        layer: tf.Tensor
+        activation: str, activation function name (default: 'relu')
+        alpha: float (LeakyReLU activation function parameter)
+    Returns:
+        tf.Tensor
+    """
+    if activation == "relu":
+        layer = layers.ReLU()(layer)
+    elif activation == "leaky_relu":
+        layer = layers.LeakyReLU(alpha=alpha)(layer)
+
+    return layer
+
+
+def residual_block(
+        x: tf.Tensor,
+        filter_num: int,
+        strides: typing.Union[int, list] = 2,
+        kernel_size: typing.Union[int, list] = 3,
+        skip_conv: bool = True,
+        padding: str = "same",
+        kernel_initializer: str = "he_uniform",
+        activation: str = "relu",
+        dropout: float = 0.2):
+    # Create skip connection tensor
+    x_skip = x
+
+    # Perform 1-st convolution
+    x = layers.Conv2D(filter_num, kernel_size, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x)
+    x = layers.BatchNormalization()(x)
+    x = activation_layer(x, activation=activation)
+
+    # Perform 2-nd convoluti
+    x = layers.Conv2D(filter_num, kernel_size, padding = padding, kernel_initializer=kernel_initializer)(x)
+    x = layers.BatchNormalization()(x)
+
+    # Perform 3-rd convolution if skip_conv is True, matchin the number of filters and the shape of the skip connection tensor
+    if skip_conv:
+        x_skip = layers.Conv2D(filter_num, 1, padding = padding, strides = strides, kernel_initializer=kernel_initializer)(x_skip)
+
+    # Add x and skip connection and apply activation function
+    x = layers.Add()([x, x_skip])     
+    x = activation_layer(x, activation=activation)
+
+    # Apply dropout
+    if dropout:
+        x = layers.Dropout(dropout)(x)
+
     return x
```

### Comparing `mltu-1.2.4/mltu/tensorflow/transformer/attention.py` & `mltu-1.2.5/mltu/tensorflow/transformer/attention.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import tensorflow as tf
-
-class BaseAttention(tf.keras.layers.Layer):
-    """
-    Base class for all attention layers. It contains the common functionality of all attention layers.
-    This layer contains a MultiHeadAttention layer, a LayerNormalization layer and an Add layer.
-    It is used as a base class for the GlobalSelfAttention, CausalSelfAttention and CrossAttention layers.
-    And it is not intended to be used directly.
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
-        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
-        add (tf.keras.layers.Add): The Add layer.
-    """
-    def __init__(self, **kwargs: dict):
-        """ Constructor of the BaseAttention layer.
-        
-        Args:
-            **kwargs: Additional keyword arguments that are passed to the MultiHeadAttention layer, e. g. 
-                        num_heads (number of heads), key_dim (dimensionality of the key space), etc.
-        """
-        super().__init__()
-        self.mha = tf.keras.layers.MultiHeadAttention(**kwargs)
-        self.layernorm = tf.keras.layers.LayerNormalization()
-        self.add = tf.keras.layers.Add()
-
-
-class CrossAttention(BaseAttention):
-    """
-    A class that implements the cross-attention layer by inheriting from the BaseAttention class.
-    This layer is used to process two different sequences and attends to the context sequence while processing the query sequence.
-
-    Methods:
-        call: Performs the forward pass of the layer.    
-
-    Attributes:
-        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
-        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
-        add (tf.keras.layers.Add): The Add layer.
-    """
-    def call(self, x: tf.Tensor, context: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the cross-attention operation.
-
-        Args:
-            x (tf.Tensor): The query (expected Transformer results) sequence of shape (batch_size, seq_length, d_model).
-            context (tf.Tensor): The context (inputs to the Transformer) sequence of shape (batch_size, seq_length, d_model).
-
-        Returns:
-            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
-        """
-        attn_output, attn_scores = self.mha(query=x, key=context, value=context, return_attention_scores=True)
-
-        # Cache the attention scores for plotting later.
-        self.last_attn_scores = attn_scores
-
-        x = self.add([x, attn_output])
-        x = self.layernorm(x)
-
-        return x
-
-
-class GlobalSelfAttention(BaseAttention):
-    """
-    A class that implements the global self-attention layer by inheriting from the BaseAttention class.
-    This layer is used to process a single sequence and attends to all the tokens in the sequence.
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
-        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
-        add (tf.keras.layers.Add): The Add layer.
-    """
-    def call(self, x: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the global self-attention operation.
-
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
-
-        Returns:
-            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
-        """
-        attn_output = self.mha(query=x, value=x, key=x)
-        x = self.add([x, attn_output])
-        x = self.layernorm(x)
-        return x
-
-
-class CausalSelfAttention(BaseAttention):
-    """
-    Call self attention on the input sequence, ensuring that each position in the 
-    output depends only on previous positions (i.e. a causal model).
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
-        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
-        add (tf.keras.layers.Add): The Add layer.
-    """
-    def call(self, x: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the causal self-attention operation.
-        
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
-
-        Returns:
-            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
-        """
-        attn_output = self.mha(query=x, value=x, key=x, use_causal_mask = True)
-        x = self.add([x, attn_output])
-        x = self.layernorm(x)
+import tensorflow as tf
+
+class BaseAttention(tf.keras.layers.Layer):
+    """
+    Base class for all attention layers. It contains the common functionality of all attention layers.
+    This layer contains a MultiHeadAttention layer, a LayerNormalization layer and an Add layer.
+    It is used as a base class for the GlobalSelfAttention, CausalSelfAttention and CrossAttention layers.
+    And it is not intended to be used directly.
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
+        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
+        add (tf.keras.layers.Add): The Add layer.
+    """
+    def __init__(self, **kwargs: dict):
+        """ Constructor of the BaseAttention layer.
+        
+        Args:
+            **kwargs: Additional keyword arguments that are passed to the MultiHeadAttention layer, e. g. 
+                        num_heads (number of heads), key_dim (dimensionality of the key space), etc.
+        """
+        super().__init__()
+        self.mha = tf.keras.layers.MultiHeadAttention(**kwargs)
+        self.layernorm = tf.keras.layers.LayerNormalization()
+        self.add = tf.keras.layers.Add()
+
+
+class CrossAttention(BaseAttention):
+    """
+    A class that implements the cross-attention layer by inheriting from the BaseAttention class.
+    This layer is used to process two different sequences and attends to the context sequence while processing the query sequence.
+
+    Methods:
+        call: Performs the forward pass of the layer.    
+
+    Attributes:
+        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
+        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
+        add (tf.keras.layers.Add): The Add layer.
+    """
+    def call(self, x: tf.Tensor, context: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the cross-attention operation.
+
+        Args:
+            x (tf.Tensor): The query (expected Transformer results) sequence of shape (batch_size, seq_length, d_model).
+            context (tf.Tensor): The context (inputs to the Transformer) sequence of shape (batch_size, seq_length, d_model).
+
+        Returns:
+            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
+        """
+        attn_output, attn_scores = self.mha(query=x, key=context, value=context, return_attention_scores=True)
+
+        # Cache the attention scores for plotting later.
+        self.last_attn_scores = attn_scores
+
+        x = self.add([x, attn_output])
+        x = self.layernorm(x)
+
+        return x
+
+
+class GlobalSelfAttention(BaseAttention):
+    """
+    A class that implements the global self-attention layer by inheriting from the BaseAttention class.
+    This layer is used to process a single sequence and attends to all the tokens in the sequence.
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
+        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
+        add (tf.keras.layers.Add): The Add layer.
+    """
+    def call(self, x: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the global self-attention operation.
+
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
+
+        Returns:
+            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
+        """
+        attn_output = self.mha(query=x, value=x, key=x)
+        x = self.add([x, attn_output])
+        x = self.layernorm(x)
+        return x
+
+
+class CausalSelfAttention(BaseAttention):
+    """
+    Call self attention on the input sequence, ensuring that each position in the 
+    output depends only on previous positions (i.e. a causal model).
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        mha (tf.keras.layers.MultiHeadAttention): The MultiHeadAttention layer.
+        layernorm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
+        add (tf.keras.layers.Add): The Add layer.
+    """
+    def call(self, x: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the causal self-attention operation.
+        
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
+
+        Returns:
+            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
+        """
+        attn_output = self.mha(query=x, value=x, key=x, use_causal_mask = True)
+        x = self.add([x, attn_output])
+        x = self.layernorm(x)
         return x
```

### Comparing `mltu-1.2.4/mltu/tensorflow/transformer/callbacks.py` & `mltu-1.2.5/mltu/tensorflow/transformer/callbacks.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import tensorflow as tf
-from keras.callbacks import Callback
-from mltu.tensorflow.callbacks import Model2onnx
-
-
-class EncDecSplitCallback(Callback):
-    """Callback to extract the encoder and decoder models from Transformer model and save them separately
-    Also, this callback incorporates Model2onnx callback to convert the encoder and decoder models to ONNX format
-
-    Args:
-        model_path (str): Path to save the encoder and decoder models
-        encoder_metadata (dict, optional): Metadata to save with the encoder model. Defaults to None.
-        decoder_metadata (dict, optional): Metadata to save with the decoder model. Defaults to None.
-    """
-
-    def __init__(
-        self,
-        model_path: str,
-        encoder_metadata: dict = None,
-        decoder_metadata: dict = None,
-        model_name = "model.h5"
-    ):
-        """Callback to extract the encoder and decoder models from Transformer model and save them separately"""
-        super(EncDecSplitCallback, self).__init__()
-        self.model_path = model_path
-        self.encoder_metadata = encoder_metadata
-        self.decoder_metadata = decoder_metadata
-        self.model_name = model_name
-
-    def on_train_end(self, epoch: int, logs: dict = None):
-        try:
-            # load best model weights
-            self.model.load_weights(self.model_path + "/" + self.model_name)
-            
-            # extract encoder and decoder models
-            encoder_model = tf.keras.Model(
-                inputs=self.model.inputs[0], outputs=self.model.get_layer("encoder").output
-            )
-            decoder_model = tf.keras.Model(
-                inputs=[self.model.inputs[1], self.model.get_layer("encoder").output],
-                outputs=self.model.layers[-1].output,
-            )
-
-            # save encoder and decoder models
-            encoder_model.save(self.model_path + "/encoder.h5")
-            decoder_model.save(self.model_path + "/decoder.h5")
-
-            # convert encoder and decoder models to onnx
-            Model2onnx.model2onnx(encoder_model, self.model_path + "/encoder.onnx")
-            Model2onnx.model2onnx(decoder_model, self.model_path + "/decoder.onnx")
-
-            # save encoder and decoder metadata
-            if self.encoder_metadata:
-                Model2onnx.include_metadata(self.model_path + "/encoder.onnx", self.encoder_metadata)
-            if self.decoder_metadata:
-                Model2onnx.include_metadata(self.model_path + "/decoder.onnx", self.decoder_metadata)
-        except Exception as e:
-            print(e)
-            pass
+import tensorflow as tf
+from keras.callbacks import Callback
+from mltu.tensorflow.callbacks import Model2onnx
+
+
+class EncDecSplitCallback(Callback):
+    """Callback to extract the encoder and decoder models from Transformer model and save them separately
+    Also, this callback incorporates Model2onnx callback to convert the encoder and decoder models to ONNX format
+
+    Args:
+        model_path (str): Path to save the encoder and decoder models
+        encoder_metadata (dict, optional): Metadata to save with the encoder model. Defaults to None.
+        decoder_metadata (dict, optional): Metadata to save with the decoder model. Defaults to None.
+    """
+
+    def __init__(
+        self,
+        model_path: str,
+        encoder_metadata: dict = None,
+        decoder_metadata: dict = None,
+        model_name = "model.h5"
+    ):
+        """Callback to extract the encoder and decoder models from Transformer model and save them separately"""
+        super(EncDecSplitCallback, self).__init__()
+        self.model_path = model_path
+        self.encoder_metadata = encoder_metadata
+        self.decoder_metadata = decoder_metadata
+        self.model_name = model_name
+
+    def on_train_end(self, epoch: int, logs: dict = None):
+        try:
+            # load best model weights
+            self.model.load_weights(self.model_path + "/" + self.model_name)
+            
+            # extract encoder and decoder models
+            encoder_model = tf.keras.Model(
+                inputs=self.model.inputs[0], outputs=self.model.get_layer("encoder").output
+            )
+            decoder_model = tf.keras.Model(
+                inputs=[self.model.inputs[1], self.model.get_layer("encoder").output],
+                outputs=self.model.layers[-1].output,
+            )
+
+            # save encoder and decoder models
+            encoder_model.save(self.model_path + "/encoder.h5")
+            decoder_model.save(self.model_path + "/decoder.h5")
+
+            # convert encoder and decoder models to onnx
+            Model2onnx.model2onnx(encoder_model, self.model_path + "/encoder.onnx")
+            Model2onnx.model2onnx(decoder_model, self.model_path + "/decoder.onnx")
+
+            # save encoder and decoder metadata
+            if self.encoder_metadata:
+                Model2onnx.include_metadata(self.model_path + "/encoder.onnx", self.encoder_metadata)
+            if self.decoder_metadata:
+                Model2onnx.include_metadata(self.model_path + "/decoder.onnx", self.decoder_metadata)
+        except Exception as e:
+            print(e)
+            pass
```

### Comparing `mltu-1.2.4/mltu/tensorflow/transformer/layers.py` & `mltu-1.2.5/mltu/tensorflow/transformer/layers.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-import tensorflow as tf
-import numpy as np
-
-from .attention import CrossAttention, GlobalSelfAttention, CausalSelfAttention
-
-def positional_encoding(length: int, depth: int):
-    """
-    Generates a positional encoding for a given length and depth.
-
-    Args:
-        length (int): The length of the input sequence.
-        depth (int): The depth that represents the dimensionality of the encoding.
-
-    Returns:
-        tf.Tensor: The positional encoding of shape (length, depth).
-    """
-    depth = depth / 2
-
-    positions = np.arange(length)[:, np.newaxis]     # (seq, 1)
-    depths = np.arange(depth)[np.newaxis, :]/depth   # (1, depth)
-
-    angle_rates = 1 / (10000**depths)         # (1, depth)
-    angle_rads = positions * angle_rates      # (pos, depth)
-
-    pos_encoding = np.concatenate([np.sin(angle_rads), np.cos(angle_rads)], axis=-1) 
-
-    return tf.cast(pos_encoding, dtype=tf.float32)
-
-
-class PositionalEmbedding(tf.keras.layers.Layer):
-    """
-    A positional embedding layer combines the input embedding with a positional encoding that helps the Transformer
-    to understand the relative position of the input tokens. This layer takes the input of tokens and converts them
-    into sequence of embeddings vector. Then, it adds the positional encoding to the embeddings.
-
-    Methods:
-        compute_mask: Computes the mask to be applied to the embeddings.
-        call: Performs the forward pass of the layer.
-    """
-    def __init__(self, vocab_size: int, d_model: int):
-        """ Constructor of the PositionalEmbedding layer.
-
-        Args:
-            vocab_size (int): The size of the vocabulary. I. e. the number of unique tokens in the input sequence.
-            d_model (int): The dimensionality of the embedding vector.
-            embedding (tf.keras.layers.Embedding): The custom embedding layer. If None, a default embedding layer will be created.
-        """
-        super().__init__()
-        self.d_model = d_model
-        if vocab_size is not None:
-            self.embedding = tf.keras.layers.Embedding(vocab_size, d_model, mask_zero=True)
-        self.pos_encoding = positional_encoding(length=2048, depth=d_model)
-
-    def compute_mask(self, *args, **kwargs):
-        """ Computes the mask to be applied to the embeddings.
-
-        Args:
-            inputs: Tensor input(s).
-            mask: Previous mask.
-
-        Returns:
-            tf.Tensor: The computed mask.
-        """
-        if hasattr(self, 'embedding'):
-            return self.embedding.compute_mask(*args, **kwargs)
-        else:
-            return None  # If no embedding layer, return no mask
-
-    def call(self, x: tf.Tensor) -> tf.Tensor:
-        """ Performs the forward pass of the layer.
-        
-        Args:
-            x (tf.Tensor): The input tensor of shape (batch_size, seq_length).
-
-        Returns:
-            tf.Tensor: The output sequence of embedding vectors with added positional information. The shape is
-                (batch_size, seq_length, d_model).
-        """
-        if hasattr(self, 'embedding'):
-            x = self.embedding(x)
-        length = tf.shape(x)[1]
-        # This factor sets the relative scale of the embedding and positonal_encoding.
-        x *= tf.math.sqrt(tf.cast(self.d_model, x.dtype))
-        x = x + tf.cast(self.pos_encoding[tf.newaxis, :length, :], dtype=x.dtype)
-        return x
-    
-class FeedForward(tf.keras.layers.Layer):
-    """
-    A class that implements the feed-forward layer.
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        seq (tf.keras.Sequential): The sequential layer that contains the feed-forward layers. It applies the two feed-forward layers and the dropout layer.
-        add (tf.keras.layers.Add): The Add layer.
-        layer_norm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
-    """
-    def __init__(self, d_model: int, dff: int, dropout_rate: float=0.1, activation: str='relu'):
-        """
-        Constructor of the FeedForward layer.
-
-        Args:
-            d_model (int): The dimensionality of the model.
-            dff (int): The dimensionality of the feed-forward layer.
-            dropout_rate (float): The dropout rate.
-        """
-        super().__init__()
-        self.seq = tf.keras.Sequential([
-            tf.keras.layers.Dense(dff, activation=activation),
-            tf.keras.layers.Dense(d_model),
-            tf.keras.layers.Dropout(dropout_rate)
-        ])
-        self.add = tf.keras.layers.Add()
-        self.layer_norm = tf.keras.layers.LayerNormalization()
-
-    def call(self, x: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the feed-forward operation. 
-
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
-
-        Returns:
-            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
-        """
-        x = self.add([x, self.seq(x)])
-        x = self.layer_norm(x) 
-        return x
-
-
-class EncoderLayer(tf.keras.layers.Layer):
-    """
-    A single layer of the Encoder. Usually there are multiple layers stacked on top of each other.
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        self_attention (GlobalSelfAttention): The global self-attention layer.
-        ffn (FeedForward): The feed-forward layer.
-    """
-    def __init__(self, d_model: int, num_heads: int, dff: int, dropout_rate: float=0.1, activation: str='relu'):
-        """
-        Constructor of the EncoderLayer.
-
-        Args:
-            d_model (int): The dimensionality of the model.
-            num_heads (int): The number of heads in the multi-head attention layer.
-            dff (int): The dimensionality of the feed-forward layer.
-            dropout_rate (float): The dropout rate.
-        """
-        super().__init__()
-
-        self.self_attention = GlobalSelfAttention(
-            num_heads=num_heads,
-            key_dim=d_model,
-            dropout=dropout_rate
-            )
-
-        self.ffn = FeedForward(d_model, dff, dropout_rate, activation)
-
-    def call(self, x: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the forward pass of the layer.
-
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
-
-        Returns:
-            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
-        """
-        x = self.self_attention(x)
-        x = self.ffn(x)
-        return x
-
-class Encoder(tf.keras.layers.Layer):
-    """
-    A custom TensorFlow layer that implements the Encoder. This layer is mostly used in the Transformer models 
-    for natural language processing tasks, such as machine translation, text summarization or text classification.
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        d_model (int): The dimensionality of the model.
-        num_layers (int): The number of layers in the encoder.
-        pos_embedding (PositionalEmbedding): The positional embedding layer.
-        enc_layers (list): The list of encoder layers.
-        dropout (tf.keras.layers.Dropout): The dropout layer.
-    """
-    def __init__(self, num_layers: int, d_model: int, num_heads: int, dff: int, vocab_size: int, dropout_rate: float=0.1, activation: str='relu', **kwargs):
-        """
-        Constructor of the Encoder.
-
-        Args:
-            num_layers (int): The number of layers in the encoder.
-            d_model (int): The dimensionality of the model.
-            num_heads (int): The number of heads in the multi-head attention layer.
-            dff (int): The dimensionality of the feed-forward layer.
-            vocab_size (int): The size of the vocabulary.
-            dropout_rate (float): The dropout rate.
-        """
-        super().__init__(**kwargs)
-
-        self.d_model = d_model
-        self.num_layers = num_layers
-
-        self.pos_embedding = PositionalEmbedding(vocab_size=vocab_size, d_model=d_model)
-
-        self.enc_layers = [
-            EncoderLayer(d_model=d_model,
-                        num_heads=num_heads,
-                        dff=dff,
-                        dropout_rate=dropout_rate,
-                        activation=activation)
-            for _ in range(num_layers)]
-        self.dropout = tf.keras.layers.Dropout(dropout_rate)
-
-
-    def call(self, x: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the forward pass of the layer.
-        
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, seq_length).
-
-        Returns:
-            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
-        """
-        x = self.pos_embedding(x)  
-        # here x has shape `(batch_size, seq_len, d_model)`
-
-        # Add dropout.
-        x = self.dropout(x)
-
-        for i in range(self.num_layers):
-            x = self.enc_layers[i](x)
-
-        return x  # Shape `(batch_size, seq_len, d_model)`.
-
-
-class DecoderLayer(tf.keras.layers.Layer):
-    """
-    A single layer of the Decoder. Usually there are multiple layers stacked on top of each other.
-    
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        causal_self_attention (CausalSelfAttention): The causal self-attention layer.
-        cross_attention (CrossAttention): The cross-attention layer.
-        ffn (FeedForward): The feed-forward layer.
-    """
-    def __init__(self, d_model: int, num_heads: int, dff: int, dropout_rate: float=0.1, activation: str='relu'):
-        """
-        Constructor of the DecoderLayer.
-
-        Args:
-            d_model (int): The dimensionality of the model.
-            num_heads (int): The number of heads in the multi-head attention layer.
-            dff (int): The dimensionality of the feed-forward layer.
-            dropout_rate (float): The dropout rate. 
-        """
-        super(DecoderLayer, self).__init__()
-
-        self.causal_self_attention = CausalSelfAttention(
-            num_heads=num_heads,
-            key_dim=d_model,
-            dropout=dropout_rate)
-
-        self.cross_attention = CrossAttention(
-            num_heads=num_heads,
-            key_dim=d_model,
-            dropout=dropout_rate)
-
-        self.ffn = FeedForward(d_model, dff, dropout_rate, activation=activation)
-
-    def call(self, x: tf.Tensor, context: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the forward pass of the layer.
-
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model). x is usually the output of the previous decoder layer.
-            context (tf.Tensor): The context sequence of shape (batch_size, seq_length, d_model). Context is usually the output of the encoder.
-        """
-        x = self.causal_self_attention(x=x)
-        x = self.cross_attention(x=x, context=context)
-
-        # Cache the last attention scores for plotting later
-        self.last_attn_scores = self.cross_attention.last_attn_scores
-
-        x = self.ffn(x)  # Shape `(batch_size, seq_len, d_model)`.
-        return x
-
-class Decoder(tf.keras.layers.Layer):
-    """
-    A custom TensorFlow layer that implements the Decoder. This layer is mostly used in the Transformer models
-    for natural language processing tasks, such as machine translation, text summarization or text classification.
-
-    Methods:
-        call: Performs the forward pass of the layer.
-
-    Attributes:
-        d_model (int): The dimensionality of the model.
-        num_layers (int): The number of layers in the decoder.
-        pos_embedding (PositionalEmbedding): The positional embedding layer.
-        dec_layers (list): The list of decoder layers.
-        dropout (tf.keras.layers.Dropout): The dropout layer.
-    """
-    def __init__(self, num_layers: int, d_model: int, num_heads: int, dff: int, vocab_size: int, dropout_rate: float=0.1, activation: str='relu', **kwargs):
-        """
-        Constructor of the Decoder.
-
-        Args:
-            num_layers (int): The number of layers in the decoder.
-            d_model (int): The dimensionality of the model.
-            num_heads (int): The number of heads in the multi-head attention layer.
-            dff (int): The dimensionality of the feed-forward layer.
-            vocab_size (int): The size of the vocabulary.
-            dropout_rate (float): The dropout rate.
-        """
-        super().__init__(**kwargs)
-
-        self.d_model = d_model
-        self.num_layers = num_layers
-
-        self.pos_embedding = PositionalEmbedding(vocab_size=vocab_size, d_model=d_model)
-        self.dropout = tf.keras.layers.Dropout(dropout_rate)
-        self.dec_layers = [
-            DecoderLayer(
-                d_model=d_model, 
-                num_heads=num_heads, 
-                dff=dff, 
-                dropout_rate=dropout_rate, 
-                activation=activation) for _ in range(num_layers)]
-
-        self.last_attn_scores = None
-
-    def call(self, x: tf.Tensor, context: tf.Tensor) -> tf.Tensor:
-        """
-        The call function that performs the forward pass of the layer.
-
-        Args:
-            x (tf.Tensor): The input sequence of shape (batch_size, target_seq_len).
-            context (tf.Tensor): The context sequence of shape (batch_size, input_seq_len, d_model).
-        """
-        # `x` is token-IDs shape (batch, target_seq_len)
-        x = self.pos_embedding(x)  # (batch_size, target_seq_len, d_model)
-
-        x = self.dropout(x)
-
-        for i in range(self.num_layers):
-            x  = self.dec_layers[i](x, context)
-
-        self.last_attn_scores = self.dec_layers[-1].last_attn_scores
-
-        # The shape of x is (batch_size, target_seq_len, d_model).
-        return x
-
-def Transformer(
-    input_vocab_size: int, 
-    target_vocab_size: int, 
-    encoder_input_size: int = None,
-    decoder_input_size: int = None,
-    num_layers: int=6, 
-    d_model: int=512, 
-    num_heads: int=8,
-    dff: int=2048,
-    dropout_rate: float=0.1,
-    ) -> tf.keras.Model:
-    """
-    A custom TensorFlow model that implements the Transformer architecture.
-
-    Args:
-        input_vocab_size (int): The size of the input vocabulary.
-        target_vocab_size (int): The size of the target vocabulary.
-        encoder_input_size (int): The size of the encoder input sequence.
-        decoder_input_size (int): The size of the decoder input sequence.
-        num_layers (int): The number of layers in the encoder and decoder.
-        d_model (int): The dimensionality of the model.
-        num_heads (int): The number of heads in the multi-head attention layer.
-        dff (int): The dimensionality of the feed-forward layer.
-        dropout_rate (float): The dropout rate.
-
-    Returns:
-        A TensorFlow Keras model.
-    """
-    encoder_input = tf.keras.layers.Input(shape=(encoder_input_size,), dtype=tf.int64)
-    decoder_input = tf.keras.layers.Input(shape=(decoder_input_size,), dtype=tf.int64)
-
-    encoder = Encoder(num_layers=num_layers, d_model=d_model, num_heads=num_heads, dff=dff, vocab_size=input_vocab_size, dropout_rate=dropout_rate)(encoder_input)
-    decoder = Decoder(num_layers=num_layers, d_model=d_model, num_heads=num_heads, dff=dff, vocab_size=target_vocab_size, dropout_rate=dropout_rate)(decoder_input, encoder)
-
-    output = tf.keras.layers.Dense(target_vocab_size)(decoder)
-
+import tensorflow as tf
+import numpy as np
+
+from .attention import CrossAttention, GlobalSelfAttention, CausalSelfAttention
+
+def positional_encoding(length: int, depth: int):
+    """
+    Generates a positional encoding for a given length and depth.
+
+    Args:
+        length (int): The length of the input sequence.
+        depth (int): The depth that represents the dimensionality of the encoding.
+
+    Returns:
+        tf.Tensor: The positional encoding of shape (length, depth).
+    """
+    depth = depth / 2
+
+    positions = np.arange(length)[:, np.newaxis]     # (seq, 1)
+    depths = np.arange(depth)[np.newaxis, :]/depth   # (1, depth)
+
+    angle_rates = 1 / (10000**depths)         # (1, depth)
+    angle_rads = positions * angle_rates      # (pos, depth)
+
+    pos_encoding = np.concatenate([np.sin(angle_rads), np.cos(angle_rads)], axis=-1) 
+
+    return tf.cast(pos_encoding, dtype=tf.float32)
+
+
+class PositionalEmbedding(tf.keras.layers.Layer):
+    """
+    A positional embedding layer combines the input embedding with a positional encoding that helps the Transformer
+    to understand the relative position of the input tokens. This layer takes the input of tokens and converts them
+    into sequence of embeddings vector. Then, it adds the positional encoding to the embeddings.
+
+    Methods:
+        compute_mask: Computes the mask to be applied to the embeddings.
+        call: Performs the forward pass of the layer.
+    """
+    def __init__(self, vocab_size: int, d_model: int):
+        """ Constructor of the PositionalEmbedding layer.
+
+        Args:
+            vocab_size (int): The size of the vocabulary. I. e. the number of unique tokens in the input sequence.
+            d_model (int): The dimensionality of the embedding vector.
+            embedding (tf.keras.layers.Embedding): The custom embedding layer. If None, a default embedding layer will be created.
+        """
+        super().__init__()
+        self.d_model = d_model
+        if vocab_size is not None:
+            self.embedding = tf.keras.layers.Embedding(vocab_size, d_model, mask_zero=True)
+        self.pos_encoding = positional_encoding(length=2048, depth=d_model)
+
+    def compute_mask(self, *args, **kwargs):
+        """ Computes the mask to be applied to the embeddings.
+
+        Args:
+            inputs: Tensor input(s).
+            mask: Previous mask.
+
+        Returns:
+            tf.Tensor: The computed mask.
+        """
+        if hasattr(self, 'embedding'):
+            return self.embedding.compute_mask(*args, **kwargs)
+        else:
+            return None  # If no embedding layer, return no mask
+
+    def call(self, x: tf.Tensor) -> tf.Tensor:
+        """ Performs the forward pass of the layer.
+        
+        Args:
+            x (tf.Tensor): The input tensor of shape (batch_size, seq_length).
+
+        Returns:
+            tf.Tensor: The output sequence of embedding vectors with added positional information. The shape is
+                (batch_size, seq_length, d_model).
+        """
+        if hasattr(self, 'embedding'):
+            x = self.embedding(x)
+        length = tf.shape(x)[1]
+        # This factor sets the relative scale of the embedding and positonal_encoding.
+        x *= tf.math.sqrt(tf.cast(self.d_model, x.dtype))
+        x = x + tf.cast(self.pos_encoding[tf.newaxis, :length, :], dtype=x.dtype)
+        return x
+    
+class FeedForward(tf.keras.layers.Layer):
+    """
+    A class that implements the feed-forward layer.
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        seq (tf.keras.Sequential): The sequential layer that contains the feed-forward layers. It applies the two feed-forward layers and the dropout layer.
+        add (tf.keras.layers.Add): The Add layer.
+        layer_norm (tf.keras.layers.LayerNormalization): The LayerNormalization layer.
+    """
+    def __init__(self, d_model: int, dff: int, dropout_rate: float=0.1, activation: str='relu'):
+        """
+        Constructor of the FeedForward layer.
+
+        Args:
+            d_model (int): The dimensionality of the model.
+            dff (int): The dimensionality of the feed-forward layer.
+            dropout_rate (float): The dropout rate.
+        """
+        super().__init__()
+        self.seq = tf.keras.Sequential([
+            tf.keras.layers.Dense(dff, activation=activation),
+            tf.keras.layers.Dense(d_model),
+            tf.keras.layers.Dropout(dropout_rate)
+        ])
+        self.add = tf.keras.layers.Add()
+        self.layer_norm = tf.keras.layers.LayerNormalization()
+
+    def call(self, x: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the feed-forward operation. 
+
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
+
+        Returns:
+            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
+        """
+        x = self.add([x, self.seq(x)])
+        x = self.layer_norm(x) 
+        return x
+
+
+class EncoderLayer(tf.keras.layers.Layer):
+    """
+    A single layer of the Encoder. Usually there are multiple layers stacked on top of each other.
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        self_attention (GlobalSelfAttention): The global self-attention layer.
+        ffn (FeedForward): The feed-forward layer.
+    """
+    def __init__(self, d_model: int, num_heads: int, dff: int, dropout_rate: float=0.1, activation: str='relu'):
+        """
+        Constructor of the EncoderLayer.
+
+        Args:
+            d_model (int): The dimensionality of the model.
+            num_heads (int): The number of heads in the multi-head attention layer.
+            dff (int): The dimensionality of the feed-forward layer.
+            dropout_rate (float): The dropout rate.
+        """
+        super().__init__()
+
+        self.self_attention = GlobalSelfAttention(
+            num_heads=num_heads,
+            key_dim=d_model,
+            dropout=dropout_rate
+            )
+
+        self.ffn = FeedForward(d_model, dff, dropout_rate, activation)
+
+    def call(self, x: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the forward pass of the layer.
+
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model).
+
+        Returns:
+            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
+        """
+        x = self.self_attention(x)
+        x = self.ffn(x)
+        return x
+
+class Encoder(tf.keras.layers.Layer):
+    """
+    A custom TensorFlow layer that implements the Encoder. This layer is mostly used in the Transformer models 
+    for natural language processing tasks, such as machine translation, text summarization or text classification.
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        d_model (int): The dimensionality of the model.
+        num_layers (int): The number of layers in the encoder.
+        pos_embedding (PositionalEmbedding): The positional embedding layer.
+        enc_layers (list): The list of encoder layers.
+        dropout (tf.keras.layers.Dropout): The dropout layer.
+    """
+    def __init__(self, num_layers: int, d_model: int, num_heads: int, dff: int, vocab_size: int, dropout_rate: float=0.1, activation: str='relu', **kwargs):
+        """
+        Constructor of the Encoder.
+
+        Args:
+            num_layers (int): The number of layers in the encoder.
+            d_model (int): The dimensionality of the model.
+            num_heads (int): The number of heads in the multi-head attention layer.
+            dff (int): The dimensionality of the feed-forward layer.
+            vocab_size (int): The size of the vocabulary.
+            dropout_rate (float): The dropout rate.
+        """
+        super().__init__(**kwargs)
+
+        self.d_model = d_model
+        self.num_layers = num_layers
+
+        self.pos_embedding = PositionalEmbedding(vocab_size=vocab_size, d_model=d_model)
+
+        self.enc_layers = [
+            EncoderLayer(d_model=d_model,
+                        num_heads=num_heads,
+                        dff=dff,
+                        dropout_rate=dropout_rate,
+                        activation=activation)
+            for _ in range(num_layers)]
+        self.dropout = tf.keras.layers.Dropout(dropout_rate)
+
+
+    def call(self, x: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the forward pass of the layer.
+        
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, seq_length).
+
+        Returns:
+            tf.Tensor: The output sequence of shape (batch_size, seq_length, d_model).
+        """
+        x = self.pos_embedding(x)  
+        # here x has shape `(batch_size, seq_len, d_model)`
+
+        # Add dropout.
+        x = self.dropout(x)
+
+        for i in range(self.num_layers):
+            x = self.enc_layers[i](x)
+
+        return x  # Shape `(batch_size, seq_len, d_model)`.
+
+
+class DecoderLayer(tf.keras.layers.Layer):
+    """
+    A single layer of the Decoder. Usually there are multiple layers stacked on top of each other.
+    
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        causal_self_attention (CausalSelfAttention): The causal self-attention layer.
+        cross_attention (CrossAttention): The cross-attention layer.
+        ffn (FeedForward): The feed-forward layer.
+    """
+    def __init__(self, d_model: int, num_heads: int, dff: int, dropout_rate: float=0.1, activation: str='relu'):
+        """
+        Constructor of the DecoderLayer.
+
+        Args:
+            d_model (int): The dimensionality of the model.
+            num_heads (int): The number of heads in the multi-head attention layer.
+            dff (int): The dimensionality of the feed-forward layer.
+            dropout_rate (float): The dropout rate. 
+        """
+        super(DecoderLayer, self).__init__()
+
+        self.causal_self_attention = CausalSelfAttention(
+            num_heads=num_heads,
+            key_dim=d_model,
+            dropout=dropout_rate)
+
+        self.cross_attention = CrossAttention(
+            num_heads=num_heads,
+            key_dim=d_model,
+            dropout=dropout_rate)
+
+        self.ffn = FeedForward(d_model, dff, dropout_rate, activation=activation)
+
+    def call(self, x: tf.Tensor, context: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the forward pass of the layer.
+
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, seq_length, d_model). x is usually the output of the previous decoder layer.
+            context (tf.Tensor): The context sequence of shape (batch_size, seq_length, d_model). Context is usually the output of the encoder.
+        """
+        x = self.causal_self_attention(x=x)
+        x = self.cross_attention(x=x, context=context)
+
+        # Cache the last attention scores for plotting later
+        self.last_attn_scores = self.cross_attention.last_attn_scores
+
+        x = self.ffn(x)  # Shape `(batch_size, seq_len, d_model)`.
+        return x
+
+class Decoder(tf.keras.layers.Layer):
+    """
+    A custom TensorFlow layer that implements the Decoder. This layer is mostly used in the Transformer models
+    for natural language processing tasks, such as machine translation, text summarization or text classification.
+
+    Methods:
+        call: Performs the forward pass of the layer.
+
+    Attributes:
+        d_model (int): The dimensionality of the model.
+        num_layers (int): The number of layers in the decoder.
+        pos_embedding (PositionalEmbedding): The positional embedding layer.
+        dec_layers (list): The list of decoder layers.
+        dropout (tf.keras.layers.Dropout): The dropout layer.
+    """
+    def __init__(self, num_layers: int, d_model: int, num_heads: int, dff: int, vocab_size: int, dropout_rate: float=0.1, activation: str='relu', **kwargs):
+        """
+        Constructor of the Decoder.
+
+        Args:
+            num_layers (int): The number of layers in the decoder.
+            d_model (int): The dimensionality of the model.
+            num_heads (int): The number of heads in the multi-head attention layer.
+            dff (int): The dimensionality of the feed-forward layer.
+            vocab_size (int): The size of the vocabulary.
+            dropout_rate (float): The dropout rate.
+        """
+        super().__init__(**kwargs)
+
+        self.d_model = d_model
+        self.num_layers = num_layers
+
+        self.pos_embedding = PositionalEmbedding(vocab_size=vocab_size, d_model=d_model)
+        self.dropout = tf.keras.layers.Dropout(dropout_rate)
+        self.dec_layers = [
+            DecoderLayer(
+                d_model=d_model, 
+                num_heads=num_heads, 
+                dff=dff, 
+                dropout_rate=dropout_rate, 
+                activation=activation) for _ in range(num_layers)]
+
+        self.last_attn_scores = None
+
+    def call(self, x: tf.Tensor, context: tf.Tensor) -> tf.Tensor:
+        """
+        The call function that performs the forward pass of the layer.
+
+        Args:
+            x (tf.Tensor): The input sequence of shape (batch_size, target_seq_len).
+            context (tf.Tensor): The context sequence of shape (batch_size, input_seq_len, d_model).
+        """
+        # `x` is token-IDs shape (batch, target_seq_len)
+        x = self.pos_embedding(x)  # (batch_size, target_seq_len, d_model)
+
+        x = self.dropout(x)
+
+        for i in range(self.num_layers):
+            x  = self.dec_layers[i](x, context)
+
+        self.last_attn_scores = self.dec_layers[-1].last_attn_scores
+
+        # The shape of x is (batch_size, target_seq_len, d_model).
+        return x
+
+def Transformer(
+    input_vocab_size: int, 
+    target_vocab_size: int, 
+    encoder_input_size: int = None,
+    decoder_input_size: int = None,
+    num_layers: int=6, 
+    d_model: int=512, 
+    num_heads: int=8,
+    dff: int=2048,
+    dropout_rate: float=0.1,
+    ) -> tf.keras.Model:
+    """
+    A custom TensorFlow model that implements the Transformer architecture.
+
+    Args:
+        input_vocab_size (int): The size of the input vocabulary.
+        target_vocab_size (int): The size of the target vocabulary.
+        encoder_input_size (int): The size of the encoder input sequence.
+        decoder_input_size (int): The size of the decoder input sequence.
+        num_layers (int): The number of layers in the encoder and decoder.
+        d_model (int): The dimensionality of the model.
+        num_heads (int): The number of heads in the multi-head attention layer.
+        dff (int): The dimensionality of the feed-forward layer.
+        dropout_rate (float): The dropout rate.
+
+    Returns:
+        A TensorFlow Keras model.
+    """
+    encoder_input = tf.keras.layers.Input(shape=(encoder_input_size,), dtype=tf.int64)
+    decoder_input = tf.keras.layers.Input(shape=(decoder_input_size,), dtype=tf.int64)
+
+    encoder = Encoder(num_layers=num_layers, d_model=d_model, num_heads=num_heads, dff=dff, vocab_size=input_vocab_size, dropout_rate=dropout_rate)(encoder_input)
+    decoder = Decoder(num_layers=num_layers, d_model=d_model, num_heads=num_heads, dff=dff, vocab_size=target_vocab_size, dropout_rate=dropout_rate)(decoder_input, encoder)
+
+    output = tf.keras.layers.Dense(target_vocab_size)(decoder)
+
     return tf.keras.Model(inputs=[encoder_input, decoder_input], outputs=output)
```

### Comparing `mltu-1.2.4/mltu/tensorflow/transformer/utils.py` & `mltu-1.2.5/mltu/tensorflow/transformer/utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import tensorflow as tf
-
-
-class MaskedLoss(tf.keras.losses.Loss):
-    """ Masked loss function for Transformer.
-
-    Args:
-        mask_value (int, optional): Mask value. Defaults to 0.
-        reduction (str, optional): Reduction method. Defaults to 'none'.
-    """
-    def __init__(self, mask_value: int=0, reduction: str='none') -> None:
-        super(MaskedLoss, self).__init__()
-        self.mask_value = mask_value
-        self.reduction = reduction
-        self.loss_object = tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True, reduction=reduction)
-
-    def __call__(self, y_true: tf.Tensor, y_pred: tf.Tensor, sample_weight=None) -> tf.Tensor:
-        """ Calculate masked loss.
-        
-        Args:
-            y_true (tf.Tensor): True labels.
-            y_pred (tf.Tensor): Predicted labels.
-
-        Returns:
-            tf.Tensor: Masked loss.
-        """
-        mask = y_true != self.mask_value
-        loss = self.loss_object(y_true, y_pred)
-
-        mask = tf.cast(mask, dtype=loss.dtype)
-        loss *= mask
-
-        loss = tf.reduce_sum(loss) / tf.reduce_sum(mask)
-        return loss
-
-
-class MaskedAccuracy(tf.keras.metrics.Metric):
-    """ Masked accuracy metric for Transformer.
-
-    Args:
-        mask_value (int, optional): Mask value. Defaults to 0.
-        name (str, optional): Name of the metric. Defaults to 'masked_accuracy'.
-    """
-    def __init__(self, mask_value: int=0, name: str='masked_accuracy') -> None:
-        super(MaskedAccuracy, self).__init__(name=name)
-        self.mask_value = mask_value
-        self.total = self.add_weight(name='total', initializer='zeros')
-        self.count = self.add_weight(name='count', initializer='zeros')
-
-    @tf.function
-    def update_state(self, y_true: tf.Tensor, y_pred: tf.Tensor, sample_weight=None):
-        """ Update state of the metric.
-
-        Args:
-            y_true (tf.Tensor): True labels.
-            y_pred (tf.Tensor): Predicted labels.
-        """
-        pred = tf.argmax(y_pred, axis=2)
-        label = tf.cast(y_true, pred.dtype)
-        match = label == pred
-
-        mask = label != self.mask_value
-
-        match = match & mask
-
-        match = tf.cast(match, dtype=tf.float32)
-        mask = tf.cast(mask, dtype=tf.float32)
-        match = tf.reduce_sum(match)
-        mask = tf.reduce_sum(mask)
-
-        self.total.assign_add(match)
-        self.count.assign_add(mask)
-
-    def result(self) -> tf.Tensor:
-        """ Calculate masked accuracy.
-
-        Returns:
-            tf.Tensor: Masked accuracy.
-        """
-        return self.total / self.count
-    
-
-class CERMetric(tf.keras.metrics.Metric):
-    """A custom TensorFlow metric to compute the Character Error Rate (CER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-        **kwargs: Additional keyword arguments.
-    """
-    def __init__(self, end_token, padding_token: int=0, name="CER", **kwargs):
-        # Initialize the base Metric class
-        super(CERMetric, self).__init__(name=name, **kwargs)
-        
-        # Initialize variables to keep track of the cumulative character/word error rates and counter
-        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
-        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
-        
-        self.padding_token = padding_token
-        self.end_token = end_token
-
-    def get_cer(self, pred, y_true, padding=-1):
-        """ Calculates the character error rate (CER) between the predicted labels and true labels for a batch of input data.
-
-        Args:
-            pred(tf.Tensor): The predicted labels, with dtype=tf.int32, usually output from tf.keras.backend.ctc_decode
-            y_true (tf.Tensor): The true labels, with dtype=tf.int32
-            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
-
-        Returns:
-            tf.Tensor: The CER between the predicted labels and true labels
-        """
-        # find index where end token is
-        equal = tf.equal(pred, self.end_token)
-        equal_int = tf.cast(equal, tf.int64)
-        end_token_index = tf.argmax(equal_int, axis=1)
-
-        # mask out everything after end token
-        new_range = tf.range(tf.shape(pred)[1], dtype=tf.int64)
-        range_matrix = tf.tile(new_range[None, :], [tf.shape(pred)[0], 1])
-
-        mask = range_matrix <= tf.expand_dims(end_token_index, axis=1)
-        masked_pred = tf.where(mask, pred, padding)
-
-        # Convert the valid predicted labels tensor to a sparse tensor
-        sparse_pred = tf.RaggedTensor.from_tensor(masked_pred, padding=padding).to_sparse()
-
-        # Convert the valid true labels tensor to a sparse tensor
-        sparse_true = tf.RaggedTensor.from_tensor(y_true, padding=padding).to_sparse()
-
-        # Calculate the normalized edit distance between the sparse predicted labels tensor and sparse true labels tensor
-        distance = tf.edit_distance(sparse_pred, sparse_true, normalize=True)
-
-        return distance
-
-    # @tf.function
-    def update_state(self, y_true, y_pred, sample_weight=None):
-        """Updates the state variables of the metric.
-
-        Args:
-            y_true: A tensor of true labels with shape (batch_size, sequence_length).
-            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
-            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
-        """
-        pred = tf.argmax(y_pred, axis=2)
-
-        # Calculate the normalized edit distance between the predicted labels and true labels tensors
-        distance = self.get_cer(pred, y_true, self.padding_token)
-
-        # Add the sum of the distance tensor to the cer_accumulator variable
-        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
-        
-        # Increment the batch_counter by the batch size
-        self.batch_counter.assign_add(len(y_true))
-
-    def result(self):
-        """ Computes and returns the metric result.
-
-        Returns:
-            A TensorFlow float representing the CER (character error rate).
-        """
+import tensorflow as tf
+
+
+class MaskedLoss(tf.keras.losses.Loss):
+    """ Masked loss function for Transformer.
+
+    Args:
+        mask_value (int, optional): Mask value. Defaults to 0.
+        reduction (str, optional): Reduction method. Defaults to 'none'.
+    """
+    def __init__(self, mask_value: int=0, reduction: str='none') -> None:
+        super(MaskedLoss, self).__init__()
+        self.mask_value = mask_value
+        self.reduction = reduction
+        self.loss_object = tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True, reduction=reduction)
+
+    def __call__(self, y_true: tf.Tensor, y_pred: tf.Tensor, sample_weight=None) -> tf.Tensor:
+        """ Calculate masked loss.
+        
+        Args:
+            y_true (tf.Tensor): True labels.
+            y_pred (tf.Tensor): Predicted labels.
+
+        Returns:
+            tf.Tensor: Masked loss.
+        """
+        mask = y_true != self.mask_value
+        loss = self.loss_object(y_true, y_pred)
+
+        mask = tf.cast(mask, dtype=loss.dtype)
+        loss *= mask
+
+        loss = tf.reduce_sum(loss) / tf.reduce_sum(mask)
+        return loss
+
+
+class MaskedAccuracy(tf.keras.metrics.Metric):
+    """ Masked accuracy metric for Transformer.
+
+    Args:
+        mask_value (int, optional): Mask value. Defaults to 0.
+        name (str, optional): Name of the metric. Defaults to 'masked_accuracy'.
+    """
+    def __init__(self, mask_value: int=0, name: str='masked_accuracy') -> None:
+        super(MaskedAccuracy, self).__init__(name=name)
+        self.mask_value = mask_value
+        self.total = self.add_weight(name='total', initializer='zeros')
+        self.count = self.add_weight(name='count', initializer='zeros')
+
+    @tf.function
+    def update_state(self, y_true: tf.Tensor, y_pred: tf.Tensor, sample_weight=None):
+        """ Update state of the metric.
+
+        Args:
+            y_true (tf.Tensor): True labels.
+            y_pred (tf.Tensor): Predicted labels.
+        """
+        pred = tf.argmax(y_pred, axis=2)
+        label = tf.cast(y_true, pred.dtype)
+        match = label == pred
+
+        mask = label != self.mask_value
+
+        match = match & mask
+
+        match = tf.cast(match, dtype=tf.float32)
+        mask = tf.cast(mask, dtype=tf.float32)
+        match = tf.reduce_sum(match)
+        mask = tf.reduce_sum(mask)
+
+        self.total.assign_add(match)
+        self.count.assign_add(mask)
+
+    def result(self) -> tf.Tensor:
+        """ Calculate masked accuracy.
+
+        Returns:
+            tf.Tensor: Masked accuracy.
+        """
+        return self.total / self.count
+    
+
+class CERMetric(tf.keras.metrics.Metric):
+    """A custom TensorFlow metric to compute the Character Error Rate (CER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+        **kwargs: Additional keyword arguments.
+    """
+    def __init__(self, end_token, padding_token: int=0, name="CER", **kwargs):
+        # Initialize the base Metric class
+        super(CERMetric, self).__init__(name=name, **kwargs)
+        
+        # Initialize variables to keep track of the cumulative character/word error rates and counter
+        self.cer_accumulator = tf.Variable(0.0, name="cer_accumulator", dtype=tf.float32)
+        self.batch_counter = tf.Variable(0, name="batch_counter", dtype=tf.int32)
+        
+        self.padding_token = padding_token
+        self.end_token = end_token
+
+    def get_cer(self, pred, y_true, padding=-1):
+        """ Calculates the character error rate (CER) between the predicted labels and true labels for a batch of input data.
+
+        Args:
+            pred(tf.Tensor): The predicted labels, with dtype=tf.int32, usually output from tf.keras.backend.ctc_decode
+            y_true (tf.Tensor): The true labels, with dtype=tf.int32
+            padding (int, optional): The padding token when converting to sparse tensor. Defaults to -1.
+
+        Returns:
+            tf.Tensor: The CER between the predicted labels and true labels
+        """
+        # find index where end token is
+        equal = tf.equal(pred, self.end_token)
+        equal_int = tf.cast(equal, tf.int64)
+        end_token_index = tf.argmax(equal_int, axis=1)
+
+        # mask out everything after end token
+        new_range = tf.range(tf.shape(pred)[1], dtype=tf.int64)
+        range_matrix = tf.tile(new_range[None, :], [tf.shape(pred)[0], 1])
+
+        mask = range_matrix <= tf.expand_dims(end_token_index, axis=1)
+        masked_pred = tf.where(mask, pred, padding)
+
+        # Convert the valid predicted labels tensor to a sparse tensor
+        sparse_pred = tf.RaggedTensor.from_tensor(masked_pred, padding=padding).to_sparse()
+
+        # Convert the valid true labels tensor to a sparse tensor
+        sparse_true = tf.RaggedTensor.from_tensor(y_true, padding=padding).to_sparse()
+
+        # Calculate the normalized edit distance between the sparse predicted labels tensor and sparse true labels tensor
+        distance = tf.edit_distance(sparse_pred, sparse_true, normalize=True)
+
+        return distance
+
+    # @tf.function
+    def update_state(self, y_true, y_pred, sample_weight=None):
+        """Updates the state variables of the metric.
+
+        Args:
+            y_true: A tensor of true labels with shape (batch_size, sequence_length).
+            y_pred: A tensor of predicted labels with shape (batch_size, sequence_length, num_classes).
+            sample_weight: (Optional) a tensor of weights with shape (batch_size, sequence_length).
+        """
+        pred = tf.argmax(y_pred, axis=2)
+
+        # Calculate the normalized edit distance between the predicted labels and true labels tensors
+        distance = self.get_cer(pred, y_true, self.padding_token)
+
+        # Add the sum of the distance tensor to the cer_accumulator variable
+        self.cer_accumulator.assign_add(tf.reduce_sum(distance))
+        
+        # Increment the batch_counter by the batch size
+        self.batch_counter.assign_add(len(y_true))
+
+    def result(self):
+        """ Computes and returns the metric result.
+
+        Returns:
+            A TensorFlow float representing the CER (character error rate).
+        """
         return tf.math.divide_no_nan(self.cer_accumulator, tf.cast(self.batch_counter, tf.float32))
```

### Comparing `mltu-1.2.4/mltu/tokenizers.py` & `mltu-1.2.5/mltu/tokenizers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-import os
-import json
-import typing
-from tqdm import tqdm
-
-class CustomTokenizer:
-    """ Custom Tokenizer class to tokenize and detokenize text data into sequences of integers
-
-    Args:
-        split (str, optional): Split token to use when tokenizing text. Defaults to " ".
-        char_level (bool, optional): Whether to tokenize at character level. Defaults to False.
-        lower (bool, optional): Whether to convert text to lowercase. Defaults to True.
-        start_token (str, optional): Start token to use when tokenizing text. Defaults to "<start>".
-        end_token (str, optional): End token to use when tokenizing text. Defaults to "<eos>".
-        filters (list, optional): List of characters to filter out. Defaults to 
-            ['!', "'", '"', '#', '$', '%', '&', '(', ')', '*', '+', ',', '-', '.', '/', ':', ';', '<', '=', '>', 
-            '?', '@', '[', '\\', ']', '^', '_', '`', '{', '|', '}', '~', '\t', '\n'].
-        filter_nums (bool, optional): Whether to filter out numbers. Defaults to True.
-        start (int, optional): Index to start tokenizing from. Defaults to 1.
-    """
-    def __init__(
-            self, 
-            split: str=" ", 
-            char_level: bool=False,
-            lower: bool=True, 
-            start_token: str="<start>", 
-            end_token: str="<eos>",
-            filters: list = ['!', "'", '"', '#', '$', '%', '&', '(', ')', '*', '+', ',', '-', '.', '/', ':', ';', '<', '=', '>', '?', '@', '[', '\\', ']', '^', '_', '`', '{', '|', '}', '~', '\t', '\n'],
-            filter_nums: bool = True,
-            start: int=1,
-        ) -> None:
-        self.split = split
-        self.char_level = char_level
-        self.lower = lower
-        self.index_word = {}
-        self.word_index = {}
-        self.max_length = 0
-        self.start_token = start_token
-        self.end_token = end_token
-        self.filters = filters
-        self.filter_nums = filter_nums
-        self.start = start
-
-    @property
-    def start_token_index(self):
-        return self.word_index[self.start_token]
-    
-    @property
-    def end_token_index(self):
-        return self.word_index[self.end_token]
-
-    def sort(self):
-        """ Sorts the word_index and index_word dictionaries"""
-        self.index_word = dict(enumerate(dict(sorted(self.word_index.items())), start=self.start))
-        self.word_index = {v: k for k, v in self.index_word.items()}
-
-    def split_line(self, line: str):
-        """ Splits a line of text into tokens
-
-        Args:
-            line (str): Line of text to split
-
-        Returns:
-            list: List of string tokens
-        """
-        line = line.lower() if self.lower else line
-
-        if self.char_level:
-            return [char for char in line]
-
-        # split line with split token and check for filters
-        line_tokens = line.split(self.split)
-
-        new_tokens = []
-        for index, token in enumerate(line_tokens):
-            filtered_tokens = ['']
-            for c_index, char in enumerate(token):
-                if char in self.filters or (self.filter_nums and char.isdigit()):
-                    filtered_tokens += [char, ''] if c_index != len(token) -1 else [char]
-                else:
-                    filtered_tokens[-1] += char
-
-            new_tokens += filtered_tokens
-            if index != len(line_tokens) -1:
-                new_tokens += [self.split]
-
-        new_tokens = [token for token in new_tokens if token != '']
-
-        return new_tokens
-
-    def fit_on_texts(self, lines: typing.List[str]):
-        """ Fits the tokenizer on a list of lines of text
-        This function will update the word_index and index_word dictionaries and set the max_length attribute
-
-        Args:
-            lines (typing.List[str]): List of lines of text to fit the tokenizer on
-        """
-        self.word_index = {key: value for value, key in enumerate([self.start_token, self.end_token, self.split] + self.filters)}
-        
-        for line in tqdm(lines, desc="Fitting tokenizer"):
-            line_tokens = self.split_line(line)
-            self.max_length = max(self.max_length, len(line_tokens) +2) # +2 for start and end tokens
-
-            for token in line_tokens:
-                if token not in self.word_index:
-                    self.word_index[token] = len(self.word_index)
-
-        self.sort()
-
-    def update(self, lines: typing.List[str]):
-        """ Updates the tokenizer with new lines of text
-        This function will update the word_index and index_word dictionaries and set the max_length attribute
-
-        Args:
-            lines (typing.List[str]): List of lines of text to update the tokenizer with
-        """
-        new_tokens = 0
-        for line in tqdm(lines, desc="Updating tokenizer"):
-            line_tokens = self.split_line(line)
-            self.max_length = max(self.max_length, len(line_tokens) +2) # +2 for start and end tokens
-            for token in line_tokens:
-                if token not in self.word_index:
-                    self.word_index[token] = len(self.word_index)
-                    new_tokens += 1
-
-        self.sort()
-        print(f"Added {new_tokens} new tokens")
-
-    def detokenize(self, sequences: typing.List[int], remove_start_end: bool=True):
-        """ Converts a list of sequences of tokens back into text
-
-        Args:
-            sequences (typing.list[int]): List of sequences of tokens to convert back into text
-            remove_start_end (bool, optional): Whether to remove the start and end tokens. Defaults to True.
-        
-        Returns:
-            typing.List[str]: List of strings of the converted sequences
-        """
-        lines = []
-        for sequence in sequences:
-            line = ""
-            for token in sequence:
-                if token == 0:
-                    break
-                if remove_start_end and (token == self.start_token_index or token == self.end_token_index):
-                    continue
-
-                line += self.index_word[token]
-
-            lines.append(line)
-
-        return lines
-
-    def texts_to_sequences(self, lines: typing.List[str], include_start_end: bool=True):
-        """ Converts a list of lines of text into a list of sequences of tokens
-        
-        Args:
-            lines (typing.list[str]): List of lines of text to convert into tokenized sequences
-            include_start_end (bool, optional): Whether to include the start and end tokens. Defaults to True.
-
-        Returns:
-            typing.List[typing.List[int]]: List of sequences of tokens
-        """
-        sequences = []
-        for line in lines:
-            line_tokens = self.split_line(line)
-            sequence = [self.word_index[word] for word in line_tokens if word in self.word_index]
-            if include_start_end:
-                sequence = [self.word_index[self.start_token]] + sequence + [self.word_index[self.end_token]]
-
-            sequences.append(sequence)
-
-        return sequences
-    
-    def save(self, path: str, type: str="json"):
-        """ Saves the tokenizer to a file
-        
-        Args:
-            path (str): Path to save the tokenizer to
-            type (str, optional): Type of file to save the tokenizer to. Defaults to "json".
-        """
-        serialised_dict = self.dict()
-        if type == "json":
-            if os.path.dirname(path):
-                os.makedirs(os.path.dirname(path), exist_ok=True)
-            with open(path, "w") as f:
-                json.dump(serialised_dict, f)
-
-    def dict(self):
-        """ Returns a dictionary of the tokenizer
-
-        Returns:
-            dict: Dictionary of the tokenizer
-        """
-        return {
-            "split": self.split,
-            "lower": self.lower,
-            "char_level": self.char_level,
-            "index_word": self.index_word,
-            "max_length": self.max_length,
-            "start_token": self.start_token,
-            "end_token": self.end_token,
-            "filters": self.filters,
-            "filter_nums": self.filter_nums,
-            "start": self.start
-        }
-
-    @staticmethod
-    def load(path: typing.Union[str, dict], type: str="json"):
-        """ Loads a tokenizer from a file
-
-        Args:
-            path (typing.Union[str, dict]): Path to load the tokenizer from or a dictionary of the tokenizer
-            type (str, optional): Type of file to load the tokenizer from. Defaults to "json".
-
-        Returns:
-            CustomTokenizer: Loaded tokenizer
-        """
-        if isinstance(path, str):
-            if type == "json":
-                with open(path, "r") as f:
-                    load_dict = json.load(f)
-
-        elif isinstance(path, dict):
-            load_dict = path
-
-        tokenizer = CustomTokenizer()
-        tokenizer.split = load_dict["split"]
-        tokenizer.lower = load_dict["lower"]
-        tokenizer.char_level = load_dict["char_level"]
-        tokenizer.index_word = {int(k): v for k, v in load_dict["index_word"].items()}
-        tokenizer.max_length = load_dict["max_length"]
-        tokenizer.start_token = load_dict["start_token"]
-        tokenizer.end_token = load_dict["end_token"]
-        tokenizer.filters = load_dict["filters"]
-        tokenizer.filter_nums = bool(load_dict["filter_nums"])
-        tokenizer.start = load_dict["start"]
-        tokenizer.word_index = {v: int(k) for k, v in tokenizer.index_word.items()}
-
-        return tokenizer
-    
-    @property
-    def lenght(self):
-        return len(self.index_word)
-
-    def __len__(self):
+import os
+import json
+import typing
+from tqdm import tqdm
+
+class CustomTokenizer:
+    """ Custom Tokenizer class to tokenize and detokenize text data into sequences of integers
+
+    Args:
+        split (str, optional): Split token to use when tokenizing text. Defaults to " ".
+        char_level (bool, optional): Whether to tokenize at character level. Defaults to False.
+        lower (bool, optional): Whether to convert text to lowercase. Defaults to True.
+        start_token (str, optional): Start token to use when tokenizing text. Defaults to "<start>".
+        end_token (str, optional): End token to use when tokenizing text. Defaults to "<eos>".
+        filters (list, optional): List of characters to filter out. Defaults to 
+            ['!', "'", '"', '#', '$', '%', '&', '(', ')', '*', '+', ',', '-', '.', '/', ':', ';', '<', '=', '>', 
+            '?', '@', '[', '\\', ']', '^', '_', '`', '{', '|', '}', '~', '\t', '\n'].
+        filter_nums (bool, optional): Whether to filter out numbers. Defaults to True.
+        start (int, optional): Index to start tokenizing from. Defaults to 1.
+    """
+    def __init__(
+            self, 
+            split: str=" ", 
+            char_level: bool=False,
+            lower: bool=True, 
+            start_token: str="<start>", 
+            end_token: str="<eos>",
+            filters: list = ['!', "'", '"', '#', '$', '%', '&', '(', ')', '*', '+', ',', '-', '.', '/', ':', ';', '<', '=', '>', '?', '@', '[', '\\', ']', '^', '_', '`', '{', '|', '}', '~', '\t', '\n'],
+            filter_nums: bool = True,
+            start: int=1,
+        ) -> None:
+        self.split = split
+        self.char_level = char_level
+        self.lower = lower
+        self.index_word = {}
+        self.word_index = {}
+        self.max_length = 0
+        self.start_token = start_token
+        self.end_token = end_token
+        self.filters = filters
+        self.filter_nums = filter_nums
+        self.start = start
+
+    @property
+    def start_token_index(self):
+        return self.word_index[self.start_token]
+    
+    @property
+    def end_token_index(self):
+        return self.word_index[self.end_token]
+
+    def sort(self):
+        """ Sorts the word_index and index_word dictionaries"""
+        self.index_word = dict(enumerate(dict(sorted(self.word_index.items())), start=self.start))
+        self.word_index = {v: k for k, v in self.index_word.items()}
+
+    def split_line(self, line: str):
+        """ Splits a line of text into tokens
+
+        Args:
+            line (str): Line of text to split
+
+        Returns:
+            list: List of string tokens
+        """
+        line = line.lower() if self.lower else line
+
+        if self.char_level:
+            return [char for char in line]
+
+        # split line with split token and check for filters
+        line_tokens = line.split(self.split)
+
+        new_tokens = []
+        for index, token in enumerate(line_tokens):
+            filtered_tokens = ['']
+            for c_index, char in enumerate(token):
+                if char in self.filters or (self.filter_nums and char.isdigit()):
+                    filtered_tokens += [char, ''] if c_index != len(token) -1 else [char]
+                else:
+                    filtered_tokens[-1] += char
+
+            new_tokens += filtered_tokens
+            if index != len(line_tokens) -1:
+                new_tokens += [self.split]
+
+        new_tokens = [token for token in new_tokens if token != '']
+
+        return new_tokens
+
+    def fit_on_texts(self, lines: typing.List[str]):
+        """ Fits the tokenizer on a list of lines of text
+        This function will update the word_index and index_word dictionaries and set the max_length attribute
+
+        Args:
+            lines (typing.List[str]): List of lines of text to fit the tokenizer on
+        """
+        self.word_index = {key: value for value, key in enumerate([self.start_token, self.end_token, self.split] + self.filters)}
+        
+        for line in tqdm(lines, desc="Fitting tokenizer"):
+            line_tokens = self.split_line(line)
+            self.max_length = max(self.max_length, len(line_tokens) +2) # +2 for start and end tokens
+
+            for token in line_tokens:
+                if token not in self.word_index:
+                    self.word_index[token] = len(self.word_index)
+
+        self.sort()
+
+    def update(self, lines: typing.List[str]):
+        """ Updates the tokenizer with new lines of text
+        This function will update the word_index and index_word dictionaries and set the max_length attribute
+
+        Args:
+            lines (typing.List[str]): List of lines of text to update the tokenizer with
+        """
+        new_tokens = 0
+        for line in tqdm(lines, desc="Updating tokenizer"):
+            line_tokens = self.split_line(line)
+            self.max_length = max(self.max_length, len(line_tokens) +2) # +2 for start and end tokens
+            for token in line_tokens:
+                if token not in self.word_index:
+                    self.word_index[token] = len(self.word_index)
+                    new_tokens += 1
+
+        self.sort()
+        print(f"Added {new_tokens} new tokens")
+
+    def detokenize(self, sequences: typing.List[int], remove_start_end: bool=True):
+        """ Converts a list of sequences of tokens back into text
+
+        Args:
+            sequences (typing.list[int]): List of sequences of tokens to convert back into text
+            remove_start_end (bool, optional): Whether to remove the start and end tokens. Defaults to True.
+        
+        Returns:
+            typing.List[str]: List of strings of the converted sequences
+        """
+        lines = []
+        for sequence in sequences:
+            line = ""
+            for token in sequence:
+                if token == 0:
+                    break
+                if remove_start_end and (token == self.start_token_index or token == self.end_token_index):
+                    continue
+
+                line += self.index_word[token]
+
+            lines.append(line)
+
+        return lines
+
+    def texts_to_sequences(self, lines: typing.List[str], include_start_end: bool=True):
+        """ Converts a list of lines of text into a list of sequences of tokens
+        
+        Args:
+            lines (typing.list[str]): List of lines of text to convert into tokenized sequences
+            include_start_end (bool, optional): Whether to include the start and end tokens. Defaults to True.
+
+        Returns:
+            typing.List[typing.List[int]]: List of sequences of tokens
+        """
+        sequences = []
+        for line in lines:
+            line_tokens = self.split_line(line)
+            sequence = [self.word_index[word] for word in line_tokens if word in self.word_index]
+            if include_start_end:
+                sequence = [self.word_index[self.start_token]] + sequence + [self.word_index[self.end_token]]
+
+            sequences.append(sequence)
+
+        return sequences
+    
+    def save(self, path: str, type: str="json"):
+        """ Saves the tokenizer to a file
+        
+        Args:
+            path (str): Path to save the tokenizer to
+            type (str, optional): Type of file to save the tokenizer to. Defaults to "json".
+        """
+        serialised_dict = self.dict()
+        if type == "json":
+            if os.path.dirname(path):
+                os.makedirs(os.path.dirname(path), exist_ok=True)
+            with open(path, "w") as f:
+                json.dump(serialised_dict, f)
+
+    def dict(self):
+        """ Returns a dictionary of the tokenizer
+
+        Returns:
+            dict: Dictionary of the tokenizer
+        """
+        return {
+            "split": self.split,
+            "lower": self.lower,
+            "char_level": self.char_level,
+            "index_word": self.index_word,
+            "max_length": self.max_length,
+            "start_token": self.start_token,
+            "end_token": self.end_token,
+            "filters": self.filters,
+            "filter_nums": self.filter_nums,
+            "start": self.start
+        }
+
+    @staticmethod
+    def load(path: typing.Union[str, dict], type: str="json"):
+        """ Loads a tokenizer from a file
+
+        Args:
+            path (typing.Union[str, dict]): Path to load the tokenizer from or a dictionary of the tokenizer
+            type (str, optional): Type of file to load the tokenizer from. Defaults to "json".
+
+        Returns:
+            CustomTokenizer: Loaded tokenizer
+        """
+        if isinstance(path, str):
+            if type == "json":
+                with open(path, "r") as f:
+                    load_dict = json.load(f)
+
+        elif isinstance(path, dict):
+            load_dict = path
+
+        tokenizer = CustomTokenizer()
+        tokenizer.split = load_dict["split"]
+        tokenizer.lower = load_dict["lower"]
+        tokenizer.char_level = load_dict["char_level"]
+        tokenizer.index_word = {int(k): v for k, v in load_dict["index_word"].items()}
+        tokenizer.max_length = load_dict["max_length"]
+        tokenizer.start_token = load_dict["start_token"]
+        tokenizer.end_token = load_dict["end_token"]
+        tokenizer.filters = load_dict["filters"]
+        tokenizer.filter_nums = bool(load_dict["filter_nums"])
+        tokenizer.start = load_dict["start"]
+        tokenizer.word_index = {v: int(k) for k, v in tokenizer.index_word.items()}
+
+        return tokenizer
+    
+    @property
+    def lenght(self):
+        return len(self.index_word)
+
+    def __len__(self):
         return len(self.index_word)
```

### Comparing `mltu-1.2.4/mltu/torch/dataProvider.py` & `mltu-1.2.5/mltu/torch/dataProvider.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-import os
-import typing
-import pandas as pd
-
-from ..augmentors import Augmentor
-from ..transformers import Transformer
-from ..dataProvider import DataProvider as BaseDataProvider
-
-import multiprocessing
-import concurrent.futures
-import threading
-import queue
-
-
-class ThreadExecutor:
-    def __init__(self, target: typing.Callable, workers: int = os.cpu_count()) -> None:
-        self.target = target
-        self.workers = workers
-        
-        self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=workers)
-
-    def __call__(self, data: typing.Any) -> typing.Any:
-        results = self._executor.map(self.target, data)
-        return results
-    
-    def __exit__(self):
-        self._executor.shutdown()
-
-
-class Worker:
-    """ Worker class for multiprocessing """
-    def __init__(self, target: typing.Callable, timeout: int=1) -> None:
-        self.target = target
-        self.timeout = timeout
-        self.conn_sender, self.conn_receiver = multiprocessing.Pipe()
-        self.worker = multiprocessing.Process(target=self.run_worker, args=(target, self.conn_receiver))
-        self.worker.start()
-        self.busy = False
-
-    def run_worker(self, function, conn_receiver):
-        while True:
-            try:
-                if conn_receiver.poll(self.timeout):
-                    data = conn_receiver.recv()
-                    if data is not None:
-                        if data == "stop":
-                            break
-                        else:
-                            result = function(data)
-                            conn_receiver.send(result)
-                            data = None
-            except:
-                pass
-
-        conn_receiver.send("stop")
-
-    def send(self, data):
-        if self.busy:
-            return None
-        
-        self.busy = True
-        self.data = data
-        self.conn_sender.send(data)
-        return self
-
-    def get(self):
-        if self.conn_sender.poll(self.timeout):
-            results = self.conn_sender.recv()
-            self.busy = False
-            return results
-        else:
-            self.busy = True
-            self.conn_sender.send(self.data)
-            return self
-    
-    def __exit__(self):
-        while True:
-            if self.busy:
-                continue
-
-            self.conn_sender.send("stop")
-            stop = self.conn_sender.recv()
-            if stop == "stop":
-                self.worker.join()
-                self.worker.terminate()
-                break
-
-
-class ProcessExecutor:
-    def __init__(self, target: typing.Callable, workers: int = os.cpu_count()) -> None:
-        self.target = target
-        self.workers = workers
-        self.busy = False
-
-        self.mp_workers = [Worker(target) for _ in range(self.workers)]
-
-    def __enter__(self):
-        return self
-    
-    def __exit__(self):
-        for worker in self.mp_workers:
-            worker.__exit__()
- 
-    def __call__(self, data) -> typing.Any:
-        self.busy = True
-        results = [None for _ in range(len(data))]
-        finished = [0 for _ in range(len(data))]
-        while True:
-            # send data to workers
-            for index, data_batch in enumerate(data):
-                for worker in self.mp_workers:
-                    if worker.busy == False and results[index] is None:
-                        results[index] = worker.send(data_batch)
-                        break
-
-            # receive data from workers
-            for i, result in enumerate(results):
-                if result is None:
-                    continue
-
-                if isinstance(result, Worker):
-                    results[i] = result.get()
-
-                if not isinstance(result, Worker):
-                    finished[i] = 1
-           
-            if sum(finished) == len(data):
-                break
-        
-        self.busy = False
-        return results
-
-
-class DataProvider(BaseDataProvider):
-    """ DataProvider for PyTorch with multiprocessing and multithreading support.
-    """
-    def __init__(
-            self, 
-            dataset: typing.Union[str, list, pd.DataFrame],
-            data_preprocessors: typing.List[typing.Callable] = None,
-            batch_size: int = 4,
-            shuffle: bool = True,
-            initial_epoch: int = 1,
-            augmentors: typing.List[Augmentor] = None,
-            transformers: typing.List[Transformer] = None,
-            batch_postprocessors: typing.List[typing.Callable] = None,
-            skip_validation: bool = True,
-            limit: int = None,
-            use_cache: bool = False,
-            workers: int = os.cpu_count(),
-            use_multiprocessing: bool = False,
-            max_queue_size: int = 5,
-            **kwargs
-        ):
-        """ Standardised object for providing data to a model while training.
-
-        Args:
-            dataset (str, list, pd.DataFrame): Path to dataset, list of data or pandas dataframe of data.
-            data_preprocessors (list): List of data preprocessors. (e.g. [read image, read audio, etc.])
-            batch_size (int): The number of samples to include in each batch. Defaults to 4.
-            shuffle (bool): Whether to shuffle the data. Defaults to True.
-            initial_epoch (int): The initial epoch. Defaults to 1.
-            augmentors (list, optional): List of augmentor functions. Defaults to None.
-            transformers (list, optional): List of transformer functions. Defaults to None.
-            batch_postprocessors (list, optional): List of batch postprocessor functions. Defaults to None.
-            skip_validation (bool, optional): Whether to skip validation. Defaults to True.
-            limit (int, optional): Limit the number of samples in the dataset. Defaults to None.
-            use_cache (bool, optional): Whether to cache the dataset. Defaults to False.
-            workers (int, optional): Number of workers to use for multiprocessing or multithreading. Defaults to os.cpu_count().
-            use_multiprocessing (bool, optional): Whether to use multiprocessing or multithreading. Defaults to multithreading (False).
-            max_queue_size (int, optional): Maximum size of the queue. Defaults to 5.
-            numpy (bool, optional): Whether to convert data to numpy. Defaults to True.
-        """
-        super(DataProvider, self).__init__(dataset=dataset, data_preprocessors=data_preprocessors, batch_size=batch_size, 
-                                           shuffle=shuffle, initial_epoch=initial_epoch, augmentors=augmentors, transformers=transformers, batch_postprocessors=batch_postprocessors,
-                                           skip_validation=skip_validation, limit=limit, use_cache=use_cache, **kwargs)
-        self.workers = workers
-        self.use_multiprocessing = use_multiprocessing
-        self.max_queue_size = max_queue_size
-
-    def start_executor(self) -> None:
-        """ Start the executor for multiprocessing or multithreading"""
-
-        if not hasattr(self, "_executor"):
-            if self.use_multiprocessing:
-                try:
-                    self._executor = ProcessExecutor(self.process_data, self.workers)
-                except:
-                    self.use_multiprocessing = False
-                    self.logger.error("Failed to start multiprocessing, switching to multithreading")
-                    self._executor = ThreadExecutor(self.process_data, self.workers)
-            else:
-                self._executor = ThreadExecutor(self.process_data, self.workers)
-
-        if not hasattr(self, "_sequenceHandler"):
-            self._sequenceHandler = SequenceHandler(self.__getitem__, len(self), self.max_queue_size, self._shuffle)
-
-    def __iter__(self):
-        """ Yealds a batch of processed data by index until the end of the dataset """
-        self.start_executor()
-        for index in range(len(self)):
-            results = self._sequenceHandler(index)
-            yield results
-
-        self.__exit__()
-
-    def __exit__(self):
-        """ Shutdown and remove the executors """
-        self._executor.__exit__()
-        del self._executor
-        self._sequenceHandler.__exit__()
-        del self._sequenceHandler
-
-
-class SequenceHandler:
-    """ SequenceHandler used to preprocess batches of data in parallel in the background."""
-    def __init__(
-            self, 
-            function: typing.Callable, 
-            max_len: int, 
-            queue_size: int=5, 
-            shuffle: bool=True
-        ) -> None:
-        self.function = function
-        self.max_len = max_len
-        self.queue_size = queue_size
-        self.shuffle = shuffle
-
-        self.data_queue, self.result_queue = queue.Queue(), queue.Queue()
-
-        self.thread_workers = [threading.Thread(target=self.worker_function) for _ in range(self.queue_size)]
-        for worker in self.thread_workers:
-            worker.start()
-
-        self.results_dict = {}
-
-    def worker_function(self):
-        while True:
-            # Get data from the queue (or other source)
-            data_index = self.data_queue.get()
-
-            if data_index == "stop":
-                self.result_queue.put("stop")
-                break
-            
-            # Perform some processing on the data
-            result = self.function(data_index)
-            
-            # Put the result in the result queue
-            self.result_queue.put({data_index: result})
-
-    def __exit__(self):
-        for _ in self.thread_workers:
-            self.data_queue.put("stop")
-            stop = self.result_queue.get()
-            if stop == "stop":
-                # worker stopped
-                pass 
-            else:
-                print("Something went wrong")
-
-    def __call__(self, index: int):
-        if index == 0:
-            for _index in range(self.queue_size):
-                if _index >= self.max_len:
-                    break
-                self.data_queue.put(_index)
-
-        while True:
-            # join results_dict with received results
-            # check if queue is not empty
-            try:
-                worker_results = self.result_queue.get(timeout=10)
-            except:
-                # used for debugging
-                continue
-
-            if not worker_results:
-                continue
-
-            if self.shuffle: # ignore batch order by index (works faster)
-                next_index = index + self.queue_size
-                if next_index < self.max_len:
-                    self.data_queue.put(next_index)
-                return list(worker_results.values())[0]
-
-            # return batch in order by index
-            self.results_dict.update(worker_results)
-            result = self.results_dict.get(index, None)
-            if result is not None:
-                next_index = index + self.queue_size
-                if next_index < self.max_len:
-                    self.data_queue.put(next_index)
-                del self.results_dict[index]
+import os
+import typing
+import pandas as pd
+
+from ..augmentors import Augmentor
+from ..transformers import Transformer
+from ..dataProvider import DataProvider as BaseDataProvider
+
+import multiprocessing
+import concurrent.futures
+import threading
+import queue
+
+
+class ThreadExecutor:
+    def __init__(self, target: typing.Callable, workers: int = os.cpu_count()) -> None:
+        self.target = target
+        self.workers = workers
+        
+        self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=workers)
+
+    def __call__(self, data: typing.Any) -> typing.Any:
+        results = self._executor.map(self.target, data)
+        return results
+    
+    def __exit__(self):
+        self._executor.shutdown()
+
+
+class Worker:
+    """ Worker class for multiprocessing """
+    def __init__(self, target: typing.Callable, timeout: int=1) -> None:
+        self.target = target
+        self.timeout = timeout
+        self.conn_sender, self.conn_receiver = multiprocessing.Pipe()
+        self.worker = multiprocessing.Process(target=self.run_worker, args=(target, self.conn_receiver))
+        self.worker.start()
+        self.busy = False
+
+    def run_worker(self, function, conn_receiver):
+        while True:
+            try:
+                if conn_receiver.poll(self.timeout):
+                    data = conn_receiver.recv()
+                    if data is not None:
+                        if data == "stop":
+                            break
+                        else:
+                            result = function(data)
+                            conn_receiver.send(result)
+                            data = None
+            except:
+                pass
+
+        conn_receiver.send("stop")
+
+    def send(self, data):
+        if self.busy:
+            return None
+        
+        self.busy = True
+        self.data = data
+        self.conn_sender.send(data)
+        return self
+
+    def get(self):
+        if self.conn_sender.poll(self.timeout):
+            results = self.conn_sender.recv()
+            self.busy = False
+            return results
+        else:
+            self.busy = True
+            self.conn_sender.send(self.data)
+            return self
+    
+    def __exit__(self):
+        while True:
+            if self.busy:
+                continue
+
+            self.conn_sender.send("stop")
+            stop = self.conn_sender.recv()
+            if stop == "stop":
+                self.worker.join()
+                self.worker.terminate()
+                break
+
+
+class ProcessExecutor:
+    def __init__(self, target: typing.Callable, workers: int = os.cpu_count()) -> None:
+        self.target = target
+        self.workers = workers
+        self.busy = False
+
+        self.mp_workers = [Worker(target) for _ in range(self.workers)]
+
+    def __enter__(self):
+        return self
+    
+    def __exit__(self):
+        for worker in self.mp_workers:
+            worker.__exit__()
+ 
+    def __call__(self, data) -> typing.Any:
+        self.busy = True
+        results = [None for _ in range(len(data))]
+        finished = [0 for _ in range(len(data))]
+        while True:
+            # send data to workers
+            for index, data_batch in enumerate(data):
+                for worker in self.mp_workers:
+                    if worker.busy == False and results[index] is None:
+                        results[index] = worker.send(data_batch)
+                        break
+
+            # receive data from workers
+            for i, result in enumerate(results):
+                if result is None:
+                    continue
+
+                if isinstance(result, Worker):
+                    results[i] = result.get()
+
+                if not isinstance(result, Worker):
+                    finished[i] = 1
+           
+            if sum(finished) == len(data):
+                break
+        
+        self.busy = False
+        return results
+
+
+class DataProvider(BaseDataProvider):
+    """ DataProvider for PyTorch with multiprocessing and multithreading support.
+    """
+    def __init__(
+            self, 
+            dataset: typing.Union[str, list, pd.DataFrame],
+            data_preprocessors: typing.List[typing.Callable] = None,
+            batch_size: int = 4,
+            shuffle: bool = True,
+            initial_epoch: int = 1,
+            augmentors: typing.List[Augmentor] = None,
+            transformers: typing.List[Transformer] = None,
+            batch_postprocessors: typing.List[typing.Callable] = None,
+            skip_validation: bool = True,
+            limit: int = None,
+            use_cache: bool = False,
+            workers: int = os.cpu_count(),
+            use_multiprocessing: bool = False,
+            max_queue_size: int = 5,
+            **kwargs
+        ):
+        """ Standardised object for providing data to a model while training.
+
+        Args:
+            dataset (str, list, pd.DataFrame): Path to dataset, list of data or pandas dataframe of data.
+            data_preprocessors (list): List of data preprocessors. (e.g. [read image, read audio, etc.])
+            batch_size (int): The number of samples to include in each batch. Defaults to 4.
+            shuffle (bool): Whether to shuffle the data. Defaults to True.
+            initial_epoch (int): The initial epoch. Defaults to 1.
+            augmentors (list, optional): List of augmentor functions. Defaults to None.
+            transformers (list, optional): List of transformer functions. Defaults to None.
+            batch_postprocessors (list, optional): List of batch postprocessor functions. Defaults to None.
+            skip_validation (bool, optional): Whether to skip validation. Defaults to True.
+            limit (int, optional): Limit the number of samples in the dataset. Defaults to None.
+            use_cache (bool, optional): Whether to cache the dataset. Defaults to False.
+            workers (int, optional): Number of workers to use for multiprocessing or multithreading. Defaults to os.cpu_count().
+            use_multiprocessing (bool, optional): Whether to use multiprocessing or multithreading. Defaults to multithreading (False).
+            max_queue_size (int, optional): Maximum size of the queue. Defaults to 5.
+            numpy (bool, optional): Whether to convert data to numpy. Defaults to True.
+        """
+        super(DataProvider, self).__init__(dataset=dataset, data_preprocessors=data_preprocessors, batch_size=batch_size, 
+                                           shuffle=shuffle, initial_epoch=initial_epoch, augmentors=augmentors, transformers=transformers, batch_postprocessors=batch_postprocessors,
+                                           skip_validation=skip_validation, limit=limit, use_cache=use_cache, **kwargs)
+        self.workers = workers
+        self.use_multiprocessing = use_multiprocessing
+        self.max_queue_size = max_queue_size
+
+    def start_executor(self) -> None:
+        """ Start the executor for multiprocessing or multithreading"""
+
+        if not hasattr(self, "_executor"):
+            if self.use_multiprocessing:
+                try:
+                    self._executor = ProcessExecutor(self.process_data, self.workers)
+                except:
+                    self.use_multiprocessing = False
+                    self.logger.error("Failed to start multiprocessing, switching to multithreading")
+                    self._executor = ThreadExecutor(self.process_data, self.workers)
+            else:
+                self._executor = ThreadExecutor(self.process_data, self.workers)
+
+        if not hasattr(self, "_sequenceHandler"):
+            self._sequenceHandler = SequenceHandler(self.__getitem__, len(self), self.max_queue_size, self._shuffle)
+
+    def __iter__(self):
+        """ Yealds a batch of processed data by index until the end of the dataset """
+        self.start_executor()
+        for index in range(len(self)):
+            results = self._sequenceHandler(index)
+            yield results
+
+        self.__exit__()
+
+    def __exit__(self):
+        """ Shutdown and remove the executors """
+        self._executor.__exit__()
+        del self._executor
+        self._sequenceHandler.__exit__()
+        del self._sequenceHandler
+
+
+class SequenceHandler:
+    """ SequenceHandler used to preprocess batches of data in parallel in the background."""
+    def __init__(
+            self, 
+            function: typing.Callable, 
+            max_len: int, 
+            queue_size: int=5, 
+            shuffle: bool=True
+        ) -> None:
+        self.function = function
+        self.max_len = max_len
+        self.queue_size = queue_size
+        self.shuffle = shuffle
+
+        self.data_queue, self.result_queue = queue.Queue(), queue.Queue()
+
+        self.thread_workers = [threading.Thread(target=self.worker_function) for _ in range(self.queue_size)]
+        for worker in self.thread_workers:
+            worker.start()
+
+        self.results_dict = {}
+
+    def worker_function(self):
+        while True:
+            # Get data from the queue (or other source)
+            data_index = self.data_queue.get()
+
+            if data_index == "stop":
+                self.result_queue.put("stop")
+                break
+            
+            # Perform some processing on the data
+            result = self.function(data_index)
+            
+            # Put the result in the result queue
+            self.result_queue.put({data_index: result})
+
+    def __exit__(self):
+        for _ in self.thread_workers:
+            self.data_queue.put("stop")
+            stop = self.result_queue.get()
+            if stop == "stop":
+                # worker stopped
+                pass 
+            else:
+                print("Something went wrong")
+
+    def __call__(self, index: int):
+        if index == 0:
+            for _index in range(self.queue_size):
+                if _index >= self.max_len:
+                    break
+                self.data_queue.put(_index)
+
+        while True:
+            # join results_dict with received results
+            # check if queue is not empty
+            try:
+                worker_results = self.result_queue.get(timeout=10)
+            except:
+                # used for debugging
+                continue
+
+            if not worker_results:
+                continue
+
+            if self.shuffle: # ignore batch order by index (works faster)
+                next_index = index + self.queue_size
+                if next_index < self.max_len:
+                    self.data_queue.put(next_index)
+                return list(worker_results.values())[0]
+
+            # return batch in order by index
+            self.results_dict.update(worker_results)
+            result = self.results_dict.get(index, None)
+            if result is not None:
+                next_index = index + self.queue_size
+                if next_index < self.max_len:
+                    self.data_queue.put(next_index)
+                del self.results_dict[index]
                 return result
```

### Comparing `mltu-1.2.4/mltu/torch/handlers.py` & `mltu-1.2.5/mltu/torch/handlers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import typing
-
-from .metrics import Metric
-from .callbacks import Callback
-
-class MetricsHandler:
-    """ Metrics handler class for training and testing loops"""
-    def __init__(self, metrics: typing.List[Metric]):
-        self.metrics = metrics
-
-        # Validate metrics
-        if not all(isinstance(m, Metric) for m in self.metrics):
-            raise TypeError("all items in the metrics argument must be of type Metric (Check mltu.metrics.metrics.py for more information)")
-        
-        self.train_results_dict = {"loss": None}
-        self.train_results_dict.update({metric.name: None for metric in self.metrics})
-        
-        self.val_results_dict = {"val_loss": None}
-        self.val_results_dict.update({"val_" + metric.name: None for metric in self.metrics})
-
-    def update(self, target, output, **kwargs):
-        for metric in self.metrics:
-            metric.update(output, target, **kwargs)
-
-    def reset(self):
-        for metric in self.metrics:
-            metric.reset()
-
-    def results(self, loss, train: bool=True):
-        suffix = "val_" if not train else ""
-        results_dict = self.val_results_dict if not train else self.train_results_dict
-        results_dict[suffix + "loss"] = loss
-        for metric in self.metrics:
-            result = metric.result()
-            if result:
-                if isinstance(result, dict):
-                    for k, v in result.items():
-                        results_dict[suffix + k] = v
-                else:
-                    results_dict[suffix + metric.name] = result
-
-        logs = {k: round(v, 4) for k, v in results_dict.items() if v is not None}
-        return logs
-    
-    def description(self, epoch: int=None, train: bool=True):
-        epoch_desc = f"Epoch {epoch} - " if epoch is not None else "          "
-        dict = self.train_results_dict if train else self.val_results_dict
-        return epoch_desc + " - ".join([f"{k}: {v:.4f}" for k, v in dict.items() if v])
-    
-
-class CallbacksHandler:
-    """ Callbacks handler class for training and testing loops"""
-    def __init__(self, model, callbacks: typing.List[Callback]):
-        self.callbacks = callbacks
-
-        # Validate callbacks
-        if not all(isinstance(c, Callback) for c in self.callbacks):
-            raise TypeError("all items in the callbacks argument must be of type Callback (Check mltu.torch.callbacks.py for more information)")
-        
-        for callback in self.callbacks:
-            callback.model = model
-        
-    def on_train_begin(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_train_begin(logs)
-
-    def on_train_end(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_train_end(logs)
-
-    def on_epoch_begin(self, epoch, logs=None):
-        for callback in self.callbacks:
-            callback.on_epoch_begin(epoch, logs)
-
-    def on_epoch_end(self, epoch, logs=None):
-        for callback in self.callbacks:
-            callback.on_epoch_end(epoch, logs)
-
-    def on_test_begin(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_test_begin(logs)
-
-    def on_test_end(self, logs=None):
-        for callback in self.callbacks:
-            callback.on_test_end(logs)
-
-    def on_batch_begin(self, batch: int, logs=None, train: bool=True):
-        for callback in self.callbacks:
-            callback.on_batch_begin(batch, logs)
-
-            if train:
-                callback.on_train_batch_begin(batch, logs)
-            else:
-                callback.on_test_batch_begin(batch, logs)
-
-    def on_batch_end(self, batch: int, logs=None, train: bool=True):
-        for callback in self.callbacks:
-            callback.on_batch_end(batch, logs)
-
-            if train:
-                callback.on_train_batch_end(batch, logs)
-            else:
+import typing
+
+from .metrics import Metric
+from .callbacks import Callback
+
+class MetricsHandler:
+    """ Metrics handler class for training and testing loops"""
+    def __init__(self, metrics: typing.List[Metric]):
+        self.metrics = metrics
+
+        # Validate metrics
+        if not all(isinstance(m, Metric) for m in self.metrics):
+            raise TypeError("all items in the metrics argument must be of type Metric (Check mltu.metrics.metrics.py for more information)")
+        
+        self.train_results_dict = {"loss": None}
+        self.train_results_dict.update({metric.name: None for metric in self.metrics})
+        
+        self.val_results_dict = {"val_loss": None}
+        self.val_results_dict.update({"val_" + metric.name: None for metric in self.metrics})
+
+    def update(self, target, output, **kwargs):
+        for metric in self.metrics:
+            metric.update(output, target, **kwargs)
+
+    def reset(self):
+        for metric in self.metrics:
+            metric.reset()
+
+    def results(self, loss, train: bool=True):
+        suffix = "val_" if not train else ""
+        results_dict = self.val_results_dict if not train else self.train_results_dict
+        results_dict[suffix + "loss"] = loss
+        for metric in self.metrics:
+            result = metric.result()
+            if result:
+                if isinstance(result, dict):
+                    for k, v in result.items():
+                        results_dict[suffix + k] = v
+                else:
+                    results_dict[suffix + metric.name] = result
+
+        logs = {k: round(v, 4) for k, v in results_dict.items() if v is not None}
+        return logs
+    
+    def description(self, epoch: int=None, train: bool=True):
+        epoch_desc = f"Epoch {epoch} - " if epoch is not None else "          "
+        dict = self.train_results_dict if train else self.val_results_dict
+        return epoch_desc + " - ".join([f"{k}: {v:.4f}" for k, v in dict.items() if v])
+    
+
+class CallbacksHandler:
+    """ Callbacks handler class for training and testing loops"""
+    def __init__(self, model, callbacks: typing.List[Callback]):
+        self.callbacks = callbacks
+
+        # Validate callbacks
+        if not all(isinstance(c, Callback) for c in self.callbacks):
+            raise TypeError("all items in the callbacks argument must be of type Callback (Check mltu.torch.callbacks.py for more information)")
+        
+        for callback in self.callbacks:
+            callback.model = model
+        
+    def on_train_begin(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_train_begin(logs)
+
+    def on_train_end(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_train_end(logs)
+
+    def on_epoch_begin(self, epoch, logs=None):
+        for callback in self.callbacks:
+            callback.on_epoch_begin(epoch, logs)
+
+    def on_epoch_end(self, epoch, logs=None):
+        for callback in self.callbacks:
+            callback.on_epoch_end(epoch, logs)
+
+    def on_test_begin(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_test_begin(logs)
+
+    def on_test_end(self, logs=None):
+        for callback in self.callbacks:
+            callback.on_test_end(logs)
+
+    def on_batch_begin(self, batch: int, logs=None, train: bool=True):
+        for callback in self.callbacks:
+            callback.on_batch_begin(batch, logs)
+
+            if train:
+                callback.on_train_batch_begin(batch, logs)
+            else:
+                callback.on_test_batch_begin(batch, logs)
+
+    def on_batch_end(self, batch: int, logs=None, train: bool=True):
+        for callback in self.callbacks:
+            callback.on_batch_end(batch, logs)
+
+            if train:
+                callback.on_train_batch_end(batch, logs)
+            else:
                 callback.on_test_batch_end(batch, logs)
```

### Comparing `mltu-1.2.4/mltu/torch/metrics.py` & `mltu-1.2.5/mltu/torch/metrics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import torch
-import typing
-import numpy as np
-from itertools import groupby
-
-from mltu.utils.text_utils import get_cer, get_wer
-
-
-class Metric:
-    """ Base class for all metrics"""
-    def __init__(self, name: str) -> None:
-        """ Initialize metric with name
-
-        Args:
-            name (str): name of metric
-        """
-        self.name = name
-
-    def reset(self):
-        """ Reset metric state to initial values and return metric value"""
-        self.__init__()
-
-    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs):
-        """ Update metric state with new data
-        
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        pass
-
-    def result(self):
-        """ Return metric value"""
-        pass
-
-
-class Accuracy(Metric):
-    """ Accuracy metric class
-    
-    Args:
-        name (str, optional): name of metric. Defaults to 'accuracy'.
-    """
-    def __init__(self, name="accuracy") -> None:
-        super(Accuracy, self).__init__(name=name)
-        self.correct = 0
-        self.total = 0
-
-    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs):
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        _, predicted = torch.max(output.data, 1)
-        self.total += target.size(0)
-        self.correct += (predicted == target).sum().item()
-
-    def result(self):
-        """ Return metric value"""
-        return self.correct / self.total
-
-
-class CERMetric(Metric):
-    """A custom PyTorch metric to compute the Character Error Rate (CER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-
-    # TODO: implement everything in Torch to avoid converting to numpy
-    """
-    def __init__(
-        self, 
-        vocabulary: typing.Union[str, list],
-        name: str = "CER"
-    ) -> None:
-        super(CERMetric, self).__init__(name=name)
-        self.vocabulary = vocabulary
-        self.reset()
-
-    def reset(self):
-        """ Reset metric state to initial values"""
-        self.cer = 0
-        self.counter = 0
-
-    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs) -> None:
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        # convert to numpy
-        output = output.detach().cpu().numpy()
-        target = target.detach().cpu().numpy()
-        # use argmax to find the index of the highest probability
-        argmax_preds = np.argmax(output, axis=-1)
-        
-        # use groupby to find continuous same indexes
-        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
-
-        # convert indexes to strings
-        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
-        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
-
-        cer = get_cer(output_texts, target_texts)
-
-        self.cer += cer
-        self.counter += 1
-
-    def result(self) -> float:
-        """ Return metric value"""
-        return self.cer / self.counter
-    
-
-class WERMetric(Metric):
-    """A custom PyTorch metric to compute the Word Error Rate (WER).
-    
-    Args:
-        vocabulary: A string of the vocabulary used to encode the labels.
-        name: (Optional) string name of the metric instance.
-
-    # TODO: implement everything in Torch to avoid converting to numpy
-    """
-    def __init__(
-        self, 
-        vocabulary: typing.Union[str, list],
-        name: str = "WER"
-    ) -> None:
-        super(WERMetric, self).__init__(name=name)
-        self.vocabulary = vocabulary
-        self.reset()
-
-    def reset(self):
-        """ Reset metric state to initial values"""
-        self.wer = 0
-        self.counter = 0
-
-    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs) -> None:
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        # convert to numpy
-        output = output.detach().cpu().numpy()
-        target = target.detach().cpu().numpy()
-        # use argmax to find the index of the highest probability
-        argmax_preds = np.argmax(output, axis=-1)
-        
-        # use groupby to find continuous same indexes
-        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
-
-        # convert indexes to strings
-        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
-        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
-
-        wer = get_wer(output_texts, target_texts)
-
-        self.wer += wer
-        self.counter += 1
-
-    def result(self) -> float:
-        """ Return metric value"""
+import torch
+import typing
+import numpy as np
+from itertools import groupby
+
+from mltu.utils.text_utils import get_cer, get_wer
+
+
+class Metric:
+    """ Base class for all metrics"""
+    def __init__(self, name: str) -> None:
+        """ Initialize metric with name
+
+        Args:
+            name (str): name of metric
+        """
+        self.name = name
+
+    def reset(self):
+        """ Reset metric state to initial values and return metric value"""
+        self.__init__()
+
+    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs):
+        """ Update metric state with new data
+        
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        pass
+
+    def result(self):
+        """ Return metric value"""
+        pass
+
+
+class Accuracy(Metric):
+    """ Accuracy metric class
+    
+    Args:
+        name (str, optional): name of metric. Defaults to 'accuracy'.
+    """
+    def __init__(self, name="accuracy") -> None:
+        super(Accuracy, self).__init__(name=name)
+        self.correct = 0
+        self.total = 0
+
+    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs):
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        _, predicted = torch.max(output.data, 1)
+        self.total += target.size(0)
+        self.correct += (predicted == target).sum().item()
+
+    def result(self):
+        """ Return metric value"""
+        return self.correct / self.total
+
+
+class CERMetric(Metric):
+    """A custom PyTorch metric to compute the Character Error Rate (CER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+
+    # TODO: implement everything in Torch to avoid converting to numpy
+    """
+    def __init__(
+        self, 
+        vocabulary: typing.Union[str, list],
+        name: str = "CER"
+    ) -> None:
+        super(CERMetric, self).__init__(name=name)
+        self.vocabulary = vocabulary
+        self.reset()
+
+    def reset(self):
+        """ Reset metric state to initial values"""
+        self.cer = 0
+        self.counter = 0
+
+    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs) -> None:
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        # convert to numpy
+        output = output.detach().cpu().numpy()
+        target = target.detach().cpu().numpy()
+        # use argmax to find the index of the highest probability
+        argmax_preds = np.argmax(output, axis=-1)
+        
+        # use groupby to find continuous same indexes
+        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
+
+        # convert indexes to strings
+        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
+        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
+
+        cer = get_cer(output_texts, target_texts)
+
+        self.cer += cer
+        self.counter += 1
+
+    def result(self) -> float:
+        """ Return metric value"""
+        return self.cer / self.counter
+    
+
+class WERMetric(Metric):
+    """A custom PyTorch metric to compute the Word Error Rate (WER).
+    
+    Args:
+        vocabulary: A string of the vocabulary used to encode the labels.
+        name: (Optional) string name of the metric instance.
+
+    # TODO: implement everything in Torch to avoid converting to numpy
+    """
+    def __init__(
+        self, 
+        vocabulary: typing.Union[str, list],
+        name: str = "WER"
+    ) -> None:
+        super(WERMetric, self).__init__(name=name)
+        self.vocabulary = vocabulary
+        self.reset()
+
+    def reset(self):
+        """ Reset metric state to initial values"""
+        self.wer = 0
+        self.counter = 0
+
+    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs) -> None:
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        # convert to numpy
+        output = output.detach().cpu().numpy()
+        target = target.detach().cpu().numpy()
+        # use argmax to find the index of the highest probability
+        argmax_preds = np.argmax(output, axis=-1)
+        
+        # use groupby to find continuous same indexes
+        grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
+
+        # convert indexes to strings
+        output_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in grouped_preds]
+        target_texts = ["".join([self.vocabulary[k] for k in group if k < len(self.vocabulary)]) for group in target]
+
+        wer = get_wer(output_texts, target_texts)
+
+        self.wer += wer
+        self.counter += 1
+
+    def result(self) -> float:
+        """ Return metric value"""
         return self.wer / self.counter
```

### Comparing `mltu-1.2.4/mltu/torch/model.py` & `mltu-1.2.5/mltu/torch/model.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,428 +1,428 @@
-import os
-import math
-import torch
-import typing
-import traceback
-import numpy as np
-from torch import nn
-from copy import deepcopy
-from qqdm import qqdm, format_str
-from pathlib import Path
-
-from .metrics import Metric
-from .callbacks import Callback
-from .dataProvider import DataProvider
-from .handlers import MetricsHandler, CallbacksHandler
-
-def toTorch(data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
-    """ Check if data is of type torch.Tensor, if not convert it to torch.Tensor
-
-    Args:
-        data (np.ndarray): data to be converted
-        target (np.ndarray): target to be converted
-
-    Returns:
-        typing.Tuple[torch.Tensor, torch.Tensor]: converted data and target
-    """
-    if not isinstance(data, torch.Tensor):
-        data = torch.from_numpy(data)
-
-    if not isinstance(target, (torch.Tensor, dict)):
-        target = torch.from_numpy(target)
-
-    if data.dtype != torch.float32:
-        data = data.float()
-
-    return data, target
-
-
-def is_parallel(model):
-    """Returns True if model is of type DP or DDP."""
-    return isinstance(model, (nn.parallel.DataParallel, nn.parallel.DistributedDataParallel))
-
-def de_parallel(model):
-    """De-parallelize a model: returns single-GPU model if model is of type DP or DDP."""
-    return model.module if is_parallel(model) else model
-
-def copy_attr(a, b, include=(), exclude=()):
-    """Copies attributes from object 'b' to object 'a', with options to include/exclude certain attributes."""
-    for k, v in b.__dict__.items():
-        if (len(include) and k not in include) or k.startswith("_") or k in exclude:
-            continue
-        else:
-            setattr(a, k, v)
-
-class ModelEMA:
-    """Updated Exponential Moving Average (EMA) from https://github.com/rwightman/pytorch-image-models
-    Keeps a moving average of everything in the model state_dict (parameters and buffers)
-    For EMA details see https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
-    To disable EMA set the `enabled` attribute to `False`.
-    """
-
-    def __init__(self, model, decay=0.9999, tau=2000, updates=0):
-        """Create EMA."""
-        self.ema = deepcopy(de_parallel(model)).eval()  # FP32 EMA
-        self.updates = updates  # number of EMA updates
-        self.decay = lambda x: decay * (1 - math.exp(-x / tau))  # decay exponential ramp (to help early epochs)
-        for p in self.ema.parameters():
-            p.requires_grad_(False)
-        self.enabled = True
-
-    def update(self, model):
-        """Update EMA parameters."""
-        if self.enabled:
-            self.updates += 1
-            d = self.decay(self.updates)
-
-            msd = de_parallel(model).state_dict()  # model state_dict
-            for k, v in self.ema.state_dict().items():
-                if v.dtype.is_floating_point:  # true for FP16 and FP32
-                    v *= d
-                    v += (1 - d) * msd[k].detach()
-                    # assert v.dtype == msd[k].dtype == torch.float32, f'{k}: EMA {v.dtype},  model {msd[k].dtype}'
-
-    def update_attr(self, model, include=(), exclude=("process_group", "reducer")):
-        """Updates attributes and saves stripped model with optimizer removed."""
-        if self.enabled:
-            copy_attr(self.ema, model, include, exclude)
-
-
-class Model:
-    """ Model class for training and testing PyTorch neural networks"""
-    def __init__(
-        self, 
-        model: torch.nn.Module, 
-        optimizer: torch.optim.Optimizer, 
-        loss: typing.Callable,
-        metrics: typing.List[Metric] = [],
-        mixed_precision: bool = False,
-        scaler = None,
-        log_errors: bool = True,
-        output_path: str = None,
-        clip_grad_norm: float = None,
-        ema = False,
-        ):
-        """ Initialize model class
-
-        Attributes:
-            model (torch.nn.Module): PyTorch neural network
-            optimizer (torch.optim.Optimizer): PyTorch optimizer
-            loss (typing.Callable): loss function
-            metrics (typing.List[Metric], optional): list of metrics. Defaults to [].
-            mixed_precision (bool, optional): whether to use mixed precision. Defaults to False.
-            scaler (torch.cuda.amp.GradScaler, optional): PyTorch GradScaler. Defaults to None.
-            log_errors (bool, optional): whether to log errors. Defaults to True.
-            output_path (str, optional): path to save model. Defaults to None.
-            clip_grad_norm (float, optional): gradient clipping value. Defaults to None.
-            ema (bool, optional): whether to use Exponential Moving Average. Defaults to False.
-        """
-        self.model = model
-        self.optimizer = optimizer
-        self.loss = loss
-        # get device on which model is running
-        self._device = next(self.model.parameters()).device
-
-        self.metrics = MetricsHandler(metrics)
-
-        self.mixed_precision = mixed_precision
-        self.scaler = torch.cuda.amp.GradScaler() if mixed_precision else scaler
-        self.log_errors = log_errors
-
-        self.output_path = Path(output_path) if output_path else None
-        if self.output_path:
-            if self.output_path.suffix == "":
-                self.output_path = Path(os.path.join(self.output_path, "model.pt"))
-            os.makedirs(self.output_path.parent, exist_ok=True)
-
-        self.stop_training = False
-        self.clip_grad_norm = clip_grad_norm
-        self.ema = ModelEMA(self.model) if ema else None
-
-        self.validate()
-
-    @property
-    def device(self):
-        return self._device
-
-    def validate(self):
-        """ Validate model, optimizer"""
-        if not isinstance(self.model, torch.nn.Module):
-            raise TypeError("model argument must be a torch.nn.Module")
-        
-        if not isinstance(self.optimizer, torch.optim.Optimizer):
-            raise TypeError("optimizer argument must be a torch.optim.Optimizer")
-        
-    def toDevice(self, data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
-        """ Check if data is on the same device as model, if not move it to the device
-
-        Args:
-            data (np.ndarray): data to be moved
-            target (np.ndarray): target to be moved
-
-        Returns:
-            typing.Tuple[torch.Tensor, torch.Tensor]: moved data and target
-        """
-        try:
-            if data.device != self._device:
-                data = data.to(self._device)
-
-            if target.device != self._device:
-                target = target.to(self._device)
-        except AttributeError:
-            if self.log_errors:
-                print("Data and target must be of type torch.Tensor")
-
-        return data, target
-
-    def train_step(
-        self, 
-        data: typing.Union[np.ndarray, torch.Tensor], 
-        target: typing.Union[np.ndarray, torch.Tensor],
-        loss_info: dict = {}
-        ) -> torch.Tensor:
-        """ Perform one training step
-
-        Args:
-            data (typing.Union[np.ndarray, torch.Tensor]): training data
-            target (typing.Union[np.ndarray, torch.Tensor]): training target
-            loss_info (dict, optional): additional loss information. Defaults to {}.
-
-        Returns:
-            torch.Tensor: loss
-        """
-        self.optimizer.zero_grad()
-        if self.mixed_precision:
-            with torch.cuda.amp.autocast():
-                output = self.model(data)
-                loss = self.loss(output, target)
-                if isinstance(loss, tuple):
-                    loss, loss_info = loss[0], loss[1:]
-                self.scaler.scale(loss).backward()
-                if self.clip_grad_norm:
-                    torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=self.clip_grad_norm)
-                self.scaler.step(self.optimizer)
-                self.scaler.update()
-
-        else:
-            output = self.model(data)
-            loss = self.loss(output, target)
-            if isinstance(loss, tuple):
-                loss, loss_info = loss[0], loss[1:]
-            loss.backward()
-            if self.clip_grad_norm:
-                torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=self.clip_grad_norm)
-            self.optimizer.step()
-
-        if self.ema:
-            try:
-                self.ema.update(self.model)
-            except RuntimeError:
-                self.ema = ModelEMA(self.model)
-                self.ema.update(self.model)
-
-        if self._device.type == "cuda":
-            torch.cuda.synchronize() # synchronize after each forward and backward pass
-
-        self.metrics.update(target, output, model=self.model, loss_info=loss_info)
-
-        return loss
-    
-    def test_step(
-        self, 
-        data: typing.Union[np.ndarray, torch.Tensor], 
-        target: typing.Union[np.ndarray, torch.Tensor],
-        loss_info: dict = {}
-        ) -> torch.Tensor:
-        """ Perform one validation step
-
-        Args:
-            data (typing.Union[np.ndarray, torch.Tensor]): validation data
-            target (typing.Union[np.ndarray, torch.Tensor]): validation target
-            loss_info (dict, optional): additional loss information. Defaults to {}.
-
-        Returns:
-            torch.Tensor: loss
-        """
-        output = self.ema.ema(data) if self.ema else self.model(data)
-        loss = self.loss(output, target)
-        if isinstance(loss, tuple):
-            loss, loss_info = loss[0], loss[1:]
-
-        self.metrics.update(target, output, model=self.model, loss_info=loss_info)
-
-        # clear GPU memory cache after each validation step
-        torch.cuda.empty_cache()
-
-        return loss
-    
-    def train(self, dataProvider: DataProvider):
-        """ Perform one training epoch
-        
-        Args:
-            dataProvider (DataProvider): data provider for training data
-
-        Returns:
-            dict: training results
-        """
-        # set model to training mode
-        self.model.train()
-
-        loss_sum = 0
-        pbar = qqdm(dataProvider, total=len(dataProvider), desc=format_str('bold', f"Epoch {self._epoch}: "))
-        for step, (data, target) in enumerate(pbar, start=1):
-            self.callbacks.on_batch_begin(step, logs=None, train=True)
-
-            data, target = self.toDevice(*toTorch(data, target))
-            loss = self.train_step(data, target)
-            loss_sum += loss.item()
-            loss_mean = loss_sum / step
-
-            # get training results of one step
-            logs = self.metrics.results(loss_mean, train=True)
-
-            # log learning rate into logs
-            if len(self.optimizer.param_groups) > 1:
-                lr_logs = {f"lr{i}": round(group["lr"], 6) for i, group in enumerate(self.optimizer.param_groups)}
-                logs.update(lr_logs)
-            else:
-                logs["lr"] = round(self.optimizer.param_groups[0]["lr"], 6)
-
-            # update progress bar description
-            pbar.set_description(desc=format_str('bold', f"Epoch {self._epoch}: "))
-            pbar.set_infos(logs)
-
-            self.callbacks.on_batch_end(step, logs=logs, train=True)
-
-        # reset metrics after each training epoch
-        self.metrics.reset()
-
-        # call on_epoch_end of data provider
-        dataProvider.on_epoch_end()
-
-        return logs
-
-    def test(self, dataProvider: DataProvider):
-        """ Perform one validation epoch
-
-        Args:
-            dataProvider (DataProvider): data provider for validation data
-
-        Returns:
-            dict: validation results
-        """
-        # set model to evaluation mode
-        self.model.eval()
-        loss_sum = 0
-        pbar = qqdm(dataProvider, total=len(dataProvider), desc=format_str('bold', 'Description'))
-        # disable autograd and gradient computation in PyTorch
-        with torch.no_grad():
-            for step, (data, target) in enumerate(pbar, start=1):
-                self.callbacks.on_batch_begin(step, logs=None, train=False)
-
-                data, target = self.toDevice(*toTorch(data, target))
-                loss = self.test_step(data, target)
-                loss_sum += loss.item()
-                loss_mean = loss_sum / step
-
-                # get testing results of one step
-                logs = self.metrics.results(loss_mean, train=False)
-
-                # update progress bar description
-                pbar.set_description(f"Epoch {self._epoch}: ")
-                pbar.set_infos(logs)
-
-                self.callbacks.on_batch_end(step, logs=logs, train=False)
-
-        # reset metrics after each test epoch
-        self.metrics.reset()
-
-        # call on_epoch_end of data provider
-        dataProvider.on_epoch_end()
-
-        return logs
-    
-    def save(self, path: str=None):
-        """ Save model state dict to file
-
-        Args:
-            path (str): path to file
-        """
-        if not path and not self.output_path:
-            print("Path to file is not provided, model will not be saved") # replace to error logging
-            return
-        
-        model_to_save = self.ema.ema if self.ema else self.model
-        
-        output_path = Path(path or self.output_path)
-        os.makedirs(output_path.parent, exist_ok=True)
-        model_to_save.eval()
-        try:
-            torch.save(model_to_save.state_dict(), output_path)
-            return str(output_path)
-        except Exception:
-            traceback.print_exc()
-            torch.save(model_to_save, output_path.with_suffix(".pth"))
-            return str(output_path.with_suffix(".pth"))
-    
-    def fit(
-        self, 
-        train_dataProvider: DataProvider, 
-        test_dataProvider: DataProvider=None, 
-        epochs: int=10, 
-        initial_epoch: int = 1, 
-        callbacks: typing.List[Callback] = []
-        ) -> dict:
-        """ Train model for a given number of epochs
-        
-        Args:
-            train_dataProvider (DataProvider): data provider for training data
-            test_dataProvider (DataProvider): data provider for validation data
-            epochs (int): number of epochs
-            initial_epoch (int, optional): initial epoch. Defaults to 1.
-            callbacks (typing.List[Callback], optional): list of callbacks. Defaults to [].
-
-        Returns:
-            dict: training results
-        """
-        self._epoch = initial_epoch
-        history = {}
-        self.callbacks = CallbacksHandler(self, callbacks)
-        self.callbacks.on_train_begin()
-        for epoch in range(initial_epoch, initial_epoch + epochs):
-            self.callbacks.on_epoch_begin(epoch)
-
-            train_logs = self.train(train_dataProvider)
-            val_logs = self.test(test_dataProvider) if test_dataProvider else {}
-
-            logs = {**train_logs, **val_logs}
-            self.callbacks.on_epoch_end(epoch, logs=logs)
-
-            if self.stop_training:
-                break
-
-            history[epoch] = logs
-            self._epoch += 1
-
-        self.callbacks.on_train_end(logs)
-
-        return history
-    
-    def evaluate(
-        self, 
-        dataProvider: DataProvider, 
-        initial_epoch: int = 1,
-        callbacks: typing.List[Callback] = [],
-        ) -> dict:
-        """ Evaluate model on validation data
-
-        Args:
-            dataProvider (DataProvider): data provider for validation data
-
-        Returns:
-            dict: validation results
-        """
-        self._epoch = initial_epoch
-        self.callbacks = CallbacksHandler(self, callbacks)
-        self.model.eval()
-        logs = self.test(dataProvider)
+import os
+import math
+import torch
+import typing
+import traceback
+import numpy as np
+from torch import nn
+from copy import deepcopy
+from qqdm import qqdm, format_str
+from pathlib import Path
+
+from .metrics import Metric
+from .callbacks import Callback
+from .dataProvider import DataProvider
+from .handlers import MetricsHandler, CallbacksHandler
+
+def toTorch(data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
+    """ Check if data is of type torch.Tensor, if not convert it to torch.Tensor
+
+    Args:
+        data (np.ndarray): data to be converted
+        target (np.ndarray): target to be converted
+
+    Returns:
+        typing.Tuple[torch.Tensor, torch.Tensor]: converted data and target
+    """
+    if not isinstance(data, torch.Tensor):
+        data = torch.from_numpy(data)
+
+    if not isinstance(target, (torch.Tensor, dict)):
+        target = torch.from_numpy(target)
+
+    if data.dtype != torch.float32:
+        data = data.float()
+
+    return data, target
+
+
+def is_parallel(model):
+    """Returns True if model is of type DP or DDP."""
+    return isinstance(model, (nn.parallel.DataParallel, nn.parallel.DistributedDataParallel))
+
+def de_parallel(model):
+    """De-parallelize a model: returns single-GPU model if model is of type DP or DDP."""
+    return model.module if is_parallel(model) else model
+
+def copy_attr(a, b, include=(), exclude=()):
+    """Copies attributes from object 'b' to object 'a', with options to include/exclude certain attributes."""
+    for k, v in b.__dict__.items():
+        if (len(include) and k not in include) or k.startswith("_") or k in exclude:
+            continue
+        else:
+            setattr(a, k, v)
+
+class ModelEMA:
+    """Updated Exponential Moving Average (EMA) from https://github.com/rwightman/pytorch-image-models
+    Keeps a moving average of everything in the model state_dict (parameters and buffers)
+    For EMA details see https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
+    To disable EMA set the `enabled` attribute to `False`.
+    """
+
+    def __init__(self, model, decay=0.9999, tau=2000, updates=0):
+        """Create EMA."""
+        self.ema = deepcopy(de_parallel(model)).eval()  # FP32 EMA
+        self.updates = updates  # number of EMA updates
+        self.decay = lambda x: decay * (1 - math.exp(-x / tau))  # decay exponential ramp (to help early epochs)
+        for p in self.ema.parameters():
+            p.requires_grad_(False)
+        self.enabled = True
+
+    def update(self, model):
+        """Update EMA parameters."""
+        if self.enabled:
+            self.updates += 1
+            d = self.decay(self.updates)
+
+            msd = de_parallel(model).state_dict()  # model state_dict
+            for k, v in self.ema.state_dict().items():
+                if v.dtype.is_floating_point:  # true for FP16 and FP32
+                    v *= d
+                    v += (1 - d) * msd[k].detach()
+                    # assert v.dtype == msd[k].dtype == torch.float32, f'{k}: EMA {v.dtype},  model {msd[k].dtype}'
+
+    def update_attr(self, model, include=(), exclude=("process_group", "reducer")):
+        """Updates attributes and saves stripped model with optimizer removed."""
+        if self.enabled:
+            copy_attr(self.ema, model, include, exclude)
+
+
+class Model:
+    """ Model class for training and testing PyTorch neural networks"""
+    def __init__(
+        self, 
+        model: torch.nn.Module, 
+        optimizer: torch.optim.Optimizer, 
+        loss: typing.Callable,
+        metrics: typing.List[Metric] = [],
+        mixed_precision: bool = False,
+        scaler = None,
+        log_errors: bool = True,
+        output_path: str = None,
+        clip_grad_norm: float = None,
+        ema = False,
+        ):
+        """ Initialize model class
+
+        Attributes:
+            model (torch.nn.Module): PyTorch neural network
+            optimizer (torch.optim.Optimizer): PyTorch optimizer
+            loss (typing.Callable): loss function
+            metrics (typing.List[Metric], optional): list of metrics. Defaults to [].
+            mixed_precision (bool, optional): whether to use mixed precision. Defaults to False.
+            scaler (torch.cuda.amp.GradScaler, optional): PyTorch GradScaler. Defaults to None.
+            log_errors (bool, optional): whether to log errors. Defaults to True.
+            output_path (str, optional): path to save model. Defaults to None.
+            clip_grad_norm (float, optional): gradient clipping value. Defaults to None.
+            ema (bool, optional): whether to use Exponential Moving Average. Defaults to False.
+        """
+        self.model = model
+        self.optimizer = optimizer
+        self.loss = loss
+        # get device on which model is running
+        self._device = next(self.model.parameters()).device
+
+        self.metrics = MetricsHandler(metrics)
+
+        self.mixed_precision = mixed_precision
+        self.scaler = torch.cuda.amp.GradScaler() if mixed_precision else scaler
+        self.log_errors = log_errors
+
+        self.output_path = Path(output_path) if output_path else None
+        if self.output_path:
+            if self.output_path.suffix == "":
+                self.output_path = Path(os.path.join(self.output_path, "model.pt"))
+            os.makedirs(self.output_path.parent, exist_ok=True)
+
+        self.stop_training = False
+        self.clip_grad_norm = clip_grad_norm
+        self.ema = ModelEMA(self.model) if ema else None
+
+        self.validate()
+
+    @property
+    def device(self):
+        return self._device
+
+    def validate(self):
+        """ Validate model, optimizer"""
+        if not isinstance(self.model, torch.nn.Module):
+            raise TypeError("model argument must be a torch.nn.Module")
+        
+        if not isinstance(self.optimizer, torch.optim.Optimizer):
+            raise TypeError("optimizer argument must be a torch.optim.Optimizer")
+        
+    def toDevice(self, data: np.ndarray, target: np.ndarray) -> typing.Tuple[torch.Tensor, torch.Tensor]:
+        """ Check if data is on the same device as model, if not move it to the device
+
+        Args:
+            data (np.ndarray): data to be moved
+            target (np.ndarray): target to be moved
+
+        Returns:
+            typing.Tuple[torch.Tensor, torch.Tensor]: moved data and target
+        """
+        try:
+            if data.device != self._device:
+                data = data.to(self._device)
+
+            if target.device != self._device:
+                target = target.to(self._device)
+        except AttributeError:
+            if self.log_errors:
+                print("Data and target must be of type torch.Tensor")
+
+        return data, target
+
+    def train_step(
+        self, 
+        data: typing.Union[np.ndarray, torch.Tensor], 
+        target: typing.Union[np.ndarray, torch.Tensor],
+        loss_info: dict = {}
+        ) -> torch.Tensor:
+        """ Perform one training step
+
+        Args:
+            data (typing.Union[np.ndarray, torch.Tensor]): training data
+            target (typing.Union[np.ndarray, torch.Tensor]): training target
+            loss_info (dict, optional): additional loss information. Defaults to {}.
+
+        Returns:
+            torch.Tensor: loss
+        """
+        self.optimizer.zero_grad()
+        if self.mixed_precision:
+            with torch.cuda.amp.autocast():
+                output = self.model(data)
+                loss = self.loss(output, target)
+                if isinstance(loss, tuple):
+                    loss, loss_info = loss[0], loss[1:]
+                self.scaler.scale(loss).backward()
+                if self.clip_grad_norm:
+                    torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=self.clip_grad_norm)
+                self.scaler.step(self.optimizer)
+                self.scaler.update()
+
+        else:
+            output = self.model(data)
+            loss = self.loss(output, target)
+            if isinstance(loss, tuple):
+                loss, loss_info = loss[0], loss[1:]
+            loss.backward()
+            if self.clip_grad_norm:
+                torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=self.clip_grad_norm)
+            self.optimizer.step()
+
+        if self.ema:
+            try:
+                self.ema.update(self.model)
+            except RuntimeError:
+                self.ema = ModelEMA(self.model)
+                self.ema.update(self.model)
+
+        if self._device.type == "cuda":
+            torch.cuda.synchronize() # synchronize after each forward and backward pass
+
+        self.metrics.update(target, output, model=self.model, loss_info=loss_info)
+
+        return loss
+    
+    def test_step(
+        self, 
+        data: typing.Union[np.ndarray, torch.Tensor], 
+        target: typing.Union[np.ndarray, torch.Tensor],
+        loss_info: dict = {}
+        ) -> torch.Tensor:
+        """ Perform one validation step
+
+        Args:
+            data (typing.Union[np.ndarray, torch.Tensor]): validation data
+            target (typing.Union[np.ndarray, torch.Tensor]): validation target
+            loss_info (dict, optional): additional loss information. Defaults to {}.
+
+        Returns:
+            torch.Tensor: loss
+        """
+        output = self.ema.ema(data) if self.ema else self.model(data)
+        loss = self.loss(output, target)
+        if isinstance(loss, tuple):
+            loss, loss_info = loss[0], loss[1:]
+
+        self.metrics.update(target, output, model=self.model, loss_info=loss_info)
+
+        # clear GPU memory cache after each validation step
+        torch.cuda.empty_cache()
+
+        return loss
+    
+    def train(self, dataProvider: DataProvider):
+        """ Perform one training epoch
+        
+        Args:
+            dataProvider (DataProvider): data provider for training data
+
+        Returns:
+            dict: training results
+        """
+        # set model to training mode
+        self.model.train()
+
+        loss_sum = 0
+        pbar = qqdm(dataProvider, total=len(dataProvider), desc=format_str('bold', f"Epoch {self._epoch}: "))
+        for step, (data, target) in enumerate(pbar, start=1):
+            self.callbacks.on_batch_begin(step, logs=None, train=True)
+
+            data, target = self.toDevice(*toTorch(data, target))
+            loss = self.train_step(data, target)
+            loss_sum += loss.item()
+            loss_mean = loss_sum / step
+
+            # get training results of one step
+            logs = self.metrics.results(loss_mean, train=True)
+
+            # log learning rate into logs
+            if len(self.optimizer.param_groups) > 1:
+                lr_logs = {f"lr{i}": round(group["lr"], 6) for i, group in enumerate(self.optimizer.param_groups)}
+                logs.update(lr_logs)
+            else:
+                logs["lr"] = round(self.optimizer.param_groups[0]["lr"], 6)
+
+            # update progress bar description
+            pbar.set_description(desc=format_str('bold', f"Epoch {self._epoch}: "))
+            pbar.set_infos(logs)
+
+            self.callbacks.on_batch_end(step, logs=logs, train=True)
+
+        # reset metrics after each training epoch
+        self.metrics.reset()
+
+        # call on_epoch_end of data provider
+        dataProvider.on_epoch_end()
+
+        return logs
+
+    def test(self, dataProvider: DataProvider):
+        """ Perform one validation epoch
+
+        Args:
+            dataProvider (DataProvider): data provider for validation data
+
+        Returns:
+            dict: validation results
+        """
+        # set model to evaluation mode
+        self.model.eval()
+        loss_sum = 0
+        pbar = qqdm(dataProvider, total=len(dataProvider), desc=format_str('bold', 'Description'))
+        # disable autograd and gradient computation in PyTorch
+        with torch.no_grad():
+            for step, (data, target) in enumerate(pbar, start=1):
+                self.callbacks.on_batch_begin(step, logs=None, train=False)
+
+                data, target = self.toDevice(*toTorch(data, target))
+                loss = self.test_step(data, target)
+                loss_sum += loss.item()
+                loss_mean = loss_sum / step
+
+                # get testing results of one step
+                logs = self.metrics.results(loss_mean, train=False)
+
+                # update progress bar description
+                pbar.set_description(f"Epoch {self._epoch}: ")
+                pbar.set_infos(logs)
+
+                self.callbacks.on_batch_end(step, logs=logs, train=False)
+
+        # reset metrics after each test epoch
+        self.metrics.reset()
+
+        # call on_epoch_end of data provider
+        dataProvider.on_epoch_end()
+
+        return logs
+    
+    def save(self, path: str=None):
+        """ Save model state dict to file
+
+        Args:
+            path (str): path to file
+        """
+        if not path and not self.output_path:
+            print("Path to file is not provided, model will not be saved") # replace to error logging
+            return
+        
+        model_to_save = self.ema.ema if self.ema else self.model
+        
+        output_path = Path(path or self.output_path)
+        os.makedirs(output_path.parent, exist_ok=True)
+        model_to_save.eval()
+        try:
+            torch.save(model_to_save.state_dict(), output_path)
+            return str(output_path)
+        except Exception:
+            traceback.print_exc()
+            torch.save(model_to_save, output_path.with_suffix(".pth"))
+            return str(output_path.with_suffix(".pth"))
+    
+    def fit(
+        self, 
+        train_dataProvider: DataProvider, 
+        test_dataProvider: DataProvider=None, 
+        epochs: int=10, 
+        initial_epoch: int = 1, 
+        callbacks: typing.List[Callback] = []
+        ) -> dict:
+        """ Train model for a given number of epochs
+        
+        Args:
+            train_dataProvider (DataProvider): data provider for training data
+            test_dataProvider (DataProvider): data provider for validation data
+            epochs (int): number of epochs
+            initial_epoch (int, optional): initial epoch. Defaults to 1.
+            callbacks (typing.List[Callback], optional): list of callbacks. Defaults to [].
+
+        Returns:
+            dict: training results
+        """
+        self._epoch = initial_epoch
+        history = {}
+        self.callbacks = CallbacksHandler(self, callbacks)
+        self.callbacks.on_train_begin()
+        for epoch in range(initial_epoch, initial_epoch + epochs):
+            self.callbacks.on_epoch_begin(epoch)
+
+            train_logs = self.train(train_dataProvider)
+            val_logs = self.test(test_dataProvider) if test_dataProvider else {}
+
+            logs = {**train_logs, **val_logs}
+            self.callbacks.on_epoch_end(epoch, logs=logs)
+
+            if self.stop_training:
+                break
+
+            history[epoch] = logs
+            self._epoch += 1
+
+        self.callbacks.on_train_end(logs)
+
+        return history
+    
+    def evaluate(
+        self, 
+        dataProvider: DataProvider, 
+        initial_epoch: int = 1,
+        callbacks: typing.List[Callback] = [],
+        ) -> dict:
+        """ Evaluate model on validation data
+
+        Args:
+            dataProvider (DataProvider): data provider for validation data
+
+        Returns:
+            dict: validation results
+        """
+        self._epoch = initial_epoch
+        self.callbacks = CallbacksHandler(self, callbacks)
+        self.model.eval()
+        logs = self.test(dataProvider)
         return logs
```

### Comparing `mltu-1.2.4/mltu/torch/yolo/annotation.py` & `mltu-1.2.5/mltu/torch/yolo/annotation.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import os
-import typing
-from pathlib import Path
-import xml.etree.ElementTree as ET
-from mltu.annotations.detections import Detections, Detection, BboxType
-
-class VOCAnnotationReader:
-    """Reads annotations from VOC format
-    """
-    def __init__(self, labels: dict, images_path: str=None):
-        self.labels = labels
-        self.images_path = images_path
-        self.dataset_found_labels = {}
-
-    @staticmethod
-    def readFromVOC(voc_annotation_path: str, labels: dict={}, images_path: str=None) -> Detections:
-        annotation_path = Path(voc_annotation_path)
-        tree = ET.parse(voc_annotation_path)
-        root = tree.getroot()
-
-        annotation_dict = {}
-
-        # Iterate through child elements
-        for child in root:
-            if child.tag == 'object':
-                obj_dict = {}
-                for obj_child in child:
-                    if obj_child.tag == 'bndbox':
-                        bbox_dict = {}
-                        for bbox_child in obj_child:
-                            bbox_dict[bbox_child.tag] = int(bbox_child.text)
-                        obj_dict[obj_child.tag] = bbox_dict
-                    else:
-                        obj_dict[obj_child.tag] = obj_child.text
-                if 'objects' not in annotation_dict:
-                    annotation_dict['objects'] = []
-                annotation_dict['objects'].append(obj_dict)
-            elif child.tag == 'size':
-                size_dict = {}
-                for size_child in child:
-                    size_dict[size_child.tag] = int(size_child.text)
-                annotation_dict['size'] = size_dict
-            else:
-                annotation_dict[child.tag] = child.text
-
-        # Get the image path if not provided
-        if images_path is None:
-            images_path = annotation_path.parent.parent / annotation_dict["folder"]
-
-        image_path = os.path.join(images_path, annotation_dict['filename'])
-        dets = []
-        for obj in annotation_dict['objects']:
-            if labels and obj['name'] not in labels.values():
-                print(f"Label {obj['name']} not found in labels")
-                continue
-
-            dets.append(Detection(
-                bbox=[obj['bndbox']['xmin'], obj['bndbox']['ymin'], obj['bndbox']['xmax'], obj['bndbox']['ymax']],
-                label=obj['name'],
-                bbox_type=BboxType.XYXY,
-                confidence=1,
-                image_path=image_path,
-                width=annotation_dict['size']['width'],
-                height=annotation_dict['size']['height'],
-                relative=False
-                ))
-        
-        detections = Detections(
-            labels=labels,
-            width=annotation_dict['size']['width'],
-            height=annotation_dict['size']['height'],
-            image_path=image_path,
-            detections=dets
-        )
-
-        return detections
-    
-    def __call__(self, image: typing.Any, annotation: str) -> typing.Tuple[typing.Any, Detections]:
-        detections = self.readFromVOC(annotation, self.labels, self.images_path)
-        if image is None:
-            image = detections.image_path
+import os
+import typing
+from pathlib import Path
+import xml.etree.ElementTree as ET
+from mltu.annotations.detections import Detections, Detection, BboxType
+
+class VOCAnnotationReader:
+    """Reads annotations from VOC format
+    """
+    def __init__(self, labels: dict, images_path: str=None):
+        self.labels = labels
+        self.images_path = images_path
+        self.dataset_found_labels = {}
+
+    @staticmethod
+    def readFromVOC(voc_annotation_path: str, labels: dict={}, images_path: str=None) -> Detections:
+        annotation_path = Path(voc_annotation_path)
+        tree = ET.parse(voc_annotation_path)
+        root = tree.getroot()
+
+        annotation_dict = {}
+
+        # Iterate through child elements
+        for child in root:
+            if child.tag == 'object':
+                obj_dict = {}
+                for obj_child in child:
+                    if obj_child.tag == 'bndbox':
+                        bbox_dict = {}
+                        for bbox_child in obj_child:
+                            bbox_dict[bbox_child.tag] = int(bbox_child.text)
+                        obj_dict[obj_child.tag] = bbox_dict
+                    else:
+                        obj_dict[obj_child.tag] = obj_child.text
+                if 'objects' not in annotation_dict:
+                    annotation_dict['objects'] = []
+                annotation_dict['objects'].append(obj_dict)
+            elif child.tag == 'size':
+                size_dict = {}
+                for size_child in child:
+                    size_dict[size_child.tag] = int(size_child.text)
+                annotation_dict['size'] = size_dict
+            else:
+                annotation_dict[child.tag] = child.text
+
+        # Get the image path if not provided
+        if images_path is None:
+            images_path = annotation_path.parent.parent / annotation_dict["folder"]
+
+        image_path = os.path.join(images_path, annotation_dict['filename'])
+        dets = []
+        for obj in annotation_dict['objects']:
+            if labels and obj['name'] not in labels.values():
+                print(f"Label {obj['name']} not found in labels")
+                continue
+
+            dets.append(Detection(
+                bbox=[obj['bndbox']['xmin'], obj['bndbox']['ymin'], obj['bndbox']['xmax'], obj['bndbox']['ymax']],
+                label=obj['name'],
+                bbox_type=BboxType.XYXY,
+                confidence=1,
+                image_path=image_path,
+                width=annotation_dict['size']['width'],
+                height=annotation_dict['size']['height'],
+                relative=False
+                ))
+        
+        detections = Detections(
+            labels=labels,
+            width=annotation_dict['size']['width'],
+            height=annotation_dict['size']['height'],
+            image_path=image_path,
+            detections=dets
+        )
+
+        return detections
+    
+    def __call__(self, image: typing.Any, annotation: str) -> typing.Tuple[typing.Any, Detections]:
+        detections = self.readFromVOC(annotation, self.labels, self.images_path)
+        if image is None:
+            image = detections.image_path
         return image, detections
```

### Comparing `mltu-1.2.4/mltu/torch/yolo/detectors/onnx_detector.py` & `mltu-1.2.5/mltu/torch/yolo/detectors/onnx_detector.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import numpy as np
-from mltu.inferenceModel import OnnxInferenceModel
-from mltu.torch.yolo.detectors.detector import BaseDetector
-from mltu.annotations.detections import BboxType, Detection, Detections
-
-class Detector(OnnxInferenceModel, BaseDetector):
-    """ YOLOv8 detector using onnxruntime"""
-    def __init__(
-            self, 
-            model_path: str,
-            input_width: int, 
-            input_height: int, 
-            confidence_threshold: float=0.5, 
-            iou_threshold: float=0.5, 
-            classes: dict = None, 
-            return_raw_output: bool=False,
-            *args, **kwargs
-        ):
-        """
-        Args:
-            model_path (str): Path to the model file
-            input_width (int): Input width to use for the model
-            input_height (int): Input height to use for the model
-            confidence_threshold (float, optional): Confidence threshold for filtering the predictions. Defaults to 0.5.
-            iou_threshold (float, optional): Intersection over union threshold for filtering the predictions. Defaults to 0.5.
-            classes (dict, optional): Dictionary of class names. Defaults to None.
-            return_raw_output (bool, optional): Return raw output of the model (return bounding boxes, scores, and class ids). Defaults to False.
-        """
-        super().__init__(model_path, *args, **kwargs)
-        self.input_width = input_width
-        self.input_height = input_height
-        self.confidence_threshold = confidence_threshold
-        self.iou_threshold = iou_threshold
-        self.return_raw_output = return_raw_output
-
-        self.classes = classes or self.metadata.get("classes", None)
-        if self.classes is None:
-            raise ValueError("The classes must be provided")
-        
-        # Generate a color palette for the classes
-        self.color_palette = np.random.uniform(0, 255, size=(len(self.classes), 3))
-
-    def predict(self, image: np.ndarray, **kwargs) -> Detections:
-        img_height, img_width, _ = image.shape
-
-        # Preprocess the image
-        preprocessed_image = self.preprocess(image, self.input_height, self.input_width)
-        
-        # Perform inference on the preprocessed image
-        preds = self.model.run(self.output_names, {self.input_names[0]: preprocessed_image})
-
-        # Extract the results from the predictions
-        results = preds[0][0]
-
-        # Calculate the scaling factors for the bounding box coordinates
-        x_factor, y_factor = img_width / self.input_width, img_height / self.input_height
-
-        # Perform postprocessing on the predictions
-        boxes, scores, class_ids = self.postprocess(results, x_factor, y_factor, self.confidence_threshold, self.iou_threshold)
-
-        if self.return_raw_output:
-            return boxes, scores, class_ids
-
-        detections = []
-        for bbox, conf, class_id in zip(boxes, scores, class_ids):
-            detection = Detection(
-                bbox = bbox,
-                label = self.classes[class_id],
-                labels = self.classes,
-                bbox_type=BboxType.XYWH,
-                confidence=conf,
-                relative=False,
-                width=img_width,
-                height=img_height
-            )
-            detections.append(detection)
-
-        return Detections(
-            labels=self.classes,
-            width=img_width, 
-            height=img_height, 
-            detections=detections, 
-            color_palette=self.color_palette,
+import numpy as np
+from mltu.inferenceModel import OnnxInferenceModel
+from mltu.torch.yolo.detectors.detector import BaseDetector
+from mltu.annotations.detections import BboxType, Detection, Detections
+
+class Detector(OnnxInferenceModel, BaseDetector):
+    """ YOLOv8 detector using onnxruntime"""
+    def __init__(
+            self, 
+            model_path: str,
+            input_width: int, 
+            input_height: int, 
+            confidence_threshold: float=0.5, 
+            iou_threshold: float=0.5, 
+            classes: dict = None, 
+            return_raw_output: bool=False,
+            *args, **kwargs
+        ):
+        """
+        Args:
+            model_path (str): Path to the model file
+            input_width (int): Input width to use for the model
+            input_height (int): Input height to use for the model
+            confidence_threshold (float, optional): Confidence threshold for filtering the predictions. Defaults to 0.5.
+            iou_threshold (float, optional): Intersection over union threshold for filtering the predictions. Defaults to 0.5.
+            classes (dict, optional): Dictionary of class names. Defaults to None.
+            return_raw_output (bool, optional): Return raw output of the model (return bounding boxes, scores, and class ids). Defaults to False.
+        """
+        super().__init__(model_path, *args, **kwargs)
+        self.input_width = input_width
+        self.input_height = input_height
+        self.confidence_threshold = confidence_threshold
+        self.iou_threshold = iou_threshold
+        self.return_raw_output = return_raw_output
+
+        self.classes = classes or self.metadata.get("classes", None)
+        if self.classes is None:
+            raise ValueError("The classes must be provided")
+        
+        # Generate a color palette for the classes
+        self.color_palette = np.random.uniform(0, 255, size=(len(self.classes), 3))
+
+    def predict(self, image: np.ndarray, **kwargs) -> Detections:
+        img_height, img_width, _ = image.shape
+
+        # Preprocess the image
+        preprocessed_image = self.preprocess(image, self.input_height, self.input_width)
+        
+        # Perform inference on the preprocessed image
+        preds = self.model.run(self.output_names, {self.input_names[0]: preprocessed_image})
+
+        # Extract the results from the predictions
+        results = preds[0][0]
+
+        # Calculate the scaling factors for the bounding box coordinates
+        x_factor, y_factor = img_width / self.input_width, img_height / self.input_height
+
+        # Perform postprocessing on the predictions
+        boxes, scores, class_ids = self.postprocess(results, x_factor, y_factor, self.confidence_threshold, self.iou_threshold)
+
+        if self.return_raw_output:
+            return boxes, scores, class_ids
+
+        detections = []
+        for bbox, conf, class_id in zip(boxes, scores, class_ids):
+            detection = Detection(
+                bbox = bbox,
+                label = self.classes[class_id],
+                labels = self.classes,
+                bbox_type=BboxType.XYWH,
+                confidence=conf,
+                relative=False,
+                width=img_width,
+                height=img_height
+            )
+            detections.append(detection)
+
+        return Detections(
+            labels=self.classes,
+            width=img_width, 
+            height=img_height, 
+            detections=detections, 
+            color_palette=self.color_palette,
         )
```

### Comparing `mltu-1.2.4/mltu/torch/yolo/loss.py` & `mltu-1.2.5/mltu/torch/yolo/loss.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import torch
-from torch import nn
-
-from ultralytics.utils.loss import BboxLoss, xywh2xyxy
-from ultralytics.utils.tal import TaskAlignedAssigner, dist2bbox, make_anchors
-
-class v8DetectionLoss:
-    """Criterion class for computing training losses."""
-
-    def __init__(self, model, box: float=7.5, cls: float=0.5, dfl: float=1.5):  # model must be de-paralleled
-        """Initializes v8DetectionLoss with the model, defining model-related properties and BCE loss function."""
-        self.model = model
-        device = next(model.parameters()).device  # get model device
-
-        self.head = model.model[-1]  # Detect() module
-        self.bce = nn.BCEWithLogitsLoss(reduction="none")
-        self.stride = self.head.stride  # model strides
-        self.nc = self.head.nc  # number of classes
-        self.no = self.head.no
-        self.reg_max = self.head.reg_max # max number of regression targets
-        self.device = device
-
-        self.use_dfl = self.head.reg_max > 1
-
-        self.assigner = TaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
-        self.bbox_loss = BboxLoss(self.head.reg_max - 1, use_dfl=self.use_dfl).to(device)
-        self.proj = torch.arange(self.head.reg_max, dtype=torch.float, device=device).to(device)
-
-        self.box = box # box gain
-        self.cls = cls # cls gain
-        self.dfl = dfl # dfl gain
-
-    def preprocess(self, targets, batch_size, scale_tensor):
-        """Preprocesses the target counts and matches with the input batch size to output a tensor."""
-        if targets.shape[0] == 0:
-            out = torch.zeros(batch_size, 0, 5, device=self.device)
-        else:
-            i = targets[:, 0]  # image index
-            _, counts = i.unique(return_counts=True)
-            counts = counts.to(dtype=torch.int32)
-            out = torch.zeros(batch_size, counts.max(), 5, device=self.device)
-            for j in range(batch_size):
-                matches = i == j
-                n = matches.sum()
-                if n:
-                    out[j, :n] = targets[matches, 1:]
-            out[..., 1:5] = xywh2xyxy(out[..., 1:5].mul_(scale_tensor))
-        return out
-
-    def bbox_decode(self, anchor_points, pred_dist):
-        """Decode predicted object bounding box coordinates from anchor points and distribution."""
-        if self.use_dfl:
-            b, a, c = pred_dist.shape  # batch, anchors, channels
-            self.proj = self.proj.to(pred_dist.device)
-            pred_dist = pred_dist.view(b, a, 4, c // 4).softmax(3).matmul(self.proj.type(pred_dist.dtype))
-
-        return dist2bbox(pred_dist, anchor_points, xywh=False)
-
-    def __call__(self, preds, batch):
-        """Calculate the sum of the loss for box, cls and dfl multiplied by batch size."""
-        loss = torch.zeros(3, device=self.device)  # box, cls, dfl
-        feats = preds[1] if isinstance(preds, tuple) else preds
-        pred_distri, pred_scores = torch.cat([xi.view(feats[0].shape[0], self.no, -1) for xi in feats], 2).split(
-            (self.reg_max * 4, self.nc), 1
-        )
-
-        pred_scores = pred_scores.permute(0, 2, 1).contiguous()
-        pred_distri = pred_distri.permute(0, 2, 1).contiguous()
-
-        dtype = pred_scores.dtype
-        batch_size = pred_scores.shape[0]
-        imgsz = torch.tensor(feats[0].shape[2:], device=self.device, dtype=dtype) * self.stride[0]  # image size (h,w)
-        anchor_points, stride_tensor = make_anchors(feats, self.stride, 0.5)
-
-        # Targets
-        targets = torch.cat((batch["batch_idx"].view(-1, 1), batch["cls"].view(-1, 1), batch["bboxes"]), 1)
-        targets = self.preprocess(targets.to(self.device), batch_size, scale_tensor=imgsz[[1, 0, 1, 0]])
-        gt_labels, gt_bboxes = targets.split((1, 4), 2)  # cls, xyxy
-        mask_gt = gt_bboxes.sum(2, keepdim=True).gt_(0)
-
-        # Pboxes
-        pred_bboxes = self.bbox_decode(anchor_points, pred_distri)  # xyxy, (b, h*w, 4)
-
-        _, target_bboxes, target_scores, fg_mask, _ = self.assigner(
-            pred_scores.detach().sigmoid(),
-            (pred_bboxes.detach() * stride_tensor).type(gt_bboxes.dtype),
-            anchor_points * stride_tensor,
-            gt_labels,
-            gt_bboxes,
-            mask_gt,
-        )
-
-        target_scores_sum = max(target_scores.sum(), 1)
-
-        # Cls loss
-        loss[1] = self.bce(pred_scores, target_scores.to(dtype)).sum() / target_scores_sum  # BCE
-
-        # Bbox loss
-        if fg_mask.sum():
-            target_bboxes /= stride_tensor
-            loss[0], loss[2] = self.bbox_loss(
-                pred_distri, pred_bboxes, anchor_points, target_bboxes, target_scores, target_scores_sum, fg_mask
-            )
-
-        loss[0] *= self.box  # box gain
-        loss[1] *= self.cls  # cls gain
-        loss[2] *= self.dfl  # dfl gain
-
-        detailed_loss = {"box_loss": loss[0].detach(), "cls_loss": loss[1].detach(), "dfl_loss": loss[2].detach()}
-
+import torch
+from torch import nn
+
+from ultralytics.utils.loss import BboxLoss, xywh2xyxy
+from ultralytics.utils.tal import TaskAlignedAssigner, dist2bbox, make_anchors
+
+class v8DetectionLoss:
+    """Criterion class for computing training losses."""
+
+    def __init__(self, model, box: float=7.5, cls: float=0.5, dfl: float=1.5):  # model must be de-paralleled
+        """Initializes v8DetectionLoss with the model, defining model-related properties and BCE loss function."""
+        self.model = model
+        device = next(model.parameters()).device  # get model device
+
+        self.head = model.model[-1]  # Detect() module
+        self.bce = nn.BCEWithLogitsLoss(reduction="none")
+        self.stride = self.head.stride  # model strides
+        self.nc = self.head.nc  # number of classes
+        self.no = self.head.no
+        self.reg_max = self.head.reg_max # max number of regression targets
+        self.device = device
+
+        self.use_dfl = self.head.reg_max > 1
+
+        self.assigner = TaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
+        self.bbox_loss = BboxLoss(self.head.reg_max - 1, use_dfl=self.use_dfl).to(device)
+        self.proj = torch.arange(self.head.reg_max, dtype=torch.float, device=device).to(device)
+
+        self.box = box # box gain
+        self.cls = cls # cls gain
+        self.dfl = dfl # dfl gain
+
+    def preprocess(self, targets, batch_size, scale_tensor):
+        """Preprocesses the target counts and matches with the input batch size to output a tensor."""
+        if targets.shape[0] == 0:
+            out = torch.zeros(batch_size, 0, 5, device=self.device)
+        else:
+            i = targets[:, 0]  # image index
+            _, counts = i.unique(return_counts=True)
+            counts = counts.to(dtype=torch.int32)
+            out = torch.zeros(batch_size, counts.max(), 5, device=self.device)
+            for j in range(batch_size):
+                matches = i == j
+                n = matches.sum()
+                if n:
+                    out[j, :n] = targets[matches, 1:]
+            out[..., 1:5] = xywh2xyxy(out[..., 1:5].mul_(scale_tensor))
+        return out
+
+    def bbox_decode(self, anchor_points, pred_dist):
+        """Decode predicted object bounding box coordinates from anchor points and distribution."""
+        if self.use_dfl:
+            b, a, c = pred_dist.shape  # batch, anchors, channels
+            self.proj = self.proj.to(pred_dist.device)
+            pred_dist = pred_dist.view(b, a, 4, c // 4).softmax(3).matmul(self.proj.type(pred_dist.dtype))
+
+        return dist2bbox(pred_dist, anchor_points, xywh=False)
+
+    def __call__(self, preds, batch):
+        """Calculate the sum of the loss for box, cls and dfl multiplied by batch size."""
+        loss = torch.zeros(3, device=self.device)  # box, cls, dfl
+        feats = preds[1] if isinstance(preds, tuple) else preds
+        pred_distri, pred_scores = torch.cat([xi.view(feats[0].shape[0], self.no, -1) for xi in feats], 2).split(
+            (self.reg_max * 4, self.nc), 1
+        )
+
+        pred_scores = pred_scores.permute(0, 2, 1).contiguous()
+        pred_distri = pred_distri.permute(0, 2, 1).contiguous()
+
+        dtype = pred_scores.dtype
+        batch_size = pred_scores.shape[0]
+        imgsz = torch.tensor(feats[0].shape[2:], device=self.device, dtype=dtype) * self.stride[0]  # image size (h,w)
+        anchor_points, stride_tensor = make_anchors(feats, self.stride, 0.5)
+
+        # Targets
+        targets = torch.cat((batch["batch_idx"].view(-1, 1), batch["cls"].view(-1, 1), batch["bboxes"]), 1)
+        targets = self.preprocess(targets.to(self.device), batch_size, scale_tensor=imgsz[[1, 0, 1, 0]])
+        gt_labels, gt_bboxes = targets.split((1, 4), 2)  # cls, xyxy
+        mask_gt = gt_bboxes.sum(2, keepdim=True).gt_(0)
+
+        # Pboxes
+        pred_bboxes = self.bbox_decode(anchor_points, pred_distri)  # xyxy, (b, h*w, 4)
+
+        _, target_bboxes, target_scores, fg_mask, _ = self.assigner(
+            pred_scores.detach().sigmoid(),
+            (pred_bboxes.detach() * stride_tensor).type(gt_bboxes.dtype),
+            anchor_points * stride_tensor,
+            gt_labels,
+            gt_bboxes,
+            mask_gt,
+        )
+
+        target_scores_sum = max(target_scores.sum(), 1)
+
+        # Cls loss
+        loss[1] = self.bce(pred_scores, target_scores.to(dtype)).sum() / target_scores_sum  # BCE
+
+        # Bbox loss
+        if fg_mask.sum():
+            target_bboxes /= stride_tensor
+            loss[0], loss[2] = self.bbox_loss(
+                pred_distri, pred_bboxes, anchor_points, target_bboxes, target_scores, target_scores_sum, fg_mask
+            )
+
+        loss[0] *= self.box  # box gain
+        loss[1] *= self.cls  # cls gain
+        loss[2] *= self.dfl  # dfl gain
+
+        detailed_loss = {"box_loss": loss[0].detach(), "cls_loss": loss[1].detach(), "dfl_loss": loss[2].detach()}
+
         return loss.sum() * batch_size, detailed_loss  # loss(box, cls, dfl)
```

### Comparing `mltu-1.2.4/mltu/torch/yolo/metrics.py` & `mltu-1.2.5/mltu/torch/yolo/metrics.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-from mltu.torch.metrics import Metric
-
-import torch
-import numpy as np
-from ultralytics.utils import ops
-from ultralytics.utils.metrics import ap_per_class
-from ultralytics.utils.metrics import Metric as YoloMetric
-from ultralytics.utils.metrics import ConfusionMatrix, box_iou
-
-
-class YoloMetrics(Metric):
-    """ Accuracy metric class
-    
-    Args:
-        name (str, optional): name of metric. Defaults to 'YoloMetrics'.
-    """
-    def __init__(self, nc, name: str="YoloMetrics", conf:float=0.001, iou:float=0.7, max_det:int=300) -> None:
-        super(YoloMetrics, self).__init__(name=name)
-        self.nc = nc
-        self.jdict = []
-        self.confusion_matrix = ConfusionMatrix(nc=nc, conf=conf)
-        self.stats = dict(tp=[], conf=[], pred_cls=[], target_cls=[])
-
-        self.conf = conf
-        self.iou = iou
-        self.lb = []
-        self.multi_label=True
-        self.single_cls=False
-        self.max_det = max_det
-        self.seen = 0
-        self.device = torch.device("cpu")
-        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
-        self.niou = self.iouv.numel()
-        self.box = YoloMetric()
-        self.loss_info = {"box_loss": [], "cls_loss": [], "dfl_loss": []}
-
-    @property
-    def keys(self):
-        return ["precision", "recall", "mAP50", "mAP50-95", "fitness"]
-
-    def reset(self):
-        self.__init__(self.nc, self.name)
-
-    def match_predictions(self, pred_classes, true_classes, iou, use_scipy=False):
-        """
-        Matches predictions to ground truth objects (pred_classes, true_classes) using IoU.
-
-        Args:
-            pred_classes (torch.Tensor): Predicted class indices of shape(N,).
-            true_classes (torch.Tensor): Target class indices of shape(M,).
-            iou (torch.Tensor): An NxM tensor containing the pairwise IoU values for predictions and ground of truth
-            use_scipy (bool): Whether to use scipy for matching (more precise).
-
-        Returns:
-            (torch.Tensor): Correct tensor of shape(N,10) for 10 IoU thresholds.
-        """
-        # Dx10 matrix, where D - detections, 10 - IoU thresholds
-        correct = np.zeros((pred_classes.shape[0], self.iouv.shape[0])).astype(bool)
-        # LxD matrix where L - labels (rows), D - detections (columns)
-        correct_class = true_classes[:, None] == pred_classes
-        iou = iou * correct_class  # zero out the wrong classes
-        iou = iou.cpu().numpy()
-        for i, threshold in enumerate(self.iouv.cpu().tolist()):
-            if use_scipy:
-                # WARNING: known issue that reduces mAP in https://github.com/ultralytics/ultralytics/pull/4708
-                import scipy  # scope import to avoid importing for all commands
-
-                cost_matrix = iou * (iou >= threshold)
-                if cost_matrix.any():
-                    labels_idx, detections_idx = scipy.optimize.linear_sum_assignment(cost_matrix, maximize=True)
-                    valid = cost_matrix[labels_idx, detections_idx] > 0
-                    if valid.any():
-                        correct[detections_idx[valid], i] = True
-            else:
-                matches = np.nonzero(iou >= threshold)  # IoU > threshold and classes match
-                matches = np.array(matches).T
-                if matches.shape[0]:
-                    if matches.shape[0] > 1:
-                        matches = matches[iou[matches[:, 0], matches[:, 1]].argsort()[::-1]]
-                        matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
-                        matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
-                    correct[matches[:, 1].astype(int), i] = True
-        return torch.tensor(correct, dtype=torch.bool, device=pred_classes.device)
-
-    def _process_batch(self, detections, gt_bboxes, gt_cls):
-        """
-        Return correct prediction matrix.
-
-        Args:
-            detections (torch.Tensor): Tensor of shape [N, 6] representing detections.
-                Each detection is of the format: x1, y1, x2, y2, conf, class.
-            labels (torch.Tensor): Tensor of shape [M, 5] representing labels.
-                Each label is of the format: class, x1, y1, x2, y2.
-
-        Returns:
-            (torch.Tensor): Correct prediction matrix of shape [N, 10] for 10 IoU levels.
-        """
-        iou = box_iou(gt_bboxes, detections[:, :4])
-        return self.match_predictions(detections[:, 5], gt_cls, iou)
-
-    def _prepare_batch(self, si, batch):
-        """Prepares a batch of images and annotations for validation."""
-        idx = batch["batch_idx"] == si
-        cls = batch["cls"][idx].squeeze(-1).to(self.device)
-        bbox = batch["bboxes"][idx].to(self.device)
-        ori_shape = batch["ori_shape"][si]
-        # imgsz = batch["img"].shape[2:]
-        imgsz = batch["resized_shape"][si]
-        ratio_pad = (batch["resized_shape"][si][0] / batch["ori_shape"][si][0], batch["resized_shape"][si][1] / batch["ori_shape"][si][1])
-        if len(cls):
-            bbox = ops.xywh2xyxy(bbox) * torch.tensor(imgsz, device=self.device)[[1, 0, 1, 0]]  # target boxes
-        return dict(cls=cls, bbox=bbox, ori_shape=ori_shape, imgsz=imgsz, ratio_pad=ratio_pad)
-
-    def update_stats(self, preds, batch):
-        """Metrics."""
-        for si, pred in enumerate(preds):
-            self.seen += 1
-            npr = len(pred)
-            stat = dict(
-                conf=torch.zeros(0, device=self.device),
-                pred_cls=torch.zeros(0, device=self.device),
-                tp=torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device),
-            )
-            pbatch = self._prepare_batch(si, batch)
-            cls, bbox = pbatch.pop("cls"), pbatch.pop("bbox")
-            nl = len(cls)
-            stat["target_cls"] = cls
-            if npr == 0:
-                if nl:
-                    for k in self.stats.keys():
-                        self.stats[k].append(stat[k])
-                continue
-
-            # Predictions
-            if self.single_cls:
-                pred[:, 5] = 0
-            predn = pred.clone().to(self.device)
-            stat["conf"] = predn[:, 4]
-            stat["pred_cls"] = predn[:, 5]
-
-            # Evaluate
-            if nl:
-                stat["tp"] = self._process_batch(predn, bbox, cls)
-            for k in self.stats.keys():
-                self.stats[k].append(stat[k])
-
-    def postprocess(self, preds):
-        """Apply Non-maximum suppression to prediction outputs."""
-        return ops.non_max_suppression(
-            preds,
-            self.conf,
-            self.iou,
-            labels=self.lb,
-            multi_label=self.multi_label,
-            agnostic=self.single_cls,
-            max_det=self.max_det,
-        )
-
-    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs):
-        """ Update metric state with new data
-
-        Args:
-            output (torch.Tensor): output of model
-            target (torch.Tensor): target of data
-        """
-        # outputs = np.squeeze(output)
-        model = kwargs.get("model")
-        loss_info = kwargs.get("loss_info", None)
-        if loss_info:
-            for k, v in loss_info[0].items():
-                self.loss_info[k].append(v.cpu().numpy())
-
-        if not model.training: # update metrics only in validation mode
-            preds = self.postprocess(output[0])
-            self.update_stats(preds, target)
-
-    def result(self) -> dict:
-        """ Return metric value"""
-        stats = {k: torch.cat(v, 0).cpu().numpy() for k, v in self.stats.items() if v}
-        loss_info_stats = {k: np.mean(v) for k, v in self.loss_info.items()}
-        if not stats:
-            if loss_info_stats:
-                return loss_info_stats
-            return None
-        
-        # Compute statistics
-        ap_per_class_results = ap_per_class(
-            stats["tp"],
-            stats["conf"],
-            stats["pred_cls"],
-            stats["target_cls"],
-            plot=False,
-            names={},
-        )[2:]
-        self.box.nc = self.nc
-        self.box.update(ap_per_class_results)
-
-        results = dict(zip(self.keys, self.box.mean_results() + [self.box.fitness()]))
-        if loss_info_stats:
-            results.update(loss_info_stats)
-
+from mltu.torch.metrics import Metric
+
+import torch
+import numpy as np
+from ultralytics.utils import ops
+from ultralytics.utils.metrics import ap_per_class
+from ultralytics.utils.metrics import Metric as YoloMetric
+from ultralytics.utils.metrics import ConfusionMatrix, box_iou
+
+
+class YoloMetrics(Metric):
+    """ Accuracy metric class
+    
+    Args:
+        name (str, optional): name of metric. Defaults to 'YoloMetrics'.
+    """
+    def __init__(self, nc, name: str="YoloMetrics", conf:float=0.001, iou:float=0.7, max_det:int=300) -> None:
+        super(YoloMetrics, self).__init__(name=name)
+        self.nc = nc
+        self.jdict = []
+        self.confusion_matrix = ConfusionMatrix(nc=nc, conf=conf)
+        self.stats = dict(tp=[], conf=[], pred_cls=[], target_cls=[])
+
+        self.conf = conf
+        self.iou = iou
+        self.lb = []
+        self.multi_label=True
+        self.single_cls=False
+        self.max_det = max_det
+        self.seen = 0
+        self.device = torch.device("cpu")
+        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
+        self.niou = self.iouv.numel()
+        self.box = YoloMetric()
+        self.loss_info = {"box_loss": [], "cls_loss": [], "dfl_loss": []}
+
+    @property
+    def keys(self):
+        return ["precision", "recall", "mAP50", "mAP50-95", "fitness"]
+
+    def reset(self):
+        self.__init__(self.nc, self.name)
+
+    def match_predictions(self, pred_classes, true_classes, iou, use_scipy=False):
+        """
+        Matches predictions to ground truth objects (pred_classes, true_classes) using IoU.
+
+        Args:
+            pred_classes (torch.Tensor): Predicted class indices of shape(N,).
+            true_classes (torch.Tensor): Target class indices of shape(M,).
+            iou (torch.Tensor): An NxM tensor containing the pairwise IoU values for predictions and ground of truth
+            use_scipy (bool): Whether to use scipy for matching (more precise).
+
+        Returns:
+            (torch.Tensor): Correct tensor of shape(N,10) for 10 IoU thresholds.
+        """
+        # Dx10 matrix, where D - detections, 10 - IoU thresholds
+        correct = np.zeros((pred_classes.shape[0], self.iouv.shape[0])).astype(bool)
+        # LxD matrix where L - labels (rows), D - detections (columns)
+        correct_class = true_classes[:, None] == pred_classes
+        iou = iou * correct_class  # zero out the wrong classes
+        iou = iou.cpu().numpy()
+        for i, threshold in enumerate(self.iouv.cpu().tolist()):
+            if use_scipy:
+                # WARNING: known issue that reduces mAP in https://github.com/ultralytics/ultralytics/pull/4708
+                import scipy  # scope import to avoid importing for all commands
+
+                cost_matrix = iou * (iou >= threshold)
+                if cost_matrix.any():
+                    labels_idx, detections_idx = scipy.optimize.linear_sum_assignment(cost_matrix, maximize=True)
+                    valid = cost_matrix[labels_idx, detections_idx] > 0
+                    if valid.any():
+                        correct[detections_idx[valid], i] = True
+            else:
+                matches = np.nonzero(iou >= threshold)  # IoU > threshold and classes match
+                matches = np.array(matches).T
+                if matches.shape[0]:
+                    if matches.shape[0] > 1:
+                        matches = matches[iou[matches[:, 0], matches[:, 1]].argsort()[::-1]]
+                        matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
+                        matches = matches[np.unique(matches[:, 0], return_index=True)[1]]
+                    correct[matches[:, 1].astype(int), i] = True
+        return torch.tensor(correct, dtype=torch.bool, device=pred_classes.device)
+
+    def _process_batch(self, detections, gt_bboxes, gt_cls):
+        """
+        Return correct prediction matrix.
+
+        Args:
+            detections (torch.Tensor): Tensor of shape [N, 6] representing detections.
+                Each detection is of the format: x1, y1, x2, y2, conf, class.
+            labels (torch.Tensor): Tensor of shape [M, 5] representing labels.
+                Each label is of the format: class, x1, y1, x2, y2.
+
+        Returns:
+            (torch.Tensor): Correct prediction matrix of shape [N, 10] for 10 IoU levels.
+        """
+        iou = box_iou(gt_bboxes, detections[:, :4])
+        return self.match_predictions(detections[:, 5], gt_cls, iou)
+
+    def _prepare_batch(self, si, batch):
+        """Prepares a batch of images and annotations for validation."""
+        idx = batch["batch_idx"] == si
+        cls = batch["cls"][idx].squeeze(-1).to(self.device)
+        bbox = batch["bboxes"][idx].to(self.device)
+        ori_shape = batch["ori_shape"][si]
+        # imgsz = batch["img"].shape[2:]
+        imgsz = batch["resized_shape"][si]
+        ratio_pad = (batch["resized_shape"][si][0] / batch["ori_shape"][si][0], batch["resized_shape"][si][1] / batch["ori_shape"][si][1])
+        if len(cls):
+            bbox = ops.xywh2xyxy(bbox) * torch.tensor(imgsz, device=self.device)[[1, 0, 1, 0]]  # target boxes
+        return dict(cls=cls, bbox=bbox, ori_shape=ori_shape, imgsz=imgsz, ratio_pad=ratio_pad)
+
+    def update_stats(self, preds, batch):
+        """Metrics."""
+        for si, pred in enumerate(preds):
+            self.seen += 1
+            npr = len(pred)
+            stat = dict(
+                conf=torch.zeros(0, device=self.device),
+                pred_cls=torch.zeros(0, device=self.device),
+                tp=torch.zeros(npr, self.niou, dtype=torch.bool, device=self.device),
+            )
+            pbatch = self._prepare_batch(si, batch)
+            cls, bbox = pbatch.pop("cls"), pbatch.pop("bbox")
+            nl = len(cls)
+            stat["target_cls"] = cls
+            if npr == 0:
+                if nl:
+                    for k in self.stats.keys():
+                        self.stats[k].append(stat[k])
+                continue
+
+            # Predictions
+            if self.single_cls:
+                pred[:, 5] = 0
+            predn = pred.clone().to(self.device)
+            stat["conf"] = predn[:, 4]
+            stat["pred_cls"] = predn[:, 5]
+
+            # Evaluate
+            if nl:
+                stat["tp"] = self._process_batch(predn, bbox, cls)
+            for k in self.stats.keys():
+                self.stats[k].append(stat[k])
+
+    def postprocess(self, preds):
+        """Apply Non-maximum suppression to prediction outputs."""
+        return ops.non_max_suppression(
+            preds,
+            self.conf,
+            self.iou,
+            labels=self.lb,
+            multi_label=self.multi_label,
+            agnostic=self.single_cls,
+            max_det=self.max_det,
+        )
+
+    def update(self, output: torch.Tensor, target: torch.Tensor, **kwargs):
+        """ Update metric state with new data
+
+        Args:
+            output (torch.Tensor): output of model
+            target (torch.Tensor): target of data
+        """
+        # outputs = np.squeeze(output)
+        model = kwargs.get("model")
+        loss_info = kwargs.get("loss_info", None)
+        if loss_info:
+            for k, v in loss_info[0].items():
+                self.loss_info[k].append(v.cpu().numpy())
+
+        if not model.training: # update metrics only in validation mode
+            preds = self.postprocess(output[0])
+            self.update_stats(preds, target)
+
+    def result(self) -> dict:
+        """ Return metric value"""
+        stats = {k: torch.cat(v, 0).cpu().numpy() for k, v in self.stats.items() if v}
+        loss_info_stats = {k: np.mean(v) for k, v in self.loss_info.items()}
+        if not stats:
+            if loss_info_stats:
+                return loss_info_stats
+            return None
+        
+        # Compute statistics
+        ap_per_class_results = ap_per_class(
+            stats["tp"],
+            stats["conf"],
+            stats["pred_cls"],
+            stats["target_cls"],
+            plot=False,
+            names={},
+        )[2:]
+        self.box.nc = self.nc
+        self.box.update(ap_per_class_results)
+
+        results = dict(zip(self.keys, self.box.mean_results() + [self.box.fitness()]))
+        if loss_info_stats:
+            results.update(loss_info_stats)
+
         return results
```

### Comparing `mltu-1.2.4/mltu/torch/yolo/optimizer.py` & `mltu-1.2.5/mltu/torch/yolo/optimizer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import torch
-from torch import nn
-
-class AccumulativeOptimizer(torch.optim.Optimizer):
-    def __init__(self, optimizer, batch_size, nbs=64):
-        super(AccumulativeOptimizer, self).__init__(optimizer.param_groups, optimizer.defaults)
-        self.optimizer = optimizer
-        self.accumulation_steps = int(nbs / batch_size)
-        self.current_step = 0
-
-    def zero_grad(self):
-        if self.current_step == 0:
-            self.optimizer.zero_grad()
-
-    def step(self):
-        self.current_step += 1
-        if self.current_step >= self.accumulation_steps:
-            self.optimizer.step()
-            self.current_step = 0
-            self.optimizer.zero_grad()
-
-
-def build_optimizer(model, name: str="AdamW", lr: float=1e-3, weight_decay: float=0.0, momentum: float=0.937, decay=0.0005):
-
-    pg0, pg1, pg2 = [], [], []  # optimizer parameter groups
-    bn = tuple(v for k, v in nn.__dict__.items() if "Norm" in k)  # normalization layers, i.e. BatchNorm2d()
-    for module_name, module in model.named_modules():
-        for param_name, param in module.named_parameters(recurse=False):
-            fullname = f"{module_name}.{param_name}" if module_name else param_name
-            if "bias" in fullname:  # bias (no decay)
-                pg2.append(param)
-            elif isinstance(module, bn):  # weight (no decay)
-                pg1.append(param)
-            else:  # weight (with decay)
-                pg0.append(param)
-
-    if name == "AdamW":
-        optimizer = torch.optim.AdamW(pg2, lr=lr, weight_decay=weight_decay, betas=(momentum, 0.999))
-    elif name == "Adam":
-        optimizer = torch.optim.Adam(pg2, lr=lr, weight_decay=weight_decay, betas=(momentum, 0.999))
-    elif name == "SGD":
-        optimizer = torch.optim.SGD(pg2, lr=lr, weight_decay=weight_decay, momentum=0.9)
-    else:
-        raise ValueError(f"Optimizer {name} not supported!")
-    
-    optimizer.add_param_group({'params': pg0, 'weight_decay': decay})  # add pg1 with weight_decay
-    optimizer.add_param_group({'params': pg1, 'weight_decay': 0.0})  # add pg2 (biases)
-
-    del pg0, pg1, pg2
-
+import torch
+from torch import nn
+
+class AccumulativeOptimizer(torch.optim.Optimizer):
+    def __init__(self, optimizer, batch_size, nbs=64):
+        super(AccumulativeOptimizer, self).__init__(optimizer.param_groups, optimizer.defaults)
+        self.optimizer = optimizer
+        self.accumulation_steps = int(nbs / batch_size)
+        self.current_step = 0
+
+    def zero_grad(self):
+        if self.current_step == 0:
+            self.optimizer.zero_grad()
+
+    def step(self):
+        self.current_step += 1
+        if self.current_step >= self.accumulation_steps:
+            self.optimizer.step()
+            self.current_step = 0
+            self.optimizer.zero_grad()
+
+
+def build_optimizer(model, name: str="AdamW", lr: float=1e-3, weight_decay: float=0.0, momentum: float=0.937, decay=0.0005):
+
+    pg0, pg1, pg2 = [], [], []  # optimizer parameter groups
+    bn = tuple(v for k, v in nn.__dict__.items() if "Norm" in k)  # normalization layers, i.e. BatchNorm2d()
+    for module_name, module in model.named_modules():
+        for param_name, param in module.named_parameters(recurse=False):
+            fullname = f"{module_name}.{param_name}" if module_name else param_name
+            if "bias" in fullname:  # bias (no decay)
+                pg2.append(param)
+            elif isinstance(module, bn):  # weight (no decay)
+                pg1.append(param)
+            else:  # weight (with decay)
+                pg0.append(param)
+
+    if name == "AdamW":
+        optimizer = torch.optim.AdamW(pg2, lr=lr, weight_decay=weight_decay, betas=(momentum, 0.999))
+    elif name == "Adam":
+        optimizer = torch.optim.Adam(pg2, lr=lr, weight_decay=weight_decay, betas=(momentum, 0.999))
+    elif name == "SGD":
+        optimizer = torch.optim.SGD(pg2, lr=lr, weight_decay=weight_decay, momentum=0.9)
+    else:
+        raise ValueError(f"Optimizer {name} not supported!")
+    
+    optimizer.add_param_group({'params': pg0, 'weight_decay': decay})  # add pg1 with weight_decay
+    optimizer.add_param_group({'params': pg1, 'weight_decay': 0.0})  # add pg2 (biases)
+
+    del pg0, pg1, pg2
+
     return optimizer
```

### Comparing `mltu-1.2.4/mltu/torch/yolo/pruning_utils.py` & `mltu-1.2.5/mltu/torch/yolo/pruning_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import torch
-from torch import nn
-from ultralytics.nn.modules import C2f, Conv, Bottleneck
-
-def infer_shortcut(bottleneck):
-    c1 = bottleneck.cv1.conv.in_channels
-    c2 = bottleneck.cv2.conv.out_channels
-    return c1 == c2 and hasattr(bottleneck, 'add') and bottleneck.add
-
-class C2f_v2(nn.Module):
-    # CSP Bottleneck with 2 convolutions
-    def __init__(self, c1, c2, n=1, shortcut=False, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
-        super().__init__()
-        self.c = int(c2 * e)  # hidden channels
-        self.cv0 = Conv(c1, self.c, 1, 1)
-        self.cv1 = Conv(c1, self.c, 1, 1)
-        self.cv2 = Conv((2 + n) * self.c, c2, 1)  # optional act=FReLU(c2)
-        self.m = nn.ModuleList(Bottleneck(self.c, self.c, shortcut, g, k=((3, 3), (3, 3)), e=1.0) for _ in range(n))
-
-    def forward(self, x):
-        # y = list(self.cv1(x).chunk(2, 1))
-        y = [self.cv0(x), self.cv1(x)]
-        y.extend(m(y[-1]) for m in self.m)
-        return self.cv2(torch.cat(y, 1))
-
-def transfer_weights(c2f, c2f_v2):
-    c2f_v2.cv2 = c2f.cv2
-    c2f_v2.m = c2f.m
-
-    state_dict = c2f.state_dict()
-    state_dict_v2 = c2f_v2.state_dict()
-
-    # Transfer cv1 weights from C2f to cv0 and cv1 in C2f_v2
-    old_weight = state_dict['cv1.conv.weight']
-    half_channels = old_weight.shape[0] // 2
-    state_dict_v2['cv0.conv.weight'] = old_weight[:half_channels]
-    state_dict_v2['cv1.conv.weight'] = old_weight[half_channels:]
-
-    # Transfer cv1 batchnorm weights and buffers from C2f to cv0 and cv1 in C2f_v2
-    for bn_key in ['weight', 'bias', 'running_mean', 'running_var']:
-        old_bn = state_dict[f'cv1.bn.{bn_key}']
-        state_dict_v2[f'cv0.bn.{bn_key}'] = old_bn[:half_channels]
-        state_dict_v2[f'cv1.bn.{bn_key}'] = old_bn[half_channels:]
-
-    # Transfer remaining weights and buffers
-    for key in state_dict:
-        if not key.startswith('cv1.'):
-            state_dict_v2[key] = state_dict[key]
-
-    # Transfer all non-method attributes
-    for attr_name in dir(c2f):
-        attr_value = getattr(c2f, attr_name)
-        if not callable(attr_value) and '_' not in attr_name:
-            setattr(c2f_v2, attr_name, attr_value)
-
-    c2f_v2.load_state_dict(state_dict_v2)
-
-def replace_c2f_with_c2f_v2(module):
-    for name, child_module in module.named_children():
-        if isinstance(child_module, C2f):
-            # Replace C2f with C2f_v2 while preserving its parameters
-            shortcut = infer_shortcut(child_module.m[0])
-            c2f_v2 = C2f_v2(child_module.cv1.conv.in_channels, child_module.cv2.conv.out_channels,
-                            n=len(child_module.m), shortcut=shortcut,
-                            g=child_module.m[0].cv2.conv.groups,
-                            e=child_module.c / child_module.cv2.conv.out_channels)
-            transfer_weights(child_module, c2f_v2)
-            setattr(module, name, c2f_v2)
-        else:
+import torch
+from torch import nn
+from ultralytics.nn.modules import C2f, Conv, Bottleneck
+
+def infer_shortcut(bottleneck):
+    c1 = bottleneck.cv1.conv.in_channels
+    c2 = bottleneck.cv2.conv.out_channels
+    return c1 == c2 and hasattr(bottleneck, 'add') and bottleneck.add
+
+class C2f_v2(nn.Module):
+    # CSP Bottleneck with 2 convolutions
+    def __init__(self, c1, c2, n=1, shortcut=False, g=1, e=0.5):  # ch_in, ch_out, number, shortcut, groups, expansion
+        super().__init__()
+        self.c = int(c2 * e)  # hidden channels
+        self.cv0 = Conv(c1, self.c, 1, 1)
+        self.cv1 = Conv(c1, self.c, 1, 1)
+        self.cv2 = Conv((2 + n) * self.c, c2, 1)  # optional act=FReLU(c2)
+        self.m = nn.ModuleList(Bottleneck(self.c, self.c, shortcut, g, k=((3, 3), (3, 3)), e=1.0) for _ in range(n))
+
+    def forward(self, x):
+        # y = list(self.cv1(x).chunk(2, 1))
+        y = [self.cv0(x), self.cv1(x)]
+        y.extend(m(y[-1]) for m in self.m)
+        return self.cv2(torch.cat(y, 1))
+
+def transfer_weights(c2f, c2f_v2):
+    c2f_v2.cv2 = c2f.cv2
+    c2f_v2.m = c2f.m
+
+    state_dict = c2f.state_dict()
+    state_dict_v2 = c2f_v2.state_dict()
+
+    # Transfer cv1 weights from C2f to cv0 and cv1 in C2f_v2
+    old_weight = state_dict['cv1.conv.weight']
+    half_channels = old_weight.shape[0] // 2
+    state_dict_v2['cv0.conv.weight'] = old_weight[:half_channels]
+    state_dict_v2['cv1.conv.weight'] = old_weight[half_channels:]
+
+    # Transfer cv1 batchnorm weights and buffers from C2f to cv0 and cv1 in C2f_v2
+    for bn_key in ['weight', 'bias', 'running_mean', 'running_var']:
+        old_bn = state_dict[f'cv1.bn.{bn_key}']
+        state_dict_v2[f'cv0.bn.{bn_key}'] = old_bn[:half_channels]
+        state_dict_v2[f'cv1.bn.{bn_key}'] = old_bn[half_channels:]
+
+    # Transfer remaining weights and buffers
+    for key in state_dict:
+        if not key.startswith('cv1.'):
+            state_dict_v2[key] = state_dict[key]
+
+    # Transfer all non-method attributes
+    for attr_name in dir(c2f):
+        attr_value = getattr(c2f, attr_name)
+        if not callable(attr_value) and '_' not in attr_name:
+            setattr(c2f_v2, attr_name, attr_value)
+
+    c2f_v2.load_state_dict(state_dict_v2)
+
+def replace_c2f_with_c2f_v2(module):
+    for name, child_module in module.named_children():
+        if isinstance(child_module, C2f):
+            # Replace C2f with C2f_v2 while preserving its parameters
+            shortcut = infer_shortcut(child_module.m[0])
+            c2f_v2 = C2f_v2(child_module.cv1.conv.in_channels, child_module.cv2.conv.out_channels,
+                            n=len(child_module.m), shortcut=shortcut,
+                            g=child_module.m[0].cv2.conv.groups,
+                            e=child_module.c / child_module.cv2.conv.out_channels)
+            transfer_weights(child_module, c2f_v2)
+            setattr(module, name, c2f_v2)
+        else:
             replace_c2f_with_c2f_v2(child_module)
```

### Comparing `mltu-1.2.4/mltu/transformers.py` & `mltu-1.2.5/mltu/transformers.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,402 +1,402 @@
-import cv2
-import time
-import queue
-import typing
-import logging
-import threading
-import importlib
-import numpy as np
-
-from . import Image
-from mltu.annotations.audio import Audio
-from mltu.annotations.detections import Detections
-
-""" Implemented Transformers:
-- ExpandDims - Expand dimension of data
-- ImageResizer - Resize image to (width, height)
-- LabelIndexer - Convert label to index by vocab
-- LabelPadding - Pad label to max_word_length
-- ImageNormalizer - Normalize image to float value, transpose axis if necessary and convert to numpy
-- SpectrogramPadding - Pad spectrogram to max_spectrogram_length
-- AudioToSpectrogram - Convert Audio to Spectrogram
-- ImageShowCV2 - Show image for visual inspection
-"""
-
-class Transformer:
-    def __init__(self, log_level: int = logging.INFO) -> None:
-        self._log_level = log_level
-
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(logging.INFO)
-
-    def __call__(self, data: typing.Any, label: typing.Any, *args, **kwargs):
-        raise NotImplementedError
-
-
-class ExpandDims(Transformer):
-    def __init__(self, axis: int=-1):
-        self.axis = axis
-
-    def __call__(self, data: np.ndarray, label: np.ndarray):
-        return np.expand_dims(data, self.axis), label
-
-class ImageResizer(Transformer):
-    """Resize image to (width, height)
-    
-    Attributes:
-        width (int): Width of image
-        height (int): Height of image
-        keep_aspect_ratio (bool): Whether to keep aspect ratio of image
-        padding_color (typing.Tuple[int]): Color to pad image
-    """
-    def __init__(
-        self, 
-        width: int, 
-        height: int, 
-        keep_aspect_ratio: bool=False, 
-        padding_color: typing.Tuple[int]=(0, 0, 0)
-        ) -> None:
-        self._width = width
-        self._height = height
-        self._keep_aspect_ratio = keep_aspect_ratio
-        self._padding_color = padding_color
-
-    @staticmethod
-    def unpad_maintaining_aspect_ratio(padded_image: np.ndarray, original_width: int, original_height: int) -> np.ndarray:
-        height, width = padded_image.shape[:2]
-        ratio = min(width / original_width, height / original_height)
-
-        delta_w = width - int(original_width * ratio)
-        delta_h = height - int(original_height * ratio)
-        left, right = delta_w//2, delta_w-(delta_w//2)
-        top, bottom = delta_h//2, delta_h-(delta_h//2)
-        unpaded_image = padded_image[top:height-bottom, left:width-right]
-
-        original_image = cv2.resize(unpaded_image, (original_width, original_height))
-
-        return original_image
-
-    @staticmethod
-    def resize_maintaining_aspect_ratio(image: np.ndarray, width_target: int, height_target: int, padding_color: typing.Tuple[int]=(0, 0, 0)) -> np.ndarray:
-        """ Resize image maintaining aspect ratio and pad with padding_color.
-
-        Args:
-            image (np.ndarray): Image to resize
-            width_target (int): Target width
-            height_target (int): Target height
-            padding_color (typing.Tuple[int]): Color to pad image
-
-        Returns:
-            np.ndarray: Resized image
-        """
-        height, width = image.shape[:2]
-        ratio = min(width_target / width, height_target / height)
-        new_w, new_h = int(width * ratio), int(height * ratio)
-
-        resized_image = cv2.resize(image, (new_w, new_h))
-        delta_w = width_target - new_w
-        delta_h = height_target - new_h
-        top, bottom = delta_h//2, delta_h-(delta_h//2)
-        left, right = delta_w//2, delta_w-(delta_w//2)
-
-        new_image = cv2.copyMakeBorder(resized_image, top, bottom, left, right, cv2.BORDER_CONSTANT, value=padding_color)
-
-        return new_image
-
-    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        if not isinstance(image, Image):
-            raise TypeError(f"Expected image to be of type Image, got {type(image)}")
-
-        # Maintains aspect ratio and resizes with padding.
-        if self._keep_aspect_ratio:
-            image_numpy = self.resize_maintaining_aspect_ratio(image.numpy(), self._width, self._height, self._padding_color)
-            if isinstance(label, Image):
-                label_numpy = self.resize_maintaining_aspect_ratio(label.numpy(), self._width, self._height, self._padding_color)
-                label.update(label_numpy)
-        else:   
-            # Resizes without maintaining aspect ratio.
-            image_numpy = cv2.resize(image.numpy(), (self._width, self._height))
-            if isinstance(label, Image):
-                label_numpy = cv2.resize(label.numpy(), (self._width, self._height))
-                label.update(label_numpy)
-
-        image.update(image_numpy)
-
-        return image, label
-
-class LabelIndexer(Transformer):
-    """Convert label to index by vocab
-    
-    Attributes:
-        vocab (typing.List[str]): List of characters in vocab
-    """
-    def __init__(
-        self, 
-        vocab: typing.List[str]
-        ) -> None:
-        self.vocab = vocab
-
-    def __call__(self, data: np.ndarray, label: np.ndarray):
-        return data, np.array([self.vocab.index(l) for l in label if l in self.vocab])
-
-class LabelPadding(Transformer):
-    """Pad label to max_word_length
-    
-    Attributes:
-        padding_value (int): Value to pad
-        max_word_length (int): Maximum length of label
-        use_on_batch (bool): Whether to use on batch. Default: False
-    """
-    def __init__(
-        self, 
-        padding_value: int,
-        max_word_length: int = None, 
-        use_on_batch: bool = False
-        ) -> None:
-        self.max_word_length = max_word_length
-        self.padding_value = padding_value
-        self.use_on_batch = use_on_batch
-
-        if not use_on_batch and max_word_length is None:
-            raise ValueError("max_word_length must be specified if use_on_batch is False")
-
-    def __call__(self, data: np.ndarray, label: np.ndarray):
-        if self.use_on_batch:
-            max_len = max([len(a) for a in label])
-            padded_labels = []
-            for l in label:
-                padded_label = np.pad(l, (0, max_len - len(l)), "constant", constant_values=self.padding_value)
-                padded_labels.append(padded_label)
-
-            padded_labels = np.array(padded_labels)
-            return data, padded_labels
-
-        label = label[:self.max_word_length]
-        return data, np.pad(label, (0, self.max_word_length - len(label)), "constant", constant_values=self.padding_value)
-
-
-class ImageNormalizer:
-    """ Normalize image to float value, transpose axis if necessary and convert to numpy
-    """
-    def __init__(self, transpose_axis: bool=False):
-        """ Initialize ImageNormalizer
-
-        Args:
-            transpose_axis (bool): Whether to transpose axis. Default: False
-        """
-        self.transpose_axis = transpose_axis
-    
-    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[np.ndarray, typing.Any]:
-        """ Convert each Image to numpy, transpose axis ant normalize to float value
-        """
-        img = image.numpy() / 255.0
-
-        if self.transpose_axis:
-            img = img.transpose(2, 0, 1)
-        
-        return img, annotation
-
-
-class SpectrogramPadding(Transformer):
-    """Pad spectrogram to max_spectrogram_length
-    
-    Attributes:
-        padding_value (int): Value to pad
-        max_spectrogram_length (int): Maximum length of spectrogram. Must be specified if use_on_batch is False. Default: None
-        use_on_batch (bool): Whether to use on batch. Default: False
-    """
-    def __init__(
-        self, 
-        padding_value: int,
-        max_spectrogram_length: int = None, 
-        use_on_batch: bool = False
-        ) -> None:
-        self.max_spectrogram_length = max_spectrogram_length
-        self.padding_value = padding_value
-        self.use_on_batch = use_on_batch
-
-        if not use_on_batch and max_spectrogram_length is None:
-            raise ValueError("max_spectrogram_length must be specified if use_on_batch is False")
-
-    def __call__(self, spectrogram: np.ndarray, label: np.ndarray):
-        if self.use_on_batch:
-            max_len = max([len(a) for a in spectrogram])
-            padded_spectrograms = []
-            for spec in spectrogram:
-                padded_spectrogram = np.pad(spec, ((0, max_len - spec.shape[0]), (0,0)), mode="constant", constant_values=self.padding_value)
-                padded_spectrograms.append(padded_spectrogram)
-
-            padded_spectrograms = np.array(padded_spectrograms)
-            label = np.array(label)
-
-            return padded_spectrograms, label
-
-        padded_spectrogram = np.pad(spectrogram, ((0, self.max_spectrogram_length - spectrogram.shape[0]),(0,0)), mode="constant", constant_values=self.padding_value)
-
-        return padded_spectrogram, label
-
-
-class AudioPadding(Transformer):
-    def __init__(self, max_audio_length: int, padding_value: int = 0, use_on_batch: bool = False, limit: bool = False):
-        super(AudioPadding, self).__init__()
-        self.max_audio_length = max_audio_length
-        self.padding_value = padding_value
-        self.use_on_batch = use_on_batch
-        self.limit = limit
-
-    def __call__(self, audio: Audio, label: typing.Any):
-        # batched padding
-        if self.use_on_batch:
-            max_len = max([len(a) for a in audio])
-            padded_audios = []
-            for a in audio:
-                # limit audio if it exceed max_audio_length
-                padded_audio = np.pad(a, (0, max_len - a.shape[0]), mode="constant", constant_values=self.padding_value)
-                padded_audios.append(padded_audio)
-
-            padded_audios = np.array(padded_audios)
-            # limit audio if it exceed max_audio_length
-            if self.limit:
-                padded_audios = padded_audios[:, :self.max_audio_length]
-
-            return padded_audios, label
-
-        audio_numpy = audio.numpy()
-        # limit audio if it exceed max_audio_length
-        if self.limit:
-            audio_numpy = audio_numpy[:self.max_audio_length]
-        padded_audio = np.pad(audio_numpy, (0, self.max_audio_length - audio_numpy.shape[0]), mode="constant", constant_values=self.padding_value)
-
-        audio.audio = padded_audio
-
-        return audio, label
-
-class AudioToSpectrogram(Transformer):
-    """Read wav file with librosa and return audio and label
-    
-    Attributes:
-        frame_length (int): Length of the frames in samples.
-        frame_step (int): Step size between frames in samples.
-        fft_length (int): Number of FFT components.
-        log_level (int): Logging level (default: logging.INFO)
-    """
-    def __init__(
-            self,
-            frame_length: int = 256,
-            frame_step: int = 160,
-            fft_length: int = 384,
-            log_level: int = logging.INFO,
-        ) -> None:
-        super(AudioToSpectrogram, self).__init__(log_level=log_level)
-        self.frame_length = frame_length
-        self.frame_step = frame_step
-        self.fft_length = fft_length
-
-        # import librosa using importlib
-        try:
-            self.librosa = importlib.import_module('librosa')
-            print("librosa version:", self.librosa.__version__)
-        except ImportError:
-            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
-
-    def __call__(self, audio: Audio, label: typing.Any):
-        """Compute the spectrogram of a WAV file
-
-        Args:
-            audio (Audio): Audio object
-            label (Any): Label of audio
-
-        Returns:
-            np.ndarray: Spectrogram of audio
-            label (Any): Label of audio
-        """
-
-        # Compute the Short Time Fourier Transform (STFT) of the audio data and store it in the variable 'spectrogram'
-        # The STFT is computed with a hop length of 'frame_step' samples, a window length of 'frame_length' samples, and 'fft_length' FFT components.
-        # The resulting spectrogram is also transposed for convenience
-        spectrogram = self.librosa.stft(audio.numpy(), hop_length=self.frame_step, win_length=self.frame_length, n_fft=self.fft_length).T
-
-        # Take the absolute value of the spectrogram to obtain the magnitude spectrum
-        spectrogram = np.abs(spectrogram)
-
-        # Take the square root of the magnitude spectrum to obtain the log spectrogram
-        spectrogram = np.power(spectrogram, 0.5)
-
-        # Normalize the spectrogram by subtracting the mean and dividing by the standard deviation.
-        # A small value of 1e-10 is added to the denominator to prevent division by zero.
-        spectrogram = (spectrogram - np.mean(spectrogram)) / (np.std(spectrogram) + 1e-10)
-
-        return spectrogram, label
-
-
-class ImageShowCV2(Transformer):
-    """Show image for visual inspection
-    """
-    def __init__(
-        self, 
-        verbose: bool = True,
-        log_level: int = logging.INFO,
-        name: str = "Image"
-        ) -> None:
-        """
-        Args:
-            verbose (bool): Whether to log label
-            log_level (int): Logging level (default: logging.INFO)
-            name (str): Name of window to show image
-        """
-        super(ImageShowCV2, self).__init__(log_level=log_level)
-        self.verbose = verbose
-        self.name = name
-        self.thread_started = False
-
-    def init_thread(self):
-        if not self.thread_started:
-            self.thread_started = True
-            self.image_queue = queue.Queue()
-
-            # Start a new thread to display the images, so that the main loop could run in multiple threads
-            self.thread = threading.Thread(target=self._display_images)
-            self.thread.start()
-
-    def _display_images(self) -> None:
-        """ Display images in a continuous loop """
-        while True:
-            image, label = self.image_queue.get()
-            if isinstance(label, Image):
-                cv2.imshow(self.name + "Label", label.numpy())
-            cv2.imshow(self.name, image.numpy())
-            cv2.waitKey(0)
-            cv2.destroyAllWindows()
-
-    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
-        """ Show image for visual inspection
-
-        Args:
-            data (np.ndarray): Image data
-            label (np.ndarray): Label data
-        
-        Returns:
-            data (np.ndarray): Image data
-            label (np.ndarray): Label data (unchanged)
-        """
-        # Start cv2 image display thread
-        self.init_thread()
-
-        if self.verbose:
-            if isinstance(label, (str, int, float)):
-                self.logger.info(f"Label: {label}")
-
-        if isinstance(label, Detections):
-            for detection in label:
-                img = detection.applyToFrame(np.asarray(image.numpy()))
-                image.update(img)
-
-        # Add image to display queue
-        # Sleep if queue is not empty
-        while not self.image_queue.empty():
-            time.sleep(0.5)
-
-        # Add image to display queue
-        self.image_queue.put((image, label))
-
+import cv2
+import time
+import queue
+import typing
+import logging
+import threading
+import importlib
+import numpy as np
+
+from . import Image
+from mltu.annotations.audio import Audio
+from mltu.annotations.detections import Detections
+
+""" Implemented Transformers:
+- ExpandDims - Expand dimension of data
+- ImageResizer - Resize image to (width, height)
+- LabelIndexer - Convert label to index by vocab
+- LabelPadding - Pad label to max_word_length
+- ImageNormalizer - Normalize image to float value, transpose axis if necessary and convert to numpy
+- SpectrogramPadding - Pad spectrogram to max_spectrogram_length
+- AudioToSpectrogram - Convert Audio to Spectrogram
+- ImageShowCV2 - Show image for visual inspection
+"""
+
+class Transformer:
+    def __init__(self, log_level: int = logging.INFO) -> None:
+        self._log_level = log_level
+
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger.setLevel(logging.INFO)
+
+    def __call__(self, data: typing.Any, label: typing.Any, *args, **kwargs):
+        raise NotImplementedError
+
+
+class ExpandDims(Transformer):
+    def __init__(self, axis: int=-1):
+        self.axis = axis
+
+    def __call__(self, data: np.ndarray, label: np.ndarray):
+        return np.expand_dims(data, self.axis), label
+
+class ImageResizer(Transformer):
+    """Resize image to (width, height)
+    
+    Attributes:
+        width (int): Width of image
+        height (int): Height of image
+        keep_aspect_ratio (bool): Whether to keep aspect ratio of image
+        padding_color (typing.Tuple[int]): Color to pad image
+    """
+    def __init__(
+        self, 
+        width: int, 
+        height: int, 
+        keep_aspect_ratio: bool=False, 
+        padding_color: typing.Tuple[int]=(0, 0, 0)
+        ) -> None:
+        self._width = width
+        self._height = height
+        self._keep_aspect_ratio = keep_aspect_ratio
+        self._padding_color = padding_color
+
+    @staticmethod
+    def unpad_maintaining_aspect_ratio(padded_image: np.ndarray, original_width: int, original_height: int) -> np.ndarray:
+        height, width = padded_image.shape[:2]
+        ratio = min(width / original_width, height / original_height)
+
+        delta_w = width - int(original_width * ratio)
+        delta_h = height - int(original_height * ratio)
+        left, right = delta_w//2, delta_w-(delta_w//2)
+        top, bottom = delta_h//2, delta_h-(delta_h//2)
+        unpaded_image = padded_image[top:height-bottom, left:width-right]
+
+        original_image = cv2.resize(unpaded_image, (original_width, original_height))
+
+        return original_image
+
+    @staticmethod
+    def resize_maintaining_aspect_ratio(image: np.ndarray, width_target: int, height_target: int, padding_color: typing.Tuple[int]=(0, 0, 0)) -> np.ndarray:
+        """ Resize image maintaining aspect ratio and pad with padding_color.
+
+        Args:
+            image (np.ndarray): Image to resize
+            width_target (int): Target width
+            height_target (int): Target height
+            padding_color (typing.Tuple[int]): Color to pad image
+
+        Returns:
+            np.ndarray: Resized image
+        """
+        height, width = image.shape[:2]
+        ratio = min(width_target / width, height_target / height)
+        new_w, new_h = int(width * ratio), int(height * ratio)
+
+        resized_image = cv2.resize(image, (new_w, new_h))
+        delta_w = width_target - new_w
+        delta_h = height_target - new_h
+        top, bottom = delta_h//2, delta_h-(delta_h//2)
+        left, right = delta_w//2, delta_w-(delta_w//2)
+
+        new_image = cv2.copyMakeBorder(resized_image, top, bottom, left, right, cv2.BORDER_CONSTANT, value=padding_color)
+
+        return new_image
+
+    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        if not isinstance(image, Image):
+            raise TypeError(f"Expected image to be of type Image, got {type(image)}")
+
+        # Maintains aspect ratio and resizes with padding.
+        if self._keep_aspect_ratio:
+            image_numpy = self.resize_maintaining_aspect_ratio(image.numpy(), self._width, self._height, self._padding_color)
+            if isinstance(label, Image):
+                label_numpy = self.resize_maintaining_aspect_ratio(label.numpy(), self._width, self._height, self._padding_color)
+                label.update(label_numpy)
+        else:   
+            # Resizes without maintaining aspect ratio.
+            image_numpy = cv2.resize(image.numpy(), (self._width, self._height))
+            if isinstance(label, Image):
+                label_numpy = cv2.resize(label.numpy(), (self._width, self._height))
+                label.update(label_numpy)
+
+        image.update(image_numpy)
+
+        return image, label
+
+class LabelIndexer(Transformer):
+    """Convert label to index by vocab
+    
+    Attributes:
+        vocab (typing.List[str]): List of characters in vocab
+    """
+    def __init__(
+        self, 
+        vocab: typing.List[str]
+        ) -> None:
+        self.vocab = vocab
+
+    def __call__(self, data: np.ndarray, label: np.ndarray):
+        return data, np.array([self.vocab.index(l) for l in label if l in self.vocab])
+
+class LabelPadding(Transformer):
+    """Pad label to max_word_length
+    
+    Attributes:
+        padding_value (int): Value to pad
+        max_word_length (int): Maximum length of label
+        use_on_batch (bool): Whether to use on batch. Default: False
+    """
+    def __init__(
+        self, 
+        padding_value: int,
+        max_word_length: int = None, 
+        use_on_batch: bool = False
+        ) -> None:
+        self.max_word_length = max_word_length
+        self.padding_value = padding_value
+        self.use_on_batch = use_on_batch
+
+        if not use_on_batch and max_word_length is None:
+            raise ValueError("max_word_length must be specified if use_on_batch is False")
+
+    def __call__(self, data: np.ndarray, label: np.ndarray):
+        if self.use_on_batch:
+            max_len = max([len(a) for a in label])
+            padded_labels = []
+            for l in label:
+                padded_label = np.pad(l, (0, max_len - len(l)), "constant", constant_values=self.padding_value)
+                padded_labels.append(padded_label)
+
+            padded_labels = np.array(padded_labels)
+            return data, padded_labels
+
+        label = label[:self.max_word_length]
+        return data, np.pad(label, (0, self.max_word_length - len(label)), "constant", constant_values=self.padding_value)
+
+
+class ImageNormalizer:
+    """ Normalize image to float value, transpose axis if necessary and convert to numpy
+    """
+    def __init__(self, transpose_axis: bool=False):
+        """ Initialize ImageNormalizer
+
+        Args:
+            transpose_axis (bool): Whether to transpose axis. Default: False
+        """
+        self.transpose_axis = transpose_axis
+    
+    def __call__(self, image: Image, annotation: typing.Any) -> typing.Tuple[np.ndarray, typing.Any]:
+        """ Convert each Image to numpy, transpose axis ant normalize to float value
+        """
+        img = image.numpy() / 255.0
+
+        if self.transpose_axis:
+            img = img.transpose(2, 0, 1)
+        
+        return img, annotation
+
+
+class SpectrogramPadding(Transformer):
+    """Pad spectrogram to max_spectrogram_length
+    
+    Attributes:
+        padding_value (int): Value to pad
+        max_spectrogram_length (int): Maximum length of spectrogram. Must be specified if use_on_batch is False. Default: None
+        use_on_batch (bool): Whether to use on batch. Default: False
+    """
+    def __init__(
+        self, 
+        padding_value: int,
+        max_spectrogram_length: int = None, 
+        use_on_batch: bool = False
+        ) -> None:
+        self.max_spectrogram_length = max_spectrogram_length
+        self.padding_value = padding_value
+        self.use_on_batch = use_on_batch
+
+        if not use_on_batch and max_spectrogram_length is None:
+            raise ValueError("max_spectrogram_length must be specified if use_on_batch is False")
+
+    def __call__(self, spectrogram: np.ndarray, label: np.ndarray):
+        if self.use_on_batch:
+            max_len = max([len(a) for a in spectrogram])
+            padded_spectrograms = []
+            for spec in spectrogram:
+                padded_spectrogram = np.pad(spec, ((0, max_len - spec.shape[0]), (0,0)), mode="constant", constant_values=self.padding_value)
+                padded_spectrograms.append(padded_spectrogram)
+
+            padded_spectrograms = np.array(padded_spectrograms)
+            label = np.array(label)
+
+            return padded_spectrograms, label
+
+        padded_spectrogram = np.pad(spectrogram, ((0, self.max_spectrogram_length - spectrogram.shape[0]),(0,0)), mode="constant", constant_values=self.padding_value)
+
+        return padded_spectrogram, label
+
+
+class AudioPadding(Transformer):
+    def __init__(self, max_audio_length: int, padding_value: int = 0, use_on_batch: bool = False, limit: bool = False):
+        super(AudioPadding, self).__init__()
+        self.max_audio_length = max_audio_length
+        self.padding_value = padding_value
+        self.use_on_batch = use_on_batch
+        self.limit = limit
+
+    def __call__(self, audio: Audio, label: typing.Any):
+        # batched padding
+        if self.use_on_batch:
+            max_len = max([len(a) for a in audio])
+            padded_audios = []
+            for a in audio:
+                # limit audio if it exceed max_audio_length
+                padded_audio = np.pad(a, (0, max_len - a.shape[0]), mode="constant", constant_values=self.padding_value)
+                padded_audios.append(padded_audio)
+
+            padded_audios = np.array(padded_audios)
+            # limit audio if it exceed max_audio_length
+            if self.limit:
+                padded_audios = padded_audios[:, :self.max_audio_length]
+
+            return padded_audios, label
+
+        audio_numpy = audio.numpy()
+        # limit audio if it exceed max_audio_length
+        if self.limit:
+            audio_numpy = audio_numpy[:self.max_audio_length]
+        padded_audio = np.pad(audio_numpy, (0, self.max_audio_length - audio_numpy.shape[0]), mode="constant", constant_values=self.padding_value)
+
+        audio.audio = padded_audio
+
+        return audio, label
+
+class AudioToSpectrogram(Transformer):
+    """Read wav file with librosa and return audio and label
+    
+    Attributes:
+        frame_length (int): Length of the frames in samples.
+        frame_step (int): Step size between frames in samples.
+        fft_length (int): Number of FFT components.
+        log_level (int): Logging level (default: logging.INFO)
+    """
+    def __init__(
+            self,
+            frame_length: int = 256,
+            frame_step: int = 160,
+            fft_length: int = 384,
+            log_level: int = logging.INFO,
+        ) -> None:
+        super(AudioToSpectrogram, self).__init__(log_level=log_level)
+        self.frame_length = frame_length
+        self.frame_step = frame_step
+        self.fft_length = fft_length
+
+        # import librosa using importlib
+        try:
+            self.librosa = importlib.import_module('librosa')
+            print("librosa version:", self.librosa.__version__)
+        except ImportError:
+            raise ImportError("librosa is required to augment Audio. Please install it with `pip install librosa`.")
+
+    def __call__(self, audio: Audio, label: typing.Any):
+        """Compute the spectrogram of a WAV file
+
+        Args:
+            audio (Audio): Audio object
+            label (Any): Label of audio
+
+        Returns:
+            np.ndarray: Spectrogram of audio
+            label (Any): Label of audio
+        """
+
+        # Compute the Short Time Fourier Transform (STFT) of the audio data and store it in the variable 'spectrogram'
+        # The STFT is computed with a hop length of 'frame_step' samples, a window length of 'frame_length' samples, and 'fft_length' FFT components.
+        # The resulting spectrogram is also transposed for convenience
+        spectrogram = self.librosa.stft(audio.numpy(), hop_length=self.frame_step, win_length=self.frame_length, n_fft=self.fft_length).T
+
+        # Take the absolute value of the spectrogram to obtain the magnitude spectrum
+        spectrogram = np.abs(spectrogram)
+
+        # Take the square root of the magnitude spectrum to obtain the log spectrogram
+        spectrogram = np.power(spectrogram, 0.5)
+
+        # Normalize the spectrogram by subtracting the mean and dividing by the standard deviation.
+        # A small value of 1e-10 is added to the denominator to prevent division by zero.
+        spectrogram = (spectrogram - np.mean(spectrogram)) / (np.std(spectrogram) + 1e-10)
+
+        return spectrogram, label
+
+
+class ImageShowCV2(Transformer):
+    """Show image for visual inspection
+    """
+    def __init__(
+        self, 
+        verbose: bool = True,
+        log_level: int = logging.INFO,
+        name: str = "Image"
+        ) -> None:
+        """
+        Args:
+            verbose (bool): Whether to log label
+            log_level (int): Logging level (default: logging.INFO)
+            name (str): Name of window to show image
+        """
+        super(ImageShowCV2, self).__init__(log_level=log_level)
+        self.verbose = verbose
+        self.name = name
+        self.thread_started = False
+
+    def init_thread(self):
+        if not self.thread_started:
+            self.thread_started = True
+            self.image_queue = queue.Queue()
+
+            # Start a new thread to display the images, so that the main loop could run in multiple threads
+            self.thread = threading.Thread(target=self._display_images)
+            self.thread.start()
+
+    def _display_images(self) -> None:
+        """ Display images in a continuous loop """
+        while True:
+            image, label = self.image_queue.get()
+            if isinstance(label, Image):
+                cv2.imshow(self.name + "Label", label.numpy())
+            cv2.imshow(self.name, image.numpy())
+            cv2.waitKey(0)
+            cv2.destroyAllWindows()
+
+    def __call__(self, image: Image, label: typing.Any) -> typing.Tuple[Image, typing.Any]:
+        """ Show image for visual inspection
+
+        Args:
+            data (np.ndarray): Image data
+            label (np.ndarray): Label data
+        
+        Returns:
+            data (np.ndarray): Image data
+            label (np.ndarray): Label data (unchanged)
+        """
+        # Start cv2 image display thread
+        self.init_thread()
+
+        if self.verbose:
+            if isinstance(label, (str, int, float)):
+                self.logger.info(f"Label: {label}")
+
+        if isinstance(label, Detections):
+            for detection in label:
+                img = detection.applyToFrame(np.asarray(image.numpy()))
+                image.update(img)
+
+        # Add image to display queue
+        # Sleep if queue is not empty
+        while not self.image_queue.empty():
+            time.sleep(0.5)
+
+        # Add image to display queue
+        self.image_queue.put((image, label))
+
         return image, label
```

### Comparing `mltu-1.2.4/mltu/utils/text_utils.py` & `mltu-1.2.5/mltu/utils/text_utils.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import typing
-import numpy as np
-from itertools import groupby
-
-
-def ctc_decoder(predictions: np.ndarray, chars: typing.Union[str, list]) -> typing.List[str]:
-    """ CTC greedy decoder for predictions
-    
-    Args:
-        predictions (np.ndarray): predictions from model
-        chars (typing.Union[str, list]): list of characters
-
-    Returns:
-        typing.List[str]: list of words
-    """
-    # use argmax to find the index of the highest probability
-    argmax_preds = np.argmax(predictions, axis=-1)
-    
-    # use groupby to find continuous same indexes
-    grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
-
-    # convert indexes to chars
-    texts = ["".join([chars[k] for k in group if k < len(chars)]) for group in grouped_preds]
-
-    return texts
-
-
-def edit_distance(prediction_tokens: typing.List[str], reference_tokens: typing.List[str]) -> int:
-    """ Standard dynamic programming algorithm to compute the Levenshtein Edit Distance Algorithm
-
-    Args:
-        prediction_tokens: A tokenized predicted sentence
-        reference_tokens: A tokenized reference sentence
-    Returns:
-        Edit distance between the predicted sentence and the reference sentence
-    """
-    # Initialize a matrix to store the edit distances
-    dp = [[0] * (len(reference_tokens) + 1) for _ in range(len(prediction_tokens) + 1)]
-
-    # Fill the first row and column with the number of insertions needed
-    for i in range(len(prediction_tokens) + 1):
-        dp[i][0] = i
-    
-    for j in range(len(reference_tokens) + 1):
-        dp[0][j] = j
-
-    # Iterate through the prediction and reference tokens
-    for i, p_tok in enumerate(prediction_tokens):
-        for j, r_tok in enumerate(reference_tokens):
-            # If the tokens are the same, the edit distance is the same as the previous entry
-            if p_tok == r_tok:
-                dp[i+1][j+1] = dp[i][j]
-            # If the tokens are different, the edit distance is the minimum of the previous entries plus 1
-            else:
-                dp[i+1][j+1] = min(dp[i][j+1], dp[i+1][j], dp[i][j]) + 1
-
-    # Return the final entry in the matrix as the edit distance     
-    return dp[-1][-1]
-
-def get_cer(
-    preds: typing.Union[str, typing.List[str]],
-    target: typing.Union[str, typing.List[str]],
-    ) -> float:
-    """ Update the cer score with the current set of references and predictions.
-
-    Args:
-        preds (typing.Union[str, typing.List[str]]): list of predicted sentences
-        target (typing.Union[str, typing.List[str]]): list of target words
-
-    Returns:
-        Character error rate score
-    """
-    if isinstance(preds, str):
-        preds = [preds]
-    if isinstance(target, str):
-        target = [target]
-
-    total, errors = 0, 0
-    for pred_tokens, tgt_tokens in zip(preds, target):
-        errors += edit_distance(list(pred_tokens), list(tgt_tokens))
-        total += len(tgt_tokens)
-
-    if total == 0:
-        return 0.0
-
-    cer = errors / total
-
-    return cer
-
-def get_wer(
-    preds: typing.Union[str, typing.List[str]],
-    target: typing.Union[str, typing.List[str]],
-    ) -> float:
-    """ Update the wer score with the current set of references and predictions.
-
-    Args:
-        target (typing.Union[str, typing.List[str]]): string of target sentence or list of target words
-        preds (typing.Union[str, typing.List[str]]): string of predicted sentence or list of predicted words
-
-    Returns:
-        Word error rate score
-    """
-    if isinstance(preds, str) and isinstance(target, str):
-        preds = [preds]
-        target = [target]
-
-    if isinstance(preds, list) and isinstance(target, list):
-        errors, total_words = 0, 0
-        for _pred, _target in zip(preds, target):
-            if isinstance(_pred, str) and isinstance(_target, str):
-                errors += edit_distance(_pred.split(), _target.split())
-                total_words += len(_target.split())
-            else:
-                print("Error: preds and target must be either both strings or both lists of strings.")
-                return np.inf
-            
-    else:
-        print("Error: preds and target must be either both strings or both lists of strings.")
-        return np.inf
-    
-    wer = errors / total_words
-            
+import typing
+import numpy as np
+from itertools import groupby
+
+
+def ctc_decoder(predictions: np.ndarray, chars: typing.Union[str, list]) -> typing.List[str]:
+    """ CTC greedy decoder for predictions
+    
+    Args:
+        predictions (np.ndarray): predictions from model
+        chars (typing.Union[str, list]): list of characters
+
+    Returns:
+        typing.List[str]: list of words
+    """
+    # use argmax to find the index of the highest probability
+    argmax_preds = np.argmax(predictions, axis=-1)
+    
+    # use groupby to find continuous same indexes
+    grouped_preds = [[k for k,_ in groupby(preds)] for preds in argmax_preds]
+
+    # convert indexes to chars
+    texts = ["".join([chars[k] for k in group if k < len(chars)]) for group in grouped_preds]
+
+    return texts
+
+
+def edit_distance(prediction_tokens: typing.List[str], reference_tokens: typing.List[str]) -> int:
+    """ Standard dynamic programming algorithm to compute the Levenshtein Edit Distance Algorithm
+
+    Args:
+        prediction_tokens: A tokenized predicted sentence
+        reference_tokens: A tokenized reference sentence
+    Returns:
+        Edit distance between the predicted sentence and the reference sentence
+    """
+    # Initialize a matrix to store the edit distances
+    dp = [[0] * (len(reference_tokens) + 1) for _ in range(len(prediction_tokens) + 1)]
+
+    # Fill the first row and column with the number of insertions needed
+    for i in range(len(prediction_tokens) + 1):
+        dp[i][0] = i
+    
+    for j in range(len(reference_tokens) + 1):
+        dp[0][j] = j
+
+    # Iterate through the prediction and reference tokens
+    for i, p_tok in enumerate(prediction_tokens):
+        for j, r_tok in enumerate(reference_tokens):
+            # If the tokens are the same, the edit distance is the same as the previous entry
+            if p_tok == r_tok:
+                dp[i+1][j+1] = dp[i][j]
+            # If the tokens are different, the edit distance is the minimum of the previous entries plus 1
+            else:
+                dp[i+1][j+1] = min(dp[i][j+1], dp[i+1][j], dp[i][j]) + 1
+
+    # Return the final entry in the matrix as the edit distance     
+    return dp[-1][-1]
+
+def get_cer(
+    preds: typing.Union[str, typing.List[str]],
+    target: typing.Union[str, typing.List[str]],
+    ) -> float:
+    """ Update the cer score with the current set of references and predictions.
+
+    Args:
+        preds (typing.Union[str, typing.List[str]]): list of predicted sentences
+        target (typing.Union[str, typing.List[str]]): list of target words
+
+    Returns:
+        Character error rate score
+    """
+    if isinstance(preds, str):
+        preds = [preds]
+    if isinstance(target, str):
+        target = [target]
+
+    total, errors = 0, 0
+    for pred_tokens, tgt_tokens in zip(preds, target):
+        errors += edit_distance(list(pred_tokens), list(tgt_tokens))
+        total += len(tgt_tokens)
+
+    if total == 0:
+        return 0.0
+
+    cer = errors / total
+
+    return cer
+
+def get_wer(
+    preds: typing.Union[str, typing.List[str]],
+    target: typing.Union[str, typing.List[str]],
+    ) -> float:
+    """ Update the wer score with the current set of references and predictions.
+
+    Args:
+        target (typing.Union[str, typing.List[str]]): string of target sentence or list of target words
+        preds (typing.Union[str, typing.List[str]]): string of predicted sentence or list of predicted words
+
+    Returns:
+        Word error rate score
+    """
+    if isinstance(preds, str) and isinstance(target, str):
+        preds = [preds]
+        target = [target]
+
+    if isinstance(preds, list) and isinstance(target, list):
+        errors, total_words = 0, 0
+        for _pred, _target in zip(preds, target):
+            if isinstance(_pred, str) and isinstance(_target, str):
+                errors += edit_distance(_pred.split(), _target.split())
+                total_words += len(_target.split())
+            else:
+                print("Error: preds and target must be either both strings or both lists of strings.")
+                return np.inf
+            
+    else:
+        print("Error: preds and target must be either both strings or both lists of strings.")
+        return np.inf
+    
+    wer = errors / total_words
+            
     return wer
```

### Comparing `mltu-1.2.4/mltu.egg-info/PKG-INFO` & `mltu-1.2.5/mltu.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1
-Name: mltu
-Version: 1.2.4
-Summary: Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch
-Home-page: https://pylessons.com/
-Author: PyLessons
-Author-email: pythonlessons0@gmail.com
-Project-URL: Source, https://github.com/pythonlessons/mltu/
-Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyYAML>=6.0
-Requires-Dist: tqdm
-Requires-Dist: qqdm==0.0.7
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: Pillow>=9.4.0
-Requires-Dist: onnxruntime>=1.15.0
-Requires-Dist: matplotlib
-Provides-Extra: gpu
-Requires-Dist: onnxruntime-gpu; extra == "gpu"
-
-# MLTU - Machine Learning Training Utilities
-Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
-<p align="center">
-  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
-</p>
-
-# Installation:
-To use MLTU in your own project, you can install it from PyPI:
-```bash
-pip install mltu
-```
-When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
-```bash
-pip install mltu==0.1.3
-```
-Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
-
-# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
-1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
-2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
-3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
-4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
-5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
-6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
-7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
-8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
-9. [Transformer training with TensorFlow for Translation task](https://pylessons.com/transformers-training), code in ```Tutorials\09_translation_transformer``` folder;
-10. [Speech Recognition in Python | finetune wav2vec2 model for a custom ASR model](https://youtu.be/h6ooEGzjkj0), code in ```Tutorials\10_wav2vec2_torch``` folder;
-11. [YOLOv8: Real-Time Object Detection Simplified](https://youtu.be/vegL__weCxY), code in ```Tutorials\11_Yolov8``` folder;
+Metadata-Version: 2.1
+Name: mltu
+Version: 1.2.5
+Summary: Machine Learning Training Utilities (MLTU) for TensorFlow and PyTorch
+Home-page: https://pylessons.com/
+Author: PyLessons
+Author-email: pythonlessons0@gmail.com
+Project-URL: Source, https://github.com/pythonlessons/mltu/
+Project-URL: Tracker, https://github.com/pythonlessons/mltu/issues
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: tqdm
+Requires-Dist: qqdm==0.0.7
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: Pillow>=9.4.0
+Requires-Dist: onnxruntime>=1.15.0
+Requires-Dist: matplotlib
+Provides-Extra: gpu
+Requires-Dist: onnxruntime-gpu; extra == "gpu"
+
+# MLTU - Machine Learning Training Utilities
+Machine Learning Training Utilities for <b>TensorFlow 2.*</b> and <b>PyTorch</b> with Python 3
+<p align="center">
+  <img src="https://pylessons.com/media/Tutorials/mltu/machine-learning-training-utilities.png">
+</p>
+
+# Installation:
+To use MLTU in your own project, you can install it from PyPI:
+```bash
+pip install mltu
+```
+When running tutorials, it's necessary to install mltu for a specific tutorial, for example:
+```bash
+pip install mltu==0.1.3
+```
+Each tutorial has its own requirements.txt file for a specific mltu version. As this project progress, the newest versions may have breaking changes, so it's recommended to use the same version as in the tutorial.
+
+# Tutorials and Examples can be found on [PyLessons.com](https://pylessons.com/mltu)
+1. [Text Recognition With TensorFlow and CTC network](https://pylessons.com/ctc-text-recognition), code in ```Tutorials\01_image_to_word``` folder;
+2. [TensorFlow OCR model for reading Captchas](https://pylessons.com/tensorflow-ocr-captcha), code in ```Tutorials\02_captcha_to_text``` folder;
+3. [Handwriting words recognition with TensorFlow](https://pylessons.com/handwriting-recognition), code in ```Tutorials\03_handwriting_recognition``` folder;
+4. [Handwritten sentence recognition with TensorFlow](https://pylessons.com/handwritten-sentence-recognition), code in ```Tutorials\04_sentence_recognition``` folder;
+5. [Introduction to speech recognition with TensorFlow](https://pylessons.com/speech-recognition), code in ```Tutorials\05_speech_recognition``` folder;
+6. [Introduction to PyTorch in a practical way](https://pylessons.com/pytorch-introduction), code in ```Tutorials\06_pytorch_introduction``` folder;
+7. [Using custom wrapper to simplify PyTorch models training pipeline](https://pylessons.com/pytorch-introduction), code in ```Tutorials\07_pytorch_wrapper``` folder;
+8. [Handwriting words recognition with PyTorch](https://pylessons.com/handwriting-recognition-pytorch), code in ```Tutorials\08_handwriting_recognition_torch``` folder;
+9. [Transformer training with TensorFlow for Translation task](https://pylessons.com/transformers-training), code in ```Tutorials\09_translation_transformer``` folder;
+10. [Speech Recognition in Python | finetune wav2vec2 model for a custom ASR model](https://youtu.be/h6ooEGzjkj0), code in ```Tutorials\10_wav2vec2_torch``` folder;
+11. [YOLOv8: Real-Time Object Detection Simplified](https://youtu.be/vegL__weCxY), code in ```Tutorials\11_Yolov8``` folder;
+12. [YOLOv8: Customizing Object Detector training](https://youtu.be/ysYiV1CbCyY), code in ```Tutorials\11_Yolov8\train_yolov8.py``` folder;
```

### Comparing `mltu-1.2.4/mltu.egg-info/SOURCES.txt` & `mltu-1.2.5/mltu.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 mltu/torch/yolo/__init__.py
 mltu/torch/yolo/annotation.py
 mltu/torch/yolo/loss.py
 mltu/torch/yolo/metrics.py
 mltu/torch/yolo/optimizer.py
 mltu/torch/yolo/preprocessors.py
 mltu/torch/yolo/pruning_utils.py
-mltu/torch/yolo/train.py
-mltu/torch/yolo/train_yolo.py
 mltu/torch/yolo/detectors/__init__.py
 mltu/torch/yolo/detectors/detector.py
 mltu/torch/yolo/detectors/onnx_detector.py
 mltu/torch/yolo/detectors/torch_detector.py
 mltu/utils/__init__.py
-mltu/utils/text_utils.py
+mltu/utils/text_utils.py
+tests/test_tensorflow_metrics.py
+tests/test_text_utils.py
```

