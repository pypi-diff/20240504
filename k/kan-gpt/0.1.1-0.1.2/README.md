# Comparing `tmp/kan_gpt-0.1.1.tar.gz` & `tmp/kan_gpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-0.1.1.tar", last modified: Sat May  4 04:51:15 2024, max compression
+gzip compressed data, was "kan_gpt-0.1.2.tar", last modified: Sat May  4 07:34:34 2024, max compression
```

## Comparing `kan_gpt-0.1.1.tar` & `kan_gpt-0.1.2.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.919294 kan_gpt-0.1.1/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.923294 kan_gpt-0.1.1/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.923294 kan_gpt-0.1.1/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.923294 kan_gpt-0.1.1/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19088 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_kan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.602879 kan_gpt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-04 07:34:34.602879 kan_gpt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.590879 kan_gpt-0.1.2/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.594879 kan_gpt-0.1.2/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.594879 kan_gpt-0.1.2/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 07:34:34.000000 kan_gpt-0.1.2/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:34:34.602879 kan_gpt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:34.598879 kan_gpt-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 07:34:26.000000 kan_gpt-0.1.2/tests/test_kan.py
```

### Comparing `kan_gpt-0.1.1/HISTORY.md` & `kan_gpt-0.1.2/HISTORY.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Feat(kan_gpt/efficient_kan/): integration with efficient kan reduced
+  training memory footprint. [Aditya NG]
+- Test(gpt-pico): reducing memory footprint. [Aditya NG]
+
+
+0.1.1 (2024-05-04)
+------------------
+- Release: version 0.1.1 🚀 [Aditya NG]
 - Test(kan_gpt,mlp_gpt,kan): test cases for forward-backward passes.
   [Aditya NG]
 - Ci(codecov): token. [Aditya NG]
 - Merge branch 'main' of https://github.com/AdityaNG/kan-gpt into main.
   [Aditya NG]
 - Update LICENSE. [Aditya]
 - Refactor(kan_gpt): linting. [Aditya NG]
```

### Comparing `kan_gpt-0.1.1/LICENSE` & `kan_gpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/PKG-INFO` & `kan_gpt-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -61,25 +61,25 @@
 
 prompt = "Bangalore is often described as the "
 
 prompt_encoded = tokenizer.encode(
   text=prompt, add_special_tokens=False
 )
 
-result = prompt
 x = torch.tensor(prompt_encoded).unsqueeze(0)
 
-for _ in range(50):  # sample 50 tokens
-  logits, loss = model(x)
-  x = torch.cat(
-    (x[:, 1:-2], logits[:, -2:-1]), dim=0
-  )
-  result += tokenizer.decode(logits[0, -2:-1])
+model.eval()
+y = model.generate(x, 50)  # sample 50 tokens
+
+result = tokenizer.decode(logits[0, -2:-1])
 
 print(result)
+
+# Bangalore is often described as the Silicon Valley of India.
+# The city has witnessed rapid growth in the past two decades.....
 ```
 
 ## Setup for Development
 
 ```bash
 # Download Repo
 git clone https://github.com/AdityaNG/kan-gpt
@@ -110,25 +110,27 @@
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [ ] Mini training POC for KAN-GPT
   - [x] Integrate KAN training logic from `KAN.train_kan`
-  - [ ] Train a dummy batch
+  - [x] Train a dummy batch w/o any memory issues
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
 - [ ] Auto Save checkpoints
 - [ ] Auto Save checkpoints to W&B
 - [ ] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
-- [ ] Test Cases
+- [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
+- [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
+  - [x] EFFICIENT_KAN: Forward-Backward test
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
```

### Comparing `kan_gpt-0.1.1/README.md` & `kan_gpt-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 
 prompt = "Bangalore is often described as the "
 
 prompt_encoded = tokenizer.encode(
   text=prompt, add_special_tokens=False
 )
 
-result = prompt
 x = torch.tensor(prompt_encoded).unsqueeze(0)
 
-for _ in range(50):  # sample 50 tokens
-  logits, loss = model(x)
-  x = torch.cat(
-    (x[:, 1:-2], logits[:, -2:-1]), dim=0
-  )
-  result += tokenizer.decode(logits[0, -2:-1])
+model.eval()
+y = model.generate(x, 50)  # sample 50 tokens
+
+result = tokenizer.decode(logits[0, -2:-1])
 
 print(result)
+
+# Bangalore is often described as the Silicon Valley of India.
+# The city has witnessed rapid growth in the past two decades.....
 ```
 
 ## Setup for Development
 
 ```bash
 # Download Repo
 git clone https://github.com/AdityaNG/kan-gpt
@@ -78,25 +78,27 @@
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [ ] Mini training POC for KAN-GPT
   - [x] Integrate KAN training logic from `KAN.train_kan`
-  - [ ] Train a dummy batch
+  - [x] Train a dummy batch w/o any memory issues
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
 - [ ] Auto Save checkpoints
 - [ ] Auto Save checkpoints to W&B
 - [ ] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
-- [ ] Test Cases
+- [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
+- [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
+  - [x] EFFICIENT_KAN: Forward-Backward test
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
```

### Comparing `kan_gpt-0.1.1/kan_gpt/cli.py` & `kan_gpt-0.1.2/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/dataset.py` & `kan_gpt-0.1.2/kan_gpt/dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/KAN.py` & `kan_gpt-0.1.2/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/KANLayer.py` & `kan_gpt-0.1.2/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/LBFGS.py` & `kan_gpt-0.1.2/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-0.1.2/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-0.1.2/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/spline.py` & `kan_gpt-0.1.2/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/kan/utils.py` & `kan_gpt-0.1.2/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/mingpt/bpe.py` & `kan_gpt-0.1.2/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/mingpt/model.py` & `kan_gpt-0.1.2/kan_gpt/mingpt/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
                     # Gophers
                     "gopher-44m": dict(n_layer=8, n_head=16, n_embd=512),
                     # (there are a number more...)
                     # I made these tiny models up
                     "gpt-mini": dict(n_layer=6, n_head=6, n_embd=192),
                     "gpt-micro": dict(n_layer=4, n_head=4, n_embd=128),
                     "gpt-nano": dict(n_layer=3, n_head=3, n_embd=48),
+                    "gpt-pico": dict(n_layer=1, n_head=1, n_embd=1),
                 }[config.model_type]
             )
 
         self.transformer = nn.ModuleDict(
             dict(
                 wte=nn.Embedding(config.vocab_size, config.n_embd),
                 wpe=nn.Embedding(config.block_size, config.n_embd),
```

### Comparing `kan_gpt-0.1.1/kan_gpt/mingpt/trainer.py` & `kan_gpt-0.1.2/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/mingpt/utils.py` & `kan_gpt-0.1.2/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/kan_gpt/model.py` & `kan_gpt-0.1.2/kan_gpt/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,23 @@
 
 import math
 
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
 
-from kan_gpt.kan.KAN import KAN
+from kan_gpt.efficient_kan.model import KAN as EFFICIENT_KAN
+from kan_gpt.kan.KAN import KAN as ORIGINAL_KAN
 from kan_gpt.mingpt.utils import CfgNode as CN
+from kan_gpt.settings import settings
+
+if settings.kan.KAN_IMPLEMENTATION == "EFFICIENT_KAN":
+    KAN = EFFICIENT_KAN  # type: ignore
+elif settings.kan.KAN_IMPLEMENTATION == "ORIGINAL_KAN":
+    KAN = ORIGINAL_KAN  # type: ignore
 
 # -----------------------------------------------------------------------------
 
 
 class NewGELU(nn.Module):
     """
     Implementation of the GELU activation function currently in Google BERT
@@ -194,14 +201,15 @@
                     # Gophers
                     "gopher-44m": dict(n_layer=8, n_head=16, n_embd=512),
                     # (there are a number more...)
                     # I made these tiny models up
                     "gpt-mini": dict(n_layer=6, n_head=6, n_embd=192),
                     "gpt-micro": dict(n_layer=4, n_head=4, n_embd=128),
                     "gpt-nano": dict(n_layer=3, n_head=3, n_embd=48),
+                    "gpt-pico": dict(n_layer=1, n_head=1, n_embd=1),
                 }[config.model_type]
             )
 
         self.transformer = nn.ModuleDict(
             dict(
                 wte=nn.Embedding(config.vocab_size, config.n_embd),
                 wpe=nn.Embedding(config.block_size, config.n_embd),
@@ -454,24 +462,25 @@
         if targets is not None:
             loss = F.cross_entropy(
                 logits.view(-1, logits.size(-1)),
                 targets.view(-1),
                 ignore_index=-1,
             )
 
-            reg = self.kan_loss(
-                x=idx,
-                lamb_l1=lamb_l1,
-                lamb_entropy=lamb_entropy,
-                lamb_coef=lamb_coef,
-                lamb_coefdiff=lamb_coefdiff,
-                small_mag_threshold=small_mag_threshold,
-                small_reg_factor=small_reg_factor,
-            )
-            loss = loss + lamb * reg
+            if settings.kan.KAN_IMPLEMENTATION == "ORIGINAL_KAN":
+                reg = self.kan_loss(
+                    x=idx,
+                    lamb_l1=lamb_l1,
+                    lamb_entropy=lamb_entropy,
+                    lamb_coef=lamb_coef,
+                    lamb_coefdiff=lamb_coefdiff,
+                    small_mag_threshold=small_mag_threshold,
+                    small_reg_factor=small_reg_factor,
+                )
+                loss = loss + lamb * reg
 
         return logits, loss
 
     @torch.no_grad()
     def generate(
         self, idx, max_new_tokens, temperature=1.0, do_sample=False, top_k=None
     ):
```

### Comparing `kan_gpt-0.1.1/kan_gpt/train.py` & `kan_gpt-0.1.2/kan_gpt/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     trainer.run()
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser("KAN-GPT Trainer")
-    parser.add_argument("--model_type", default="gpt-nano")
+    parser.add_argument("--model_type", default="gpt-mini")
     parser.add_argument("--dummy_dataset", action="store_true")
     parser.add_argument("--learning_rate", default=5e-3)
     parser.add_argument("--max_iters", default=2000)
     parser.add_argument("--num_workers", default=0)
     parser.add_argument("--batch_size", default=64)
 
     parser.add_argument(
```

### Comparing `kan_gpt-0.1.1/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-0.1.2/kan_gpt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -61,25 +61,25 @@
 
 prompt = "Bangalore is often described as the "
 
 prompt_encoded = tokenizer.encode(
   text=prompt, add_special_tokens=False
 )
 
-result = prompt
 x = torch.tensor(prompt_encoded).unsqueeze(0)
 
-for _ in range(50):  # sample 50 tokens
-  logits, loss = model(x)
-  x = torch.cat(
-    (x[:, 1:-2], logits[:, -2:-1]), dim=0
-  )
-  result += tokenizer.decode(logits[0, -2:-1])
+model.eval()
+y = model.generate(x, 50)  # sample 50 tokens
+
+result = tokenizer.decode(logits[0, -2:-1])
 
 print(result)
+
+# Bangalore is often described as the Silicon Valley of India.
+# The city has witnessed rapid growth in the past two decades.....
 ```
 
 ## Setup for Development
 
 ```bash
 # Download Repo
 git clone https://github.com/AdityaNG/kan-gpt
@@ -110,25 +110,27 @@
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [ ] Mini training POC for KAN-GPT
   - [x] Integrate KAN training logic from `KAN.train_kan`
-  - [ ] Train a dummy batch
+  - [x] Train a dummy batch w/o any memory issues
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
 - [ ] Auto Save checkpoints
 - [ ] Auto Save checkpoints to W&B
 - [ ] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
-- [ ] Test Cases
+- [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
+- [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
+  - [x] EFFICIENT_KAN: Forward-Backward test
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
```

### Comparing `kan_gpt-0.1.1/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-0.1.2/kan_gpt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 kan_gpt/VERSION
 kan_gpt/__init__.py
 kan_gpt/__main__.py
 kan_gpt/base.py
 kan_gpt/cli.py
 kan_gpt/dataset.py
 kan_gpt/model.py
+kan_gpt/settings.py
 kan_gpt/train.py
 kan_gpt.egg-info/PKG-INFO
 kan_gpt.egg-info/SOURCES.txt
 kan_gpt.egg-info/dependency_links.txt
 kan_gpt.egg-info/entry_points.txt
 kan_gpt.egg-info/requires.txt
 kan_gpt.egg-info/top_level.txt
+kan_gpt/efficient_kan/model.py
 kan_gpt/kan/KAN.py
 kan_gpt/kan/KANLayer.py
 kan_gpt/kan/LBFGS.py
 kan_gpt/kan/Symbolic_KANLayer.py
 kan_gpt/kan/__init__.py
 kan_gpt/kan/spline.py
 kan_gpt/kan/utils.py
@@ -44,10 +46,11 @@
 kan_gpt/mingpt/bpe.py
 kan_gpt/mingpt/model.py
 kan_gpt/mingpt/trainer.py
 kan_gpt/mingpt/utils.py
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
+tests/test_efficient_kan.py
 tests/test_gpt_kan.py
 tests/test_gpt_mlp.py
 tests/test_kan.py
```

### Comparing `kan_gpt-0.1.1/setup.py` & `kan_gpt-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.1/tests/test_gpt_kan.py` & `kan_gpt-0.1.2/tests/test_gpt_mlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import torch
-from kan_gpt.model import GPT as KAN_GPT
+from kan_gpt.mingpt.model import GPT as MLP_GPT
 
 VOCAB_SIZE = 8
 BLOCK_SIZE = 16
-MODEL_TYPE = "gpt-nano"
+MODEL_TYPE = "gpt-pico"
 
 
-def get_gpt_model() -> KAN_GPT:
-    model_config = KAN_GPT.get_default_config()
+def get_gpt_model() -> MLP_GPT:
+    model_config = MLP_GPT.get_default_config()
     model_config.model_type = MODEL_TYPE
     model_config.vocab_size = VOCAB_SIZE
     model_config.block_size = BLOCK_SIZE
-    model = KAN_GPT(model_config)
+    model = MLP_GPT(model_config)
     return model
 
 
 def test_forward():
     with torch.no_grad():
         model = get_gpt_model()
         x = torch.zeros((1, BLOCK_SIZE), dtype=torch.long)
```

### Comparing `kan_gpt-0.1.1/tests/test_kan.py` & `kan_gpt-0.1.2/tests/test_kan.py`

 * *Files identical despite different names*

