# Comparing `tmp/albumentations-1.4.4.tar.gz` & `tmp/albumentations-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albumentations-1.4.4.tar", last modified: Wed Apr 17 02:43:53 2024, max compression
+gzip compressed data, was "albumentations-1.4.6.tar", last modified: Sat May  4 05:33:59 2024, max compression
```

## Comparing `albumentations-1.4.4.tar` & `albumentations-1.4.6.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.151548 albumentations-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 02:43:43.000000 albumentations-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 02:43:43.000000 albumentations-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37431 2024-04-17 02:43:53.151548 albumentations-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35643 2024-04-17 02:43:43.000000 albumentations-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.139548 albumentations-1.4.4/albumentations/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/blur/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/blur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/blur/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/blur/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/crops/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/crops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/crops/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    51295 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/crops/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/domain_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/domain_adaptation_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/dropout/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/grid_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/mask_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/xy_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    51483 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/augmentations/geometric/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43928 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/resize.py
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    79800 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/augmentations/mixing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/mixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/mixing/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/mixing/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)   125104 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20469 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/bbox_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/keypoints_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/transforms_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/pytorch/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.151548 albumentations-1.4.4/albumentations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37431 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-17 02:43:43.000000 albumentations-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:43:53.151548 albumentations-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-17 02:43:43.000000 albumentations-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.151548 albumentations-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39987 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    52080 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_functional_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_functional_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_keypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    37460 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    52422 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.691548 albumentations-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 05:33:46.000000 albumentations-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 05:33:46.000000 albumentations-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-04 05:33:59.691548 albumentations-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35779 2024-05-04 05:33:46.000000 albumentations-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.675548 albumentations-1.4.6/albumentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.679548 albumentations-1.4.6/albumentations/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.679548 albumentations-1.4.6/albumentations/augmentations/blur/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/blur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/blur/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/blur/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.679548 albumentations-1.4.6/albumentations/augmentations/crops/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/crops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/crops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/crops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/domain_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/domain_adaptation_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/augmentations/dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/grid_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/mask_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/xy_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51656 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/augmentations/geometric/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43682 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79877 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/augmentations/mixing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/mixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/mixing/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/mixing/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125204 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22401 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/keypoints_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14159 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/transforms_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.687548 albumentations-1.4.6/albumentations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/pytorch/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.687548 albumentations-1.4.6/albumentations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-04 05:33:46.000000 albumentations-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:33:59.691548 albumentations-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-04 05:33:46.000000 albumentations-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.687548 albumentations-1.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40223 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12940 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54144 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_functional_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_functional_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38359 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57647 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_transforms.py
```

### Comparing `albumentations-1.4.4/LICENSE` & `albumentations-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/PKG-INFO` & `albumentations-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.4
+Version: 1.4.6
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,24 +28,28 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: PyYAML
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: scikit-learn>=1.3.2
-Requires-Dist: pydantic>=2.6.4
+Requires-Dist: pydantic>=2.7.0
 Requires-Dist: opencv-python-headless>=4.9.0
 
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/albumentations.svg?label=PyPI%20downloads)](
+https://pypi.org/project/albumentations/)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/albumentations.svg?label=Conda%20downloads)](
+https://anaconda.org/conda-forge/albumentations)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
+https://stackoverflow.com/questions/tagged/albumentations)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
 [Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
```

### Comparing `albumentations-1.4.4/README.md` & `albumentations-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/albumentations.svg?label=PyPI%20downloads)](
+https://pypi.org/project/albumentations/)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/albumentations.svg?label=Conda%20downloads)](
+https://anaconda.org/conda-forge/albumentations)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
+https://stackoverflow.com/questions/tagged/albumentations)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
 [Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
 # Albumentations [![PyPI version](https://badge.fury.io/py/albumentations.svg)]
 (https://badge.fury.io/py/albumentations) ![CI](https://github.com/
-albumentations-team/albumentations/workflows/CI/badge.svg) [![License: MIT]
-(https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://
-opensource.org/licenses/MIT) [![Ruff](https://img.shields.io/
-endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/
-badge/v2.json)](https://github.com/astral-sh/ruff) [![Pydantic v2](https://
-img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/
-pydantic/main/docs/badge/v2.json)](https://pydantic.dev) [Docs](https://
+albumentations-team/albumentations/workflows/CI/badge.svg) [![PyPI Downloads]
+(https://img.shields.io/pypi/dm/albumentations.svg?label=PyPI%20downloads)]
+( https://pypi.org/project/albumentations/) [![Conda Downloads](https://
+img.shields.io/conda/dn/conda-forge/
+albumentations.svg?label=Conda%20downloads)]( https://anaconda.org/conda-forge/
+albumentations) [![Stack Overflow](https://img.shields.io/badge/stackoverflow-
+Ask%20questions-blue.svg)]( https://stackoverflow.com/questions/tagged/
+albumentations) [![License: MIT](https://img.shields.io/badge/License-MIT-
+brightgreen.svg)](https://opensource.org/licenses/MIT) [Docs](https://
 albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter]
 (https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/
 company/100504475/) Albumentations is a Python library for image augmentation.
 Image augmentation is used in deep learning and computer vision tasks to
 increase the quality of trained models. The purpose of image augmentation is to
 create new training samples from the existing data. Here is an example of how
 you can apply some [pixel-level](#pixel-level-transforms) augmentations from
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/__init__.py` & `albumentations-1.4.6/albumentations/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/augmentations/blur/functional.py` & `albumentations-1.4.6/albumentations/augmentations/blur/functional.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 import numpy as np
 
 from albumentations.augmentations.functional import convolve
 from albumentations.augmentations.geometric.functional import scale
 from albumentations.augmentations.utils import (
     _maybe_process_in_chunks,
     clipped,
-    preserve_shape,
+    preserve_channel_dim,
 )
 
 __all__ = ["blur", "median_blur", "gaussian_blur", "glass_blur", "defocus", "central_zoom", "zoom_blur"]
 
 TWO = 2
 EIGHT = 8
 
 
-@preserve_shape
+@preserve_channel_dim
 def blur(img: np.ndarray, ksize: int) -> np.ndarray:
     blur_fn = _maybe_process_in_chunks(cv2.blur, ksize=(ksize, ksize))
     return blur_fn(img)
 
 
-@preserve_shape
+@preserve_channel_dim
 def median_blur(img: np.ndarray, ksize: int) -> np.ndarray:
     if img.dtype == np.float32 and ksize not in {3, 5}:
         raise ValueError(f"Invalid ksize value {ksize}. For a float32 image the only valid ksize values are 3 and 5")
 
     blur_fn = _maybe_process_in_chunks(cv2.medianBlur, ksize=ksize)
     return blur_fn(img)
 
 
-@preserve_shape
+@preserve_channel_dim
 def gaussian_blur(img: np.ndarray, ksize: int, sigma: float = 0) -> np.ndarray:
     # When sigma=0, it is computed as `sigma = 0.3*((ksize-1)*0.5 - 1) + 0.8`
     blur_fn = _maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
     return blur_fn(img)
 
 
-@preserve_shape
+@preserve_channel_dim
 def glass_blur(
     img: np.ndarray,
     sigma: float,
     max_delta: int,
     iterations: int,
     dxy: np.ndarray,
     mode: str,
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/blur/transforms.py` & `albumentations-1.4.6/albumentations/augmentations/blur/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,19 +68,19 @@
     class InitSchema(BlurInitSchema):
         pass
 
     def __init__(self, blur_limit: ScaleIntType = 7, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply, p)
         self.blur_limit = cast(Tuple[int, int], blur_limit)
 
-    def apply(self, img: np.ndarray, kernel: int = 3, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, kernel: int, **params: Any) -> np.ndarray:
         return F.blur(img, kernel)
 
     def get_params(self) -> Dict[str, Any]:
-        return {"ksize": int(random.choice(list(range(self.blur_limit[0], self.blur_limit[1] + 1, 2))))}
+        return {"kernel": random_utils.choice(list(range(self.blur_limit[0], self.blur_limit[1] + 1, 2)))}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("blur_limit",)
 
 
 class MotionBlur(Blur):
     """Apply motion blur to the input image using a random-sized kernel.
@@ -129,15 +129,15 @@
         super().__init__(blur_limit=blur_limit, always_apply=always_apply, p=p)
         self.allow_shifted = allow_shifted
         self.blur_limit = cast(Tuple[int, int], blur_limit)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (*super().get_transform_init_args_names(), "allow_shifted")
 
-    def apply(self, img: np.ndarray, kernel: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, kernel: np.ndarray, **params: Any) -> np.ndarray:
         return FMain.convolve(img, kernel=kernel)
 
     def get_params(self) -> Dict[str, Any]:
         ksize = random.choice(list(range(self.blur_limit[0], self.blur_limit[1] + 1, 2)))
         if ksize <= TWO:
             raise ValueError(f"ksize must be > 2. Got: {ksize}")
         kernel = np.zeros((ksize, ksize), dtype=np.uint8)
@@ -190,15 +190,15 @@
         uint8, float32
 
     """
 
     def __init__(self, blur_limit: ScaleIntType = 7, always_apply: bool = False, p: float = 0.5):
         super().__init__(blur_limit, always_apply, p)
 
-    def apply(self, img: np.ndarray, kernel: int = 3, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, kernel: int, **params: Any) -> np.ndarray:
         return F.median_blur(img, kernel)
 
 
 class GaussianBlur(ImageOnlyTransform):
     """Blur the input image using a Gaussian filter with a random kernel size.
 
     Args:
@@ -256,15 +256,15 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.blur_limit = cast(Tuple[int, int], blur_limit)
         self.sigma_limit = cast(Tuple[float, float], sigma_limit)
 
-    def apply(self, img: np.ndarray, ksize: int = 3, sigma: float = 0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, ksize: int, sigma: float, **params: Any) -> np.ndarray:
         return F.gaussian_blur(img, ksize, sigma=sigma)
 
     def get_params(self) -> Dict[str, float]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1)
         if ksize != 0 and ksize % 2 != 1:
             ksize = (ksize + 1) % (self.blur_limit[1] + 1)
 
@@ -314,15 +314,15 @@
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.sigma = sigma
         self.max_delta = max_delta
         self.iterations = iterations
         self.mode = mode
 
-    def apply(self, img: np.ndarray, *args: Any, dxy: np.ndarray = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, *args: Any, dxy: np.ndarray, **params: Any) -> np.ndarray:
         if dxy is None:
             msg = "dxy is None"
             raise ValueError(msg)
 
         return F.glass_blur(img, self.sigma, self.max_delta, self.iterations, dxy, self.mode)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
@@ -446,15 +446,15 @@
         self.blur_limit = cast(Tuple[int, int], blur_limit)
         self.sigma_x_limit = cast(Tuple[float, float], sigma_x_limit)
         self.sigma_y_limit = cast(Tuple[float, float], sigma_y_limit)
         self.rotate_limit = cast(Tuple[int, int], rotate_limit)
         self.beta_limit = cast(Tuple[float, float], beta_limit)
         self.noise_limit = cast(Tuple[float, float], noise_limit)
 
-    def apply(self, img: np.ndarray, kernel: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, kernel: np.ndarray, **params: Any) -> np.ndarray:
         return FMain.convolve(img, kernel=kernel)
 
     def get_params(self) -> Dict[str, np.ndarray]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2)
         sigma_x = random_utils.uniform(*self.sigma_x_limit)
         sigma_y = random_utils.uniform(*self.sigma_y_limit)
         angle = np.deg2rad(random.uniform(*self.rotate_limit))
@@ -528,15 +528,15 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.radius = cast(Tuple[int, int], radius)
         self.alias_blur = cast(Tuple[float, float], alias_blur)
 
-    def apply(self, img: np.ndarray, radius: int = 3, alias_blur: float = 0.5, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, radius: int, alias_blur: float, **params: Any) -> np.ndarray:
         return F.defocus(img, radius, alias_blur)
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "radius": random_utils.randint(self.radius[0], self.radius[1] + 1),
             "alias_blur": random_utils.uniform(self.alias_blur[0], self.alias_blur[1]),
         }
@@ -578,19 +578,15 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.max_factor = cast(Tuple[float, float], max_factor)
         self.step_factor = cast(Tuple[float, float], step_factor)
 
-    def apply(self, img: np.ndarray, zoom_factors: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
-        if zoom_factors is None:
-            msg = "zoom_factors is None"
-            raise ValueError(msg)
-
+    def apply(self, img: np.ndarray, zoom_factors: np.ndarray, **params: Any) -> np.ndarray:
         return F.zoom_blur(img, zoom_factors)
 
     def get_params(self) -> Dict[str, Any]:
         max_factor = random.uniform(self.max_factor[0], self.max_factor[1])
         step_factor = random.uniform(self.step_factor[0], self.step_factor[1])
         return {"zoom_factors": np.arange(1.0, max_factor, step_factor)}
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/crops/functional.py` & `albumentations-1.4.6/albumentations/augmentations/crops/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/augmentations/crops/transforms.py` & `albumentations-1.4.6/albumentations/augmentations/crops/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     NonNegativeFloatRangeType,
     OnePlusIntRangeType,
     ProbabilityType,
     ZeroOneRangeType,
 )
 from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import (
+    NUM_MULTI_CHANNEL_DIMENSIONS,
     BoxInternalType,
     ColorType,
     KeypointInternalType,
     ScaleFloatType,
     ScaleIntType,
     Targets,
 )
@@ -42,15 +43,14 @@
     "RandomSizedBBoxSafeCrop",
     "CropAndPad",
     "RandomCropFromBorders",
     "BBoxSafeRandomCrop",
 ]
 
 TWO = 2
-THREE = 3
 
 
 class CropInitSchema(BaseTransformInitSchema):
     height: Optional[int] = Field(description="Height of the crop", ge=1)
     width: Optional[int] = Field(description="Width of the crop", ge=1)
     p: ProbabilityType = 1
 
@@ -77,15 +77,15 @@
         pass
 
     def __init__(self, height: int, width: int, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
 
-    def apply(self, img: np.ndarray, h_start: int = 0, w_start: int = 0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, h_start: int, w_start: int, **params: Any) -> np.ndarray:
         return F.random_crop(img, self.height, self.width, h_start, w_start)
 
     def get_params(self) -> Dict[str, float]:
         return {"h_start": random.random(), "w_start": random.random()}
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return F.bbox_random_crop(bbox, self.height, self.width, **params)
@@ -244,29 +244,29 @@
         self.width = width
         self.ignore_values = ignore_values
         self.ignore_channels = ignore_channels
 
     def apply(
         self,
         img: np.ndarray,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> np.ndarray:
         return F.crop(img, x_min, y_min, x_max, y_max)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> BoxInternalType:
         return F.bbox_crop(
             bbox,
             x_min=x_min,
             x_max=x_max,
             y_min=y_min,
@@ -274,30 +274,30 @@
             rows=params["rows"],
             cols=params["cols"],
         )
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> KeypointInternalType:
         return F.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
 
     def _preprocess_mask(self, mask: np.ndarray) -> np.ndarray:
         mask_height, mask_width = mask.shape[:2]
 
         if self.ignore_values is not None:
             ignore_values_np = np.array(self.ignore_values)
             mask = np.where(np.isin(mask, ignore_values_np), 0, mask)
 
-        if mask.ndim == THREE and self.ignore_channels is not None:
+        if mask.ndim == NUM_MULTI_CHANNEL_DIMENSIONS and self.ignore_channels is not None:
             target_channels = np.array([ch for ch in range(mask.shape[-1]) if ch not in self.ignore_channels])
             mask = np.take(mask, target_channels, axis=-1)
 
         if self.height > mask_height or self.width > mask_width:
             raise ValueError(
                 f"Crop size ({self.height},{self.width}) is larger than image ({mask_height},{mask_width})",
             )
@@ -316,15 +316,15 @@
         else:
             msg = "Can not find mask for CropNonEmptyMaskIfExists"
             raise RuntimeError(msg)
 
         mask_height, mask_width = mask.shape[:2]
 
         if mask.any():
-            mask = mask.sum(axis=-1) if mask.ndim == THREE else mask
+            mask = mask.sum(axis=-1) if mask.ndim == NUM_MULTI_CHANNEL_DIMENSIONS else mask
             non_zero_yx = np.argwhere(mask)
             y, x = random.choice(non_zero_yx)
             x_min = x - random.randint(0, self.width - 1)
             y_min = y - random.randint(0, self.height - 1)
             x_min = np.clip(x_min, 0, mask_width - self.width)
             y_min = np.clip(y_min, 0, mask_height - self.height)
         else:
@@ -352,15 +352,16 @@
         return value
 
 
 class _BaseRandomSizedCrop(DualTransform):
     # Base class for RandomSizedCrop and RandomResizedCrop
 
     class InitSchema(BaseRandomSizedCropInitSchema):
-        pass
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        size: Tuple[int, int]
 
     def __init__(
         self,
         size: Tuple[int, int],
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
@@ -368,46 +369,46 @@
         super().__init__(always_apply, p)
         self.size = size
         self.interpolation = interpolation
 
     def apply(
         self,
         img: np.ndarray,
-        crop_height: int = 0,
-        crop_width: int = 0,
-        h_start: int = 0,
-        w_start: int = 0,
-        interpolation: int = cv2.INTER_LINEAR,
+        crop_height: int,
+        crop_width: int,
+        h_start: int,
+        w_start: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         crop = F.random_crop(img, crop_height, crop_width, h_start, w_start)
         return FGeometric.resize(crop, self.size[0], self.size[1], interpolation)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        crop_height: int = 0,
-        crop_width: int = 0,
-        h_start: int = 0,
-        w_start: int = 0,
-        rows: int = 0,
-        cols: int = 0,
+        crop_height: int,
+        crop_width: int,
+        h_start: int,
+        w_start: int,
+        rows: int,
+        cols: int,
         **params: Any,
     ) -> BoxInternalType:
         return F.bbox_random_crop(bbox, crop_height, crop_width, h_start, w_start, rows, cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        crop_height: int = 0,
-        crop_width: int = 0,
-        h_start: int = 0,
-        w_start: int = 0,
-        rows: int = 0,
-        cols: int = 0,
+        crop_height: int,
+        crop_width: int,
+        h_start: int,
+        w_start: int,
+        rows: int,
+        cols: int,
         **params: Any,
     ) -> KeypointInternalType:
         keypoint = F.keypoint_random_crop(keypoint, crop_height, crop_width, h_start, w_start, rows, cols)
         scale_y = self.size[0] / crop_height
         scale_x = self.size[1] / crop_width
         return FGeometric.keypoint_scale(keypoint, scale_x, scale_y)
 
@@ -435,45 +436,44 @@
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     class InitSchema(BaseTransformInitSchema):
         interpolation: InterpolationType = cv2.INTER_LINEAR
         p: ProbabilityType = 1
         min_max_height: OnePlusIntRangeType
         w2h_ratio: Annotated[float, Field(gt=0, description="Aspect ratio of crop.")]
-        width: Optional[int] = None
-        height: Optional[int] = None
+        width: Optional[int] = Field(
+            None,
+            deprecated=(
+                "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
+                "Please use a tuple (height, width) for the 'size' argument."
+            ),
+        )
+        height: Optional[int] = Field(
+            None,
+            deprecated=(
+                "Initializing with 'height' and 'width' is deprecated. "
+                "Please use a tuple (height, width) for the 'size' argument."
+            ),
+        )
         size: Optional[ScaleIntType] = None
 
         @model_validator(mode="after")
         def process(self) -> Self:
             if isinstance(self.size, int):
                 if isinstance(self.width, int):
                     self.size = (self.size, self.width)
-                    warn(
-                        "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
-                        "Please use a tuple (height, width) for the 'size' argument.",
-                        DeprecationWarning,
-                        stacklevel=2,
-                    )
                 else:
                     msg = "If size is an integer, width as integer must be specified."
                     raise TypeError(msg)
 
             if self.size is None:
                 if self.height is None or self.width is None:
                     message = "If 'size' is not provided, both 'height' and 'width' must be specified."
                     raise ValueError(message)
                 self.size = (self.height, self.width)
-                warn(
-                    "Initializing with 'height' and 'width' is deprecated. "
-                    "Please use a tuple (height, width) for the 'size' argument.",
-                    DeprecationWarning,
-                    stacklevel=2,
-                )
-
             return self
 
     def __init__(
         self,
         min_max_height: Tuple[int, int],
         # NOTE @zetyquickly: when (width, height) are deprecated, make 'size' non optional
         size: Optional[ScaleIntType] = None,
@@ -523,46 +523,38 @@
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     class InitSchema(BaseTransformInitSchema):
         scale: ZeroOneRangeType = (0.08, 1.0)
         ratio: NonNegativeFloatRangeType = (0.75, 1.3333333333333333)
-        width: Optional[int] = None
-        height: Optional[int] = None
+        width: Optional[int] = Field(
+            None, deprecated="Initializing with 'height' and 'width' is deprecated. Use size instead."
+        )
+        height: Optional[int] = Field(
+            None, deprecated="Initializing with 'height' and 'width' is deprecated. Use size instead."
+        )
         size: Optional[ScaleIntType] = None
         p: ProbabilityType = 1
         interpolation: InterpolationType = cv2.INTER_LINEAR
 
         @model_validator(mode="after")
         def process(self) -> Self:
             if isinstance(self.size, int):
                 if isinstance(self.width, int):
                     self.size = (self.size, self.width)
-                    warn(
-                        "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
-                        "Please use a tuple (height, width) for the 'size' argument.",
-                        DeprecationWarning,
-                        stacklevel=2,
-                    )
                 else:
                     msg = "If size is an integer, width as integer must be specified."
                     raise TypeError(msg)
 
             if self.size is None:
                 if self.height is None or self.width is None:
                     message = "If 'size' is not provided, both 'height' and 'width' must be specified."
                     raise ValueError(message)
                 self.size = (self.height, self.width)
-                warn(
-                    "Initializing with 'height' and 'width' is deprecated. "
-                    "Please use a tuple (height, width) for the 'size' argument.",
-                    DeprecationWarning,
-                    stacklevel=2,
-                )
 
             return self
 
     def __init__(
         self,
         # NOTE @zetyquickly: when (width, height) are deprecated, make 'size' non optional
         size: Optional[ScaleIntType] = None,
@@ -687,18 +679,18 @@
 
         self.max_part_shift = cast(Tuple[float, float], max_part_shift)
         self.cropping_bbox_key = cropping_bbox_key
 
     def apply(
         self,
         img: np.ndarray,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> np.ndarray:
         return F.clamping_crop(img, x_min, y_min, x_max, y_max)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, int]:
         bbox = params[self.cropping_bbox_key]
         h_max_shift = round((bbox[3] - bbox[1]) * self.max_part_shift[0])
@@ -717,18 +709,18 @@
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return F.bbox_crop(bbox, **params)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> KeypointInternalType:
         return F.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
 
     @property
     def targets_as_params(self) -> List[str]:
         return [self.cropping_bbox_key]
@@ -764,18 +756,18 @@
     def __init__(self, erosion_rate: float = 0.0, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.erosion_rate = erosion_rate
 
     def apply(
         self,
         img: np.ndarray,
-        crop_height: int = 0,
-        crop_width: int = 0,
-        h_start: int = 0,
-        w_start: int = 0,
+        crop_height: int,
+        crop_width: int,
+        h_start: int,
+        w_start: int,
         **params: Any,
     ) -> np.ndarray:
         return F.random_crop(img, crop_height, crop_width, h_start, w_start)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Union[int, float]]:
         img_h, img_w = params["image"].shape[:2]
         if len(params["bboxes"]) == 0:  # less likely, this class is for use with bboxes.
@@ -803,20 +795,20 @@
         h_start = np.clip(0.0 if bh >= 1.0 else by / (1.0 - bh), 0.0, 1.0)
         w_start = np.clip(0.0 if bw >= 1.0 else bx / (1.0 - bw), 0.0, 1.0)
         return {"h_start": h_start, "w_start": w_start, "crop_height": crop_height, "crop_width": crop_width}
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        crop_height: int = 0,
-        crop_width: int = 0,
-        h_start: int = 0,
-        w_start: int = 0,
-        rows: int = 0,
-        cols: int = 0,
+        crop_height: int,
+        crop_width: int,
+        h_start: int,
+        w_start: int,
+        rows: int,
+        cols: int,
         **params: Any,
     ) -> BoxInternalType:
         return F.bbox_random_crop(bbox, crop_height, crop_width, h_start, w_start, rows, cols)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image", "bboxes"]
@@ -867,23 +859,22 @@
         self.height = height
         self.width = width
         self.interpolation = interpolation
 
     def apply(
         self,
         img: np.ndarray,
-        crop_height: int = 0,
-        crop_width: int = 0,
-        h_start: int = 0,
-        w_start: int = 0,
-        interpolation: int = cv2.INTER_LINEAR,
+        crop_height: int,
+        crop_width: int,
+        h_start: int,
+        w_start: int,
         **params: Any,
     ) -> np.ndarray:
         crop = F.random_crop(img, crop_height, crop_width, h_start, w_start)
-        return FGeometric.resize(crop, self.height, self.width, interpolation)
+        return FGeometric.resize(crop, self.height, self.width, self.interpolation)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (*super().get_transform_init_args_names(), "height", "width", "interpolation")
 
 
 class CropAndPad(DualTransform):
     """Crop and pad images by pixel amounts or fractions of image sizes.
@@ -1037,20 +1028,20 @@
         self.sample_independently = sample_independently
 
         self.interpolation = interpolation
 
     def apply(
         self,
         img: np.ndarray,
-        crop_params: Sequence[int] = (),
-        pad_params: Sequence[int] = (),
-        pad_value: float = 0,
-        rows: int = 0,
-        cols: int = 0,
-        interpolation: int = cv2.INTER_LINEAR,
+        crop_params: Sequence[int],
+        pad_params: Sequence[int],
+        pad_value: float,
+        rows: int,
+        cols: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.crop_and_pad(
             img,
             crop_params,
             pad_params,
             pad_value,
@@ -1060,20 +1051,20 @@
             self.pad_mode,
             self.keep_size,
         )
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        crop_params: Optional[Sequence[int]] = None,
-        pad_params: Optional[Sequence[int]] = None,
-        pad_value_mask: Optional[float] = None,
-        rows: int = 0,
-        cols: int = 0,
-        interpolation: int = cv2.INTER_NEAREST,
+        crop_params: Sequence[int],
+        pad_params: Sequence[int],
+        pad_value_mask: float,
+        rows: int,
+        cols: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.crop_and_pad(
             mask,
             crop_params,
             pad_params,
             pad_value_mask,
@@ -1083,33 +1074,33 @@
             self.pad_mode,
             self.keep_size,
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        crop_params: Optional[Sequence[int]] = None,
-        pad_params: Optional[Sequence[int]] = None,
-        rows: int = 0,
-        cols: int = 0,
-        result_rows: int = 0,
-        result_cols: int = 0,
+        crop_params: Sequence[int],
+        pad_params: Sequence[int],
+        rows: int,
+        cols: int,
+        result_rows: int,
+        result_cols: int,
         **params: Any,
     ) -> BoxInternalType:
         return F.crop_and_pad_bbox(bbox, crop_params, pad_params, rows, cols, result_rows, result_cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        crop_params: Optional[Sequence[int]] = None,
-        pad_params: Optional[Sequence[int]] = None,
-        rows: int = 0,
-        cols: int = 0,
-        result_rows: int = 0,
-        result_cols: int = 0,
+        crop_params: Sequence[int],
+        pad_params: Sequence[int],
+        rows: int,
+        cols: int,
+        result_rows: int,
+        result_cols: int,
         **params: Any,
     ) -> KeypointInternalType:
         return F.crop_and_pad_keypoint(
             keypoint,
             crop_params,
             pad_params,
             rows,
@@ -1265,33 +1256,33 @@
             "keep_size",
             "sample_independently",
             "interpolation",
         )
 
 
 class RandomCropFromBorders(DualTransform):
-    """Crop bbox from image randomly cut parts from borders without resize at the end
+    """Randomly crops parts of the image from the borders without resizing at the end. The cropped regions are defined
+    as fractions of the original image dimensions, specified for each side of the image (left, right, top, bottom).
 
     Args:
-        crop_left (float): single float value in (0.0, 1.0) range. Default 0.1. Image will be randomly cut
-        from left side in range [0, crop_left * width)
-        crop_right (float): single float value in (0.0, 1.0) range. Default 0.1. Image will be randomly cut
-        from right side in range [(1 - crop_right) * width, width)
-        crop_top (float): singlefloat value in (0.0, 1.0) range. Default 0.1. Image will be randomly cut
-        from top side in range [0, crop_top * height)
-        crop_bottom (float): single float value in (0.0, 1.0) range. Default 0.1. Image will be randomly cut
-        from bottom side in range [(1 - crop_bottom) * height, height)
-        p (float): probability of applying the transform. Default: 1.
+        crop_left (float): Fraction of the width to randomly crop from the left side. Must be in the range [0.0, 1.0].
+                            Default is 0.1.
+        crop_right (float): Fraction of the width to randomly crop from the right side. Must be in the range [0.0, 1.0].
+                            Default is 0.1.
+        crop_top (float): Fraction of the height to randomly crop from the top side. Must be in the range [0.0, 1.0].
+                          Default is 0.1.
+        crop_bottom (float): Fraction of the height to randomly crop from the bottom side.
+                             Must be in the range [0.0, 1.0]. Default is 0.1.
+        p (float): Probability of applying the transform. Default is 1.
 
     Targets:
         image, mask, bboxes, keypoints
 
     Image types:
         uint8, float32
-
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     class InitSchema(BaseTransformInitSchema):
         crop_left: float = Field(
             default=0.1,
@@ -1317,19 +1308,19 @@
             le=1.0,
             description="Fraction of height to randomly crop from the bottom side.",
         )
         p: ProbabilityType = 1
 
         @model_validator(mode="after")
         def validate_crop_values(self) -> Self:
-            if self.crop_left + self.crop_right >= 1.0:
-                msg = "The sum of crop_left and crop_right must be less than 1."
+            if self.crop_left + self.crop_right > 1.0:
+                msg = "The sum of crop_left and crop_right must be <= 1."
                 raise ValueError(msg)
-            if self.crop_top + self.crop_bottom >= 1.0:
-                msg = "The sum of crop_top and crop_bottom must be less than 1."
+            if self.crop_top + self.crop_bottom > 1.0:
+                msg = "The sum of crop_top and crop_bottom must be <= 1."
                 raise ValueError(msg)
             return self
 
     def __init__(
         self,
         crop_left: float = 0.1,
         crop_right: float = 0.1,
@@ -1341,62 +1332,65 @@
         super().__init__(always_apply, p)
         self.crop_left = crop_left
         self.crop_right = crop_right
         self.crop_top = crop_top
         self.crop_bottom = crop_bottom
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, int]:
-        img = params["image"]
-        x_min = random_utils.randint(0, int(self.crop_left * img.shape[1]))
-        x_max = random_utils.randint(max(x_min + 1, int((1 - self.crop_right) * img.shape[1])), img.shape[1])
-        y_min = random_utils.randint(0, int(self.crop_top * img.shape[0]))
-        y_max = random_utils.randint(max(y_min + 1, int((1 - self.crop_bottom) * img.shape[0])), img.shape[0])
+        height, width = params["image"].shape[:2]
+
+        x_min = random_utils.randint(0, int(self.crop_left * width) + 1)
+        x_max = random_utils.randint(max(x_min + 1, int((1 - self.crop_right) * width)), width + 1)
+
+        y_min = random_utils.randint(0, int(self.crop_top * height) + 1)
+        y_max = random_utils.randint(max(y_min + 1, int((1 - self.crop_bottom) * height)), height + 1)
+
         return {"x_min": x_min, "x_max": x_max, "y_min": y_min, "y_max": y_max}
 
     def apply(
         self,
         img: np.ndarray,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> np.ndarray:
         return F.clamping_crop(img, x_min, y_min, x_max, y_max)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> np.ndarray:
         return F.clamping_crop(mask, x_min, y_min, x_max, y_max)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         return F.bbox_crop(bbox, x_min, y_min, x_max, y_max, rows, cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        x_min: int = 0,
-        x_max: int = 0,
-        y_min: int = 0,
-        y_max: int = 0,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> KeypointInternalType:
         return F.crop_keypoint_by_coords(keypoint, crop_coords=(x_min, y_min, x_max, y_max))
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/domain_adaptation.py` & `albumentations-1.4.6/albumentations/augmentations/domain_adaptation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Tuple, cast
+from typing import Any, Callable, Dict, List, Literal, Sequence, Tuple, cast
 
 import cv2
 import numpy as np
 from pydantic import field_validator
 
 from albumentations.augmentations.domain_adaptation_functional import (
     adapt_pixel_distribution,
@@ -90,16 +90,16 @@
         self.reference_images = reference_images
         self.read_fn = read_fn
         self.blend_ratio = blend_ratio
 
     def apply(
         self: np.ndarray,
         img: np.ndarray,
-        reference_image: Optional[np.ndarray] = None,
-        blend_ratio: float = 0.5,
+        reference_image: np.ndarray,
+        blend_ratio: float,
         **params: Any,
     ) -> np.ndarray:
         return apply_histogram(img, reference_image, blend_ratio)
 
     def get_params(self) -> Dict[str, np.ndarray]:
         return {
             "reference_image": self.read_fn(random.choice(self.reference_images)),
@@ -189,16 +189,16 @@
         self.reference_images = reference_images
         self.read_fn = read_fn
         self.beta_limit = cast(Tuple[float, float], beta_limit)
 
     def apply(
         self,
         img: np.ndarray,
-        target_image: Optional[np.ndarray] = None,
-        beta: float = 0.1,
+        target_image: np.ndarray,
+        beta: float,
         **params: Any,
     ) -> np.ndarray:
         return fourier_domain_adaptation(img, target_image, beta)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
         img = params["image"]
         target_img = self.read_fn(random.choice(self.reference_images))
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/domain_adaptation_functional.py` & `albumentations-1.4.6/albumentations/augmentations/domain_adaptation_functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 from typing_extensions import Protocol
 
 from albumentations.augmentations.utils import (
     clipped,
     get_opencv_dtype_from_numpy,
-    preserve_shape,
+    preserve_channel_dim,
 )
 
 GRAYSCALE_IMAGE_SHAPE = 2
 NON_GRAY_IMAGE_SHAPE = 3
 RGB_NUM_CHANNELS = 3
 
 __all__ = [
@@ -86,15 +86,15 @@
             self.target_transformer.components_ *= -1
 
         representation = self.source_transformer.transform(pixels)
         result = self.target_transformer.inverse_transform(representation)
         return self.reconstruct(result, height, width)
 
 
-@preserve_shape
+@preserve_channel_dim
 def adapt_pixel_distribution(
     img: np.ndarray,
     ref: np.ndarray,
     transform_type: str = "pca",
     weight: float = 0.5,
 ) -> np.ndarray:
     initial_type = img.dtype
@@ -111,15 +111,15 @@
     h1, h2 = max(0, center_y - border), min(center_y + border, height - 1)
     w1, w2 = max(0, center_h - border), min(center_h + border, width - 1)
     amp_src[h1:h2, w1:w2] = amp_trg[h1:h2, w1:w2]
     return amp_src
 
 
 @clipped
-@preserve_shape
+@preserve_channel_dim
 def fourier_domain_adaptation(img: np.ndarray, target_img: np.ndarray, beta: float) -> np.ndarray:
     src_img = img.astype(np.float32)
     trg_img = target_img.astype(np.float32)
 
     if len(src_img.shape) == GRAYSCALE_IMAGE_SHAPE:
         src_img = np.expand_dims(src_img, axis=-1)
     if len(trg_img.shape) == GRAYSCALE_IMAGE_SHAPE:
@@ -155,15 +155,15 @@
 
         # Store the result in the corresponding channel of the output image
         src_in_trg[:, :, channel_id] = np.real(src_in_trg_channel)
 
     return src_in_trg
 
 
-@preserve_shape
+@preserve_channel_dim
 def apply_histogram(img: np.ndarray, reference_image: np.ndarray, blend_ratio: float) -> np.ndarray:
     # Resize reference image only if necessary
     if img.shape[:2] != reference_image.shape[:2]:
         reference_image = cv2.resize(reference_image, dsize=(img.shape[1], img.shape[0]))
 
     img, reference_image = np.squeeze(img), np.squeeze(reference_image)
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/dropout/channel_dropout.py` & `albumentations-1.4.6/albumentations/augmentations/dropout/channel_dropout.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
         self.channel_drop_range = channel_drop_range
         self.fill_value = fill_value
 
-    def apply(self, img: np.ndarray, channels_to_drop: Tuple[int, ...] = (0,), **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, channels_to_drop: Tuple[int, ...], **params: Any) -> np.ndarray:
         return channel_dropout(img, channels_to_drop, self.fill_value)
 
     def get_params_dependent_on_targets(self, params: Mapping[str, Any]) -> Dict[str, Any]:
         img = params["image"]
         num_channels = img.shape[-1]
 
         if is_grayscale_image(img):
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/dropout/grid_dropout.py` & `albumentations-1.4.6/albumentations/augmentations/dropout/grid_dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,21 @@
         self.holes_number_y = holes_number_y
         self.shift_x = shift_x
         self.shift_y = shift_y
         self.random_offset = random_offset
         self.fill_value = fill_value
         self.mask_fill_value = mask_fill_value
 
-    def apply(self, img: np.ndarray, holes: Iterable[Tuple[int, int, int, int]] = (), **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, holes: Iterable[Tuple[int, int, int, int]], **params: Any) -> np.ndarray:
         return F.cutout(img, holes, self.fill_value)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        holes: Iterable[Tuple[int, int, int, int]] = (),
+        holes: Iterable[Tuple[int, int, int, int]],
         **params: Any,
     ) -> np.ndarray:
         if self.mask_fill_value is None:
             return mask
 
         return F.cutout(mask, holes, self.mask_fill_value)
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/dropout/mask_dropout.py` & `albumentations-1.4.6/albumentations/augmentations/dropout/mask_dropout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Tuple, Union, cast
 
 import cv2
 import numpy as np
 from pydantic import Field
 from skimage.measure import label
 from typing_extensions import Literal
 
@@ -88,30 +88,30 @@
                 for label_index in labels_index:
                     dropout_mask |= label_image == label_index
 
         params.update({"dropout_mask": dropout_mask})
         del params["mask"]
         return params
 
-    def apply(self, img: np.ndarray, dropout_mask: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, dropout_mask: np.ndarray, **params: Any) -> np.ndarray:
         if dropout_mask is None:
             return img
 
         if self.image_fill_value == "inpaint":
             dropout_mask = dropout_mask.astype(np.uint8)
             _, _, width, height = cv2.boundingRect(dropout_mask)
             radius = min(3, max(width, height) // 2)
             return cv2.inpaint(img, dropout_mask, radius, cv2.INPAINT_NS)
 
         img = img.copy()
         img[dropout_mask] = self.image_fill_value
 
         return img
 
-    def apply_to_mask(self, mask: np.ndarray, dropout_mask: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply_to_mask(self, mask: np.ndarray, dropout_mask: np.ndarray, **params: Any) -> np.ndarray:
         if dropout_mask is None:
             return mask
 
         mask = mask.copy()
         mask[dropout_mask] = self.mask_fill_value
         return mask
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/dropout/xy_masking.py` & `albumentations-1.4.6/albumentations/augmentations/dropout/xy_masking.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/augmentations/functional.py` & `albumentations-1.4.6/albumentations/augmentations/functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     clip,
     clipped,
     ensure_contiguous,
     is_grayscale_image,
     is_rgb_image,
     non_rgb_warning,
     preserve_channel_dim,
-    preserve_shape,
 )
 from albumentations.core.types import (
     ColorType,
     ImageMode,
     ScalarType,
     SpatterMode,
 )
@@ -100,15 +99,15 @@
 def normalize_numpy(img: np.ndarray, mean: np.ndarray, denominator: np.ndarray) -> np.ndarray:
     img = img.astype(np.float32)
     img -= mean
     img *= denominator
     return img
 
 
-@preserve_shape
+@preserve_channel_dim
 def normalize(img: np.ndarray, mean: ColorType, std: ColorType, max_pixel_value: float = 255.0) -> np.ndarray:
     mean_np = np.array(mean, dtype=np.float32)
     mean_np *= max_pixel_value
 
     std_np = np.array(std, dtype=np.float32)
     std_np *= max_pixel_value
 
@@ -116,15 +115,15 @@
 
     if is_rgb_image(img):
         return normalize_cv2(img, mean_np, denominator)
 
     return normalize_numpy(img, mean_np, denominator)
 
 
-@preserve_shape
+@preserve_channel_dim
 def normalize_per_image(
     img: np.ndarray,
     normalization: Literal["image", "image_per_channel", "min_max", "min_max_per_channel"],
 ) -> np.ndarray:
     """Apply per-image normalization based on the specified strategy.
 
     Args:
@@ -224,15 +223,15 @@
     if val_shift != 0:
         val = clip(cv2.add(val, val_shift), dtype, 1.0)
 
     img = cv2.merge((hue, sat, val))
     return cv2.cvtColor(img, cv2.COLOR_HSV2RGB)
 
 
-@preserve_shape
+@preserve_channel_dim
 def shift_hsv(img: np.ndarray, hue_shift: np.ndarray, sat_shift: np.ndarray, val_shift: np.ndarray) -> np.ndarray:
     if hue_shift == 0 and sat_shift == 0 and val_shift == 0:
         return img
 
     is_gray = is_grayscale_image(img)
     if is_gray:
         if hue_shift != 0 or sat_shift != 0:
@@ -281,15 +280,15 @@
 
     result_img = img.copy()
     cond = img >= threshold
     result_img[cond] = max_val - result_img[cond]
     return result_img
 
 
-@preserve_shape
+@preserve_channel_dim
 def posterize(img: np.ndarray, bits: int) -> np.ndarray:
     """Reduce the number of bits for each color channel.
 
     Args:
         img: image to posterize.
         bits: number of high bits. Must be in range [0, 8]
 
@@ -437,15 +436,15 @@
     for i in range(3):
         _mask = _handle_mask(mask, img, by_channels, i)
         result_img[..., i] = function(img[..., i], _mask)
 
     return result_img
 
 
-@preserve_shape
+@preserve_channel_dim
 def move_tone_curve(img: np.ndarray, low_y: float, high_y: float) -> np.ndarray:
     """Rescales the relationship between bright and dark areas of the image by manipulating its tone curve.
 
     Args:
         img: RGB or grayscale image.
         low_y: y-position of a Bezier control point used
             to adjust the tone curve, must be in range [0, 1]
@@ -497,15 +496,15 @@
     lut = np.arange(0, max_value + 1).astype("float32")
     lut += value
 
     lut = np.clip(lut, 0, max_value).astype(img.dtype)
     return cv2.LUT(img, lut)
 
 
-@preserve_shape
+@preserve_channel_dim
 def _shift_rgb_uint8(img: np.ndarray, r_shift: ScalarType, g_shift: ScalarType, b_shift: ScalarType) -> np.ndarray:
     if r_shift == g_shift == b_shift:
         height, width, channels = img.shape
         img = img.reshape([height, width * channels])
 
         return _shift_image_uint8(img, r_shift)
 
@@ -541,23 +540,23 @@
         return clahe_mat.apply(img)
 
     img = cv2.cvtColor(img, cv2.COLOR_RGB2LAB)
     img[:, :, 0] = clahe_mat.apply(img[:, :, 0])
     return cv2.cvtColor(img, cv2.COLOR_LAB2RGB)
 
 
-@preserve_shape
+@preserve_channel_dim
 def convolve(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
     conv_fn = _maybe_process_in_chunks(cv2.filter2D, ddepth=-1, kernel=kernel)
     return conv_fn(img)
 
 
-@preserve_shape
-def image_compression(img: np.ndarray, quality: int, image_type: np.dtype) -> np.ndarray:
-    if image_type in [".jpeg", ".jpg"]:
+@preserve_channel_dim
+def image_compression(img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp", ".jpeg"]) -> np.ndarray:
+    if image_type in {".jpeg", ".jpg"}:
         quality_flag = cv2.IMWRITE_JPEG_QUALITY
     elif image_type == ".webp":
         quality_flag = cv2.IMWRITE_WEBP_QUALITY
     else:
         NotImplementedError("Only '.jpg' and '.webp' compression transforms are implemented. ")
 
     input_dtype = img.dtype
@@ -579,15 +578,15 @@
     img = cv2.imdecode(encoded_img, cv2.IMREAD_UNCHANGED)
 
     if needs_float:
         img = to_float(img, max_value=255)
     return img
 
 
-@preserve_shape
+@preserve_channel_dim
 def add_snow(img: np.ndarray, snow_point: float, brightness_coeff: float) -> np.ndarray:
     """Bleaches out pixels, imitation snow.
 
     From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
 
     Args:
         img: Image.
@@ -625,15 +624,15 @@
 
     if needs_float:
         image_rgb = to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
-@preserve_shape
+@preserve_channel_dim
 def add_rain(
     img: np.ndarray,
     slant: int,
     drop_length: int,
     drop_width: int,
     drop_color: Tuple[int, int, int],
     blur_value: int,
@@ -689,15 +688,15 @@
 
     if needs_float:
         return to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
-@preserve_shape
+@preserve_channel_dim
 def add_fog(img: np.ndarray, fog_coef: float, alpha_coef: float, haze_list: List[Tuple[int, int]]) -> np.ndarray:
     """Add fog to the image.
 
     From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
 
     Args:
         img: Image.
@@ -740,15 +739,15 @@
 
     if needs_float:
         image_rgb = to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
-@preserve_shape
+@preserve_channel_dim
 def add_sun_flare(
     img: np.ndarray,
     flare_center_x: float,
     flare_center_y: float,
     src_radius: int,
     src_color: ColorType,
     circles: List[Any],
@@ -804,15 +803,15 @@
     if needs_float:
         image_rgb = to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
 @ensure_contiguous
-@preserve_shape
+@preserve_channel_dim
 def add_shadow(img: np.ndarray, vertices_list: List[np.ndarray]) -> np.ndarray:
     """Add shadows to the image.
 
     Args:
         img (numpy.ndarray):
         vertices_list (list[numpy.ndarray]):
 
@@ -847,15 +846,15 @@
     if needs_float:
         return to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
 @ensure_contiguous
-@preserve_shape
+@preserve_channel_dim
 def add_gravel(img: np.ndarray, gravels: List[Any]) -> np.ndarray:
     """Add gravel to the image.
 
     From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
 
     Args:
         img (numpy.ndarray): image to add gravel to
@@ -896,15 +895,15 @@
     return MAX_VALUES_BY_DTYPE[img.dtype] - img
 
 
 def channel_shuffle(img: np.ndarray, channels_shuffled: np.ndarray) -> np.ndarray:
     return img[..., channels_shuffled]
 
 
-@preserve_shape
+@preserve_channel_dim
 def gamma_transform(img: np.ndarray, gamma: float) -> np.ndarray:
     if img.dtype == np.uint8:
         table = (np.arange(0, 256.0 / 255, 1.0 / 255) ** gamma) * 255
         return cv2.LUT(img, table.astype(np.uint8))
     return np.power(img, gamma)
 
 
@@ -931,15 +930,15 @@
             max_value = MAX_VALUES_BY_DTYPE[dtype]
             img += beta * max_value
         else:
             img += beta * np.mean(img)
     return img
 
 
-@preserve_shape
+@preserve_channel_dim
 def _brightness_contrast_adjust_uint(
     img: np.ndarray,
     alpha: float = 1,
     beta: float = 0,
     beta_by_max: bool = False,
 ) -> np.ndarray:
     dtype = np.dtype("uint8")
@@ -1025,15 +1024,15 @@
     return cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)
 
 
 def gray_to_rgb(img: np.ndarray) -> np.ndarray:
     return cv2.cvtColor(img, cv2.COLOR_GRAY2RGB)
 
 
-@preserve_shape
+@preserve_channel_dim
 def downscale(
     img: np.ndarray,
     scale: float,
     down_interpolation: int = cv2.INTER_AREA,
     up_interpolation: int = cv2.INTER_LINEAR,
 ) -> np.ndarray:
     height, width = img.shape[:2]
@@ -1103,15 +1102,15 @@
 
 @clipped
 def _multiply_uint8(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
     img = img.astype(np.float32)
     return np.multiply(img, multiplier)
 
 
-@preserve_shape
+@preserve_channel_dim
 def _multiply_uint8_optimized(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
     if is_grayscale_image(img) or len(multiplier) == 1:
         multiplier = multiplier[0]
         lut = np.arange(0, 256, dtype=np.float32)
         lut *= multiplier
         lut = clip(lut, np.uint8, MAX_VALUES_BY_DTYPE[img.dtype])
         func = _maybe_process_in_chunks(cv2.LUT, lut=lut)
@@ -1259,15 +1258,15 @@
 
 def _adjust_brightness_torchvision_uint8(img: np.ndarray, factor: float) -> np.ndarray:
     lut = np.arange(0, 256) * factor
     lut = np.clip(lut, 0, 255).astype(np.uint8)
     return cv2.LUT(img, lut)
 
 
-@preserve_shape
+@preserve_channel_dim
 def adjust_brightness_torchvision(img: np.ndarray, factor: np.ndarray) -> np:
     if factor == 0:
         return np.zeros_like(img)
     if factor == 1:
         return img
 
     if img.dtype == np.uint8:
@@ -1280,15 +1279,15 @@
     lut = np.arange(0, 256) * factor
     lut = lut + mean * (1 - factor)
     lut = clip(lut, img.dtype, 255)
 
     return cv2.LUT(img, lut)
 
 
-@preserve_shape
+@preserve_channel_dim
 def adjust_contrast_torchvision(img: np.ndarray, factor: float) -> np.ndarray:
     if factor == 1:
         return img
 
     mean = img.mean() if is_grayscale_image(img) else cv2.cvtColor(img, cv2.COLOR_RGB2GRAY).mean()
 
     if factor == 0:
@@ -1302,15 +1301,15 @@
     return clip(
         img.astype(np.float32) * factor + mean * (1 - factor),
         img.dtype,
         MAX_VALUES_BY_DTYPE[img.dtype],
     )
 
 
-@preserve_shape
+@preserve_channel_dim
 def adjust_saturation_torchvision(img: np.ndarray, factor: float, gamma: float = 0) -> np.ndarray:
     if factor == 1:
         return img
 
     if is_grayscale_image(img):
         return img
 
@@ -1349,15 +1348,15 @@
         return _adjust_hue_torchvision_uint8(img, factor)
 
     img = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
     img[..., 0] = np.mod(img[..., 0] + factor * 360, 360)
     return cv2.cvtColor(img, cv2.COLOR_HSV2RGB)
 
 
-@preserve_shape
+@preserve_channel_dim
 def superpixels(
     image: np.ndarray,
     n_segments: int,
     replace_samples: Sequence[bool],
     max_size: Optional[int],
     interpolation: int,
 ) -> np.ndarray:
@@ -1417,22 +1416,22 @@
         )
         return resize_fn(image)
 
     return image
 
 
 @clipped
-@preserve_shape
+@preserve_channel_dim
 def add_weighted(img1: np.ndarray, alpha: float, img2: np.ndarray, beta: float) -> np.ndarray:
     img2 = img2.reshape(img1.shape).astype(img1.dtype)
     return cv2.addWeighted(img1, alpha, img2, beta, 0)
 
 
 @clipped
-@preserve_shape
+@preserve_channel_dim
 def unsharp_mask(
     image: np.ndarray,
     ksize: int,
     sigma: float = 0.0,
     alpha: float = 0.2,
     threshold: int = 10,
 ) -> np.ndarray:
@@ -1456,25 +1455,25 @@
     sharp = np.clip(sharp, 0, 1)
 
     soft_mask = blur_fn(mask)
     output = soft_mask * sharp + (1 - soft_mask) * image
     return from_float(output, dtype=input_dtype)
 
 
-@preserve_shape
+@preserve_channel_dim
 def pixel_dropout(image: np.ndarray, drop_mask: np.ndarray, drop_value: Union[float, Sequence[float]]) -> np.ndarray:
     if isinstance(drop_value, (int, float)) and drop_value == 0:
         drop_values = np.zeros_like(image)
     else:
         drop_values = np.full_like(image, drop_value)
     return np.where(drop_mask, drop_values, image)
 
 
 @clipped
-@preserve_shape
+@preserve_channel_dim
 def spatter(
     img: np.ndarray,
     non_mud: Optional[np.ndarray],
     mud: Optional[np.ndarray],
     rain: Optional[np.ndarray],
     mode: SpatterMode,
 ) -> np.ndarray:
@@ -1680,20 +1679,20 @@
         map_x,
         map_y,
         interpolation=interpolation,
         borderMode=cv2.BORDER_REPLICATE,
     )
 
 
-@preserve_shape
+@preserve_channel_dim
 def erode(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
     return cv2.erode(img, kernel, iterations=1)
 
 
-@preserve_shape
+@preserve_channel_dim
 def dilate(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
     return cv2.dilate(img, kernel, iterations=1)
 
 
 def morphology(img: np.ndarray, kernel: np.ndarray, operation: str) -> np.ndarray:
     if operation == "dilation":
         return dilate(img, kernel)
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/geometric/functional.py` & `albumentations-1.4.6/albumentations/augmentations/geometric/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from albumentations import random_utils
 from albumentations.augmentations.utils import (
     _maybe_process_in_chunks,
     angle_2pi_range,
     clipped,
     preserve_channel_dim,
-    preserve_shape,
 )
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
 from albumentations.core.types import BoxInternalType, ColorType, D4Type, KeypointInternalType
 
 __all__ = [
     "optical_distortion",
     "elastic_transform_approx",
@@ -151,34 +150,33 @@
 def keypoint_rot90(
     keypoint: KeypointInternalType,
     factor: int,
     rows: int,
     cols: int,
     **params: Any,
 ) -> KeypointInternalType:
-    """Rotates a keypoint by 90 degrees CCW (see np.rot90)
+    """Rotates a keypoint by 90 degrees CCW
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
         factor: Number of CCW rotations. Must be in range [0;3] See np.rot90.
         rows: Image height.
         cols: Image width.
 
     Returns:
         tuple: A keypoint `(x, y, angle, scale)`.
 
     Raises:
         ValueError: if factor not in set {0, 1, 2, 3}
 
     """
-    x, y, angle, scale = keypoint[:4]
+    x, y, angle, scale = keypoint
 
     if factor not in {0, 1, 2, 3}:
-        msg = "Parameter n must be in set {0, 1, 2, 3}"
-        raise ValueError(msg)
+        raise ValueError("Parameter factor must be in set {0, 1, 2, 3}")
 
     if factor == 1:
         x, y, angle = y, (cols - 1) - x, angle - math.pi / 2
     elif factor == ROT90_180_FACTOR:
         x, y, angle = (cols - 1) - x, (rows - 1) - y, angle - math.pi
     elif factor == ROT90_270_FACTOR:
         x, y, angle = (rows - 1) - y, x, angle + math.pi / 2
@@ -326,15 +324,15 @@
     center = (cols - 1) * 0.5, (rows - 1) * 0.5
     matrix = cv2.getRotationMatrix2D(center, angle, 1.0)
     x, y, a, s = keypoint[:4]
     x, y = cv2.transform(np.array([[[x, y]]]), matrix).squeeze()
     return x, y, a + math.radians(angle), s
 
 
-@preserve_shape
+@preserve_channel_dim
 def elastic_transform(
     img: np.ndarray,
     alpha: float,
     sigma: float,
     alpha_affine: float,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
@@ -423,15 +421,15 @@
     )
     return remap_fn(img)
 
 
 @preserve_channel_dim
 def resize(img: np.ndarray, height: int, width: int, interpolation: int = cv2.INTER_LINEAR) -> np.ndarray:
     img_height, img_width = img.shape[:2]
-    if height == img_height and width == img_width:
+    if (height, width) == img.shape[:2]:
         return img
     resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(width, height), interpolation=interpolation)
     return resize_fn(img)
 
 
 @preserve_channel_dim
 def scale(img: np.ndarray, scale: float, interpolation: int = cv2.INTER_LINEAR) -> np.ndarray:
@@ -911,15 +909,14 @@
     return np.ascontiguousarray(img[:, ::-1, ...])
 
 
 def hflip_cv2(img: np.ndarray) -> np.ndarray:
     return cv2.flip(img, 1)
 
 
-@preserve_shape
 def d4(img: np.ndarray, group_member: D4Type) -> np.ndarray:
     """Applies a `D_4` symmetry group transformation to an image array.
 
     This function manipulates an image using transformations such as rotations and flips,
     corresponding to the `D_4` dihedral group symmetry operations.
     Each transformation is identified by a unique group member code.
 
@@ -961,15 +958,15 @@
     # Execute the appropriate transformation
     if group_member in transformations:
         return np.ascontiguousarray(transformations[group_member](img))
 
     raise ValueError(f"Invalid group member: {group_member}")
 
 
-@preserve_shape
+@preserve_channel_dim
 def random_flip(img: np.ndarray, code: int) -> np.ndarray:
     return cv2.flip(img, code)
 
 
 def transpose(img: np.ndarray) -> np.ndarray:
     """Transposes the first two dimensions of an array of any dimensionality.
     Retains the order of any additional dimensions.
@@ -1138,15 +1135,15 @@
     else:
         raise ValueError(f"Invalid d value {d}. Valid values are -1, 0 and 1")
     return keypoint
 
 
 @angle_2pi_range
 def keypoint_transpose(keypoint: KeypointInternalType, rows: int, cols: int) -> KeypointInternalType:
-    """Transposes a keypoint along a specified axis: main diagonal (0) or secondary diagonal (1).
+    """Transposes a keypoint along a specified axis: main diagonal
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
         rows: Total number of rows (height) in the image.
         cols: Total number of columns (width) in the image.
 
     Returns:
@@ -1218,15 +1215,15 @@
         right=w_pad_right,
         borderType=border_mode,
         value=value,
     )
     return pad_fn(img)
 
 
-@preserve_shape
+@preserve_channel_dim
 def optical_distortion(
     img: np.ndarray,
     k: int = 0,
     dx: int = 0,
     dy: int = 0,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
@@ -1251,29 +1248,24 @@
     camera_matrix = np.array([[fx, 0, cx], [0, fy, cy], [0, 0, 1]], dtype=np.float32)
 
     distortion = np.array([k, k, 0, 0, 0], dtype=np.float32)
     map1, map2 = cv2.initUndistortRectifyMap(camera_matrix, distortion, None, None, (width, height), cv2.CV_32FC1)
     return cv2.remap(img, map1, map2, interpolation=interpolation, borderMode=border_mode, borderValue=value)
 
 
-@preserve_shape
+@preserve_channel_dim
 def grid_distortion(
     img: np.ndarray,
     num_steps: int = 10,
     xsteps: Tuple[()] = (),
     ysteps: Tuple[()] = (),
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
     value: Optional[ColorType] = None,
 ) -> np.ndarray:
-    """Perform a grid distortion of an input image.
-
-    Reference:
-        http://pythology.blogspot.sg/2014/03/interpolation-on-regular-distorted-grid.html
-    """
     height, width = img.shape[:2]
 
     x_step = width // num_steps
     xx = np.zeros(width, np.float32)
     prev = 0
     for idx in range(num_steps + 1):
         x = idx * x_step
@@ -1315,15 +1307,15 @@
         interpolation=interpolation,
         borderMode=border_mode,
         borderValue=value,
     )
     return remap_fn(img)
 
 
-@preserve_shape
+@preserve_channel_dim
 def elastic_transform_approx(
     img: np.ndarray,
     alpha: float,
     sigma: float,
     alpha_affine: float,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/geometric/resize.py` & `albumentations-1.4.6/albumentations/augmentations/geometric/resize.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,28 +68,28 @@
 
     def get_params(self) -> Dict[str, float]:
         return {"scale": random.uniform(self.scale_limit[0], self.scale_limit[1])}
 
     def apply(
         self,
         img: np.ndarray,
-        scale: float = 0,
-        interpolation: int = cv2.INTER_LINEAR,
+        scale: float,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.scale(img, scale, interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         # Bounding box coordinates are scale invariant
         return bbox
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        scale: float = 0,
+        scale: float,
         **params: Any,
     ) -> KeypointInternalType:
         return F.keypoint_scale(keypoint, scale, scale)
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {"interpolation": self.interpolation, "scale_limit": to_tuple(self.scale_limit, bias=-1.0)}
 
@@ -145,28 +145,28 @@
         super().__init__(always_apply, p)
         self.interpolation = interpolation
         self.max_size = max_size
 
     def apply(
         self,
         img: np.ndarray,
-        max_size: int = 1024,
-        interpolation: int = cv2.INTER_LINEAR,
+        max_size: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.longest_max_size(img, max_size=max_size, interpolation=interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         # Bounding box coordinates are scale invariant
         return bbox
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        max_size: int = 1024,
+        max_size: int,
         **params: Any,
     ) -> KeypointInternalType:
         height = params["rows"]
         width = params["cols"]
 
         scale = max_size / max([height, width])
         return F.keypoint_scale(keypoint, scale, scale)
@@ -210,27 +210,27 @@
         super().__init__(always_apply, p)
         self.interpolation = interpolation
         self.max_size = max_size
 
     def apply(
         self,
         img: np.ndarray,
-        max_size: int = 1024,
-        interpolation: int = cv2.INTER_LINEAR,
+        max_size: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.smallest_max_size(img, max_size=max_size, interpolation=interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return bbox
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        max_size: int = 1024,
+        max_size: int,
         **params: Any,
     ) -> KeypointInternalType:
         height = params["rows"]
         width = params["cols"]
 
         scale = max_size / min([height, width])
         return F.keypoint_scale(keypoint, scale, scale)
@@ -278,15 +278,15 @@
         p: float = 1,
     ):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
         self.interpolation = interpolation
 
-    def apply(self, img: np.ndarray, interpolation: int = cv2.INTER_LINEAR, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, interpolation: int, **params: Any) -> np.ndarray:
         return F.resize(img, height=self.height, width=self.width, interpolation=interpolation)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         # Bounding box coordinates are scale invariant
         return bbox
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/geometric/rotate.py` & `albumentations-1.4.6/albumentations/augmentations/geometric/rotate.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,29 +37,29 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
-    def apply(self, img: np.ndarray, factor: float = 0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, factor: float, **params: Any) -> np.ndarray:
         """Args:
         factor (int): number of times the input will be rotated by 90 degrees.
 
         """
         return np.ascontiguousarray(np.rot90(img, factor))
 
     def get_params(self) -> Dict[str, int]:
         # Random int in the range [0, 3]
         return {"factor": random.randint(0, 3)}
 
-    def apply_to_bbox(self, bbox: BoxInternalType, factor: int = 0, **params: Any) -> BoxInternalType:
+    def apply_to_bbox(self, bbox: BoxInternalType, factor: int, **params: Any) -> BoxInternalType:
         return F.bbox_rot90(bbox, factor, **params)
 
-    def apply_to_keypoint(self, keypoint: KeypointInternalType, factor: int = 0, **params: Any) -> BoxInternalType:
+    def apply_to_keypoint(self, keypoint: KeypointInternalType, factor: int, **params: Any) -> BoxInternalType:
         return F.keypoint_rot90(keypoint, factor, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class RotateInitSchema(BaseTransformInitSchema):
@@ -111,15 +111,15 @@
         crop_border: bool = Field(
             default=False,
             description="If True, makes a largest possible crop within the rotated image.",
         )
 
     def __init__(
         self,
-        limit: ScaleFloatType = 90,
+        limit: ScaleFloatType = (-90, 90),
         interpolation: int = cv2.INTER_LINEAR,
         border_mode: int = cv2.BORDER_REFLECT_101,
         value: Optional[ColorType] = None,
         mask_value: Optional[ColorType] = None,
         rotate_method: Literal["largest_box", "ellipse"] = "largest_box",
         crop_border: bool = False,
         always_apply: bool = False,
@@ -133,73 +133,73 @@
         self.mask_value = mask_value
         self.rotate_method = rotate_method
         self.crop_border = crop_border
 
     def apply(
         self,
         img: np.ndarray,
-        angle: float = 0,
-        interpolation: int = cv2.INTER_LINEAR,
-        x_min: Optional[int] = None,
-        x_max: Optional[int] = None,
-        y_min: Optional[int] = None,
-        y_max: Optional[int] = None,
+        angle: float,
+        interpolation: int,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> np.ndarray:
         img_out = F.rotate(img, angle, interpolation, self.border_mode, self.value)
-        if self.crop_border and x_min is not None and x_max is not None and y_min is not None and y_max is not None:
+        if self.crop_border:
             return FCrops.crop(img_out, x_min, y_min, x_max, y_max)
         return img_out
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         angle: float,
-        x_min: Optional[int] = None,
-        x_max: Optional[int] = None,
-        y_min: Optional[int] = None,
-        y_max: Optional[int] = None,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
         **params: Any,
     ) -> np.ndarray:
         img_out = F.rotate(mask, angle, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
-        if self.crop_border and x_min is not None and x_max is not None and y_min is not None and y_max is not None:
+        if self.crop_border:
             return FCrops.crop(img_out, x_min, y_min, x_max, y_max)
         return img_out
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        angle: float = 0,
-        x_min: Optional[int] = None,
-        x_max: Optional[int] = None,
-        y_min: Optional[int] = None,
-        y_max: Optional[int] = None,
-        cols: int = 0,
-        rows: int = 0,
+        angle: float,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
+        cols: int,
+        rows: int,
         **params: Any,
     ) -> np.ndarray:
         bbox_out = F.bbox_rotate(bbox, angle, self.rotate_method, rows, cols)
-        if self.crop_border and x_min is not None and x_max is not None and y_min is not None and y_max is not None:
+        if self.crop_border:
             return FCrops.bbox_crop(bbox_out, x_min, y_min, x_max, y_max, rows, cols)
         return bbox_out
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        angle: float = 0,
-        x_min: Optional[int] = None,
-        x_max: Optional[int] = None,
-        y_min: Optional[int] = None,
-        y_max: Optional[int] = None,
-        cols: int = 0,
-        rows: int = 0,
+        angle: float,
+        x_min: int,
+        x_max: int,
+        y_min: int,
+        y_max: int,
+        cols: int,
+        rows: int,
         **params: Any,
     ) -> KeypointInternalType:
         keypoint_out = F.keypoint_rotate(keypoint, angle, rows, cols, **params)
-        if self.crop_border and x_min is not None and x_max is not None and y_min is not None and y_max is not None:
+        if self.crop_border:
             return FCrops.crop_keypoint_by_coords(keypoint_out, (x_min, y_min, x_max, y_max))
         return keypoint_out
 
     @staticmethod
     def _rotated_rect_with_max_area(height: int, width: int, angle: float) -> Dict[str, int]:
         """Given a rectangle of size wxh that has been rotated by 'angle' (in
         degrees), computes the width and height of the largest possible
@@ -237,14 +237,17 @@
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         out_params = {"angle": random.uniform(self.limit[0], self.limit[1])}
         if self.crop_border:
             height, width = params["image"].shape[:2]
             out_params.update(self._rotated_rect_with_max_area(height, width, out_params["angle"]))
+        else:
+            out_params.update({"x_min": -1, "x_max": -1, "y_min": -1, "y_max": -1})
+
         return out_params
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("limit", "interpolation", "border_mode", "value", "mask_value", "rotate_method", "crop_border")
 
 
 class SafeRotate(DualTransform):
@@ -295,31 +298,31 @@
         super().__init__(always_apply, p)
         self.limit = cast(Tuple[float, float], limit)
         self.interpolation = interpolation
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
 
-    def apply(self, img: np.ndarray, matrix: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
-        return F.safe_rotate(img, matrix, cast(int, self.interpolation), self.value, self.border_mode)
+    def apply(self, img: np.ndarray, matrix: np.ndarray, **params: Any) -> np.ndarray:
+        return F.safe_rotate(img, matrix, self.interpolation, self.value, self.border_mode)
 
-    def apply_to_mask(self, mask: np.ndarray, matrix: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply_to_mask(self, mask: np.ndarray, matrix: np.ndarray, **params: Any) -> np.ndarray:
         return F.safe_rotate(mask, matrix, cv2.INTER_NEAREST, self.mask_value, self.border_mode)
 
-    def apply_to_bbox(self, bbox: BoxInternalType, cols: int = 0, rows: int = 0, **params: Any) -> BoxInternalType:
+    def apply_to_bbox(self, bbox: BoxInternalType, cols: int, rows: int, **params: Any) -> BoxInternalType:
         return F.bbox_safe_rotate(bbox, params["matrix"], cols, rows)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        angle: float = 0,
-        scale_x: float = 0,
-        scale_y: float = 0,
-        cols: int = 0,
-        rows: int = 0,
+        angle: float,
+        scale_x: float,
+        scale_y: float,
+        cols: int,
+        rows: int,
         **params: Any,
     ) -> KeypointInternalType:
         return F.keypoint_safe_rotate(keypoint, params["matrix"], angle, scale_x, scale_y, cols, rows)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
@@ -358,9 +361,9 @@
         _tmp = np.diag(np.ones(3))
         _tmp[:2] = rotation_mat
         _tmp = scale_mat @ _tmp
         rotation_mat = _tmp[:2]
 
         return {"matrix": rotation_mat, "angle": angle, "scale_x": scale_x, "scale_y": scale_y}
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str, str, str]:
-        return ("limit", "interpolation", "border_mode", "value", "mask_value")
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
+        return "limit", "interpolation", "border_mode", "value", "mask_value"
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/geometric/transforms.py` & `albumentations-1.4.6/albumentations/augmentations/geometric/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 import numpy as np
 import skimage.transform
 from pydantic import Field, ValidationInfo, field_validator, model_validator
 from typing_extensions import Annotated, Self
 
 from albumentations import random_utils
 from albumentations.augmentations.functional import bbox_from_mask
-from albumentations.augmentations.utils import BIG_INTEGER, check_range
+from albumentations.augmentations.utils import BIG_INTEGER, check_range, get_num_channels
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
 from albumentations.core.pydantic import (
     BorderModeType,
     InterpolationType,
     NonNegativeFloatRangeType,
     ProbabilityType,
     SymmetricRangeType,
 )
 from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import (
+    NUM_MULTI_CHANNEL_DIMENSIONS,
     BoxInternalType,
     ColorType,
     D4Type,
     KeypointInternalType,
     ScaleFloatType,
     ScaleIntType,
     SizeType,
@@ -50,15 +51,14 @@
     "OpticalDistortion",
     "GridDistortion",
     "PadIfNeeded",
     "D4",
 ]
 
 TWO = 2
-THREE = 3
 
 
 class ElasticTransform(DualTransform):
     """Elastic deformation of images as described in [Simard2003]_ (with modifications).
 
     .. [Simard2003] Simard, Steinkraus and Platt, "Best Practices for
          Convolutional Neural Networks applied to Visual Document Analysis", in
@@ -138,49 +138,49 @@
         self.mask_value = mask_value
         self.approximate = approximate
         self.same_dxdy = same_dxdy
 
     def apply(
         self,
         img: np.ndarray,
-        random_state: Optional[int] = None,
-        interpolation: int = cv2.INTER_LINEAR,
+        random_seed: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.elastic_transform(
             img,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             interpolation,
             self.border_mode,
             self.value,
-            np.random.RandomState(random_state),
+            np.random.RandomState(random_seed),
             self.approximate,
             self.same_dxdy,
         )
 
-    def apply_to_mask(self, mask: np.ndarray, random_state: Optional[int] = None, **params: Any) -> np.ndarray:
+    def apply_to_mask(self, mask: np.ndarray, random_seed: int, **params: Any) -> np.ndarray:
         return F.elastic_transform(
             mask,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             cv2.INTER_NEAREST,
             self.border_mode,
             self.mask_value,
-            np.random.RandomState(random_state),
+            np.random.RandomState(random_seed),
             self.approximate,
             self.same_dxdy,
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        random_state: Optional[int] = None,
+        random_seed: int,
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
         bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
@@ -189,22 +189,22 @@
             mask,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             cv2.INTER_NEAREST,
             self.border_mode,
             self.mask_value,
-            np.random.RandomState(random_state),
+            np.random.RandomState(random_seed),
             self.approximate,
         )
         bbox_returned = bbox_from_mask(mask)
         return cast(BoxInternalType, F.normalize_bbox(bbox_returned, rows, cols))
 
     def get_params(self) -> Dict[str, int]:
-        return {"random_state": random.randint(0, 10000)}
+        return {"random_seed": random_utils.get_random_seed()}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
             "alpha",
             "sigma",
             "alpha_affine",
             "interpolation",
@@ -678,59 +678,59 @@
             raise ValueError(msg)
         # translate by pixels
         return translate_percent, cls._handle_dict_arg(translate_px, "translate_px")
 
     def apply(
         self,
         img: np.ndarray,
-        matrix: skimage.transform.ProjectiveTransform = None,
-        output_shape: Sequence[int] = (),
+        matrix: skimage.transform.ProjectiveTransform,
+        output_shape: Sequence[int],
         **params: Any,
     ) -> np.ndarray:
         return F.warp_affine(
             img,
             matrix,
-            interpolation=cast(int, self.interpolation),
+            interpolation=self.interpolation,
             cval=self.cval,
             mode=self.mode,
             output_shape=output_shape,
         )
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        matrix: skimage.transform.ProjectiveTransform = None,
-        output_shape: Sequence[int] = (),
+        matrix: skimage.transform.ProjectiveTransform,
+        output_shape: Sequence[int],
         **params: Any,
     ) -> np.ndarray:
         return F.warp_affine(
             mask,
             matrix,
             interpolation=self.mask_interpolation,
             cval=self.cval_mask,
             mode=self.mode,
             output_shape=output_shape,
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        matrix: skimage.transform.ProjectiveTransform = None,
-        rows: int = 0,
-        cols: int = 0,
-        output_shape: Sequence[int] = (),
+        matrix: skimage.transform.ProjectiveTransform,
+        rows: int,
+        cols: int,
+        output_shape: Sequence[int],
         **params: Any,
     ) -> BoxInternalType:
         return F.bbox_affine(bbox, matrix, self.rotate_method, rows, cols, output_shape)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        matrix: Optional[skimage.transform.ProjectiveTransform] = None,
-        scale: Optional[Dict[str, Any]] = None,
+        matrix: skimage.transform.ProjectiveTransform,
+        scale: Dict[str, Any],
         **params: Any,
     ) -> KeypointInternalType:
         if scale is None:
             msg = "Expected scale to be provided, but got None."
             raise ValueError(msg)
         if matrix is None:
             msg = "Expected matrix to be provided, but got None."
@@ -815,15 +815,15 @@
         corners = matrix(corners)
         minc = corners[:, 0].min()
         minr = corners[:, 1].min()
         maxc = corners[:, 0].max()
         maxr = corners[:, 1].max()
         out_height = maxr - minr + 1
         out_width = maxc - minc + 1
-        if len(input_shape) == THREE:
+        if len(input_shape) == NUM_MULTI_CHANNEL_DIMENSIONS:
             output_shape = np.ceil((out_height, out_width, input_shape[2]))
         else:
             output_shape = np.ceil((out_height, out_width))
         output_shape_tuple = tuple([int(v) for v in output_shape.tolist()])
         # fit output image in new shape
         translation = (-minc, -minr)
         matrix_to_fit = skimage.transform.SimilarityTransform(translation=translation)
@@ -1149,43 +1149,43 @@
         return {
             "matrix": matrix,
         }
 
     def apply(
         self,
         img: np.ndarray,
-        matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None,
+        matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> np.ndarray:
-        return F.piecewise_affine(img, matrix, cast(int, self.interpolation), self.mode, self.cval)
+        return F.piecewise_affine(img, matrix, self.interpolation, self.mode, self.cval)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None,
+        matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> np.ndarray:
         return F.piecewise_affine(mask, matrix, self.mask_interpolation, self.mode, self.cval_mask)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        rows: int = 0,
-        cols: int = 0,
-        matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None,
+        rows: int,
+        cols: int,
+        matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> BoxInternalType:
         return F.bbox_piecewise_affine(bbox, matrix, rows, cols, self.keypoints_threshold)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        rows: int = 0,
-        cols: int = 0,
-        matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None,
+        rows: int,
+        cols: int,
+        matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> KeypointInternalType:
         return F.keypoint_piecewise_affine(keypoint, matrix, rows, cols, self.keypoints_threshold)
 
 
 class PadIfNeeded(DualTransform):
     """Pad side of the image / max if side is less than desired number.
@@ -1343,18 +1343,18 @@
             },
         )
         return params
 
     def apply(
         self,
         img: np.ndarray,
-        pad_top: int = 0,
-        pad_bottom: int = 0,
-        pad_left: int = 0,
-        pad_right: int = 0,
+        pad_top: int,
+        pad_bottom: int,
+        pad_left: int,
+        pad_right: int,
         **params: Any,
     ) -> np.ndarray:
         return F.pad_with_params(
             img,
             pad_top,
             pad_bottom,
             pad_left,
@@ -1362,18 +1362,18 @@
             border_mode=self.border_mode,
             value=self.value,
         )
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        pad_top: int = 0,
-        pad_bottom: int = 0,
-        pad_left: int = 0,
-        pad_right: int = 0,
+        pad_top: int,
+        pad_bottom: int,
+        pad_left: int,
+        pad_right: int,
         **params: Any,
     ) -> np.ndarray:
         return F.pad_with_params(
             mask,
             pad_top,
             pad_bottom,
             pad_left,
@@ -1381,33 +1381,33 @@
             border_mode=self.border_mode,
             value=self.mask_value,
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        pad_top: int = 0,
-        pad_bottom: int = 0,
-        pad_left: int = 0,
-        pad_right: int = 0,
-        rows: int = 0,
-        cols: int = 0,
+        pad_top: int,
+        pad_bottom: int,
+        pad_left: int,
+        pad_right: int,
+        rows: int,
+        cols: int,
         **params: Any,
     ) -> BoxInternalType:
         x_min, y_min, x_max, y_max = denormalize_bbox(bbox, rows, cols)[:4]
         bbox = x_min + pad_left, y_min + pad_top, x_max + pad_left, y_max + pad_top
         return cast(BoxInternalType, normalize_bbox(bbox, rows + pad_top + pad_bottom, cols + pad_left + pad_right))
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
-        pad_top: int = 0,
-        pad_bottom: int = 0,
-        pad_left: int = 0,
-        pad_right: int = 0,
+        pad_top: int,
+        pad_bottom: int,
+        pad_left: int,
+        pad_right: int,
         **params: Any,
     ) -> KeypointInternalType:
         x, y, angle, scale = keypoint[:4]
         return x + pad_left, y + pad_top, angle, scale
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
@@ -1505,15 +1505,15 @@
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        if img.ndim == THREE and img.shape[2] > 1 and img.dtype == np.uint8:
+        if get_num_channels(img) > 1 and img.dtype == np.uint8:
             # Opencv is faster than numpy only in case of
             # non-gray scale 8bits images
             return F.hflip_cv2(img)
 
         return F.hflip(img)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
@@ -1538,15 +1538,15 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
-    def apply(self, img: np.ndarray, d: int = 0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, d: int, **params: Any) -> np.ndarray:
         """Args:
         d (int): code that specifies how to flip the input. 0 for vertical flipping, 1 for horizontal flipping,
                 -1 for both vertical and horizontal flipping (which is also could be seen as rotating the input by
                 180 degrees).
         """
         return F.random_flip(img, d)
 
@@ -1652,31 +1652,31 @@
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
 
     def apply(
         self,
         img: np.ndarray,
-        k: int = 0,
-        dx: int = 0,
-        dy: int = 0,
-        interpolation: int = cv2.INTER_LINEAR,
+        k: int,
+        dx: int,
+        dy: int,
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.optical_distortion(img, k, dx, dy, interpolation, self.border_mode, self.value)
 
-    def apply_to_mask(self, mask: np.ndarray, k: int = 0, dx: int = 0, dy: int = 0, **params: Any) -> np.ndarray:
+    def apply_to_mask(self, mask: np.ndarray, k: int, dx: int, dy: int, **params: Any) -> np.ndarray:
         return F.optical_distortion(mask, k, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        k: int = 0,
-        dx: int = 0,
-        dy: int = 0,
+        k: int,
+        dx: int,
+        dy: int,
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
         bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
@@ -1700,37 +1700,45 @@
             "border_mode",
             "value",
             "mask_value",
         )
 
 
 class GridDistortion(DualTransform):
-    """Args:
-        num_steps (int): count of grid cells on each side.
-        distort_limit (float, (float, float)): If distort_limit is a single float, the range
-            will be (-distort_limit, distort_limit). Default: (-0.03, 0.03).
-        interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
+    """Applies grid distortion augmentation to images, masks, and bounding boxes. This technique involves dividing
+    the image into a grid of cells and randomly displacing the intersection points of the grid,
+    resulting in localized distortions.
+
+    Args:
+        num_steps (int): Number of grid cells on each side (minimum 1).
+        distort_limit (float, (float, float)): Range of distortion limits. If a single float is provided,
+            the range will be from (-distort_limit, distort_limit). Default: (-0.03, 0.03).
+        interpolation (OpenCV flag): Interpolation algorithm used for image transformation. Options are:
             cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
             Default: cv2.INTER_LINEAR.
-        border_mode (OpenCV flag): flag that is used to specify the pixel extrapolation method. Should be one of:
-            cv2.BORDER_CONSTANT, cv2.BORDER_REPLICATE, cv2.BORDER_REFLECT, cv2.BORDER_WRAP, cv2.BORDER_REFLECT_101.
-            Default: cv2.BORDER_REFLECT_101
-        value (int, float, list of ints, list of float): padding value if border_mode is cv2.BORDER_CONSTANT.
-        mask_value (int, float,
-                    list of ints,
-                    list of float): padding value if border_mode is cv2.BORDER_CONSTANT applied for masks.
-        normalized (bool): if true, distortion will be normalized to do not go outside the image. Default: False
-            See for more information: https://github.com/albumentations-team/albumentations/pull/722
+        border_mode (OpenCV flag): Pixel extrapolation method used when pixels outside the image are required.
+            Options are: cv2.BORDER_CONSTANT, cv2.BORDER_REPLICATE, cv2.BORDER_REFLECT, cv2.BORDER_WRAP,
+            cv2.BORDER_REFLECT_101.
+            Default: cv2.BORDER_REFLECT_101.
+        value (int, float, list of ints, list of floats, optional): Value used for padding when
+            border_mode is cv2.BORDER_CONSTANT.
+        mask_value (int, float, list of ints, list of floats, optional): Padding value for masks when
+            border_mode is cv2.BORDER_CONSTANT.
+        normalized (bool): If True, ensures that distortion does not exceed image boundaries. Default: False.
+            Reference: https://github.com/albumentations-team/albumentations/pull/722
 
     Targets:
         image, mask, bboxes
 
     Image types:
         uint8, float32
 
+    Note:
+        This transform is helpful in medical imagery, Optical Character Recognition, and other tasks where local
+        distance may not be preserved.
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES)
 
     class InitSchema(BaseTransformInitSchema):
         num_steps: Annotated[int, Field(ge=1, description="Count of grid cells on each side.")]
         distort_limit: SymmetricRangeType = (-0.03, 0.03)
@@ -1778,26 +1786,26 @@
         self.value = value
         self.mask_value = mask_value
         self.normalized = normalized
 
     def apply(
         self,
         img: np.ndarray,
-        stepsx: Tuple[()] = (),
-        stepsy: Tuple[()] = (),
-        interpolation: int = cv2.INTER_LINEAR,
+        stepsx: Tuple[()],
+        stepsy: Tuple[()],
+        interpolation: int,
         **params: Any,
     ) -> np.ndarray:
         return F.grid_distortion(img, self.num_steps, stepsx, stepsy, interpolation, self.border_mode, self.value)
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
-        stepsx: Tuple[()] = (),
-        stepsy: Tuple[()] = (),
+        stepsx: Tuple[()],
+        stepsy: Tuple[()],
         **params: Any,
     ) -> np.ndarray:
         return F.grid_distortion(
             mask,
             self.num_steps,
             stepsx,
             stepsy,
@@ -1805,16 +1813,16 @@
             self.border_mode,
             self.mask_value,
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
-        stepsx: Tuple[()] = (),
-        stepsy: Tuple[()] = (),
+        stepsx: Tuple[()],
+        stepsy: Tuple[()],
         **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
         bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/mixing/transforms.py` & `albumentations-1.4.6/albumentations/augmentations/mixing/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/augmentations/transforms.py` & `albumentations-1.4.6/albumentations/augmentations/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,45 +4,50 @@
 import warnings
 from types import LambdaType
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
-from pydantic import Field, ValidationInfo, field_validator, model_validator
+from pydantic import AfterValidator, BaseModel, Field, ValidationInfo, field_validator, model_validator
 from scipy import special
 from scipy.ndimage import gaussian_filter
-from typing_extensions import Annotated, Literal, Self
+from typing_extensions import Annotated, Literal, Self, TypedDict
 
 from albumentations import random_utils
 from albumentations.augmentations.blur.functional import blur
 from albumentations.augmentations.blur.transforms import BlurInitSchema, process_blur_limit
 from albumentations.augmentations.utils import (
     check_range,
     get_num_channels,
     is_grayscale_image,
     is_rgb_image,
 )
 from albumentations.core.pydantic import (
     InterpolationType,
     NonNegativeFloatRangeType,
     OnePlusFloatRangeType,
+    OnePlusIntNonDecreasingRangeType,
     OnePlusIntRangeType,
     ProbabilityType,
     SymmetricRangeType,
     ZeroOneRangeType,
+    check_01_range,
+    check_nondecreasing_range,
 )
 from albumentations.core.transforms_interface import (
     BaseTransformInitSchema,
     DualTransform,
     ImageOnlyTransform,
     Interpolation,
     NoOp,
 )
 from albumentations.core.types import (
+    MONO_CHANNEL_DIMENSIONS,
+    NUM_RGB_CHANNELS,
     BoxInternalType,
     ChromaticAberrationMode,
     ColorType,
     ImageCompressionType,
     ImageMode,
     KeypointInternalType,
     MorphologyMode,
@@ -99,17 +104,14 @@
     "PixelDropout",
     "Spatter",
     "ChromaticAberration",
     "Morphological",
 ]
 
 NUM_BITS_ARRAY_LENGTH = 3
-GRAYSCALE_SHAPE_LEN = 2
-NUM_RGB_CHANNELS = 3
-NUM_BITS_ARRAY_LENGTH = 3
 MAX_JPEG_QUALITY = 100
 TWENTY = 20
 PAIR = 2
 
 
 class RandomGridShuffle(DualTransform):
     """Randomly shuffles the grid's cells on an image, mask, or keypoints,
@@ -187,18 +189,18 @@
         warn(
             "Keypoint not in any tile, returning it unchanged. This is unexpected and should be investigated.",
             RuntimeWarning,
         )
         return keypoint
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
-        height, weight = params["image"].shape[:2]
+        height, width = params["image"].shape[:2]
         random_state = random_utils.get_random_state()
         original_tiles = F.split_uniform_grid(
-            (height, weight),
+            (height, width),
             self.grid,
             random_state=random_state,
         )
         shape_groups = F.create_shape_groups(original_tiles)
         mapping = F.shuffle_tiles_within_shape_groups(shape_groups, random_state=random_state)
 
         return {"tiles": original_tiles, "mapping": mapping}
@@ -235,28 +237,25 @@
                 The default mean and std are based on ImageNet.
             - "image": Normalizes the whole image based on its global mean and standard deviation.
             - "image_per_channel": Normalizes the image per channel based on each channel's mean and standard deviation.
             - "min_max": Scales the image pixel values to a [0, 1] range based on the global
                 minimum and maximum pixel values.
             - "min_max_per_channel": Scales each channel of the image pixel values to a [0, 1]
                 range based on the per-channel minimum and maximum pixel values.
-            - "inception": Applies normalization suitable for Inception models
-                with mean and std values of (0.5, 0.5, 0.5) respectively.
 
         p (float): Probability of applying the transform. Defaults to 1.0.
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
     Note:
         For "standard" normalization, `mean`, `std`, and `max_pixel_value` must be provided.
-        For "inception" normalization, the specific mean and std values should be used.
         For other normalization types, these parameters are ignored.
     """
 
     class InitSchema(BaseTransformInitSchema):
         mean: Optional[ColorType] = Field(
             default=(0.485, 0.456, 0.406),
             description="Mean values for normalization, defaulting to ImageNet mean values.",
@@ -268,15 +267,14 @@
         max_pixel_value: Optional[float] = Field(default=255.0, description="Maximum possible pixel value.")
         normalization: Literal[
             "standard",
             "image",
             "image_per_channel",
             "min_max",
             "min_max_per_channel",
-            "inception",
         ] = "standard"
         p: ProbabilityType = 1
 
         @model_validator(mode="after")
         def validate_normalization(self) -> Self:
             if (
                 self.mean is None
@@ -360,16 +358,18 @@
     ):
         super().__init__(always_apply, p)
 
         self.quality_lower = quality_lower
         self.quality_upper = quality_upper
         self.compression_type = compression_type
 
-    def apply(self, img: np.ndarray, quality: int = 100, image_type: str = ".jpg", **params: Any) -> np.ndarray:
-        if img.ndim != GRAYSCALE_SHAPE_LEN and img.shape[-1] not in (1, 3, 4):
+    def apply(
+        self, img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp", ".jpeg"], **params: Any
+    ) -> np.ndarray:
+        if img.ndim != MONO_CHANNEL_DIMENSIONS and img.shape[-1] not in (1, 3, 4):
             msg = "ImageCompression transformation expects 1, 3 or 4 channel images."
             raise TypeError(msg)
         return F.image_compression(img, quality, image_type)
 
     def get_params(self) -> Dict[str, Any]:
         image_type = ".jpg"
 
@@ -429,40 +429,41 @@
     ):
         super().__init__(always_apply, p)
 
         self.snow_point_lower = snow_point_lower
         self.snow_point_upper = snow_point_upper
         self.brightness_coeff = brightness_coeff
 
-    def apply(self, img: np.ndarray, snow_point: float = 0.1, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, snow_point: float, **params: Any) -> np.ndarray:
         return F.add_snow(img, snow_point, self.brightness_coeff)
 
     def get_params(self) -> Dict[str, np.ndarray]:
         return {"snow_point": random.uniform(self.snow_point_lower, self.snow_point_upper)}
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str]:
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("snow_point_lower", "snow_point_upper", "brightness_coeff")
 
 
 class RandomGravel(ImageOnlyTransform):
     """Add gravels.
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         gravel_roi: (top-left x, top-left y,
             bottom-right x, bottom right y). Should be in [0, 1] range
         number_of_patches: no. of gravel patches required
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+
     """
 
     class InitSchema(BaseTransformInitSchema):
         gravel_roi: Tuple[float, float, float, float] = Field(
             default=(0.1, 0.4, 0.9, 0.9),
             description="Region of interest for gravel placement",
         )
@@ -491,15 +492,15 @@
         area = abs((x2 - x1) * (y2 - y1))
         count = area // 10
         gravels = np.empty([count, 2], dtype=np.int64)
         gravels[:, 0] = random_utils.randint(x1, x2, count)
         gravels[:, 1] = random_utils.randint(y1, y2, count)
         return gravels
 
-    def apply(self, img: np.ndarray, gravels_infos: Optional[List[Any]] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, gravels_infos: List[Any], **params: Any) -> np.ndarray:
         if gravels_infos is None:
             gravels_infos = []
         return F.add_gravel(img, gravels_infos)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
@@ -561,16 +562,14 @@
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return "gravel_roi", "number_of_patches"
 
 
 class RandomRain(ImageOnlyTransform):
     """Adds rain effects.
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         slant_lower: should be in range [-20, 20].
         slant_upper: should be in range [-20, 20].
         drop_length: should be in range [0, 100].
         drop_width: should be in range [1, 5].
         drop_color (list of (r, g, b)): rain lines color.
         blur_value (int): rainy view are blurry
@@ -579,14 +578,17 @@
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+
     """
 
     class InitSchema(BaseTransformInitSchema):
         slant_lower: int = Field(default=-10, description="Lower bound for rain slant angle", ge=-20, le=20)
         slant_upper: int = Field(default=10, description="Upper bound for rain slant angle", ge=-20, le=20)
         drop_length: int = Field(default=20, description="Length of raindrops", ge=0, le=100)
         drop_width: int = Field(default=1, description="Width of raindrops", ge=1, le=5)
@@ -629,21 +631,19 @@
         self.blur_value = blur_value
         self.brightness_coefficient = brightness_coefficient
         self.rain_type = rain_type
 
     def apply(
         self,
         img: np.ndarray,
-        slant: int = 10,
-        drop_length: int = 20,
-        rain_drops: Optional[List[Tuple[int, int]]] = None,
+        slant: int,
+        drop_length: int,
+        rain_drops: List[Tuple[int, int]],
         **params: Any,
     ) -> np.ndarray:
-        if rain_drops is None:
-            rain_drops = []
         return F.add_rain(
             img,
             slant,
             drop_length,
             self.drop_width,
             self.drop_color,
             self.blur_value,
@@ -712,15 +712,14 @@
 
     Image types:
         uint8, float32
 
     Reference:
         https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
 
-
     """
 
     class InitSchema(BaseTransformInitSchema):
         fog_coef_lower: float = Field(default=0.3, description="Lower limit for fog intensity coefficient", ge=0, le=1)
         fog_coef_upper: float = Field(default=1, description="Upper limit for fog intensity coefficient", ge=0, le=1)
         alpha_coef: float = Field(default=0.08, description="Transparency of the fog circles", ge=0, le=1)
 
@@ -743,20 +742,18 @@
         self.fog_coef_lower = fog_coef_lower
         self.fog_coef_upper = fog_coef_upper
         self.alpha_coef = alpha_coef
 
     def apply(
         self,
         img: np.ndarray,
-        fog_coef: np.ndarray = 0.1,
-        haze_list: Optional[List[Tuple[int, int]]] = None,
+        fog_coef: np.ndarray,
+        haze_list: List[Tuple[int, int]],
         **params: Any,
     ) -> np.ndarray:
-        if haze_list is None:
-            haze_list = []
         return F.add_fog(img, fog_coef, self.alpha_coef, haze_list)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
@@ -787,16 +784,14 @@
     def get_transform_init_args_names(self) -> Tuple[str, str, str]:
         return ("fog_coef_lower", "fog_coef_upper", "alpha_coef")
 
 
 class RandomSunFlare(ImageOnlyTransform):
     """Simulates Sun Flare for the image
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         flare_roi: region of the image where flare will appear (x_min, y_min, x_max, y_max).
             All values should be in range [0, 1].
         angle_lower: should be in range [0, `angle_upper`].
         angle_upper: should be in range [`angle_lower`, 1].
         num_flare_circles_lower: lower limit for the number of flare circles.
             Should be in range [0, `num_flare_circles_upper`].
@@ -807,14 +802,17 @@
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+
     """
 
     class InitSchema(BaseTransformInitSchema):
         flare_roi: Tuple[float, float, float, float] = Field(
             default=(0, 0, 1, 0.5),
             description="Region of the image where flare will appear",
         )
@@ -867,17 +865,17 @@
         self.src_radius = src_radius
         self.src_color = src_color
         self.flare_roi = flare_roi
 
     def apply(
         self,
         img: np.ndarray,
-        flare_center_x: float = 0.5,
-        flare_center_y: float = 0.5,
-        circles: Optional[List[Any]] = None,
+        flare_center_x: float,
+        flare_center_y: float,
+        circles: List[Any],
         **params: Any,
     ) -> np.ndarray:
         if circles is None:
             circles = []
         return F.add_sun_flare(
             img,
             flare_center_x,
@@ -976,47 +974,39 @@
     """
 
     class InitSchema(BaseTransformInitSchema):
         shadow_roi: Tuple[float, float, float, float] = Field(
             default=(0, 0.5, 1, 1),
             description="Region of the image where shadows will appear",
         )
-        num_shadows_limit: Tuple[int, int] = Field(default=(1, 2))
+        num_shadows_limit: OnePlusIntNonDecreasingRangeType = (1, 2)
         num_shadows_lower: Optional[int] = Field(
             default=None,
             description="Lower limit for the possible number of shadows",
+            deprecated="num_shadows_lower is deprecated. Use num_shadows_limit instead.",
         )
         num_shadows_upper: Optional[int] = Field(
             default=None,
             description="Upper limit for the possible number of shadows",
+            deprecated="num_shadows_upper is deprecated. Use num_shadows_limit instead.",
         )
         shadow_dimension: int = Field(default=5, description="Number of edges in the shadow polygons", gt=0)
 
         @model_validator(mode="after")
         def validate_shadows(self) -> Self:
-            if self.num_shadows_limit[0] > self.num_shadows_limit[1]:
-                msg = "num_shadows_limit[0] must be less than or equal to num_shadows_limit[1]."
-                raise ValueError(msg)
+            if self.num_shadows_lower is not None or self.num_shadows_upper is not None:
+                self.num_shadows_limit = cast(Tuple[int, int], (self.num_shadows_lower, self.num_shadows_upper))
+                self.num_shadows_lower = None
+                self.num_shadows_upper = None
 
             shadow_lower_x, shadow_lower_y, shadow_upper_x, shadow_upper_y = self.shadow_roi
 
             if not 0 <= shadow_lower_x <= shadow_upper_x <= 1 or not 0 <= shadow_lower_y <= shadow_upper_y <= 1:
                 raise ValueError(f"Invalid shadow_roi. Got: {self.shadow_roi}")
 
-            if self.num_shadows_lower is not None or self.num_shadows_upper is not None:
-                warn(
-                    "`num_shadows_lower` and `num_shadows_upper` are deprecated. "
-                    "Use `num_shadows_limit` as tuple (num_shadows_lower, num_shadows_upper) instead.",
-                    DeprecationWarning,
-                    stacklevel=2,
-                )
-                self.num_shadows_limit = cast(Tuple[int, int], (self.num_shadows_lower, self.num_shadows_upper))
-                self.num_shadows_lower = None
-                self.num_shadows_upper = None
-
             return self
 
     def __init__(
         self,
         shadow_roi: Tuple[float, float, float, float] = (0, 0.5, 1, 1),
         num_shadows_limit: Tuple[int, int] = (1, 2),
         num_shadows_lower: Optional[int] = None,
@@ -1027,17 +1017,15 @@
     ):
         super().__init__(always_apply=always_apply, p=p)
 
         self.shadow_roi = shadow_roi
         self.shadow_dimension = shadow_dimension
         self.num_shadows_limit = num_shadows_limit
 
-    def apply(self, img: np.ndarray, vertices_list: Optional[List[np.ndarray]] = None, **params: Any) -> np.ndarray:
-        if vertices_list is None:
-            vertices_list = []
+    def apply(self, img: np.ndarray, vertices_list: List[np.ndarray], **params: Any) -> np.ndarray:
         return F.add_shadow(img, vertices_list)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, List[np.ndarray]]:
@@ -1157,32 +1145,32 @@
         self.hue_shift_limit = cast(Tuple[float, float], hue_shift_limit)
         self.sat_shift_limit = cast(Tuple[float, float], sat_shift_limit)
         self.val_shift_limit = cast(Tuple[float, float], val_shift_limit)
 
     def apply(
         self,
         img: np.ndarray,
-        hue_shift: int = 0,
-        sat_shift: int = 0,
-        val_shift: int = 0,
+        hue_shift: int,
+        sat_shift: int,
+        val_shift: int,
         **params: Any,
     ) -> np.ndarray:
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "HueSaturationValue transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
         return F.shift_hsv(img, hue_shift, sat_shift, val_shift)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "hue_shift": random.uniform(self.hue_shift_limit[0], self.hue_shift_limit[1]),
             "sat_shift": random.uniform(self.sat_shift_limit[0], self.sat_shift_limit[1]),
             "val_shift": random.uniform(self.val_shift_limit[0], self.val_shift_limit[1]),
         }
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str]:
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("hue_shift_limit", "sat_shift_limit", "val_shift_limit")
 
 
 class Solarize(ImageOnlyTransform):
     """Invert all pixel values above a threshold.
 
     Args:
@@ -1201,15 +1189,15 @@
     class InitSchema(BaseTransformInitSchema):
         threshold: OnePlusFloatRangeType = (128, 128)
 
     def __init__(self, threshold: ScaleType = (128, 128), always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply=always_apply, p=p)
         self.threshold = cast(Tuple[float, float], threshold)
 
-    def apply(self, img: np.ndarray, threshold: int = 0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, threshold: int, **params: Any) -> np.ndarray:
         return F.solarize(img, threshold)
 
     def get_params(self) -> Dict[str, float]:
         return {"threshold": random.uniform(self.threshold[0], self.threshold[1])}
 
     def get_transform_init_args_names(self) -> Tuple[str]:
         return ("threshold",)
@@ -1254,15 +1242,15 @@
         num_bits: Union[int, Tuple[int, int], Tuple[int, int, int]] = 4,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.num_bits = cast(Union[Tuple[int, ...], List[Tuple[int, ...]]], num_bits)
 
-    def apply(self, img: np.ndarray, num_bits: int = 1, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, num_bits: int, **params: Any) -> np.ndarray:
         return F.posterize(img, num_bits)
 
     def get_params(self) -> Dict[str, Any]:
         if len(self.num_bits) == NUM_BITS_ARRAY_LENGTH:
             return {"num_bits": [random.randint(int(i[0]), int(i[1])) for i in self.num_bits]}  # type: ignore[index]
         num_bits = self.num_bits
         return {"num_bits": random.randint(int(num_bits[0]), int(num_bits[1]))}  # type: ignore[arg-type]
@@ -1312,15 +1300,15 @@
         super().__init__(always_apply=always_apply, p=p)
 
         self.mode = mode
         self.by_channels = by_channels
         self.mask = mask
         self.mask_params = mask_params
 
-    def apply(self, img: np.ndarray, mask: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, mask: np.ndarray, **params: Any) -> np.ndarray:
         return F.equalize(img, mode=self.mode, by_channels=self.by_channels, mask=mask)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         if not callable(self.mask):
             return {"mask": self.mask}
 
         return {"mask": self.mask(**params)}
@@ -1367,25 +1355,25 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.r_shift_limit = cast(Tuple[float, float], r_shift_limit)
         self.g_shift_limit = cast(Tuple[float, float], g_shift_limit)
         self.b_shift_limit = cast(Tuple[float, float], b_shift_limit)
 
-    def apply(self, img: np.ndarray, r_shift: int = 0, g_shift: int = 0, b_shift: int = 0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, r_shift: int, g_shift: int, b_shift: int, **params: Any) -> np.ndarray:
         if not is_rgb_image(img):
             msg = "RGBShift transformation expects 3-channel images."
             raise TypeError(msg)
         return F.shift_rgb(img, r_shift, g_shift, b_shift)
 
     def get_params(self) -> Dict[str, Any]:
         return {
-            "r_shift": random.uniform(self.r_shift_limit[0], self.r_shift_limit[1]),
-            "g_shift": random.uniform(self.g_shift_limit[0], self.g_shift_limit[1]),
-            "b_shift": random.uniform(self.b_shift_limit[0], self.b_shift_limit[1]),
+            "r_shift": random_utils.uniform(self.r_shift_limit[0], self.r_shift_limit[1]),
+            "g_shift": random_utils.uniform(self.g_shift_limit[0], self.g_shift_limit[1]),
+            "b_shift": random_utils.uniform(self.b_shift_limit[0], self.b_shift_limit[1]),
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str]:
         return ("r_shift_limit", "g_shift_limit", "b_shift_limit")
 
 
 class RandomBrightnessContrast(ImageOnlyTransform):
@@ -1422,15 +1410,15 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.brightness_limit = cast(Tuple[float, float], brightness_limit)
         self.contrast_limit = cast(Tuple[float, float], contrast_limit)
         self.brightness_by_max = brightness_by_max
 
-    def apply(self, img: np.ndarray, alpha: float = 1.0, beta: float = 0.0, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, alpha: float, beta: float, **params: Any) -> np.ndarray:
         return F.brightness_contrast_adjust(img, alpha, beta, self.brightness_by_max)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "alpha": 1.0 + random.uniform(self.contrast_limit[0], self.contrast_limit[1]),
             "beta": 0.0 + random.uniform(self.brightness_limit[0], self.brightness_limit[1]),
         }
@@ -1472,36 +1460,36 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.var_limit = cast(Tuple[float, float], var_limit)
         self.mean = mean
         self.per_channel = per_channel
 
-    def apply(self, img: np.ndarray, gauss: Optional[float] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, gauss: float, **params: Any) -> np.ndarray:
         return F.gauss_noise(img, gauss=gauss)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, float]:
         image = params["image"]
         var = random.uniform(self.var_limit[0], self.var_limit[1])
         sigma = var**0.5
 
         if self.per_channel:
             gauss = random_utils.normal(self.mean, sigma, image.shape)
         else:
             gauss = random_utils.normal(self.mean, sigma, image.shape[:2])
-            if len(image.shape) > GRAYSCALE_SHAPE_LEN:
+            if image.ndim > MONO_CHANNEL_DIMENSIONS:
                 gauss = np.expand_dims(gauss, -1)
 
         return {"gauss": gauss}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str]:
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("var_limit", "per_channel", "mean")
 
 
 class ISONoise(ImageOnlyTransform):
     """Apply camera sensor noise.
 
     Args:
@@ -1541,26 +1529,26 @@
         super().__init__(always_apply=always_apply, p=p)
         self.intensity = intensity
         self.color_shift = color_shift
 
     def apply(
         self,
         img: np.ndarray,
-        color_shift: float = 0.05,
-        intensity: float = 1.0,
-        random_state: Optional[int] = None,
+        color_shift: float,
+        intensity: float,
+        random_seed: int,
         **params: Any,
     ) -> np.ndarray:
-        return F.iso_noise(img, color_shift, intensity, np.random.RandomState(random_state))
+        return F.iso_noise(img, color_shift, intensity, np.random.RandomState(random_seed))
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "color_shift": random_utils.uniform(self.color_shift[0], self.color_shift[1]),
             "intensity": random_utils.uniform(self.intensity[0], self.intensity[1]),
-            "random_state": random_utils.randint(0, 65536),
+            "random_seed": random_utils.get_random_seed(),
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("intensity", "color_shift")
 
 
 class CLAHE(ImageOnlyTransform):
@@ -1591,30 +1579,30 @@
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.clip_limit = cast(Tuple[float, float], clip_limit)
         self.tile_grid_size = tile_grid_size
 
-    def apply(self, img: np.ndarray, clip_limit: float = 2, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, clip_limit: float, **params: Any) -> np.ndarray:
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "CLAHE transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
 
         return F.clahe(img, clip_limit, self.tile_grid_size)
 
     def get_params(self) -> Dict[str, float]:
         return {"clip_limit": random.uniform(self.clip_limit[0], self.clip_limit[1])}
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("clip_limit", "tile_grid_size")
 
 
 class ChannelShuffle(ImageOnlyTransform):
-    """Randomly rearrange channels of the input RGB image.
+    """Randomly rearrange channels of the image.
 
     Args:
         p: probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
@@ -1623,15 +1611,15 @@
 
     """
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
-    def apply(self, img: np.ndarray, channels_shuffled: Tuple[int, int, int] = (0, 1, 2), **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, channels_shuffled: Tuple[int, ...], **params: Any) -> np.ndarray:
         return F.channel_shuffle(img, channels_shuffled)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
         ch_arr = list(range(img.shape[2]))
         ch_arr = random_utils.shuffle(ch_arr)
         return {"channels_shuffled": ch_arr}
@@ -1696,37 +1684,43 @@
         gamma_limit: ScaleIntType = (80, 120),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.gamma_limit = cast(Tuple[float, float], gamma_limit)
 
-    def apply(self, img: np.ndarray, gamma: float = 1, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, gamma: float, **params: Any) -> np.ndarray:
         return F.gamma_transform(img, gamma=gamma)
 
     def get_params(self) -> Dict[str, float]:
         return {"gamma": random.uniform(self.gamma_limit[0], self.gamma_limit[1]) / 100.0}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("gamma_limit",)
 
 
 class ToGray(ImageOnlyTransform):
-    """Convert the input RGB image to grayscale. If the mean pixel value for the resulting image is greater
-    than 127, invert the resulting grayscale image.
+    """Convert the input RGB image to grayscale. If the input image is already grayscale, a warning is issued but
+    the original image is returned unchanged. This transformation checks if the image is RGB; if not, it raises
+    a TypeError.
 
     Args:
-        p: probability of applying the transform. Default: 0.5.
+        p (float): Probability of applying the transform. Default is 0.5.
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Note:
+        This transform assumes the input image is in RGB format.
+
+    Raises:
+        TypeError: If the input image is not a 3-channel RGB image.
     """
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if is_grayscale_image(img):
             warnings.warn("The image is already gray.")
             return img
         if not is_rgb_image(img):
@@ -1878,104 +1872,130 @@
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         return F.from_float(img, self.dtype, self.max_value)
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {"dtype": self.dtype.name, "max_value": self.max_value}
 
 
+class InterpolationDict(TypedDict):
+    upscale: int
+    downscale: int
+
+
+class InterpolationPydantic(BaseModel):
+    upscale: InterpolationType
+    downscale: InterpolationType
+
+
 class Downscale(ImageOnlyTransform):
-    """Decreases image quality by downscaling and upscaling back.
+    """Decreases image quality by downscaling and then upscaling it back to its original size.
 
     Args:
-        scale_min: lower bound on the image scale. Should be <= scale_max.
-        scale_max: upper bound on the image scale. Should be < 1.
-        interpolation: cv2 interpolation method. Could be:
-            - single cv2 interpolation flag - selected method will be used for downscale and upscale.
-            - dict(downscale=flag, upscale=flag)
-            - Downscale.Interpolation(downscale=flag, upscale=flag) -
-            Default: Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST)
+        scale_range (Tuple[float, float]): A tuple defining the minimum and maximum scale to which the image
+            will be downscaled. The range should be between 0 and 1, inclusive at minimum and exclusive at maximum.
+            The first value should be less than or equal to the second value.
+        interpolation_pair (InterpolationDict): A dictionary specifying the interpolation methods to use for
+            downscaling and upscaling. Should include keys 'downscale' and 'upscale' with cv2 interpolation
+                flags as values.
+            Example: {"downscale": cv2.INTER_NEAREST, "upscale": cv2.INTER_LINEAR}.
+        always_apply (bool): If set to True, the transform will always be applied. Defaults to False.
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Note:
+        Previous parameters `scale_min`, `scale_max`, and `interpolation` are deprecated. Use `scale_range`
+        and `interpolation_pair` for specifying scaling bounds and interpolation methods respectively.
+
+    Example:
+        >>> transform = Downscale(scale_range=(0.5, 0.9), interpolation_pair={"downscale": cv2.INTER_AREA,
+                                                          "upscale": cv2.INTER_CUBIC})
+        >>> transformed = transform(image=img)
     """
 
     class InitSchema(BaseTransformInitSchema):
-        scale_min: float = Field(default=0.25, ge=0, le=1, description="Lower bound on the image scale.")
-        scale_max: float = Field(default=0.25, ge=0, lt=1, description="Upper bound on the image scale.")
-        interpolation: Optional[Union[int, Interpolation, Dict[str, int]]] = Field(
+        scale_min: Optional[float] = Field(
+            default=None,
+            ge=0,
+            le=1,
+            description="Lower bound on the image scale.",
+            deprecated="Use scale_range instead.",
+        )
+        scale_max: Optional[float] = Field(
+            default=None,
+            ge=0,
+            lt=1,
+            description="Upper bound on the image scale.",
+            deprecated="Use scale_range instead.",
+        )
+
+        interpolation: Optional[Union[int, Interpolation, InterpolationDict]] = Field(
             default_factory=lambda: Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST),
-            description="CV2 interpolation method or a dictionary specifying downscale and upscale methods.",
+            deprecated="Use interpolation_pair instead.",
         )
+        interpolation_pair: InterpolationPydantic
 
-        @model_validator(mode="after")
-        def validate_scale(self) -> Self:
-            if self.scale_min > self.scale_max:
-                msg = "scale_min must be less than or equal to scale_max"
-                raise ValueError(msg)
-            return self
+        scale_range: Annotated[
+            Tuple[float, float], AfterValidator(check_01_range), AfterValidator(check_nondecreasing_range)
+        ] = (0.25, 0.25)
 
-        @field_validator("interpolation")
-        @classmethod
-        def set_interpolation(cls, v: Any) -> Interpolation:
-            if isinstance(v, dict):
-                return Interpolation(**v)
-            if isinstance(v, int):
-                return Interpolation(downscale=v, upscale=v)
-            if isinstance(v, Interpolation):
-                return v
-            if v is None:
-                return Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST)
+        @model_validator(mode="after")
+        def validate_params(self) -> Self:
+            if self.scale_min is not None and self.scale_max is not None:
+                self.scale_range = (self.scale_min, self.scale_max)
+                self.scale_min = None
+                self.scale_max = None
+
+            if self.interpolation is not None:
+                if isinstance(self.interpolation, dict):
+                    self.interpolation_pair = InterpolationPydantic(**self.interpolation)
+                elif isinstance(self.interpolation, int):
+                    self.interpolation_pair = InterpolationPydantic(
+                        upscale=self.interpolation, downscale=self.interpolation
+                    )
+                elif isinstance(self.interpolation, Interpolation):
+                    self.interpolation_pair = InterpolationPydantic(
+                        upscale=self.interpolation.upscale, downscale=self.interpolation.downscale
+                    )
+                self.interpolation = None
 
-            msg = (
-                "Interpolation must be an int, Interpolation instance, "
-                "or dict specifying downscale and upscale methods."
-            )
-            raise ValueError(msg)
+            return self
 
     def __init__(
         self,
-        scale_min: float = 0.25,
-        scale_max: float = 0.25,
-        interpolation: Optional[Union[int, Interpolation, Dict[str, int]]] = None,
+        scale_min: Optional[float] = None,
+        scale_max: Optional[float] = None,
+        interpolation: Optional[Union[int, Interpolation, InterpolationDict]] = None,
+        scale_range: Tuple[float, float] = (0.25, 0.25),
+        interpolation_pair: InterpolationDict = InterpolationDict(
+            {"upscale": cv2.INTER_NEAREST, "downscale": cv2.INTER_NEAREST}
+        ),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
-        self.scale_min = scale_min
-        self.scale_max = scale_max
-        self.interpolation = cast(Interpolation, interpolation)
+        self.scale_range = scale_range
+        self.interpolation_pair = interpolation_pair
 
     def apply(self, img: np.ndarray, scale: float, **params: Any) -> np.ndarray:
-        if isinstance(self.interpolation, int):
-            msg = "Should not be here, added for typing purposes. Please report this issue."
-            raise TypeError(msg)
         return F.downscale(
             img,
             scale=scale,
-            down_interpolation=self.interpolation.downscale,
-            up_interpolation=self.interpolation.upscale,
+            down_interpolation=self.interpolation_pair["downscale"],
+            up_interpolation=self.interpolation_pair["upscale"],
         )
 
     def get_params(self) -> Dict[str, Any]:
-        return {"scale": random.uniform(self.scale_min, self.scale_max)}
+        return {"scale": random.uniform(self.scale_range[0], self.scale_range[1])}
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
-        return "scale_min", "scale_max"
-
-    def to_dict_private(self) -> Dict[str, Any]:
-        if isinstance(self.interpolation, int):
-            msg = "Should not be here, added for typing purposes. Please report this issue."
-            raise TypeError(msg)
-        result = super().to_dict_private()
-        result["interpolation"] = {"upscale": self.interpolation.upscale, "downscale": self.interpolation.downscale}
-        return result
+        return ("scale_range", "interpolation_pair")
 
 
 class Lambda(NoOp):
     """A flexible transformation class for using user-defined transformation functions per targets.
     Function signature must include **kwargs to accept optional arguments like interpolation method, image size, etc:
 
     Args:
@@ -2101,15 +2121,15 @@
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.multiplier = cast(Tuple[float, float], multiplier)
         self.per_channel = per_channel
         self.elementwise = elementwise
 
-    def apply(self, img: np.ndarray, multiplier: float = np.array([1]), **kwargs: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, multiplier: float, **kwargs: Any) -> np.ndarray:
         return F.multiply(img, multiplier)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         if self.multiplier[0] == self.multiplier[1]:
             return {"multiplier": np.array([self.multiplier[0]])}
 
         img = params["image"]
@@ -2117,33 +2137,33 @@
         height, width = img.shape[:2]
 
         num_channels = (1 if is_grayscale_image(img) else img.shape[-1]) if self.per_channel else 1
 
         shape = [height, width, num_channels] if self.elementwise else [num_channels]
 
         multiplier = random_utils.uniform(self.multiplier[0], self.multiplier[1], tuple(shape))
-        if is_grayscale_image(img) and img.ndim == GRAYSCALE_SHAPE_LEN:
+        if img.ndim == MONO_CHANNEL_DIMENSIONS:
             multiplier = np.squeeze(multiplier)
 
         return {"multiplier": multiplier}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str]:
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "multiplier", "per_channel", "elementwise"
 
 
 class FancyPCA(ImageOnlyTransform):
     """Augment RGB image using FancyPCA from Krizhevsky's paper
     "ImageNet Classification with Deep Convolutional Neural Networks"
 
     Args:
-        alpha:  how much to perturb/scale the eigen vecs and vals.
+        alpha:  how much to perturb/scale the eigen vectors and eigenvalues.
             scale is samples from gaussian distribution (mu=0, sigma=alpha)
 
     Targets:
         image
 
     Image types:
         3-channel uint8 images only
@@ -2158,15 +2178,15 @@
     class InitSchema(BaseTransformInitSchema):
         alpha: float = Field(default=0.1, description="Scale for perturbing the eigen vectors and values", ge=0)
 
     def __init__(self, alpha: float = 0.1, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply=always_apply, p=p)
         self.alpha = alpha
 
-    def apply(self, img: np.ndarray, alpha: float = 0.1, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, alpha: float, **params: Any) -> np.ndarray:
         return F.fancy_pca(img, alpha)
 
     def get_params(self) -> Dict[str, float]:
         return {"alpha": random.gauss(0, self.alpha)}
 
     def get_transform_init_args_names(self) -> Tuple[str]:
         return ("alpha",)
@@ -2266,19 +2286,19 @@
             "hue": hue,
             "order": order,
         }
 
     def apply(
         self,
         img: np.ndarray,
-        brightness: float = 1.0,
-        contrast: float = 1.0,
-        saturation: float = 1.0,
-        hue: float = 0,
-        order: Optional[List[int]] = None,
+        brightness: float,
+        contrast: float,
+        saturation: float,
+        hue: float,
+        order: List[int],
         **params: Any,
     ) -> np.ndarray:
         if order is None:
             order = [0, 1, 2, 3]
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "ColorJitter transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
@@ -2332,15 +2352,15 @@
 
     def get_params(self) -> Dict[str, np.ndarray]:
         alpha = random.uniform(*self.alpha)
         lightness = random.uniform(*self.lightness)
         sharpening_matrix = self.__generate_sharpening_matrix(alpha_sample=alpha, lightness_sample=lightness)
         return {"sharpening_matrix": sharpening_matrix}
 
-    def apply(self, img: np.ndarray, sharpening_matrix: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, sharpening_matrix: np.ndarray, **params: Any) -> np.ndarray:
         return F.convolve(img, sharpening_matrix)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("alpha", "lightness")
 
 
 class Emboss(ImageOnlyTransform):
@@ -2387,15 +2407,15 @@
 
     def get_params(self) -> Dict[str, np.ndarray]:
         alpha = random.uniform(*self.alpha)
         strength = random.uniform(*self.strength)
         emboss_matrix = self.__generate_emboss_matrix(alpha_sample=alpha, strength_sample=strength)
         return {"emboss_matrix": emboss_matrix}
 
-    def apply(self, img: np.ndarray, emboss_matrix: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, emboss_matrix: np.ndarray, **params: Any) -> np.ndarray:
         return F.convolve(img, emboss_matrix)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("alpha", "strength")
 
 
 class Superpixels(ImageOnlyTransform):
@@ -2409,17 +2429,17 @@
     Examples:
                 * A probability of ``0.0`` would mean, that the pixels in no
                   segment are replaced by their average color (image is not
                   changed at all).
                 * A probability of ``0.5`` would mean, that around half of all
                   segments are replaced by their average color.
                 * A probability of ``1.0`` would mean, that all segments are
-                  replaced by their average color (resulting in a voronoi
+                  replaced by their average color (resulting in a Voronoi
                   image).
-            Behaviour based on chosen data types for this parameter:
+            Behavior based on chosen data types for this parameter:
                 * If a ``float``, then that ``flat`` will always be used.
                 * If ``tuple`` ``(a, b)``, then a random probability will be
                   sampled from the interval ``[a, b]`` per image.
         n_segments (tuple of int): Rough target number of how many superpixels to generate (the algorithm
             may deviate from this number). Lower value will lead to coarser superpixels.
             Higher values are computationally more intensive and will hence lead to a slowdown
             Then a value from the discrete interval ``[a..b]`` will be sampled per image.
@@ -2470,19 +2490,19 @@
         n_segments = random_utils.randint(self.n_segments[0], self.n_segments[1] + 1)
         p = random.uniform(*self.p_replace)
         return {"replace_samples": random_utils.random(n_segments) < p, "n_segments": n_segments}
 
     def apply(
         self,
         img: np.ndarray,
-        replace_samples: Sequence[bool] = (False,),
-        n_segments: int = 1,
+        replace_samples: Sequence[bool],
+        n_segments: int,
         **kwargs: Any,
     ) -> np.ndarray:
-        return F.superpixels(img, n_segments, replace_samples, self.max_size, cast(int, self.interpolation))
+        return F.superpixels(img, n_segments, replace_samples, self.max_size, self.interpolation)
 
 
 class TemplateTransform(ImageOnlyTransform):
     """Apply blending of input image with specified templates
     Args:
         templates (numpy array or list of numpy arrays): Images as template for transform.
         img_weight: If single float weight will be sampled from (0, img_weight).
@@ -2542,17 +2562,17 @@
         self.template_weight = cast(Tuple[float, float], template_weight)
         self.template_transform = template_transform
         self.name = name
 
     def apply(
         self,
         img: np.ndarray,
-        template: Optional[np.ndarray] = None,
-        img_weight: float = 0.5,
-        template_weight: float = 0.5,
+        template: np.ndarray,
+        img_weight: float,
+        template_weight: float,
         **params: Any,
     ) -> np.ndarray:
         return F.add_weighted(img, img_weight, template, template_weight)
 
     def get_params(self) -> Dict[str, float]:
         return {
             "img_weight": random.uniform(self.img_weight[0], self.img_weight[1]),
@@ -2668,15 +2688,15 @@
         kernel[(ksize - 1) // 2, (ksize - 1) // 2] = cutoff**2 / (4 * np.pi)
 
         # Normalize kernel
         kernel = kernel.astype(np.float32) / np.sum(kernel)
 
         return {"kernel": kernel}
 
-    def apply(self, img: np.ndarray, kernel: Optional[int] = None, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, kernel: int, **params: Any) -> np.ndarray:
         return F.convolve(img, kernel)
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("blur_limit", "cutoff")
 
 
 class UnsharpMask(ImageOnlyTransform):
@@ -2740,18 +2760,18 @@
     def get_params(self) -> Dict[str, Any]:
         return {
             "ksize": random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2),
             "sigma": random.uniform(*self.sigma_limit),
             "alpha": random.uniform(*self.alpha),
         }
 
-    def apply(self, img: np.ndarray, ksize: int = 3, sigma: int = 0, alpha: float = 0.2, **params: Any) -> np.ndarray:
+    def apply(self, img: np.ndarray, ksize: int, sigma: int, alpha: float, **params: Any) -> np.ndarray:
         return F.unsharp_mask(img, ksize, sigma=sigma, alpha=alpha, threshold=self.threshold)
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "blur_limit", "sigma_limit", "alpha", "threshold"
 
 
 class PixelDropout(DualTransform):
     """Set pixels to 0 with some probability.
 
     Args:
@@ -2811,25 +2831,25 @@
         self.per_channel = per_channel
         self.drop_value = drop_value
         self.mask_drop_value = mask_drop_value
 
     def apply(
         self,
         img: np.ndarray,
-        drop_mask: Optional[np.ndarray] = None,
-        drop_value: Union[float, Sequence[float]] = (),
+        drop_mask: np.ndarray,
+        drop_value: Union[float, Sequence[float]],
         **params: Any,
     ) -> np.ndarray:
         return F.pixel_dropout(img, drop_mask, drop_value)
 
-    def apply_to_mask(self, mask: np.ndarray, drop_mask: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
+    def apply_to_mask(self, mask: np.ndarray, drop_mask: np.ndarray, **params: Any) -> np.ndarray:
         if self.mask_drop_value is None:
             return mask
 
-        if mask.ndim == GRAYSCALE_SHAPE_LEN:
+        if mask.ndim == MONO_CHANNEL_DIMENSIONS:
             drop_mask = np.squeeze(drop_mask)
 
         return F.pixel_dropout(mask, drop_mask, self.mask_drop_value)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return bbox
 
@@ -2981,18 +3001,18 @@
         self.intensity = cast(Tuple[float, float], intensity)
         self.mode = mode
         self.color = cast(Dict[str, Sequence[int]], color)
 
     def apply(
         self,
         img: np.ndarray,
-        non_mud: Optional[np.ndarray] = None,
-        mud: Optional[np.ndarray] = None,
-        drops: Optional[np.ndarray] = None,
-        mode: SpatterMode = "mud",
+        non_mud: np.ndarray,
+        mud: np.ndarray,
+        drops: np.ndarray,
+        mode: SpatterMode,
         **params: Dict[str, Any],
     ) -> np.ndarray:
         return F.spatter(img, non_mud, mud, drops, mode)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
@@ -3105,27 +3125,27 @@
         self.secondary_distortion_limit = cast(Tuple[float, float], secondary_distortion_limit)
         self.mode = mode
         self.interpolation = interpolation
 
     def apply(
         self,
         img: np.ndarray,
-        primary_distortion_red: float = -0.02,
-        secondary_distortion_red: float = -0.05,
-        primary_distortion_blue: float = -0.02,
-        secondary_distortion_blue: float = -0.05,
+        primary_distortion_red: float,
+        secondary_distortion_red: float,
+        primary_distortion_blue: float,
+        secondary_distortion_blue: float,
         **params: Any,
     ) -> np.ndarray:
         return F.chromatic_aberration(
             img,
             primary_distortion_red,
             secondary_distortion_red,
             primary_distortion_blue,
             secondary_distortion_blue,
-            cast(int, self.interpolation),
+            self.interpolation,
         )
 
     def get_params(self) -> Dict[str, float]:
         primary_distortion_red = random_utils.uniform(*self.primary_distortion_limit)
         secondary_distortion_red = random_utils.uniform(*self.secondary_distortion_limit)
         primary_distortion_blue = random_utils.uniform(*self.primary_distortion_limit)
         secondary_distortion_blue = random_utils.uniform(*self.secondary_distortion_limit)
```

### Comparing `albumentations-1.4.4/albumentations/augmentations/utils.py` & `albumentations-1.4.6/albumentations/augmentations/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 from typing import Any, Callable, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 from typing_extensions import Concatenate, ParamSpec
 
 from albumentations.core.keypoints_utils import angle_to_2pi_range
-from albumentations.core.types import KeypointInternalType
+from albumentations.core.types import (
+    MONO_CHANNEL_DIMENSIONS,
+    NUM_MULTI_CHANNEL_DIMENSIONS,
+    NUM_RGB_CHANNELS,
+    KeypointInternalType,
+)
 
 __all__ = [
     "read_bgr_image",
     "read_rgb_image",
     "read_grayscale",
     "MAX_VALUES_BY_DTYPE",
     "NPDTYPE_TO_OPENCV_DTYPE",
     "clipped",
     "get_opencv_dtype_from_numpy",
     "angle_2pi_range",
     "clip",
-    "preserve_shape",
     "preserve_channel_dim",
     "ensure_contiguous",
     "is_rgb_image",
     "is_grayscale_image",
     "is_multispectral_image",
     "get_num_channels",
     "non_rgb_warning",
@@ -53,16 +57,14 @@
     np.dtype("uint16"): cv2.CV_16U,
     np.dtype("int32"): cv2.CV_32S,
     np.dtype("float32"): cv2.CV_32F,
     np.dtype("float64"): cv2.CV_64F,
 }
 
 TWO = 2
-THREE = 3
-RGB_NUM_CHANNELS = 3
 FOUR = 4
 BIG_INTEGER = MAX_VALUES_BY_DTYPE[np.uint32]
 
 
 def read_bgr_image(path: Union[str, Path]) -> np.ndarray:
     return cv2.imread(str(path), cv2.IMREAD_COLOR)
 
@@ -107,39 +109,32 @@
     def wrapped_function(keypoint: KeypointInternalType, *args: P.args, **kwargs: P.kwargs) -> KeypointInternalType:
         (x, y, a, s) = func(keypoint, *args, **kwargs)[:4]
         return (x, y, angle_to_2pi_range(a), s)
 
     return wrapped_function
 
 
-def preserve_shape(
-    func: Callable[Concatenate[np.ndarray, P], np.ndarray],
-) -> Callable[Concatenate[np.ndarray, P], np.ndarray]:
-    """Preserve shape of the image"""
-
-    @wraps(func)
-    def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
-        shape = img.shape
-        result = func(img, *args, **kwargs)
-        return result.reshape(shape)
-
-    return wrapped_function
-
-
 def preserve_channel_dim(
     func: Callable[Concatenate[np.ndarray, P], np.ndarray],
 ) -> Callable[Concatenate[np.ndarray, P], np.ndarray]:
     """Preserve dummy channel dim."""
 
     @wraps(func)
     def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
         shape = img.shape
         result = func(img, *args, **kwargs)
-        if len(shape) == THREE and shape[-1] == 1 and len(result.shape) == TWO:
-            result = np.expand_dims(result, axis=-1)
+        if (
+            len(shape) == NUM_MULTI_CHANNEL_DIMENSIONS
+            and shape[-1] == 1
+            and len(result.shape) == MONO_CHANNEL_DIMENSIONS
+        ):
+            return np.expand_dims(result, axis=-1)
+
+        if len(shape) == MONO_CHANNEL_DIMENSIONS and len(result.shape) == NUM_MULTI_CHANNEL_DIMENSIONS:
+            return result[:, :, 0]
         return result
 
     return wrapped_function
 
 
 def ensure_contiguous(
     func: Callable[Concatenate[np.ndarray, P], np.ndarray],
@@ -150,28 +145,29 @@
     def wrapped_function(img: np.ndarray, *args: P.args, **kwargs: P.kwargs) -> np.ndarray:
         img = np.require(img, requirements=["C_CONTIGUOUS"])
         return func(img, *args, **kwargs)
 
     return wrapped_function
 
 
+def get_num_channels(image: np.ndarray) -> int:
+    return image.shape[2] if len(image.shape) == NUM_MULTI_CHANNEL_DIMENSIONS else 1
+
+
 def is_rgb_image(image: np.ndarray) -> bool:
-    return len(image.shape) == THREE and image.shape[-1] == RGB_NUM_CHANNELS
+    return get_num_channels(image) == NUM_RGB_CHANNELS
 
 
 def is_grayscale_image(image: np.ndarray) -> bool:
-    return (len(image.shape) == TWO) or (len(image.shape) == THREE and image.shape[-1] == 1)
+    return get_num_channels(image) == 1
 
 
 def is_multispectral_image(image: np.ndarray) -> bool:
-    return len(image.shape) == THREE and image.shape[-1] not in [1, 3]
-
-
-def get_num_channels(image: np.ndarray) -> int:
-    return image.shape[2] if len(image.shape) == THREE else 1
+    num_channels = get_num_channels(image)
+    return num_channels not in {1, 3}
 
 
 def non_rgb_warning(image: np.ndarray) -> None:
     if not is_rgb_image(image):
         message = "This transformation expects 3-channel images"
         if is_grayscale_image(image):
             message += "\nYou can convert your grayscale image to RGB using cv2.cvtColor(image, cv2.COLOR_GRAY2RGB))"
```

### Comparing `albumentations-1.4.4/albumentations/core/bbox_utils.py` & `albumentations-1.4.6/albumentations/core/bbox_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,67 +27,71 @@
 BBOX_WITH_LABEL_SHAPE = 5
 
 
 class BboxParams(Params):
     """Parameters of bounding boxes
 
     Args:
-        format (str): format of bounding boxes. Should be 'coco', 'pascal_voc', 'albumentations' or 'yolo'.
+        format (str): format of bounding boxes. Should be `coco`, `pascal_voc`, `albumentations` or `yolo`.
 
             The `coco` format
                 `[x_min, y_min, width, height]`, e.g. [97, 12, 150, 200].
             The `pascal_voc` format
                 `[x_min, y_min, x_max, y_max]`, e.g. [97, 12, 247, 212].
             The `albumentations` format
                 is like `pascal_voc`, but normalized,
                 in other words: `[x_min, y_min, x_max, y_max]`, e.g. [0.2, 0.3, 0.4, 0.5].
             The `yolo` format
                 `[x, y, width, height]`, e.g. [0.1, 0.2, 0.3, 0.4];
                 `x`, `y` - normalized bbox center; `width`, `height` - normalized bbox width and height.
-        label_fields (list): list of fields that are joined with boxes, e.g labels.
-            Should be same type as boxes.
-        min_area (float): minimum area of a bounding box. All bounding boxes whose
-            visible area in pixels is less than this value will be removed. Default: 0.0.
-        min_visibility (float): minimum fraction of area for a bounding box
-            to remain this box in list. Default: 0.0.
-        min_width (float): Minimum width of a bounding box. All bounding boxes whose width is
-            less than this value will be removed. Default: 0.0.
-        min_height (float): Minimum height of a bounding box. All bounding boxes whose height is
-            less than this value will be removed. Default: 0.0.
-        check_each_transform (bool): if `True`, then bboxes will be checked after each dual transform.
-            Default: `True`
+
+        label_fields (list): List of fields joined with boxes, e.g., labels.
+        min_area (float): Minimum area of a bounding box in pixels or normalized units.
+            Bounding boxes with an area less than this value will be removed. Default: 0.0.
+        min_visibility (float): Minimum fraction of area for a bounding box to remain in the list.
+            Bounding boxes with a visible area less than this fraction will be removed. Default: 0.0.
+        min_width (float): Minimum width of a bounding box in pixels or normalized units.
+            Bounding boxes with a width less than this value will be removed. Default: 0.0.
+        min_height (float): Minimum height of a bounding box in pixels or normalized units.
+            Bounding boxes with a height less than this value will be removed. Default: 0.0.
+        check_each_transform (bool): If True, bounding boxes will be checked after each dual transform. Default: True.
+        clip (bool): If True, bounding boxes will be clipped to the image borders before applying any transform.
+            Default: False.
 
     """
 
     def __init__(
         self,
         format: str,
-        label_fields: Optional[Sequence[str]] = None,
+        label_fields: Optional[Sequence[Any]] = None,
         min_area: float = 0.0,
         min_visibility: float = 0.0,
         min_width: float = 0.0,
         min_height: float = 0.0,
         check_each_transform: bool = True,
+        clip: bool = False,
     ):
         super().__init__(format, label_fields)
         self.min_area = min_area
         self.min_visibility = min_visibility
         self.min_width = min_width
         self.min_height = min_height
         self.check_each_transform = check_each_transform
+        self.clip = clip
 
     def to_dict_private(self) -> Dict[str, Any]:
         data = super().to_dict_private()
         data.update(
             {
                 "min_area": self.min_area,
                 "min_visibility": self.min_visibility,
                 "min_width": self.min_width,
                 "min_height": self.min_height,
                 "check_each_transform": self.check_each_transform,
+                "clip": self.clip,
             },
         )
         return data
 
     @classmethod
     def is_serializable(cls) -> bool:
         return True
@@ -133,14 +137,21 @@
     def check(self, data: Sequence[BoxType], rows: int, cols: int) -> None:
         check_bboxes(data)
 
     def convert_from_albumentations(self, data: Sequence[BoxType], rows: int, cols: int) -> List[BoxType]:
         return convert_bboxes_from_albumentations(data, self.params.format, rows, cols, check_validity=True)
 
     def convert_to_albumentations(self, data: Sequence[BoxType], rows: int, cols: int) -> List[BoxType]:
+        if self.params.clip:
+            data = convert_bboxes_to_albumentations(data, self.params.format, rows, cols, check_validity=False)
+            data = filter_bboxes(data, rows, cols, min_area=0, min_visibility=0, min_width=0, min_height=0)
+            for bbox in data:
+                check_bbox(bbox)
+            return data
+
         return convert_bboxes_to_albumentations(data, self.params.format, rows, cols, check_validity=True)
 
 
 def normalize_bbox(bbox: BoxType, rows: int, cols: int) -> BoxType:
     """Normalize coordinates of a bounding box. Divide x-coordinates by image width and y-coordinates
     by image height.
 
@@ -336,21 +347,21 @@
     elif source_format == "yolo":
         # https://github.com/pjreddie/darknet/blob/f6d861736038da22c9eb0739dca84003c5a5e275/scripts/voc_label.py#L12
         _bbox = np.array(bbox[:4])
         if check_validity and np.any((_bbox <= 0) | (_bbox > 1)):
             msg = "In YOLO format all coordinates must be float and in range (0, 1]"
             raise ValueError(msg)
 
-        (x, y, w, h), tail = bbox[:4], bbox[4:]
+        (x, y, width, height), tail = bbox[:4], bbox[4:]
 
-        w_half, h_half = w / 2, h / 2
+        w_half, h_half = width / 2, height / 2
         x_min = x - w_half
         y_min = y - h_half
-        x_max = x_min + w
-        y_max = y_min + h
+        x_max = x_min + width
+        y_max = y_min + height
     else:
         (x_min, y_min, x_max, y_max), tail = bbox[:4], bbox[4:]
 
     bbox = (x_min, y_min, x_max, y_max, *tuple(tail))
 
     if source_format != "yolo":
         bbox = normalize_bbox(bbox, rows, cols)
@@ -401,17 +412,17 @@
         width = x_max - x_min
         height = y_max - y_min
         bbox = cast(BoxType, (x_min, y_min, width, height, *tail))
     elif target_format == "yolo":
         (x_min, y_min, x_max, y_max), tail = bbox[:4], bbox[4:]
         x = (x_min + x_max) / 2.0
         y = (y_min + y_max) / 2.0
-        w = x_max - x_min
-        h = y_max - y_min
-        bbox = cast(BoxType, (x, y, w, h, *tail))
+        width = x_max - x_min
+        height = y_max - y_min
+        bbox = cast(BoxType, (x, y, width, height, *tail))
     return bbox
 
 
 def convert_bboxes_to_albumentations(
     bboxes: Sequence[BoxType],
     source_format: str,
     rows: int,
@@ -460,14 +471,38 @@
 
 def check_bboxes(bboxes: Sequence[BoxType]) -> None:
     """Check if bboxes boundaries are in range 0, 1 and minimums are lesser then maximums"""
     for bbox in bboxes:
         check_bbox(bbox)
 
 
+def clip_bbox(bbox: BoxType, rows: int, cols: int) -> BoxType:
+    """Clips the bounding box coordinates to ensure they fit within the boundaries of an image.
+
+    The function first denormalizes the bounding box coordinates from relative to absolute (pixel) values.
+    Each coordinate is then clipped to the respective dimension of the image to ensure that the bounding box
+    does not exceed the image's boundaries. Finally, the bounding box is normalized back to relative values.
+
+    Parameters:
+        bbox (BoxInternalType): The bounding box in normalized format (relative to image dimensions).
+        rows (int): The number of rows (height) in the image.
+        cols (int): The number of columns (width) in the image.
+
+    Returns:
+        BoxInternalType: The clipped bounding box, normalized to the image dimensions.
+    """
+    x_min, y_min, x_max, y_max = denormalize_bbox(bbox, rows, cols)[:4]
+
+    x_min = np.clip(x_min, 0, cols - 1)
+    x_max = np.clip(x_max, 0, cols - 1)
+    y_min = np.clip(y_min, 0, rows - 1)
+    y_max = np.clip(y_max, 0, rows - 1)
+    return cast(BoxType, normalize_bbox((x_min, y_min, x_max, y_max), rows, cols) + tuple(bbox[4:]))
+
+
 def filter_bboxes(
     bboxes: Sequence[BoxType],
     rows: int,
     cols: int,
     min_area: float = 0.0,
     min_visibility: float = 0.0,
     min_width: float = 0.0,
@@ -493,15 +528,18 @@
 
     """
     resulting_boxes: List[BoxType] = []
     for i in range(len(bboxes)):
         bbox = bboxes[i]
         # Calculate areas of bounding box before and after clipping.
         transformed_box_area = calculate_bbox_area(bbox, rows, cols)
-        bbox, tail = cast(BoxType, tuple(np.clip(bbox[:4], 0, 1.0))), tuple(bbox[4:])
+        clipped_bbox = clip_bbox(bbox, rows, cols)
+
+        bbox, tail = clipped_bbox[:4], clipped_bbox[4:]
+
         clipped_box_area = calculate_bbox_area(bbox, rows, cols)
 
         # Calculate width and height of the clipped bounding box.
         x_min, y_min, x_max, y_max = denormalize_bbox(bbox, rows, cols)[:4]
         clipped_width, clipped_height = x_max - x_min, y_max - y_min
 
         if (
@@ -529,13 +567,13 @@
         tuple: A bounding box `(x_min, y_min, x_max, y_max)`.
 
     """
     x1, y1 = width, height
     x2, y2 = 0, 0
     for bbox in bboxes:
         x_min, y_min, x_max, y_max = bbox[:4]
-        w, h = x_max - x_min, y_max - y_min
-        lim_x1, lim_y1 = x_min + erosion_rate * w, y_min + erosion_rate * h
-        lim_x2, lim_y2 = x_max - erosion_rate * w, y_max - erosion_rate * h
+        bbox_width, bbox_height = x_max - x_min, y_max - y_min
+        lim_x1, lim_y1 = x_min + erosion_rate * bbox_width, y_min + erosion_rate * bbox_height
+        lim_x2, lim_y2 = x_max - erosion_rate * bbox_width, y_max - erosion_rate * bbox_height
         x1, y1 = np.min([x1, lim_x1]), np.min([y1, lim_y1])
         x2, y2 = np.max([x2, lim_x2]), np.max([y2, lim_y2])
     return x1, y1, x2, y2
```

### Comparing `albumentations-1.4.4/albumentations/core/composition.py` & `albumentations-1.4.6/albumentations/core/composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import random
 import warnings
 from collections import defaultdict
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Union, cast
 
+import cv2
 import numpy as np
 
 from albumentations import random_utils
 
 from .bbox_utils import BboxParams, BboxProcessor
 from .keypoints_utils import KeypointParams, KeypointsProcessor
 from .serialization import (
@@ -26,20 +27,20 @@
     "OneOrOther",
     "BboxParams",
     "KeypointParams",
     "ReplayCompose",
     "Sequential",
     "TransformType",
     "TransformsSeqType",
+    "SelectiveChannelTransform",
 ]
 
-TWO = 2
-
-
+NUM_ONEOF_TRANSFORMS = 2
 REPR_INDENT_STEP = 2
+
 TransformType = Union[BasicTransform, "BaseCompose"]
 TransformsSeqType = List[TransformType]
 
 
 def get_always_apply(transforms: Union["BaseCompose", TransformsSeqType]) -> TransformsSeqType:
     new_transforms: TransformsSeqType = []
     for transform in transforms:
@@ -187,14 +188,17 @@
 
         self.add_targets(additional_targets)
 
         self.is_check_args = True
         self._disable_check_args_for_transforms(self.transforms)
 
         self.is_check_shapes = is_check_shapes
+        self._check_each_transform = tuple(  # processors that checks after each transform
+            proc for proc in self.processors.values() if getattr(proc.params, "check_each_transform", False)
+        )
 
     @staticmethod
     def _disable_check_args_for_transforms(transforms: TransformsSeqType) -> None:
         for transform in transforms:
             if isinstance(transform, BaseCompose):
                 Compose._disable_check_args_for_transforms(transform.transforms)
             if isinstance(transform, Compose):
@@ -216,42 +220,38 @@
 
         need_to_run = force_apply or random.random() < self.p
 
         for p in self.processors.values():
             p.ensure_data_valid(data)
         transforms = self.transforms if need_to_run else get_always_apply(self.transforms)
 
-        check_each_transform = any(
-            getattr(item.params, "check_each_transform", False) for item in self.processors.values()
-        )
-
         for p in self.processors.values():
             p.preprocess(data)
 
         for t in transforms:
             data = t(**data)
 
-            if check_each_transform:
+            if self._check_each_transform:
                 data = self._check_data_post_transform(data)
         data = Compose._make_targets_contiguous(data)  # ensure output targets are contiguous
 
         for p in self.processors.values():
             p.postprocess(data)
 
         return data
 
     def _check_data_post_transform(self, data: Any) -> Dict[str, Any]:
         rows, cols = get_shape(data["image"])
 
-        for p in self.processors.values():
-            if not getattr(p.params, "check_each_transform", False):
-                continue
-
-            for data_name in p.data_fields:
-                data[data_name] = p.filter(data[data_name], rows, cols)
+        for p in self._check_each_transform:
+            for data_name in data:
+                if data_name in p.data_fields or (
+                    data_name in self._additional_targets and self._additional_targets[data_name] in p.data_fields
+                ):
+                    data[data_name] = p.filter(data[data_name], rows, cols)
         return data
 
     def to_dict_private(self) -> Dict[str, Any]:
         dictionary = super().to_dict_private()
         bbox_processor = self.processors.get("bboxes")
         keypoints_processor = self.processors.get("keypoints")
         dictionary.update(
@@ -279,14 +279,15 @@
         )
         return dictionary
 
     def _check_args(self, **kwargs: Any) -> None:
         checked_single = ["image", "mask"]
         checked_multi = ["masks"]
         check_bbox_param = ["bboxes"]
+        check_keypoints_param = ["keypoints"]
         shapes = []
         for data_name, data in kwargs.items():
             internal_data_name = self._additional_targets.get(data_name, data_name)
             if internal_data_name in checked_single:
                 if not isinstance(data, np.ndarray):
                     raise TypeError(f"{data_name} must be numpy array type")
                 shapes.append(data.shape[:2])
@@ -294,14 +295,18 @@
                 if not isinstance(data[0], np.ndarray):
                     raise TypeError(f"{data_name} must be list of numpy arrays")
                 shapes.append(data[0].shape[:2])
             if internal_data_name in check_bbox_param and self.processors.get("bboxes") is None:
                 msg = "bbox_params must be specified for bbox transformations"
                 raise ValueError(msg)
 
+            if internal_data_name in check_keypoints_param and self.processors.get("keypoints") is None:
+                msg = "keypoints_params must be specified for keypoint transformations"
+                raise ValueError(msg)
+
         if self.is_check_shapes and shapes and shapes.count(shapes[0]) != len(shapes):
             msg = (
                 "Height and Width of image, mask or masks should be equal. You can disable shapes check "
                 "by setting a parameter is_check_shapes=False of Compose class (do it only if you are sure "
                 "about your data consistency)."
             )
             raise ValueError(msg)
@@ -398,60 +403,82 @@
     ):
         if transforms is None:
             if first is None or second is None:
                 msg = "You must set both first and second or set transforms argument."
                 raise ValueError(msg)
             transforms = [first, second]
         super().__init__(transforms, p)
-        if len(self.transforms) != TWO:
+        if len(self.transforms) != NUM_ONEOF_TRANSFORMS:
             warnings.warn("Length of transforms is not equal to 2.")
 
     def __call__(self, *args: Any, force_apply: bool = False, **data: Any) -> Dict[str, Any]:
         if self.replay_mode:
             for t in self.transforms:
                 data = t(**data)
             return data
 
         if random.random() < self.p:
             return self.transforms[0](force_apply=True, **data)
 
         return self.transforms[-1](force_apply=True, **data)
 
 
-class PerChannel(BaseCompose):
-    """Apply transformations per-channel
+class SelectiveChannelTransform(BaseCompose):
+    """A transformation class to apply specified transforms to selected channels of an image.
 
-    Args:
-        transforms (list): list of transformations to compose.
-        channels (sequence): channels to apply the transform to. Pass None to apply to all.
-        Default: None (apply to all)
-        p (float): probability of applying the transform. Default: 0.5.
+    This class extends BaseCompose to allow selective application of transformations to
+    specified image channels. It extracts the selected channels, applies the transformations,
+    and then reinserts the transformed channels back into their original positions in the image.
+
+    Parameters:
+        transforms (TransformsSeqType):
+            A sequence of transformations (from Albumentations) to be applied to the specified channels.
+        channels (Sequence[int]):
+            A sequence of integers specifying the indices of the channels to which the transforms should be applied.
+        always_apply (bool):
+            If True, the transform will always be applied, ignoring the probability `p`.
+        p (float):
+            Probability that the transform will be applied; the default is 1.0 (always apply).
+
+    Methods:
+        __call__(*args, **kwargs):
+            Applies the transforms to the image according to the specified channels.
+            The input data should include 'image' key with the image array.
 
+    Returns:
+        Dict[str, Any]: The transformed data dictionary, which includes the transformed 'image' key.
     """
 
-    def __init__(self, transforms: TransformsSeqType, channels: Optional[Sequence[int]] = None, p: float = 0.5):
+    def __init__(
+        self,
+        transforms: TransformsSeqType,
+        channels: Sequence[int] = (0, 1, 2),
+        always_apply: bool = False,
+        p: float = 1.0,
+    ) -> None:
         super().__init__(transforms, p)
         self.channels = channels
 
     def __call__(self, *args: Any, force_apply: bool = False, **data: Any) -> Dict[str, Any]:
         if force_apply or random.random() < self.p:
             image = data["image"]
 
-            # Expand mono images to have a single channel
-            if len(image.shape) == TWO:
-                image = np.expand_dims(image, -1)
-
-            if self.channels is None:
-                self.channels = range(image.shape[2])
-
-            for c in self.channels:
-                for t in self.transforms:
-                    image[:, :, c] = t(image=image[:, :, c])["image"]
+            selected_channels = image[:, :, self.channels]
+            sub_image = np.ascontiguousarray(selected_channels)
+
+            for t in self.transforms:
+                sub_image = t(image=sub_image)["image"]
+
+            transformed_channels = cv2.split(sub_image)
+            output_img = image.copy()
+
+            for idx, channel in zip(self.channels, transformed_channels):
+                output_img[:, :, idx] = channel
 
-            data["image"] = image
+            data["image"] = np.ascontiguousarray(output_img)
 
         return data
 
 
 class ReplayCompose(Compose):
     def __init__(
         self,
```

### Comparing `albumentations-1.4.4/albumentations/core/keypoints_utils.py` & `albumentations-1.4.6/albumentations/core/keypoints_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/core/pydantic.py` & `albumentations-1.4.6/albumentations/core/pydantic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Tuple
 
 import cv2
 from pydantic import Field
 from pydantic.functional_validators import AfterValidator
 from typing_extensions import Annotated
 
-from albumentations.core.types import ScaleType
+from albumentations.core.types import ScalarType, ScaleType
 from albumentations.core.utils import to_tuple
 
 valid_interpolations = [
     cv2.INTER_NEAREST,
     cv2.INTER_LINEAR,
     cv2.INTER_CUBIC,
     cv2.INTER_AREA,
@@ -67,28 +67,50 @@
 def create_symmetric_range(value: ScaleType) -> Tuple[float, float]:
     return to_tuple(value)
 
 
 SymmetricRangeType = Annotated[ScaleType, AfterValidator(create_symmetric_range)]
 
 
-def check_1plus_range(value: ScaleType) -> Tuple[float, float]:
-    result = to_tuple(value, low=1)
+def convert_to_1plus_range(value: ScaleType) -> Tuple[float, float]:
+    return to_tuple(value, low=1)
 
-    if not all(x >= 1 for x in result):
+
+def check_1plus_range(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
+    if any(x < 1 for x in value):
         raise ValueError(f"All values should be >= 1, got {value} instead")
-    return result
+    return value
+
+
+def check_nondecreasing_range(value: Tuple[ScalarType, ScalarType]) -> Tuple[ScalarType, ScalarType]:
+    if not value[0] <= value[1]:
+        raise ValueError(f"First value should be less than the second value, got {value} instead")
+    return value
 
 
-OnePlusFloatRangeType = Annotated[ScaleType, AfterValidator(check_1plus_range)]
-OnePlusIntRangeType = Annotated[ScaleType, AfterValidator(check_1plus_range), AfterValidator(float2int)]
+OnePlusFloatRangeType = Annotated[ScaleType, AfterValidator(convert_to_1plus_range), AfterValidator(check_1plus_range)]
+OnePlusIntRangeType = Annotated[
+    ScaleType,
+    AfterValidator(convert_to_1plus_range),
+    AfterValidator(check_1plus_range),
+    AfterValidator(float2int),
+]
+
+OnePlusIntNonDecreasingRangeType = Annotated[
+    Tuple[ScalarType, ScalarType],
+    AfterValidator(check_1plus_range),
+    AfterValidator(check_nondecreasing_range),
+    AfterValidator(float2int),
+]
 
 
-def check_01_range(value: ScaleType) -> Tuple[float, float]:
-    result = to_tuple(value, 0)
+def convert_to_0plus_range(value: ScaleType) -> Tuple[float, float]:
+    return to_tuple(value, low=0)
 
-    if not all(0 <= x <= 1 for x in result):
+
+def check_01_range(value: Tuple[float, float]) -> Tuple[float, float]:
+    if not all(0 <= x <= 1 for x in value):
         raise ValueError(f"All values should be in [0, 1], got {value} instead")
-    return result
+    return value
 
 
-ZeroOneRangeType = Annotated[ScaleType, AfterValidator(check_01_range)]
+ZeroOneRangeType = Annotated[ScaleType, AfterValidator(convert_to_0plus_range), AfterValidator(check_01_range)]
```

### Comparing `albumentations-1.4.4/albumentations/core/serialization.py` & `albumentations-1.4.6/albumentations/core/serialization.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/core/transforms_interface.py` & `albumentations-1.4.6/albumentations/core/transforms_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,33 +39,35 @@
 
 
 class CombinedMeta(SerializableMeta, ValidatedTransformMeta):
     pass
 
 
 class BasicTransform(Serializable, metaclass=CombinedMeta):
+    # `_targets` defines the types of targets (e.g., image, mask) that the transform can be applied to.
+    _targets: Union[Tuple[Targets, ...], Targets]
     call_backup = None
-    interpolation: Union[int, Interpolation]
+    interpolation: int
     fill_value: ColorType
     mask_fill_value: Optional[ColorType]
+    # replay mode params
+    deterministic: bool = False
+    save_key = "replay"
+    replay_mode = False
+    applied_in_replay = False
 
     class InitSchema(BaseTransformInitSchema):
         pass
 
     def __init__(self, always_apply: bool = False, p: float = 0.5):
         self.p = p
         self.always_apply = always_apply
         self._additional_targets: Dict[str, str] = {}
-
         # replay mode params
-        self.deterministic = False
-        self.save_key = "replay"
         self.params: Dict[Any, Any] = {}
-        self.replay_mode = False
-        self.applied_in_replay = False
 
     def __call__(self, *args: Any, force_apply: bool = False, **kwargs: Any) -> Any:
         if args:
             msg = "You have to pass data to augmentations as named arguments, for example: aug(image=image)"
             raise KeyError(msg)
         if self.replay_mode:
             if self.applied_in_replay:
@@ -81,74 +83,78 @@
                     msg = f"{self.__class__.__name__} requires {self.targets_as_params}"
                     raise ValueError(msg)
 
                 targets_as_params = {k: kwargs[k] for k in self.targets_as_params}
                 params_dependent_on_targets = self.get_params_dependent_on_targets(targets_as_params)
                 params.update(params_dependent_on_targets)
             if self.deterministic:
-                if self.targets_as_params:
-                    warn(
-                        self.get_class_fullname() + " could work incorrectly in ReplayMode for other input data"
-                        " because its' params depend on targets.",
-                    )
                 kwargs[self.save_key][id(self)] = deepcopy(params)
             return self.apply_with_params(params, **kwargs)
 
         return kwargs
 
     def apply_with_params(self, params: Dict[str, Any], *args: Any, **kwargs: Any) -> Dict[str, Any]:
-        if params is None:
-            return kwargs
+        """Apply transforms with parameters."""
         params = self.update_params(params, **kwargs)
         res = {}
         for key, arg in kwargs.items():
             if arg is not None:
                 target_function = self._get_target_function(key)
                 target_dependencies = {k: kwargs[k] for k in self.target_dependence.get(key, [])}
                 res[key] = target_function(arg, **dict(params, **target_dependencies))
             else:
                 res[key] = None
         return res
 
     def set_deterministic(self, flag: bool, save_key: str = "replay") -> "BasicTransform":
+        """Set transform to be deterministic."""
         if save_key == "params":
             msg = "params save_key is reserved"
             raise KeyError(msg)
 
         self.deterministic = flag
+        if self.deterministic and self.targets_as_params:
+            warn(
+                self.get_class_fullname() + " could work incorrectly in ReplayMode for other input data"
+                " because its' params depend on targets.",
+            )
         self.save_key = save_key
         return self
 
     def __repr__(self) -> str:
         state = self.get_base_init_args()
         state.update(self.get_transform_init_args())
         return f"{self.__class__.__name__}({format_args(state)})"
 
     def _get_target_function(self, key: str) -> Callable[..., Any]:
+        """Returns function to process target"""
         transform_key = key
         if key in self._additional_targets:
             transform_key = self._additional_targets.get(key, key)
 
         return self.targets.get(transform_key, lambda x, **p: x)
 
     def apply(self, img: np.ndarray, *args: Any, **params: Any) -> np.ndarray:
+        """Apply transform on image."""
         raise NotImplementedError
 
     def get_params(self) -> Dict[str, Any]:
+        """Returns parameters independent of input"""
         return {}
 
     @property
     def targets(self) -> Dict[str, Callable[..., Any]]:
-        # you must specify targets in subclass
-        # foe example:
-        # >>  ('image', 'mask')
-        # >>  ('image', 'boxes')
+        # mapping for targets and methods for which they depend
+        # for example:
+        # >>  {"image": self.apply}
+        # >>  {"masks": self.apply_to_masks}
         raise NotImplementedError
 
     def update_params(self, params: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
+        """Update parameters with transform specific params"""
         if hasattr(self, "interpolation"):
             params["interpolation"] = self.interpolation
         if hasattr(self, "fill_value"):
             params["fill_value"] = self.fill_value
         if hasattr(self, "mask_fill_value"):
             params["mask_fill_value"] = self.mask_fill_value
         params.update({"cols": kwargs["image"].shape[1], "rows": kwargs["image"].shape[0]})
@@ -168,35 +174,41 @@
             additional_targets (dict): keys - new target name, values - old target name. ex: {'image2': 'image'}
 
         """
         self._additional_targets = {**self._additional_targets, **additional_targets}
 
     @property
     def targets_as_params(self) -> List[str]:
+        """Targets used to get params"""
         return []
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
+        """Returns parameters dependent on targets.
+        Dependent target is defined in `self.targets_as_params`
+        """
         raise NotImplementedError(
             "Method get_params_dependent_on_targets is not implemented in class " + self.__class__.__name__,
         )
 
     @classmethod
     def get_class_fullname(cls) -> str:
         return get_shortest_class_fullname(cls)
 
     @classmethod
     def is_serializable(cls) -> bool:
         return True
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
+        """Returns names of arguments that are used in __init__ method of the transform"""
         msg = f"Class {self.get_class_fullname()} is not serializable because the `get_transform_init_args_names` "
         "method is not implemented"
         raise NotImplementedError(msg)
 
     def get_base_init_args(self) -> Dict[str, Any]:
+        """Returns base init args - always_apply and p"""
         return {"always_apply": self.always_apply, "p": self.p}
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {k: getattr(self, k) for k in self.get_transform_init_args_names()}
 
     def to_dict_private(self) -> Dict[str, Any]:
         state = {"__class_fullname__": self.get_class_fullname()}
@@ -303,15 +315,15 @@
 
     @property
     def targets(self) -> Dict[str, Callable[..., Any]]:
         return {"image": self.apply}
 
 
 class NoOp(DualTransform):
-    """Does nothing
+    """Identity transform (does nothing).
 
     Targets:
         image, mask, bboxes, keypoints, global_label
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS, Targets.GLOBAL_LABEL)
```

### Comparing `albumentations-1.4.4/albumentations/core/types.py` & `albumentations-1.4.6/albumentations/core/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,7 +61,12 @@
         JPEG (int): Represents the JPEG image compression format.
         WEBP (int): Represents the WEBP image compression format.
 
     """
 
     JPEG = 0
     WEBP = 1
+
+
+NUM_MULTI_CHANNEL_DIMENSIONS = 3
+MONO_CHANNEL_DIMENSIONS = 2
+NUM_RGB_CHANNELS = 3
```

### Comparing `albumentations-1.4.4/albumentations/core/utils.py` & `albumentations-1.4.6/albumentations/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
+from typing_extensions import Literal
 
 from .serialization import Serializable
 from .types import BoxOrKeypointType, ScalarType, ScaleType, SizeType
 
 if TYPE_CHECKING:
     import torch
 
 PAIR = 2
 
 
 def get_shape(img: Union["np.ndarray", "torch.Tensor"]) -> SizeType:
     if isinstance(img, np.ndarray):
-        rows, cols = img.shape[:2]
-        return rows, cols
+        return img.shape[:2]
 
     try:
         import torch
 
         if torch.is_tensor(img):
             return img.shape[-2:]
     except ImportError:
@@ -71,39 +71,42 @@
     def ensure_transforms_valid(self, transforms: Sequence[object]) -> None:
         pass
 
     def postprocess(self, data: Dict[str, Any]) -> Dict[str, Any]:
         rows, cols = get_shape(data["image"])
 
         for data_name in self.data_fields:
-            data[data_name] = self.filter(data[data_name], rows, cols)
-            data[data_name] = self.check_and_convert(data[data_name], rows, cols, direction="from")
+            if data_name in data:
+                data[data_name] = self.filter(data[data_name], rows, cols)
+                data[data_name] = self.check_and_convert(data[data_name], rows, cols, direction="from")
 
         return self.remove_label_fields_from_data(data)
 
     def preprocess(self, data: Dict[str, Any]) -> None:
         data = self.add_label_fields_to_data(data)
 
         rows, cols = data["image"].shape[:2]
         for data_name in self.data_fields:
-            data[data_name] = self.check_and_convert(data[data_name], rows, cols, direction="to")
+            if data_name in data:
+                data[data_name] = self.check_and_convert(data[data_name], rows, cols, direction="to")
 
     def check_and_convert(
         self,
         data: List[BoxOrKeypointType],
         rows: int,
         cols: int,
-        direction: str = "to",
+        direction: Literal["to", "from"] = "to",
     ) -> List[BoxOrKeypointType]:
         if self.params.format == "albumentations":
             self.check(data, rows, cols)
             return data
 
         if direction == "to":
             return self.convert_to_albumentations(data, rows, cols)
+
         if direction == "from":
             return self.convert_from_albumentations(data, rows, cols)
 
         raise ValueError(f"Invalid direction. Must be `to` or `from`. Got `{direction}`")
 
     @abstractmethod
     def filter(self, data: Sequence[BoxOrKeypointType], rows: int, cols: int) -> Sequence[BoxOrKeypointType]:
@@ -126,32 +129,36 @@
     ) -> List[BoxOrKeypointType]:
         pass
 
     def add_label_fields_to_data(self, data: Dict[str, Any]) -> Dict[str, Any]:
         if self.params.label_fields is None:
             return data
         for data_name in self.data_fields:
-            for field in self.params.label_fields:
-                if not len(data[data_name]) == len(data[field]):
-                    raise ValueError
-
-                data_with_added_field = []
-                for d, field_value in zip(data[data_name], data[field]):
-                    data_with_added_field.append([*list(d), field_value])
-                data[data_name] = data_with_added_field
+            if data_name in data:
+                for field in self.params.label_fields:
+                    if not len(data[data_name]) == len(data[field]):
+                        raise ValueError(
+                            f"The lengths of bboxes and labels do not match. Got {len(data[data_name])} "
+                            f"and {len(data[field])} respectively.",
+                        )
+
+                    data_with_added_field = []
+                    for d, field_value in zip(data[data_name], data[field]):
+                        data_with_added_field.append([*list(d), field_value])
+                    data[data_name] = data_with_added_field
         return data
 
     def remove_label_fields_from_data(self, data: Dict[str, Any]) -> Dict[str, Any]:
-        if self.params.label_fields is None:
+        if not self.params.label_fields:
             return data
+        label_fields_len = len(self.params.label_fields)
         for data_name in self.data_fields:
-            label_fields_len = len(self.params.label_fields)
-            for idx, field in enumerate(self.params.label_fields):
-                data[field] = [bbox[-label_fields_len + idx] for bbox in data[data_name]]
-            if label_fields_len:
+            if data_name in data:
+                for idx, field in enumerate(self.params.label_fields):
+                    data[field] = [bbox[-label_fields_len + idx] for bbox in data[data_name]]
                 data[data_name] = [d[:-label_fields_len] for d in data[data_name]]
         return data
 
 
 def to_tuple(
     param: ScaleType,
     low: Optional[ScaleType] = None,
```

### Comparing `albumentations-1.4.4/albumentations/core/validation.py` & `albumentations-1.4.6/albumentations/core/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inspect import Parameter, signature
 from typing import Any, Callable, Dict, Optional, Tuple, Type
+from warnings import warn
 
 from pydantic import BaseModel
 
 
 class ValidatedTransformMeta(type):
     def __new__(cls: Type[Any], name: str, bases: Tuple[type, ...], dct: Dict[str, Any]) -> Type[Any]:
         if "InitSchema" in dct and issubclass(dct["InitSchema"], BaseModel):
@@ -24,14 +25,19 @@
                     if name != "self" and name not in full_kwargs and param.default is not Parameter.empty:
                         full_kwargs[name] = param.default
 
                 # No try-except block needed as we want the exception to propagate naturally
                 config = dct["InitSchema"](**full_kwargs)
 
                 validated_kwargs = config.model_dump()
+                for name_arg in kwargs:
+                    if name_arg not in validated_kwargs:
+                        warn(
+                            f"Argument '{name_arg}' is not valid and will be ignored.",
+                        )
 
                 original_init(self, **validated_kwargs)
 
             # Preserve the original signature and docstring
             custom_init.__signature__ = original_sig  # type: ignore[attr-defined]
             custom_init.__doc__ = original_init.__doc__
```

### Comparing `albumentations-1.4.4/albumentations/pytorch/transforms.py` & `albumentations-1.4.6/albumentations/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/albumentations/random_utils.py` & `albumentations-1.4.6/albumentations/random_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 
 import numpy as np
 from numpy.typing import DTypeLike
 
 from .core.types import FloatNumType, IntNumType, NumType, SizeType
 
 
+def get_random_seed() -> int:
+    return py_random.randint(0, (1 << 32) - 1)
+
+
 def get_random_state() -> np.random.RandomState:
-    return np.random.RandomState(py_random.randint(0, (1 << 32) - 1))
+    return np.random.RandomState(get_random_seed())
 
 
 def uniform(
     low: NumType = 0.0,
     high: NumType = 1.0,
     size: Optional[Union[SizeType, int]] = None,
     random_state: Optional[np.random.RandomState] = None,
```

### Comparing `albumentations-1.4.4/albumentations.egg-info/PKG-INFO` & `albumentations-1.4.6/albumentations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.4
+Version: 1.4.6
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,24 +28,28 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: PyYAML
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: scikit-learn>=1.3.2
-Requires-Dist: pydantic>=2.6.4
+Requires-Dist: pydantic>=2.7.0
 Requires-Dist: opencv-python-headless>=4.9.0
 
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/albumentations.svg?label=PyPI%20downloads)](
+https://pypi.org/project/albumentations/)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/albumentations.svg?label=Conda%20downloads)](
+https://anaconda.org/conda-forge/albumentations)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
+https://stackoverflow.com/questions/tagged/albumentations)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
 [Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
```

### Comparing `albumentations-1.4.4/albumentations.egg-info/SOURCES.txt` & `albumentations-1.4.6/albumentations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 albumentations/core/types.py
 albumentations/core/utils.py
 albumentations/core/validation.py
 albumentations/pytorch/__init__.py
 albumentations/pytorch/transforms.py
 tests/test_augmentations.py
 tests/test_bbox.py
+tests/test_blur.py
 tests/test_core.py
 tests/test_functional.py
 tests/test_functional_cutout.py
 tests/test_functional_mixing.py
 tests/test_keypoint.py
 tests/test_mixing.py
 tests/test_pydantic.py
```

### Comparing `albumentations-1.4.4/pyproject.toml` & `albumentations-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,16 @@
     "D415",
     "D101",
     "D205",
     "D105",
     "D417",
     "D106",
     "EM101",
+    "COM812",
+    "B008",
 ]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
```

### Comparing `albumentations-1.4.4/setup.py` & `albumentations-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pkg_resources import DistributionNotFound, get_distribution
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
     "numpy>=1.24.4", "scipy>=1.10.0", "scikit-image>=0.21.0",
     "PyYAML", "typing-extensions>=4.9.0", "scikit-learn>=1.3.2",
-    "pydantic>=2.6.4"
+    "pydantic>=2.7.0"
 ]
 
 CHOOSE_INSTALL_REQUIRES = [
     (
         ("opencv-python>=4.9.0", "opencv-contrib-python>=4.9.0", "opencv-contrib-python-headless>=4.9.0"),
         "opencv-python-headless>=4.9.0",
     ),
```

### Comparing `albumentations-1.4.4/tests/test_augmentations.py` & `albumentations-1.4.6/tests/test_augmentations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, Tuple, Type
 
 import cv2
 import numpy as np
 import pytest
 
 import albumentations as A
+from tests.conftest import FLOAT32_IMAGES, IMAGES, SQUARE_FLOAT_IMAGE, SQUARE_IMAGES, SQUARE_UINT8_IMAGE, UINT8_IMAGES
 
 from .utils import get_dual_transforms, get_image_only_transforms, get_transforms, set_seed
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_image_only_transforms(
@@ -35,19 +36,21 @@
             }
         },
         except_augmentations={
             A.FromFloat, A.Normalize, A.ToFloat
             },
     ),
 )
-def test_image_only_augmentations_mask_persists(augmentation_cls, params, image, mask):
+def test_image_only_augmentations_mask_persists(augmentation_cls, params):
+    image = SQUARE_UINT8_IMAGE
+    mask = image.copy()
     aug = augmentation_cls(p=1, **params)
     data = aug(image=image, mask=mask)
-    assert data["image"].dtype == np.uint8
-    assert data["mask"].dtype == np.uint8
+    assert data["image"].dtype == image.dtype
+    assert data["mask"].dtype == mask.dtype
     assert np.array_equal(data["mask"], mask)
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_image_only_transforms(
         custom_arguments={
@@ -81,19 +84,21 @@
             A.FromFloat,
             A.ISONoise,
             A.Posterize,
             A.RandomToneCurve,
         },
     ),
 )
-def test_image_only_augmentations_with_float_values(augmentation_cls, params, float_image, mask):
+def test_image_only_augmentations(augmentation_cls, params):
+    image = SQUARE_FLOAT_IMAGE
+    mask = image[:, :, 0].copy().astype(np.uint8)
     aug = augmentation_cls(p=1, **params)
-    data = aug(image=float_image, mask=mask)
-    assert data["image"].dtype == np.float32
-    assert data["mask"].dtype == np.uint8
+    data = aug(image=image, mask=mask)
+    assert data["image"].dtype == image.dtype
+    assert data["mask"].dtype == mask.dtype
     assert np.array_equal(data["mask"], mask)
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_dual_transforms(
         custom_arguments={
@@ -109,32 +114,33 @@
                 "num_masks_x": (1, 3),
                 "num_masks_y": (1, 3),
                 "mask_x_length": 10,
                 "mask_y_length": 10,
                 "fill_value": 0,
                 "mask_fill_value": 1,
             },
-              A.MixUp: {
+            A.MixUp: {
                 "reference_data": [{"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
                                     "mask": np.random.randint(0, 1, [100, 100, 1], dtype=np.uint8),
                                     }],
                 "read_fn": lambda x: x,
             },
-
         },
         except_augmentations={
             A.RandomCropNearBBox, A.RandomSizedBBoxSafeCrop, A.BBoxSafeRandomCrop
             },
     ),
 )
-def test_dual_augmentations(augmentation_cls, params, image, mask):
-    aug = augmentation_cls(p=1, **params)
+def test_dual_augmentations(augmentation_cls, params):
+    image = SQUARE_UINT8_IMAGE
+    mask = image[:, :, 0].copy()
+    aug = A.Compose([augmentation_cls(p=1, **params)])
     data = aug(image=image, mask=mask)
-    assert data["image"].dtype == np.uint8
-    assert data["mask"].dtype == np.uint8
+    assert data["image"].dtype == image.dtype
+    assert data["mask"].dtype == mask.dtype
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_dual_transforms(
         custom_arguments={
             A.Crop: {"y_min": 0, "y_max": 10, "x_min": 0, "x_max": 10},
@@ -161,17 +167,19 @@
             }
         },
         except_augmentations={
             A.RandomCropNearBBox, A.RandomSizedBBoxSafeCrop, A.BBoxSafeRandomCrop
             },
     ),
 )
-def test_dual_augmentations_with_float_values(augmentation_cls, params, float_image, mask):
+def test_dual_augmentations_with_float_values(augmentation_cls, params):
+    image = SQUARE_FLOAT_IMAGE
+    mask = image.copy()[:, :, 0].astype(np.uint8)
     aug = augmentation_cls(p=1, **params)
-    data = aug(image=float_image, mask=mask)
+    data = aug(image=image, mask=mask)
     assert data["image"].dtype == np.float32
     assert data["mask"].dtype == np.uint8
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_transforms(
@@ -216,15 +224,17 @@
             }
         },
         except_augmentations={
             A.RandomCropNearBBox, A.RandomSizedBBoxSafeCrop, A.BBoxSafeRandomCrop
             },
     ),
 )
-def test_augmentations_wont_change_input(augmentation_cls, params, image, mask):
+def test_augmentations_wont_change_input(augmentation_cls, params):
+    image = np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8)
+    mask = image[:, :, 0].copy()
     image_copy = image.copy()
     mask_copy = mask.copy()
     aug = augmentation_cls(p=1, **params)
     aug(image=image, mask=mask)
     assert np.array_equal(image, image_copy)
     assert np.array_equal(mask, mask_copy)
 
@@ -284,19 +294,20 @@
             A.RandomSizedBBoxSafeCrop,
             A.BBoxSafeRandomCrop,
             A.CropNonEmptyMaskIfExists,
             A.MaskDropout,
         },
     ),
 )
-def test_augmentations_wont_change_float_input(augmentation_cls, params, float_image):
-    float_image_copy = float_image.copy()
+def test_augmentations_wont_change_float_input(augmentation_cls, params):
+    image = np.random.uniform(low=0.0, high=1.0, size=(100, 100, 3)).astype(np.float32)
+    float_image_copy = image.copy()
     aug = augmentation_cls(p=1, **params)
-    aug(image=float_image)
-    assert np.array_equal(float_image, float_image_copy)
+    aug(image=image)
+    assert np.array_equal(image, float_image_copy)
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_transforms(
         custom_arguments={
             A.HistogramMatching: {
@@ -315,15 +326,15 @@
                 "num_masks_x": (1, 3),
                 "num_masks_y": (1, 3),
                 "mask_x_length": 10,
                 "mask_y_length": 10,
                 "mask_fill_value": 1,
                 "fill_value": 0,
             },
-             A.MixUp: {
+            A.MixUp: {
                 "reference_data": [{"image": np.random.randint(0, 256, (224, 224), dtype=np.uint8),
                                     "mask": np.random.randint(0, 1, (224, 224), dtype=np.uint8),
                                     }],
                 "read_fn": lambda x: x,
             }
         },
         except_augmentations={
@@ -359,31 +370,25 @@
             A.UnsharpMask,
             A.RandomCropFromBorders,
             A.Spatter,
             A.ChromaticAberration,
         },
     ),
 )
-def test_augmentations_wont_change_shape_grayscale(augmentation_cls, params, image, mask):
+@pytest.mark.parametrize("shape", [(224, 224), (224, 224, 1)])
+def test_augmentations_wont_change_shape_grayscale(augmentation_cls, params, shape):
     aug = augmentation_cls(p=1, **params)
 
     # Test for grayscale image
-    image = np.zeros((224, 224), dtype=np.uint8)
-    mask = np.zeros((224, 224))
+    image = np.zeros(shape, dtype=np.uint8)
+    mask = np.zeros(shape)
     result = aug(image=image, mask=mask)
     assert np.array_equal(image.shape, result["image"].shape)
     assert np.array_equal(mask.shape, result["mask"].shape)
 
-    # Test for grayscale image with dummy dim
-    image_1ch = np.zeros((224, 224, 1), dtype=np.uint8)
-    mask_1ch = np.zeros((224, 224, 1))
-
-    result = aug(image=image_1ch, mask=mask_1ch)
-    assert np.array_equal(image_1ch.shape, result["image"].shape)
-    assert np.array_equal(mask_1ch.shape, result["mask"].shape)
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_transforms(
         custom_arguments={
             A.HistogramMatching: {
@@ -433,32 +438,34 @@
             A.SmallestMaxSize,
             A.PadIfNeeded,
             A.RandomScale,
             A.RandomCropFromBorders,
         },
     ),
 )
-def test_augmentations_wont_change_shape_rgb(augmentation_cls, params, image, mask):
+def test_augmentations_wont_change_shape_rgb(augmentation_cls, params):
+    shape = (224, 224, 3)
     aug = augmentation_cls(p=1, **params)
 
     # Test for RGB image
-    image_3ch = np.zeros((224, 224, 3), dtype=np.uint8)
-    mask_3ch = np.zeros((224, 224, 3))
+    image_3ch = np.zeros(shape, dtype=np.uint8)
+    mask_3ch = np.zeros(shape)
 
     result = aug(image=image_3ch, mask=mask_3ch)
     assert np.array_equal(image_3ch.shape, result["image"].shape)
     assert np.array_equal(mask_3ch.shape, result["mask"].shape)
 
 
 @pytest.mark.parametrize(["augmentation_cls", "params"], [[A.RandomCropNearBBox, {"max_part_shift": 0.15}]])
-def test_image_only_crop_around_bbox_augmentation(augmentation_cls, params, image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_image_only_crop_around_bbox_augmentation(augmentation_cls, params, image):
     aug = augmentation_cls(p=1, **params)
     annotations = {"image": image, "cropping_bbox": [-59, 77, 177, 231]}
     data = aug(**annotations)
-    assert data["image"].dtype == np.uint8
+    assert data["image"].dtype == image.dtype
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     [
         [
             A.PadIfNeeded,
```

### Comparing `albumentations-1.4.4/tests/test_bbox.py` & `albumentations-1.4.6/tests/test_bbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     denormalize_bbox,
     denormalize_bboxes,
     normalize_bbox,
     normalize_bboxes,
 )
 from albumentations.core.composition import BboxParams, Compose, ReplayCompose
 from albumentations.core.transforms_interface import NoOp
-
+import albumentations as A
 
 @pytest.mark.parametrize(
     ["bbox", "expected"],
     [((15, 25, 100, 200), (0.0375, 0.125, 0.25, 1.0)), ((15, 25, 100, 200, 99), (0.0375, 0.125, 0.25, 1.0, 99))],
 )
 def test_normalize_bbox(bbox, expected):
     normalized_bbox = normalize_bbox(bbox, 200, 400)
@@ -269,16 +269,42 @@
     np.testing.assert_almost_equal(transformed["bboxes"], transformed2["bboxes"])
 
 
 @pytest.mark.parametrize(
     ["transforms", "bboxes", "result_bboxes", "min_area", "min_visibility"],
     [
         [[Crop(10, 10, 20, 20)], [[0, 0, 10, 10, 0]], [], 0, 0],
-        [[Crop(0, 0, 90, 90)], [[0, 0, 91, 91, 0], [0, 0, 90, 90, 0]], [[0, 0, 90, 90, 0]], 0, 1],
+        [[Crop(0, 0, 90, 90)], [[0, 0, 91, 91, 0], [0, 0, 89, 89, 0]], [[0, 0, 89, 89, 0]], 0, 1],
         [[Crop(0, 0, 90, 90)], [[0, 0, 1, 10, 0], [0, 0, 1, 11, 0]], [[0, 0, 1, 10, 0], [0, 0, 1, 11, 0]], 10, 0],
     ],
 )
 def test_bbox_params_edges(transforms, bboxes, result_bboxes, min_area, min_visibility):
     image = np.empty([100, 100, 3], dtype=np.uint8)
     aug = Compose(transforms, bbox_params=BboxParams("pascal_voc", min_area=min_area, min_visibility=min_visibility))
     res = aug(image=image, bboxes=bboxes)["bboxes"]
-    assert np.allclose(res, result_bboxes)
+    assert np.array_equal(res, result_bboxes)
+
+def test_bounding_box_partially_outside_no_clip():
+    """
+    Test error is raised when bounding box exceeds image boundaries without clipping.
+    """
+    # Define a transformation with NoOp
+    transform = Compose([NoOp()],
+                        bbox_params={'format': 'pascal_voc', 'label_fields': ['labels']})
+
+    # Bounding box that exceeds the image dimensions
+    bbox = (110, 50, 140, 90)  # x_min, y_min, x_max, y_max in pixel values
+    labels = [1]
+
+    # Test should raise an error since bbox is out of image bounds and clipping is not enabled
+    with pytest.raises(ValueError):
+        transform(image=np.zeros((100, 100, 3), dtype=np.uint8), bboxes=[bbox], labels=labels)
+
+@pytest.mark.parametrize("image_size, bbox, expected_bbox", [
+    ((100, 100), (-10, -10, 110, 110), (0, 0, 99, 99)),
+    ((200, 200), (-20, -20, 220, 220), (0, 0, 199, 199)),
+    ((50, 50), (-5, -5, 55, 55), (0, 0, 49, 49))
+])
+def test_bounding_box_outside_clip(image_size, bbox, expected_bbox):
+    transform = Compose([A.NoOp()], bbox_params={'format': 'pascal_voc', 'label_fields': ['labels'], 'clip': True})
+    transformed = transform(image=np.zeros((*image_size, 3), dtype=np.uint8), bboxes=[bbox], labels=[1])
+    assert transformed['bboxes'][0] == expected_bbox
```

### Comparing `albumentations-1.4.4/tests/test_core.py` & `albumentations-1.4.6/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 from albumentations.core.composition import (
     BaseCompose,
     BboxParams,
     Compose,
     KeypointParams,
     OneOf,
     OneOrOther,
-    PerChannel,
     ReplayCompose,
     Sequential,
     SomeOf,
 )
 from albumentations.core.transforms_interface import (
     DualTransform,
     ImageOnlyTransform
 )
 from albumentations.core.utils import to_tuple
+from tests.conftest import IMAGES
 
 from .utils import get_filtered_transforms
 
 
 def test_one_or_other():
     first = MagicMock()
     second = MagicMock()
@@ -59,15 +59,15 @@
     image = np.ones((8, 8))
     augmentation(image=image)
     assert first.called
     assert second.called
 
 
 def oneof_always_apply_crash():
-    aug = Compose([HorizontalFlip(), Rotate(), OneOf([Blur(), MedianBlur()], p=1)], p=1)
+    aug = Compose([HorizontalFlip(p=1), Rotate(p=1), OneOf([Blur(p=1), MedianBlur(p=1)], p=1)], p=1)
     image = np.ones((8, 8))
     data = aug(image=image)
     assert data
 
 
 def test_always_apply():
     first = MagicMock(always_apply=True)
@@ -117,56 +117,61 @@
     (10, {"bias": 1}, (-9, 11)),
     (100, {"bias": 2}, (-98, 102)),
 ])
 def test_to_tuple(input, kwargs, expected):
     assert to_tuple(input, **kwargs) == expected
 
 
-def test_image_only_transform(image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_image_only_transform(image):
+    mask = image.copy()
     height, width = image.shape[:2]
     with mock.patch.object(ImageOnlyTransform, "apply") as mocked_apply:
         with mock.patch.object(ImageOnlyTransform, "get_params", return_value={"interpolation": cv2.INTER_LINEAR}):
             aug = ImageOnlyTransform(p=1)
             data = aug(image=image, mask=mask)
             mocked_apply.assert_called_once_with(image, interpolation=cv2.INTER_LINEAR, cols=width, rows=height)
             assert np.array_equal(data["mask"], mask)
 
-
+@pytest.mark.parametrize("image", IMAGES)
 def test_compose_doesnt_pass_force_apply(image):
     transforms = [HorizontalFlip(p=0, always_apply=False)]
     augmentation = Compose(transforms, p=1)
     result = augmentation(force_apply=True, image=image)
     assert np.array_equal(result["image"], image)
 
-
-def test_dual_transform(image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_dual_transform(image):
+    mask = image.copy()
     image_call = call(image, interpolation=cv2.INTER_LINEAR, cols=image.shape[1], rows=image.shape[0])
     mask_call = call(mask, interpolation=cv2.INTER_NEAREST, cols=mask.shape[1], rows=mask.shape[0])
     with mock.patch.object(DualTransform, "apply") as mocked_apply:
         with mock.patch.object(DualTransform, "get_params", return_value={"interpolation": cv2.INTER_LINEAR}):
             aug = DualTransform(p=1)
             aug(image=image, mask=mask)
             mocked_apply.assert_has_calls([image_call, mask_call], any_order=True)
 
 
-def test_additional_targets(image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_additional_targets(image):
+    mask = image.copy()
     image_call = call(image, interpolation=cv2.INTER_LINEAR, cols=image.shape[1], rows=image.shape[0])
     image2_call = call(mask, interpolation=cv2.INTER_LINEAR, cols=mask.shape[1], rows=mask.shape[0])
     with mock.patch.object(DualTransform, "apply") as mocked_apply:
         with mock.patch.object(DualTransform, "get_params", return_value={"interpolation": cv2.INTER_LINEAR}):
             aug = DualTransform(p=1)
             aug.add_targets({"image2": "image"})
             aug(image=image, image2=mask)
             mocked_apply.assert_has_calls([image_call, image2_call], any_order=True)
 
 
 def test_check_bboxes_with_correct_values():
     try:
         check_bboxes([[0.1, 0.5, 0.8, 1.0], [0.2, 0.5, 0.5, 0.6, 99]])
-    except Exception as e:  # skipcq: PYL-W0703
+    except Exception as e:
         pytest.fail(f"Unexpected Exception {e!r}")
 
 
 def test_check_bboxes_with_values_less_than_zero():
     with pytest.raises(ValueError) as exc_info:
         check_bboxes([[0.2, 0.5, 0.5, 0.6, 99], [-0.1, 0.5, 0.8, 1.0]])
     message = "Expected x_min for bbox [-0.1, 0.5, 0.8, 1.0] to be in the range [0.0, 1.0], got -0.1."
@@ -183,30 +188,14 @@
 def test_check_bboxes_with_end_greater_that_start():
     with pytest.raises(ValueError) as exc_info:
         check_bboxes([[0.8, 0.5, 0.7, 0.6, 99], [0.1, 0.5, 0.8, 1.0]])
     message = "x_max is less than or equal to x_min for bbox [0.8, 0.5, 0.7, 0.6, 99]."
     assert str(exc_info.value) == message
 
 
-def test_per_channel_mono():
-    transforms = [Blur(), Rotate()]
-    augmentation = PerChannel(transforms, p=1)
-    image = np.ones((8, 8))
-    data = augmentation(image=image)
-    assert data
-
-
-def test_per_channel_multi():
-    transforms = [Blur(), Rotate()]
-    augmentation = PerChannel(transforms, p=1)
-    image = np.ones((8, 8, 5))
-    data = augmentation(image=image)
-    assert data
-
-
 def test_deterministic_oneof():
     aug = ReplayCompose([OneOf([HorizontalFlip(), Blur()])], p=1)
     for _ in range(10):
         image = (np.random.random((8, 8)) * 255).astype(np.uint8)
         image2 = np.copy(image)
         data = aug(image=image)
         assert "replay" in data
@@ -299,24 +288,24 @@
             None,
             {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 95, 95, 0], [85, 85, 95, 95, 0]]},
         ],
         [
             {"bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]]},
             BboxParams("pascal_voc", check_each_transform=True),
             None,
-            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 75, 75, 0]]},
+            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 74, 74, 0]]},
         ],
         [
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
             },
             BboxParams("pascal_voc", check_each_transform=True),
             KeypointParams("xy", check_each_transform=True),
-            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 75, 75, 0]], "keypoints": np.array([[10, 10]]) + 25},
+            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 74, 74, 0]], "keypoints": np.array([[10, 10]]) + 25},
         ],
         [
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
             },
             BboxParams("pascal_voc", check_each_transform=False),
@@ -330,15 +319,15 @@
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
             },
             BboxParams("pascal_voc", check_each_transform=True),
             KeypointParams("xy", check_each_transform=False),
             {
-                "bboxes": [[25, 25, 35, 35, 0], [30, 30, 75, 75, 0]],
+                "bboxes": [[25, 25, 35, 35, 0], [30, 30, 74, 74, 0]],
                 "keypoints": np.array([[10, 10], [70, 70], [10, 70], [70, 10]]) + 25,
             },
         ],
         [
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
@@ -358,15 +347,15 @@
         [Crop(0, 0, 50, 50), PadIfNeeded(100, 100)], bbox_params=bbox_params, keypoint_params=keypoint_params
     )
     res = augs(image=image, **targets)
 
     for key, item in expected.items():
         assert np.all(np.array(item) == np.array(res[key]))
 
-
+@pytest.mark.parametrize("image", IMAGES)
 def test_bbox_params_is_not_set(image, bboxes):
     t = Compose([])
     with pytest.raises(ValueError) as exc_info:
         t(image=image, bboxes=bboxes)
     assert str(exc_info.value) == "bbox_params must be specified for bbox transformations"
 
 
@@ -454,45 +443,138 @@
     transforms.add_targets({"image2": "image"})
     with pytest.raises(ValueError) as exc_info:
         transforms.add_targets({"image2": "mask"})
     assert str(exc_info.value) == "Trying to overwrite existed additional targets. Key=image2 Exists=image New value: mask"
 
 
 # Test 1: Probability 1 with HorizontalFlip
-def test_sequential_with_horizontal_flip_prob_1(image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_sequential_with_horizontal_flip_prob_1(image):
+    mask = image.copy()
     # Setup transformations
     transform = Sequential([HorizontalFlip(p=1)], p=1)
     expected_transform = Compose([HorizontalFlip(p=1)])
 
     with patch('random.random', return_value=0.1):  # Mocking probability less than 1
         result = transform(image=image, mask=mask)
         expected = expected_transform(image=image, mask=mask)
 
     assert np.array_equal(result['image'], expected['image'])
     assert np.array_equal(result['mask'], expected['mask'])
 
 # Test 2: Probability 0 with HorizontalFlip
-def test_sequential_with_horizontal_flip_prob_0(image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_sequential_with_horizontal_flip_prob_0(image):
+    mask = image.copy()
     transform = Sequential([HorizontalFlip(p=1)], p=0)
 
     with patch('random.random', return_value=0.99):  # Mocking probability greater than 0
         result = transform(image=image, mask=mask)
 
     assert np.array_equal(result['image'], image)
     assert np.array_equal(result['mask'], mask)
 
 
-# Test 3: Multiple flips and transpose
-
+# Test 3: Multiple flips and Transpose with probability 1
+@pytest.mark.parametrize("image", IMAGES)
 @pytest.mark.parametrize("aug", [A.HorizontalFlip, A.VerticalFlip, A.Transpose])
-def test_sequential_multiple_transformations(image, mask, aug):
+def test_sequential_multiple_transformations(image, aug):
+    mask = image.copy()
+
     transform = A.Sequential([
         aug(p=1),
         aug(p=1),
     ], p=1)
 
     with patch('random.random', return_value=0.1):  # Ensuring all transforms are applied
         result = transform(image=image, mask=mask)
 
     # Since HorizontalFlip, VerticalFlip, and Transpose are all applied twice, the image should be the same
     assert np.array_equal(result['image'], image)
     assert np.array_equal(result['mask'], mask)
+
+
+@pytest.mark.parametrize(
+    "transforms",
+    [
+        [  # image only
+            A.Blur(p=1),
+            A.MedianBlur(p=1),
+            A.ToGray(p=1),
+            A.CLAHE(p=1),
+            A.RandomBrightnessContrast(p=1),
+            A.RandomGamma(p=1),
+            A.ImageCompression(quality_lower=75, p=1),
+        ],
+        [  # with dual
+            A.Blur(p=1),
+            A.MedianBlur(p=1),
+            A.ToGray(p=1),
+            A.CLAHE(p=1),
+            A.RandomBrightnessContrast(p=1),
+            A.RandomGamma(p=1),
+            A.ImageCompression(quality_lower=75, p=1),
+            A.Crop(x_max=50, y_max=50),
+        ]
+    ]
+)
+@pytest.mark.parametrize(
+    ["compose_args", "args"],
+    [
+        [
+            {},
+            {"image": np.empty([100, 100, 3], dtype=np.uint8)}
+        ],
+        [
+            {},
+            {
+                "image": np.empty([100, 100, 3], dtype=np.uint8),
+                "mask": np.empty([100, 100, 3], dtype=np.uint8),
+            }
+        ],
+        [
+            {},
+            {
+                "image": np.empty([100, 100, 3], dtype=np.uint8),
+                "masks": [np.empty([100, 100, 3], dtype=np.uint8)] * 3,
+            }
+        ],
+        [
+            dict(bbox_params=A.BboxParams(format="yolo", label_fields=["class_labels"])),
+            {
+                "image": np.empty([100, 100, 3], dtype=np.uint8),
+                "bboxes": [[0.5, 0.5, 0.1, 0.1]],
+                "class_labels": [1],
+            }
+        ],
+        [
+            dict(keypoint_params=A.KeypointParams(format="xy", label_fields=["class_labels"])),
+            {
+                "image": np.empty([100, 100, 3], dtype=np.uint8),
+                "keypoints": [[10, 20]],
+                "class_labels": [1],
+            }
+        ],
+        [
+            dict(
+                bbox_params=A.BboxParams(format="yolo", label_fields=["class_labels_1"]),
+                keypoint_params=A.KeypointParams(format="xy", label_fields=["class_labels_2"])
+            ),
+            {
+                "image": np.empty([100, 100, 3], dtype=np.uint8),
+                "mask": np.empty([100, 100, 3], dtype=np.uint8),
+                "bboxes": [[0.5, 0.5, 0.1, 0.1]],
+                "class_labels_1": [1],
+                "keypoints": [[10, 20]],
+                "class_labels_2": [1],
+            }
+        ],
+    ]
+)
+def test_common_pipeline_validity(transforms: list, compose_args: dict, args: dict):
+    # Just check that everything is fine - no errors
+
+    pipeline = A.Compose(transforms, **compose_args)
+
+    res = pipeline(**args)
+    for k in args.keys():
+        assert k in res
```

### Comparing `albumentations-1.4.4/tests/test_functional.py` & `albumentations-1.4.6/tests/test_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.augmentations.utils import get_opencv_dtype_from_numpy, is_multispectral_image, MAX_VALUES_BY_DTYPE
 from albumentations.core.bbox_utils import filter_bboxes
 from albumentations.core.types import d4_group_elements
+from tests.conftest import IMAGES, RECTANGULAR_IMAGES
 from tests.utils import convert_2d_to_target_format, set_seed
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_vflip(target):
     img = np.array([[1, 1, 1], [0, 1, 1], [0, 0, 1]], dtype=np.uint8)
     expected = np.array([[0, 0, 1], [0, 1, 1], [1, 1, 1]], dtype=np.uint8)
@@ -174,35 +175,35 @@
     """
     Generates a rotation matrix for the given angle with rotation around the center of the image.
     """
     height, width = image.shape[:2]
     center = (width / 2 - 0.5, height / 2 - 0.5)
     return cv2.getRotationMatrix2D(center, angle, 1.0)
 
-@pytest.mark.parametrize("image_type", ['image', 'float_image'])
-def test_compare_rotate_and_affine_with_fixtures(request, image_type):
-    test_image = request.getfixturevalue(image_type)
+
+@pytest.mark.parametrize("image", IMAGES)
+def test_compare_rotate_and_affine(image):
     # Generate the rotation matrix for a 60-degree rotation around the image center
-    rotation_matrix = generate_rotation_matrix(test_image, 60)
+    rotation_matrix = generate_rotation_matrix(image, 60)
 
     # Apply rotation using FGeometric.rotate
-    rotated_img_1 = FGeometric.rotate(test_image, angle=60, border_mode = cv2.BORDER_CONSTANT, value = 0)
+    rotated_img_1 = FGeometric.rotate(image, angle=60, border_mode = cv2.BORDER_CONSTANT, value = 0)
 
     # Convert 2x3 cv2 matrix to 3x3 for skimage's ProjectiveTransform
     full_matrix = np.vstack([rotation_matrix, [0, 0, 1]])
     projective_transform = skimage.transform.ProjectiveTransform(matrix=full_matrix)
 
     # Apply rotation using warp_affine
     rotated_img_2 = FGeometric.warp_affine(
-        img=test_image,
+        img=image,
         matrix=projective_transform,
         interpolation=cv2.INTER_LINEAR,
         cval=0,
         mode=cv2.BORDER_CONSTANT,
-        output_shape=test_image.shape[:2]
+        output_shape=image.shape[:2]
     )
 
     # Assert that the two rotated images are equal
     assert np.array_equal(rotated_img_1, rotated_img_2), "Rotated images should be identical."
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_center_crop(target):
@@ -643,14 +644,38 @@
 
 
 def test_bbox_random_crop():
     cropped_bbox = A.bbox_random_crop((0.5, 0.2, 0.9, 0.7), 80, 80, 0.2, 0.1, 100, 100)
     assert cropped_bbox == (0.6, 0.2, 1.1, 0.825)
 
 
+@pytest.mark.parametrize("factor, expected_positions", [
+    (1, (199, 150)),  # Rotated 90 degrees CCW
+    (2, (249, 199)), # Rotated 180 degrees
+    (3, (100, 249)),  # Rotated 270 degrees CCW
+])
+def test_keypoint_image_rot90_match(factor, expected_positions):
+    rows, cols = 300, 400  # Non-square dimensions
+    img = np.zeros((rows, cols), dtype=int)
+    # Placing the keypoint away from the center and edge: (150, 100)
+    keypoint = (150, 100, 0, 1)
+    img[keypoint[1], keypoint[0]] = 1
+
+    # Rotate the image
+    rotated_img = FGeometric.rot90(img, factor)
+
+    # Rotate the keypoint
+    rotated_keypoint = FGeometric.keypoint_rot90(keypoint, factor, img.shape[0], img.shape[1])
+
+    # Assert that the rotated keypoint lands where expected
+    assert rotated_img[rotated_keypoint[1], rotated_keypoint[0]] == 1, \
+           f"Key point after rotation factor {factor} is not at the expected position {expected_positions}, but at {rotated_keypoint}"
+
+
+
 def test_bbox_rot90():
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 0, 100, 200) == (0.1, 0.2, 0.3, 0.4)
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 1, 100, 200) == (0.2, 0.7, 0.4, 0.9)
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 2, 100, 200) == (0.7, 0.6, 0.9, 0.8)
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 3, 100, 200) == (0.6, 0.1, 0.8, 0.3)
 
 
@@ -664,19 +689,19 @@
 @pytest.mark.parametrize(
     ["bboxes", "min_area", "min_visibility", "target"],
     [
         (
             [(0.1, 0.5, 1.1, 0.9), (-0.1, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
             0,
             0,
-            [(0.1, 0.5, 1.0, 0.9), (0.0, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
+            [(0.1, 0.5, 0.99, 0.9), (0.0, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
         ),
         ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.5, 0.5, 0.6)], 150, 0, [(0.1, 0.5, 0.8, 0.9)]),
         ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.9, 0.5, 1.6)], 0, 0.75, [(0.1, 0.5, 0.8, 0.9)]),
-        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 1.1)], 0, 0.7, [(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 1.0)]),
+        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 1.1)], 0, 0.7, [(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 0.99)]),
     ],
 )
 def test_filter_bboxes(bboxes, min_area, min_visibility, target):
     filtered_bboxes = filter_bboxes(bboxes, min_area=min_area, min_visibility=min_visibility, rows=100, cols=100)
     assert filtered_bboxes == target
 
 
@@ -1045,26 +1070,26 @@
     assert get_opencv_dtype_from_numpy(np.dtype("float64")) == cv2.CV_64F
     assert get_opencv_dtype_from_numpy(np.dtype("int32")) == cv2.CV_32S
 
 
 @pytest.mark.parametrize(
     ["image", "mean", "std"],
     [
-        [np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8), [0.485, 0.456, 0.406], [0.229, 0.224, 0.225]],
-        [np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8), 0.5, 0.5],
-        [np.random.randint(0, 256, [100, 100], dtype=np.uint8), 0.5, 0.5],
+        [np.random.randint(0, 256, [101, 99, 3], dtype=np.uint8), [0.485, 0.456, 0.406], [0.229, 0.224, 0.225]],
+        [np.random.randint(0, 256, [101, 99, 3], dtype=np.uint8), 0.5, 0.5],
+        [np.random.randint(0, 256, [101, 99], dtype=np.uint8), 0.5, 0.5],
     ],
 )
 def test_normalize_np_cv_equal(image, mean, std):
     mean = np.array(mean, dtype=np.float32)
     std = np.array(std, dtype=np.float32)
 
     res1 = F.normalize_cv2(image, mean, std)
     res2 = F.normalize_numpy(image, mean, std)
-    assert np.allclose(res1, res2)
+    assert np.array_equal(res1, res2)
 
 
 @pytest.mark.parametrize("beta_by_max", [True, False])
 def test_brightness_contrast_adjust_equal(beta_by_max):
     image_int = np.random.randint(0, 256, [512, 512, 3], dtype=np.uint8)
     image_float = image_int.astype(np.float32) / 255
 
@@ -1200,22 +1225,47 @@
 
 def get_md5_hash(image):
     image_bytes = image.tobytes()
     hash_md5 = hashlib.md5()
     hash_md5.update(image_bytes)
     return hash_md5.hexdigest()
 
-
+@pytest.mark.parametrize("image", IMAGES)
 def test_d4_unique(image):
     hashes = set()
     for element in d4_group_elements:
         hashes.add(get_md5_hash(FGeometric.d4(image, element)))
 
     assert len(hashes) == len(set(hashes)), "d4 should generate unique images for all group elements"
 
+@pytest.mark.parametrize("image", RECTANGULAR_IMAGES)
+@pytest.mark.parametrize("group_member", d4_group_elements)
+def test_d4_output_shape(image, group_member):
+    result = FGeometric.d4(image, group_member)
+    if group_member in ['r90', 'r270', 't', 'hvt']:
+        assert result.shape[:2] == image.shape[:2][::-1], "Output shape should be the transpose of input shape"
+    else:
+        assert result.shape == image.shape, "Output shape should match input shape"
+
+
+@pytest.mark.parametrize("image", RECTANGULAR_IMAGES)
+def test_d4_output_shape(image):
+    result = FGeometric.transpose(image)
+    assert result.shape[:2] == image.shape[:2][::-1], "Output shape should be the transpose of input shape"
+
+
+@pytest.mark.parametrize("image", RECTANGULAR_IMAGES)
+@pytest.mark.parametrize("factor", [0, 1, 2, 3])
+def test_d4_output_shape(image, factor):
+    result = FGeometric.rot90(image, factor)
+    if factor in {1, 3}:
+        assert result.shape[:2] == image.shape[:2][::-1], "Output shape should be the transpose of input shape"
+    else:
+        assert result.shape == image.shape, "Output shape should match input shape"
+
 
 
 @pytest.mark.parametrize("bbox, group_member, rows, cols, expected", [
     ((0.05, 0.1, 0.55, 0.6), 'e', 200, 200, (0.05, 0.1, 0.55, 0.6)),  # Identity
     ((0.05, 0.1, 0.55, 0.6), 'r90', 200, 200, (0.1, 0.45, 0.6, 0.95)),  # Rotate 90 degrees CCW
     ((0.05, 0.1, 0.55, 0.6), 'r180', 200, 200, (0.45, 0.4, 0.95, 0.9)),  # Rotate 180 degrees
     ((0.05, 0.1, 0.55, 0.6), 'r270', 200, 200, (0.4, 0.05, 0.9, 0.55)),  # Rotate 270 degrees CCW
@@ -1242,15 +1292,14 @@
 
     vflipped_keypoint = FGeometric.keypoint_vflip(keypoint, rows, cols)
     hvflipped_keypoint = FGeometric.keypoint_hflip(vflipped_keypoint, rows, cols)
 
     assert vhflipped_keypoint == pytest.approx(hvflipped_keypoint), "Sequential vflip + hflip not equivalent to hflip + vflip"
     assert vhflipped_keypoint == pytest.approx(FGeometric.keypoint_rot90(keypoint, 2, rows, cols)), "rot180 not equivalent to vflip + hflip"
 
-
 base_matrix = np.array([[1, 2, 3],
                         [4, 5, 6],
                         [7, 8, 9]])
 expected_main_diagonal = np.array([[1, 4, 7],
                                    [2, 5, 8],
                                    [3, 6, 9]])
 expected_second_diagonal = np.array([[9, 6, 3],
```

### Comparing `albumentations-1.4.4/tests/test_functional_mixing.py` & `albumentations-1.4.6/tests/test_functional_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/tests/test_keypoint.py` & `albumentations-1.4.6/tests/test_keypoint.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/tests/test_mixing.py` & `albumentations-1.4.6/tests/test_mixing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import pytest
 import math
 
 import albumentations as A
+from tests.conftest import IMAGES, UINT8_IMAGES
+from tests.utils import set_seed
 from .test_functional_mixing import find_mix_coef
 
 def image_generator():
     yield {"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8)}
 
 def complex_image_generator():
     height = 100
@@ -35,17 +37,18 @@
               }),
               (A.MixUp, {
             "reference_data": image_generator(),
             "read_fn": lambda x: x}),
               (A.MixUp, {
             "reference_data": complex_image_generator(),
             "read_fn": complex_read_fn_image})] )
-def test_image_only(augmentation_cls, params, image):
+def test_image_only(augmentation_cls, params):
+    square_image = UINT8_IMAGES[0]
     aug = A.Compose([augmentation_cls(p=1, **params)], p=1)
-    data = aug(image=image)
+    data = aug(image=square_image)
     assert data["image"].dtype == np.uint8
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
              [(A.MixUp, {
                 "reference_data": [{"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
                                    "global_label": np.array([0, 0, 1])}],
@@ -53,31 +56,32 @@
             (A.MixUp, {
                   "reference_data": [1],
                   "read_fn": lambda x: {"image": np.ones((100, 100, 3)).astype(np.uint8),
                                         "global_label": np.array([0, 0, 1])}},
               ),
               ]
 )
-def test_image_global_label(augmentation_cls, params, image, global_label):
+def test_image_global_label(augmentation_cls, params, global_label):
+    square_image = UINT8_IMAGES[0]
     aug = A.Compose([augmentation_cls(p=1, **params)], p=1)
 
-    data = aug(image=image, global_label=global_label)
+    data = aug(image=square_image, global_label=global_label)
 
     assert data["image"].dtype == np.uint8
 
     reference_data = params["reference_data"][0]
 
     reference_item = params["read_fn"](reference_data)
 
     reference_image = reference_item["image"]
     reference_global_label = reference_item["global_label"]
 
     mix_coef = data["mix_coef"]
 
-    mix_coeff_image = find_mix_coef(data["image"], image, reference_image)
+    mix_coeff_image = find_mix_coef(data["image"], square_image, reference_image)
     mix_coeff_label = find_mix_coef(data["global_label"], global_label, reference_global_label)
 
     assert math.isclose(mix_coef, mix_coeff_image, abs_tol=0.01)
     assert math.isclose(mix_coeff_image, mix_coeff_label, abs_tol=0.01)
     assert 0 <= mix_coeff_image <= 1
 
 @pytest.mark.parametrize(
@@ -85,51 +89,69 @@
              [(A.MixUp, {
                 "reference_data": [{"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
                                     "mask": np.random.randint(0, 256, (100, 100, 1), dtype=np.uint8),
                                    "global_label": np.array([0, 0, 1])}],
 
                 "read_fn": lambda x: x})]
 )
-def test_image_mask_global_label(augmentation_cls, params, image, mask, global_label):
+def test_image_mask_global_label(augmentation_cls, params, global_label):
+    image = UINT8_IMAGES[0]
+    mask = image[:, :, 0].copy()
+
+    reference_data = params["reference_data"][0]
+
     aug = A.Compose([augmentation_cls(p=1, **params)], p=1)
 
     data = aug(image=image, global_label=global_label, mask=mask)
 
-    reference_data = params["reference_data"][0]
 
     mix_coef = data["mix_coef"]
 
     mix_coeff_image = find_mix_coef(data["image"], image, reference_data["image"])
     mix_coeff_mask = find_mix_coef(data["mask"], mask, reference_data["mask"])
     mix_coeff_label = find_mix_coef(data["global_label"], global_label, reference_data["global_label"])
 
     assert math.isclose(mix_coef, mix_coeff_image, abs_tol=0.01)
     assert math.isclose(mix_coeff_image, mix_coeff_label, abs_tol=0.01)
     assert math.isclose(mix_coeff_image, mix_coeff_mask, abs_tol=0.01)
     assert 0 <= mix_coeff_image <= 1
 
+@pytest.mark.parametrize("image", IMAGES)
+def test_additional_targets(image, global_label):
+    set_seed(42)
+
+    mask = image.copy()
+    image1 = np.random.randint(0, 256, image.shape, dtype=np.uint8).astype(image.dtype)
+    mask1 = np.random.randint(0, 256, mask.shape, dtype=np.uint8).astype(mask.dtype)
+    reference_image = np.random.randint(0, 256, image.shape, dtype=np.uint8).astype(image.dtype)
+    reference_mask = np.random.randint(0, 256, mask.shape, dtype=np.uint8).astype(mask.dtype)
+
+    if image.dtype == np.float32:
+        image /= 255
+        mask1 /= 255
+        image1 /= 255
+        mask1 /= 255
+        reference_image /= 255
+        reference_mask /= 255
 
-def test_additional_targets(image, mask, global_label):
-    reference_data = [{"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
-                                    "mask": np.random.randint(0, 256, (100, 100), dtype=np.uint8),
+    reference_data = [{"image": reference_image,
+                                    "mask": reference_mask,
                                    "global_label": np.array([0, 0, 1])}]
 
 
     aug = A.Compose([A.MixUp(p=1, reference_data=reference_data, read_fn = lambda x: x)], additional_targets={'image1': 'image', 'mask1': 'mask',
                                                                            'global_label1': 'global_label'})
 
-    image1 = np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8)
-    mask1 = np.random.randint(0, 256, (100, 100), dtype=np.uint8)
     global_label1 = np.array([0, 1, 0])
 
     data = aug(image=image, global_label=global_label, mask=mask, image1=image1, global_label1=global_label1, mask1=mask1)
 
     mix_coef = data["mix_coef"]
 
-    assert data["image"].dtype == np.uint8
+    assert data["image"].dtype == image.dtype
 
     mix_coeff_image = find_mix_coef(data["image"], image, reference_data[0]["image"])
     mix_coeff_mask = find_mix_coef(data["mask"], mask, reference_data[0]["mask"])
     mix_coeff_label = find_mix_coef(data["global_label"], global_label, reference_data[0]["global_label"])
 
     mix_coeff_image1 = find_mix_coef(data["image1"], image1, reference_data[0]["image"])
     mix_coeff_mask1 = find_mix_coef(data["mask1"], mask1, reference_data[0]["mask"])
@@ -141,55 +163,62 @@
     assert math.isclose(mix_coeff_image, mix_coeff_mask, abs_tol=0.01)
     assert 0 <= mix_coeff_image <= 1
 
     assert math.isclose(mix_coeff_image, mix_coeff_image1, abs_tol=0.01)
     assert math.isclose(mix_coeff_image, mix_coeff_mask1, abs_tol=0.01)
     assert math.isclose(mix_coeff_image, mix_coeff_label1, abs_tol=0.01)
 
+@pytest.mark.parametrize("image", IMAGES)
+def test_bbox_error(image, global_label, bboxes):
+    mask = image.copy()
 
-def test_bbox_error(image, mask, global_label, bboxes):
     reference_data = [
-        {"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
-         "mask": np.random.randint(0, 256, (100, 100, 1), dtype=np.uint8),
+        {"image": np.random.randint(0, 256, image.shape, dtype=np.uint8).astype(image.dtype),
+         "mask": np.random.randint(0, 256, mask.shape, dtype=np.uint8).astype(mask.dtype),
          "bboxes": [[15, 12, 75, 30, 1], [55, 25, 90, 90, 2]],
          "global_label": np.array([0, 0, 1])}
         ]
 
     aug = A.Compose([A.MixUp(p=1, reference_data=reference_data, read_fn=lambda x: x)], p=1, bbox_params=A.BboxParams(format="pascal_voc", min_area=16))
 
     with pytest.raises(NotImplementedError):
         aug(image=image, global_label=global_label, mask=mask, bboxes=bboxes)
 
-def test_keypoint_error(image, mask, global_label, keypoints):
+@pytest.mark.parametrize("image", IMAGES)
+def test_keypoint_error(image, global_label, keypoints):
+    mask = image.copy()
+
     reference_data = [
-        {"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
-         "mask": np.random.randint(0, 256, (100, 100, 1), dtype=np.uint8),
+        {"image": np.random.randint(0, 256, image.shape, dtype=np.uint8).astype(image.dtype),
+         "mask": np.random.randint(0, 256, mask.shape, dtype=np.uint8).astype(mask.dtype),
          "keypoints": [[20, 30, 40, 50, 1], [20, 30, 60, 80, 2]],
          "global_label": np.array([0, 0, 1])}
     ]
 
     aug = A.Compose([A.MixUp(p=1, reference_data=reference_data, read_fn=lambda x: x)], p=1, keypoint_params=A.KeypointParams(format="xy"))
 
     with pytest.raises(NotImplementedError):
         aug(image=image, global_label=global_label, mask=mask, keypoints=keypoints)
 
+@pytest.mark.parametrize("image", IMAGES)
+@pytest.mark.parametrize( ["augmentation_cls", "params"], [(A.ColorJitter, {"p": 1}), (A.HorizontalFlip, {"p": 1})])
+def test_pipeline(augmentation_cls, params, image, global_label):
+    mask = image.copy()
 
-@pytest.mark.parametrize( ["augmentation_cls", "params"], [(A.CLAHE, {"p": 1}), (A.HorizontalFlip, {"p": 1})])
-def test_pipeline(augmentation_cls, params, image, mask, global_label):
-    reference_data =[{"image": np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8),
-                     "mask": np.random.randint(0, 256, (100, 100, 1), dtype=np.uint8),
+    reference_data =[{"image": np.random.randint(0, 256, image.shape, dtype=np.uint8).astype(image.dtype),
+                     "mask": np.random.randint(0, 256, mask.shape, dtype=np.uint8).astype(mask.dtype),
                      "global_label": np.array([0, 0, 1])}]
 
     mix_up = A.MixUp(p=1, reference_data=reference_data, read_fn=lambda x: x)
 
     aug = A.Compose([augmentation_cls(**params), mix_up], p=1)
 
     data = aug(image=image, global_label=global_label, mask=mask)
 
-    assert data["image"].dtype == np.uint8
+    assert data["image"].dtype == image.dtype
 
     mix_coef = data["mix_coef"]
 
     mix_coeff_label = find_mix_coef(data["global_label"], global_label, reference_data[0]["global_label"])
 
     assert math.isclose(mix_coef, mix_coeff_label, abs_tol=0.01)
     assert 0 <= mix_coeff_label <= 1
```

### Comparing `albumentations-1.4.4/tests/test_pydantic.py` & `albumentations-1.4.6/tests/test_pydantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional
+import warnings
 import pytest
 import cv2
 
 from pydantic import BaseModel, ValidationError
 import albumentations as A
 from inspect import signature, Parameter
 from albumentations.core.transforms_interface import ImageOnlyTransform
@@ -96,38 +97,38 @@
     (5, (-5.0, 5.0)),
     ((-1, 1), (-1.0, 1.0)),
 ])
 def test_create_symmetric_range(value, expected):
     assert create_symmetric_range(value) == expected
 
 @pytest.mark.parametrize("value", [
-    (0.9),  # Invalid input
+    (0, 0.9),  # Invalid input
+    (0, 1.1),  # Invalid input
 ])
 def test_check_1plus_range_with_invalid_input(value):
     with pytest.raises(ValueError):
         check_1plus_range(value)
 
 @pytest.mark.parametrize("value,expected", [
     ((1, 2), (1.0, 2.0)),
-    (2, (1.0, 2.0)),
 ])
 def test_check_1plus_range_with_valid_input(value, expected):
     assert check_1plus_range(value) == expected
 
 @pytest.mark.parametrize("value", [
-    (-0.1),
-    (1.2),
+    (0, -0.1),
+    (2, 1.2),
 ])
 def test_check_01_range_with_invalid_input(value):
     with pytest.raises(ValueError):
         check_01_range(value)
 
 @pytest.mark.parametrize("value,expected", [
     ((0, 1), (0.0, 1.0)),
-    ((0.3), (0.0, 0.3)),
+    ((0, 0.3), (0.0, 0.3)),
 ])
 def test_check_01_range_with_valid_input(value, expected):
     assert check_01_range(value) == expected
 
 class ValidationModel(BaseModel):
     interpolation: Optional[InterpolationType] = None
     border_mode: Optional[BorderModeType] = None
@@ -300,7 +301,19 @@
     assert 'p' in expected_params
     assert expected_params['p'] == Parameter('p', kind=Parameter.POSITIONAL_OR_KEYWORD, default=0.5, annotation=float)
 
     # Ensure the correct defaults and types
     assert expected_params['always_apply'].default is False
     assert expected_params['p'].default == 0.5
     assert expected_params['custom_param'].annotation is int
+
+
+def test_wrong_argument() -> None:
+    """Test that pas Transform will get warning"""
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        transform = A.Crop(wrong_param=10)
+        assert not hasattr(transform, "wrong_param")
+        assert len(w) == 1
+        assert issubclass(w[0].category, UserWarning)
+        assert str(w[0].message) == "Argument 'wrong_param' is not valid and will be ignored."
+    warnings.resetwarnings()
```

### Comparing `albumentations-1.4.4/tests/test_pytorch.py` & `albumentations-1.4.6/tests/test_pytorch.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,45 +2,55 @@
 import pytest
 import torch
 from PIL import Image
 from torchvision.transforms import ColorJitter
 
 import albumentations as A
 from albumentations.pytorch.transforms import ToTensorV2
+from tests.conftest import UINT8_IMAGES
 from .utils import set_seed
 
 
-def test_torch_to_tensor_v2_augmentations(image, mask):
+@pytest.mark.parametrize("image", UINT8_IMAGES)
+def test_torch_to_tensor_v2_augmentations(image):
+    mask = image.copy()
     aug = ToTensorV2()
     data = aug(image=image, mask=mask, force_apply=True)
     height, width, num_channels = image.shape
     assert isinstance(data["image"], torch.Tensor) and data["image"].shape == (num_channels, height, width)
     assert isinstance(data["mask"], torch.Tensor) and data["mask"].shape == mask.shape
     assert data["image"].dtype == torch.uint8
     assert data["mask"].dtype == torch.uint8
 
 
-def test_torch_to_tensor_v2_augmentations_with_transpose_2d_mask(image, mask):
+@pytest.mark.parametrize("image", UINT8_IMAGES)
+def test_torch_to_tensor_v2_augmentations_with_transpose_2d_mask(image):
+    mask = image[:, :, 0].copy()
+
     aug = ToTensorV2(transpose_mask=True)
+
     data = aug(image=image, mask=mask, force_apply=True)
     image_height, image_width, image_num_channels = image.shape
     mask_height, mask_width = mask.shape
+
     assert isinstance(data["image"], torch.Tensor) and data["image"].shape == (
         image_num_channels,
         image_height,
         image_width,
     )
     assert isinstance(data["mask"], torch.Tensor) and data["mask"].shape == (mask_height, mask_width)
     assert data["image"].dtype == torch.uint8
     assert data["mask"].dtype == torch.uint8
 
 
+@pytest.mark.parametrize("image", UINT8_IMAGES)
 def test_torch_to_tensor_v2_augmentations_with_transpose_3d_mask(image):
     aug = ToTensorV2(transpose_mask=True)
-    mask = np.random.randint(low=0, high=256, size=(100, 100, 4), dtype=np.uint8)
+    mask_shape = image.shape[:2] + (4,)
+    mask = np.random.randint(low=0, high=256, size=mask_shape, dtype=np.uint8)
     data = aug(image=image, mask=mask, force_apply=True)
     image_height, image_width, image_num_channels = image.shape
     mask_height, mask_width, mask_num_channels = mask.shape
     assert isinstance(data["image"], torch.Tensor) and data["image"].shape == (
         image_num_channels,
         image_height,
         image_width,
```

### Comparing `albumentations-1.4.4/tests/test_random.py` & `albumentations-1.4.6/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/tests/test_serialization.py` & `albumentations-1.4.6/tests/test_serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 from deepdiff import DeepDiff
 
 import albumentations as A
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.core.serialization import SERIALIZABLE_REGISTRY, shorten_class_name
 from albumentations.core.transforms_interface import ImageOnlyTransform
 from albumentations.core.types import ImageCompressionType
+from tests.conftest import FLOAT32_IMAGES, IMAGES, SQUARE_UINT8_IMAGE, UINT8_IMAGES
+
 
 from .utils import (
     OpenMock,
     check_all_augs_exists,
     get_image_only_transforms,
     get_transforms,
     set_seed,
 )
 
+images = []
+
 TEST_SEEDS = (0, 1, 42)
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_transforms(
         custom_arguments={
             A.Crop: {"y_min": 0, "y_max": 10, "x_min": 0, "x_max": 10},
@@ -72,15 +76,18 @@
             A.MixUp
         },
     ),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
-def test_augmentations_serialization(augmentation_cls, params, p, seed, image, mask, always_apply):
+@pytest.mark.parametrize("image", IMAGES)
+def test_augmentations_serialization(augmentation_cls, params, p, seed, image, always_apply):
+    mask = image.copy()
+
     aug = augmentation_cls(p=p, always_apply=always_apply, **params)
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
     aug_data = aug(image=image, mask=mask)
     set_seed(seed)
     deserialized_aug_data = deserialized_aug(image=image, mask=mask)
@@ -106,15 +113,15 @@
     [A.Blur, {"blur_limit": 3}],
     [A.MotionBlur, {"blur_limit": 3}],
     [A.MedianBlur, {"blur_limit": 3}],
     [A.GaussianBlur, {"blur_limit": 3}],
     [A.GaussNoise, {"var_limit": (20, 90), "mean": 10, "per_channel": False}],
     [A.CLAHE, {"clip_limit": 2, "tile_grid_size": (12, 12)}],
     [A.RandomGamma, {"gamma_limit": (10, 90)}],
-    [A.CoarseDropout, {"max_holes": 4, "max_height": 4, "max_width": 4}],
+    [A.CoarseDropout, {"num_holes_range": (2, 5), "hole_height_range": (3, 4), "hole_width_range": (4, 6)}],
     [
         A.RandomSnow,
         {"snow_point_lower": 0.2, "snow_point_upper": 0.4, "brightness_coeff": 4},
     ],
     [
         A.RandomRain,
         {
@@ -469,39 +476,43 @@
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     check_all_augs_exists(AUGMENTATION_CLS_PARAMS, AUGMENTATION_CLS_EXCEPT),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
+@pytest.mark.parametrize("image", UINT8_IMAGES)
 def test_augmentations_serialization_with_custom_parameters(
-    augmentation_cls, params, p, seed, image, mask, always_apply
+    augmentation_cls, params, p, seed, image, always_apply
 ):
+    mask = image[:, :, 0].copy()
     aug = augmentation_cls(p=p, always_apply=always_apply, **params)
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
     aug_data = aug(image=image, mask=mask)
     set_seed(seed)
     deserialized_aug_data = deserialized_aug(image=image, mask=mask)
     assert np.array_equal(aug_data["image"], deserialized_aug_data["image"])
     assert np.array_equal(aug_data["mask"], deserialized_aug_data["mask"])
 
 
+@pytest.mark.parametrize("image", UINT8_IMAGES)
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     check_all_augs_exists(AUGMENTATION_CLS_PARAMS, AUGMENTATION_CLS_EXCEPT),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
 @pytest.mark.parametrize("data_format", ("yaml", "json"))
 def test_augmentations_serialization_to_file_with_custom_parameters(
-    augmentation_cls, params, p, seed, image, mask, always_apply, data_format
+    augmentation_cls, params, p, seed, image, always_apply, data_format
 ):
+    mask = image[:, :, 0].copy()
     with patch("builtins.open", OpenMock()):
         aug = augmentation_cls(p=p, always_apply=always_apply, **params)
         filepath = f"serialized.{data_format}"
         A.save(aug, filepath, data_format=data_format)
         deserialized_aug = A.load(filepath, data_format=data_format)
         set_seed(seed)
         aug_data = aug(image=image, mask=mask)
@@ -549,14 +560,15 @@
             A.Morphological
         },
     ),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
+@pytest.mark.parametrize("image", UINT8_IMAGES)
 def test_augmentations_for_bboxes_serialization(
     augmentation_cls, params, p, seed, image, albumentations_bboxes, always_apply
 ):
     aug = augmentation_cls(p=p, always_apply=always_apply, **params)
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
@@ -613,14 +625,15 @@
             A.Morphological
         },
     ),
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
+@pytest.mark.parametrize("image", UINT8_IMAGES)
 def test_augmentations_for_keypoints_serialization(augmentation_cls, params, p, seed, image, keypoints, always_apply):
     aug = augmentation_cls(p=p, always_apply=always_apply, **params)
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
     aug_data = aug(image=image, keypoints=keypoints)
     set_seed(seed)
@@ -638,39 +651,43 @@
             {"cropping_bbox": [-59, 77, 177, 231]},
         ]
     ],
 )
 @pytest.mark.parametrize("p", [0.5, 1])
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("always_apply", (False, True))
+@pytest.mark.parametrize("image", IMAGES)
 def test_augmentations_serialization_with_call_params(
     augmentation_cls, params, call_params, p, seed, image, always_apply
 ):
     aug = augmentation_cls(p=p, always_apply=always_apply, **params)
     annotations = {"image": image, **call_params}
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
     aug_data = aug(**annotations)
     set_seed(seed)
     deserialized_aug_data = deserialized_aug(**annotations)
     assert np.array_equal(aug_data["image"], deserialized_aug_data["image"])
 
 
-def test_from_float_serialization(float_image):
+@pytest.mark.parametrize("image", FLOAT32_IMAGES)
+def test_from_float_serialization(image):
     aug = A.FromFloat(p=1, dtype="uint8")
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
-    aug_data = aug(image=float_image)
-    deserialized_aug_data = deserialized_aug(image=float_image)
+    aug_data = aug(image=image)
+    deserialized_aug_data = deserialized_aug(image=image)
     assert np.array_equal(aug_data["image"], deserialized_aug_data["image"])
 
 
 @pytest.mark.parametrize("seed", TEST_SEEDS)
-def test_transform_pipeline_serialization(seed, image, mask):
+@pytest.mark.parametrize("image", IMAGES)
+def test_transform_pipeline_serialization(seed, image):
+    mask = image.copy()
     aug = A.Compose(
         [
             A.OneOrOther(
                 A.Compose(
                     [
                         A.Resize(1024, 1024),
                         A.RandomSizedCrop(min_max_height=(256, 1024), size=(512, 512), p=1),
@@ -697,15 +714,15 @@
                         A.OneOf([A.HueSaturationValue(p=0.5), A.RGBShift(p=0.7)], p=1),
                     ]
                 ),
             ),
             A.SomeOf(
                 [
                     A.HorizontalFlip(p=1),
-                    A.Transpose(p=1),
+                    A.D4(p=1),
                     A.HueSaturationValue(p=0.5),
                     A.RandomBrightnessContrast(p=0.5),
                 ],
                 2,
                 replace=False,
             ),
         ]
@@ -728,14 +745,15 @@
         ([(20, 30, 60, 80)], "pascal_voc", [2]),
         ([(20, 30, 60, 80, 99)], "pascal_voc", [1]),
         ([(0.2, 0.3, 0.4, 0.5)], "yolo", [2]),
         ([(0.2, 0.3, 0.4, 0.5, 99)], "yolo", [1]),
     ],
 )
 @pytest.mark.parametrize("seed", TEST_SEEDS)
+@pytest.mark.parametrize("image", IMAGES)
 def test_transform_pipeline_serialization_with_bboxes(seed, image, bboxes, bbox_format, labels):
     aug = A.Compose(
         [
             A.OneOrOther(
                 A.Compose(
                     [
                         A.RandomRotate90(),
@@ -748,15 +766,15 @@
                         A.OneOf([A.HueSaturationValue(p=0.5), A.RGBShift(p=0.7)], p=1),
                     ]
                 ),
             ),
             A.SomeOf(
                 [
                     A.HorizontalFlip(p=1),
-                    A.Transpose(p=1),
+                    A.D4(p=1),
                     A.HueSaturationValue(p=0.5),
                     A.RandomBrightnessContrast(p=0.5),
                 ],
                 n=5,
             ),
         ],
         bbox_params={"format": bbox_format, "label_fields": ["labels"]},
@@ -777,14 +795,15 @@
         ([(20, 30, 40, 50)], "xyas", [1]),
         ([(20, 30, 40, 50, 99), (10, 40, 30, 20, 9)], "xy", [1, 2]),
         ([(20, 30, 60, 80)], "yx", [2]),
         ([(20, 30, 60, 80, 99)], "xys", [1]),
     ],
 )
 @pytest.mark.parametrize("seed", TEST_SEEDS)
+@pytest.mark.parametrize("image", IMAGES)
 def test_transform_pipeline_serialization_with_keypoints(seed, image, keypoints, keypoint_format, labels):
     aug = A.Compose(
         [
             A.OneOrOther(
                 A.Compose(
                     [
                         A.RandomRotate90(),
@@ -829,19 +848,21 @@
             A.FDA,
             A.PixelDistributionAdaptation,
             A.TemplateTransform,
         },
     ),
 )
 @pytest.mark.parametrize("seed", TEST_SEEDS)
+@pytest.mark.parametrize("image", UINT8_IMAGES)
 def test_additional_targets_for_image_only_serialization(augmentation_cls, params, image, seed):
     aug = A.Compose(
         [augmentation_cls(always_apply=True, **params)],
         additional_targets={"image2": "image"},
     )
+
     image2 = image.copy()
 
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
     aug_data = aug(image=image, image2=image2)
     set_seed(seed)
@@ -849,27 +870,30 @@
 
     assert np.array_equal(aug_data["image"], deserialized_aug_data["image"])
     assert np.array_equal(aug_data["image2"], deserialized_aug_data["image2"])
 
 
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("p", [1])
-def test_lambda_serialization(image, mask, albumentations_bboxes, keypoints, seed, p):
+@pytest.mark.parametrize("image", IMAGES)
+def test_lambda_serialization(image, albumentations_bboxes, keypoints, seed, p):
     def vflip_image(image, **kwargs):
         return FGeometric.vflip(image)
 
     def vflip_mask(mask, **kwargs):
         return FGeometric.vflip(mask)
 
     def vflip_bbox(bbox, **kwargs):
         return FGeometric.bbox_vflip(bbox, **kwargs)
 
     def vflip_keypoint(keypoint, **kwargs):
         return FGeometric.keypoint_vflip(keypoint, **kwargs)
 
+    mask = image.copy()
+
     aug = A.Lambda(
         name="vflip",
         image=vflip_image,
         mask=vflip_mask,
         bbox=vflip_bbox,
         keypoint=vflip_keypoint,
         p=p,
@@ -994,15 +1018,16 @@
 )
 def test_shorten_class_name(class_fullname, expected_short_class_name):
     assert shorten_class_name(class_fullname) == expected_short_class_name
 
 
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("p", [1])
-def test_template_transform_serialization(image, template, seed, p):
+def test_template_transform_serialization(template, seed, p):
+    image = SQUARE_UINT8_IMAGE
     template_transform = A.TemplateTransform(name="template", templates=template, p=p)
 
     aug = A.Compose([A.Flip(), template_transform, A.Blur()])
 
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug, nonserializable={"template": template_transform})
 
@@ -1042,33 +1067,35 @@
         },                                                                        except_augmentations={
             A.FDA,
             A.HistogramMatching,
             A.PixelDistributionAdaptation,
             A.Lambda,
             A.TemplateTransform,
             A.MixUp,
-            A.ShiftScaleRotate,
         }) )
 def test_augmentations_serialization(augmentation_cls, params):
     instance = augmentation_cls(**params)
 
     def get_all_init_schema_fields(model_cls):
         """
         Recursively collects fields from InitSchema classes defined in the given augmentation class
         and its base classes.
 
         Args:
             model_cls (Type): The augmentation class possibly containing an InitSchema class.
 
         Returns:
-            Set[str]: A set of field names collected from all InitSchema classes.
+            Set[str]: A set of field names collected from all InitSchema classes, excluding
+                  fields marked as deprecated.
         """
         fields = set()
         if hasattr(model_cls, 'InitSchema'):
-            fields |= set(model_cls.InitSchema.model_fields.keys())
+            for field_name, field in model_cls.InitSchema.model_fields.items():
+                if not field.deprecated:
+                    fields.add(field_name)
 
         for base in model_cls.__bases__:
             fields |= get_all_init_schema_fields(base)
 
         return fields
 
     model_fields = get_all_init_schema_fields(augmentation_cls)
```

### Comparing `albumentations-1.4.4/tests/test_targets.py` & `albumentations-1.4.6/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.4/tests/test_transforms.py` & `albumentations-1.4.6/tests/test_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import warnings
 from torchvision import transforms as torch_transforms
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.augmentations.blur.functional import gaussian_blur
+from albumentations.random_utils import get_random_seed
+from tests.conftest import IMAGES, SQUARE_MULTI_UINT8_IMAGE, SQUARE_UINT8_IMAGE
 
 from .utils import get_dual_transforms, get_image_only_transforms, get_transforms, set_seed
 
 
 
 def test_transpose_both_image_and_mask():
     image = np.ones((8, 6, 3))
@@ -94,36 +96,41 @@
     assert np.array_equal(data["image"].shape, (size, size, 3))
 
 
 @pytest.mark.parametrize("interpolation", [cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC])
 def test_elastic_transform_interpolation(monkeypatch, interpolation):
     image = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
     mask = np.random.randint(low=0, high=2, size=(100, 100), dtype=np.uint8)
+
+    random_seed = get_random_seed()
+
     monkeypatch.setattr(
-        "albumentations.augmentations.geometric.ElasticTransform.get_params", lambda *_: {"random_state": 1111}
+        "albumentations.augmentations.geometric.ElasticTransform.get_params", lambda *_: {"random_seed": random_seed}
     )
+
     aug = A.ElasticTransform(alpha=1, sigma=50, alpha_affine=50, interpolation=interpolation, p=1)
+
     data = aug(image=image, mask=mask)
     expected_image = FGeometric.elastic_transform(
         image,
         alpha=1,
         sigma=50,
         alpha_affine=50,
         interpolation=interpolation,
         border_mode=cv2.BORDER_REFLECT_101,
-        random_state=np.random.RandomState(1111),
+        random_state=np.random.RandomState(random_seed),
     )
     expected_mask = FGeometric.elastic_transform(
         mask,
         alpha=1,
         sigma=50,
         alpha_affine=50,
         interpolation=cv2.INTER_NEAREST,
         border_mode=cv2.BORDER_REFLECT_101,
-        random_state=np.random.RandomState(1111),
+        random_state=np.random.RandomState(random_seed),
     )
     assert np.array_equal(data["image"], expected_image)
     assert np.array_equal(data["mask"], expected_mask)
 
 
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
@@ -311,15 +318,15 @@
         res = aug(image=image1, image2=image2)
         aug1 = res["image"]
         aug2 = res["image2"]
         assert np.array_equal(aug1, aug2)
 
     aug = A.Compose([augmentation_cls(always_apply=True, **params)])
     aug.add_targets(additional_targets={"image2": "image"})
-    for _i in range(10):
+    for _ in range(10):
         image1 = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
         image2 = image1.copy()
         res = aug(image=image1, image2=image2)
         aug1 = res["image"]
         aug2 = res["image2"]
         assert np.array_equal(aug1, aug2)
 
@@ -698,34 +705,14 @@
 
 @pytest.mark.parametrize(
     ["blur_limit", "sigma", "result_blur", "result_sigma"],
     [
         [[0, 0], [1, 1], 0, 1],
         [[1, 1], [0, 0], 1, 0],
         [[1, 1], [1, 1], 1, 1],
-        [[0, 0], [0, 0], 3, 0],
-        [[0, 3], [0, 0], 3, 0],
-        [[0, 3], [0.1, 0.1], 3, 0.1],
-    ],
-)
-def test_gaus_blur_limits(blur_limit, sigma, result_blur, result_sigma):
-    img = np.zeros([100, 100, 3], dtype=np.uint8)
-
-    aug = A.Compose([A.GaussianBlur(blur_limit=blur_limit, sigma_limit=sigma, p=1)])
-
-    res = aug(image=img)["image"]
-    assert np.allclose(res, gaussian_blur(img, result_blur, result_sigma))
-
-
-@pytest.mark.parametrize(
-    ["blur_limit", "sigma", "result_blur", "result_sigma"],
-    [
-        [[0, 0], [1, 1], 0, 1],
-        [[1, 1], [0, 0], 1, 0],
-        [[1, 1], [1, 1], 1, 1],
     ],
 )
 def test_unsharp_mask_limits(blur_limit, sigma, result_blur, result_sigma):
     img = np.zeros([100, 100, 3], dtype=np.uint8)
 
     aug = A.Compose([A.UnsharpMask(blur_limit=blur_limit, sigma_limit=sigma, p=1)])
 
@@ -841,41 +828,17 @@
             res1 = t1(image=img)["image"]
             res2 = (t2(image=img.astype(np.float32) / 255.0)["image"] * 255).astype(np.uint8)
 
             _max = np.abs(res1.astype(np.int32) - res2).max()
             assert _max <= 10, f"Max value: {_max}"
 
 
-@pytest.mark.parametrize(["val_uint8"], [[0], [1], [128], [255]])
-def test_glass_blur_float_uint8_diff_less_than_two(val_uint8):
-    x_uint8 = np.zeros((5, 5)).astype(np.uint8)
-    x_uint8[2, 2] = val_uint8
-
-    x_float32 = np.zeros((5, 5)).astype(np.float32)
-    x_float32[2, 2] = val_uint8 / 255.0
-
-    glassblur = A.GlassBlur(always_apply=True, max_delta=1)
-
-    set_seed(0)
-    blur_uint8 = glassblur(image=x_uint8)["image"]
-
-    set_seed(0)
-    blur_float32 = glassblur(image=x_float32)["image"]
-
-    # Before comparison, rescale the blur_float32 to [0, 255]
-    diff = np.abs(blur_uint8 - blur_float32 * 255)
-
-    # The difference between the results of float32 and uint8 will be at most 2.
-    assert np.all(diff <= 2.0)
-
-
 def test_perspective_keep_size():
     h, w = 100, 100
     img = np.zeros([h, w, 3], dtype=np.uint8)
-    h, w = img.shape[:2]
     bboxes = []
     for _ in range(10):
         x1 = np.random.randint(0, w - 1)
         y1 = np.random.randint(0, h - 1)
         x2 = np.random.randint(x1 + 1, w)
         y2 = np.random.randint(y1 + 1, h)
         bboxes.append([x1, y1, x2, y2])
@@ -883,25 +846,25 @@
 
     transform_1 = A.Compose(
         [A.Perspective(keep_size=True, p=1)],
         keypoint_params=A.KeypointParams("xys"),
         bbox_params=A.BboxParams("pascal_voc", label_fields=["labels"]),
     )
     transform_2 = A.Compose(
-        [A.Perspective(keep_size=False, p=1), A.Resize(h, w)],
+        [A.Perspective(keep_size=False, p=1), A.Resize(h, w, p=1)],
         keypoint_params=A.KeypointParams("xys"),
         bbox_params=A.BboxParams("pascal_voc", label_fields=["labels"]),
     )
 
     set_seed(0)
     res_1 = transform_1(image=img, bboxes=bboxes, keypoints=keypoints, labels=[0] * len(bboxes))
     set_seed(0)
     res_2 = transform_2(image=img, bboxes=bboxes, keypoints=keypoints, labels=[0] * len(bboxes))
 
-    assert np.allclose(res_1["bboxes"], res_2["bboxes"])
+    assert np.allclose(res_1["bboxes"], res_2["bboxes"], atol=0.2)
     assert np.allclose(res_1["keypoints"], res_2["keypoints"])
 
 
 def test_longest_max_size_list():
     img = np.random.randint(0, 256, [50, 10], np.uint8)
     keypoints = [(9, 5, 0, 0)]
 
@@ -978,52 +941,14 @@
     message = (
         "Template must be a single channel or has the same number of channels "
         "as input image ({}), got {}".format(img_channels, template.shape[-1])
     )
     assert str(exc_info.value) == message
 
 
-@pytest.mark.parametrize(["val_uint8"], [[0], [1], [128], [255]])
-def test_advanced_blur_float_uint8_diff_less_than_two(val_uint8):
-    x_uint8 = np.zeros((5, 5)).astype(np.uint8)
-    x_uint8[2, 2] = val_uint8
-
-    x_float32 = np.zeros((5, 5)).astype(np.float32)
-    x_float32[2, 2] = val_uint8 / 255.0
-
-    adv_blur = A.AdvancedBlur(blur_limit=(3, 5), always_apply=True)
-
-    set_seed(0)
-    adv_blur_uint8 = adv_blur(image=x_uint8)["image"]
-
-    set_seed(0)
-    adv_blur_float32 = adv_blur(image=x_float32)["image"]
-
-    # Before comparison, rescale the adv_blur_float32 to [0, 255]
-    diff = np.abs(adv_blur_uint8 - adv_blur_float32 * 255)
-
-    # The difference between the results of float32 and uint8 will be at most 2.
-    assert np.all(diff <= 2.0)
-
-
-@pytest.mark.parametrize(
-    ["params"],
-    [
-        [{"blur_limit": (2, 5)}],
-        [{"blur_limit": (3, 6)}],
-        [{"sigma_x_limit": (0.0, 1.0), "sigma_y_limit": (0.0, 1.0)}],
-        [{"beta_limit": (0.1, 0.9)}],
-        [{"beta_limit": (1.1, 8.0)}],
-    ],
-)
-def test_advanced_blur_raises_on_incorrect_params(params):
-    with pytest.raises(ValueError):
-        A.AdvancedBlur(**params)
-
-
 @pytest.mark.parametrize(
     ["params"],
     [
         [{"scale": (0.5, 1.0)}],
         [{"scale": (0.5, 1.0), "keep_ratio": False}],
         [{"scale": (0.5, 1.0), "keep_ratio": True}],
     ],
@@ -1076,16 +1001,16 @@
                     [199, 99, 20, 20],
                     [0, 99, 30, 30],
                 ],
             },
             {
                 "bboxes": [
                     [15.65896994771262, 0.2946228229078849, 21.047137067150473, 4.617219579173327, 0],
-                    [194.29851584295034, 25.564320319214918, 199.68668296238818, 29.88691707548036, 0],
-                    [178.9528629328495, 95.38278042082668, 184.34103005228735, 99.70537717709212, 0],
+                    [194.29851584295034, 25.564320319214918, 199, 29.88691707548036, 0],
+                    [178.9528629328495, 95.38278042082668, 184.34103005228735, 99, 0],
                     [0.47485022613917677, 70.11308292451965, 5.701484157049652, 73.70074852182076, 0],
                 ],
                 "keypoints": [
                     [16.466635890349504, 0.2946228229078849, 147.04220486917677, 0.0],
                     [198.770582727028, 26.08267308836993, 157.04220486917674, 9.30232558139535],
                     [182.77879706281766, 98.84085782583904, 167.04220486917674, 18.6046511627907],
                     [0.4748502261391767, 73.05280756037699, 177.04220486917674, 27.90697674418604],
@@ -1108,15 +1033,15 @@
                     [0, 99, 30, 30],
                 ],
             },
             {
                 "bboxes": [
                     [0.3133170376117963, 25.564320319214918, 5.701484157049649, 29.88691707548036, 0],
                     [178.9528629328495, 0.2946228229078862, 184.34103005228735, 4.617219579173327, 0],
-                    [194.29851584295034, 70.11308292451965, 199.68668296238818, 74.43567968078509, 0],
+                    [194.29851584295034, 70.11308292451965, 199, 74.43567968078509, 0],
                     [15.658969947712617, 95.38278042082668, 20.88560387862309, 98.97044601812779, 0],
                 ],
                 "keypoints": [
                     [0.3133170376117963, 26.212261280658684, 212.95779513082323, 0.0],
                     [182.6172638742903, 0.42421101519664006, 222.95779513082323, 9.30232558139535],
                     [198.60904953850064, 73.18239575266574, 232.9577951308232, 18.6046511627907],
                     [16.305102701822126, 98.97044601812779, 242.9577951308232, 27.906976744186046],
@@ -1191,32 +1116,32 @@
     assert np.allclose(res_a["image"], res_b["image"])
     res_a = np.array(res_a["keypoints"])
     res_b = np.array(res_b["keypoints"])
     diff = np.round(np.abs(res_a - res_b))
     assert diff[:, :2].max() <= 2
     assert (diff[:, -1] % 360).max() <= 1
 
-
 @pytest.mark.parametrize(
     "get_transform",
     [
         lambda sign: A.Affine(translate_px=sign * 2),
         lambda sign: A.ShiftScaleRotate(shift_limit=(sign * 0.02, sign * 0.02), scale_limit=0, rotate_limit=0),
     ],
 )
 @pytest.mark.parametrize(
     ["bboxes", "expected", "min_visibility", "sign"],
     [
         [[(0, 0, 10, 10, 1)], [], 0.9, -1],
         [[(0, 0, 10, 10, 1)], [(0, 0, 8, 8, 1)], 0.6, -1],
         [[(90, 90, 100, 100, 1)], [], 0.9, 1],
-        [[(90, 90, 100, 100, 1)], [(92, 92, 100, 100, 1)], 0.6, 1],
+        [[(90, 90, 100, 100, 1)], [(92, 92, 99, 99, 1)], 0.49, 1],
     ],
 )
-def test_bbox_clipping(get_transform, image, bboxes, expected, min_visibility: float, sign: int):
+def test_bbox_clipping(get_transform, bboxes, expected, min_visibility: float, sign: int):
+    image = np.zeros([100, 100, 3], dtype=np.uint8)
     transform = get_transform(sign)
     transform.p = 1
     transform = A.Compose([transform], bbox_params=A.BboxParams(format="pascal_voc", min_visibility=min_visibility))
 
     res = transform(image=image, bboxes=bboxes)["bboxes"]
     assert res == expected
 
@@ -1319,36 +1244,16 @@
 
     image = np.random.randint(0, 256, (224, 224, 3), dtype=np.uint8)
     transformed_image_albu = transform_albu(image=image)['image']
     transform_albu_height_is_size = transform_albu_new(image=image)['image']
     assert transformed_image_albu.shape == transformed_image_pt_np.shape
     assert transform_albu_height_is_size.shape == transformed_image_pt_np.shape
 
-@pytest.mark.parametrize("size, width, height, expected_warning", [
-    ((100, 200), None, None, None),
-    (None, 200, 100, DeprecationWarning),
-    (100, None, None, TypeError),
-])
-def test_deprecation_warnings(size, width, height, expected_warning):
-    with warnings.catch_warnings(record=True) as w:
-        warnings.simplefilter("always")
-        if expected_warning == TypeError:
-            with pytest.raises(TypeError):
-                A.RandomResizedCrop(size=size, width=width, height=height)
-        else:
-            A.RandomResizedCrop(size=size, width=width, height=height)
-        if expected_warning is DeprecationWarning:
-            assert len(w) == 1
-            assert issubclass(w[-1].category, expected_warning)
-        else:
-            assert not w
-    warnings.resetwarnings()
-
-
 @pytest.mark.parametrize("num_shadows_limit, num_shadows_lower, num_shadows_upper, expected_warning", [
+    ((1, 1), None, None, None),
     ((1, 2), None, None, None),
     ((2, 3), None, None, None),
     ((1, 2), 1, None, DeprecationWarning),
     ((1, 2), None, 2, DeprecationWarning),
     ((1, 2), 1, 2, DeprecationWarning),
     ((2, 1), None, None, ValueError),
 ])
@@ -1358,42 +1263,251 @@
     num_shadows_upper: Optional[int],
     expected_warning: Optional[Type[Warning]],
 ) -> None:
     """
     Test deprecation warnings for RandomShadow
     """
     with warnings.catch_warnings(record=True) as w:
-        warnings.simplefilter("always")
+        warnings.simplefilter("always")  # Change the filter to capture all warnings
         if expected_warning == ValueError:
             with pytest.raises(ValueError):
                 A.RandomShadow(num_shadows_limit=num_shadows_limit, num_shadows_lower=num_shadows_lower,
                                num_shadows_upper=num_shadows_upper, p=1)
-        else:
+        elif expected_warning is DeprecationWarning:
             A.RandomShadow(num_shadows_limit=num_shadows_limit, num_shadows_lower=num_shadows_lower,
                            num_shadows_upper=num_shadows_upper, p=1)
-        if expected_warning is DeprecationWarning:
-            assert len(w) == 1
-            assert issubclass(w[-1].category, expected_warning)
-        else:
-            assert not w
-    warnings.resetwarnings()
+            for warning in w:
+                print(f"Warning captured: {warning.category.__name__}, Message: '{warning.message}'")
 
+                if warning.category is DeprecationWarning:
+                    print(f"Deprecation Warning: {warning.message}")
+            assert any(issubclass(warning.category, DeprecationWarning) for warning in w), \
+                "No DeprecationWarning found"
+        else:
+            assert not w, "Unexpected warnings raised"
 
+@pytest.mark.parametrize("image", IMAGES)
 @pytest.mark.parametrize("grid", [
-    (2, 2), (3, 3), (4, 4), (5, 7)
+    (3, 3), (4, 4), (5, 7)
 ])
-def test_grid_shuffle(image, mask, grid):
-    set_seed(4)
+def test_grid_shuffle(image, grid):
+    """
+    As we reshuffle the grid, the mean and sum of the image and mask should remain the same,
+    while the reshuffled image and mask should not be equal to the original image and mask.
+    """
+    set_seed(0)
+
+    mask = image.copy()
+
     aug = A.Compose([A.RandomGridShuffle(grid=grid, p=1)])
 
     res = aug(image=image, mask=mask)
     assert res["image"].shape == image.shape
     assert res["mask"].shape == mask.shape
 
     assert not np.array_equal(res["image"], image)
     assert not np.array_equal(res["mask"], mask)
 
-    assert np.array_equal(res["image"].mean(axis=(0, 1)), image.mean(axis=(0, 1)))
-    assert np.array_equal(res["image"].sum(axis=(0, 1)), image.sum(axis=(0, 1)))
+    np.testing.assert_allclose(res["image"].sum(axis=(0, 1)), image.sum(axis=(0, 1)), atol=0.03)
+    np.testing.assert_allclose(res["mask"].sum(axis=(0, 1)), mask.sum(axis=(0, 1)), atol=0.03)
+
+@pytest.mark.parametrize("image", IMAGES)
+@pytest.mark.parametrize("crop_left, crop_right, crop_top, crop_bottom", [
+    (0, 0, 0, 0),
+    (0, 1, 0, 1),
+    (1, 0, 1, 0),
+    (0.5, 0.5, 0.5, 0.5),
+    ( 0.1, 0.1, 0.1, 0.1 ),
+                                                                          ( 0.3, 0.3, 0.3, 0.3 )])
+def test_random_crop_from_borders(image, bboxes, keypoints, crop_left, crop_right, crop_top, crop_bottom):
+    set_seed(0)
+    aug = A.Compose([A.RandomCropFromBorders(crop_left=crop_left,
+                                             crop_right=crop_right,
+                                             crop_top=crop_top,
+                                             crop_bottom=crop_bottom,
+                                             p=1)],
+                    bbox_params=A.BboxParams("pascal_voc"),
+                    keypoint_params=A.KeypointParams("xy"))
+
+    assert aug(image=image, mask=image, bboxes=bboxes, keypoints=keypoints)
+
+@pytest.mark.parametrize("params, expected", [
+    # Default values
+    ({}, {"num_holes_range": (1, 1), "hole_height_range": (8, 8), "hole_width_range": (8, 8)}),
+    # Boundary values
+    ({"num_holes_range": (2, 3)}, {"num_holes_range": (2, 3)}),
+    ({"hole_height_range": (0.1, 0.1)}, {"hole_height_range": (0.1, 0.1)}),
+    ({"hole_width_range": (0.1, 0.1)}, {"hole_width_range": (0.1, 0.1)}),
+    # Random fill value
+    ({"fill_value": 'random'}, {"fill_value": 'random'}),
+    ({"fill_value": (255, 255, 255)}, {"fill_value": (255, 255, 255)}),
+    # Deprecated values handling
+    ({"min_holes": 1, "max_holes": 5}, {"num_holes_range": (1, 5)}),
+    ({"min_height": 2, "max_height": 6}, {"hole_height_range": (2, 6)}),
+    ({"min_width": 3, "max_width": 7}, {"hole_width_range": (3, 7)}),
+])
+def test_coarse_dropout_functionality(params, expected):
+    aug = A.CoarseDropout(**params, p=1)
+    aug_dict = aug.to_dict()["transform"]
+    for key, value in expected.items():
+        assert aug_dict[key] == value, f"Failed on {key} with value {value}"
 
-    assert np.array_equal(res["mask"].mean(axis=(0, 1)), mask.mean(axis=(0, 1)))
-    assert np.array_equal(res["mask"].sum(axis=(0, 1)), mask.sum(axis=(0, 1)))
+
+@pytest.mark.parametrize("params", [
+    ({"num_holes_range": (5, 1)}),  # Invalid range
+    ({"num_holes_range": (0, 3)}),  # Invalid range
+    ({"hole_height_range": (2.1, 3)}),  # Invalid type
+    ({"hole_height_range": ('a', 'b')}),  # Invalid type
+])
+def test_coarse_dropout_invalid_input(params):
+    with pytest.raises(Exception):
+        aug = A.CoarseDropout(**params, p=1)
+
+
+@pytest.mark.parametrize(
+    ["augmentation_cls", "params"],
+    get_transforms(
+        custom_arguments={
+            A.Crop: {"y_min": 0, "y_max": 10, "x_min": 0, "x_max": 10},
+            A.CenterCrop: {"height": 10, "width": 10},
+            A.CropNonEmptyMaskIfExists: {"height": 10, "width": 10},
+            A.RandomCrop: {"height": 10, "width": 10},
+            A.RandomResizedCrop: {"height": 10, "width": 10},
+            A.RandomSizedCrop: {"min_max_height": (4, 8), "height": 10, "width": 10},
+            A.CropAndPad: {"px": 10},
+            A.Resize: {"height": 10, "width": 10},
+            A.TemplateTransform: {
+                "templates": np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8),
+            },
+            A.XYMasking: {
+                "num_masks_x": (1, 3),
+                "num_masks_y": (1, 3),
+                "mask_x_length": 10,
+                "mask_y_length": 10,
+                "mask_fill_value": 1,
+                "fill_value": 0,
+            },
+            A.Superpixels: {"p_replace": (1, 1),
+                             "n_segments": (10, 10),
+                             "max_size": 10
+                            },
+        },
+        except_augmentations={
+            A.RandomCropNearBBox,
+            A.RandomSizedBBoxSafeCrop,
+            A.BBoxSafeRandomCrop,
+            A.CropNonEmptyMaskIfExists,
+            A.FDA,
+            A.HistogramMatching,
+            A.PixelDistributionAdaptation,
+            A.MaskDropout,
+            A.MixUp,
+            A.NoOp,
+            A.Lambda,
+            A.ToRGB,
+            A.RandomRotate90,
+            A.FancyPCA
+        },
+    ),
+)
+def test_change_image(augmentation_cls, params):
+    """Checks whether transform performs changes to the image."""
+    aug = A.Compose([augmentation_cls(p=1, **params)])
+    image = SQUARE_UINT8_IMAGE
+    assert not np.array_equal(aug(image=image)["image"], image)
+
+@pytest.mark.parametrize(
+    ["augmentation_cls", "params"],
+    get_transforms(
+        custom_arguments={
+            A.XYMasking: {
+                "num_masks_x": (1, 3),
+                "num_masks_y": (1, 3),
+                "mask_x_length": 10,
+                "mask_y_length": 10,
+                "mask_fill_value": 1,
+                "fill_value": 0,
+            },
+            A.Superpixels: {"p_replace": (1, 1),
+                             "n_segments": (10, 10),
+                             "max_size": 10
+                            },
+            A.FancyPCA: {"alpha":1}
+        },
+        except_augmentations={
+            A.Crop,
+            A.CenterCrop,
+            A.CropNonEmptyMaskIfExists,
+            A.RandomCrop,
+            A.RandomResizedCrop,
+            A.RandomSizedCrop,
+            A.CropAndPad,
+            A.Resize,
+            A.TemplateTransform,
+            A.RandomCropNearBBox,
+            A.RandomSizedBBoxSafeCrop,
+            A.BBoxSafeRandomCrop,
+            A.CropNonEmptyMaskIfExists,
+            A.FDA,
+            A.HistogramMatching,
+            A.PixelDistributionAdaptation,
+            A.MaskDropout,
+            A.MixUp,
+            A.NoOp,
+            A.Lambda,
+            A.ToRGB,
+            A.ChannelDropout,
+            A.LongestMaxSize,
+            A.PadIfNeeded,
+            A.RandomCropFromBorders,
+            A.SmallestMaxSize,
+            A.RandomScale,
+            A.ChannelShuffle,
+            A.ChromaticAberration,
+            A.RandomRotate90,
+            A.FancyPCA
+        },
+    ),
+)
+def test_selective_channel(augmentation_cls, params):
+    set_seed(0)
+
+    image = SQUARE_MULTI_UINT8_IMAGE
+    channels = [3, 2, 4]
+
+    aug = A.Compose(
+        [A.SelectiveChannelTransform(transforms=[augmentation_cls(**params, always_apply=True, p=1)], channels=channels, always_apply=True, p=1)],
+    )
+
+    transformed_image = aug(image=image)["image"]
+
+    for channel in range(image.shape[-1]):
+        if channel in channels:
+            assert not np.array_equal(image[..., channel], transformed_image[..., channel])
+        else:
+            assert np.array_equal(image[..., channel], transformed_image[..., channel])
+
+
+@pytest.mark.parametrize("params, expected", [
+    # Default values
+    ({}, {"scale_range": (0.25, 0.25), "interpolation_pair": {"downscale": cv2.INTER_NEAREST, "upscale": cv2.INTER_NEAREST}}),
+    # Boundary values
+    ({"scale_range": (0.1, 0.9)}, {"scale_range": (0.1, 0.9)}),
+    ({"interpolation_pair": {"downscale": cv2.INTER_LINEAR, "upscale": cv2.INTER_CUBIC}}, {"interpolation_pair": {"downscale": cv2.INTER_LINEAR, "upscale": cv2.INTER_CUBIC}}),
+    # Deprecated values handling
+    ({"scale_min": 0.1, "scale_max": 0.9}, {"scale_range": (0.1, 0.9)}),
+    ({"interpolation": cv2.INTER_AREA}, {"interpolation_pair": {"downscale": cv2.INTER_AREA, "upscale": cv2.INTER_AREA}}),
+])
+def test_downscale_functionality(params, expected):
+    aug = A.Downscale(**params, p=1)
+    aug_dict = aug.get_transform_init_args()
+    for key, value in expected.items():
+        assert aug_dict[key] == value, f"Failed on {key} with value {value}"
+
+@pytest.mark.parametrize("params", [
+    ({"scale_range": (0.9, 0.1)}),  # Invalid range, max < min
+    ({"scale_range": (1.1, 1.2)}),  # Values outside valid scale range (0, 1)
+    ({"interpolation_pair": {"downscale": 9999, "upscale": 9999}}),  # Invalid interpolation method
+])
+def test_downscale_invalid_input(params):
+    with pytest.raises(Exception):
+        aug = A.Downscale(**params, p=1)
```

