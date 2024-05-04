# Comparing `tmp/kan_gpt-0.1.2.tar.gz` & `tmp/kan_gpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-0.1.2.tar", last modified: Sat May  4 07:34:34 2024, max compression
+gzip compressed data, was "kan_gpt-0.1.3.tar", last modified: Sat May  4 14:00:52 2024, max compression
```

## Comparing `kan_gpt-0.1.2.tar` & `kan_gpt-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.602879 kan_gpt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-04 07:34:34.602879 kan_gpt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.590879 kan_gpt-0.1.2/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.594879 kan_gpt-0.1.2/kan_gpt/efficient_kan/
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/efficient_kan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.594879 kan_gpt-0.1.2/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:34:34.602879 kan_gpt-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_efficient_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_kan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.897132 kan_gpt-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-04 14:00:52.897132 kan_gpt-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.889132 kan_gpt-0.1.3/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.889132 kan_gpt-0.1.3/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.889132 kan_gpt-0.1.3/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.893132 kan_gpt-0.1.3/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.893132 kan_gpt-0.1.3/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.897132 kan_gpt-0.1.3/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-04 14:00:52.000000 kan_gpt-0.1.3/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 14:00:52.000000 kan_gpt-0.1.3/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:00:52.000000 kan_gpt-0.1.3/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 14:00:52.000000 kan_gpt-0.1.3/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 14:00:52.000000 kan_gpt-0.1.3/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 14:00:52.000000 kan_gpt-0.1.3/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:00:52.897132 kan_gpt-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:52.897132 kan_gpt-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 14:00:42.000000 kan_gpt-0.1.3/tests/test_kan.py
```

### Comparing `kan_gpt-0.1.2/HISTORY.md` & `kan_gpt-0.1.3/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Fix(dataset): padding and range fix. [Aditya NG]
+
+
+0.1.2 (2024-05-04)
+------------------
+- Release: version 0.1.2 🚀 [Aditya NG]
 - Feat(kan_gpt/efficient_kan/): integration with efficient kan reduced
   training memory footprint. [Aditya NG]
 - Test(gpt-pico): reducing memory footprint. [Aditya NG]
 
 
 0.1.1 (2024-05-04)
 ------------------
```

### Comparing `kan_gpt-0.1.2/LICENSE` & `kan_gpt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/PKG-INFO` & `kan_gpt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
```

### Comparing `kan_gpt-0.1.2/README.md` & `kan_gpt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/cli.py` & `kan_gpt-0.1.3/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/efficient_kan/model.py` & `kan_gpt-0.1.3/kan_gpt/efficient_kan/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/KAN.py` & `kan_gpt-0.1.3/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/KANLayer.py` & `kan_gpt-0.1.3/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/LBFGS.py` & `kan_gpt-0.1.3/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-0.1.3/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-0.1.3/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/spline.py` & `kan_gpt-0.1.3/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/kan/utils.py` & `kan_gpt-0.1.3/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/mingpt/bpe.py` & `kan_gpt-0.1.3/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/mingpt/model.py` & `kan_gpt-0.1.3/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/mingpt/trainer.py` & `kan_gpt-0.1.3/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/mingpt/utils.py` & `kan_gpt-0.1.3/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/model.py` & `kan_gpt-0.1.3/kan_gpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/kan_gpt/train.py` & `kan_gpt-0.1.3/kan_gpt/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,51 +40,53 @@
         "learning_rate": args.learning_rate,
         "max_iters": args.max_iters,
         "num_workers": args.num_workers,
         "architecture": args.architecture,
         "device": args.device,
     }
 
-    wandb.init(project="KAN-GPT", config=config)
-
     model_type = args.model_type
 
     # print an example instance of the dataset
     if args.dummy_dataset:
         train_dataset = WebTextDataset("test", "gpt2")
     else:
         train_dataset = WebTextDataset("train", "gpt2")
 
     test_dataset = WebTextDataset("test", "gpt2")
 
+    print("test_dataset: ", len(test_dataset))
+    print("train_dataset: ", len(train_dataset))
+
     if args.architecture == "KAN":
         GPT = KAN_GPT
     else:
         GPT = MLP_GPT
 
     # create a GPT instance
     model_config = GPT.get_default_config()
     model_config.model_type = model_type
     model_config.vocab_size = train_dataset.get_vocab_size()
     model_config.block_size = train_dataset.get_block_size()
     model = GPT(model_config)
 
-    wandb.watch(model)
-
     # create a Trainer object
     train_config = Trainer.get_default_config()
     train_config.learning_rate = float(
         args.learning_rate
     )  # the model we're using is so small that we can go a bit faster
     train_config.max_iters = int(args.max_iters)
     train_config.num_workers = int(args.num_workers)
     train_config.batch_size = int(args.batch_size)
     train_config.device = args.device
     trainer = Trainer(train_config, model, train_dataset)
 
+    wandb.init(project="KAN-GPT", config=config)
+    wandb.watch(model)
+
     def batch_end_callback(trainer):
         # TODO: Add W&B Hooks
         if trainer.iter_num % 100 == 0:
             print(
                 f"iter_dt {trainer.iter_dt * 1000:.2f}ms; "
                 f"iter {trainer.iter_num}: "
                 f"train loss {trainer.loss.item():.5f}"
```

### Comparing `kan_gpt-0.1.2/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-0.1.3/kan_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
```

### Comparing `kan_gpt-0.1.2/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-0.1.3/kan_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/setup.py` & `kan_gpt-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/tests/test_efficient_kan.py` & `kan_gpt-0.1.3/tests/test_efficient_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/tests/test_gpt_kan.py` & `kan_gpt-0.1.3/tests/test_gpt_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/tests/test_gpt_mlp.py` & `kan_gpt-0.1.3/tests/test_gpt_mlp.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.2/tests/test_kan.py` & `kan_gpt-0.1.3/tests/test_kan.py`

 * *Files identical despite different names*

