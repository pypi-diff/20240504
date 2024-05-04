# Comparing `tmp/foundation_cancer_image_biomarker-1.0.1a0.tar.gz` & `tmp/foundation_cancer_image_biomarker-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-1.0.1a0.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-1.0.1a1.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-1.0.1a0.tar` & `foundation_cancer_image_biomarker-1.0.1a1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1076 2024-04-23 19:10:19.003139 foundation_cancer_image_biomarker-1.0.1a0/LICENSE
--rw-r--r--   0        0        0     2340 2024-04-23 19:10:19.003139 foundation_cancer_image_biomarker-1.0.1a0/README.md
--rw-r--r--   0        0        0       24 2024-04-23 19:10:40.251048 foundation_cancer_image_biomarker-1.0.1a0/fmcib/__init__.py
--rw-r--r--   0        0        0       46 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/callbacks/__init__.py
--rw-r--r--   0        0        0     3355 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/callbacks/prediction_saver.py
--rw-r--r--   0        0        0     1069 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/callbacks/utils.py
--rw-r--r--   0        0        0     3193 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/datasets/__init__.py
--rw-r--r--   0        0        0     7460 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/datasets/ssl_radiomics_dataset.py
--rw-r--r--   0        0        0     2922 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/datasets/utils.py
--rw-r--r--   0        0        0     1221 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/__init__.py
--rw-r--r--   0        0        0     3912 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/autoencoder.py
--rw-r--r--   0        0        0     4881 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/load_model.py
--rw-r--r--   0        0        0    13087 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/models_genesis.py
--rw-r--r--   0        0        0       23 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/optimizers/__init__.py
--rw-r--r--   0        0        0     6826 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/optimizers/lars.py
--rw-r--r--   0        0        0     2532 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     5641 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0     2308 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/run.py
--rw-r--r--   0        0        0        0 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/__init__.py
--rw-r--r--   0        0        0      226 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/__init__.py
--rw-r--r--   0        0        0     8551 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/neg_mining_info_nce_loss.py
--rw-r--r--   0        0        0     1110 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/nnclr_loss.py
--rw-r--r--   0        0        0      967 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/ntxent_loss.py
--rw-r--r--   0        0        0     4490 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/ntxent_mined_loss.py
--rw-r--r--   0        0        0     1872 2024-04-23 19:10:19.779139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/swav_loss.py
--rw-r--r--   0        0        0      113 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/exneg_simclr.py
--rw-r--r--   0        0        0     2809 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/nnclr.py
--rw-r--r--   0        0        0     1922 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/simclr.py
--rw-r--r--   0        0        0     7822 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/swav.py
--rw-r--r--   0        0        0      166 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/__init__.py
--rw-r--r--   0        0        0     1373 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/duplicate.py
--rw-r--r--   0        0        0     1385 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/med3d.py
--rw-r--r--   0        0        0     1709 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/multicrop.py
--rw-r--r--   0        0        0     1532 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/random_resized_crop.py
--rw-r--r--   0        0        0       67 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/utils/__init__.py
--rw-r--r--   0        0        0      680 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0     9373 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0       44 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0     3342 2024-04-23 19:10:19.783139 foundation_cancer_image_biomarker-1.0.1a0/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4570 2024-04-23 19:10:40.203048 foundation_cancer_image_biomarker-1.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-1.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-04 05:11:49.211526 foundation_cancer_image_biomarker-1.0.1a1/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-04 05:11:49.211526 foundation_cancer_image_biomarker-1.0.1a1/README.md
+-rw-r--r--   0        0        0       24 2024-05-04 05:12:11.291516 foundation_cancer_image_biomarker-1.0.1a1/fmcib/__init__.py
+-rw-r--r--   0        0        0       46 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/__init__.py
+-rw-r--r--   0        0        0     3355 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/prediction_saver.py
+-rw-r--r--   0        0        0     1069 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/utils.py
+-rw-r--r--   0        0        0     3193 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/__init__.py
+-rw-r--r--   0        0        0     7460 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/ssl_radiomics_dataset.py
+-rw-r--r--   0        0        0     2922 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/utils.py
+-rw-r--r--   0        0        0     1221 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/__init__.py
+-rw-r--r--   0        0        0     3912 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/autoencoder.py
+-rw-r--r--   0        0        0     4881 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/load_model.py
+-rw-r--r--   0        0        0    13087 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/models_genesis.py
+-rw-r--r--   0        0        0       23 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/optimizers/__init__.py
+-rw-r--r--   0        0        0     6826 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/optimizers/lars.py
+-rw-r--r--   0        0        0     2532 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5641 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0     2308 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/run.py
+-rw-r--r--   0        0        0        0 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/__init__.py
+-rw-r--r--   0        0        0     8551 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/neg_mining_info_nce_loss.py
+-rw-r--r--   0        0        0     1110 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/nnclr_loss.py
+-rw-r--r--   0        0        0      967 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_loss.py
+-rw-r--r--   0        0        0     4490 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_mined_loss.py
+-rw-r--r--   0        0        0     1872 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/swav_loss.py
+-rw-r--r--   0        0        0      113 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/__init__.py
+-rw-r--r--   0        0        0     1997 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/exneg_simclr.py
+-rw-r--r--   0        0        0     2809 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/nnclr.py
+-rw-r--r--   0        0        0     1922 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/simclr.py
+-rw-r--r--   0        0        0     7822 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/swav.py
+-rw-r--r--   0        0        0      166 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/__init__.py
+-rw-r--r--   0        0        0     1373 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/duplicate.py
+-rw-r--r--   0        0        0     1385 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/med3d.py
+-rw-r--r--   0        0        0     1709 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/multicrop.py
+-rw-r--r--   0        0        0     1532 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/random_resized_crop.py
+-rw-r--r--   0        0        0       67 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     9373 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0     3342 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4570 2024-05-04 05:12:11.247516 foundation_cancer_image_biomarker-1.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-1.0.1a1/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/LICENSE` & `foundation_cancer_image_biomarker-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/README.md` & `foundation_cancer_image_biomarker-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/callbacks/prediction_saver.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/prediction_saver.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/callbacks/utils.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/datasets/__init__.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/datasets/ssl_radiomics_dataset.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/ssl_radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/datasets/utils.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/__init__.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/autoencoder.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/load_model.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/load_model.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/models/models_genesis.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/models_genesis.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/optimizers/lars.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/preprocessing/__init__.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/seed_based_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/run.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/run.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/neg_mining_info_nce_loss.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/neg_mining_info_nce_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/nnclr_loss.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/nnclr_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/ntxent_loss.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/ntxent_mined_loss.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_mined_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/losses/swav_loss.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/swav_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/exneg_simclr.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/exneg_simclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/nnclr.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/nnclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/simclr.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/simclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/ssl/modules/swav.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/swav.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/duplicate.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/duplicate.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/med3d.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/med3d.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/multicrop.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/multicrop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/transforms/random_resized_crop.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/utils/download_utils.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/utils/idc_helper.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/idc_helper.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/fmcib/visualization/verify_io.py` & `foundation_cancer_image_biomarker-1.0.1a1/fmcib/visualization/verify_io.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/pyproject.toml` & `foundation_cancer_image_biomarker-1.0.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "1.0.1a0"
+version = "1.0.1a1"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
```

### Comparing `foundation_cancer_image_biomarker-1.0.1a0/PKG-INFO` & `foundation_cancer_image_biomarker-1.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundation-cancer-image-biomarker
-Version: 1.0.1a0
+Version: 1.0.1a1
 Summary: Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]
 Home-page: https://aim.hms.harvard.edu/foundation-cancer-image-biomarker
 License: MIT
 Author: Suraj Pai
 Author-email: bspai@bwh.harvard.edu
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundation-cancer-image-biomarker Version: 1.0.1a0
+Metadata-Version: 2.1 Name: foundation-cancer-image-biomarker Version: 1.0.1a1
 Summary: Official repo for Foundation Models for Quantitative Biomarker
 Discovery in Cancer Imaging [INSERT DOI] Home-page: https://
 aim.hms.harvard.edu/foundation-cancer-image-biomarker License: MIT Author:
 Suraj Pai Author-email: bspai@bwh.harvard.edu Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

