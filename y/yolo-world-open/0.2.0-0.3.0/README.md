# Comparing `tmp/yolo_world_open-0.2.0.tar.gz` & `tmp/yolo_world_open-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolo_world_open-0.2.0.tar", last modified: Fri May  3 20:33:30 2024, max compression
+gzip compressed data, was "yolo_world_open-0.3.0.tar", last modified: Sat May  4 20:24:32 2024, max compression
```

## Comparing `yolo_world_open-0.2.0.tar` & `yolo_world_open-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    70296 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/LICENSE
--rw-r--r--   0 nisyad    (1000) nisyad    (1000)    18940 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/PKG-INFO
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    17709 2024-05-03 03:39:22.000000 yolo_world_open-0.2.0/README.md
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     1467 2024-05-03 20:32:48.000000 yolo_world_open-0.2.0/pyproject.toml
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       38 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/setup.cfg
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      342 2024-05-03 03:39:22.000000 yolo_world_open-0.2.0/yolo_world/__init__.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/datasets/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      685 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     4086 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/mm_dataset.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/datasets/transformers/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      383 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/transformers/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    47488 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/transformers/mm_mix_img_transforms.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     4676 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/transformers/mm_transforms.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     2152 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/utils.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      491 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/yolov5_lvis.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     7432 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/yolov5_mixed_grounding.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      508 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/yolov5_obj365v1.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      508 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/yolov5_obj365v2.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     3839 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/datasets/yolov5_v3det.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/engine/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       84 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/engine/__init__.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/engine/optimizers/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      161 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/engine/optimizers/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     8648 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/engine/optimizers/yolow_v5_optim_constructor.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      314 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/__init__.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/assigner/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       91 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/assigner/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     4380 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/assigner/task_aligned_assigner.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/backbones/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      458 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/backbones/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     8441 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/backbones/mm_backbone.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/data_preprocessors/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      146 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/data_preprocessors/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     2331 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/data_preprocessors/data_preprocessor.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/dense_heads/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      296 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/dense_heads/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    27793 2024-05-03 03:39:22.000000 yolo_world_open-0.2.0/yolo_world/models/dense_heads/yolo_world_head.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    24647 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/dense_heads/yolo_world_seg_head.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/detectors/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      177 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/detectors/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     8380 2024-05-03 03:39:22.000000 yolo_world_open-0.2.0/yolo_world/models/detectors/yolo_world.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/layers/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      408 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/layers/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    19059 2024-05-03 03:39:22.000000 yolo_world_open-0.2.0/yolo_world/models/layers/yolo_bricks.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/losses/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      113 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/losses/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     1292 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/losses/dynamic_loss.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world/models/necks/
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      167 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/necks/__init__.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     9838 2024-03-29 20:38:18.000000 yolo_world_open-0.2.0/yolo_world/models/necks/yolo_world_pafpn.py
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      744 2024-05-03 03:39:22.000000 yolo_world_open-0.2.0/yolo_world/version.py
-drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-03 20:33:30.048644 yolo_world_open-0.2.0/yolo_world_open.egg-info/
--rw-r--r--   0 nisyad    (1000) nisyad    (1000)    18940 2024-05-03 20:33:30.000000 yolo_world_open-0.2.0/yolo_world_open.egg-info/PKG-INFO
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     1650 2024-05-03 20:33:30.000000 yolo_world_open-0.2.0/yolo_world_open.egg-info/SOURCES.txt
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)        1 2024-05-03 20:33:30.000000 yolo_world_open-0.2.0/yolo_world_open.egg-info/dependency_links.txt
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      181 2024-05-03 20:33:30.000000 yolo_world_open-0.2.0/yolo_world_open.egg-info/requires.txt
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       11 2024-05-03 20:33:30.000000 yolo_world_open-0.2.0/yolo_world_open.egg-info/top_level.txt
--rw-rw-r--   0 nisyad    (1000) nisyad    (1000)        1 2024-05-03 04:05:14.000000 yolo_world_open-0.2.0/yolo_world_open.egg-info/zip-safe
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.731065 yolo_world_open-0.3.0/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    70296 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/LICENSE
+-rw-r--r--   0 nisyad    (1000) nisyad    (1000)    18940 2024-05-04 20:24:32.731065 yolo_world_open-0.3.0/PKG-INFO
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    17709 2024-05-03 03:39:22.000000 yolo_world_open-0.3.0/README.md
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     1468 2024-05-04 20:23:50.000000 yolo_world_open-0.3.0/pyproject.toml
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       38 2024-05-04 20:24:32.731065 yolo_world_open-0.3.0/setup.cfg
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      342 2024-05-03 03:39:22.000000 yolo_world_open-0.3.0/yolo_world/__init__.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/datasets/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      685 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     4086 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/mm_dataset.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/datasets/transformers/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      383 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/transformers/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    47488 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/transformers/mm_mix_img_transforms.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     4676 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/transformers/mm_transforms.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     2152 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/utils.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      491 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/yolov5_lvis.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     7432 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/yolov5_mixed_grounding.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      508 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/yolov5_obj365v1.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      508 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/yolov5_obj365v2.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     3839 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/datasets/yolov5_v3det.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/engine/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       84 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/engine/__init__.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/engine/optimizers/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      161 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/engine/optimizers/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     8648 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/engine/optimizers/yolow_v5_optim_constructor.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      314 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/__init__.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/assigner/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       91 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/assigner/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     4380 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/assigner/task_aligned_assigner.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/backbones/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      458 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/backbones/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     8441 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/backbones/mm_backbone.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/data_preprocessors/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      146 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/data_preprocessors/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     2331 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/data_preprocessors/data_preprocessor.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/dense_heads/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      296 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/dense_heads/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    27793 2024-05-03 03:39:22.000000 yolo_world_open-0.3.0/yolo_world/models/dense_heads/yolo_world_head.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    24647 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/dense_heads/yolo_world_seg_head.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/detectors/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      177 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/detectors/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     8380 2024-05-03 03:39:22.000000 yolo_world_open-0.3.0/yolo_world/models/detectors/yolo_world.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.727065 yolo_world_open-0.3.0/yolo_world/models/layers/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      408 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/layers/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)    19059 2024-05-03 03:39:22.000000 yolo_world_open-0.3.0/yolo_world/models/layers/yolo_bricks.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.731065 yolo_world_open-0.3.0/yolo_world/models/losses/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      113 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/losses/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     1292 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/losses/dynamic_loss.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.731065 yolo_world_open-0.3.0/yolo_world/models/necks/
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      167 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/necks/__init__.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     9838 2024-03-29 20:38:18.000000 yolo_world_open-0.3.0/yolo_world/models/necks/yolo_world_pafpn.py
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      744 2024-05-03 03:39:22.000000 yolo_world_open-0.3.0/yolo_world/version.py
+drwxrwxr-x   0 nisyad    (1000) nisyad    (1000)        0 2024-05-04 20:24:32.731065 yolo_world_open-0.3.0/yolo_world_open.egg-info/
+-rw-r--r--   0 nisyad    (1000) nisyad    (1000)    18940 2024-05-04 20:24:32.000000 yolo_world_open-0.3.0/yolo_world_open.egg-info/PKG-INFO
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)     1650 2024-05-04 20:24:32.000000 yolo_world_open-0.3.0/yolo_world_open.egg-info/SOURCES.txt
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)        1 2024-05-04 20:24:32.000000 yolo_world_open-0.3.0/yolo_world_open.egg-info/dependency_links.txt
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)      181 2024-05-04 20:24:32.000000 yolo_world_open-0.3.0/yolo_world_open.egg-info/requires.txt
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)       11 2024-05-04 20:24:32.000000 yolo_world_open-0.3.0/yolo_world_open.egg-info/top_level.txt
+-rw-rw-r--   0 nisyad    (1000) nisyad    (1000)        1 2024-05-03 04:05:14.000000 yolo_world_open-0.3.0/yolo_world_open.egg-info/zip-safe
```

### Comparing `yolo_world_open-0.2.0/LICENSE` & `yolo_world_open-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/PKG-INFO` & `yolo_world_open-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolo_world_open
-Version: 0.2.0
+Version: 0.3.0
 Summary: YOLO-World: Real-time Open Vocabulary Object Detection
 Author-email: Tencent AILab <ronnysong@tencent.com>
 License: Apache License 2.0
 Keywords: object detection
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,22 +20,22 @@
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: torch>=2.1.0
 Requires-Dist: torchvision>=0.16.2
 Requires-Dist: transformers
 Requires-Dist: tokenizers
 Requires-Dist: numpy
-Requires-Dist: opencv-python-headless
 Requires-Dist: supervision==0.19.0
 Requires-Dist: openmim
 Requires-Dist: mmcv-lite>=2.0.0rc4
 Requires-Dist: mmdet>=3.0.0
 Requires-Dist: mmengine>=0.7.1
 Requires-Dist: mmcv
 Requires-Dist: mmyolo
+Requires-Dist: opencv-python-headless
 
 <div align="center">
 <img src="./assets/yolo_logo.png" width=60%>
 <br>
 <a href="https://scholar.google.com/citations?hl=zh-CN&user=PH8rJHYAAAAJ">Tianheng Cheng</a><sup><span>2,3,*</span></sup>, 
 <a href="https://linsong.info/">Lin Song</a><sup><span>1,📧,*</span></sup>,
 <a href="https://yxgeee.github.io/">Yixiao Ge</a><sup><span>1,🌟,2</span></sup>,
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: yolo_world_open Version: 0.2.0 Summary: YOLO-World:
+Metadata-Version: 2.1 Name: yolo_world_open Version: 0.3.0 Summary: YOLO-World:
 Real-time Open Vocabulary Object Detection Author-email: Tencent AILab
 tencent.com> License: Apache License 2.0 Keywords: object detection Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: wheel Requires-Dist: torch>=2.1.0 Requires-Dist: torchvision>=0.16.2
 Requires-Dist: transformers Requires-Dist: tokenizers Requires-Dist: numpy
-Requires-Dist: opencv-python-headless Requires-Dist: supervision==0.19.0
-Requires-Dist: openmim Requires-Dist: mmcv-lite>=2.0.0rc4 Requires-Dist:
-mmdet>=3.0.0 Requires-Dist: mmengine>=0.7.1 Requires-Dist: mmcv Requires-Dist:
-mmyolo
+Requires-Dist: supervision==0.19.0 Requires-Dist: openmim Requires-Dist: mmcv-
+lite>=2.0.0rc4 Requires-Dist: mmdet>=3.0.0 Requires-Dist: mmengine>=0.7.1
+Requires-Dist: mmcv Requires-Dist: mmyolo Requires-Dist: opencv-python-headless
                            [./assets/yolo_logo.png]
 _T_i_a_n_h_e_n_g_ _C_h_e_n_g2,3,*, _L_i_n_ _S_o_n_g1,ð§,*, _Y_i_x_i_a_o_ _G_e1,ð,2, _W_e_n_y_u_ _L_i_u3, _X_i_n_g_g_a_n_g
      _W_a_n_g3,ð§, _Y_i_n_g_ _S_h_a_n1,2 \* Equal contribution ð Project lead ð§
    Corresponding author 1 Tencent AI Lab, 2 ARC Lab, Tencent PCG 3 Huazhong
                      University of Science and Technology
   [![arxiv paper](https://img.shields.io/badge/Project-Page-green)](https://
  wondervictor.github.io/) [![arxiv paper](https://img.shields.io/badge/arXiv-
```

### Comparing `yolo_world_open-0.2.0/README.md` & `yolo_world_open-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/pyproject.toml` & `yolo_world_open-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","torch"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yolo_world_open"
-version = "0.2.0"
+version = "0.3.0"
 description = "YOLO-World: Real-time Open Vocabulary Object Detection"
 readme = "README.md"
 keywords = ["object detection"]
 authors = [
     { name = "Tencent AILab", email = "ronnysong@tencent.com" },
 ]
 license = {text = "Apache License 2.0"}
@@ -30,22 +30,22 @@
 dependencies = [
     "wheel",
     "torch>=2.1.0",
     "torchvision>=0.16.2",
     "transformers",
     "tokenizers",
     "numpy",
-    "opencv-python-headless",
     "supervision==0.19.0",
     "openmim",
     "mmcv-lite>=2.0.0rc4",
     "mmdet>=3.0.0",
     "mmengine>=0.7.1",
     "mmcv",
-    "mmyolo"
+    "mmyolo",
+    "opencv-python-headless",
 
 ]
 
 [tool.setuptools]
 package-dir = {"yolo_world_open" = "yolo_world"}
 include-package-data = false
 license-files = ["LICENSE"]
```

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/__init__.py` & `yolo_world_open-0.3.0/yolo_world/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/mm_dataset.py` & `yolo_world_open-0.3.0/yolo_world/datasets/mm_dataset.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/transformers/mm_mix_img_transforms.py` & `yolo_world_open-0.3.0/yolo_world/datasets/transformers/mm_mix_img_transforms.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/transformers/mm_transforms.py` & `yolo_world_open-0.3.0/yolo_world/datasets/transformers/mm_transforms.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/utils.py` & `yolo_world_open-0.3.0/yolo_world/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/yolov5_mixed_grounding.py` & `yolo_world_open-0.3.0/yolo_world/datasets/yolov5_mixed_grounding.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/datasets/yolov5_v3det.py` & `yolo_world_open-0.3.0/yolo_world/datasets/yolov5_v3det.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/engine/optimizers/yolow_v5_optim_constructor.py` & `yolo_world_open-0.3.0/yolo_world/engine/optimizers/yolow_v5_optim_constructor.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/assigner/task_aligned_assigner.py` & `yolo_world_open-0.3.0/yolo_world/models/assigner/task_aligned_assigner.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/backbones/mm_backbone.py` & `yolo_world_open-0.3.0/yolo_world/models/backbones/mm_backbone.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/data_preprocessors/data_preprocessor.py` & `yolo_world_open-0.3.0/yolo_world/models/data_preprocessors/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/dense_heads/yolo_world_head.py` & `yolo_world_open-0.3.0/yolo_world/models/dense_heads/yolo_world_head.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/dense_heads/yolo_world_seg_head.py` & `yolo_world_open-0.3.0/yolo_world/models/dense_heads/yolo_world_seg_head.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/detectors/yolo_world.py` & `yolo_world_open-0.3.0/yolo_world/models/detectors/yolo_world.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/layers/yolo_bricks.py` & `yolo_world_open-0.3.0/yolo_world/models/layers/yolo_bricks.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/losses/dynamic_loss.py` & `yolo_world_open-0.3.0/yolo_world/models/losses/dynamic_loss.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/models/necks/yolo_world_pafpn.py` & `yolo_world_open-0.3.0/yolo_world/models/necks/yolo_world_pafpn.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world/version.py` & `yolo_world_open-0.3.0/yolo_world/version.py`

 * *Files identical despite different names*

### Comparing `yolo_world_open-0.2.0/yolo_world_open.egg-info/PKG-INFO` & `yolo_world_open-0.3.0/yolo_world_open.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolo_world_open
-Version: 0.2.0
+Version: 0.3.0
 Summary: YOLO-World: Real-time Open Vocabulary Object Detection
 Author-email: Tencent AILab <ronnysong@tencent.com>
 License: Apache License 2.0
 Keywords: object detection
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,22 +20,22 @@
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: torch>=2.1.0
 Requires-Dist: torchvision>=0.16.2
 Requires-Dist: transformers
 Requires-Dist: tokenizers
 Requires-Dist: numpy
-Requires-Dist: opencv-python-headless
 Requires-Dist: supervision==0.19.0
 Requires-Dist: openmim
 Requires-Dist: mmcv-lite>=2.0.0rc4
 Requires-Dist: mmdet>=3.0.0
 Requires-Dist: mmengine>=0.7.1
 Requires-Dist: mmcv
 Requires-Dist: mmyolo
+Requires-Dist: opencv-python-headless
 
 <div align="center">
 <img src="./assets/yolo_logo.png" width=60%>
 <br>
 <a href="https://scholar.google.com/citations?hl=zh-CN&user=PH8rJHYAAAAJ">Tianheng Cheng</a><sup><span>2,3,*</span></sup>, 
 <a href="https://linsong.info/">Lin Song</a><sup><span>1,📧,*</span></sup>,
 <a href="https://yxgeee.github.io/">Yixiao Ge</a><sup><span>1,🌟,2</span></sup>,
```

#### html2text {}

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1 Name: yolo_world_open Version: 0.2.0 Summary: YOLO-World:
+Metadata-Version: 2.1 Name: yolo_world_open Version: 0.3.0 Summary: YOLO-World:
 Real-time Open Vocabulary Object Detection Author-email: Tencent AILab
 tencent.com> License: Apache License 2.0 Keywords: object detection Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: wheel Requires-Dist: torch>=2.1.0 Requires-Dist: torchvision>=0.16.2
 Requires-Dist: transformers Requires-Dist: tokenizers Requires-Dist: numpy
-Requires-Dist: opencv-python-headless Requires-Dist: supervision==0.19.0
-Requires-Dist: openmim Requires-Dist: mmcv-lite>=2.0.0rc4 Requires-Dist:
-mmdet>=3.0.0 Requires-Dist: mmengine>=0.7.1 Requires-Dist: mmcv Requires-Dist:
-mmyolo
+Requires-Dist: supervision==0.19.0 Requires-Dist: openmim Requires-Dist: mmcv-
+lite>=2.0.0rc4 Requires-Dist: mmdet>=3.0.0 Requires-Dist: mmengine>=0.7.1
+Requires-Dist: mmcv Requires-Dist: mmyolo Requires-Dist: opencv-python-headless
                            [./assets/yolo_logo.png]
 _T_i_a_n_h_e_n_g_ _C_h_e_n_g2,3,*, _L_i_n_ _S_o_n_g1,ð§,*, _Y_i_x_i_a_o_ _G_e1,ð,2, _W_e_n_y_u_ _L_i_u3, _X_i_n_g_g_a_n_g
      _W_a_n_g3,ð§, _Y_i_n_g_ _S_h_a_n1,2 \* Equal contribution ð Project lead ð§
    Corresponding author 1 Tencent AI Lab, 2 ARC Lab, Tencent PCG 3 Huazhong
                      University of Science and Technology
   [![arxiv paper](https://img.shields.io/badge/Project-Page-green)](https://
  wondervictor.github.io/) [![arxiv paper](https://img.shields.io/badge/arXiv-
```

### Comparing `yolo_world_open-0.2.0/yolo_world_open.egg-info/SOURCES.txt` & `yolo_world_open-0.3.0/yolo_world_open.egg-info/SOURCES.txt`

 * *Files identical despite different names*

