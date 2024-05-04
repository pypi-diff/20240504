# Comparing `tmp/kan_gpt-0.1.0.tar.gz` & `tmp/kan_gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-0.1.0.tar", last modified: Fri May  3 03:33:30 2024, max compression
+gzip compressed data, was "kan_gpt-0.1.1.tar", last modified: Sat May  4 04:51:15 2024, max compression
```

## Comparing `kan_gpt-0.1.0.tar` & `kan_gpt-0.1.1.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.967784 kan_gpt-0.1.0/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.967784 kan_gpt-0.1.0/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57097 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-03 03:33:30.000000 kan_gpt-0.1.0/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-03 03:33:30.000000 kan_gpt-0.1.0/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:33:30.000000 kan_gpt-0.1.0/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 03:33:30.000000 kan_gpt-0.1.0/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 03:33:30.000000 kan_gpt-0.1.0/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 03:33:30.000000 kan_gpt-0.1.0/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:30.971784 kan_gpt-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 03:33:18.000000 kan_gpt-0.1.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.919294 kan_gpt-0.1.1/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.923294 kan_gpt-0.1.1/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.923294 kan_gpt-0.1.1/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.923294 kan_gpt-0.1.1/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19088 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 04:51:15.000000 kan_gpt-0.1.1/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:15.927294 kan_gpt-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 04:51:07.000000 kan_gpt-0.1.1/tests/test_kan.py
```

### Comparing `kan_gpt-0.1.0/PKG-INFO` & `kan_gpt-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -31,15 +31,15 @@
 Requires-Dist: types-requests; extra == "test"
 
 # KAN-GPT
 
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
 
-Awesome KAN-GPT created by AdityaNG
+The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
@@ -50,67 +50,85 @@
 
 model_config = GPT.get_default_config()
 model_config.model_type = "gpt2"
 model_config.vocab_size = 5
 model_config.block_size = 10
 model = GPT(model_config)
 
+tokenizer = GPT2Tokenizer.from_pretrained('gpt2')
+
 x = torch.zeros((1, 10), dtype=torch.long)
 y = torch.zeros((1, 10), dtype=torch.long)
 
-# x = x.cuda()
-# y = y.cuda()
-# model = model.cuda()
-
-logits, loss = model(x, y)
+prompt = "Bangalore is often described as the "
 
-print(logits.shape)
-```
+prompt_encoded = tokenizer.encode(
+  text=prompt, add_special_tokens=False
+)
+
+result = prompt
+x = torch.tensor(prompt_encoded).unsqueeze(0)
+
+for _ in range(50):  # sample 50 tokens
+  logits, loss = model(x)
+  x = torch.cat(
+    (x[:, 1:-2], logits[:, -2:-1]), dim=0
+  )
+  result += tokenizer.decode(logits[0, -2:-1])
 
-```bash
-$ python -m kan_gpt.train
+print(result)
 ```
 
-## Setup
+## Setup for Development
 
 ```bash
 # Download Repo
-%cd /content
-!git clone https://github.com/AdityaNG/kan-gpt
-%cd kan-gpt
-!git pull
+git clone https://github.com/AdityaNG/kan-gpt
+cd kan-gpt
+git pull
 
 # Download Dataset
-!./scripts/download_webtext.sh
+./scripts/download_webtext.sh
 
 # Install dependencies for development
-!pip install -r requirements.txt
-!pip install -e .
+pip install -r requirements.txt
+pip install -e .
 ```
 
 ## Train
 
-Dummy script to make sure everything is working as expected
+Use the following dummy script to make sure everything is working as expected
+```bash
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu
+```
+
+Then make use of the training script
 ```bash
-CUDA_VISIBLE_DEVICE="0" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset
+python -m kan_gpt.train
 ```
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [ ] Mini training POC for KAN-GPT
-  - [ ] Integrate KAN training logic from `KAN.train_kan`
+  - [x] Integrate KAN training logic from `KAN.train_kan`
+  - [ ] Train a dummy batch
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
 - [ ] Auto Save checkpoints
 - [ ] Auto Save checkpoints to W&B
 - [ ] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
+- [ ] Test Cases
+  - [x] KAN: Forward-Backward test
+  - [x] GPT: Forward-Backward test
+  - [x] KAN_GPT: Forward-Backward test
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
```

### Comparing `kan_gpt-0.1.0/README.md` & `kan_gpt-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # KAN-GPT
 
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
 
-Awesome KAN-GPT created by AdityaNG
+The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
@@ -18,67 +18,85 @@
 
 model_config = GPT.get_default_config()
 model_config.model_type = "gpt2"
 model_config.vocab_size = 5
 model_config.block_size = 10
 model = GPT(model_config)
 
+tokenizer = GPT2Tokenizer.from_pretrained('gpt2')
+
 x = torch.zeros((1, 10), dtype=torch.long)
 y = torch.zeros((1, 10), dtype=torch.long)
 
-# x = x.cuda()
-# y = y.cuda()
-# model = model.cuda()
-
-logits, loss = model(x, y)
+prompt = "Bangalore is often described as the "
 
-print(logits.shape)
-```
+prompt_encoded = tokenizer.encode(
+  text=prompt, add_special_tokens=False
+)
+
+result = prompt
+x = torch.tensor(prompt_encoded).unsqueeze(0)
+
+for _ in range(50):  # sample 50 tokens
+  logits, loss = model(x)
+  x = torch.cat(
+    (x[:, 1:-2], logits[:, -2:-1]), dim=0
+  )
+  result += tokenizer.decode(logits[0, -2:-1])
 
-```bash
-$ python -m kan_gpt.train
+print(result)
 ```
 
-## Setup
+## Setup for Development
 
 ```bash
 # Download Repo
-%cd /content
-!git clone https://github.com/AdityaNG/kan-gpt
-%cd kan-gpt
-!git pull
+git clone https://github.com/AdityaNG/kan-gpt
+cd kan-gpt
+git pull
 
 # Download Dataset
-!./scripts/download_webtext.sh
+./scripts/download_webtext.sh
 
 # Install dependencies for development
-!pip install -r requirements.txt
-!pip install -e .
+pip install -r requirements.txt
+pip install -e .
 ```
 
 ## Train
 
-Dummy script to make sure everything is working as expected
+Use the following dummy script to make sure everything is working as expected
+```bash
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu
+```
+
+Then make use of the training script
 ```bash
-CUDA_VISIBLE_DEVICE="0" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset
+python -m kan_gpt.train
 ```
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [ ] Mini training POC for KAN-GPT
-  - [ ] Integrate KAN training logic from `KAN.train_kan`
+  - [x] Integrate KAN training logic from `KAN.train_kan`
+  - [ ] Train a dummy batch
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
 - [ ] Auto Save checkpoints
 - [ ] Auto Save checkpoints to W&B
 - [ ] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
+- [ ] Test Cases
+  - [x] KAN: Forward-Backward test
+  - [x] GPT: Forward-Backward test
+  - [x] KAN_GPT: Forward-Backward test
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
```

### Comparing `kan_gpt-0.1.0/kan_gpt/cli.py` & `kan_gpt-0.1.1/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/dataset.py` & `kan_gpt-0.1.1/kan_gpt/dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/KAN.py` & `kan_gpt-0.1.1/kan_gpt/kan/KAN.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 import copy
 import glob
 import os
 import random
 
 import matplotlib.pyplot as plt
 import numpy as np
+import sympy
 import torch
 import torch.nn as nn
 from tqdm import tqdm
 
-from .KANLayer import *
-from .LBFGS import *
-from .Symbolic_KANLayer import *
+from .KANLayer import KANLayer
+from .LBFGS import LBFGS
+from .spline import curve2coef
+from .Symbolic_KANLayer import SYMBOLIC_LIB, Symbolic_KANLayer
 
 
 class KAN(nn.Module):
     """
     KAN class
 
     Attributes:
     -----------
         biases: a list of nn.Linear()
-            biases are added on nodes (in principle, biases can be absorbed into activation functions. However, we still have them for better optimization)
+            biases are added on nodes (in principle, biases can be absorbed
+            into activation functions. However, we still have them for better optimization)
         act_fun: a list of KANLayer
             KANLayers
         depth: int
             depth of KAN
         width: list
-            number of neurons in each layer. e.g., [2,5,5,3] means 2D inputs, 5D outputs, with 2 layers of 5 hidden neurons.
+            number of neurons in each layer. e.g., [2,5,5,3] means 2D inputs,
+            5D outputs, with 2 layers of 5 hidden neurons.
         grid: int
             the number of grid intervals
         k: int
             the order of piecewise polynomial
         base_fun: fun
-            residual function b(x). an activation function phi(x) = sb_scale * b(x) + sp_scale * spline(x)
+            residual function b(x). an activation function
+            phi(x) = sb_scale * b(x) + sp_scale * spline(x)
         symbolic_fun: a list of Symbolic_KANLayer
             Symbolic_KANLayers
         symbolic_enabled: bool
-            If False, the symbolic front is not computed (to save time). Default: True.
+            If False, the symbolic front is not computed (to save time).
+            Default: True.
 
     Methods:
     --------
         __init__():
             initialize a KAN
         initialize_from_another_model():
-            initialize a KAN from another KAN (with the same shape, but potentially different grids)
+            initialize a KAN from another KAN (with the same shape, but
+            potentially different grids)
         update_grid_from_samples():
             update spline grids based on samples
         initialize_grid_from_another_model():
             initalize KAN grids from another KAN
         forward():
             forward
         set_mode():
-            set the mode of an activation function: 'n' for numeric, 's' for symbolic, 'ns' for combined (note they are visualized differently in plot(). 'n' as black, 's' as red, 'ns' as purple).
+            set the mode of an activation function: 'n' for numeric, 's' for
+            symbolic, 'ns' for combined (note they are visualized differently
+            in plot(). 'n' as black, 's' as red, 'ns' as purple).
         fix_symbolic():
             fix an activation function to be symbolic
         suggest_symbolic():
-            suggest the symbolic candicates of a numeric spline-based activation function
+            suggest the symbolic candicates of a numeric spline-based
+            activation function
         lock():
             lock activation functions to share parameters
         unlock():
             unlock locked activations
         get_range():
             get the input and output ranges of an activation function
         plot():
@@ -97,29 +107,34 @@
     ):
         """
         initalize a KAN model
 
         Args:
         -----
             width : list of int
-                :math:`[n_0, n_1, .., n_{L-1}]` specify the number of neurons in each layer (including inputs/outputs)
+                :math:`[n_0, n_1, .., n_{L-1}]` specify the number of neurons
+                in each layer (including inputs/outputs)
             grid : int
                 number of grid intervals. Default: 3.
             k : int
                 order of piecewise polynomial. Default: 3.
             noise_scale : float
                 initial injected noise to spline. Default: 0.1.
             base_fun : fun
                 the residual function b(x). Default: torch.nn.SiLU().
             symbolic_enabled : bool
-                compute or skip symbolic computations (for efficiency). By default: True.
+                compute or skip symbolic computations (for efficiency).
+                By default: True.
             bias_trainable : bool
                 bias parameters are updated or not. By default: True
             grid_eps : float
-                When grid_eps = 0, the grid is uniform; when grid_eps = 1, the grid is partitioned using percentiles of samples. 0 < grid_eps < 1 interpolates between the two extremes. Default: 0.02.
+                When grid_eps = 0, the grid is uniform; when grid_eps = 1,
+                the grid is partitioned using percentiles of samples.
+                0 < grid_eps < 1 interpolates between the two extremes.
+                Default: 0.02.
             grid_range : list/np.array of shape (2,))
                 setting the range of grids. Default: [-1,1].
             sp_trainable : bool
                 If true, scale_sp is trainable. Default: True.
             sb_trainable : bool
                 If true, scale_base is trainable. Default: True.
             seed : int
@@ -128,15 +143,16 @@
         Returns:
         --------
             self
 
         Example
         -------
         >>> model = KAN(width=[2,5,1], grid=5, k=3)
-        >>> (model.act_fun[0].in_dim, model.act_fun[0].out_dim), (model.act_fun[1].in_dim, model.act_fun[1].out_dim)
+        >>> (model.act_fun[0].in_dim, model.act_fun[0].out_dim), \
+            (model.act_fun[1].in_dim, model.act_fun[1].out_dim)
         ((2, 5), (5, 1))
         """
         super(KAN, self).__init__()
 
         torch.manual_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
@@ -198,15 +214,16 @@
             self.symbolic_fun.append(sb_batch)
 
         self.symbolic_fun = nn.ModuleList(self.symbolic_fun)
         self.symbolic_enabled = symbolic_enabled
 
     def initialize_from_another_model(self, another_model, x):
         """
-        initialize from a parent model. The parent has the same width as the current model but may have different grids.
+        initialize from a parent model. The parent has the same width as the
+        current model but may have different grids.
 
         Args:
         -----
             another_model : KAN
                 the parent model used to initialize the current model
             x : 2D torch.float
                 inputs, shape (batch, input dimension)
@@ -298,15 +315,16 @@
         Returns:
         --------
             None
 
         Example
         -------
         >>> model_parent = KAN(width=[1,1], grid=5, k=3)
-        >>> model_parent.act_fun[0].grid.data = torch.linspace(-2,2,steps=6)[None,:]
+        >>> model_parent.act_fun[0].grid.data = torch.linspace(-2,2,steps=6)\
+            [None,:]
         >>> x = torch.linspace(-2,2,steps=1001)[:,None]
         >>> model = KAN(width=[1,1], grid=5, k=3)
         >>> print(model.act_fun[0].grid.data)
         >>> model = model.initialize_from_another_model(model_parent, x)
         >>> print(model.act_fun[0].grid.data)
         tensor([[-1.0000, -0.6000, -0.2000,  0.2000,  0.6000,  1.0000]])
         tensor([[-2.0000, -1.2000, -0.4000,  0.4000,  1.2000,  2.0000]])
@@ -355,15 +373,15 @@
 
         for l in range(self.depth):
 
             x_numerical, preacts, postacts_numerical, postspline = (
                 self.act_fun[l](x)
             )
 
-            if self.symbolic_enabled == True:
+            if self.symbolic_enabled:
                 x_symbolic, postacts_symbolic = self.symbolic_fun[l](x)
             else:
                 x_symbolic = 0.0
                 postacts_symbolic = 0.0
 
             x = x_numerical + x_symbolic
             postacts = postacts_numerical + postacts_symbolic
@@ -413,15 +431,15 @@
         if mode == "s":
             mask_n = 0.0
             mask_s = 1.0
         elif mode == "n":
             mask_n = 1.0
             mask_s = 0.0
         elif mode == "sn" or mode == "ns":
-            if mask_n == None:
+            if mask_n is None:
                 mask_n = 1.0
             else:
                 mask_n = mask_n
             mask_s = 1.0
         else:
             mask_n = 0.0
             mask_s = 0.0
@@ -451,15 +469,16 @@
             i : int
                 input neuron index
             j : int
                 output neuron index
             fun_name : str
                 function name
             fit_params_bool : bool
-                obtaining affine parameters through fitting (True) or setting default values (False)
+                obtaining affine parameters through fitting (True) or setting
+                default values (False)
             a_range : tuple
                 sweeping range of a
             b_range : tuple
                 sweeping range of b
             verbose : bool
                 If True, more information is printed.
             random : bool
@@ -482,20 +501,22 @@
                 [0., 0., 1., 0., 0.]])
 
         Example 2
         ---------
         >>> # when fit_params_bool = True
         >>> model = KAN(width=[2,5,1], grid=5, k=3, noise_scale=1.)
         >>> x = torch.normal(0,1,size=(100,2))
-        >>> model(x) # obtain activations (otherwise model does not have attributes acts)
+        >>> model(x) # obtain activations (otherwise model does not have \
+        attributes acts)
         >>> model.fix_symbolic(0,1,3,'sin',fit_params_bool=True)
         >>> print(model.act_fun[0].mask.reshape(2,5))
         >>> print(model.symbolic_fun[0].mask.reshape(2,5))
         r2 is 0.8131332993507385
-        r2 is not very high, please double check if you are choosing the correct symbolic function.
+        r2 is not very high, please double check if you are choosing the \
+            correct symbolic function.
         tensor([[1., 1., 1., 1., 1.],
                 [1., 1., 0., 1., 1.]])
         tensor([[0., 0., 0., 0., 0.],
                 [0., 0., 1., 0., 0.]])
         """
         self.set_mode(l, i, j, mode="s")
         if not fit_params_bool:
@@ -538,15 +559,16 @@
         lock ids in the l-th layer to be the same function
 
         Args:
         -----
             l : int
                 layer index
             ids : 2D list
-                :math:`[[i_1,j_1],[i_2,j_2],...]` set :math:`(l,i_i,j_1), (l,i_2,j_2), ...` to be the same function
+                :math:`[[i_1,j_1],[i_2,j_2],...]` set :math:`(l,i_i,j_1), \
+                    (l,i_2,j_2), ...` to be the same function
 
         Returns:
         --------
             None
 
         Example
         -------
@@ -568,15 +590,16 @@
         unlock ids in the l-th layer to be the same function
 
         Args:
         -----
             l : int
                 layer index
             ids : 2D list)
-                [[i1,j1],[i2,j2],...] set (l,ii,j1), (l,i2,j2), ... to be unlocked
+                [[i1,j1],[i2,j2],...] set (l,ii,j1), (l,i2,j2), ... to be
+                unlocked
 
         Example:
         --------
         >>> model = KAN(width=[2,3,1], grid=5, k=3, noise_scale=1.)
         >>> model.lock(0,[[1,0],[1,1]])
         >>> print(model.act_fun[0].weight_sharing.reshape(3,2))
         >>> model.unlock(0,[[1,0],[1,1]])
@@ -652,19 +675,24 @@
         plot KAN
 
         Args:
         -----
             folder : str
                 the folder to store pngs
             beta : float
-                positive number. control the transparency of each activation. transparency = tanh(beta*l1).
+                positive number. control the transparency of each activation.
+                transparency = tanh(beta*l1).
             mask : bool
-                If True, plot with mask (need to run prune() first to obtain mask). If False (by default), plot all activation functions.
+                If True, plot with mask (need to run prune() first to obtain
+                mask). If False (by default), plot all activation functions.
             mode : bool
-                "supervised" or "unsupervised". If "supervised", l1 is measured by absolution value (not subtracting mean); if "unsupervised", l1 is measured by standard deviation (subtracting mean).
+                "supervised" or "unsupervised". If "supervised", l1 is
+                measured by absolution value (not subtracting mean);
+                if "unsupervised", l1 is measured by standard deviation
+                (subtracting mean).
             scale : float
                 control the size of the diagram
             in_vars: None or list of str
                 the name(s) of input variables
             out_vars: None or list of str
                 the name(s) of output variables
             title: None or str
@@ -689,15 +717,15 @@
         for l in range(depth):
             w_large = 2.0
             for i in range(self.width[l]):
                 for j in range(self.width[l + 1]):
                     rank = torch.argsort(self.acts[l][:, i])
                     fig, ax = plt.subplots(figsize=(w_large, w_large))
 
-                    num = rank.shape[0]
+                    num = rank.shape[0]  # noqa
 
                     symbol_mask = self.symbolic_fun[l].mask[j][i]
                     numerical_mask = self.act_fun[l].mask.reshape(
                         self.width[l + 1], self.width[l]
                     )[j][i]
                     if symbol_mask > 0.0 and numerical_mask > 0.0:
                         color = "purple"
@@ -708,15 +736,15 @@
                     if symbol_mask == 0.0 and numerical_mask > 0.0:
                         color = "black"
                         alpha_mask = 1
                     if symbol_mask == 0.0 and numerical_mask == 0.0:
                         color = "white"
                         alpha_mask = 0
 
-                    if tick == True:
+                    if tick:
                         ax.tick_params(
                             axis="y", direction="in", pad=-22, labelsize=50
                         )
                         ax.tick_params(
                             axis="x", direction="in", pad=-15, labelsize=50
                         )
                         x_min, x_max, y_min, y_max = self.get_range(
@@ -743,15 +771,15 @@
                         self.spline_postacts[l][:, j, i][rank]
                         .cpu()
                         .detach()
                         .numpy(),
                         color=color,
                         lw=5,
                     )
-                    if sample == True:
+                    if sample:
                         plt.scatter(
                             self.acts[l][:, i][rank].cpu().detach().numpy(),
                             self.spline_postacts[l][:, j, i][rank]
                             .cpu()
                             .detach()
                             .numpy(),
                             color=color,
@@ -798,27 +826,27 @@
         A = 1
         y0 = 0.4  # 0.4
 
         # plt.figure(figsize=(5,5*(neuron_depth-1)*y0))
         neuron_depth = len(width)
         min_spacing = A / np.maximum(np.max(width), 5)
 
-        max_neuron = np.max(width)
+        max_neuron = np.max(width)  # noqa
         max_num_weights = np.max(width[:-1] * width[1:])
         y1 = 0.4 / np.maximum(max_num_weights, 3)
 
         fig, ax = plt.subplots(
             figsize=(10 * scale, 10 * scale * (neuron_depth - 1) * y0)
         )
         # fig, ax = plt.subplots(figsize=(5,5*(neuron_depth-1)*y0))
 
         # plot scatters and lines
         for l in range(neuron_depth):
             n = width[l]
-            spacing = A / n
+            spacing = A / n  # noqa
             for i in range(n):
                 plt.scatter(
                     1 / (2 * n) + i / n,
                     l * y0,
                     s=min_spacing**2 * 10000 * scale**2,
                     color="black",
                 )
@@ -842,15 +870,15 @@
                             alpha_mask = 1.0
                         if symbol_mask == 0.0 and numerical_mask == 1.0:
                             color = "black"
                             alpha_mask = 1.0
                         if symbol_mask == 0.0 and numerical_mask == 0.0:
                             color = "white"
                             alpha_mask = 0.0
-                        if mask == True:
+                        if mask:
                             plt.plot(
                                 [1 / (2 * n) + i / n, 1 / (2 * N) + id_ / N],
                                 [l * y0, (l + 1 / 2) * y0 - y1],
                                 color=color,
                                 lw=2 * scale,
                                 alpha=alpha[l][j][i]
                                 * self.mask[l][i].item()
@@ -890,15 +918,15 @@
             plt.xlim(0, 1)
             plt.ylim(-0.1 * y0, (neuron_depth - 1 + 0.1) * y0)
 
         # -- Transformation functions
         DC_to_FC = ax.transData.transform
         FC_to_NFC = fig.transFigure.inverted().transform
         # -- Take data coordinates and transform them to normalized figure coordinates
-        DC_to_NFC = lambda x: FC_to_NFC(DC_to_FC(x))
+        DC_to_NFC = lambda x: FC_to_NFC(DC_to_FC(x))  # noqa
 
         plt.axis("off")
 
         # plot splines
         for l in range(neuron_depth - 1):
             n = width[l]
             for i in range(n):
@@ -911,51 +939,51 @@
                     right = DC_to_NFC([1 / (2 * N) + id_ / N + y1, 0])[0]
                     bottom = DC_to_NFC([0, (l + 1 / 2) * y0 - y1])[1]
                     up = DC_to_NFC([0, (l + 1 / 2) * y0 + y1])[1]
                     newax = fig.add_axes(
                         [left, bottom, right - left, up - bottom]
                     )
                     # newax = fig.add_axes([1/(2*N)+id_/N-y1, (l+1/2)*y0-y1, y1, y1], anchor='NE')
-                    if mask == False:
+                    if not mask:
                         newax.imshow(im, alpha=alpha[l][j][i])
                     else:
                         # make sure to run model.prune() first to compute mask ###
                         newax.imshow(
                             im,
                             alpha=alpha[l][j][i]
                             * self.mask[l][i].item()
                             * self.mask[l + 1][j].item(),
                         )
                     newax.axis("off")
 
-        if in_vars != None:
+        if in_vars is not None:
             n = self.width[0]
             for i in range(n):
                 plt.gcf().get_axes()[0].text(
                     1 / (2 * (n)) + i / (n),
                     -0.1,
                     in_vars[i],
                     fontsize=40 * scale,
                     horizontalalignment="center",
                     verticalalignment="center",
                 )
 
-        if out_vars != None:
+        if out_vars is not None:
             n = self.width[-1]
             for i in range(n):
                 plt.gcf().get_axes()[0].text(
                     1 / (2 * (n)) + i / (n),
                     y0 * (len(self.width) - 1) + 0.1,
                     out_vars[i],
                     fontsize=40 * scale,
                     horizontalalignment="center",
                     verticalalignment="center",
                 )
 
-        if title != None:
+        if title is not None:
             plt.gcf().get_axes()[0].text(
                 0.5,
                 y0 * (len(self.width) - 1) + 0.2,
                 title,
                 fontsize=40 * scale,
                 horizontalalignment="center",
                 verticalalignment="center",
@@ -992,15 +1020,16 @@
     ):
         """
         training
 
         Args:
         -----
             dataset : dic
-                contains dataset['train_input'], dataset['train_label'], dataset['test_input'], dataset['test_label']
+                contains dataset['train_input'], dataset['train_label'],
+                dataset['test_input'], dataset['test_label']
             opt : str
                 "LBFGS" or "Adam"
             steps : int
                 training steps
             log : int
                 logging frequency
             lamb : float
@@ -1018,17 +1047,19 @@
             grid_update_num : int
                 the number of grid updates before stop_grid_update_step
             stop_grid_update_step : int
                 no grid updates after this training step
             batch : int
                 batch size, if -1 then full.
             small_mag_threshold : float
-                threshold to determine large or small numbers (may want to apply larger penalty to smaller numbers)
+                threshold to determine large or small numbers (may want to
+                apply larger penalty to smaller numbers)
             small_reg_factor : float
-                penalty strength applied to small factors relative to large factos
+                penalty strength applied to small factors relative to large
+                factos
             device : str
                 device
             save_fig_freq : int
                 save figure every (save_fig_freq) step
 
         Returns:
         --------
@@ -1080,15 +1111,15 @@
                 )
                 reg_ += lamb_coef * coeff_l1 + lamb_coefdiff * coeff_diff_l1
 
             return reg_
 
         pbar = tqdm(range(steps), desc="description", ncols=100)
 
-        if loss_fn == None:
+        if loss_fn is None:
             loss_fn = loss_fn_eval = lambda x, y: torch.mean((x - y) ** 2)
         else:
             loss_fn = loss_fn_eval = loss_fn
 
         grid_update_freq = int(stop_grid_update_step / grid_update_num)
 
         if opt == "Adam":
@@ -1104,15 +1135,15 @@
                 tolerance_ys=1e-32,
             )
 
         results = {}
         results["train_loss"] = []
         results["test_loss"] = []
         results["reg"] = []
-        if metrics != None:
+        if metrics is not None:
             for i in range(len(metrics)):
                 results[metrics[i].__name__] = []
 
         if batch == -1 or batch > dataset["train_input"].shape[0]:
             batch_size = dataset["train_input"].shape[0]
             batch_size_test = dataset["test_input"].shape[0]
         else:
@@ -1121,18 +1152,16 @@
 
         global train_loss, reg_
 
         def closure():
             global train_loss, reg_
             optimizer.zero_grad()
             pred = self.forward(dataset["train_input"][train_id].to(device))
-            if sglr_avoid == True:
-                id_ = torch.where(
-                    torch.isnan(torch.sum(pred, dim=1)) == False
-                )[0]
+            if sglr_avoid:
+                id_ = torch.where(~torch.isnan(torch.sum(pred, dim=1)))[0]
                 train_loss = loss_fn(
                     pred[id_], dataset["train_label"][train_id][id_].to(device)
                 )
             else:
                 train_loss = loss_fn(
                     pred, dataset["train_label"][train_id].to(device)
                 )
@@ -1166,18 +1195,16 @@
             if opt == "LBFGS":
                 optimizer.step(closure)
 
             if opt == "Adam":
                 pred = self.forward(
                     dataset["train_input"][train_id].to(device)
                 )
-                if sglr_avoid == True:
-                    id_ = torch.where(
-                        torch.isnan(torch.sum(pred, dim=1)) == False
-                    )[0]
+                if sglr_avoid:
+                    id_ = torch.where(~torch.isnan(torch.sum(pred, dim=1)))[0]
                     train_loss = loss_fn(
                         pred[id_],
                         dataset["train_label"][train_id][id_].to(device),
                     )
                 else:
                     train_loss = loss_fn(
                         pred, dataset["train_label"][train_id].to(device)
@@ -1199,15 +1226,15 @@
                     % (
                         torch.sqrt(train_loss).cpu().detach().numpy(),
                         torch.sqrt(test_loss).cpu().detach().numpy(),
                         reg_.cpu().detach().numpy(),
                     )
                 )
 
-            if metrics != None:
+            if metrics is not None:
                 for i in range(len(metrics)):
                     results[metrics[i].__name__].append(metrics[i]().item())
 
             results["train_loss"].append(
                 torch.sqrt(train_loss).cpu().detach().numpy()
             )
             results["test_loss"].append(
@@ -1230,24 +1257,30 @@
                 )
                 plt.close()
 
         return results
 
     def prune(self, threshold=1e-2, mode="auto", active_neurons_id=None):
         """
-        pruning KAN on the node level. If a node has small incoming or outgoing connection, it will be pruned away.
+        pruning KAN on the node level. If a node has small incoming or
+        outgoing connection, it will be pruned away.
 
         Args:
         -----
             threshold : float
                 the threshold used to determine whether a node is small enough
             mode : str
-                "auto" or "manual". If "auto", the thresold will be used to automatically prune away nodes. If "manual", active_neuron_id is needed to specify which neurons are kept (others are thrown away).
+                "auto" or "manual". If "auto", the thresold will be used to
+                automatically prune away nodes. If "manual", active_neuron_id
+                is needed to specify which neurons are kept
+                (others are thrown away).
             active_neuron_id : list of id lists
-                For example, [[0,1],[0,2,3]] means keeping the 0/1 neuron in the 1st hidden layer and the 0/2/3 neuron in the 2nd hidden layer. Pruning input and output neurons is not supported yet.
+                For example, [[0,1],[0,2,3]] means keeping the 0/1 neuron in
+                the 1st hidden layer and the 0/2/3 neuron in the 2nd hidden
+                layer. Pruning input and output neurons is not supported yet.
 
         Returns:
         --------
             model2 : KAN
                 pruned model
 
         Example
@@ -1278,15 +1311,15 @@
                 overall_important = in_important * out_important
             elif mode == "manual":
                 overall_important = torch.zeros(
                     self.width[i + 1], dtype=torch.bool
                 )
                 overall_important[active_neurons_id[i + 1]] = True
             mask.append(overall_important.float())
-            active_neurons.append(torch.where(overall_important == True)[0])
+            active_neurons.append(torch.where(~overall_important)[0])
         active_neurons.append(list(range(self.width[-1])))
         mask.append(
             torch.ones(
                 self.width[-1],
             )
         )
 
@@ -1338,15 +1371,16 @@
         --------
             None
         """
         self.act_fun[l].mask[j * self.width[l] + i] = 0.0
 
     def remove_node(self, l, i):
         """
-        remove neuron (l,i) (set the masks of all incoming and outgoing activation functions to zero)
+        remove neuron (l,i) (set the masks of all incoming and outgoing
+        activation functions to zero)
 
         Args:
         -----
             l : int
                 layer index
             i : int
                 neuron index
@@ -1382,15 +1416,16 @@
             l : int
                 layer index
             i : int
                 input neuron index
             j : int
                 output neuron index
             lib : dic
-                library of symbolic bases. If lib = None, the global default library will be used.
+                library of symbolic bases. If lib = None, the global default
+                library will be used.
             topk : int
                 display the top k symbolic functions (according to r2)
             verbose : bool
                 If True, more information will be printed.
 
         Returns:
         --------
@@ -1410,15 +1445,15 @@
         gaussian , 0.9196369051933289
         tanh , 0.8608126044273376
         sigmoid , 0.8578218817710876
         arctan , 0.842217743396759
         """
         r2s = []
 
-        if lib == None:
+        if lib is None:
             symbolic_lib = SYMBOLIC_LIB
         else:
             symbolic_lib = {}
             for item in lib:
                 symbolic_lib[item] = SYMBOLIC_LIB[item]
 
         for name, fun in symbolic_lib.items():
@@ -1428,15 +1463,15 @@
             r2s.append(r2.item())
 
         self.unfix_symbolic(l, i, j)
 
         sorted_ids = np.argsort(r2s)[::-1][:topk]
         r2s = np.array(r2s)[sorted_ids][:topk]
         topk = np.minimum(topk, len(symbolic_lib))
-        if verbose == True:
+        if verbose:
             print("function", ",", "r2")
             for i in range(topk):
                 print(
                     list(symbolic_lib.items())[sorted_ids[i]][0], ",", r2s[i]
                 )
 
         best_name = list(symbolic_lib.items())[sorted_ids[0]][0]
@@ -1444,15 +1479,16 @@
         best_r2 = r2s[0]
         return best_name, best_fun, best_r2
 
     def auto_symbolic(
         self, a_range=(-10, 10), b_range=(-10, 10), lib=None, verbose=1
     ):
         """
-        automatic symbolic regression: using top 1 suggestion from suggest_symbolic to replace splines with symbolic activations
+        automatic symbolic regression: using top 1 suggestion from
+        suggest_symbolic to replace splines with symbolic activations
 
         Args:
         -----
             lib : None or a list of function names
                 the symbolic library
             verbose : int
                 verbosity
@@ -1517,57 +1553,61 @@
         obtain the symbolic formula
 
         Args:
         -----
             floating_digit : int
                 the number of digits to display
             var : list of str
-                the name of variables (if not provided, by default using ['x_1', 'x_2', ...])
+                the name of variables (if not provided, by default using
+                ['x_1', 'x_2', ...])
             normalizer : [mean array (floats), varaince array (floats)]
                 the normalization applied to inputs
             simplify : bool
-                If True, simplify the equation at each step (usually quite slow), so set up False by default.
+                If True, simplify the equation at each step
+                (usually quite slow), so set up False by default.
 
         Returns:
         --------
             symbolic formula : sympy function
 
         Example
         -------
-        >>> model = KAN(width=[2,5,1], grid=5, k=3, noise_scale=0.1, seed=0, grid_eps=0.02)
+        >>> model = KAN(width=[2,5,1], grid=5, k=3, noise_scale=0.1, seed=0, \
+            grid_eps=0.02)
         >>> f = lambda x: torch.exp(torch.sin(torch.pi*x[:,[0]]) + x[:,[1]]**2)
         >>> dataset = create_dataset(f, n_var=2)
         >>> model.train(dataset, opt='LBFGS', steps=50, lamb=0.01);
         >>> model = model.prune()
         >>> model(dataset['train_input'])
         >>> model.auto_symbolic(lib=['exp','sin','x^2'])
-        >>> model.train(dataset, opt='LBFGS', steps=50, lamb=0.00, update_grid=False);
+        >>> model.train(dataset, opt='LBFGS', steps=50, lamb=0.00, \
+            update_grid=False);
         >>> model.symbolic_formula()
         """
         symbolic_acts = []
         x = []
 
         def ex_round(ex1, floating_digit=floating_digit):
             ex2 = ex1
             for a in sympy.preorder_traversal(ex1):
                 if isinstance(a, sympy.Float):
                     ex2 = ex2.subs(a, round(a, floating_digit))
             return ex2
 
         # define variables
-        if var == None:
+        if var is None:
             for ii in range(1, self.width[0] + 1):
                 exec(f"x{ii} = sympy.Symbol('x_{ii}')")
                 exec(f"x.append(x{ii})")
         else:
             x = [sympy.symbols(var_) for var_ in var]
 
         x0 = x
 
-        if normalizer != None:
+        if normalizer is not None:
             mean = normalizer[0]
             std = normalizer[1]
             x = [(x[i] - mean[i]) / std[i] for i in range(len(x))]
 
         symbolic_acts.append(x)
 
         for l in range(len(self.width) - 1):
@@ -1575,20 +1615,21 @@
             for j in range(self.width[l + 1]):
                 yj = 0.0
                 for i in range(self.width[l]):
                     a, b, c, d = self.symbolic_fun[l].affine[j, i]
                     sympy_fun = self.symbolic_fun[l].funs_sympy[j][i]
                     try:
                         yj += c * sympy_fun(a * x[i] + b) + d
-                    except:
+                    except:  # noqa
                         print(
-                            "make sure all activations need to be converted to symbolic formulas first!"
+                            "make sure all activations need to be converted \
+                                to symbolic formulas first!"
                         )
                         return
-                if simplify == True:
+                if simplify:
                     y.append(
                         sympy.simplify(yj + self.biases[l].weight.data[0, j])
                     )
                 else:
                     y.append(yj + self.biases[l].weight.data[0, j])
 
             x = y
@@ -1598,15 +1639,15 @@
             [
                 ex_round(symbolic_acts[l][i])
                 for i in range(len(symbolic_acts[l]))
             ]
             for l in range(len(symbolic_acts))
         ]
 
-        out_dim = len(symbolic_acts[-1])
+        out_dim = len(symbolic_acts[-1])  # noqa
         return [
             ex_round(symbolic_acts[-1][i])
             for i in range(len(symbolic_acts[-1]))
         ], x0
 
     def clear_ckpts(self, folder="./model_ckpt"):
         """
```

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/KANLayer.py` & `kan_gpt-0.1.1/kan_gpt/kan/KANLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import torch
 import torch.nn as nn
 
-from .spline import *
+from .spline import coef2curve, curve2coef
 
 
 class KANLayer(nn.Module):
     """
     KANLayer class
 
 
@@ -487,15 +487,15 @@
         num = len(ids)
         locked = True
         for i in range(num):
             locked *= (
                 self.weight_sharing[ids[i][1] * self.in_dim + ids[i][0]]
                 == self.weight_sharing[ids[0][1] * self.in_dim + ids[0][0]]
             )
-        if locked == False:
+        if not locked:
             print("they are not locked. unlock failed.")
             return 0
         for i in range(len(ids)):
             self.weight_sharing[ids[i][1] * self.in_dim + ids[i][0]] = (
                 ids[i][1] * self.in_dim + ids[i][0]
             )
             self.lock_id[ids[i][1] * self.in_dim + ids[i][0]] = 0
```

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/LBFGS.py` & `kan_gpt-0.1.1/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-0.1.1/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 
-from .utils import *
+from .utils import SYMBOLIC_LIB, fit_params
 
 
 class Symbolic_KANLayer(nn.Module):
     """
     KANLayer class
 
     Attributes:
@@ -100,15 +100,15 @@
         >>> sb = Symbolic_KANLayer(in_dim=3, out_dim=5)
         >>> x = torch.normal(0,1,size=(100,3))
         >>> y, postacts = sb(x)
         >>> y.shape, postacts.shape
         (torch.Size([100, 5]), torch.Size([100, 5, 3]))
         """
 
-        batch = x.shape[0]
+        batch = x.shape[0]  # noqa
         postacts = []
 
         for i in range(self.in_dim):
             postacts_ = []
             for j in range(self.out_dim):
                 xij = (
                     self.affine[j, i, 2]
@@ -226,18 +226,18 @@
         tensor([2.9981, 1.9997, 5.0039, 0.6978])
         """
         if isinstance(fun_name, str):
             fun = SYMBOLIC_LIB[fun_name][0]
             fun_sympy = SYMBOLIC_LIB[fun_name][1]
             self.funs_sympy[j][i] = fun_sympy
             self.funs_name[j][i] = fun_name
-            if x == None or y == None:
+            if x is None or y is None:
                 # initialzie from just fun
                 self.funs[j][i] = fun
-                if random == False:
+                if not random:
                     self.affine.data[j][i] = torch.tensor([1.0, 0.0, 1.0, 0.0])
                 else:
                     self.affine.data[j][i] = (
                         torch.rand(
                             4,
                         )
                         * 2
@@ -261,15 +261,15 @@
             # if fun_name itself is a function
             fun = fun_name
             fun_sympy = fun_name
             self.funs_sympy[j][i] = fun_sympy
             self.funs_name[j][i] = "anonymous"
 
             self.funs[j][i] = fun
-            if random == False:
+            if not random:
                 self.affine.data[j][i] = torch.tensor([1.0, 0.0, 1.0, 0.0])
             else:
                 self.affine.data[j][i] = (
                     torch.rand(
                         4,
                     )
                     * 2
```

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-0.1.1/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/spline.py` & `kan_gpt-0.1.1/kan_gpt/kan/spline.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         for i in range(k_extend):
             grid = torch.cat([grid[:, [0]] - h, grid], dim=1)
             grid = torch.cat([grid, grid[:, [-1]] + h], dim=1)
         grid = grid.to(device)
         return grid
 
-    if extend == True:
+    if extend:
         grid = extend_grid(grid, k_extend=k)
 
     grid = grid.unsqueeze(dim=2).to(device)
     x = x.unsqueeze(dim=1).to(device)
 
     if k == 0:
         value = (x >= grid[:, :-1]) * (x < grid[:, 1:])
```

### Comparing `kan_gpt-0.1.0/kan_gpt/kan/utils.py` & `kan_gpt-0.1.1/kan_gpt/kan/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "abs": (lambda x: torch.abs(x), lambda x: sympy.Abs(x)),
     "sin": (lambda x: torch.sin(x), lambda x: sympy.sin(x)),
     "tan": (lambda x: torch.tan(x), lambda x: sympy.tan(x)),
     "tanh": (lambda x: torch.tanh(x), lambda x: sympy.tanh(x)),
     "sigmoid": (lambda x: torch.sigmoid(x), sympy.Function("sigmoid")),
     # 'relu': (lambda x: torch.relu(x), relu),
     "sgn": (lambda x: torch.sign(x), lambda x: sympy.sign(x)),
-    "arcsin": (lambda x: torch.arcsin(x), lambda x: sympy.arcsin(x)),
+    "arcsin": (lambda x: torch.arcsin(x), lambda x: sympy.asin(x)),
     "arctan": (lambda x: torch.arctan(x), lambda x: sympy.atan(x)),
     "arctanh": (lambda x: torch.arctanh(x), lambda x: sympy.atanh(x)),
     "0": (lambda x: x * 0, lambda x: x * 0),
     "gaussian": (lambda x: torch.exp(-(x**2)), lambda x: sympy.exp(-(x**2))),
     "cosh": (lambda x: torch.cosh(x), lambda x: sympy.cosh(x)),
     # 'logcosh': (lambda x: torch.log(torch.cosh(x)), lambda x: sympy.log(sympy.cosh(x))),
     # 'cosh^2': (lambda x: torch.cosh(x)**2, lambda x: sympy.cosh(x)**2),
@@ -111,21 +111,21 @@
 
     train_label = f(train_input)
     test_label = f(test_input)
 
     def normalize(data, mean, std):
         return (data - mean) / std
 
-    if normalize_input == True:
+    if normalize_input:
         mean_input = torch.mean(train_input, dim=0, keepdim=True)
         std_input = torch.std(train_input, dim=0, keepdim=True)
         train_input = normalize(train_input, mean_input, std_input)
         test_input = normalize(test_input, mean_input, std_input)
 
-    if normalize_label == True:
+    if normalize_label:
         mean_label = torch.mean(train_label, dim=0, keepdim=True)
         std_label = torch.std(train_label, dim=0, keepdim=True)
         train_label = normalize(train_label, mean_label, std_label)
         test_label = normalize(test_label, mean_label, std_label)
 
     dataset = {}
     dataset["train_input"] = train_input.to(device)
@@ -226,39 +226,40 @@
 
         if (
             a_id == 0
             or a_id == grid_number - 1
             or b_id == 0
             or b_id == grid_number - 1
         ):
-            if _ == 0 and verbose == True:
+            if _ == 0 and verbose:
                 print("Best value at boundary.")
             if a_id == 0:
-                a_arange = [a_[0], a_[1]]
+                a_arange = [a_[0], a_[1]]  # noqa
             if a_id == grid_number - 1:
-                a_arange = [a_[-2], a_[-1]]
+                a_arange = [a_[-2], a_[-1]]  # noqa
             if b_id == 0:
-                b_arange = [b_[0], b_[1]]
+                b_arange = [b_[0], b_[1]]  # noqa
             if b_id == grid_number - 1:
-                b_arange = [b_[-2], b_[-1]]
+                b_arange = [b_[-2], b_[-1]]  # noqa
 
         else:
             a_range = [a_[a_id - 1], a_[a_id + 1]]
             b_range = [b_[b_id - 1], b_[b_id + 1]]
 
     a_best = a_[a_id]
     b_best = b_[b_id]
     post_fun = fun(a_best * x + b_best)
     r2_best = r2[a_id, b_id]
 
-    if verbose == True:
+    if verbose:
         print(f"r2 is {r2_best}")
         if r2_best < 0.9:
             print(
-                f"r2 is not very high, please double check if you are choosing the correct symbolic function."
+                "r2 is not very high, please double check if you are",
+                "choosing the correct symbolic function.",
             )
 
     post_fun = torch.nan_to_num(post_fun)
     reg = LinearRegression().fit(
         post_fun[:, None].detach().numpy(), y.detach().numpy()
     )
     c_best = torch.from_numpy(reg.coef_)[0]
```

### Comparing `kan_gpt-0.1.0/kan_gpt/mingpt/bpe.py` & `kan_gpt-0.1.1/kan_gpt/mingpt/bpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             while i < len(word):
 
                 # find the next occurence of first in the sequence of current words
                 try:
                     j = word.index(first, i)
                     new_word.extend(word[i:j])
                     i = j
-                except:
+                except:  # noqa
                     new_word.extend(word[i:])
                     break
 
                 # if this occurence is also followed by second, then merge them into one
                 if (
                     word[i] == first
                     and i < len(word) - 1
```

### Comparing `kan_gpt-0.1.0/kan_gpt/mingpt/model.py` & `kan_gpt-0.1.1/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/mingpt/trainer.py` & `kan_gpt-0.1.1/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/mingpt/utils.py` & `kan_gpt-0.1.1/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.1.0/kan_gpt/model.py` & `kan_gpt-0.1.1/kan_gpt/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Full definition of a GPT Language Model, all of it in this single file.
 
 References:
 1) the official GPT-2 TensorFlow implementation released by OpenAI:
 https://github.com/openai/gpt-2/blob/master/src/model.py
 2) huggingface/transformers PyTorch implementation:
-https://github.com/huggingface/transformers/blob/main/src/transformers/models/gpt2/modeling_gpt2.py
+https://github.com/huggingface/transformers/blob/main/src/transformers\
+/models/gpt2/modeling_gpt2.py
 """
 
 import math
 
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
@@ -18,16 +19,18 @@
 from kan_gpt.mingpt.utils import CfgNode as CN
 
 # -----------------------------------------------------------------------------
 
 
 class NewGELU(nn.Module):
     """
-    Implementation of the GELU activation function currently in Google BERT repo (identical to OpenAI GPT).
-    Reference: Gaussian Error Linear Units (GELU) paper: https://arxiv.org/abs/1606.08415
+    Implementation of the GELU activation function currently in Google BERT
+    repo (identical to OpenAI GPT).
+    Reference: Gaussian Error Linear Units (GELU) paper:
+    https://arxiv.org/abs/1606.08415
     """
 
     def forward(self, x):
         return (
             0.5
             * x
             * (
@@ -38,57 +41,61 @@
                 )
             )
         )
 
 
 class CausalSelfAttention(nn.Module):
     """
-    A vanilla multi-head masked self-attention layer with a projection at the end.
-    It is possible to use torch.nn.MultiheadAttention here but I am including an
-    explicit implementation here to show that there is nothing too scary here.
+    A vanilla multi-head masked self-attention layer with a projection at
+    the end. It is possible to use torch.nn.MultiheadAttention here but I am
+    including an explicit implementation here to show that there is nothing
+    too scary here.
     """
 
     def __init__(self, config):
         super().__init__()
         assert config.n_embd % config.n_head == 0
         # key, query, value projections for all heads, but in a batch
         self.c_attn = KAN(width=[config.n_embd, 3 * config.n_embd])
         # output projection
         self.c_proj = KAN(width=[config.n_embd, config.n_embd])
         # regularization
         self.attn_dropout = nn.Dropout(config.attn_pdrop)
         self.resid_dropout = nn.Dropout(config.resid_pdrop)
-        # causal mask to ensure that attention is only applied to the left in the input sequence
+        # causal mask to ensure that attention is only applied to the left in
+        # the input sequence
         self.register_buffer(
             "bias",
             torch.tril(torch.ones(config.block_size, config.block_size)).view(
                 1, 1, config.block_size, config.block_size
             ),
         )
         self.n_head = config.n_head
         self.n_embd = config.n_embd
 
     def forward(self, x):
         B, T, C = (
             x.size()
         )  # batch size, sequence length, embedding dimensionality (n_embd)
 
-        # calculate query, key, values for all heads in batch and move head forward to be the batch dim
+        # calculate query, key, values for all heads in batch and move head
+        # forward to be the batch dim
         q, k, v = self.c_attn(x).split(self.n_embd, dim=2)
         k = k.view(B, T, self.n_head, C // self.n_head).transpose(
             1, 2
         )  # (B, nh, T, hs)
         q = q.view(B, T, self.n_head, C // self.n_head).transpose(
             1, 2
         )  # (B, nh, T, hs)
         v = v.view(B, T, self.n_head, C // self.n_head).transpose(
             1, 2
         )  # (B, nh, T, hs)
 
-        # causal self-attention; Self-attend: (B, nh, T, hs) x (B, nh, hs, T) -> (B, nh, T, T)
+        # causal self-attention;
+        # Self-attend: (B, nh, T, hs) x (B, nh, hs, T) -> (B, nh, T, T)
         att = (q @ k.transpose(-2, -1)) * (1.0 / math.sqrt(k.size(-1)))
         att = att.masked_fill(self.bias[:, :, :T, :T] == 0, float("-inf"))
         att = F.softmax(att, dim=-1)
         att = self.attn_dropout(att)
         y = att @ v  # (B, nh, T, T) x (B, nh, T, hs) -> (B, nh, T, hs)
         y = (
             y.transpose(1, 2).contiguous().view(B, T, C)
@@ -128,15 +135,16 @@
 
 class GPT(nn.Module):
     """GPT Language Model"""
 
     @staticmethod
     def get_default_config():
         C = CN()
-        # either model_type or (n_layer, n_head, n_embd) must be given in the config
+        # either model_type or (n_layer, n_head, n_embd)
+        # must be given in the config
         C.model_type = "gpt"
         C.n_layer = None
         C.n_head = None
         C.n_embd = None
         # these options must be filled in externally
         C.vocab_size = None
         C.block_size = None
@@ -204,26 +212,83 @@
                 ln_f=nn.LayerNorm(config.n_embd),
             )
         )
         self.lm_head = KAN(
             width=[config.n_embd, config.vocab_size], bias_trainable=False
         )
 
-        # init all weights, and apply a special scaled init to the residual projections, per GPT-2 paper
+        # init all weights, and apply a special scaled init to the residual
+        # projections, per GPT-2 paper
         self.apply(self._init_weights)
         for pn, p in self.named_parameters():
             if pn.endswith("c_proj.weight"):
                 torch.nn.init.normal_(
                     p, mean=0.0, std=0.02 / math.sqrt(2 * config.n_layer)
                 )
 
-        # report number of parameters (note we don't count the decoder parameters in lm_head)
+        # report number of parameters (note we don't count the decoder
+        # parameters in lm_head)
         n_params = sum(p.numel() for p in self.transformer.parameters())
         print("number of parameters: %.2fM" % (n_params / 1e6,))
 
+    def kan_loss(
+        self,
+        x: torch.Tensor,
+        lamb_l1=1.0,
+        lamb_entropy=2.0,
+        lamb_coef=0.0,
+        lamb_coefdiff=0.0,
+        small_mag_threshold=1e-16,
+        small_reg_factor=1.0,
+    ):
+
+        def reg(mod):
+
+            def nonlinear(x, th=small_mag_threshold, factor=small_reg_factor):
+                return (x < th) * x * factor + (x > th) * (
+                    x + (factor - 1) * th
+                )
+
+            reg_ = 0.0
+            for i in range(len(mod.acts_scale)):
+                vec = mod.acts_scale[i].reshape(
+                    -1,
+                )
+
+                p = vec / torch.sum(vec)
+                l1 = torch.sum(nonlinear(vec))
+                entropy = -torch.sum(p * torch.log2(p + 1e-4))
+                reg_ += (
+                    lamb_l1 * l1 + lamb_entropy * entropy
+                )  # both l1 and entropy
+
+            # regularize coefficient to encourage spline to be zero
+            for i in range(len(mod.act_fun)):
+                coeff_l1 = torch.sum(
+                    torch.mean(torch.abs(mod.act_fun[i].coef), dim=1)
+                )
+                coeff_diff_l1 = torch.sum(
+                    torch.mean(
+                        torch.abs(torch.diff(mod.act_fun[i].coef)), dim=1
+                    )
+                )
+                reg_ += lamb_coef * coeff_l1 + lamb_coefdiff * coeff_diff_l1
+
+            return reg_
+
+        total_reg = torch.tensor(0.0).to(device=x.device, dtype=torch.float32)
+        size = 0
+        for mod in self.modules():
+            if isinstance(mod, KAN):
+                total_reg += reg(mod)
+                size += 1
+
+        mean_reg = total_reg / size
+        return mean_reg
+
     def _init_weights(self, module):
         if isinstance(module, KAN):
             # torch.nn.init.normal_(module.weight, mean=0.0, std=0.02)
             # if module.bias is not None:
             #     torch.nn.init.zeros_(module.bias)
             # TODO: init weights
             pass
@@ -250,26 +315,28 @@
         model = GPT(config)
         sd = model.state_dict()
 
         # init a huggingface/transformers model
         model_hf = GPT2LMHeadModel.from_pretrained(model_type)
         sd_hf = model_hf.state_dict()
 
-        # copy while ensuring all of the parameters are aligned and match in names and shapes
+        # copy while ensuring all of the parameters are aligned and
+        # match in names and shapes
         keys = [
             k for k in sd_hf if not k.endswith("attn.masked_bias")
         ]  # ignore these
         transposed = [
             "attn.c_attn.weight",
             "attn.c_proj.weight",
             "mlp.c_fc.weight",
             "mlp.c_proj.weight",
         ]
-        # basically the openai checkpoints use a "Conv1D" module, but we only want to use a vanilla nn.Linear.
-        # this means that we have to transpose these weights when we import them
+        # basically the openai checkpoints use a "Conv1D" module, but we only
+        # want to use a vanilla nn.Linear. this means that we have to
+        # transpose these weights when we import them
         assert len(keys) == len(sd)
         for k in keys:
             if any(k.endswith(w) for w in transposed):
                 # special treatment for the Conv1D weights we need to transpose
                 assert sd_hf[k].shape[::-1] == sd[k].shape
                 with torch.no_grad():
                     sd[k].copy_(sd_hf[k].t())
@@ -279,31 +346,34 @@
                 with torch.no_grad():
                     sd[k].copy_(sd_hf[k])
 
         return model
 
     def configure_optimizers(self, train_config):
         """
-        This long function is unfortunately doing something very simple and is being very defensive:
-        We are separating out all parameters of the model into two buckets: those that will experience
-        weight decay for regularization and those that won't (biases, and layernorm/embedding weights).
-        We are then returning the PyTorch optimizer object.
+        This long function is unfortunately doing something very simple and
+        is being very defensive: We are separating out all parameters of the
+        model into two buckets: those that will experience weight decay for
+        regularization and those that won't (biases, and layernorm/embedding
+        weights). We are then returning the PyTorch optimizer object.
         """
 
-        # separate out all parameters to those that will and won't experience regularizing weight decay
+        # separate out all parameters to those that will and won't experience
+        # regularizing weight decay
         decay = set()
         no_decay = set()
         whitelist_weight_modules = (KAN,)
         blacklist_weight_modules = (torch.nn.LayerNorm, torch.nn.Embedding)
         for mn, m in self.named_modules():
             for pn, p in m.named_parameters():
                 fpn = "%s.%s" % (mn, pn) if mn else pn  # full param name
-                # random note: because named_modules and named_parameters are recursive
-                # we will see the same tensors p many many times. but doing it this way
-                # allows us to know which parent module any tensor p belongs to...
+                # random note: because named_modules and named_parameters
+                # are recursive we will see the same tensors p many many
+                # times. but doing it this way allows us to know which
+                # parent module any tensor p belongs to...
                 if pn.endswith("bias"):
                     # all biases will not be decayed
                     no_decay.add(fpn)
                 elif isinstance(m, whitelist_weight_modules):
                     # weights of whitelist modules will be weight decayed
                     decay.add(fpn)
                 elif pn.endswith("weight") and isinstance(
@@ -340,20 +410,32 @@
         optimizer = torch.optim.AdamW(
             optim_groups,
             lr=train_config.learning_rate,
             betas=train_config.betas,
         )
         return optimizer
 
-    def forward(self, idx, targets=None):
+    def forward(
+        self,
+        idx,
+        targets=None,
+        lamb=0.01,
+        lamb_l1=1.0,
+        lamb_entropy=2.0,
+        lamb_coef=0.0,
+        lamb_coefdiff=0.0,
+        small_mag_threshold=1e-16,
+        small_reg_factor=1.0,
+    ):
         device = idx.device
         b, t = idx.size()
-        assert (
-            t <= self.block_size
-        ), f"Cannot forward sequence of length {t}, block size is only {self.block_size}"
+        assert t <= self.block_size, (
+            f"Cannot forward sequence of length {t}, "
+            f"block size is only {self.block_size}"
+        )
         pos = torch.arange(0, t, dtype=torch.long, device=device).unsqueeze(
             0
         )  # shape (1, t)
 
         # forward the GPT model itself
         tok_emb = self.transformer.wte(
             idx
@@ -372,43 +454,59 @@
         if targets is not None:
             loss = F.cross_entropy(
                 logits.view(-1, logits.size(-1)),
                 targets.view(-1),
                 ignore_index=-1,
             )
 
+            reg = self.kan_loss(
+                x=idx,
+                lamb_l1=lamb_l1,
+                lamb_entropy=lamb_entropy,
+                lamb_coef=lamb_coef,
+                lamb_coefdiff=lamb_coefdiff,
+                small_mag_threshold=small_mag_threshold,
+                small_reg_factor=small_reg_factor,
+            )
+            loss = loss + lamb * reg
+
         return logits, loss
 
     @torch.no_grad()
     def generate(
         self, idx, max_new_tokens, temperature=1.0, do_sample=False, top_k=None
     ):
         """
-        Take a conditioning sequence of indices idx (LongTensor of shape (b,t)) and complete
-        the sequence max_new_tokens times, feeding the predictions back into the model each time.
-        Most likely you'll want to make sure to be in model.eval() mode of operation for this.
+        Take a conditioning sequence of indices idx (LongTensor of shape
+        (b,t)) and complete the sequence max_new_tokens times, feeding the
+        predictions back into the model each time. Most likely you'll want
+        to make sure to be in model.eval() mode of operation for this.
         """
         for _ in range(max_new_tokens):
-            # if the sequence context is growing too long we must crop it at block_size
+            # if the sequence context is growing too long we must crop it at
+            # block_size
             idx_cond = (
                 idx
                 if idx.size(1) <= self.block_size
                 else idx[:, -self.block_size :]
             )
-            # forward the model to get the logits for the index in the sequence
+            # forward the model to get the logits for the index in the
+            # sequence
             logits, _ = self(idx_cond)
-            # pluck the logits at the final step and scale by desired temperature
+            # pluck the logits at the final step and scale by desired
+            # temperature
             logits = logits[:, -1, :] / temperature
             # optionally crop the logits to only the top k options
             if top_k is not None:
                 v, _ = torch.topk(logits, top_k)
                 logits[logits < v[:, [-1]]] = -float("Inf")
             # apply softmax to convert logits to (normalized) probabilities
             probs = F.softmax(logits, dim=-1)
-            # either sample from the distribution or take the most likely element
+            # either sample from the distribution or take the most likely
+            # element
             if do_sample:
                 idx_next = torch.multinomial(probs, num_samples=1)
             else:
                 _, idx_next = torch.topk(probs, k=1, dim=-1)
             # append sampled index to the running sequence and continue
             idx = torch.cat((idx, idx_next), dim=1)
```

### Comparing `kan_gpt-0.1.0/kan_gpt/train.py` & `kan_gpt-0.1.1/kan_gpt/train.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 from torch.utils.data.dataloader import DataLoader
 
 import wandb
 from kan_gpt.dataset import WebTextDataset
 from kan_gpt.mingpt.model import GPT as MLP_GPT
 from kan_gpt.mingpt.trainer import Trainer
-from kan_gpt.mingpt.utils import set_seed
 from kan_gpt.model import GPT as KAN_GPT
 
+
 def eval_split(
     trainer, split, max_batches, batch_size, model, train_dataset, test_dataset
 ):
     dataset = {"train": train_dataset, "test": test_dataset}[split]
     results = []
 
     loader = DataLoader(
@@ -37,30 +37,28 @@
         "model_type": args.model_type,
         "batch_size": args.batch_size,
         "dummy_dataset": args.dummy_dataset,
         "learning_rate": args.learning_rate,
         "max_iters": args.max_iters,
         "num_workers": args.num_workers,
         "architecture": args.architecture,
+        "device": args.device,
     }
 
-    wandb.init(
-        project="KAN-GPT",
-        config=config
-    )
+    wandb.init(project="KAN-GPT", config=config)
 
     model_type = args.model_type
 
     # print an example instance of the dataset
     if args.dummy_dataset:
-        train_dataset = WebTextDataset("test", model_type)
+        train_dataset = WebTextDataset("test", "gpt2")
     else:
-        train_dataset = WebTextDataset("train", model_type)
+        train_dataset = WebTextDataset("train", "gpt2")
 
-    test_dataset = WebTextDataset("test", model_type)
+    test_dataset = WebTextDataset("test", "gpt2")
 
     if args.architecture == "KAN":
         GPT = KAN_GPT
     else:
         GPT = MLP_GPT
 
     # create a GPT instance
@@ -76,21 +74,24 @@
     train_config = Trainer.get_default_config()
     train_config.learning_rate = float(
         args.learning_rate
     )  # the model we're using is so small that we can go a bit faster
     train_config.max_iters = int(args.max_iters)
     train_config.num_workers = int(args.num_workers)
     train_config.batch_size = int(args.batch_size)
+    train_config.device = args.device
     trainer = Trainer(train_config, model, train_dataset)
 
     def batch_end_callback(trainer):
         # TODO: Add W&B Hooks
         if trainer.iter_num % 100 == 0:
             print(
-                f"iter_dt {trainer.iter_dt * 1000:.2f}ms; iter {trainer.iter_num}: train loss {trainer.loss.item():.5f}"
+                f"iter_dt {trainer.iter_dt * 1000:.2f}ms; "
+                f"iter {trainer.iter_num}: "
+                f"train loss {trainer.loss.item():.5f}"
             )
 
             print("=" * 20)
             print("EVAL")
             print("=" * 20)
 
             model.eval()
@@ -132,24 +133,27 @@
     trainer.run()
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser("KAN-GPT Trainer")
-    parser.add_argument("--model_type", default="gpt2")
+    parser.add_argument("--model_type", default="gpt-nano")
     parser.add_argument("--dummy_dataset", action="store_true")
     parser.add_argument("--learning_rate", default=5e-3)
     parser.add_argument("--max_iters", default=2000)
     parser.add_argument("--num_workers", default=0)
     parser.add_argument("--batch_size", default=64)
 
     parser.add_argument(
         "--architecture", choices=["MLP", "KAN"], default="KAN"
     )
+    parser.add_argument(
+        "--device", choices=["auto", "cpu", "cuda"], default="auto"
+    )
 
     args = parser.parse_args()
 
     args.learning_rate = float(args.learning_rate)
     args.max_iters = int(args.max_iters)
     args.num_workers = int(args.num_workers)
     args.batch_size = int(args.batch_size)
```

### Comparing `kan_gpt-0.1.0/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-0.1.1/kan_gpt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -31,15 +31,15 @@
 Requires-Dist: types-requests; extra == "test"
 
 # KAN-GPT
 
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
 
-Awesome KAN-GPT created by AdityaNG
+The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
@@ -50,67 +50,85 @@
 
 model_config = GPT.get_default_config()
 model_config.model_type = "gpt2"
 model_config.vocab_size = 5
 model_config.block_size = 10
 model = GPT(model_config)
 
+tokenizer = GPT2Tokenizer.from_pretrained('gpt2')
+
 x = torch.zeros((1, 10), dtype=torch.long)
 y = torch.zeros((1, 10), dtype=torch.long)
 
-# x = x.cuda()
-# y = y.cuda()
-# model = model.cuda()
-
-logits, loss = model(x, y)
+prompt = "Bangalore is often described as the "
 
-print(logits.shape)
-```
+prompt_encoded = tokenizer.encode(
+  text=prompt, add_special_tokens=False
+)
+
+result = prompt
+x = torch.tensor(prompt_encoded).unsqueeze(0)
+
+for _ in range(50):  # sample 50 tokens
+  logits, loss = model(x)
+  x = torch.cat(
+    (x[:, 1:-2], logits[:, -2:-1]), dim=0
+  )
+  result += tokenizer.decode(logits[0, -2:-1])
 
-```bash
-$ python -m kan_gpt.train
+print(result)
 ```
 
-## Setup
+## Setup for Development
 
 ```bash
 # Download Repo
-%cd /content
-!git clone https://github.com/AdityaNG/kan-gpt
-%cd kan-gpt
-!git pull
+git clone https://github.com/AdityaNG/kan-gpt
+cd kan-gpt
+git pull
 
 # Download Dataset
-!./scripts/download_webtext.sh
+./scripts/download_webtext.sh
 
 # Install dependencies for development
-!pip install -r requirements.txt
-!pip install -e .
+pip install -r requirements.txt
+pip install -e .
 ```
 
 ## Train
 
-Dummy script to make sure everything is working as expected
+Use the following dummy script to make sure everything is working as expected
+```bash
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset --device cpu
+WANDB_MODE=offline CUDA_VISIBLE_DEVICE="" python3 -m kan_gpt.train --architecture KAN --batch_size 1 --dummy_dataset --device cpu
+```
+
+Then make use of the training script
 ```bash
-CUDA_VISIBLE_DEVICE="0" python3 -m kan_gpt.train --architecture MLP --batch_size 1 --dummy_dataset
+python -m kan_gpt.train
 ```
 
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [ ] Mini training POC for KAN-GPT
-  - [ ] Integrate KAN training logic from `KAN.train_kan`
+  - [x] Integrate KAN training logic from `KAN.train_kan`
+  - [ ] Train a dummy batch
 - [x] Mini training POC for MLP-GPT
 - [x] Train MLP-GPT on the webtext dataset as a baseline
 - [ ] Auto Save checkpoints
 - [ ] Auto Save checkpoints to W&B
 - [ ] Script to load checkpoint in interactive mode
 - [ ] Training script to PyTorch Lighting
+- [ ] Test Cases
+  - [x] KAN: Forward-Backward test
+  - [x] GPT: Forward-Backward test
+  - [x] KAN_GPT: Forward-Backward test
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## References
```

### Comparing `kan_gpt-0.1.0/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-0.1.1/kan_gpt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,8 +43,11 @@
 kan_gpt/mingpt/__init__.py
 kan_gpt/mingpt/bpe.py
 kan_gpt/mingpt/model.py
 kan_gpt/mingpt/trainer.py
 kan_gpt/mingpt/utils.py
 tests/__init__.py
 tests/conftest.py
-tests/test_base.py
+tests/test_base.py
+tests/test_gpt_kan.py
+tests/test_gpt_mlp.py
+tests/test_kan.py
```

### Comparing `kan_gpt-0.1.0/setup.py` & `kan_gpt-0.1.1/setup.py`

 * *Files identical despite different names*

