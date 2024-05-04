# Comparing `tmp/TensorFlowASR-1.0.3.tar.gz` & `tmp/TensorFlowASR-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TensorFlowASR-1.0.3.tar", last modified: Sat Mar 12 07:39:34 2022, max compression
+gzip compressed data, was "TensorFlowASR-2.0.0.tar", last modified: Sat May  4 17:02:01 2024, max compression
```

## Comparing `TensorFlowASR-1.0.3.tar` & `TensorFlowASR-2.0.0.tar`

### file list

```diff
@@ -1,96 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.451143 TensorFlowASR-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14050 2022-03-12 07:39:34.451143 TensorFlowASR-1.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)    11272 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/TensorFlowASR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14050 2022-03-12 07:39:34.000000 TensorFlowASR-1.0.3/TensorFlowASR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-03-12 07:39:34.000000 TensorFlowASR-1.0.3/TensorFlowASR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-12 07:39:34.000000 TensorFlowASR-1.0.3/TensorFlowASR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-03-12 07:39:34.000000 TensorFlowASR-1.0.3/TensorFlowASR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-12 07:39:34.000000 TensorFlowASR-1.0.3/TensorFlowASR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      224 2022-03-12 07:39:34.451143 TensorFlowASR-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/methods/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/methods/base_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/augmentations/methods/specaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/configs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/datasets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15814 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/datasets/asr_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/datasets/base_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/methods/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8724 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/methods/gammatone.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19625 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/speech_featurizers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19024 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/featurizers/text_featurizers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/helpers/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/helpers/exec_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/helpers/featurizer_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.443143 TensorFlowASR-1.0.3/tensorflow_asr/losses/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/losses/ctc_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)    13224 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/losses/rnnt_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.447143 TensorFlowASR-1.0.3/tensorflow_asr/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/metrics/error_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.447143 TensorFlowASR-1.0.3/tensorflow_asr/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.447143 TensorFlowASR-1.0.3/tensorflow_asr/models/activations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/activations/glu.py
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.447143 TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7819 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/base_ctc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12632 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/deepspeech2.py
--rw-r--r--   0 runner    (1001) docker     (121)    15186 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/jasper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.447143 TensorFlowASR-1.0.3/tensorflow_asr/models/encoders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15160 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/encoders/conformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7722 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/encoders/contextnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.447143 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2826 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/bnlstmcell.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (121)    11324 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/multihead_attention.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1710 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/point_wise_ffn.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3376 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/positional_encoding.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3309 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/row_conv_1d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/sequence_wise_bn.py
--rw-r--r--   0 runner    (1001) docker     (121)     6228 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/layers/subsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.451143 TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38678 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/base_transducer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/conformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8493 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/contextnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    14967 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/rnn_transducer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.451143 TensorFlowASR-1.0.3/tensorflow_asr/optimizers/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/optimizers/accumulation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5541 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/optimizers/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:34.451143 TensorFlowASR-1.0.3/tensorflow_asr/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/app_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/data_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/env_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/feature_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/layer_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/math_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/metric_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-03-12 07:39:22.000000 TensorFlowASR-1.0.3/tensorflow_asr/utils/shape_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8995 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      234 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/base_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/gaussnoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/specaugment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20538 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/features/gammatone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/losses/ctc_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/losses/rnnt_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/metrics/error_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/activations/glu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28243 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/base_ctc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/deepspeech2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/jasper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/decoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24566 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/contextnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/deepspeech2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/jasper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/rnnt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.399423 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/multihead_attention.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6990 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/sequence_wise_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/subsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.399423 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49153 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/base_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/contextnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/rnnt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.399423 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/regularizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4495 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16765 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/tensorflow_asr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/app_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/feature_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/layer_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/math_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/metric_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/plot_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/shape_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/tf_util.py
```

### Comparing `TensorFlowASR-1.0.3/LICENSE` & `TensorFlowASR-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-1.0.3/PKG-INFO` & `TensorFlowASR-2.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,251 +1,251 @@
 Metadata-Version: 2.1
 Name: TensorFlowASR
-Version: 1.0.3
+Version: 2.0.0
 Summary: Almost State-of-the-art Automatic Speech Recognition using Tensorflow 2
 Home-page: https://github.com/TensorSpeech/TensorFlowASR
 Author: Huy Le Nguyen
 Author-email: nlhuy.cs.16@gmail.com
-License: UNKNOWN
-Description: <h1 align="center">
-        <p>TensorFlowASR :zap:</p>
-        <p align="center">
-        <a href="https://github.com/TensorSpeech/TensorFlowASR/blob/main/LICENSE">
-          <img alt="GitHub" src="https://img.shields.io/github/license/TensorSpeech/TensorFlowASR?logo=apache&logoColor=green">
-        </a>
-        <img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.6-blue?logo=python">
-        <img alt="tensorflow" src="https://img.shields.io/badge/tensorflow-%3E%3D2.5.1-orange?logo=tensorflow">
-        <a href="https://pypi.org/project/TensorFlowASR/">
-          <img alt="PyPI" src="https://img.shields.io/pypi/v/TensorFlowASR?color=%234285F4&label=release&logo=pypi&logoColor=%234285F4">
-        </a>
-        </p>
-        </h1>
-        <h2 align="center">
-        <p>Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2</p>
-        </h2>
-        
-        <p align="center">
-        TensorFlowASR implements some automatic speech recognition architectures such as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These models can be converted to TFLite to reduce memory and computation for deployment :smile:
-        </p>
-        
-        ## What's New?
-        
-        - (04/17/2021) Refactor repository with new version 1.x
-        - (02/16/2021) Supported for TPU training
-        - (12/27/2020) Supported _naive_ token level timestamp, see [demo](./examples/demonstration/conformer.py) with flag `--timestamp`
-        - (12/17/2020) Supported ContextNet [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191)
-        - (12/12/2020) Add support for using masking
-        - (11/14/2020) Supported Gradient Accumulation for Training in Larger Batch Size
-        
-        ## Table of Contents
-        
-        <!-- TOC -->
-        
-        - [What's New?](#whats-new)
-        - [Table of Contents](#table-of-contents)
-        - [:yum: Supported Models](#yum-supported-models)
-          - [Baselines](#baselines)
-          - [Publications](#publications)
-        - [Installation](#installation)
-          - [Installing from source (recommended)](#installing-from-source-recommended)
-          - [Installing via PyPi](#installing-via-pypi)
-          - [Running in a container](#running-in-a-container)
-        - [Setup training and testing](#setup-training-and-testing)
-        - [TFLite Convertion](#tflite-convertion)
-        - [Features Extraction](#features-extraction)
-        - [Augmentations](#augmentations)
-        - [Training & Testing Tutorial](#training--testing-tutorial)
-        - [Corpus Sources and Pretrained Models](#corpus-sources-and-pretrained-models)
-          - [English](#english)
-          - [Vietnamese](#vietnamese)
-          - [German](#german)
-        - [References & Credits](#references--credits)
-        - [Contact](#contact)
-        
-        <!-- /TOC -->
-        
-        ## :yum: Supported Models
-        
-        ### Baselines
-        
-        - **Transducer Models** (End2end models using RNNT Loss for training, currently supported Conformer, ContextNet, Streaming Transducer)
-        - **CTCModel** (End2end models using CTC Loss for training, currently supported DeepSpeech2, Jasper)
-        
-        ### Publications
-        
-        - **Conformer Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100))
-          See [examples/conformer](./examples/conformer)
-        - **Streaming Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621))
-          See [examples/streaming_transducer](./examples/streaming_transducer)
-        - **ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
-          See [examples/contextnet](./examples/contextnet)
-        - **Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/1512.02595))
-          See [examples/deepspeech2](./examples/deepspeech2)
-        - **Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288))
-          See [examples/jasper](./examples/jasper)
-        
-        ## Installation
-        
-        For training and testing, you should use `git clone` for installing necessary packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.)
-        
-        ### Installing from source (recommended)
-        
-        ```bash
-        git clone https://github.com/TensorSpeech/TensorFlowASR.git
-        cd TensorFlowASR
-        # Tensorflow 2.x (with 2.x.x >= 2.5.1)
-        pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]"
-        ```
-        
-        For anaconda3:
-        
-        ```bash
-        conda create -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes sure conda install all dependencies for tensorflow
-        conda activate tfasr
-        pip install -U tensorflow-gpu # upgrade to latest version of tensorflow
-        git clone https://github.com/TensorSpeech/TensorFlowASR.git
-        cd TensorFlowASR
-        # Tensorflow 2.x (with 2.x.x >= 2.5.1)
-        pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]"
-        ```
-        
-        ### Installing via PyPi
-        
-        ```bash
-        # Tensorflow 2.x (with 2.x >= 2.3)
-        pip3 install -U "TensorFlowASR[tf2.x]" # or pip3 install -U "TensorFlowASR[tf2.x-gpu]"
-        ```
-        
-        
-        ### Running in a container
-        
-        ```bash
-        docker-compose up -d
-        ```
-        
-        ## Setup training and testing
-        
-        - For datasets, see [datasets](./tensorflow_asr/datasets/README.md)
-        
-        - For _training, testing and using_ **CTC Models**, run `./scripts/install_ctc_decoders.sh`
-        
-        - For _training_ **Transducer Models** with RNNT Loss in TF, make sure that [warp-transducer](https://github.com/HawkAaron/warp-transducer) **is not installed** (by simply run `pip3 uninstall warprnnt-tensorflow`) (**Recommended**)
-        
-        - For _training_ **Transducer Models** with RNNT Loss from [warp-transducer](https://github.com/HawkAaron/warp-transducer), run `export CUDA_HOME=/usr/local/cuda && ./scripts/install_rnnt_loss.sh` (**Note**: only `export CUDA_HOME` when you have CUDA)
-        
-        - For _mixed precision training_, use flag `--mxp` when running python scripts from [examples](./examples)
-        
-        - For _enabling XLA_, run `TF_XLA_FLAGS=--tf_xla_auto_jit=2 python3 $path_to_py_script`)
-        
-        - For _hiding warnings_, run `export TF_CPP_MIN_LOG_LEVEL=2` before running any examples
-        
-        ## TFLite Convertion
-        
-        After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **unicode code points**, then we can convert unicode points to string.
-        
-        1. Install `tf-nightly` using `pip install tf-nightly`
-        2. Build a model with the same architecture as the trained model _(if model has tflite argument, you must set it to True)_, then load the weights from trained model to the built model
-        3. Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function `add_featurizers`
-        4. Convert model's function to tflite as follows:
-        
-        ```python
-        func = model.make_tflite_function(**options) # options are the arguments of the function
-        concrete_func = func.get_concrete_function()
-        converter = tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
-        converter.experimental_new_converter = True
-        converter.optimizations = [tf.lite.Optimize.DEFAULT]
-        converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS,
-                                               tf.lite.OpsSet.SELECT_TF_OPS]
-        tflite_model = converter.convert()
-        ```
-        
-        5. Save the converted tflite model as follows:
-        
-        ```python
-        if not os.path.exists(os.path.dirname(tflite_path)):
-            os.makedirs(os.path.dirname(tflite_path))
-        with open(tflite_path, "wb") as tflite_out:
-            tflite_out.write(tflite_model)
-        ```
-        
-        5. Then the `.tflite` model is ready to be deployed
-        
-        ## Features Extraction
-        
-        See [features_extraction](./tensorflow_asr/featurizers/README.md)
-        
-        ## Augmentations
-        
-        See [augmentations](./tensorflow_asr/augmentations/README.md)
-        
-        ## Training & Testing Tutorial
-        
-        1. Define config YAML file, see the `config.yml` files in the [example folder](./examples) for reference (you can copy and modify values such as parameters, paths, etc.. to match your local machine configuration)
-        2. Download your corpus (a.k.a datasets) and create a script to generate `transcripts.tsv` files from your corpus (this is general format used in this project because each dataset has different format). For more detail, see [datasets](./tensorflow_asr/datasets/README.md). **Note:** Make sure your data contain only characters in your language, for example, english has `a` to `z` and `'`. **Do not use `cache` if your dataset size is not fit in the RAM**.
-        3. [Optional] Generate TFRecords to use `tf.data.TFRecordDataset` for better performance by using the script [create_tfrecords.py](./scripts/create_tfrecords.py)
-        4. Create vocabulary file (characters or subwords/wordpieces) by defining `language.characters`, using the scripts [generate_vocab_subwords.py](./scripts/generate_vocab_subwords.py) or [generate_vocab_sentencepiece.py](./scripts/generate_vocab_sentencepiece.py). There're predefined ones in [vocabularies](./vocabularies)
-        5. [Optional] Generate metadata file for your dataset by using script [generate_metadata.py](./scripts/generate_metadata.py). This metadata file contains maximum lengths calculated with your `config.yml` and total number of elements in each dataset, for static shape training and precalculated steps per epoch.
-        6. For training, see `train.py` files in the [example folder](./examples) to see the options
-        7. For testing, see `test.py` files in the [example folder](./examples) to see the options. **Note:** Testing is currently not supported for TPUs. It will print nothing other than the progress bar in the console, but it will store the predicted transcripts to the file `output.tsv` and then calculate the metrics from that file.
-        
-        **FYI**: Keras builtin training uses **infinite dataset**, which avoids the potential last partial batch.
-        
-        See [examples](./examples/) for some predefined ASR models and results
-        
-        ## Corpus Sources and Pretrained Models
-        
-        For pretrained models, go to [drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing)
-        
-        ### English
-        
-        |   **Name**   |                             **Source**                             | **Hours** |
-        | :----------: | :----------------------------------------------------------------: | :-------: |
-        | LibriSpeech  |              [LibriSpeech](http://www.openslr.org/12)              |   970h    |
-        | Common Voice | [https://commonvoice.mozilla.org](https://commonvoice.mozilla.org) |   1932h   |
-        
-        ### Vietnamese
-        
-        |                **Name**                |                                       **Source**                                       | **Hours** |
-        | :------------------------------------: | :------------------------------------------------------------------------------------: | :-------: |
-        |                 Vivos                  |          [https://ailab.hcmus.edu.vn/vivos](https://ailab.hcmus.edu.vn/vivos)          |    15h    |
-        |          InfoRe Technology 1           |  [InfoRe1 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip)   |    25h    |
-        | InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/audiobooks.zip) |   415h    |
-        
-        ### German
-        
-        |   **Name**   |                             **Source**                              | **Hours** |
-        | :----------: | :-----------------------------------------------------------------: | :-------: |
-        | Common Voice | [https://commonvoice.mozilla.org/](https://commonvoice.mozilla.org) |   750h    |
-        
-        ## References & Credits
-        
-        1. [NVIDIA OpenSeq2Seq Toolkit](https://github.com/NVIDIA/OpenSeq2Seq)
-        2. [https://github.com/noahchalifour/warp-transducer](https://github.com/noahchalifour/warp-transducer)
-        3. [Sequence Transduction with Recurrent Neural Network](https://arxiv.org/abs/1211.3711)
-        4. [End-to-End Speech Processing Toolkit in PyTorch](https://github.com/espnet/espnet)
-        5. [https://github.com/iankur/ContextNet](https://github.com/iankur/ContextNet)
-        
-        ## Contact
-        
-        Huy Le Nguyen
-        
-        Email: nlhuy.cs.16@gmail.com
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-Provides-Extra: tf2.5
-Provides-Extra: tf2.5-gpu
-Provides-Extra: tf2.6
-Provides-Extra: tf2.6-gpu
-Provides-Extra: tf2.7
-Provides-Extra: tf2.7-gpu
-Provides-Extra: tf2.8
-Provides-Extra: tf2.8-gpu
+Provides-Extra: dev
+Provides-Extra: tf2-12
+Provides-Extra: tf2-12-gpu
+Provides-Extra: tf2-13
+Provides-Extra: tf2-13-gpu
+Provides-Extra: tf2-14
+Provides-Extra: tf2-14-gpu
+Provides-Extra: tf2-15
+Provides-Extra: tf2-15-gpu
+License-File: LICENSE
+
+<h1 align="center">
+<p>TensorFlowASR :zap:</p>
+<p align="center">
+<a href="https://github.com/TensorSpeech/TensorFlowASR/blob/main/LICENSE">
+  <img alt="GitHub" src="https://img.shields.io/github/license/TensorSpeech/TensorFlowASR?logo=apache&logoColor=green">
+</a>
+<img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.6-blue?logo=python">
+<img alt="tensorflow" src="https://img.shields.io/badge/tensorflow-%3E%3D2.12.0-orange?logo=tensorflow">
+<a href="https://pypi.org/project/TensorFlowASR/">
+  <img alt="PyPI" src="https://img.shields.io/pypi/v/TensorFlowASR?color=%234285F4&label=release&logo=pypi&logoColor=%234285F4">
+</a>
+</p>
+</h1>
+<h2 align="center">
+<p>Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2</p>
+</h2>
+
+<p align="center">
+TensorFlowASR implements some automatic speech recognition architectures such as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These models can be converted to TFLite to reduce memory and computation for deployment :smile:
+</p>
+
+## What's New?
+
+## Table of Contents
+
+<!-- TOC -->
+
+- [What's New?](#whats-new)
+- [Table of Contents](#table-of-contents)
+- [:yum: Supported Models](#yum-supported-models)
+  - [Baselines](#baselines)
+  - [Publications](#publications)
+- [Installation](#installation)
+  - [Installing from source (recommended)](#installing-from-source-recommended)
+  - [Installing via PyPi](#installing-via-pypi)
+  - [Installing for development](#installing-for-development)
+  - [Install for Apple Sillicon](#install-for-apple-sillicon)
+  - [Running in a container](#running-in-a-container)
+- [Training \& Testing Tutorial](#training--testing-tutorial)
+- [Features Extraction](#features-extraction)
+- [Augmentations](#augmentations)
+- [TFLite Convertion](#tflite-convertion)
+- [Pretrained Models](#pretrained-models)
+- [Corpus Sources](#corpus-sources)
+  - [English](#english)
+  - [Vietnamese](#vietnamese)
+- [How to contribute](#how-to-contribute)
+- [References \& Credits](#references--credits)
+- [Contact](#contact)
+
+<!-- /TOC -->
+
+## :yum: Supported Models
+
+### Baselines
+
+- **Transducer Models** (End2end models using RNNT Loss for training, currently supported Conformer, ContextNet, Streaming Transducer)
+- **CTCModel** (End2end models using CTC Loss for training, currently supported DeepSpeech2, Jasper)
+
+### Publications
+
+- **Conformer Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100))
+  See [examples/conformer](./examples/conformer)
+- **ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
+  See [examples/contextnet](./examples/contextnet)
+- **RNN Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621))
+  See [examples/rnn_transducer](./examples/rnn_transducer)
+- **Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/1512.02595))
+  See [examples/deepspeech2](./examples/deepspeech2)
+- **Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288))
+  See [examples/jasper](./examples/jasper)
+
+## Installation
+
+For training and testing, you should use `git clone` for installing necessary packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.)
+
+### Installing from source (recommended)
+
+```bash
+git clone https://github.com/TensorSpeech/TensorFlowASR.git
+cd TensorFlowASR
+# Tensorflow 2.x (with 2.x.x >= 2.5.1)
+pip3 install ".[tf2.x]" # or ".[tf2.x-gpu]"
+```
+
+For anaconda3:
+
+```bash
+conda create -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes sure conda install all dependencies for tensorflow
+conda activate tfasr
+pip install -U tensorflow-gpu # upgrade to latest version of tensorflow
+git clone https://github.com/TensorSpeech/TensorFlowASR.git
+cd TensorFlowASR
+# Tensorflow 2.x (with 2.x.x >= 2.5.1)
+pip3 install ".[tf2.x]" # or ".[tf2.x-gpu]"
+```
+
+### Installing via PyPi
+
+```bash
+# Tensorflow 2.x (with 2.x >= 2.3)
+pip3 install "TensorFlowASR[tf2.x]" # or pip3 install "TensorFlowASR[tf2.x-gpu]"
+```
+
+### Installing for development
+
+```bash
+git clone https://github.com/TensorSpeech/TensorFlowASR.git
+cd TensorFlowASR
+pip3 install -e ".[dev]"
+pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine
+```
+
+### Install for Apple Sillicon
+
+Due to tensorflow-text is not built for Apple Sillicon, we need to install it with the prebuilt wheel file from [sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon](https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon)
+
+Do this after installing TensorFlowASR with tensorflow above
+
+```bash
+TF_VERSION="$(python3 -c 'import tensorflow; print(tensorflow.__version__)')" && \
+TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -d'.' -f1,2)" && \
+URL="https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon" && \
+pip3 install "${URL}/releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-cp310-cp310-macosx_11_0_arm64.whl"
+```
+
+### Running in a container
+
+```bash
+docker-compose up -d
+```
+
+
+
+## Training & Testing Tutorial
+
+- For training, please read [tutorial_training](./docs/1_tutorial_training.md)
+- For testing, please read [tutorial_testing](./docs/2_tutorial_testing.md)
+
+**FYI**: Keras builtin training uses **infinite dataset**, which avoids the potential last partial batch.
+
+See [examples](./examples/) for some predefined ASR models and results
+
+## Features Extraction
+
+See [features_extraction](./tensorflow_asr/featurizers/README.md)
+
+## Augmentations
+
+See [augmentations](./tensorflow_asr/augmentations/README.md)
+
+## TFLite Convertion
+
+After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **unicode code points**, then we can convert unicode points to string.
+
+1. Install `tf-nightly` using `pip install tf-nightly`
+2. Build a model with the same architecture as the trained model _(if model has tflite argument, you must set it to True)_, then load the weights from trained model to the built model
+3. Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function `add_featurizers`
+4. Convert model's function to tflite as follows:
+
+```python
+func = model.make_tflite_function(**options) # options are the arguments of the function
+concrete_func = func.get_concrete_function()
+converter = tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
+converter.experimental_new_converter = True
+converter.optimizations = [tf.lite.Optimize.DEFAULT]
+converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS,
+                                       tf.lite.OpsSet.SELECT_TF_OPS]
+tflite_model = converter.convert()
+```
+
+5. Save the converted tflite model as follows:
+
+```python
+if not os.path.exists(os.path.dirname(tflite_path)):
+    os.makedirs(os.path.dirname(tflite_path))
+with open(tflite_path, "wb") as tflite_out:
+    tflite_out.write(tflite_model)
+```
+
+5. Then the `.tflite` model is ready to be deployed
+
+## Pretrained Models
+
+Go to [drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing)
+
+## Corpus Sources
+
+### English
+
+| **Name**     | **Source**                                                         | **Hours** |
+| :----------- | :----------------------------------------------------------------- | :-------- |
+| LibriSpeech  | [LibriSpeech](http://www.openslr.org/12)                           | 970h      |
+| Common Voice | [https://commonvoice.mozilla.org](https://commonvoice.mozilla.org) | 1932h     |
+
+### Vietnamese
+
+| **Name**                               | **Source**                                                                             | **Hours** |
+| :------------------------------------- | :------------------------------------------------------------------------------------- | :-------- |
+| Vivos                                  | [https://ailab.hcmus.edu.vn/vivos](https://ailab.hcmus.edu.vn/vivos)                   | 15h       |
+| InfoRe Technology 1                    | [InfoRe1 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip)    | 25h       |
+| InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/audiobooks.zip) | 415h      |
+
+## How to contribute
+
+1. Fork the project
+2. [Install for development](#installing-for-development)
+3. Create a branch
+4. Make a pull request to this repo
+
+## References & Credits
+
+1. [NVIDIA OpenSeq2Seq Toolkit](https://github.com/NVIDIA/OpenSeq2Seq)
+2. [https://github.com/noahchalifour/warp-transducer](https://github.com/noahchalifour/warp-transducer)
+3. [Sequence Transduction with Recurrent Neural Network](https://arxiv.org/abs/1211.3711)
+4. [End-to-End Speech Processing Toolkit in PyTorch](https://github.com/espnet/espnet)
+5. [https://github.com/iankur/ContextNet](https://github.com/iankur/ContextNet)
+
+## Contact
+
+Huy Le Nguyen
+
+Email: nlhuy.cs.16@gmail.com
```

#### html2text {}

```diff
@@ -1,151 +1,121 @@
-Metadata-Version: 2.1 Name: TensorFlowASR Version: 1.0.3 Summary: Almost State-
+Metadata-Version: 2.1 Name: TensorFlowASR Version: 2.0.0 Summary: Almost State-
 of-the-art Automatic Speech Recognition using Tensorflow 2 Home-page: https://
 github.com/TensorSpeech/TensorFlowASR Author: Huy Le Nguyen Author-email:
-nlhuy.cs.16@gmail.com License: UNKNOWN Description:
+nlhuy.cs.16@gmail.com Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Science/Research Classifier: Operating System
+:: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: tf2-12 Provides-Extra: tf2-12-gpu Provides-
+Extra: tf2-13 Provides-Extra: tf2-13-gpu Provides-Extra: tf2-14 Provides-Extra:
+tf2-14-gpu Provides-Extra: tf2-15 Provides-Extra: tf2-15-gpu License-File:
+LICENSE
       ************ TTeennssoorrFFlloowwAASSRR ::zzaapp::_[[_GG_ii_tt_HH_uu_bb_]][[ppyytthhoonn]][[tteennssoorrffllooww]]_[[_PP_yy_PP_II_]] ************
   ********** AAllmmoosstt SSttaattee--ooff--tthhee--aarrtt AAuuttoommaattiicc SSppeeeecchh RReeccooggnniittiioonn iinn TTeennssoorrffllooww 22
                                      **********
  TensorFlowASR implements some automatic speech recognition architectures such
    as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These
     models can be converted to TFLite to reduce memory and computation for
                               deployment :smile:
-## What's New? - (04/17/2021) Refactor repository with new version 1.x - (02/
-16/2021) Supported for TPU training - (12/27/2020) Supported _naive_ token
-level timestamp, see [demo](./examples/demonstration/conformer.py) with flag `-
--timestamp` - (12/17/2020) Supported ContextNet [http://arxiv.org/abs/
-2005.03191](http://arxiv.org/abs/2005.03191) - (12/12/2020) Add support for
-using masking - (11/14/2020) Supported Gradient Accumulation for Training in
-Larger Batch Size ## Table of Contents - [What's New?](#whats-new) - [Table of
+## What's New? ## Table of Contents - [What's New?](#whats-new) - [Table of
 Contents](#table-of-contents) - [:yum: Supported Models](#yum-supported-models)
 - [Baselines](#baselines) - [Publications](#publications) - [Installation]
 (#installation) - [Installing from source (recommended)](#installing-from-
-source-recommended) - [Installing via PyPi](#installing-via-pypi) - [Running in
-a container](#running-in-a-container) - [Setup training and testing](#setup-
-training-and-testing) - [TFLite Convertion](#tflite-convertion) - [Features
-Extraction](#features-extraction) - [Augmentations](#augmentations) - [Training
-& Testing Tutorial](#training--testing-tutorial) - [Corpus Sources and
-Pretrained Models](#corpus-sources-and-pretrained-models) - [English](#english)
-- [Vietnamese](#vietnamese) - [German](#german) - [References & Credits]
-(#references--credits) - [Contact](#contact) ## :yum: Supported Models ###
-Baselines - **Transducer Models** (End2end models using RNNT Loss for training,
-currently supported Conformer, ContextNet, Streaming Transducer) - **CTCModel**
-(End2end models using CTC Loss for training, currently supported DeepSpeech2,
-Jasper) ### Publications - **Conformer Transducer** (Reference: [https://
-arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100)) See [examples/
-conformer](./examples/conformer) - **Streaming Transducer** (Reference: [https:
-//arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621)) See [examples/
-streaming_transducer](./examples/streaming_transducer) - **ContextNet**
-(Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
-See [examples/contextnet](./examples/contextnet) - **Deep Speech 2**
-(Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/
-1512.02595)) See [examples/deepspeech2](./examples/deepspeech2) - **Jasper**
-(Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/
-1904.03288)) See [examples/jasper](./examples/jasper) ## Installation For
+source-recommended) - [Installing via PyPi](#installing-via-pypi) - [Installing
+for development](#installing-for-development) - [Install for Apple Sillicon]
+(#install-for-apple-sillicon) - [Running in a container](#running-in-a-
+container) - [Training \& Testing Tutorial](#training--testing-tutorial) -
+[Features Extraction](#features-extraction) - [Augmentations](#augmentations) -
+[TFLite Convertion](#tflite-convertion) - [Pretrained Models](#pretrained-
+models) - [Corpus Sources](#corpus-sources) - [English](#english) -
+[Vietnamese](#vietnamese) - [How to contribute](#how-to-contribute) -
+[References \& Credits](#references--credits) - [Contact](#contact) ## :yum:
+Supported Models ### Baselines - **Transducer Models** (End2end models using
+RNNT Loss for training, currently supported Conformer, ContextNet, Streaming
+Transducer) - **CTCModel** (End2end models using CTC Loss for training,
+currently supported DeepSpeech2, Jasper) ### Publications - **Conformer
+Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/
+abs/2005.08100)) See [examples/conformer](./examples/conformer) -
+**ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/
+abs/2005.03191)) See [examples/contextnet](./examples/contextnet) - **RNN
+Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/
+abs/1811.06621)) See [examples/rnn_transducer](./examples/rnn_transducer) -
+**Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://
+arxiv.org/abs/1512.02595)) See [examples/deepspeech2](./examples/deepspeech2) -
+**Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/
+abs/1904.03288)) See [examples/jasper](./examples/jasper) ## Installation For
 training and testing, you should use `git clone` for installing necessary
 packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.) ### Installing
 from source (recommended) ```bash git clone https://github.com/TensorSpeech/
 TensorFlowASR.git cd TensorFlowASR # Tensorflow 2.x (with 2.x.x >= 2.5.1) pip3
-install -e ".[tf2.x]" # or ".[tf2.x-gpu]" ``` For anaconda3: ```bash conda
-create -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this
-makes sure conda install all dependencies for tensorflow conda activate tfasr
-pip install -U tensorflow-gpu # upgrade to latest version of tensorflow git
-clone https://github.com/TensorSpeech/TensorFlowASR.git cd TensorFlowASR #
-Tensorflow 2.x (with 2.x.x >= 2.5.1) pip3 install -e ".[tf2.x]" # or ".[tf2.x-
-gpu]" ``` ### Installing via PyPi ```bash # Tensorflow 2.x (with 2.x >= 2.3)
-pip3 install -U "TensorFlowASR[tf2.x]" # or pip3 install -U "TensorFlowASR
-[tf2.x-gpu]" ``` ### Running in a container ```bash docker-compose up -d ``` ##
-Setup training and testing - For datasets, see [datasets](./tensorflow_asr/
-datasets/README.md) - For _training, testing and using_ **CTC Models**, run `./
-scripts/install_ctc_decoders.sh` - For _training_ **Transducer Models** with
-RNNT Loss in TF, make sure that [warp-transducer](https://github.com/HawkAaron/
-warp-transducer) **is not installed** (by simply run `pip3 uninstall warprnnt-
-tensorflow`) (**Recommended**) - For _training_ **Transducer Models** with RNNT
-Loss from [warp-transducer](https://github.com/HawkAaron/warp-transducer), run
-`export CUDA_HOME=/usr/local/cuda && ./scripts/install_rnnt_loss.sh` (**Note**:
-only `export CUDA_HOME` when you have CUDA) - For _mixed precision training_,
-use flag `--mxp` when running python scripts from [examples](./examples) - For
-_enabling XLA_, run `TF_XLA_FLAGS=--tf_xla_auto_jit=2 python3
-$path_to_py_script`) - For _hiding warnings_, run `export
-TF_CPP_MIN_LOG_LEVEL=2` before running any examples ## TFLite Convertion After
-converting to tflite, the tflite model is like a function that transforms
-directly from an **audio signal** to **unicode code points**, then we can
-convert unicode points to string. 1. Install `tf-nightly` using `pip install
-tf-nightly` 2. Build a model with the same architecture as the trained model _
-(if model has tflite argument, you must set it to True)_, then load the weights
-from trained model to the built model 3. Load `TFSpeechFeaturizer` and
-`TextFeaturizer` to model using function `add_featurizers` 4. Convert model's
-function to tflite as follows: ```python func = model.make_tflite_function
-(**options) # options are the arguments of the function concrete_func =
-func.get_concrete_function() converter =
+install ".[tf2.x]" # or ".[tf2.x-gpu]" ``` For anaconda3: ```bash conda create
+-y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes
+sure conda install all dependencies for tensorflow conda activate tfasr pip
+install -U tensorflow-gpu # upgrade to latest version of tensorflow git clone
+https://github.com/TensorSpeech/TensorFlowASR.git cd TensorFlowASR # Tensorflow
+2.x (with 2.x.x >= 2.5.1) pip3 install ".[tf2.x]" # or ".[tf2.x-gpu]" ``` ###
+Installing via PyPi ```bash # Tensorflow 2.x (with 2.x >= 2.3) pip3 install
+"TensorFlowASR[tf2.x]" # or pip3 install "TensorFlowASR[tf2.x-gpu]" ``` ###
+Installing for development ```bash git clone https://github.com/TensorSpeech/
+TensorFlowASR.git cd TensorFlowASR pip3 install -e ".[dev]" pip3 install -e ".
+[tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine ``` ###
+Install for Apple Sillicon Due to tensorflow-text is not built for Apple
+Sillicon, we need to install it with the prebuilt wheel file from
+[sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon]
+(https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-
+Apple-Silicon) Do this after installing TensorFlowASR with tensorflow above
+```bash TF_VERSION="$(python3 -c 'import tensorflow; print
+(tensorflow.__version__)')" && \ TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -
+d'.' -f1,2)" && \ URL="https://github.com/sun1638650145/Libraries-and-
+Extensions-for-TensorFlow-for-Apple-Silicon" && \ pip3 install "${URL}/
+releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-
+cp310-cp310-macosx_11_0_arm64.whl" ``` ### Running in a container ```bash
+docker-compose up -d ``` ## Training & Testing Tutorial - For training, please
+read [tutorial_training](./docs/1_tutorial_training.md) - For testing, please
+read [tutorial_testing](./docs/2_tutorial_testing.md) **FYI**: Keras builtin
+training uses **infinite dataset**, which avoids the potential last partial
+batch. See [examples](./examples/) for some predefined ASR models and results
+## Features Extraction See [features_extraction](./tensorflow_asr/featurizers/
+README.md) ## Augmentations See [augmentations](./tensorflow_asr/augmentations/
+README.md) ## TFLite Convertion After converting to tflite, the tflite model is
+like a function that transforms directly from an **audio signal** to **unicode
+code points**, then we can convert unicode points to string. 1. Install `tf-
+nightly` using `pip install tf-nightly` 2. Build a model with the same
+architecture as the trained model _(if model has tflite argument, you must set
+it to True)_, then load the weights from trained model to the built model 3.
+Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function
+`add_featurizers` 4. Convert model's function to tflite as follows: ```python
+func = model.make_tflite_function(**options) # options are the arguments of the
+function concrete_func = func.get_concrete_function() converter =
 tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
 converter.experimental_new_converter = True converter.optimizations =
 [tf.lite.Optimize.DEFAULT] converter.target_spec.supported_ops =
 [tf.lite.OpsSet.TFLITE_BUILTINS, tf.lite.OpsSet.SELECT_TF_OPS] tflite_model =
 converter.convert() ``` 5. Save the converted tflite model as follows:
 ```python if not os.path.exists(os.path.dirname(tflite_path)): os.makedirs
 (os.path.dirname(tflite_path)) with open(tflite_path, "wb") as tflite_out:
 tflite_out.write(tflite_model) ``` 5. Then the `.tflite` model is ready to be
-deployed ## Features Extraction See [features_extraction](./tensorflow_asr/
-featurizers/README.md) ## Augmentations See [augmentations](./tensorflow_asr/
-augmentations/README.md) ## Training & Testing Tutorial 1. Define config YAML
-file, see the `config.yml` files in the [example folder](./examples) for
-reference (you can copy and modify values such as parameters, paths, etc.. to
-match your local machine configuration) 2. Download your corpus (a.k.a
-datasets) and create a script to generate `transcripts.tsv` files from your
-corpus (this is general format used in this project because each dataset has
-different format). For more detail, see [datasets](./tensorflow_asr/datasets/
-README.md). **Note:** Make sure your data contain only characters in your
-language, for example, english has `a` to `z` and `'`. **Do not use `cache` if
-your dataset size is not fit in the RAM**. 3. [Optional] Generate TFRecords to
-use `tf.data.TFRecordDataset` for better performance by using the script
-[create_tfrecords.py](./scripts/create_tfrecords.py) 4. Create vocabulary file
-(characters or subwords/wordpieces) by defining `language.characters`, using
-the scripts [generate_vocab_subwords.py](./scripts/generate_vocab_subwords.py)
-or [generate_vocab_sentencepiece.py](./scripts/
-generate_vocab_sentencepiece.py). There're predefined ones in [vocabularies](./
-vocabularies) 5. [Optional] Generate metadata file for your dataset by using
-script [generate_metadata.py](./scripts/generate_metadata.py). This metadata
-file contains maximum lengths calculated with your `config.yml` and total
-number of elements in each dataset, for static shape training and precalculated
-steps per epoch. 6. For training, see `train.py` files in the [example folder]
-(./examples) to see the options 7. For testing, see `test.py` files in the
-[example folder](./examples) to see the options. **Note:** Testing is currently
-not supported for TPUs. It will print nothing other than the progress bar in
-the console, but it will store the predicted transcripts to the file
-`output.tsv` and then calculate the metrics from that file. **FYI**: Keras
-builtin training uses **infinite dataset**, which avoids the potential last
-partial batch. See [examples](./examples/) for some predefined ASR models and
-results ## Corpus Sources and Pretrained Models For pretrained models, go to
-[drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-
-yR28C5FW3LqzZxtLOQfl?usp=sharing) ### English | **Name** | **Source** |
-**Hours** | | :----------: | :-------------------------------------------------
----------------: | :-------: | | LibriSpeech | [LibriSpeech](http://
-www.openslr.org/12) | 970h | | Common Voice | [https://commonvoice.mozilla.org]
-(https://commonvoice.mozilla.org) | 1932h | ### Vietnamese | **Name** |
-**Source** | **Hours** | | :------------------------------------: | :----------
---------------------------------------------------------------------------: | :
--------: | | Vivos | [https://ailab.hcmus.edu.vn/vivos](https://
-ailab.hcmus.edu.vn/vivos) | 15h | | InfoRe Technology 1 | [InfoRe1 (passwd:
-BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip) | 25h | |
-InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd:
+deployed ## Pretrained Models Go to [drive](https://drive.google.com/drive/
+folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing) ## Corpus Sources ###
+English | **Name** | **Source** | **Hours** | | :----------- | :---------------
+-------------------------------------------------- | :-------- | | LibriSpeech
+| [LibriSpeech](http://www.openslr.org/12) | 970h | | Common Voice | [https://
+commonvoice.mozilla.org](https://commonvoice.mozilla.org) | 1932h | ###
+Vietnamese | **Name** | **Source** | **Hours** | | :---------------------------
+---------- | :-----------------------------------------------------------------
+-------------------- | :-------- | | Vivos | [https://ailab.hcmus.edu.vn/vivos]
+(https://ailab.hcmus.edu.vn/vivos) | 15h | | InfoRe Technology 1 | [InfoRe1
+(passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip) |
+25h | | InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd:
 BroughtToYouByInfoRe)](https://files.huylenguyen.com/audiobooks.zip) | 415h |
-### German | **Name** | **Source** | **Hours** | | :----------: | :------------
------------------------------------------------------: | :-------: | | Common
-Voice | [https://commonvoice.mozilla.org/](https://commonvoice.mozilla.org) |
-750h | ## References & Credits 1. [NVIDIA OpenSeq2Seq Toolkit](https://
+## How to contribute 1. Fork the project 2. [Install for development]
+(#installing-for-development) 3. Create a branch 4. Make a pull request to this
+repo ## References & Credits 1. [NVIDIA OpenSeq2Seq Toolkit](https://
 github.com/NVIDIA/OpenSeq2Seq) 2. [https://github.com/noahchalifour/warp-
 transducer](https://github.com/noahchalifour/warp-transducer) 3. [Sequence
 Transduction with Recurrent Neural Network](https://arxiv.org/abs/1211.3711) 4.
 [End-to-End Speech Processing Toolkit in PyTorch](https://github.com/espnet/
 espnet) 5. [https://github.com/iankur/ContextNet](https://github.com/iankur/
-ContextNet) ## Contact Huy Le Nguyen Email: nlhuy.cs.16@gmail.com Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Intended Audience :: Science/Research Classifier: Operating System :: POSIX ::
-Linux Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown Provides-
-Extra: tf2.5 Provides-Extra: tf2.5-gpu Provides-Extra: tf2.6 Provides-Extra:
-tf2.6-gpu Provides-Extra: tf2.7 Provides-Extra: tf2.7-gpu Provides-Extra: tf2.8
-Provides-Extra: tf2.8-gpu
+ContextNet) ## Contact Huy Le Nguyen Email: nlhuy.cs.16@gmail.com
```

### Comparing `TensorFlowASR-1.0.3/README.md` & `TensorFlowASR-2.0.0/TensorFlowASR.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,43 @@
+Metadata-Version: 2.1
+Name: TensorFlowASR
+Version: 2.0.0
+Summary: Almost State-of-the-art Automatic Speech Recognition using Tensorflow 2
+Home-page: https://github.com/TensorSpeech/TensorFlowASR
+Author: Huy Le Nguyen
+Author-email: nlhuy.cs.16@gmail.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tf2-12
+Provides-Extra: tf2-12-gpu
+Provides-Extra: tf2-13
+Provides-Extra: tf2-13-gpu
+Provides-Extra: tf2-14
+Provides-Extra: tf2-14-gpu
+Provides-Extra: tf2-15
+Provides-Extra: tf2-15-gpu
+License-File: LICENSE
+
 <h1 align="center">
 <p>TensorFlowASR :zap:</p>
 <p align="center">
 <a href="https://github.com/TensorSpeech/TensorFlowASR/blob/main/LICENSE">
   <img alt="GitHub" src="https://img.shields.io/github/license/TensorSpeech/TensorFlowASR?logo=apache&logoColor=green">
 </a>
 <img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.6-blue?logo=python">
-<img alt="tensorflow" src="https://img.shields.io/badge/tensorflow-%3E%3D2.5.1-orange?logo=tensorflow">
+<img alt="tensorflow" src="https://img.shields.io/badge/tensorflow-%3E%3D2.12.0-orange?logo=tensorflow">
 <a href="https://pypi.org/project/TensorFlowASR/">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/TensorFlowASR?color=%234285F4&label=release&logo=pypi&logoColor=%234285F4">
 </a>
 </p>
 </h1>
 <h2 align="center">
 <p>Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2</p>
@@ -17,44 +45,39 @@
 
 <p align="center">
 TensorFlowASR implements some automatic speech recognition architectures such as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These models can be converted to TFLite to reduce memory and computation for deployment :smile:
 </p>
 
 ## What's New?
 
-- (04/17/2021) Refactor repository with new version 1.x
-- (02/16/2021) Supported for TPU training
-- (12/27/2020) Supported _naive_ token level timestamp, see [demo](./examples/demonstration/conformer.py) with flag `--timestamp`
-- (12/17/2020) Supported ContextNet [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191)
-- (12/12/2020) Add support for using masking
-- (11/14/2020) Supported Gradient Accumulation for Training in Larger Batch Size
-
 ## Table of Contents
 
 <!-- TOC -->
 
 - [What's New?](#whats-new)
 - [Table of Contents](#table-of-contents)
 - [:yum: Supported Models](#yum-supported-models)
   - [Baselines](#baselines)
   - [Publications](#publications)
 - [Installation](#installation)
   - [Installing from source (recommended)](#installing-from-source-recommended)
   - [Installing via PyPi](#installing-via-pypi)
+  - [Installing for development](#installing-for-development)
+  - [Install for Apple Sillicon](#install-for-apple-sillicon)
   - [Running in a container](#running-in-a-container)
-- [Setup training and testing](#setup-training-and-testing)
-- [TFLite Convertion](#tflite-convertion)
+- [Training \& Testing Tutorial](#training--testing-tutorial)
 - [Features Extraction](#features-extraction)
 - [Augmentations](#augmentations)
-- [Training & Testing Tutorial](#training--testing-tutorial)
-- [Corpus Sources and Pretrained Models](#corpus-sources-and-pretrained-models)
+- [TFLite Convertion](#tflite-convertion)
+- [Pretrained Models](#pretrained-models)
+- [Corpus Sources](#corpus-sources)
   - [English](#english)
   - [Vietnamese](#vietnamese)
-  - [German](#german)
-- [References & Credits](#references--credits)
+- [How to contribute](#how-to-contribute)
+- [References \& Credits](#references--credits)
 - [Contact](#contact)
 
 <!-- /TOC -->
 
 ## :yum: Supported Models
 
 ### Baselines
@@ -62,18 +85,18 @@
 - **Transducer Models** (End2end models using RNNT Loss for training, currently supported Conformer, ContextNet, Streaming Transducer)
 - **CTCModel** (End2end models using CTC Loss for training, currently supported DeepSpeech2, Jasper)
 
 ### Publications
 
 - **Conformer Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100))
   See [examples/conformer](./examples/conformer)
-- **Streaming Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621))
-  See [examples/streaming_transducer](./examples/streaming_transducer)
 - **ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
   See [examples/contextnet](./examples/contextnet)
+- **RNN Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621))
+  See [examples/rnn_transducer](./examples/rnn_transducer)
 - **Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/1512.02595))
   See [examples/deepspeech2](./examples/deepspeech2)
 - **Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288))
   See [examples/jasper](./examples/jasper)
 
 ## Installation
 
@@ -81,58 +104,82 @@
 
 ### Installing from source (recommended)
 
 ```bash
 git clone https://github.com/TensorSpeech/TensorFlowASR.git
 cd TensorFlowASR
 # Tensorflow 2.x (with 2.x.x >= 2.5.1)
-pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]"
+pip3 install ".[tf2.x]" # or ".[tf2.x-gpu]"
 ```
 
 For anaconda3:
 
 ```bash
 conda create -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes sure conda install all dependencies for tensorflow
 conda activate tfasr
 pip install -U tensorflow-gpu # upgrade to latest version of tensorflow
 git clone https://github.com/TensorSpeech/TensorFlowASR.git
 cd TensorFlowASR
 # Tensorflow 2.x (with 2.x.x >= 2.5.1)
-pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]"
+pip3 install ".[tf2.x]" # or ".[tf2.x-gpu]"
 ```
 
 ### Installing via PyPi
 
 ```bash
 # Tensorflow 2.x (with 2.x >= 2.3)
-pip3 install -U "TensorFlowASR[tf2.x]" # or pip3 install -U "TensorFlowASR[tf2.x-gpu]"
+pip3 install "TensorFlowASR[tf2.x]" # or pip3 install "TensorFlowASR[tf2.x-gpu]"
+```
+
+### Installing for development
+
+```bash
+git clone https://github.com/TensorSpeech/TensorFlowASR.git
+cd TensorFlowASR
+pip3 install -e ".[dev]"
+pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine
 ```
 
+### Install for Apple Sillicon
+
+Due to tensorflow-text is not built for Apple Sillicon, we need to install it with the prebuilt wheel file from [sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon](https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon)
+
+Do this after installing TensorFlowASR with tensorflow above
+
+```bash
+TF_VERSION="$(python3 -c 'import tensorflow; print(tensorflow.__version__)')" && \
+TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -d'.' -f1,2)" && \
+URL="https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon" && \
+pip3 install "${URL}/releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-cp310-cp310-macosx_11_0_arm64.whl"
+```
 
 ### Running in a container
 
 ```bash
 docker-compose up -d
 ```
 
-## Setup training and testing
 
-- For datasets, see [datasets](./tensorflow_asr/datasets/README.md)
 
-- For _training, testing and using_ **CTC Models**, run `./scripts/install_ctc_decoders.sh`
+## Training & Testing Tutorial
+
+- For training, please read [tutorial_training](./docs/1_tutorial_training.md)
+- For testing, please read [tutorial_testing](./docs/2_tutorial_testing.md)
+
+**FYI**: Keras builtin training uses **infinite dataset**, which avoids the potential last partial batch.
 
-- For _training_ **Transducer Models** with RNNT Loss in TF, make sure that [warp-transducer](https://github.com/HawkAaron/warp-transducer) **is not installed** (by simply run `pip3 uninstall warprnnt-tensorflow`) (**Recommended**)
+See [examples](./examples/) for some predefined ASR models and results
 
-- For _training_ **Transducer Models** with RNNT Loss from [warp-transducer](https://github.com/HawkAaron/warp-transducer), run `export CUDA_HOME=/usr/local/cuda && ./scripts/install_rnnt_loss.sh` (**Note**: only `export CUDA_HOME` when you have CUDA)
+## Features Extraction
 
-- For _mixed precision training_, use flag `--mxp` when running python scripts from [examples](./examples)
+See [features_extraction](./tensorflow_asr/featurizers/README.md)
 
-- For _enabling XLA_, run `TF_XLA_FLAGS=--tf_xla_auto_jit=2 python3 $path_to_py_script`)
+## Augmentations
 
-- For _hiding warnings_, run `export TF_CPP_MIN_LOG_LEVEL=2` before running any examples
+See [augmentations](./tensorflow_asr/augmentations/README.md)
 
 ## TFLite Convertion
 
 After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **unicode code points**, then we can convert unicode points to string.
 
 1. Install `tf-nightly` using `pip install tf-nightly`
 2. Build a model with the same architecture as the trained model _(if model has tflite argument, you must set it to True)_, then load the weights from trained model to the built model
@@ -157,60 +204,41 @@
     os.makedirs(os.path.dirname(tflite_path))
 with open(tflite_path, "wb") as tflite_out:
     tflite_out.write(tflite_model)
 ```
 
 5. Then the `.tflite` model is ready to be deployed
 
-## Features Extraction
-
-See [features_extraction](./tensorflow_asr/featurizers/README.md)
-
-## Augmentations
-
-See [augmentations](./tensorflow_asr/augmentations/README.md)
-
-## Training & Testing Tutorial
-
-1. Define config YAML file, see the `config.yml` files in the [example folder](./examples) for reference (you can copy and modify values such as parameters, paths, etc.. to match your local machine configuration)
-2. Download your corpus (a.k.a datasets) and create a script to generate `transcripts.tsv` files from your corpus (this is general format used in this project because each dataset has different format). For more detail, see [datasets](./tensorflow_asr/datasets/README.md). **Note:** Make sure your data contain only characters in your language, for example, english has `a` to `z` and `'`. **Do not use `cache` if your dataset size is not fit in the RAM**.
-3. [Optional] Generate TFRecords to use `tf.data.TFRecordDataset` for better performance by using the script [create_tfrecords.py](./scripts/create_tfrecords.py)
-4. Create vocabulary file (characters or subwords/wordpieces) by defining `language.characters`, using the scripts [generate_vocab_subwords.py](./scripts/generate_vocab_subwords.py) or [generate_vocab_sentencepiece.py](./scripts/generate_vocab_sentencepiece.py). There're predefined ones in [vocabularies](./vocabularies)
-5. [Optional] Generate metadata file for your dataset by using script [generate_metadata.py](./scripts/generate_metadata.py). This metadata file contains maximum lengths calculated with your `config.yml` and total number of elements in each dataset, for static shape training and precalculated steps per epoch.
-6. For training, see `train.py` files in the [example folder](./examples) to see the options
-7. For testing, see `test.py` files in the [example folder](./examples) to see the options. **Note:** Testing is currently not supported for TPUs. It will print nothing other than the progress bar in the console, but it will store the predicted transcripts to the file `output.tsv` and then calculate the metrics from that file.
-
-**FYI**: Keras builtin training uses **infinite dataset**, which avoids the potential last partial batch.
-
-See [examples](./examples/) for some predefined ASR models and results
+## Pretrained Models
 
-## Corpus Sources and Pretrained Models
+Go to [drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing)
 
-For pretrained models, go to [drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing)
+## Corpus Sources
 
 ### English
 
-|   **Name**   |                             **Source**                             | **Hours** |
-| :----------: | :----------------------------------------------------------------: | :-------: |
-| LibriSpeech  |              [LibriSpeech](http://www.openslr.org/12)              |   970h    |
-| Common Voice | [https://commonvoice.mozilla.org](https://commonvoice.mozilla.org) |   1932h   |
+| **Name**     | **Source**                                                         | **Hours** |
+| :----------- | :----------------------------------------------------------------- | :-------- |
+| LibriSpeech  | [LibriSpeech](http://www.openslr.org/12)                           | 970h      |
+| Common Voice | [https://commonvoice.mozilla.org](https://commonvoice.mozilla.org) | 1932h     |
 
 ### Vietnamese
 
-|                **Name**                |                                       **Source**                                       | **Hours** |
-| :------------------------------------: | :------------------------------------------------------------------------------------: | :-------: |
-|                 Vivos                  |          [https://ailab.hcmus.edu.vn/vivos](https://ailab.hcmus.edu.vn/vivos)          |    15h    |
-|          InfoRe Technology 1           |  [InfoRe1 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip)   |    25h    |
-| InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/audiobooks.zip) |   415h    |
-
-### German
-
-|   **Name**   |                             **Source**                              | **Hours** |
-| :----------: | :-----------------------------------------------------------------: | :-------: |
-| Common Voice | [https://commonvoice.mozilla.org/](https://commonvoice.mozilla.org) |   750h    |
+| **Name**                               | **Source**                                                                             | **Hours** |
+| :------------------------------------- | :------------------------------------------------------------------------------------- | :-------- |
+| Vivos                                  | [https://ailab.hcmus.edu.vn/vivos](https://ailab.hcmus.edu.vn/vivos)                   | 15h       |
+| InfoRe Technology 1                    | [InfoRe1 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip)    | 25h       |
+| InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/audiobooks.zip) | 415h      |
+
+## How to contribute
+
+1. Fork the project
+2. [Install for development](#installing-for-development)
+3. Create a branch
+4. Make a pull request to this repo
 
 ## References & Credits
 
 1. [NVIDIA OpenSeq2Seq Toolkit](https://github.com/NVIDIA/OpenSeq2Seq)
 2. [https://github.com/noahchalifour/warp-transducer](https://github.com/noahchalifour/warp-transducer)
 3. [Sequence Transduction with Recurrent Neural Network](https://arxiv.org/abs/1211.3711)
 4. [End-to-End Speech Processing Toolkit in PyTorch](https://github.com/espnet/espnet)
```

#### html2text {}

```diff
@@ -1,137 +1,121 @@
+Metadata-Version: 2.1 Name: TensorFlowASR Version: 2.0.0 Summary: Almost State-
+of-the-art Automatic Speech Recognition using Tensorflow 2 Home-page: https://
+github.com/TensorSpeech/TensorFlowASR Author: Huy Le Nguyen Author-email:
+nlhuy.cs.16@gmail.com Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Science/Research Classifier: Operating System
+:: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: tf2-12 Provides-Extra: tf2-12-gpu Provides-
+Extra: tf2-13 Provides-Extra: tf2-13-gpu Provides-Extra: tf2-14 Provides-Extra:
+tf2-14-gpu Provides-Extra: tf2-15 Provides-Extra: tf2-15-gpu License-File:
+LICENSE
       ************ TTeennssoorrFFlloowwAASSRR ::zzaapp::_[[_GG_ii_tt_HH_uu_bb_]][[ppyytthhoonn]][[tteennssoorrffllooww]]_[[_PP_yy_PP_II_]] ************
   ********** AAllmmoosstt SSttaattee--ooff--tthhee--aarrtt AAuuttoommaattiicc SSppeeeecchh RReeccooggnniittiioonn iinn TTeennssoorrffllooww 22
                                      **********
  TensorFlowASR implements some automatic speech recognition architectures such
    as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These
     models can be converted to TFLite to reduce memory and computation for
                               deployment :smile:
-## What's New? - (04/17/2021) Refactor repository with new version 1.x - (02/
-16/2021) Supported for TPU training - (12/27/2020) Supported _naive_ token
-level timestamp, see [demo](./examples/demonstration/conformer.py) with flag `-
--timestamp` - (12/17/2020) Supported ContextNet [http://arxiv.org/abs/
-2005.03191](http://arxiv.org/abs/2005.03191) - (12/12/2020) Add support for
-using masking - (11/14/2020) Supported Gradient Accumulation for Training in
-Larger Batch Size ## Table of Contents - [What's New?](#whats-new) - [Table of
+## What's New? ## Table of Contents - [What's New?](#whats-new) - [Table of
 Contents](#table-of-contents) - [:yum: Supported Models](#yum-supported-models)
 - [Baselines](#baselines) - [Publications](#publications) - [Installation]
 (#installation) - [Installing from source (recommended)](#installing-from-
-source-recommended) - [Installing via PyPi](#installing-via-pypi) - [Running in
-a container](#running-in-a-container) - [Setup training and testing](#setup-
-training-and-testing) - [TFLite Convertion](#tflite-convertion) - [Features
-Extraction](#features-extraction) - [Augmentations](#augmentations) - [Training
-& Testing Tutorial](#training--testing-tutorial) - [Corpus Sources and
-Pretrained Models](#corpus-sources-and-pretrained-models) - [English](#english)
-- [Vietnamese](#vietnamese) - [German](#german) - [References & Credits]
-(#references--credits) - [Contact](#contact) ## :yum: Supported Models ###
-Baselines - **Transducer Models** (End2end models using RNNT Loss for training,
-currently supported Conformer, ContextNet, Streaming Transducer) - **CTCModel**
-(End2end models using CTC Loss for training, currently supported DeepSpeech2,
-Jasper) ### Publications - **Conformer Transducer** (Reference: [https://
-arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100)) See [examples/
-conformer](./examples/conformer) - **Streaming Transducer** (Reference: [https:
-//arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621)) See [examples/
-streaming_transducer](./examples/streaming_transducer) - **ContextNet**
-(Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
-See [examples/contextnet](./examples/contextnet) - **Deep Speech 2**
-(Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/
-1512.02595)) See [examples/deepspeech2](./examples/deepspeech2) - **Jasper**
-(Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/
-1904.03288)) See [examples/jasper](./examples/jasper) ## Installation For
+source-recommended) - [Installing via PyPi](#installing-via-pypi) - [Installing
+for development](#installing-for-development) - [Install for Apple Sillicon]
+(#install-for-apple-sillicon) - [Running in a container](#running-in-a-
+container) - [Training \& Testing Tutorial](#training--testing-tutorial) -
+[Features Extraction](#features-extraction) - [Augmentations](#augmentations) -
+[TFLite Convertion](#tflite-convertion) - [Pretrained Models](#pretrained-
+models) - [Corpus Sources](#corpus-sources) - [English](#english) -
+[Vietnamese](#vietnamese) - [How to contribute](#how-to-contribute) -
+[References \& Credits](#references--credits) - [Contact](#contact) ## :yum:
+Supported Models ### Baselines - **Transducer Models** (End2end models using
+RNNT Loss for training, currently supported Conformer, ContextNet, Streaming
+Transducer) - **CTCModel** (End2end models using CTC Loss for training,
+currently supported DeepSpeech2, Jasper) ### Publications - **Conformer
+Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/
+abs/2005.08100)) See [examples/conformer](./examples/conformer) -
+**ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/
+abs/2005.03191)) See [examples/contextnet](./examples/contextnet) - **RNN
+Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/
+abs/1811.06621)) See [examples/rnn_transducer](./examples/rnn_transducer) -
+**Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://
+arxiv.org/abs/1512.02595)) See [examples/deepspeech2](./examples/deepspeech2) -
+**Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/
+abs/1904.03288)) See [examples/jasper](./examples/jasper) ## Installation For
 training and testing, you should use `git clone` for installing necessary
 packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.) ### Installing
 from source (recommended) ```bash git clone https://github.com/TensorSpeech/
 TensorFlowASR.git cd TensorFlowASR # Tensorflow 2.x (with 2.x.x >= 2.5.1) pip3
-install -e ".[tf2.x]" # or ".[tf2.x-gpu]" ``` For anaconda3: ```bash conda
-create -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this
-makes sure conda install all dependencies for tensorflow conda activate tfasr
-pip install -U tensorflow-gpu # upgrade to latest version of tensorflow git
-clone https://github.com/TensorSpeech/TensorFlowASR.git cd TensorFlowASR #
-Tensorflow 2.x (with 2.x.x >= 2.5.1) pip3 install -e ".[tf2.x]" # or ".[tf2.x-
-gpu]" ``` ### Installing via PyPi ```bash # Tensorflow 2.x (with 2.x >= 2.3)
-pip3 install -U "TensorFlowASR[tf2.x]" # or pip3 install -U "TensorFlowASR
-[tf2.x-gpu]" ``` ### Running in a container ```bash docker-compose up -d ``` ##
-Setup training and testing - For datasets, see [datasets](./tensorflow_asr/
-datasets/README.md) - For _training, testing and using_ **CTC Models**, run `./
-scripts/install_ctc_decoders.sh` - For _training_ **Transducer Models** with
-RNNT Loss in TF, make sure that [warp-transducer](https://github.com/HawkAaron/
-warp-transducer) **is not installed** (by simply run `pip3 uninstall warprnnt-
-tensorflow`) (**Recommended**) - For _training_ **Transducer Models** with RNNT
-Loss from [warp-transducer](https://github.com/HawkAaron/warp-transducer), run
-`export CUDA_HOME=/usr/local/cuda && ./scripts/install_rnnt_loss.sh` (**Note**:
-only `export CUDA_HOME` when you have CUDA) - For _mixed precision training_,
-use flag `--mxp` when running python scripts from [examples](./examples) - For
-_enabling XLA_, run `TF_XLA_FLAGS=--tf_xla_auto_jit=2 python3
-$path_to_py_script`) - For _hiding warnings_, run `export
-TF_CPP_MIN_LOG_LEVEL=2` before running any examples ## TFLite Convertion After
-converting to tflite, the tflite model is like a function that transforms
-directly from an **audio signal** to **unicode code points**, then we can
-convert unicode points to string. 1. Install `tf-nightly` using `pip install
-tf-nightly` 2. Build a model with the same architecture as the trained model _
-(if model has tflite argument, you must set it to True)_, then load the weights
-from trained model to the built model 3. Load `TFSpeechFeaturizer` and
-`TextFeaturizer` to model using function `add_featurizers` 4. Convert model's
-function to tflite as follows: ```python func = model.make_tflite_function
-(**options) # options are the arguments of the function concrete_func =
-func.get_concrete_function() converter =
+install ".[tf2.x]" # or ".[tf2.x-gpu]" ``` For anaconda3: ```bash conda create
+-y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes
+sure conda install all dependencies for tensorflow conda activate tfasr pip
+install -U tensorflow-gpu # upgrade to latest version of tensorflow git clone
+https://github.com/TensorSpeech/TensorFlowASR.git cd TensorFlowASR # Tensorflow
+2.x (with 2.x.x >= 2.5.1) pip3 install ".[tf2.x]" # or ".[tf2.x-gpu]" ``` ###
+Installing via PyPi ```bash # Tensorflow 2.x (with 2.x >= 2.3) pip3 install
+"TensorFlowASR[tf2.x]" # or pip3 install "TensorFlowASR[tf2.x-gpu]" ``` ###
+Installing for development ```bash git clone https://github.com/TensorSpeech/
+TensorFlowASR.git cd TensorFlowASR pip3 install -e ".[dev]" pip3 install -e ".
+[tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine ``` ###
+Install for Apple Sillicon Due to tensorflow-text is not built for Apple
+Sillicon, we need to install it with the prebuilt wheel file from
+[sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon]
+(https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-
+Apple-Silicon) Do this after installing TensorFlowASR with tensorflow above
+```bash TF_VERSION="$(python3 -c 'import tensorflow; print
+(tensorflow.__version__)')" && \ TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -
+d'.' -f1,2)" && \ URL="https://github.com/sun1638650145/Libraries-and-
+Extensions-for-TensorFlow-for-Apple-Silicon" && \ pip3 install "${URL}/
+releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-
+cp310-cp310-macosx_11_0_arm64.whl" ``` ### Running in a container ```bash
+docker-compose up -d ``` ## Training & Testing Tutorial - For training, please
+read [tutorial_training](./docs/1_tutorial_training.md) - For testing, please
+read [tutorial_testing](./docs/2_tutorial_testing.md) **FYI**: Keras builtin
+training uses **infinite dataset**, which avoids the potential last partial
+batch. See [examples](./examples/) for some predefined ASR models and results
+## Features Extraction See [features_extraction](./tensorflow_asr/featurizers/
+README.md) ## Augmentations See [augmentations](./tensorflow_asr/augmentations/
+README.md) ## TFLite Convertion After converting to tflite, the tflite model is
+like a function that transforms directly from an **audio signal** to **unicode
+code points**, then we can convert unicode points to string. 1. Install `tf-
+nightly` using `pip install tf-nightly` 2. Build a model with the same
+architecture as the trained model _(if model has tflite argument, you must set
+it to True)_, then load the weights from trained model to the built model 3.
+Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function
+`add_featurizers` 4. Convert model's function to tflite as follows: ```python
+func = model.make_tflite_function(**options) # options are the arguments of the
+function concrete_func = func.get_concrete_function() converter =
 tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
 converter.experimental_new_converter = True converter.optimizations =
 [tf.lite.Optimize.DEFAULT] converter.target_spec.supported_ops =
 [tf.lite.OpsSet.TFLITE_BUILTINS, tf.lite.OpsSet.SELECT_TF_OPS] tflite_model =
 converter.convert() ``` 5. Save the converted tflite model as follows:
 ```python if not os.path.exists(os.path.dirname(tflite_path)): os.makedirs
 (os.path.dirname(tflite_path)) with open(tflite_path, "wb") as tflite_out:
 tflite_out.write(tflite_model) ``` 5. Then the `.tflite` model is ready to be
-deployed ## Features Extraction See [features_extraction](./tensorflow_asr/
-featurizers/README.md) ## Augmentations See [augmentations](./tensorflow_asr/
-augmentations/README.md) ## Training & Testing Tutorial 1. Define config YAML
-file, see the `config.yml` files in the [example folder](./examples) for
-reference (you can copy and modify values such as parameters, paths, etc.. to
-match your local machine configuration) 2. Download your corpus (a.k.a
-datasets) and create a script to generate `transcripts.tsv` files from your
-corpus (this is general format used in this project because each dataset has
-different format). For more detail, see [datasets](./tensorflow_asr/datasets/
-README.md). **Note:** Make sure your data contain only characters in your
-language, for example, english has `a` to `z` and `'`. **Do not use `cache` if
-your dataset size is not fit in the RAM**. 3. [Optional] Generate TFRecords to
-use `tf.data.TFRecordDataset` for better performance by using the script
-[create_tfrecords.py](./scripts/create_tfrecords.py) 4. Create vocabulary file
-(characters or subwords/wordpieces) by defining `language.characters`, using
-the scripts [generate_vocab_subwords.py](./scripts/generate_vocab_subwords.py)
-or [generate_vocab_sentencepiece.py](./scripts/
-generate_vocab_sentencepiece.py). There're predefined ones in [vocabularies](./
-vocabularies) 5. [Optional] Generate metadata file for your dataset by using
-script [generate_metadata.py](./scripts/generate_metadata.py). This metadata
-file contains maximum lengths calculated with your `config.yml` and total
-number of elements in each dataset, for static shape training and precalculated
-steps per epoch. 6. For training, see `train.py` files in the [example folder]
-(./examples) to see the options 7. For testing, see `test.py` files in the
-[example folder](./examples) to see the options. **Note:** Testing is currently
-not supported for TPUs. It will print nothing other than the progress bar in
-the console, but it will store the predicted transcripts to the file
-`output.tsv` and then calculate the metrics from that file. **FYI**: Keras
-builtin training uses **infinite dataset**, which avoids the potential last
-partial batch. See [examples](./examples/) for some predefined ASR models and
-results ## Corpus Sources and Pretrained Models For pretrained models, go to
-[drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-
-yR28C5FW3LqzZxtLOQfl?usp=sharing) ### English | **Name** | **Source** |
-**Hours** | | :----------: | :-------------------------------------------------
----------------: | :-------: | | LibriSpeech | [LibriSpeech](http://
-www.openslr.org/12) | 970h | | Common Voice | [https://commonvoice.mozilla.org]
-(https://commonvoice.mozilla.org) | 1932h | ### Vietnamese | **Name** |
-**Source** | **Hours** | | :------------------------------------: | :----------
---------------------------------------------------------------------------: | :
--------: | | Vivos | [https://ailab.hcmus.edu.vn/vivos](https://
-ailab.hcmus.edu.vn/vivos) | 15h | | InfoRe Technology 1 | [InfoRe1 (passwd:
-BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip) | 25h | |
-InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd:
+deployed ## Pretrained Models Go to [drive](https://drive.google.com/drive/
+folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing) ## Corpus Sources ###
+English | **Name** | **Source** | **Hours** | | :----------- | :---------------
+-------------------------------------------------- | :-------- | | LibriSpeech
+| [LibriSpeech](http://www.openslr.org/12) | 970h | | Common Voice | [https://
+commonvoice.mozilla.org](https://commonvoice.mozilla.org) | 1932h | ###
+Vietnamese | **Name** | **Source** | **Hours** | | :---------------------------
+---------- | :-----------------------------------------------------------------
+-------------------- | :-------- | | Vivos | [https://ailab.hcmus.edu.vn/vivos]
+(https://ailab.hcmus.edu.vn/vivos) | 15h | | InfoRe Technology 1 | [InfoRe1
+(passwd: BroughtToYouByInfoRe)](https://files.huylenguyen.com/25hours.zip) |
+25h | | InfoRe Technology 2 (used in VLSP2019) | [InfoRe2 (passwd:
 BroughtToYouByInfoRe)](https://files.huylenguyen.com/audiobooks.zip) | 415h |
-### German | **Name** | **Source** | **Hours** | | :----------: | :------------
------------------------------------------------------: | :-------: | | Common
-Voice | [https://commonvoice.mozilla.org/](https://commonvoice.mozilla.org) |
-750h | ## References & Credits 1. [NVIDIA OpenSeq2Seq Toolkit](https://
+## How to contribute 1. Fork the project 2. [Install for development]
+(#installing-for-development) 3. Create a branch 4. Make a pull request to this
+repo ## References & Credits 1. [NVIDIA OpenSeq2Seq Toolkit](https://
 github.com/NVIDIA/OpenSeq2Seq) 2. [https://github.com/noahchalifour/warp-
 transducer](https://github.com/noahchalifour/warp-transducer) 3. [Sequence
 Transduction with Recurrent Neural Network](https://arxiv.org/abs/1211.3711) 4.
 [End-to-End Speech Processing Toolkit in PyTorch](https://github.com/espnet/
 espnet) 5. [https://github.com/iankur/ContextNet](https://github.com/iankur/
 ContextNet) ## Contact Huy Le Nguyen Email: nlhuy.cs.16@gmail.com
```

### Comparing `TensorFlowASR-1.0.3/TensorFlowASR.egg-info/SOURCES.txt` & `TensorFlowASR-2.0.0/TensorFlowASR.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,69 +7,78 @@
 setup.py
 TensorFlowASR.egg-info/PKG-INFO
 TensorFlowASR.egg-info/SOURCES.txt
 TensorFlowASR.egg-info/dependency_links.txt
 TensorFlowASR.egg-info/requires.txt
 TensorFlowASR.egg-info/top_level.txt
 tensorflow_asr/__init__.py
+tensorflow_asr/callbacks.py
+tensorflow_asr/configs.py
+tensorflow_asr/datasets.py
+tensorflow_asr/schemas.py
+tensorflow_asr/tokenizers.py
 tensorflow_asr/augmentations/__init__.py
 tensorflow_asr/augmentations/augmentation.py
 tensorflow_asr/augmentations/methods/__init__.py
 tensorflow_asr/augmentations/methods/base_method.py
+tensorflow_asr/augmentations/methods/gaussnoise.py
 tensorflow_asr/augmentations/methods/specaugment.py
-tensorflow_asr/configs/__init__.py
-tensorflow_asr/configs/config.py
-tensorflow_asr/datasets/__init__.py
-tensorflow_asr/datasets/asr_dataset.py
-tensorflow_asr/datasets/base_dataset.py
-tensorflow_asr/featurizers/__init__.py
-tensorflow_asr/featurizers/speech_featurizers.py
-tensorflow_asr/featurizers/text_featurizers.py
-tensorflow_asr/featurizers/methods/__init__.py
-tensorflow_asr/featurizers/methods/gammatone.py
-tensorflow_asr/helpers/__init__.py
-tensorflow_asr/helpers/dataset_helpers.py
-tensorflow_asr/helpers/exec_helpers.py
-tensorflow_asr/helpers/featurizer_helpers.py
+tensorflow_asr/features/__init__.py
+tensorflow_asr/features/gammatone.py
 tensorflow_asr/losses/__init__.py
 tensorflow_asr/losses/ctc_loss.py
 tensorflow_asr/losses/rnnt_loss.py
 tensorflow_asr/metrics/__init__.py
 tensorflow_asr/metrics/error_rates.py
 tensorflow_asr/models/__init__.py
+tensorflow_asr/models/base_layer.py
 tensorflow_asr/models/base_model.py
 tensorflow_asr/models/activations/__init__.py
 tensorflow_asr/models/activations/glu.py
 tensorflow_asr/models/ctc/__init__.py
 tensorflow_asr/models/ctc/base_ctc.py
+tensorflow_asr/models/ctc/conformer.py
 tensorflow_asr/models/ctc/deepspeech2.py
 tensorflow_asr/models/ctc/jasper.py
+tensorflow_asr/models/ctc/transformer.py
+tensorflow_asr/models/decoders/__init__.py
 tensorflow_asr/models/encoders/__init__.py
 tensorflow_asr/models/encoders/conformer.py
 tensorflow_asr/models/encoders/contextnet.py
+tensorflow_asr/models/encoders/deepspeech2.py
+tensorflow_asr/models/encoders/jasper.py
+tensorflow_asr/models/encoders/rnnt.py
+tensorflow_asr/models/encoders/transformer.py
 tensorflow_asr/models/layers/__init__.py
-tensorflow_asr/models/layers/bnlstmcell.py
+tensorflow_asr/models/layers/blurpool.py
+tensorflow_asr/models/layers/convolution.py
 tensorflow_asr/models/layers/embedding.py
+tensorflow_asr/models/layers/feature_extraction.py
+tensorflow_asr/models/layers/memory.py
 tensorflow_asr/models/layers/multihead_attention.py
-tensorflow_asr/models/layers/point_wise_ffn.py
 tensorflow_asr/models/layers/positional_encoding.py
-tensorflow_asr/models/layers/row_conv_1d.py
+tensorflow_asr/models/layers/residual.py
 tensorflow_asr/models/layers/sequence_wise_bn.py
 tensorflow_asr/models/layers/subsampling.py
 tensorflow_asr/models/transducer/__init__.py
 tensorflow_asr/models/transducer/base_transducer.py
 tensorflow_asr/models/transducer/conformer.py
 tensorflow_asr/models/transducer/contextnet.py
-tensorflow_asr/models/transducer/rnn_transducer.py
+tensorflow_asr/models/transducer/rnnt.py
+tensorflow_asr/models/transducer/transformer.py
 tensorflow_asr/optimizers/__init__.py
 tensorflow_asr/optimizers/accumulation.py
+tensorflow_asr/optimizers/regularizers.py
 tensorflow_asr/optimizers/schedules.py
 tensorflow_asr/utils/__init__.py
 tensorflow_asr/utils/app_util.py
+tensorflow_asr/utils/cli_util.py
 tensorflow_asr/utils/data_util.py
 tensorflow_asr/utils/env_util.py
 tensorflow_asr/utils/feature_util.py
 tensorflow_asr/utils/file_util.py
 tensorflow_asr/utils/layer_util.py
 tensorflow_asr/utils/math_util.py
 tensorflow_asr/utils/metric_util.py
-tensorflow_asr/utils/shape_util.py
+tensorflow_asr/utils/plot_util.py
+tensorflow_asr/utils/shape_util.py
+tensorflow_asr/utils/tf_util.py
```

### Comparing `TensorFlowASR-1.0.3/setup.py` & `TensorFlowASR-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from setuptools import find_packages, setup
-from typing import List
 from collections import defaultdict
+from typing import List
+
+from setuptools import find_packages, setup
 
 
 def parse_requirements(lines: List[str]):
-    extras_requires = defaultdict(list)
+    _extras_requires = defaultdict(list)
     extra = "requires"
     for line in lines:
         line = line.strip()
         if line.startswith("# extra="):
             extra = line.split("=")[1].strip()
             continue
         if line and line[0] != "#":
             lib_package = line.split("#")[0].strip()  # split comments
-            extras_requires[extra].append(lib_package)
-    install_requires = extras_requires.pop("requires")
-    return install_requires, extras_requires
+            _extras_requires[extra].append(lib_package)
+    _install_requires = _extras_requires.pop("requires")
+    return _install_requires, _extras_requires
 
 
 with open("requirements.txt", "r", encoding="utf-8") as fr:
     install_requires, extras_requires = parse_requirements(fr.readlines())
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="TensorFlowASR",
-    version="1.0.3",
+    version="2.0.0",
     author="Huy Le Nguyen",
     author_email="nlhuy.cs.16@gmail.com",
     description="Almost State-of-the-art Automatic Speech Recognition using Tensorflow 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TensorSpeech/TensorFlowASR",
     packages=find_packages(include=("tensorflow_asr", "tensorflow_asr.*")),
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/augmentations/methods/base_method.py` & `TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/base_method.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import tensorflow as tf
-
 
 class AugmentationMethod:
-    @tf.function
+    def __init__(self, prob: float = 0.5):
+        self.prob = prob
+
     def augment(self, *args, **kwargs):
         raise NotImplementedError()
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/datasets/asr_dataset.py` & `TensorFlowASR-2.0.0/tensorflow_asr/datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,389 +1,539 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Dataset Structures :kissing:
+
+# To make a custom dataset, inherit the `BaseDataset` class and override following methods:
+
+# 1. `create` to create `tf.data.Dataset` instance.
+# 2. `parse` for transforming `tf.data.Dataset` during creation by applyting `tf.data.Dataset.map` function.
+
+# _Note_: To create transcripts for **librispeech**, see [create_librispeech_trans.py](../../scripts/create_librispeech_trans.py)
+
+# ## ASR Datasets
+
+# An ASR dataset is some `.tsv` files in format: `PATH\tDURATION\tTRANSCRIPT`. You must create those files by your own with your own data and methods.
+
+# **Note**: Each `.tsv` file must include a header `PATH\tDURATION\tTRANSCRIPT` because it will remove these headers when loading dataset, otherwise you will lose 1 data file :sob:
+
+# **For transcript**, if you want to include characters such as dots, commas, double quote, etc.. you must create your own `.txt` vocabulary file. Default is [English](../featurizers/english.txt)
+
+# **Inputs**
+
+# ```python
+# class ASRTFRecordDataset(ASRDataset):
+#     """ Dataset for ASR using TFRecords """
+
+# class ASRSliceDataset(ASRDataset):
+#     """ Dataset for ASR using Slice """
+# ```
+
+# **Outputs when iterating dataset**
+
+# ```python
+# (
+#     {
+#         "inputs": ...,
+#         "inputs_length": ...,
+#         "predictions": ...,
+#         "predictions_length": ...,
+#     },
+#     {
+#         "labels": ...,
+#         "labels_length": ...
+#     }
+# )
+# ```
+
+# Where `predictions` and `predictions_length` are the label prepanded by blank and its length for training *Transducer*
+
 import json
 import os
-from typing import Union
+from dataclasses import asdict, dataclass
+
 import numpy as np
 import tensorflow as tf
 import tqdm
 
-from tensorflow_asr.augmentations.augmentation import Augmentation
-from tensorflow_asr.datasets.base_dataset import AUTOTUNE, BUFFER_SIZE, TFRECORD_SHARDS, BaseDataset
-from tensorflow_asr.featurizers.speech_featurizers import (
-    SpeechFeaturizer,
-    load_and_convert_to_wav,
-    read_raw_audio,
-    tf_read_raw_audio,
-)
-from tensorflow_asr.featurizers.text_featurizers import TextFeaturizer
+from tensorflow_asr import schemas
+from tensorflow_asr.configs import Config, DatasetConfig
+from tensorflow_asr.tokenizers import Tokenizer
 from tensorflow_asr.utils import data_util, feature_util, file_util, math_util
 
 logger = tf.get_logger()
 
 
+@dataclass
+class ASR_DATASER_TYPES:
+    TFRECORD: str = "tfrecord"
+    SLICE: str = "slice"
+    GENERATOR: str = "generator"
+
+
+def get(
+    tokenizer: Tokenizer,
+    dataset_config: DatasetConfig,
+    dataset_type: str,
+):
+    if dataset_type == ASR_DATASER_TYPES.TFRECORD:
+        return ASRTFRecordDataset(tokenizer=tokenizer, **vars(dataset_config))
+    if dataset_type == ASR_DATASER_TYPES.SLICE:
+        return ASRSliceDataset(tokenizer=tokenizer, **vars(dataset_config))
+    if dataset_type == ASR_DATASER_TYPES.GENERATOR:
+        return ASRDataset(tokenizer=tokenizer, **vars(dataset_config))
+    raise ValueError(f"dataset_type must in {asdict(ASR_DATASER_TYPES()).values()}")
+
+
+def get_global_shape(
+    config: Config,
+    strategy,
+    *datasets,
+    batch_size: int = None,
+    ga_steps: int = None,
+):
+    batch_size = (batch_size or config.learning_config.running_config.batch_size) * strategy.num_replicas_in_sync
+    ds_batch_size = batch_size
+    if ga_steps is not None and ga_steps > 1:
+        ds_batch_size *= ga_steps
+
+    max_input_length, max_label_length = 0, 0
+    for dset in datasets:
+        max_input_length = max(max_input_length, dset.max_input_length or 0)
+        max_label_length = max(max_label_length, dset.max_label_length or 0)
+    max_input_length = None if max_input_length == 0 else max_input_length
+    max_label_length = None if max_label_length == 0 else max_label_length
+
+    input_shape = [max_input_length]
+    prediction_shape = [max_label_length + 1] if max_label_length else [None]
+    label_shape = [max_label_length]
+    padded_shapes = (
+        schemas.TrainInput(
+            inputs=tf.TensorShape(input_shape),
+            inputs_length=tf.TensorShape([]),
+            predictions=tf.TensorShape(prediction_shape),
+            predictions_length=tf.TensorShape([]),
+        ),
+        schemas.TrainLabel(
+            labels=tf.TensorShape(label_shape),
+            labels_length=tf.TensorShape([]),
+        ),
+    )
+
+    return dict(
+        ds_batch_size=ds_batch_size,
+        batch_size=batch_size,
+        input_shape=input_shape,
+        prediction_shape=prediction_shape,
+        label_shape=label_shape,
+        padded_shapes=padded_shapes,
+    )
+
+
+BUFFER_SIZE = 100
+TFRECORD_SHARDS = 16
+AUTOTUNE = int(os.environ.get("AUTOTUNE") or tf.data.experimental.AUTOTUNE)
+
+
+class BaseDataset:
+    """Based dataset for all models"""
+
+    def __init__(
+        self,
+        data_paths: list,
+        cache: bool = False,
+        shuffle: bool = False,
+        buffer_size: int = BUFFER_SIZE,
+        indefinite: bool = False,
+        drop_remainder: bool = True,
+        enabled: bool = True,
+        metadata: str = None,
+        sample_rate: int = 16000,
+        stage: str = "train",
+        name: str = "",
+        **kwargs,
+    ):
+        self.data_paths = data_paths or []
+        if not isinstance(self.data_paths, list):
+            raise ValueError("data_paths must be a list of string paths")
+        self.cache = cache  # whether to cache transformed dataset to memory
+        self.shuffle = shuffle  # whether to shuffle tf.data.Dataset
+        self.buffer_size = buffer_size  # shuffle buffer size
+        self.stage = stage  # for defining tfrecords files
+        self.enabled = enabled
+        self.drop_remainder = drop_remainder  # whether to drop remainder for multi gpu training
+        self.indefinite = indefinite  # Whether to make dataset repeat indefinitely -> avoid the potential last partial batch
+        self.total_steps = None  # for better training visualization
+        self.metadata = metadata
+        self.sample_rate = sample_rate
+        self.name = name
+
+    def parse(self, *args, **kwargs):
+        raise NotImplementedError()
+
+    def create(self, batch_size):
+        raise NotImplementedError()
+
+
 class ASRDataset(BaseDataset):
     """Dataset for ASR using Generator"""
 
     def __init__(
         self,
         stage: str,
-        speech_featurizer: SpeechFeaturizer,
-        text_featurizer: TextFeaturizer,
+        tokenizer: Tokenizer,
         data_paths: list,
-        augmentations: Augmentation = Augmentation(None),
         cache: bool = False,
         shuffle: bool = False,
-        indefinite: bool = False,
+        indefinite: bool = True,
         drop_remainder: bool = True,
-        use_tf: bool = False,
+        enabled: bool = True,
+        metadata: str = None,
         buffer_size: int = BUFFER_SIZE,
+        sample_rate: int = 16000,
+        name: str = "",
         **kwargs,
     ):
         super().__init__(
             data_paths=data_paths,
-            augmentations=augmentations,
             cache=cache,
             shuffle=shuffle,
             stage=stage,
             buffer_size=buffer_size,
             drop_remainder=drop_remainder,
-            use_tf=use_tf,
+            enabled=enabled,
+            metadata=metadata,
             indefinite=indefinite,
+            sample_rate=sample_rate,
+            name=name,
+            **kwargs,
         )
-        self.speech_featurizer = speech_featurizer
-        self.text_featurizer = text_featurizer
+        self.entries = []
+        self.tokenizer = tokenizer
+        self.max_input_length = None
+        self.max_label_length = None
+        self.load_metadata()
 
     # -------------------------------- metadata -------------------------------------
 
     def compute_metadata(self):
+        self.max_input_length = 0 if self.max_input_length is None else self.max_input_length
+        self.max_label_length = 0 if self.max_label_length is None else self.max_label_length
+        if self.max_input_length > 0 and self.max_label_length > 0:
+            return  # already computed
         self.read_entries()
-        for _, duration, indices in tqdm.tqdm(self.entries, desc=f"Computing metadata for entries in {self.stage} dataset"):
-            input_length = self.speech_featurizer.get_length_from_duration(duration)
-            label = str(indices).split()
+        for _, duration, transcript in tqdm.tqdm(self.entries, desc=f"Computing metadata for entries in {self.stage} dataset"):
+            input_length = math_util.get_nsamples(duration, self.sample_rate)
+            label = self.tokenizer.tokenize(transcript).numpy()
             label_length = len(label)
-            self.speech_featurizer.update_length(input_length)
-            self.text_featurizer.update_length(label_length)
+            self.max_input_length = max(self.max_input_length, input_length)
+            self.max_label_length = max(self.max_label_length, label_length)
 
-    def save_metadata(self, metadata: str = None):
-        if metadata is None:
+    def save_metadata(self):
+        if self.metadata is None:
             return
-        metadata = file_util.preprocess_paths(metadata)
-        if tf.io.gfile.exists(metadata):
-            with tf.io.gfile.GFile(metadata, "r") as f:
+        self.metadata = file_util.preprocess_paths(self.metadata)
+        if tf.io.gfile.exists(self.metadata):
+            with tf.io.gfile.GFile(self.metadata, "r") as f:
                 try:
                     content = json.loads(f.read())
-                except json.JSONDecodeError:
-                    raise ValueError(f"File {metadata} is currently not in json format. Please update the file")
+                except json.JSONDecodeError as e:
+                    raise ValueError(f"File {self.metadata} is currently not in json format. Please update the file") from e
         else:
             content = {}
-        content[self.stage] = {
-            "max_input_length": self.speech_featurizer.max_length,
-            "max_label_length": self.text_featurizer.max_length,
-            "num_entries": self.total_steps,
-        }
-        with tf.io.gfile.GFile(metadata, "w") as f:
+        content[self.stage] = dict(
+            max_input_length=self.max_input_length,
+            max_label_length=self.max_label_length,
+            num_entries=self.total_steps,
+        )
+        with tf.io.gfile.GFile(self.metadata, "w") as f:
             f.write(json.dumps(content, indent=2))
-        logger.info(f"Metadata written to {metadata}")
+        logger.info(f"Metadata written to {self.metadata}")
 
-    def load_metadata(self, metadata: Union[str, dict] = None):
-        if metadata is None:
+    def load_metadata(self):
+        if self.metadata is None:
+            return
+        if not self.enabled:
             return
         content = None
-        if isinstance(metadata, dict):
-            content = metadata
-        else:
-            metadata = file_util.preprocess_paths(metadata)
-            if tf.io.gfile.exists(metadata):
-                logger.info(f"Loading metadata from {metadata} ...")
-                with tf.io.gfile.GFile(metadata, "r") as f:
-                    try:
-                        content = json.loads(f.read()).get(self.stage, {})
-                    except json.JSONDecodeError:
-                        raise ValueError(f"File {metadata} must be in json format")
+        self.metadata = file_util.preprocess_paths(self.metadata)
+        if tf.io.gfile.exists(self.metadata):
+            logger.info(f"Loading metadata from {self.metadata} ...")
+            with tf.io.gfile.GFile(self.metadata, "r") as f:
+                try:
+                    content = json.loads(f.read()).get(self.stage, {})
+                except json.JSONDecodeError as e:
+                    raise ValueError(f"File {self.metadata} must be in json format") from e
         if not content:
             return
-        self.speech_featurizer.update_length(int(content.get("max_input_length", 0)))
-        self.text_featurizer.update_length(int(content.get("max_label_length", 0)))
+        self.max_input_length = content.get("max_input_length")
+        self.max_label_length = content.get("max_label_length")
         self.total_steps = int(content.get("num_entries", 0))
+        self.num_entries = self.total_steps
 
-    def update_metadata(self, metadata: str = None):
-        self.load_metadata(metadata)
+    def update_metadata(self):
+        self.load_metadata()
         self.compute_metadata()
-        self.save_metadata(metadata)
+        self.save_metadata()
 
     # -------------------------------- ENTRIES -------------------------------------
 
     def read_entries(self):
         if hasattr(self, "entries") and len(self.entries) > 0:
             return
-        self.entries = []
+        self.data_paths = file_util.preprocess_paths(self.data_paths, enabled=self.enabled, check_exists=True)
         for file_path in self.data_paths:
             logger.info(f"Reading {file_path} ...")
             with tf.io.gfile.GFile(file_path, "r") as f:
-                temp_lines = f.read().splitlines()
-                # Skip the header of tsv file
-                self.entries += temp_lines[1:]
-        # The files is "\t" seperated
-        self.entries = [line.split("\t", 2) for line in self.entries]
-        for i, line in enumerate(self.entries):
-            self.entries[i][-1] = " ".join([str(x) for x in self.text_featurizer.extract(line[-1]).numpy()])
+                for line in f.read().splitlines()[1:]:  # Skip the header of tsv file
+                    self.entries.append(line.split("\t", 2))  # The files is "\t" seperated
         self.entries = np.array(self.entries)
         if self.shuffle:
             np.random.shuffle(self.entries)  # Mix transcripts.tsv
         self.total_steps = len(self.entries)
+        self.num_entries = self.total_steps
 
     # -------------------------------- LOAD AND PREPROCESS -------------------------------------
 
     def generator(self):
-        for path, _, indices in self.entries:
-            audio = load_and_convert_to_wav(path).numpy()
-            yield bytes(path, "utf-8"), audio, bytes(indices, "utf-8")
-
-    def preprocess(self, path: tf.Tensor, audio: tf.Tensor, indices: tf.Tensor):
-        with tf.device("/CPU:0"):
-
-            def fn(_path: bytes, _audio: bytes, _indices: bytes):
-                signal = read_raw_audio(_audio, sample_rate=self.speech_featurizer.sample_rate)
-                signal = self.augmentations.signal_augment(signal)
-                features = self.speech_featurizer.extract(signal.numpy())
-                features = self.augmentations.feature_augment(features)
-                features = tf.convert_to_tensor(features, tf.float32)
-                input_length = tf.cast(tf.shape(features)[0], tf.int32)
-
-                label = tf.strings.to_number(tf.strings.split(_indices), out_type=tf.int32)
-                label_length = tf.cast(tf.shape(label)[0], tf.int32)
+        for path, _, transcript in self.entries:
+            audio = data_util.load_and_convert_to_wav(path, sample_rate=self.sample_rate).numpy()
+            yield bytes(path, "utf-8"), audio, bytes(transcript, "utf-8")
 
-                prediction = self.text_featurizer.prepand_blank(label)
-                prediction_length = tf.cast(tf.shape(prediction)[0], tf.int32)
+    def _process_item(self, path: tf.Tensor, audio: tf.Tensor, transcript: tf.Tensor):
+        inputs = data_util.read_raw_audio(audio)
+        inputs_length = tf.shape(inputs)[0]
 
-                return _path, features, input_length, label, label_length, prediction, prediction_length
+        labels = self.tokenizer.tokenize(transcript)
+        labels_length = tf.shape(labels, out_type=tf.int32)[0]
 
-            return tf.numpy_function(
-                fn, inp=[path, audio, indices], Tout=[tf.string, tf.float32, tf.int32, tf.int32, tf.int32, tf.int32, tf.int32]
-            )
+        predictions = self.tokenizer.prepand_blank(labels)
+        predictions_length = tf.shape(predictions, out_type=tf.int32)[0]
 
-    def tf_preprocess(self, path: tf.Tensor, audio: tf.Tensor, indices: tf.Tensor):
-        with tf.device("/CPU:0"):
-            signal = tf_read_raw_audio(audio, self.speech_featurizer.sample_rate)
-            signal = self.augmentations.signal_augment(signal)
-            features = self.speech_featurizer.tf_extract(signal)
-            features = self.augmentations.feature_augment(features)
-            input_length = tf.cast(tf.shape(features)[0], tf.int32)
-
-            label = tf.strings.to_number(tf.strings.split(indices), out_type=tf.int32)
-            label_length = tf.cast(tf.shape(label)[0], tf.int32)
+        return path, inputs, inputs_length, labels, labels_length, predictions, predictions_length
 
-            prediction = self.text_featurizer.prepand_blank(label)
-            prediction_length = tf.cast(tf.shape(prediction)[0], tf.int32)
-
-            return path, features, input_length, label, label_length, prediction, prediction_length
-
-    def parse(self, path: tf.Tensor, audio: tf.Tensor, indices: tf.Tensor):
+    def parse(self, path: tf.Tensor, audio: tf.Tensor, transcript: tf.Tensor):
         """
         Returns:
             path, features, input_lengths, labels, label_lengths, pred_inp
         """
-        data = self.tf_preprocess(path, audio, indices) if self.use_tf else self.preprocess(path, audio, indices)
-        _, features, input_length, label, label_length, prediction, prediction_length = data
+        (
+            _,
+            inputs,
+            inputs_length,
+            labels,
+            labels_length,
+            predictions,
+            predictions_length,
+        ) = self._process_item(path=path, audio=audio, transcript=transcript)
         return (
-            data_util.create_inputs(
-                inputs=features, inputs_length=input_length, predictions=prediction, predictions_length=prediction_length
-            ),
-            data_util.create_labels(labels=label, labels_length=label_length),
+            schemas.TrainInput(inputs=inputs, inputs_length=inputs_length, predictions=predictions, predictions_length=predictions_length),
+            schemas.TrainLabel(labels=labels, labels_length=labels_length),
         )
 
     # -------------------------------- CREATION -------------------------------------
 
-    def process(self, dataset, batch_size):
-        dataset = dataset.map(self.parse, num_parallel_calls=AUTOTUNE)
-        self.total_steps = math_util.get_num_batches(self.total_steps, batch_size, drop_remainders=self.drop_remainder)
-
+    def process(self, dataset: tf.data.Dataset, batch_size: int, padded_shapes=None):
         if self.cache:
-            dataset = dataset.cache()
+            dataset = dataset.cache()  # cache original (unchanged data)
+
+        dataset = dataset.map(self.parse, num_parallel_calls=AUTOTUNE, deterministic=False)
+        self.total_steps = math_util.get_num_batches(self.num_entries, batch_size, drop_remainders=self.drop_remainder)
 
         if self.shuffle:
-            dataset = dataset.shuffle(self.buffer_size, reshuffle_each_iteration=True)
+            dataset = dataset.shuffle(self.buffer_size or self.num_entries, reshuffle_each_iteration=True)
 
         if self.indefinite and self.total_steps:
             dataset = dataset.repeat()
 
-        # PADDED BATCH the dataset
-        dataset = dataset.padded_batch(
-            batch_size=batch_size,
-            padded_shapes=(
-                data_util.create_inputs(
-                    inputs=tf.TensorShape(self.speech_featurizer.shape),
+        if padded_shapes is None:
+            padded_shapes = (
+                schemas.TrainInput(
+                    inputs=tf.TensorShape([self.max_input_length]),
                     inputs_length=tf.TensorShape([]),
-                    predictions=tf.TensorShape(self.text_featurizer.prepand_shape),
+                    predictions=tf.TensorShape([self.max_label_length + 1 if self.max_label_length else None]),
                     predictions_length=tf.TensorShape([]),
                 ),
-                data_util.create_labels(labels=tf.TensorShape(self.text_featurizer.shape), labels_length=tf.TensorShape([])),
-            ),
-            padding_values=(
-                data_util.create_inputs(
-                    inputs=0.0, inputs_length=0, predictions=self.text_featurizer.blank, predictions_length=0
+                schemas.TrainLabel(
+                    labels=tf.TensorShape([self.max_label_length]),
+                    labels_length=tf.TensorShape([]),
                 ),
-                data_util.create_labels(labels=self.text_featurizer.blank, labels_length=0),
+            )
+
+        # PADDED BATCH the dataset
+        dataset = dataset.padded_batch(
+            batch_size=batch_size,
+            padded_shapes=padded_shapes,
+            padding_values=(
+                schemas.TrainInput(inputs=0.0, inputs_length=0, predictions=self.tokenizer.blank, predictions_length=0),
+                schemas.TrainLabel(labels=self.tokenizer.blank, labels_length=0),
             ),
             drop_remainder=self.drop_remainder,
         )
 
         # PREFETCH to improve speed of input length
         dataset = dataset.prefetch(AUTOTUNE)
         return dataset
 
-    def create(self, batch_size: int):
+    def create(self, batch_size: int, padded_shapes=None):
+        if not self.enabled:
+            return None
         self.read_entries()
         if not self.total_steps or self.total_steps == 0:
             return None
         dataset = tf.data.Dataset.from_generator(
             self.generator,
             output_types=(tf.string, tf.string, tf.string),
             output_shapes=(tf.TensorShape([]), tf.TensorShape([]), tf.TensorShape([])),
         )
-        return self.process(dataset, batch_size)
+        return self.process(dataset, batch_size, padded_shapes=padded_shapes)
 
 
 class ASRTFRecordDataset(ASRDataset):
     """Dataset for ASR using TFRecords"""
 
     def __init__(
         self,
         data_paths: list,
         tfrecords_dir: str,
-        speech_featurizer: SpeechFeaturizer,
-        text_featurizer: TextFeaturizer,
+        tokenizer: Tokenizer,
         stage: str,
-        augmentations: Augmentation = Augmentation(None),
         tfrecords_shards: int = TFRECORD_SHARDS,
         cache: bool = False,
         shuffle: bool = False,
-        use_tf: bool = False,
-        indefinite: bool = False,
+        enabled: bool = True,
+        metadata: str = None,
+        indefinite: bool = True,
         drop_remainder: bool = True,
         buffer_size: int = BUFFER_SIZE,
+        compression_type: str = "GZIP",
+        sample_rate: int = 16000,
+        name: str = "",
         **kwargs,
     ):
         super().__init__(
             stage=stage,
-            speech_featurizer=speech_featurizer,
-            text_featurizer=text_featurizer,
+            tokenizer=tokenizer,
             data_paths=data_paths,
-            augmentations=augmentations,
             cache=cache,
             shuffle=shuffle,
             buffer_size=buffer_size,
             drop_remainder=drop_remainder,
-            use_tf=use_tf,
+            enabled=enabled,
+            metadata=metadata,
             indefinite=indefinite,
+            sample_rate=sample_rate,
+            name=name,
+            **kwargs,
         )
         if not self.stage:
             raise ValueError("stage must be defined, either 'train', 'eval' or 'test'")
         self.tfrecords_dir = tfrecords_dir
         if tfrecords_shards <= 0:
             raise ValueError("tfrecords_shards must be positive")
         self.tfrecords_shards = tfrecords_shards
+        self.compression_type = compression_type
 
-    @staticmethod
-    def write_tfrecord_file(splitted_entries):
+    def write_tfrecord_file(self, splitted_entries: tuple):
         shard_path, entries = splitted_entries
-
-        def parse(record):
-            def fn(path, indices):
-                audio = load_and_convert_to_wav(path.decode("utf-8")).numpy()
-                feature = {
-                    "path": feature_util.bytestring_feature([path]),
-                    "audio": feature_util.bytestring_feature([audio]),
-                    "indices": feature_util.bytestring_feature([indices]),
-                }
-                example = tf.train.Example(features=tf.train.Features(feature=feature))
-                return example.SerializeToString()
-
-            return tf.numpy_function(fn, inp=[record[0], record[2]], Tout=tf.string)
-
-        dataset = tf.data.Dataset.from_tensor_slices(entries)
-        dataset = dataset.map(parse, num_parallel_calls=AUTOTUNE)
-        writer = tf.data.experimental.TFRecordWriter(shard_path, compression_type="ZLIB")
         logger.info(f"Processing {shard_path} ...")
-        writer.write(dataset)
+        with tf.io.TFRecordWriter(shard_path, options=tf.io.TFRecordOptions(compression_type=self.compression_type)) as writer:
+            for path, _, transcript in entries:
+                audio = data_util.load_and_convert_to_wav(path, sample_rate=self.sample_rate).numpy()
+                feature = dict(
+                    path=feature_util.bytestring_feature([path.encode("utf-8")]),
+                    audio=feature_util.bytestring_feature([audio]),
+                    transcript=feature_util.bytestring_feature([transcript.encode("utf-8")]),
+                )
+                example = tf.train.Example(features=tf.train.Features(feature=feature))
+                writer.write(example.SerializeToString())
         logger.info(f"Created {shard_path}")
 
     def create_tfrecords(self):
         if not self.tfrecords_dir:
             return False
+        self.tfrecords_dir = file_util.preprocess_paths(self.tfrecords_dir, isdir=True, enabled=self.enabled)
 
         if tf.io.gfile.glob(os.path.join(self.tfrecords_dir, f"{self.stage}*.tfrecord")):
             logger.info(f"TFRecords're already existed: {self.stage}")
             return True
 
         logger.info(f"Creating {self.stage}.tfrecord ...")
 
         self.read_entries()
         if not self.total_steps or self.total_steps == 0:
             return False
 
-        def get_shard_path(shard_id):
+        def get_shard_path(shard_id: int):
             return os.path.join(self.tfrecords_dir, f"{self.stage}_{shard_id}.tfrecord")
 
         shards = [get_shard_path(idx) for idx in range(1, self.tfrecords_shards + 1)]
 
         splitted_entries = np.array_split(self.entries, self.tfrecords_shards)
         for entries in zip(shards, splitted_entries):
             self.write_tfrecord_file(entries)
 
         return True
 
-    def parse(self, record: tf.Tensor):
-        feature_description = {
-            "path": tf.io.FixedLenFeature([], tf.string),
-            "audio": tf.io.FixedLenFeature([], tf.string),
-            "indices": tf.io.FixedLenFeature([], tf.string),
-        }
+    def parse(self, record: tf.Tensor, **kwargs):
+        feature_description = dict(
+            path=tf.io.FixedLenFeature([], tf.string),
+            audio=tf.io.FixedLenFeature([], tf.string),
+            transcript=tf.io.FixedLenFeature([], tf.string),
+        )
         example = tf.io.parse_single_example(record, feature_description)
         return super().parse(**example)
 
-    def create(self, batch_size: int):
+    def create(self, batch_size: int, padded_shapes=None):
+        if not self.enabled:
+            return None
         have_data = self.create_tfrecords()
         if not have_data:
             return None
 
         pattern = os.path.join(self.tfrecords_dir, f"{self.stage}*.tfrecord")
-        files_ds = tf.data.Dataset.list_files(pattern)
+        files_ds = tf.data.Dataset.list_files(pattern, shuffle=self.shuffle)
         ignore_order = tf.data.Options()
-        ignore_order.experimental_deterministic = False
+        ignore_order.deterministic = False
         files_ds = files_ds.with_options(ignore_order)
-        dataset = tf.data.TFRecordDataset(files_ds, compression_type="ZLIB", num_parallel_reads=AUTOTUNE)
+        dataset = tf.data.TFRecordDataset(files_ds, compression_type=self.compression_type, num_parallel_reads=AUTOTUNE)
 
-        return self.process(dataset, batch_size)
+        return self.process(dataset, batch_size, padded_shapes=padded_shapes)
 
 
 class ASRSliceDataset(ASRDataset):
     """Dataset for ASR using Slice"""
 
-    @staticmethod
-    def load(record: tf.Tensor):
-        def fn(path: bytes):
-            return load_and_convert_to_wav(path.decode("utf-8")).numpy()
-
-        audio = tf.numpy_function(fn, inp=[record[0]], Tout=tf.string)
+    def load(self, record):
+        audio = tf.numpy_function(
+            lambda path: data_util.load_and_convert_to_wav(path.decode("utf-8"), sample_rate=self.sample_rate).numpy(),
+            inp=[record[0]],
+            Tout=tf.string,
+        )
         return record[0], audio, record[2]
 
-    def create(self, batch_size: int):
+    def create(self, batch_size: int, padded_shapes=None):
+        if not self.enabled:
+            return None
         self.read_entries()
         if not self.total_steps or self.total_steps == 0:
             return None
+
         dataset = tf.data.Dataset.from_tensor_slices(self.entries)
-        dataset = dataset.map(self.load, num_parallel_calls=AUTOTUNE)
-        return self.process(dataset, batch_size)
+        options = tf.data.Options()
+        options.deterministic = False
+        options.experimental_distribute.auto_shard_policy = tf.data.experimental.AutoShardPolicy.DATA
+        dataset = dataset.with_options(options)
+        dataset = dataset.map(self.load, num_parallel_calls=AUTOTUNE, deterministic=False)
+
+        return self.process(dataset, batch_size, padded_shapes=padded_shapes)
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/featurizers/methods/gammatone.py` & `TensorFlowASR-2.0.0/tensorflow_asr/features/gammatone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit) and Huy Phan (@pquochuy)
+# Copyright 2020 Huy Le Nguyen (@nglehuy) and Huy Phan (@pquochuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -116,19 +116,19 @@
     # TODO: Factor these parameters out
     ear_q = 9.26449  # Glasberg and Moore Parameters
     min_bw = 24.7
 
     # All of the following expressions are derived in Apple TR #35, "An
     # Efficient Implementation of the Patterson-Holdsworth Cochlear Filter
     # Bank." See pages 33-34.
-    erb_point = -ear_q * min_bw + tf.exp(
-        fraction * (-tf.math.log(high_freq + ear_q * min_bw) + tf.math.log(low_freq + ear_q * min_bw))
-    ) * (high_freq + ear_q * min_bw)
+    erbp = (-ear_q * min_bw) + (
+        tf.exp(fraction * ((-1 * tf.math.log(high_freq + ear_q * min_bw)) + tf.math.log(low_freq + ear_q * min_bw))) * (high_freq + ear_q * min_bw)
+    )
 
-    return tf.cast(erb_point, tf.complex64)
+    return tf.cast(erbp, tf.complex64)
 
 
 def erb_space(
     low_freq=DEFAULT_LOW_FREQ,
     high_freq=DEFAULT_HIGH_FREQ,
     num=DEFAULT_FILTER_NUM,
 ):
@@ -196,28 +196,28 @@
     # Change the followFreqing three parameters if you wish to use a different
     # ERB scale. Must change in ERBSpace too.
     # TODO: factor these out
     ear_q = 9.26449  # Glasberg and Moore Parameters
     min_bw = 24.7
     order = 1
 
-    erb = width * ((centre_freqs / ear_q) ** order + min_bw ** order) ** (1 / order)
+    erb = width * ((centre_freqs / ear_q) ** order + min_bw**order) ** (1 / order)
     B = 1.019 * 2 * pi * erb
 
     arg = 2 * centre_freqs * pi * T
     vec = tf.exp(2j * arg)
 
     A0 = T
     A2 = 0
     B0 = 1
     B1 = -2 * tf.cos(arg) / tf.exp(B * T)
     B2 = tf.exp(-2 * B * T)
 
-    rt_pos = tf.cast(tf.sqrt(3 + 2 ** 1.5), tf.complex64)
-    rt_neg = tf.cast(tf.sqrt(3 - 2 ** 1.5), tf.complex64)
+    rt_pos = tf.cast(tf.sqrt(3 + 2**1.5), tf.complex64)
+    rt_neg = tf.cast(tf.sqrt(3 - 2**1.5), tf.complex64)
 
     common = -T * tf.exp(-(B * T))
 
     # TODO: This could be simplified to a matrix calculation involving the
     # constant first term and the alternating rt_pos/rt_neg and +/-1 second
     # terms
     k11 = tf.cos(arg) + rt_pos * tf.sin(arg)
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/featurizers/text_featurizers.py` & `TensorFlowASR-2.0.0/tensorflow_asr/tokenizers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,47 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import abc
 import codecs
+import multiprocessing
 import os
 import unicodedata
-from multiprocessing import cpu_count
-import numpy as np
+from dataclasses import asdict, dataclass
+
 import sentencepiece as sp
 import tensorflow as tf
-import tensorflow_datasets as tds
+import tensorflow_text as tft
+from tensorflow_text.tools.wordpiece_vocab import bert_vocab_from_dataset as bert_vocab
 
-from tensorflow_asr.configs.config import DecoderConfig
+from tensorflow_asr.configs import Config, DecoderConfig
 from tensorflow_asr.utils import file_util
 
+logger = tf.get_logger()
+
+
+@dataclass
+class TOKENIZER_TYPES:
+    CHARACTERS: str = "characters"
+    WORDPIECE: str = "wordpiece"
+    SENTENCEPIECE: str = "sentencepiece"
+
+
 ENGLISH_CHARACTERS = [
+    "<blank>",
     " ",
     "a",
     "b",
     "c",
     "d",
     "e",
     "f",
@@ -53,27 +65,62 @@
     "x",
     "y",
     "z",
     "'",
 ]
 
 
-class TextFeaturizer(metaclass=abc.ABCMeta):
-    def __init__(
-        self,
-        decoder_config: dict,
-    ):
+def get(config: Config):
+    if config.decoder_config.type == TOKENIZER_TYPES.SENTENCEPIECE:
+        logger.info("Loading SentencePiece model ...")
+        tokenizer = SentencePieceTokenizer(config.decoder_config)
+    elif config.decoder_config.type == TOKENIZER_TYPES.WORDPIECE:
+        logger.info("Loading wordpiece ...")
+        tokenizer = WordPieceTokenizer(config.decoder_config)
+    elif config.decoder_config.type == TOKENIZER_TYPES.CHARACTERS:
+        logger.info("Use characters ...")
+        tokenizer = CharTokenizer(config.decoder_config)
+    else:
+        raise ValueError(f"type must be in {asdict(TOKENIZER_TYPES()).values()}, received {config.decoder_config.type}")
+    return tokenizer
+
+
+def build(config: Config):
+    if config.decoder_config.type == TOKENIZER_TYPES.CHARACTERS:
+        CharTokenizer.build_from_corpus(config.decoder_config)
+        return
+    if config.decoder_config.type == TOKENIZER_TYPES.SENTENCEPIECE:
+        SentencePieceTokenizer.build_from_corpus(config.decoder_config)
+        return
+    if config.decoder_config.type == TOKENIZER_TYPES.WORDPIECE:
+        WordPieceTokenizer.build_from_corpus(config.decoder_config)
+        return
+
+
+class Tokenizer:
+    def __init__(self, decoder_config: DecoderConfig):
         self.scorer = None
-        self.decoder_config = DecoderConfig(decoder_config)
+        self.decoder_config = decoder_config
         self.blank = None
         self.tokens2indices = {}
         self.tokens = []
         self.num_classes = None
         self.max_length = 0
 
+    @classmethod
+    def corpus_generator(cls, decoder_config: DecoderConfig):
+        for file_path in file_util.preprocess_paths(decoder_config.train_files):
+            logger.info(f"Reading {file_path} ...")
+            with tf.io.gfile.GFile(file_path, "r") as f:
+                temp_lines = f.read().splitlines()
+                for line in temp_lines[1:]:  # Skip the header of tsv file
+                    data = line.split("\t", 2)[-1]  # get only transcript
+                    data = cls.normalize_text(data, decoder_config.normalization_form).numpy()
+                    yield data
+
     @property
     def shape(self) -> list:
         return [self.max_length if self.max_length > 0 else None]
 
     @property
     def prepand_shape(self) -> list:
         return [self.max_length + 1 if self.max_length > 0 else None]
@@ -83,493 +130,310 @@
         length: int,
     ):
         self.max_length = max(self.max_length, length)
 
     def reset_length(self):
         self.max_length = 0
 
-    def preprocess_text(self, text):
-        text = unicodedata.normalize("NFC", text.lower())
-        return text.strip("\n")  # remove trailing newline
+    @classmethod
+    def normalize_text(cls, text: tf.Tensor, normalization_form: str = "NFKC"):
+        text = tft.normalize_utf8(text, normalization_form)
+        text = tf.strings.regex_replace(text, r"\p{Cc}|\p{Cf}", " ")
+        text = tf.strings.regex_replace(text, r" +", " ")
+        text = tf.strings.lower(text, encoding="utf-8")
+        text = tf.strings.strip(text)  # remove trailing whitespace
+        return text
 
-    def add_scorer(
-        self,
-        scorer: any = None,
-    ):
+    def add_scorer(self, scorer: any = None):
         """Add scorer to this instance"""
         self.scorer = scorer
 
-    def normalize_indices(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+    def normalize_indices(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Remove -1 in indices by replacing them with blanks
         Args:
             indices (tf.Tensor): shape any
 
         Returns:
             tf.Tensor: normalized indices with shape same as indices
         """
         with tf.name_scope("normalize_indices"):
             minus_one = -1 * tf.ones_like(indices, dtype=tf.int32)
             blank_like = self.blank * tf.ones_like(indices, dtype=tf.int32)
             return tf.where(indices == minus_one, blank_like, indices)
 
-    def prepand_blank(
-        self,
-        text: tf.Tensor,
-    ) -> tf.Tensor:
+    def prepand_blank(self, text: tf.Tensor) -> tf.Tensor:
         """Prepand blank index for transducer models"""
-        return tf.concat([[self.blank], text], axis=0)
+        return tf.concat([[self.blank], text], 0)
 
-    @abc.abstractclassmethod
-    def extract(self, text):
+    def tokenize(self, text: str) -> tf.Tensor:
         raise NotImplementedError()
 
-    @abc.abstractclassmethod
-    def iextract(self, indices):
+    def detokenize(self, indices: tf.Tensor) -> tf.Tensor:
         raise NotImplementedError()
 
-    @abc.abstractclassmethod
-    def indices2upoints(self, indices):
+    def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         raise NotImplementedError()
 
 
-class CharFeaturizer(TextFeaturizer):
+class CharTokenizer(Tokenizer):
     """
     Extract text feature based on char-level granularity.
     By looking up the vocabulary table, each line of transcript will be
     converted to a sequence of integer indexes.
     """
 
-    def __init__(
-        self,
-        decoder_config: dict,
-    ):
-        """
-        decoder_config = {
-            "vocabulary": str,
-            "blank_at_zero": bool,
-            "beam_width": int,
-            "lm_config": {
-                ...
-            }
-        }
-        """
-        super(CharFeaturizer, self).__init__(decoder_config)
-        self.__init_vocabulary()
-
-    def __init_vocabulary(self):
+    def __init__(self, decoder_config: DecoderConfig):
+        super().__init__(decoder_config)
         lines = []
         if self.decoder_config.vocabulary is not None:
             with codecs.open(self.decoder_config.vocabulary, "r", "utf-8") as fin:
                 lines.extend(fin.readlines())
         else:
             lines = ENGLISH_CHARACTERS
-        self.blank = 0 if self.decoder_config.blank_at_zero else None
-        self.tokens2indices = {}
+        self.blank = self.decoder_config.blank_index
         self.tokens = []
-        index = 1 if self.blank == 0 else 0
         for line in lines:
-            line = self.preprocess_text(line)
+            line = unicodedata.normalize(self.decoder_config.normalization_form, line.lower()).strip("\n")
             if line.startswith("#") or not line:
                 continue
-            self.tokens2indices[line[0]] = index
-            self.tokens.append(line[0])
-            index += 1
+            self.tokens.append(line)
         if self.blank is None:
             self.blank = len(self.tokens)  # blank not at zero
-        self.non_blank_tokens = self.tokens.copy()
-        self.tokens.insert(self.blank, "")  # add blank token to tokens
         self.num_classes = len(self.tokens)
-        self.tokens = tf.convert_to_tensor(self.tokens, dtype=tf.string)
+        self.indices = tf.range(self.num_classes, dtype=tf.int32)
+        self.tokenizer = tf.lookup.StaticHashTable(
+            tf.lookup.KeyValueTensorInitializer(keys=self.tokens, values=self.indices, key_dtype=tf.string, value_dtype=tf.int32),
+            default_value=self.blank,
+        )
+        self.detokenizer = tf.lookup.StaticHashTable(
+            tf.lookup.KeyValueTensorInitializer(keys=self.indices, values=self.tokens, key_dtype=tf.int32, value_dtype=tf.string),
+            default_value=self.tokens[self.blank],
+        )
         self.upoints = tf.strings.unicode_decode(self.tokens, "UTF-8").to_tensor(shape=[None, 1])
 
-    def extract(
-        self,
-        text: str,
-    ) -> tf.Tensor:
-        """
-        Convert string to a list of integers
-        Args:
-            text: string (sequence of characters)
+    @classmethod
+    def build_from_corpus(cls, decoder_config: DecoderConfig):
+        if os.path.exists(decoder_config.vocabulary):
+            return cls(decoder_config)
 
-        Returns:
-            sequence of ints in tf.Tensor
-        """
-        text = self.preprocess_text(text)
-        text = list(text.strip())  # remove trailing space
-        indices = [self.tokens2indices[token] for token in text]
-        return tf.convert_to_tensor(indices, dtype=tf.int32)
+        def write_vocab_file(filepath, vocab):
+            with tf.io.gfile.GFile(filepath, "w") as f:
+                for token in vocab:
+                    print(token, file=f)
 
-    def iextract(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+        vocab = set()
+        for text in cls.corpus_generator(decoder_config):
+            vocab.update(text)
+
+        write_vocab_file(decoder_config.vocabulary, vocab)
+
+        return cls(decoder_config)
+
+    def tokenize(self, text):
+        text = self.normalize_text(text, self.decoder_config.normalization_form)
+        text = tf.strings.unicode_split(text, "UTF-8")
+        return self.tokenizer.lookup(text)
+
+    def detokenize(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Convert list of indices to string
         Args:
             indices: tf.Tensor with dim [B, None]
 
         Returns:
             transcripts: tf.Tensor of dtype tf.string with dim [B]
         """
         indices = self.normalize_indices(indices)
-        tokens = tf.gather_nd(self.tokens, tf.expand_dims(indices, axis=-1))
-        with tf.device("/CPU:0"):  # string data is not supported on GPU
-            tokens = tf.strings.reduce_join(tokens, axis=-1)
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
+        tokens = self.detokenizer.lookup(indices)
+        tokens = tf.strings.reduce_join(tokens, axis=-1)
         return tokens
 
     @tf.function(input_signature=[tf.TensorSpec([None], dtype=tf.int32)])
-    def indices2upoints(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+    def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Transform Predicted Indices to Unicode Code Points (for using tflite)
         Args:
             indices: tf.Tensor of Classes in shape [None]
 
         Returns:
             unicode code points transcript with dtype tf.int32 and shape [None]
         """
         with tf.name_scope("indices2upoints"):
             indices = self.normalize_indices(indices)
             upoints = tf.gather_nd(self.upoints, tf.expand_dims(indices, axis=-1))
             return tf.gather_nd(upoints, tf.where(tf.not_equal(upoints, 0)))
 
 
-class SubwordFeaturizer(TextFeaturizer):
-    """
-    Extract text feature based on char-level granularity.
-    By looking up the vocabulary table, each line of transcript will be
-    converted to a sequence of integer indexes.
-    """
-
-    def __init__(
-        self,
-        decoder_config: dict,
-        subwords=None,
-    ):
-        """
-        decoder_config = {
-            "target_vocab_size": int,
-            "max_subword_length": 4,
-            "max_corpus_chars": None,
-            "reserved_tokens": None,
-            "beam_width": int,
-            "lm_config": {
-                ...
-            }
-        }
-        """
-        super(SubwordFeaturizer, self).__init__(decoder_config)
-        self.subwords = self.__load_subwords() if subwords is None else subwords
-        self.blank = 0  # subword treats blank as 0
-        self.num_classes = self.subwords.vocab_size
-        # create upoints
-        self.__init_vocabulary()
+class SentencePieceTokenizer(Tokenizer):
+    def __init__(self, decoder_config: DecoderConfig):
+        super().__init__(decoder_config)
+        self.blank = self.decoder_config.blank_index
+        self.tokenizer = tft.FastSentencepieceTokenizer(self.__load_model(), reverse=False, add_bos=False, add_eos=False)
+        self.num_classes = int(self.tokenizer.vocab_size())
 
-    def __init_vocabulary(self):
-        self.tokens = []
-        for idx in np.arange(1, self.num_classes, dtype=np.int32):
-            self.tokens.append(self.subwords.decode([idx]))
-        self.non_blank_tokens = self.tokens.copy()
-        self.tokens.insert(0, "")
-        self.upoints = tf.strings.unicode_decode(self.tokens, "UTF-8")
-        self.upoints = self.upoints.to_tensor()  # [num_classes, max_subword_length]
-
-    def __load_subwords(self):
-        filename_prefix = os.path.splitext(self.decoder_config.vocabulary)[0]
-        return tds.deprecated.text.SubwordTextEncoder.load_from_file(filename_prefix)
+    def __load_model(self):
+        with file_util.read_file(self.decoder_config.vocabulary) as path:
+            with open(path, "rb") as f:
+                return f.read()
 
     @classmethod
-    def build_from_corpus(
-        cls,
-        decoder_config: dict,
-        corpus_files: list = None,
-    ):
-        dconf = DecoderConfig(decoder_config.copy())
-        corpus_files = dconf.corpus_files if corpus_files is None or len(corpus_files) == 0 else corpus_files
+    def build_from_corpus(cls, decoder_config: DecoderConfig):
+        if os.path.exists(decoder_config.vocabulary):
+            return cls(decoder_config)
 
-        def corpus_generator():
-            for file in corpus_files:
-                with open(file, "r", encoding="utf-8") as f:
-                    lines = f.read().splitlines()
-                    lines = lines[1:]
-                for line in lines:
-                    line = line.split("\t")
-                    yield line[-1]
-
-        subwords = tds.deprecated.text.SubwordTextEncoder.build_from_corpus(
-            corpus_generator(),
-            dconf.target_vocab_size,
-            dconf.max_subword_length,
-            dconf.max_corpus_chars,
-            dconf.reserved_tokens,
+        sp.SentencePieceTrainer.Train(
+            sentence_iterator=cls.corpus_generator(decoder_config),
+            model_prefix=os.path.splitext(decoder_config.vocabulary)[0],
+            model_type=decoder_config.model_type,
+            vocab_size=decoder_config.vocab_size,
+            hard_vocab_limit=True,
+            unk_id=decoder_config.unknown_index,
+            bos_id=decoder_config.bos_index,
+            eos_id=decoder_config.eos_index,
+            pad_id=decoder_config.pad_index,
+            character_coverage=decoder_config.character_coverage,
+            unk_surface="",  # change default unk surface U+2047("⁇") by ""
+            allow_whitespace_only_pieces=False,
+            split_by_whitespace=(not decoder_config.keep_whitespace),
+            treat_whitespace_as_suffix=False,
+            user_defined_symbols="",
+            max_sentencepiece_length=decoder_config.max_sentencepiece_length,
+            max_sentence_length=decoder_config.max_sentence_length,  # bytes
+            remove_extra_whitespaces=True,
+            num_threads=multiprocessing.cpu_count(),
         )
-        return cls(decoder_config, subwords)
-
-    @classmethod
-    def load_from_file(
-        cls,
-        decoder_config: dict,
-        filename: str = None,
-    ):
-        dconf = DecoderConfig(decoder_config.copy())
-        filename = dconf.vocabulary if filename is None else file_util.preprocess_paths(filename)
-        filename_prefix = os.path.splitext(filename)[0]
-        subwords = tds.deprecated.text.SubwordTextEncoder.load_from_file(filename_prefix)
-        return cls(decoder_config, subwords)
 
-    def save_to_file(
-        self,
-        filename: str = None,
-    ):
-        filename = self.decoder_config.vocabulary if filename is None else file_util.preprocess_paths(filename)
-        filename_prefix = os.path.splitext(filename)[0]
-        return self.subwords.save_to_file(filename_prefix)
+        return cls(decoder_config)
 
-    def extract(
-        self,
-        text: str,
-    ) -> tf.Tensor:
-        """
-        Convert string to a list of integers
-        Args:
-            text: string (sequence of characters)
+    def tokenize(self, text: tf.Tensor) -> tf.Tensor:
+        text = self.normalize_text(text, self.decoder_config.normalization_form)
+        indices = self.tokenizer.tokenize(text)
+        indices = tf.cast(indices, tf.int32)
+        return indices
 
-        Returns:
-            sequence of ints in tf.Tensor
-        """
-        text = self.preprocess_text(text)
-        text = text.strip()  # remove trailing space
-        indices = self.subwords.encode(text)
-        return tf.convert_to_tensor(indices, dtype=tf.int32)
-
-    def iextract(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+    def detokenize(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Convert list of indices to string
         Args:
             indices: tf.Tensor with dim [B, None]
 
         Returns:
             transcripts: tf.Tensor of dtype tf.string with dim [B]
         """
-        with tf.device("/CPU:0"):  # string data is not supported on GPU
-            total = tf.shape(indices)[0]
-            batch = tf.constant(0, dtype=tf.int32)
-            transcripts = tf.TensorArray(
-                dtype=tf.string,
-                size=total,
-                dynamic_size=False,
-                infer_shape=False,
-                clear_after_read=False,
-                element_shape=tf.TensorShape([]),
-            )
-
-            def cond(batch, total, _):
-                return tf.less(batch, total)
-
-            def body(batch, total, transcripts):
-                norm_indices = self.normalize_indices(indices[batch])
-                norm_indices = tf.gather_nd(norm_indices, tf.where(tf.not_equal(norm_indices, 0)))
-                decoded = tf.numpy_function(self.subwords.decode, inp=[norm_indices], Tout=tf.string)
-                transcripts = transcripts.write(batch, decoded)
-                return batch + 1, total, transcripts
-
-            _, _, transcripts = tf.while_loop(cond, body, loop_vars=[batch, total, transcripts])
-
-            return transcripts.stack()
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.unknown_index))
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.bos_index))
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.eos_index))
+        transcripts = self.tokenizer.detokenize(indices)
+        transcripts = tf.strings.regex_replace(transcripts, r" +", " ")
+        return transcripts
 
     @tf.function(input_signature=[tf.TensorSpec([None], dtype=tf.int32)])
-    def indices2upoints(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+    def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Transform Predicted Indices to Unicode Code Points (for using tflite)
         Args:
             indices: tf.Tensor of Classes in shape [None]
 
         Returns:
             unicode code points transcript with dtype tf.int32 and shape [None]
         """
         with tf.name_scope("indices2upoints"):
-            indices = self.normalize_indices(indices)
-            upoints = tf.gather_nd(self.upoints, tf.expand_dims(indices, axis=-1))
-            return tf.gather_nd(upoints, tf.where(tf.not_equal(upoints, 0)))
-
-
-class SentencePieceFeaturizer(TextFeaturizer):
-    """
-    Extract text feature based on sentence piece package.
-    """
-
-    UNK_TOKEN, UNK_TOKEN_ID = "<unk>", 1
-    BOS_TOKEN, BOS_TOKEN_ID = "<s>", 2
-    EOS_TOKEN, EOS_TOKEN_ID = "</s>", 3
-    PAD_TOKEN, PAD_TOKEN_ID = "<pad>", 0  # unused, by default
-
-    def __init__(
-        self,
-        decoder_config: dict,
-        model=None,
-    ):
-        super(SentencePieceFeaturizer, self).__init__(decoder_config)
-        self.model = self.__load_model() if model is None else model
-        self.blank = 0  # treats blank as 0 (pad)
-        # vocab size
-        self.num_classes = self.model.get_piece_size()
-        self.__init_vocabulary()
-
-    def __load_model(self):
-        filename_prefix = os.path.splitext(self.decoder_config.vocabulary)[0]
-        processor = sp.SentencePieceProcessor()
-        processor.load(filename_prefix + ".model")
-        return processor
-
-    def __init_vocabulary(self):
-        self.tokens = []
-        for idx in range(1, self.num_classes):
-            self.tokens.append(self.model.decode_ids([idx]))
-        self.non_blank_tokens = self.tokens.copy()
-        self.tokens.insert(0, "")
-        self.upoints = tf.strings.unicode_decode(self.tokens, "UTF-8")
-        self.upoints = self.upoints.to_tensor()  # [num_classes, max_subword_length]
+            transcripts = self.detokenize(tf.reshape(indices, [1, -1]))
+            upoints = tf.strings.unicode_decode(transcripts, "UTF-8").to_tensor()
+            return tf.reshape(upoints, [-1])
+
+
+class WordPieceTokenizer(Tokenizer):
+    def __init__(self, decoder_config: DecoderConfig):
+        super().__init__(decoder_config)
+        self.blank = self.decoder_config.blank_index  # treat [PAD] as blank
+        self.vocab = None
+        with tf.io.gfile.GFile(self.decoder_config.vocabulary, "r") as voc:
+            self.vocab = voc.read().splitlines()
+        if not self.vocab:
+            raise ValueError("Unable to read vocabulary")
+        self.tokenizer = tft.FastWordpieceTokenizer(
+            vocab=self.vocab,
+            token_out_type=tf.int32,
+            unknown_token=self.decoder_config.unknown_token,
+            no_pretokenization=True,  # False is limited, so we manually do pretokenization
+            support_detokenization=True,
+        )
+        self.num_classes = len(self.vocab)
 
     @classmethod
-    def build_from_corpus(
-        cls,
-        decoder_config: dict,
-    ):
-        """
-        --model_prefix: output model name prefix. <model_name>.model and <model_name>.vocab are generated.
-        --vocab_size: vocabulary size, e.g., 8000, 16000, or 32000
-        --model_type: model type. Choose from unigram (default), bpe, char, or word.
-        The input sentence must be pretokenized when using word type."""
-        decoder_cfg = DecoderConfig(decoder_config)
-        # Train SentencePiece Model
-
-        def corpus_iterator():
-            for file in decoder_cfg.corpus_files:
-                with open(file, "r", encoding="utf-8") as f:
-                    lines = f.read().splitlines()
-                    lines = lines[1:]
-                for line in lines:
-                    line = line.split("\t")
-                    yield line[-1]
-
-        sp.SentencePieceTrainer.Train(
-            sentence_iterator=corpus_iterator(),
-            model_prefix=decoder_cfg.output_path_prefix,
-            model_type=decoder_cfg.model_type,
-            vocab_size=decoder_cfg.target_vocab_size,
-            num_threads=cpu_count(),
-            unk_id=cls.UNK_TOKEN_ID,
-            bos_id=cls.BOS_TOKEN_ID,
-            eos_id=cls.EOS_TOKEN_ID,
-            pad_id=cls.PAD_TOKEN_ID,
-            unk_surface="__UNKNOWN__",  # change default unk surface U+2047("⁇") by "__UNKNOWN__"
+    def build_from_corpus(cls, decoder_config: DecoderConfig):
+        if os.path.exists(decoder_config.vocabulary):
+            return cls(decoder_config)
+
+        def generator():
+            for data in cls.corpus_generator(decoder_config):
+                yield data
+
+        def write_vocab_file(filepath, vocab):
+            with tf.io.gfile.GFile(filepath, "w") as f:
+                for token in vocab:
+                    print(token, file=f)
+
+        dataset = tf.data.Dataset.from_generator(generator, output_signature=tf.TensorSpec(shape=(), dtype=tf.string)).batch(1000).prefetch(2)
+        vocab = bert_vocab.bert_vocab_from_dataset(
+            dataset,
+            vocab_size=decoder_config.vocab_size,
+            reserved_tokens=decoder_config.reserved_tokens,
+            bert_tokenizer_params={
+                "lower_case": False,  # keep original from dataset
+                "keep_whitespace": decoder_config.keep_whitespace,
+                "normalization_form": decoder_config.normalization_form,
+                "preserve_unused_token": False,
+            },
+            learn_params={
+                "max_token_length": decoder_config.max_token_length,
+                "max_unique_chars": decoder_config.max_unique_chars,
+                "num_iterations": decoder_config.num_iterations,
+            },
         )
-        # Export fairseq dictionary
-        processor = sp.SentencePieceProcessor()
-        processor.Load(decoder_cfg.output_path_prefix + ".model")
-        vocab = {i: processor.IdToPiece(i) for i in range(processor.GetPieceSize())}
-        assert (
-            vocab.get(cls.UNK_TOKEN_ID) == cls.UNK_TOKEN
-            and vocab.get(cls.BOS_TOKEN_ID) == cls.BOS_TOKEN
-            and vocab.get(cls.EOS_TOKEN_ID) == cls.EOS_TOKEN
-        )
-        vocab = {i: s for i, s in vocab.items() if s not in {cls.UNK_TOKEN, cls.BOS_TOKEN, cls.EOS_TOKEN, cls.PAD_TOKEN}}
-        with open(decoder_cfg.output_path_prefix + ".txt", "w") as f_out:
-            for _, s in sorted(vocab.items(), key=lambda x: x[0]):
-                f_out.write(f"{s} 1\n")
+        write_vocab_file(decoder_config.vocabulary, vocab)
 
-        return cls(decoder_config, processor)
+        return cls(decoder_config)
 
-    @classmethod
-    def load_from_file(
-        cls,
-        decoder_config: dict,
-        filename: str = None,
-    ):
-        if filename is not None:
-            filename_prefix = os.path.splitext(file_util.preprocess_paths(filename))[0]
+    def tokenize(self, text: tf.Tensor) -> tf.Tensor:
+        text = self.normalize_text(text, self.decoder_config.normalization_form)
+        if self.decoder_config.keep_whitespace:
+            text = tf.strings.regex_replace(text, " ", "| |")
+            text = tf.strings.split(text, sep="|")
         else:
-            filename_prefix = decoder_config.get("output_path_prefix", None)
-        processor = sp.SentencePieceProcessor()
-        processor.load(filename_prefix + ".model")
-        return cls(decoder_config, processor)
-
-    def extract(
-        self,
-        text: str,
-    ) -> tf.Tensor:
-        """
-        Convert string to a list of integers
-        # encode: text => id
-        sp.encode_as_pieces('This is a test') --> ['▁This', '▁is', '▁a', '▁t', 'est']
-        sp.encode_as_ids('This is a test') --> [209, 31, 9, 375, 586]
-        Args:
-            text: string (sequence of characters)
+            text = tf.strings.split(text)
+        indices = self.tokenizer.tokenize(text).merge_dims(0, 1)
+        return indices
 
-        Returns:
-            sequence of ints in tf.Tensor
-        """
-        text = self.preprocess_text(text)
-        text = text.strip()  # remove trailing space
-        indices = self.model.encode_as_ids(text)
-        return tf.convert_to_tensor(indices, dtype=tf.int32)
-
-    def iextract(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+    def detokenize(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Convert list of indices to string
-        # decode: id => text
-        sp.decode_pieces(['▁This', '▁is', '▁a', '▁t', 'est']) --> This is a test
-        sp.decode_ids([209, 31, 9, 375, 586]) --> This is a test
-
         Args:
             indices: tf.Tensor with dim [B, None]
 
         Returns:
             transcripts: tf.Tensor of dtype tf.string with dim [B]
         """
-        indices = self.normalize_indices(indices)
-        with tf.device("/CPU:0"):  # string data is not supported on GPU
-
-            def decode(x):
-                if x[0] == self.blank:
-                    x = x[1:]
-                return self.model.decode_ids(x.tolist())
-
-            text = tf.map_fn(
-                lambda x: tf.numpy_function(decode, inp=[x], Tout=tf.string),
-                indices,
-                fn_output_signature=tf.TensorSpec([], dtype=tf.string),
-            )
-        return text
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
+        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.unknown_index))
+        transcripts = self.tokenizer.detokenize(indices)
+        transcripts = tf.strings.regex_replace(transcripts, r" +", " ")
+        return transcripts
 
     @tf.function(input_signature=[tf.TensorSpec([None], dtype=tf.int32)])
-    def indices2upoints(
-        self,
-        indices: tf.Tensor,
-    ) -> tf.Tensor:
+    def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Transform Predicted Indices to Unicode Code Points (for using tflite)
         Args:
             indices: tf.Tensor of Classes in shape [None]
 
         Returns:
             unicode code points transcript with dtype tf.int32 and shape [None]
         """
         with tf.name_scope("indices2upoints"):
-            indices = self.normalize_indices(indices)
-            upoints = tf.gather_nd(self.upoints, tf.expand_dims(indices, axis=-1))
-            return tf.gather_nd(upoints, tf.where(tf.not_equal(upoints, 0)))
+            transcripts = self.detokenize(tf.reshape(indices, [1, -1]))
+            upoints = tf.strings.unicode_decode(transcripts, "UTF-8").to_tensor()
+            return tf.reshape(upoints, [-1])
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/losses/rnnt_loss.py` & `TensorFlowASR-2.0.0/tensorflow_asr/losses/rnnt_loss.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,129 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit) and M. Yusuf Sarıgöz (@monatis)
+# pylint: disable=no-name-in-module,unexpected-keyword-arg,no-value-for-parameter
+# Copyright 2020 Huy Le Nguyen (@nglehuy) and M. Yusuf Sarıgöz (@monatis)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # RNNT loss implementation in pure TensorFlow is borrowed from [iamjanvijay's repo](https://github.com/iamjanvijay/rnnt)
 
-import tensorflow as tf
-from tensorflow.python.ops.gen_array_ops import matrix_diag_part_v2
+import importlib.util
+import os
 
-from tensorflow_asr.utils import env_util
+import numpy as np
+import tensorflow as tf
 
-logger = tf.get_logger()
+from tensorflow_asr.utils import env_util, math_util, shape_util
 
-LOG_0 = float("-inf")
+warp_rnnt_loss = importlib.import_module("warprnnt_tensorflow").rnnt_loss if importlib.util.find_spec("warprnnt_tensorflow") is not None else None
 
-try:
-    from warprnnt_tensorflow import rnnt_loss as warp_rnnt_loss
+USE_CPU_LOSS = os.getenv("USE_CPU_LOSS", "False") == "True"
 
-    use_warprnnt = True
-    logger.info("Use RNNT loss in WarpRnnt")
-except ImportError:
-    logger.info("Use RNNT loss in TensorFlow")
-    use_warprnnt = False
+logger = tf.get_logger()
 
 
 class RnntLoss(tf.keras.losses.Loss):
     def __init__(
         self,
-        blank=0,
-        global_batch_size=None,
+        blank,
+        reduction=tf.keras.losses.Reduction.AUTO,
+        output_shapes=None,
         name=None,
     ):
-        super(RnntLoss, self).__init__(reduction=tf.keras.losses.Reduction.NONE, name=name)
+        if blank != 0 and warp_rnnt_loss is None:  # restrict blank index
+            raise ValueError("RNNT loss in tensorflow must use blank = 0")
+        super().__init__(reduction=reduction, name=name)
         self.blank = blank
-        self.global_batch_size = global_batch_size
+        self.use_cpu = USE_CPU_LOSS or (not env_util.has_devices("GPU") and not env_util.has_devices("TPU"))
+        self.output_shapes = output_shapes
+        # fmt: off
+        logger.info(f"[RNNT loss] Use {'CPU' if self.use_cpu else 'GPU/TPU'} implementation in {'Tensorflow' if warp_rnnt_loss is None else 'WarpRNNT'}") # pylint: disable=line-too-long
+        # fmt: on
+        if self.output_shapes:
+            logger.info(f"[RNNT loss] Use model's output shapes: {self.output_shapes}")
+            if not all(self.output_shapes):
+                logger.info("[RNNT loss] Detected dynamic shape")
+                self.output_shapes = None
 
     def call(self, y_true, y_pred):
-        loss = rnnt_loss(
-            logits=y_pred["logits"],
-            logit_length=y_pred["logits_length"],
-            labels=y_true["labels"],
-            label_length=y_true["labels_length"],
+        return rnnt_loss(
+            logits=y_pred,
+            logits_length=math_util.compute_time_length(y_pred) if env_util.LENGTH_AS_OUTPUT else y_pred._keras_length,
+            labels=y_true,
+            labels_length=math_util.compute_time_length(y_true) if env_util.LENGTH_AS_OUTPUT else y_true._keras_length,
             blank=self.blank,
             name=self.name,
+            use_cpu=self.use_cpu,
+            output_shapes=self.output_shapes,
         )
-        return tf.nn.compute_average_loss(loss, global_batch_size=self.global_batch_size)
 
 
-@tf.function
 def rnnt_loss(
     logits,
+    logits_length,
     labels,
-    label_length,
-    logit_length,
+    labels_length,
     blank=0,
     name=None,
+    use_cpu=False,
+    output_shapes=None,
 ):
-    if use_warprnnt:
-        return rnnt_loss_warprnnt(
-            logits=logits, labels=labels, label_length=label_length, logit_length=logit_length, blank=blank
-        )
-    else:
-        return rnnt_loss_tf(
-            logits=logits,
-            labels=labels,
-            label_length=label_length,
-            logit_length=logit_length,
-            name=name,
-        )
+    kwargs = dict(
+        logits=logits,
+        labels=labels,
+        label_length=labels_length,
+        logit_length=logits_length,
+        blank=blank,
+        use_cpu=use_cpu,
+        output_shapes=output_shapes,
+        name=name,
+    )
+    loss_fn = rnnt_loss_tf if warp_rnnt_loss is None else rnnt_loss_warprnnt
+    if use_cpu:
+        with tf.device("/CPU:0"):
+            return loss_fn(**kwargs)
+    return loss_fn(**kwargs)
+
+
+# ------------------------ RNNT LOSS IN WARP TRANDUCER ----------------------- #
 
 
 def rnnt_loss_warprnnt(
     logits,
     labels,
     label_length,
     logit_length,
     blank=0,
+    use_cpu=False,
+    **kwargs,
 ):
-    if not env_util.has_devices(["GPU", "TPU"]):
+    orig_dtype = logits.dtype
+    if orig_dtype in (tf.float16, tf.bfloat16):
+        logits = tf.cast(logits, tf.float32)
+    if use_cpu:
         logits = tf.nn.log_softmax(logits)
-    loss = warp_rnnt_loss(
-        acts=tf.cast(logits, tf.float32),
-        label_lengths=tf.cast(label_length, tf.int32),
-        labels=tf.cast(labels, tf.int32),
-        input_lengths=tf.cast(logit_length, tf.int32),
-        blank_label=blank,
-    )
+    loss = warp_rnnt_loss(acts=logits, label_lengths=label_length, labels=labels, input_lengths=logit_length, blank_label=blank)
+    if orig_dtype in (tf.float16, tf.bfloat16):
+        loss = tf.cast(loss, orig_dtype)
     return loss
 
 
+# ------------------------------ RNNT LOSS IN TF ----------------------------- #
+
+LOG_0 = -np.inf
+
+
 def nan_to_zero(
     input_tensor,
 ):
     return tf.where(tf.math.is_nan(input_tensor), tf.zeros_like(input_tensor), input_tensor)
 
 
 def reduce_logsumexp(
@@ -116,19 +139,15 @@
     log_probs,
 ):
     time_steps = tf.shape(log_probs)[1]  # T
     output_steps = tf.shape(log_probs)[2]  # U + 1
     reverse_log_probs = tf.reverse(log_probs, axis=[-1])
     paddings = [[0, 0], [0, 0], [time_steps - 1, 0]]
     padded_reverse_log_probs = tf.pad(reverse_log_probs, paddings, "CONSTANT", constant_values=LOG_0)
-    diagonals = matrix_diag_part_v2(
-        padded_reverse_log_probs,
-        k=(0, time_steps + output_steps - 2),
-        padding_value=LOG_0,
-    )
+    diagonals = tf.raw_ops.MatrixDiagPartV2(input=padded_reverse_log_probs, k=(0, time_steps + output_steps - 2), padding_value=LOG_0)
 
     return tf.transpose(diagonals, perm=[1, 0, 2])
 
 
 def transition_probs(
     one_hot_labels,
     log_probs,
@@ -160,26 +179,20 @@
 
         x_b = tf.concat([LOG_0 * tf.ones(shape=[batch_size, 1]), x[:, :-1] + blank_probs], axis=1)
         x_t = x + truth_probs
 
         x = tf.math.reduce_logsumexp(tf.stack([x_b, x_t], axis=0), axis=0)
         return x
 
-    initial_alpha = tf.concat(
-        [
-            tf.zeros(shape=[batch_size, 1]),
-            tf.ones(shape=[batch_size, input_max_len - 1]) * LOG_0,
-        ],
-        axis=1,
-    )
+    initial_alpha = tf.concat([tf.zeros(shape=[batch_size, 1]), tf.ones(shape=[batch_size, input_max_len - 1]) * LOG_0], axis=1)
 
     fwd = tf.scan(next_state, (bp_diags[:-1, :, :-1], tp_diags), initializer=initial_alpha)
 
     alpha = tf.transpose(tf.concat([tf.expand_dims(initial_alpha, axis=0), fwd], axis=0), perm=[1, 2, 0])
-    alpha = matrix_diag_part_v2(alpha, k=(0, target_max_len - 1), padding_value=LOG_0)
+    alpha = tf.raw_ops.MatrixDiagPartV2(input=alpha, k=(0, target_max_len - 1), padding_value=LOG_0)
     alpha = tf.transpose(tf.reverse(alpha, axis=[1]), perm=[0, 2, 1])
 
     return alpha
 
 
 def backward_dp(
     bp_diags,
@@ -198,210 +211,169 @@
     def next_state(x, mask_and_trans_probs):
         mask_s, blank_probs_s, truth_probs = mask_and_trans_probs
 
         beta_b = tf.concat([x[:, 1:] + blank_probs_s, LOG_0 * tf.ones(shape=[batch_size, 1])], axis=1)
         beta_t = tf.concat([x[:, :-1] + truth_probs, LOG_0 * tf.ones(shape=[batch_size, 1])], axis=1)
 
         beta_next = reduce_logsumexp(tf.stack([beta_b, beta_t], axis=0), axis=0)
-        masked_beta_next = nan_to_zero(beta_next * tf.expand_dims(mask_s, axis=1)) + nan_to_zero(
-            x * tf.expand_dims((1.0 - mask_s), axis=1)
-        )
-        return tf.reshape(masked_beta_next, shape=tf.shape(x))
+        masked_beta_next = nan_to_zero(beta_next * tf.expand_dims(mask_s, axis=1)) + nan_to_zero(x * tf.expand_dims((1.0 - mask_s), axis=1))
+        return tf.ensure_shape(masked_beta_next, x.shape)
 
     # Initial beta for batches.
     initial_beta_mask = tf.one_hot(logit_length - 1, depth=input_max_len + 1)
     initial_beta = tf.expand_dims(blank_sl, axis=1) * initial_beta_mask + nan_to_zero(LOG_0 * (1.0 - initial_beta_mask))
 
     # Mask for scan iterations.
-    mask = tf.sequence_mask(
-        logit_length + label_length - 1,
-        input_max_len + target_max_len - 2,
-        dtype=tf.dtypes.float32,
-    )
+    mask = tf.sequence_mask(logit_length + label_length - 1, input_max_len + target_max_len - 2, dtype=tf.dtypes.float32)
     mask = tf.transpose(mask, perm=[1, 0])
 
-    bwd = tf.scan(
-        next_state,
-        (mask, bp_diags[:-1, :, :], tp_diags),
-        initializer=initial_beta,
-        reverse=True,
-    )
+    bwd = tf.scan(next_state, (mask, bp_diags[:-1, :, :], tp_diags), initializer=initial_beta, reverse=True)
 
     beta = tf.transpose(tf.concat([bwd, tf.expand_dims(initial_beta, axis=0)], axis=0), perm=[1, 2, 0])[:, :-1, :]
-    beta = matrix_diag_part_v2(beta, k=(0, target_max_len - 1), padding_value=LOG_0)
+    beta = tf.raw_ops.MatrixDiagPartV2(input=beta, k=(0, target_max_len - 1), padding_value=LOG_0)
     beta = tf.transpose(tf.reverse(beta, axis=[1]), perm=[0, 2, 1])
 
     return beta
 
 
-def compute_rnnt_loss_and_grad_helper(logits, labels, label_length, logit_length):
-    batch_size = tf.shape(logits)[0]
-    input_max_len = tf.shape(logits)[1]
-    target_max_len = tf.shape(logits)[2]
-    vocab_size = tf.shape(logits)[3]
-
-    one_hot_labels = tf.one_hot(
-        tf.tile(tf.expand_dims(labels, axis=1), multiples=[1, input_max_len, 1]),
-        depth=vocab_size,
-    )
+def compute_rnnt_loss_and_grad_helper(
+    logits,
+    labels,
+    label_length,
+    logit_length,
+    use_cpu=False,
+    output_shapes=None,
+):
+    if output_shapes is None:  # dynamic shape
+        batch_size = shape_util.get_dim(logits, 0)
+        input_max_len = shape_util.get_dim(logits, 1)
+        target_max_len = shape_util.get_dim(logits, 2)
+        vocab_size = shape_util.get_dim(logits, 3)
+    else:
+        batch_size = output_shapes["logits"][0]
+        input_max_len = output_shapes["logits"][1]
+        target_max_len = output_shapes["logits"][2]
+        vocab_size = output_shapes["logits"][3]
+
+    one_hot_labels = tf.one_hot(tf.tile(tf.expand_dims(labels, axis=1), multiples=[1, input_max_len, 1]), depth=vocab_size)
 
     log_probs = tf.nn.log_softmax(logits)
     blank_probs, truth_probs = transition_probs(one_hot_labels, log_probs)
     bp_diags = extract_diagonals(blank_probs)
     tp_diags = extract_diagonals(truth_probs)
 
-    label_mask = tf.expand_dims(
-        tf.sequence_mask(label_length + 1, maxlen=target_max_len, dtype=tf.float32),
-        axis=1,
-    )
+    label_mask = tf.expand_dims(tf.sequence_mask(label_length + 1, maxlen=target_max_len, dtype=tf.float32), axis=1)
     small_label_mask = tf.expand_dims(tf.sequence_mask(label_length, maxlen=target_max_len, dtype=tf.float32), axis=1)
     input_mask = tf.expand_dims(tf.sequence_mask(logit_length, maxlen=input_max_len, dtype=tf.float32), axis=2)
-    small_input_mask = tf.expand_dims(
-        tf.sequence_mask(logit_length - 1, maxlen=input_max_len, dtype=tf.float32),
-        axis=2,
-    )
+    small_input_mask = tf.expand_dims(tf.sequence_mask(logit_length - 1, maxlen=input_max_len, dtype=tf.float32), axis=2)
     mask = label_mask * input_mask
     grad_blank_mask = (label_mask * small_input_mask)[:, :-1, :]
     grad_truth_mask = (small_label_mask * input_mask)[:, :, :-1]
 
     alpha = forward_dp(bp_diags, tp_diags, batch_size, input_max_len, target_max_len) * mask
 
     indices = tf.stack([logit_length - 1, label_length], axis=1)
     blank_sl = tf.gather_nd(blank_probs, indices, batch_dims=1)
 
-    beta = (
-        backward_dp(
-            bp_diags,
-            tp_diags,
-            batch_size,
-            input_max_len,
-            target_max_len,
-            label_length,
-            logit_length,
-            blank_sl,
-        )
-        * mask
-    )
-    beta = tf.where(tf.math.is_nan(beta), tf.zeros_like(beta), beta)
+    beta = backward_dp(bp_diags, tp_diags, batch_size, input_max_len, target_max_len, label_length, logit_length, blank_sl) * mask
     final_state_probs = beta[:, 0, 0]
+    beta = nan_to_zero(beta)
 
     # Compute gradients of loss w.r.t. blank log-probabilities.
     grads_blank = (
         -tf.exp(
-            (
-                alpha[:, :-1, :]
-                + beta[:, 1:, :]
-                - tf.reshape(final_state_probs, shape=[batch_size, 1, 1])
-                + blank_probs[:, :-1, :]
-            )
-            * grad_blank_mask
+            (alpha[:, :-1, :] + beta[:, 1:, :] - tf.reshape(final_state_probs, shape=[batch_size, 1, 1]) + blank_probs[:, :-1, :]) * grad_blank_mask
         )
         * grad_blank_mask
     )
     grads_blank = tf.concat([grads_blank, tf.zeros(shape=(batch_size, 1, target_max_len))], axis=1)
     last_grads_blank = -1 * tf.scatter_nd(
-        tf.concat(
-            [
-                tf.reshape(tf.range(batch_size, dtype=tf.int64), shape=[batch_size, 1]),
-                tf.cast(indices, dtype=tf.int64),
-            ],
-            axis=1,
-        ),
+        tf.concat([tf.reshape(tf.range(batch_size, dtype=tf.int64), shape=[batch_size, 1]), tf.cast(indices, dtype=tf.int64)], axis=1),
         tf.ones(batch_size, dtype=tf.float32),
         [batch_size, input_max_len, target_max_len],
+        name="last_grads_blank_scatter",
     )
     grads_blank = grads_blank + last_grads_blank
 
     # Compute gradients of loss w.r.t. truth log-probabilities.
     grads_truth = (
-        -tf.exp(
-            (alpha[:, :, :-1] + beta[:, :, 1:] - tf.reshape(final_state_probs, shape=[batch_size, 1, 1]) + truth_probs)
-            * grad_truth_mask
-        )
+        -tf.exp((alpha[:, :, :-1] + beta[:, :, 1:] - tf.reshape(final_state_probs, shape=[batch_size, 1, 1]) + truth_probs) * grad_truth_mask)
         * grad_truth_mask
     )
 
     # Compute gradients of loss w.r.t. activations.
-    a = tf.tile(
-        tf.reshape(
-            tf.range(target_max_len - 1, dtype=tf.int64),
-            shape=(1, 1, target_max_len - 1, 1),
-        ),
-        multiples=[batch_size, 1, 1, 1],
-    )
-    b = tf.cast(
-        tf.reshape(labels - 1, shape=(batch_size, 1, target_max_len - 1, 1)),
-        dtype=tf.int64,
-    )
-    if not env_util.has_devices(["GPU", "TPU"]):
+    a = tf.tile(tf.reshape(tf.range(target_max_len - 1, dtype=tf.int64), shape=(1, 1, target_max_len - 1, 1)), multiples=[batch_size, 1, 1, 1])
+    b = tf.cast(tf.reshape(labels - 1, shape=(batch_size, 1, target_max_len - 1, 1)), dtype=tf.int64)
+    if use_cpu:
         b = tf.where(tf.equal(b, -1), tf.zeros_like(b), b)  # for cpu testing (index -1 on cpu will raise errors)
     c = tf.concat([a, b], axis=3)
     d = tf.tile(c, multiples=(1, input_max_len, 1, 1))
-    e = tf.tile(
-        tf.reshape(tf.range(input_max_len, dtype=tf.int64), shape=(1, input_max_len, 1, 1)),
-        multiples=(batch_size, 1, target_max_len - 1, 1),
-    )
+    e = tf.tile(tf.reshape(tf.range(input_max_len, dtype=tf.int64), shape=(1, input_max_len, 1, 1)), multiples=(batch_size, 1, target_max_len - 1, 1))
     f = tf.concat([e, d], axis=3)
-    g = tf.tile(
-        tf.reshape(tf.range(batch_size, dtype=tf.int64), shape=(batch_size, 1, 1, 1)),
-        multiples=[1, input_max_len, target_max_len - 1, 1],
-    )
+    g = tf.tile(tf.reshape(tf.range(batch_size, dtype=tf.int64), shape=(batch_size, 1, 1, 1)), multiples=[1, input_max_len, target_max_len - 1, 1])
     scatter_idx = tf.concat([g, f], axis=3)
     # TODO - improve the part of code for scatter_idx computation.
     probs = tf.exp(log_probs)
     grads_truth_scatter = tf.scatter_nd(
         scatter_idx,
         grads_truth,
         [batch_size, input_max_len, target_max_len, vocab_size - 1],
+        name="grads_truth_scatter",
     )
-    grads = tf.concat(
-        [
-            tf.reshape(grads_blank, shape=(batch_size, input_max_len, target_max_len, -1)),
-            grads_truth_scatter,
-        ],
-        axis=3,
-    )
+    grads = tf.concat([tf.reshape(grads_blank, shape=(batch_size, input_max_len, target_max_len, -1)), grads_truth_scatter], axis=3)
     grads_logits = grads - probs * (tf.reduce_sum(grads, axis=3, keepdims=True))
 
     loss = -final_state_probs
     return loss, grads_logits
 
 
 def rnnt_loss_tf(
     logits,
     labels,
     label_length,
     logit_length,
     name=None,
+    use_cpu=False,
+    output_shapes=None,
+    **kwargs,
 ):
     name = "rnnt_loss" if name is None else name
     with tf.name_scope(name):
         logits = tf.convert_to_tensor(logits, name="logits")
         labels = tf.convert_to_tensor(labels, name="labels")
         label_length = tf.convert_to_tensor(label_length, name="label_length")
         logit_length = tf.convert_to_tensor(logit_length, name="logit_length")
 
+        orig_dtype = logits.dtype
+        if orig_dtype in (tf.float16, tf.bfloat16):
+            logits = tf.cast(logits, tf.float32)
+
         args = [logits, labels, label_length, logit_length]
 
         @tf.custom_gradient
         def compute_rnnt_loss_and_grad(logits_t, labels_t, label_length_t, logit_length_t):
             """Compute RNN-T loss and gradients."""
             logits_t.set_shape(logits.shape)
             labels_t.set_shape(labels.shape)
             label_length_t.set_shape(label_length.shape)
             logit_length_t.set_shape(logit_length.shape)
             kwargs = dict(
                 logits=logits_t,
                 labels=labels_t,
                 label_length=label_length_t,
                 logit_length=logit_length_t,
+                use_cpu=use_cpu,
+                output_shapes=output_shapes,
             )
             result = compute_rnnt_loss_and_grad_helper(**kwargs)
 
             def grad(grad_loss):
                 grads = [tf.reshape(grad_loss, [-1, 1, 1, 1]) * result[1]]
                 grads += [None] * (len(args) - len(grads))
                 return grads
 
             return result[0], grad
 
-        return compute_rnnt_loss_and_grad(*args)
+        loss = compute_rnnt_loss_and_grad(*args)
+        if orig_dtype in (tf.float16, tf.bfloat16):
+            loss = tf.cast(loss, orig_dtype)
+        return loss
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/metrics/error_rates.py` & `TensorFlowASR-2.0.0/tensorflow_asr/metrics/error_rates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,29 +14,19 @@
 
 import tensorflow as tf
 
 
 class ErrorRate(tf.keras.metrics.Metric):
     """Metric for WER or CER"""
 
-    def __init__(
-        self,
-        func,
-        name="error_rate",
-        **kwargs,
-    ):
-        super(ErrorRate, self).__init__(name=name, **kwargs)
-        self.numerator = self.add_weight(name=f"{name}_numerator", initializer="zeros")
-        self.denominator = self.add_weight(name=f"{name}_denominator", initializer="zeros")
-        self.func = func
-
-    def update_state(
-        self,
-        decode: tf.Tensor,
-        target: tf.Tensor,
-    ):
-        n, d = self.func(decode, target)
-        self.numerator.assign_add(n)
-        self.denominator.assign_add(d)
+    def __init__(self, name="error_rate", **kwargs):
+        super().__init__(name=name, **kwargs)
+        self.numerator = self.add_weight(name="numerator", initializer="zeros")
+        self.denominator = self.add_weight(name="denominator", initializer="zeros")
+
+    def update_state(self, data):
+        numer, denom = data
+        self.numerator.assign_add(tf.reduce_sum(numer))
+        self.denominator.assign_add(tf.reduce_sum(denom))
 
     def result(self):
-        return tf.math.divide_no_nan(self.numerator, self.denominator)
+        return tf.math.divide(self.numerator, self.denominator)
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/activations/glu.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/activations/glu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,31 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
+from tensorflow_asr.models.base_layer import Layer
 
-class GLU(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        axis=-1,
-        name="glu_activation",
-        **kwargs,
-    ):
-        super(GLU, self).__init__(name=name, **kwargs)
+
+class GLU(Layer):
+    def __init__(self, axis=-1, name="glu", **kwargs):
+        super().__init__(name=name, **kwargs)
         self.axis = axis
 
-    def call(
-        self,
-        inputs,
-        **kwargs,
-    ):
+    def call(self, inputs):
         a, b = tf.split(inputs, 2, axis=self.axis)
         b = tf.nn.sigmoid(b)
         return tf.multiply(a, b)
 
-    def get_config(self):
-        conf = super(GLU, self).get_config()
-        conf.update({"axis": self.axis})
-        return conf
+    def compute_output_shape(self, input_shape):
+        B, T, V = input_shape
+        return (B, T, V // 2)
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/base_ctc.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/rnnt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,227 +1,203 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+""" http://arxiv.org/abs/1811.06621 """
 
-from typing import Dict, Union
-import numpy as np
 import tensorflow as tf
 
-from tensorflow_asr.featurizers.speech_featurizers import TFSpeechFeaturizer
-from tensorflow_asr.featurizers.text_featurizers import TextFeaturizer
-from tensorflow_asr.losses.ctc_loss import CtcLoss
-from tensorflow_asr.utils import data_util, math_util, shape_util
-from tensorflow_asr.models.base_model import BaseModel
+from tensorflow_asr.models.base_layer import Layer, Reshape
+from tensorflow_asr.models.layers.subsampling import TimeReduction
+from tensorflow_asr.utils import layer_util, math_util
 
 
-class CtcModel(BaseModel):
+class RnnTransducerBlock(Layer):
     def __init__(
         self,
-        encoder: tf.keras.Model,
-        decoder: Union[tf.keras.Model, tf.keras.layers.Layer] = None,
-        vocabulary_size: int = None,
+        reduction_factor: int = 0,
+        dmodel: int = 640,
+        rnn_type: str = "lstm",
+        rnn_units: int = 2048,
+        rnn_unroll: bool = False,
+        layer_norm: bool = True,
+        kernel_regularizer=None,
+        bias_regularizer=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.encoder = encoder
-        if decoder is None:
-            assert vocabulary_size is not None, "vocabulary_size must be set"
-            self.decoder = tf.keras.layers.Dense(
-                units=vocabulary_size,
-                name=f"{self.name}_logits",
-            )
-        else:
-            self.decoder = decoder
-        self.time_reduction_factor = 1
-
-    def make(
-        self,
-        input_shape,
-        batch_size=None,
-    ):
-        inputs = tf.keras.Input(input_shape, batch_size=batch_size, dtype=tf.float32)
-        inputs_length = tf.keras.Input(shape=[], batch_size=batch_size, dtype=tf.int32)
-        self(
-            data_util.create_inputs(
-                inputs=inputs,
-                inputs_length=inputs_length,
-            ),
-            training=False,
+        self.reduction = TimeReduction(reduction_factor, name="reduction", dtype=self.dtype) if reduction_factor > 0 else None
+        self.rnn = layer_util.get_rnn(rnn_type)(
+            units=rnn_units,
+            return_sequences=True,
+            name=rnn_type,
+            unroll=rnn_unroll,
+            return_state=True,
+            zero_output_for_mask=True,
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            dtype=self.dtype,
         )
-
-    def summary(
-        self,
-        line_length=None,
-        **kwargs,
-    ):
-        self.encoder.summary(line_length=line_length, **kwargs)
-        super().summary(line_length=line_length, **kwargs)
-
-    def compile(
-        self,
-        optimizer,
-        global_batch_size,
-        blank=0,
-        run_eagerly=None,
-        **kwargs,
-    ):
-        loss = CtcLoss(blank=blank, global_batch_size=global_batch_size)
-        super().compile(loss=loss, optimizer=optimizer, run_eagerly=run_eagerly, **kwargs)
-
-    def add_featurizers(
-        self,
-        speech_featurizer: TFSpeechFeaturizer,
-        text_featurizer: TextFeaturizer,
-    ):
-        self.speech_featurizer = speech_featurizer
-        self.text_featurizer = text_featurizer
-
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        logits = self.encoder(inputs["inputs"], training=training, **kwargs)
-        logits = self.decoder(logits, training=training, **kwargs)
-        return data_util.create_logits(
-            logits=logits,
-            logits_length=math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor),
+        self.ln = (
+            tf.keras.layers.LayerNormalization(name="ln", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype)
+            if layer_norm
+            else None
+        )
+        self.projection = tf.keras.layers.Dense(
+            dmodel,
+            name="projection",
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            dtype=self.dtype,
         )
 
-    # -------------------------------- GREEDY -------------------------------------
-
-    @tf.function
-    def recognize(
-        self,
-        inputs: Dict[str, tf.Tensor],
-    ):
-        logits = self(inputs, training=False)
-        probs = tf.nn.softmax(logits["logits"])
-
-        def map_fn(prob):
-            return tf.numpy_function(self._perform_greedy, inp=[prob], Tout=tf.string)
-
-        return tf.map_fn(map_fn, probs, fn_output_signature=tf.TensorSpec([], dtype=tf.string))
-
-    def _perform_greedy(
-        self,
-        probs: np.ndarray,
-    ):
-        from ctc_decoders import ctc_greedy_decoder
-
-        decoded = ctc_greedy_decoder(probs, vocabulary=self.text_featurizer.non_blank_tokens)
-        return tf.convert_to_tensor(decoded, dtype=tf.string)
+    def call(self, inputs, training=False):
+        outputs, outputs_length = inputs
+        if self.reduction is not None:
+            outputs, outputs_length = self.reduction((outputs, outputs_length))
+        outputs, *_ = self.rnn(outputs, training=training)
+        if self.ln is not None:
+            outputs = self.ln(outputs, training=training)
+        outputs = self.projection(outputs, training=training)
+        return outputs, outputs_length
+
+    def compute_mask(self, inputs, mask=None):
+        if self.reduction is not None:
+            mask = self.reduction.compute_mask(inputs)
+        return mask
 
-    def recognize_tflite(
-        self,
-        signal,
-    ):
+    def call_next(self, inputs, inputs_length, previous_encoder_states):
         """
-        Function to convert to tflite using greedy decoding
-        Args:
-            signal: tf.Tensor with shape [None] indicating a single audio signal
+        Recognize function for encoder network from the previous encoder states
 
-        Return:
-            transcript: tf.Tensor of Unicode Code Points with shape [None] and dtype tf.int32
+        Parameters
+        ----------
+        inputs : tf.Tensor, shape [B, T, E]
+        previous_encoder_states : tf.Tensor, shape [nstates, B, rnn_units]
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor, tf.Tensor], shapes ([B, T, dmodel], [B], [nstates, B, rnn_units])
         """
-        features = self.speech_featurizer.tf_extract(signal)
-        features = tf.expand_dims(features, axis=0)
-        input_length = shape_util.shape_list(features)[1]
-        input_length = math_util.get_reduced_length(input_length, self.time_reduction_factor)
-        input_length = tf.expand_dims(input_length, axis=0)
-        logits = self.encoder(features, training=False)
-        logits = self.decoder(logits, training=False)
-        probs = tf.nn.softmax(logits)
-        decoded = tf.keras.backend.ctc_decode(y_pred=probs, input_length=input_length, greedy=True)
-        decoded = tf.cast(decoded[0][0][0], dtype=tf.int32)
-        transcript = self.text_featurizer.indices2upoints(decoded)
-        return transcript
-
-    # -------------------------------- BEAM SEARCH -------------------------------------
-
-    @tf.function
-    def recognize_beam(
-        self,
-        inputs: Dict[str, tf.Tensor],
-        lm: bool = False,
-    ):
-        logits = self(inputs, training=False)
-        probs = tf.nn.softmax(logits["logits"])
-
-        def map_fn(prob):
-            return tf.numpy_function(self._perform_beam_search, inp=[prob, lm], Tout=tf.string)
+        with tf.name_scope(f"{self.name}_call_next"):
+            outputs, outputs_length = inputs, inputs_length
+            outputs, *_states = self.rnn(
+                outputs,
+                training=False,
+                initial_state=tf.unstack(previous_encoder_states, axis=0),
+                mask=getattr(inputs, "_keras_mask", None),
+            )
+            new_states = tf.stack(_states, axis=0)
+            if self.ln is not None:
+                outputs = self.ln(outputs, training=False)
+            if self.reduction is not None:
+                outputs, outputs_length = self.reduction([outputs, outputs_length])
+            outputs = self.projection(outputs, training=False)
+            return outputs, outputs_length, new_states
+
+    def compute_output_shape(self, input_shape):
+        output_shape, output_length_shape = input_shape
+        if self.reduction is not None:
+            output_shape, output_length_shape = self.reduction.compute_output_shape((output_shape, output_length_shape))
+        output_shape = self.projection.compute_output_shape(output_shape)
+        return output_shape, output_length_shape
 
-        return tf.map_fn(map_fn, probs, dtype=tf.string)
 
-    def _perform_beam_search(
+class RnnTransducerEncoder(Layer):
+    def __init__(
         self,
-        probs: np.ndarray,
-        lm: bool = False,
+        reduction_factors: list = [6, 0, 0, 0, 0, 0, 0, 0],
+        dmodel: int = 640,
+        nlayers: int = 8,
+        rnn_type: str = "lstm",
+        rnn_units: int = 2048,
+        rnn_unroll: bool = False,
+        layer_norm: bool = True,
+        kernel_regularizer=None,
+        bias_regularizer=None,
+        **kwargs,
     ):
-        from ctc_decoders import ctc_beam_search_decoder
+        super().__init__(**kwargs)
+        assert len(reduction_factors) == nlayers, "reduction_factors length must be equal to nlayers"
+        self.reshape = Reshape(name="reshape", dtype=self.dtype)
 
-        decoded = ctc_beam_search_decoder(
-            probs_seq=probs,
-            vocabulary=self.text_featurizer.non_blank_tokens,
-            beam_size=self.text_featurizer.decoder_config.beam_width,
-            ext_scoring_func=self.text_featurizer.scorer if lm else None,
-        )
-        decoded = decoded[0][-1]
+        self.time_reduction_factor = 1
+        self.blocks = []
+        for i in range(nlayers):
+            block = RnnTransducerBlock(
+                reduction_factor=reduction_factors[i],
+                dmodel=dmodel,
+                rnn_type=rnn_type,
+                rnn_units=rnn_units,
+                rnn_unroll=rnn_unroll,
+                layer_norm=layer_norm,
+                kernel_regularizer=kernel_regularizer,
+                bias_regularizer=bias_regularizer,
+                name=f"block_{i}",
+                dtype=self.dtype,
+            )
+            self.blocks.append(block)
+            self.time_reduction_factor *= getattr(block.reduction, "time_reduction_factor", 1)
 
-        return tf.convert_to_tensor(decoded, dtype=tf.string)
+    def get_initial_state(self, batch_size=1):
+        """Get zeros states
 
-    def recognize_beam_tflite(
-        self,
-        signal,
-    ):
+        Returns:
+            tf.Tensor: states having shape [num_rnns, 1 or 2, 1, P]
         """
-        Function to convert to tflite using beam search decoding
-        Args:
-            signal: tf.Tensor with shape [None] indicating a single audio signal
+        states = []
+        for block in self.blocks:
+            states.append(tf.stack(block.rnn.get_initial_state(tf.zeros([batch_size, 1, 1], dtype=self.dtype)), axis=0))
+        return tf.stack(states, axis=0)
+
+    def call(self, inputs, training=False):
+        outputs, outputs_length, caching = inputs
+        outputs, outputs_length = self.reshape((outputs, outputs_length))
+        for block in self.blocks:
+            outputs, outputs_length = block((outputs, outputs_length), training=training)
+        return outputs, outputs_length, caching
 
-        Return:
-            transcript: tf.Tensor of Unicode Code Points with shape [None] and dtype tf.int32
+    def call_next(self, features, features_length, previous_encoder_states, *args, **kwargs):
         """
-        features = self.speech_featurizer.tf_extract(signal)
-        features = tf.expand_dims(features, axis=0)
-        input_length = shape_util.shape_list(features)[1]
-        input_length = math_util.get_reduced_length(input_length, self.time_reduction_factor)
-        input_length = tf.expand_dims(input_length, axis=0)
-        logits = self.encoder(features, training=False)
-        logits = self.decoder(logits, training=False)
-        probs = tf.nn.softmax(logits)
-        decoded = tf.keras.backend.ctc_decode(
-            y_pred=probs,
-            input_length=input_length,
-            greedy=False,
-            beam_width=self.text_featurizer.decoder_config.beam_width,
-        )
-        decoded = tf.cast(decoded[0][0][0], dtype=tf.int32)
-        transcript = self.text_featurizer.indices2upoints(decoded)
-        return transcript
+        Recognize function for encoder network from previous encoder states
 
-    # -------------------------------- TFLITE -------------------------------------
-
-    def make_tflite_function(
-        self,
-        greedy: bool = False,
-    ):
-        if greedy:
-            return tf.function(
-                self.recognize_tflite,
-                input_signature=[tf.TensorSpec([None], dtype=tf.float32)],
-            )
-        return tf.function(
-            self.recognize_beam_tflite,
-            input_signature=[tf.TensorSpec([None], dtype=tf.float32)],
-        )
+        Parameters
+        ----------
+        features : tf.Tensor, shape [B, T, F, C]
+        features_length : tf.Tensor, shape [B]
+        previous_encoder_states : tf.Tensor, shape [B, nlayers, nstates, rnn_units] -> [nlayers, nstates, B, rnn_units]
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor, tf.Tensor], shape ([B, T, dmodel], [B], [nlayers, nstates, B, rnn_units] -> [B, nlayers, nstates, rnn_units])
+        """
+        with tf.name_scope(f"{self.name}_call_next"):
+            previous_encoder_states = tf.transpose(previous_encoder_states, perm=[1, 2, 0, 3])
+            outputs, outputs_length = self.reshape((features, features_length))
+            new_states = []
+            for i, block in enumerate(self.blocks):
+                outputs, outputs_length, block_states = block.call_next(outputs, outputs_length, previous_encoder_states=previous_encoder_states[i])
+                new_states.append(block_states)
+            return outputs, outputs_length, tf.transpose(tf.stack(new_states, axis=0), perm=[2, 0, 1, 3])
+
+    def compute_mask(self, inputs, mask=None):
+        outputs, outputs_length, caching = inputs
+        maxlen = tf.shape(outputs)[1]
+        maxlen, outputs_length = (math_util.get_reduced_length(length, self.time_reduction_factor) for length in (maxlen, outputs_length))
+        mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
+        return mask, None, getattr(caching, "_keras_mask", None)
+
+    def compute_output_shape(self, input_shape):
+        *output_shape, caching_shape = input_shape
+        output_shape = self.reshape.compute_output_shape(output_shape)
+        for block in self.blocks:
+            output_shape = block.compute_output_shape(output_shape)
+        return *output_shape, caching_shape
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/ctc/jasper.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/jasper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,239 +10,205 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
+from tensorflow_asr.models.base_layer import Layer, Reshape
+from tensorflow_asr.models.layers.convolution import Conv1D
 from tensorflow_asr.utils import math_util
-from tensorflow_asr.models.ctc.base_ctc import CtcModel
-
-
-class Reshape(tf.keras.layers.Layer):
-    def call(self, inputs):
-        return math_util.merge_two_last_dims(inputs)
 
 
 class JasperSubBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         channels: int = 256,
         kernels: int = 11,
         strides: int = 1,
         dropout: float = 0.1,
+        padding: str = "causal",
         dilation: int = 1,
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(JasperSubBlock, self).__init__(**kwargs)
-        self.conv1d = tf.keras.layers.Conv1D(
+        super().__init__(**kwargs)
+        self.conv1d = Conv1D(
             filters=channels,
             kernel_size=kernels,
             strides=strides,
             dilation_rate=dilation,
-            padding="same",
+            padding=padding,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_conv1d",
+            name="conv1d",
+            dtype=self.dtype,
+        )
+        self.bn = tf.keras.layers.BatchNormalization(
+            name="bn", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
         )
-        self.bn = tf.keras.layers.BatchNormalization(name=f"{self.name}_bn")
-        self.relu = tf.keras.layers.ReLU(name=f"{self.name}_relu")
-        self.do = tf.keras.layers.Dropout(dropout, name=f"{self.name}_dropout")
+        self.relu = tf.keras.layers.ReLU(name="relu", dtype=self.dtype)
+        self.do = tf.keras.layers.Dropout(dropout, name="dropout", dtype=self.dtype)
         self.reduction_factor = strides
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
+    def call(self, inputs, training=False):
         outputs = inputs
         outputs = self.conv1d(outputs, training=training)
         outputs = self.bn(outputs, training=training)
         outputs = self.relu(outputs, training=training)
         outputs = self.do(outputs, training=training)
         return outputs
 
-    def get_config(self):
-        conf = super(JasperSubBlock, self).get_config()
-        conf.update(self.conv1d.get_config())
-        conf.update(self.bn.get_config())
-        conf.update(self.relu.get_config())
-        conf.update(self.do.get_config())
-        return conf
-
 
 class JasperResidual(tf.keras.layers.Layer):
     def __init__(
         self,
         channels: int = 256,
+        padding: str = "causal",
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(JasperResidual, self).__init__(**kwargs)
-        self.pointwise_conv1d = tf.keras.layers.Conv1D(
+        super().__init__(**kwargs)
+        self.pointwise_conv1d = Conv1D(
             filters=channels,
             kernel_size=1,
             strides=1,
-            padding="same",
+            padding=padding,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_pointwise_conv1d",
+            name="pointwise_conv1d",
+            dtype=self.dtype,
+        )
+        self.bn = tf.keras.layers.BatchNormalization(
+            name="bn", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
         )
-        self.bn = tf.keras.layers.BatchNormalization(name=f"{self.name}_bn")
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
+    def call(self, inputs, training=False):
         outputs = self.pointwise_conv1d(inputs, training=training)
         outputs = self.bn(outputs, training=training)
         return outputs
 
-    def get_config(self):
-        conf = super(JasperResidual, self).get_config()
-        conf.update(self.pointwise_conv1d.get_config())
-        conf.update(self.bn.get_config())
-        return conf
-
 
 class JasperSubBlockResidual(JasperSubBlock):
     def __init__(
         self,
         channels: int = 256,
         kernels: int = 11,
         strides: int = 1,
         dropout: float = 0.1,
+        padding: str = "causal",
         dilation: int = 1,
         nresiduals: int = 1,
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(JasperSubBlockResidual, self).__init__(
+        super().__init__(
             channels=channels,
             kernels=kernels,
             strides=strides,
             dropout=dropout,
+            padding=padding,
             dilation=dilation,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             **kwargs,
         )
 
         self.residuals = [
             JasperResidual(
                 channels=channels,
+                padding=padding,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
-                name=f"{self.name}_residual_{i}",
+                name=f"residual_{i}",
+                dtype=self.dtype,
             )
             for i in range(nresiduals)
         ]
 
-        self.add = tf.keras.layers.Add(name=f"{self.name}_add")
+        self.add = tf.keras.layers.Add(name="add")
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
+    def call(self, inputs, training=False):
         outputs, residuals = inputs
         outputs = self.conv1d(outputs, training=training)
         outputs = self.bn(outputs, training=training)
         for i, res in enumerate(residuals):
-            res = self.residuals[i](res, training=training, **kwargs)
+            res = self.residuals[i](res, training=training)
             outputs = self.add([outputs, res], training=training)
         outputs = self.relu(outputs, training=training)
         outputs = self.do(outputs, training=training)
         return outputs
 
-    def get_config(self):
-        conf = super(JasperSubBlockResidual, self).get_config()
-        conf.update(self.residual.get_config())
-        conf.update(self.add.get_config())
-        return conf
-
 
-class JasperBlock(tf.keras.Model):
+class JasperBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         nsubblocks: int = 3,
         channels: int = 256,
         kernels: int = 11,
         dropout: float = 0.1,
+        padding: str = "causal",
         dense: bool = False,
         nresiduals: int = 1,
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(JasperBlock, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         self.dense = dense
 
         self.subblocks = [
             JasperSubBlock(
                 channels=channels,
                 kernels=kernels,
                 dropout=dropout,
+                padding=padding,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
-                name=f"{self.name}_subordinate_{i}",
+                name=f"subordinate_{i}",
+                dtype=self.dtype,
             )
             for i in range(nsubblocks - 1)
         ]
 
         self.subblock_residual = JasperSubBlockResidual(
             channels=channels,
             kernels=kernels,
             dropout=dropout,
             nresiduals=nresiduals,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_subordinate_{nsubblocks - 1}",
+            name=f"subordinate_{nsubblocks - 1}",
+            dtype=self.dtype,
         )
 
         self.reduction_factor = 1
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
+    def call(self, inputs, training=False):
         inputs, residuals = inputs
         outputs = inputs
         for subblock in self.subblocks:
-            outputs = subblock(outputs, training=training, **kwargs)
+            outputs = subblock(outputs, training=training)
         if self.dense:
             residuals.append(inputs)
-            outputs = self.subblock_residual([outputs, residuals], training=training, **kwargs)
+            outputs = self.subblock_residual([outputs, residuals], training=training)
         else:
-            outputs = self.subblock_residual([outputs, [inputs]], training=training, **kwargs)
+            outputs = self.subblock_residual([outputs, [inputs]], training=training)
         return outputs, residuals
 
-    def get_config(self):
-        conf = self.subblock_residual.get_config()
-        conf.update({"dense": self.dense})
-        for subblock in self.subblocks:
-            conf.update(subblock.get_config())
-        return conf
-
 
-class JasperEncoder(tf.keras.Model):
+class JasperEncoder(Layer):
     def __init__(
         self,
         dense: bool = False,
+        padding: str = "causal",
         first_additional_block_channels: int = 256,
         first_additional_block_kernels: int = 11,
         first_additional_block_strides: int = 2,
         first_additional_block_dilation: int = 1,
         first_additional_block_dropout: int = 0.2,
         nsubblocks: int = 5,
         block_channels: list = [256, 384, 512, 640, 768],
@@ -256,169 +222,95 @@
         third_additional_block_channels: int = 1024,
         third_additional_block_kernels: int = 1,
         third_additional_block_strides: int = 1,
         third_additional_block_dilation: int = 1,
         third_additional_block_dropout: int = 0.4,
         kernel_regularizer=None,
         bias_regularizer=None,
-        name: str = "jasper_encoder",
         **kwargs,
     ):
-        super().__init__(name=name, **kwargs)
+        super().__init__(**kwargs)
 
         assert len(block_channels) == len(block_kernels) == len(block_dropout)
 
-        self.reshape = Reshape(name=f"{self.name}_reshape")
+        self.reshape = Reshape(name="reshape")
 
         self.first_additional_block = JasperSubBlock(
             channels=first_additional_block_channels,
             kernels=first_additional_block_kernels,
             strides=first_additional_block_strides,
             dropout=first_additional_block_dropout,
+            padding=padding,
             dilation=first_additional_block_dilation,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_first_block",
+            name="first_block",
+            dtype=self.dtype,
         )
 
         self.blocks = [
             JasperBlock(
                 nsubblocks=nsubblocks,
                 channels=block_channels[i],
                 kernels=block_kernels[i],
                 dropout=block_dropout[i],
                 dense=dense,
                 nresiduals=(i + 1) if dense else 1,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
-                name=f"{self.name}_block_{i}",
+                name=f"block_{i}",
+                dtype=self.dtype,
             )
             for i in range(len(block_channels))
         ]
 
         self.second_additional_block = JasperSubBlock(
             channels=second_additional_block_channels,
             kernels=second_additional_block_kernels,
             strides=second_additional_block_strides,
             dropout=second_additional_block_dropout,
+            padding=padding,
             dilation=second_additional_block_dilation,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_second_block",
+            name="second_block",
+            dtype=self.dtype,
         )
 
         self.third_additional_block = JasperSubBlock(
             channels=third_additional_block_channels,
             kernels=third_additional_block_kernels,
             strides=third_additional_block_strides,
             dropout=third_additional_block_dropout,
+            padding=padding,
             dilation=third_additional_block_dilation,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_third_block",
+            name="third_block",
+            dtype=self.dtype,
         )
-
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        outputs = self.reshape(inputs)
-        outputs = self.first_additional_block(outputs, training=training, **kwargs)
+        self.time_reduction_factor = self.first_additional_block.reduction_factor
+        self.time_reduction_factor *= self.second_additional_block.reduction_factor
+        self.time_reduction_factor *= self.third_additional_block.reduction_factor
+
+    def call(self, inputs, training=False):
+        outputs, outputs_length, caching = inputs
+        outputs, outputs_length = self.reshape((outputs, outputs_length))
+        outputs = self.first_additional_block(outputs, training=training)
 
         residuals = []
         for block in self.blocks:
-            outputs, residuals = block([outputs, residuals], training=training, **kwargs)
-
-        outputs = self.second_additional_block(outputs, training=training, **kwargs)
-        outputs = self.third_additional_block(outputs, training=training, **kwargs)
-        return outputs
-
-    def summary(
-        self,
-        line_length=100,
-        **kwargs,
-    ):
-        super().summary(line_length=line_length, **kwargs)
-
-    def get_config(self):
-        conf = super().get_config()
-        conf.update(self.reshape.get_config())
-        conf.update(self.first_additional_block.get_config())
-        for block in self.blocks:
-            conf.update(block.get_config())
-        conf.update(self.second_additional_block.get_config())
-        conf.update(self.third_additional_block.get_config())
-        return conf
+            outputs, residuals = block([outputs, residuals], training=training)
 
-
-class Jasper(CtcModel):
-    def __init__(
-        self,
-        vocabulary_size: int,
-        dense: bool = False,
-        first_additional_block_channels: int = 256,
-        first_additional_block_kernels: int = 11,
-        first_additional_block_strides: int = 2,
-        first_additional_block_dilation: int = 1,
-        first_additional_block_dropout: int = 0.2,
-        nsubblocks: int = 5,
-        block_channels: list = [256, 384, 512, 640, 768],
-        block_kernels: list = [11, 13, 17, 21, 25],
-        block_dropout: list = [0.2, 0.2, 0.2, 0.3, 0.3],
-        second_additional_block_channels: int = 896,
-        second_additional_block_kernels: int = 1,
-        second_additional_block_strides: int = 1,
-        second_additional_block_dilation: int = 2,
-        second_additional_block_dropout: int = 0.4,
-        third_additional_block_channels: int = 1024,
-        third_additional_block_kernels: int = 1,
-        third_additional_block_strides: int = 1,
-        third_additional_block_dilation: int = 1,
-        third_additional_block_dropout: int = 0.4,
-        kernel_regularizer=None,
-        bias_regularizer=None,
-        name="jasper",
-        **kwargs,
-    ):
-        super().__init__(
-            encoder=JasperEncoder(
-                dense=dense,
-                first_additional_block_channels=first_additional_block_channels,
-                first_additional_block_kernels=first_additional_block_kernels,
-                first_additional_block_strides=first_additional_block_strides,
-                first_additional_block_dilation=first_additional_block_dilation,
-                first_additional_block_dropout=first_additional_block_dropout,
-                nsubblocks=nsubblocks,
-                block_channels=block_channels,
-                block_kernels=block_kernels,
-                block_dropout=block_dropout,
-                second_additional_block_channels=second_additional_block_channels,
-                second_additional_block_kernels=second_additional_block_kernels,
-                second_additional_block_strides=second_additional_block_strides,
-                second_additional_block_dilation=second_additional_block_dilation,
-                second_additional_block_dropout=second_additional_block_dropout,
-                third_additional_block_channels=third_additional_block_channels,
-                third_additional_block_kernels=third_additional_block_kernels,
-                third_additional_block_strides=third_additional_block_strides,
-                third_additional_block_dilation=third_additional_block_dilation,
-                third_additional_block_dropout=third_additional_block_dropout,
-                kernel_regularizer=None,
-                bias_regularizer=None,
-            ),
-            decoder=tf.keras.layers.Conv1D(
-                filters=vocabulary_size,
-                kernel_size=1,
-                strides=1,
-                padding="same",
-                kernel_regularizer=kernel_regularizer,
-                bias_regularizer=bias_regularizer,
-                name=f"{name}_logits",
-            ),
-            vocabulary_size=vocabulary_size,
-            name=name,
-            **kwargs,
-        )
-        self.time_reduction_factor = self.encoder.first_additional_block.reduction_factor
-        self.time_reduction_factor *= self.encoder.second_additional_block.reduction_factor
-        self.time_reduction_factor *= self.encoder.third_additional_block.reduction_factor
+        outputs = self.second_additional_block(outputs, training=training)
+        outputs = self.third_additional_block(outputs, training=training)
+        outputs_length = math_util.get_reduced_length(outputs_length, self.time_reduction_factor)
+        outputs = math_util.apply_mask(outputs, mask=tf.sequence_mask(outputs_length, maxlen=tf.shape(outputs)[1], dtype=tf.bool))
+        return outputs, outputs_length, caching
+
+    def compute_output_shape(self, input_shape):
+        inputs_shape, inputs_length_shape, caching_shape = input_shape
+        outputs_time = None if inputs_shape[1] is None else math_util.legacy_get_reduced_length(inputs_shape[1], self.time_reduction_factor)
+        outputs_batch = inputs_shape[0]
+        outputs_size = self.third_additional_block.conv1d.filters
+        outputs_shape = [outputs_batch, outputs_time, outputs_size]
+        return tuple(outputs_shape), tuple(inputs_length_shape), caching_shape
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/encoders/conformer.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/transformer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# pylint: disable=attribute-defined-outside-init
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,419 +11,332 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from tensorflow_asr.utils import shape_util
-from tensorflow_asr.models.activations.glu import GLU
-from tensorflow_asr.models.layers.multihead_attention import MultiHeadAttention, RelPositionMultiHeadAttention
-from tensorflow_asr.models.layers.positional_encoding import PositionalEncoding, PositionalEncodingConcat
-from tensorflow_asr.models.layers.subsampling import Conv2dSubsampling, VggSubsampling
+from tensorflow_asr.models.base_layer import Layer
+from tensorflow_asr.models.layers.multihead_attention import MultiHeadAttention, MultiHeadRelativeAttention
+from tensorflow_asr.models.layers.positional_encoding import RelativeSinusoidalPositionalEncoding, SinusoidalPositionalEncoding
+from tensorflow_asr.models.layers.residual import Residual
+from tensorflow_asr.models.layers.subsampling import Conv1dSubsampling, Conv2dSubsampling, VggSubsampling
 
-L2 = tf.keras.regularizers.l2(1e-6)
 
-
-class FFModule(tf.keras.layers.Layer):
+class Pointwiseffn(Layer):
     def __init__(
         self,
-        input_dim,
-        dropout=0.0,
-        fc_factor=0.5,
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name="ff_module",
+        dmodel,
+        dff,
+        activation="relu",
+        kernel_regularizer=None,
+        bias_regularizer=None,
         **kwargs,
     ):
-        super(FFModule, self).__init__(name=name, **kwargs)
-        self.fc_factor = fc_factor
-        self.ln = tf.keras.layers.LayerNormalization(
-            name=f"{name}_ln",
-            gamma_regularizer=kernel_regularizer,
-            beta_regularizer=bias_regularizer,
-        )
+        super().__init__(**kwargs)
         self.ffn1 = tf.keras.layers.Dense(
-            4 * input_dim,
-            name=f"{name}_dense_1",
+            units=dff,
+            activation=activation,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
+            name="ffn_1",
+            dtype=self.dtype,
         )
-        self.swish = tf.keras.layers.Activation(tf.nn.swish, name=f"{name}_swish_activation")
-        self.do1 = tf.keras.layers.Dropout(dropout, name=f"{name}_dropout_1")
         self.ffn2 = tf.keras.layers.Dense(
-            input_dim,
-            name=f"{name}_dense_2",
+            units=dmodel,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
+            name="ffn_2",
+            dtype=self.dtype,
         )
-        self.do2 = tf.keras.layers.Dropout(dropout, name=f"{name}_dropout_2")
-        self.res_add = tf.keras.layers.Add(name=f"{name}_add")
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        outputs = self.ln(inputs, training=training)
-        outputs = self.ffn1(outputs, training=training)
-        outputs = self.swish(outputs)
-        outputs = self.do1(outputs, training=training)
+    def call(self, inputs, training=False):
+        outputs = self.ffn1(inputs, training=training)
         outputs = self.ffn2(outputs, training=training)
-        outputs = self.do2(outputs, training=training)
-        outputs = self.res_add([inputs, self.fc_factor * outputs])
         return outputs
 
-    def get_config(self):
-        conf = super(FFModule, self).get_config()
-        conf.update({"fc_factor": self.fc_factor})
-        conf.update(self.ln.get_config())
-        conf.update(self.ffn1.get_config())
-        conf.update(self.swish.get_config())
-        conf.update(self.do1.get_config())
-        conf.update(self.ffn2.get_config())
-        conf.update(self.do2.get_config())
-        conf.update(self.res_add.get_config())
-        return conf
 
-
-class MHSAModule(tf.keras.layers.Layer):
+class TransformerBlock(Layer):
     def __init__(
         self,
-        head_size,
+        dmodel,
+        dff,
         num_heads,
-        dropout=0.0,
-        mha_type="relmha",
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name="mhsa_module",
+        head_size,
+        mha_type="mha",
+        relmha_causal=False,
+        norm_position="post",
+        residual_factor=1.0,
+        pwffn_activation="relu",
+        dropout=0.1,
+        memory_length=None,
+        use_attention_bias=False,
+        kernel_regularizer=None,
+        bias_regularizer=None,
         **kwargs,
     ):
-        super(MHSAModule, self).__init__(name=name, **kwargs)
-        self.ln = tf.keras.layers.LayerNormalization(
-            name=f"{name}_ln",
-            gamma_regularizer=kernel_regularizer,
-            beta_regularizer=bias_regularizer,
+        super().__init__(**kwargs)
+        assert norm_position in ("pre", "post", "none")
+        assert mha_type in ("mha", "relmha")
+        self._norm_position = norm_position
+        self._mha_type = mha_type
+        self.norm1 = (
+            None
+            if self._norm_position == "none"
+            else tf.keras.layers.LayerNormalization(
+                beta_regularizer=kernel_regularizer, gamma_regularizer=bias_regularizer, name="ln_1", dtype=self.dtype
+            )
         )
-        if mha_type == "relmha":
-            self.mha = RelPositionMultiHeadAttention(
-                name=f"{name}_mhsa",
-                head_size=head_size,
+        self.mha = (
+            MultiHeadAttention(
                 num_heads=num_heads,
+                key_dim=head_size,
+                output_shape=dmodel,
+                memory_length=memory_length,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
+                name="mhsa",
+                dtype=self.dtype,
             )
-        elif mha_type == "mha":
-            self.mha = MultiHeadAttention(
-                name=f"{name}_mhsa",
-                head_size=head_size,
+            if mha_type == "mha"
+            else MultiHeadRelativeAttention(
+                causal=relmha_causal,
                 num_heads=num_heads,
+                key_dim=head_size,
+                output_shape=dmodel,
+                memory_length=memory_length,
+                use_attention_bias=use_attention_bias,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
+                name="mhsa",
+                dtype=self.dtype,
             )
-        else:
-            raise ValueError("mha_type must be either 'mha' or 'relmha'")
-        self.do = tf.keras.layers.Dropout(dropout, name=f"{name}_dropout")
-        self.res_add = tf.keras.layers.Add(name=f"{name}_add")
-        self.mha_type = mha_type
-
-    def call(
-        self,
-        inputs,
-        training=False,
-        mask=None,
-        **kwargs,
-    ):
-        inputs, pos = inputs  # pos is positional encoding
-        outputs = self.ln(inputs, training=training)
-        if self.mha_type == "relmha":
-            outputs = self.mha([outputs, outputs, outputs, pos], training=training, mask=mask)
-        else:
-            outputs = outputs + pos
-            outputs = self.mha([outputs, outputs, outputs], training=training, mask=mask)
-        outputs = self.do(outputs, training=training)
-        outputs = self.res_add([inputs, outputs])
-        return outputs
-
-    def get_config(self):
-        conf = super(MHSAModule, self).get_config()
-        conf.update({"mha_type": self.mha_type})
-        conf.update(self.ln.get_config())
-        conf.update(self.mha.get_config())
-        conf.update(self.do.get_config())
-        conf.update(self.res_add.get_config())
-        return conf
-
-
-class ConvModule(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        input_dim,
-        kernel_size=32,
-        dropout=0.0,
-        depth_multiplier=1,
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name="conv_module",
-        **kwargs,
-    ):
-        super(ConvModule, self).__init__(name=name, **kwargs)
-        self.ln = tf.keras.layers.LayerNormalization()
-        self.pw_conv_1 = tf.keras.layers.Conv2D(
-            filters=2 * input_dim,
-            kernel_size=1,
-            strides=1,
-            padding="valid",
-            name=f"{name}_pw_conv_1",
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
         )
-        self.glu = GLU(name=f"{name}_glu")
-        self.dw_conv = tf.keras.layers.DepthwiseConv2D(
-            kernel_size=(kernel_size, 1),
-            strides=1,
-            padding="same",
-            name=f"{name}_dw_conv",
-            depth_multiplier=depth_multiplier,
-            depthwise_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-        )
-        self.bn = tf.keras.layers.BatchNormalization(
-            name=f"{name}_bn",
-            gamma_regularizer=kernel_regularizer,
-            beta_regularizer=bias_regularizer,
-        )
-        self.swish = tf.keras.layers.Activation(
-            tf.nn.swish,
-            name=f"{name}_swish_activation",
+        self.do1 = tf.keras.layers.Dropout(dropout, name="do_1", dtype=self.dtype)
+        self.residual1 = Residual(factor=residual_factor, regularizer=bias_regularizer, name="residual_1", dtype=self.dtype)
+        self.norm2 = (
+            None
+            if self._norm_position == "none"
+            else tf.keras.layers.LayerNormalization(
+                beta_regularizer=kernel_regularizer, gamma_regularizer=bias_regularizer, name="ln_2", dtype=self.dtype
+            )
         )
-        self.pw_conv_2 = tf.keras.layers.Conv2D(
-            filters=input_dim,
-            kernel_size=1,
-            strides=1,
-            padding="valid",
-            name=f"{name}_pw_conv_2",
+        self.pwffn = Pointwiseffn(
+            dmodel=dmodel,
+            dff=dff,
+            activation=pwffn_activation,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
+            name="pwffn",
+            dtype=self.dtype,
         )
-        self.do = tf.keras.layers.Dropout(dropout, name=f"{name}_dropout")
-        self.res_add = tf.keras.layers.Add(name=f"{name}_add")
+        self.do2 = tf.keras.layers.Dropout(dropout, name="do_2", dtype=self.dtype)
+        self.residual2 = Residual(factor=residual_factor, regularizer=bias_regularizer, name="residual_2", dtype=self.dtype)
 
     def call(
         self,
         inputs,
         training=False,
-        **kwargs,
-    ):
-        outputs = self.ln(inputs, training=training)
-        B, T, E = shape_util.shape_list(outputs)
-        outputs = tf.reshape(outputs, [B, T, 1, E])
-        outputs = self.pw_conv_1(outputs, training=training)
-        outputs = self.glu(outputs)
-        outputs = self.dw_conv(outputs, training=training)
-        outputs = self.bn(outputs, training=training)
-        outputs = self.swish(outputs)
-        outputs = self.pw_conv_2(outputs, training=training)
-        outputs = tf.reshape(outputs, [B, T, E])
-        outputs = self.do(outputs, training=training)
-        outputs = self.res_add([inputs, outputs])
-        return outputs
-
-    def get_config(self):
-        conf = super(ConvModule, self).get_config()
-        conf.update(self.ln.get_config())
-        conf.update(self.pw_conv_1.get_config())
-        conf.update(self.glu.get_config())
-        conf.update(self.dw_conv.get_config())
-        conf.update(self.bn.get_config())
-        conf.update(self.swish.get_config())
-        conf.update(self.pw_conv_2.get_config())
-        conf.update(self.do.get_config())
-        conf.update(self.res_add.get_config())
-        return conf
-
-
-class ConformerBlock(tf.keras.layers.Layer):
-    def __init__(
-        self,
-        input_dim,
-        dropout=0.0,
-        fc_factor=0.5,
-        head_size=36,
-        num_heads=4,
-        mha_type="relmha",
-        kernel_size=32,
-        depth_multiplier=1,
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name="conformer_block",
-        **kwargs,
+        attention_mask=None,
+        use_causal_mask=False,
+        use_auto_mask=True,
     ):
-        super(ConformerBlock, self).__init__(name=name, **kwargs)
-        self.ffm1 = FFModule(
-            input_dim=input_dim,
-            dropout=dropout,
-            fc_factor=fc_factor,
-            name=f"{name}_ff_module_1",
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-        )
-        self.mhsam = MHSAModule(
-            mha_type=mha_type,
-            head_size=head_size,
-            num_heads=num_heads,
-            dropout=dropout,
-            name=f"{name}_mhsa_module",
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-        )
-        self.convm = ConvModule(
-            input_dim=input_dim,
-            kernel_size=kernel_size,
-            dropout=dropout,
-            name=f"{name}_conv_module",
-            depth_multiplier=depth_multiplier,
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-        )
-        self.ffm2 = FFModule(
-            input_dim=input_dim,
-            dropout=dropout,
-            fc_factor=fc_factor,
-            name=f"{name}_ff_module_2",
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
+        original_outputs, caching, relative_position_encoding, content_attention_bias, positional_attention_bias = inputs
+        outputs = self.norm1(original_outputs, training=training) if self._norm_position == "pre" else original_outputs
+        outputs, caching = self.mha(
+            [outputs, outputs, outputs, caching, relative_position_encoding, content_attention_bias, positional_attention_bias],
+            training=training,
+            attention_mask=attention_mask,
+            use_causal_mask=use_causal_mask,
+            use_auto_mask=use_auto_mask,
         )
-        self.ln = tf.keras.layers.LayerNormalization(
-            name=f"{name}_ln",
-            gamma_regularizer=kernel_regularizer,
-            beta_regularizer=kernel_regularizer,
-        )
-
-    def call(
-        self,
-        inputs,
-        training=False,
-        mask=None,
-        **kwargs,
-    ):
-        inputs, pos = inputs  # pos is positional encoding
-        outputs = self.ffm1(inputs, training=training, **kwargs)
-        outputs = self.mhsam([outputs, pos], training=training, mask=mask, **kwargs)
-        outputs = self.convm(outputs, training=training, **kwargs)
-        outputs = self.ffm2(outputs, training=training, **kwargs)
-        outputs = self.ln(outputs, training=training)
-        return outputs
+        outputs = self.do1(outputs, training=training)
+        outputs = self.norm1(outputs, training=training) if self._norm_position == "post" else outputs
+        original_outputs = self.residual1([original_outputs, outputs], training=training)
+        outputs = self.norm2(original_outputs, training=training) if self._norm_position == "pre" else original_outputs
+        outputs = self.pwffn(outputs, training=training)
+        outputs = self.do2(outputs, training=training)
+        outputs = self.norm2(outputs, training=training) if self._norm_position == "post" else outputs
+        outputs = self.residual2([original_outputs, outputs], training=training)
+        return outputs, caching
 
-    def get_config(self):
-        conf = super(ConformerBlock, self).get_config()
-        conf.update(self.ffm1.get_config())
-        conf.update(self.mhsam.get_config())
-        conf.update(self.convm.get_config())
-        conf.update(self.ffm2.get_config())
-        conf.update(self.ln.get_config())
-        return conf
+    def compute_output_shape(self, input_shape):
+        output_shape, caching_shape, *_ = input_shape
+        return output_shape, caching_shape
 
 
-class ConformerEncoder(tf.keras.Model):
+class TransformerEncoder(Layer):
     def __init__(
         self,
         subsampling,
-        positional_encoding="sinusoid",
-        dmodel=144,
-        num_blocks=16,
-        mha_type="relmha",
-        head_size=36,
+        num_blocks=6,
+        dmodel=512,
+        dff=1024,
         num_heads=4,
-        kernel_size=32,
-        depth_multiplier=1,
-        fc_factor=0.5,
-        dropout=0.0,
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name="conformer_encoder",
+        head_size=128,
+        dropout=0.1,
+        mha_type="mha",
+        relmha_causal=False,
+        norm_position="post",
+        residual_factor=1.0,
+        interleave_relpe=True,
+        use_attention_causal_mask=False,
+        use_attention_auto_mask=True,
+        use_attention_bias=False,
+        pwffn_activation="relu",
+        memory_length=None,
+        kernel_regularizer=None,
+        bias_regularizer=None,
+        name="transformer_encoder",
         **kwargs,
     ):
-        super(ConformerEncoder, self).__init__(name=name, **kwargs)
+        super().__init__(name=name, **kwargs)
+        self._use_attention_causal_mask = use_attention_causal_mask
+        self._use_attention_auto_mask = use_attention_auto_mask
+        self._num_blocks = num_blocks
+        self._dmodel = dmodel
+        self._memory_length = memory_length
 
-        subsampling_name = subsampling.pop("type", "conv2d")
+        subsampling_name = subsampling.pop("type", None)
         if subsampling_name == "vgg":
             subsampling_class = VggSubsampling
         elif subsampling_name == "conv2d":
             subsampling_class = Conv2dSubsampling
+        elif subsampling_name == "conv1d":
+            subsampling_class = Conv1dSubsampling
         else:
-            raise ValueError("subsampling must be either  'conv2d' or 'vgg'")
-
-        self.conv_subsampling = subsampling_class(
+            raise ValueError("subsampling must be either 'vgg', 'conv2d', 'conv1d'")
+        self.subsampling = subsampling_class(
             **subsampling,
-            name=f"{name}_subsampling",
+            name="subsampling",
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
+            dtype=self.dtype,
         )
-
-        if positional_encoding == "sinusoid":
-            self.pe = PositionalEncoding(name=f"{name}_pe")
-        elif positional_encoding == "sinusoid_v2":
-            self.pe = PositionalEncoding(alpha=2, beta=0, name=f"{name}_pe")
-        elif positional_encoding == "sinusoid_concat":
-            self.pe = PositionalEncodingConcat(name=f"{name}_pe")
-        elif positional_encoding == "sinusoid_concat_v2":
-            self.pe = PositionalEncodingConcat(alpha=2, beta=-1, name=f"{name}_pe")
-        elif positional_encoding == "subsampling":
-            self.pe = tf.keras.layers.Activation("linear", name=f"{name}_pe")
-        else:
-            raise ValueError(
-                "positional_encoding must be either 'sinusoid', \
-                'sinusoid_concat', 'sinusoid_v2', 'sinusoid_concat_v2' or 'subsampling'"
-            )
-
+        self.time_reduction_factor = self.subsampling.time_reduction_factor
         self.linear = tf.keras.layers.Dense(
-            dmodel,
-            name=f"{name}_linear",
+            units=dmodel,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
+            name="linear",
+            dtype=self.dtype,
         )
-        self.do = tf.keras.layers.Dropout(dropout, name=f"{name}_dropout")
+        self.do = tf.keras.layers.Dropout(dropout, name="dropout", dtype=self.dtype)
 
-        self.conformer_blocks = []
-        for i in range(num_blocks):
-            conformer_block = ConformerBlock(
-                input_dim=dmodel,
-                dropout=dropout,
-                fc_factor=fc_factor,
-                head_size=head_size,
+        if mha_type == "relmha":
+            self.relpe = RelativeSinusoidalPositionalEncoding(
+                interleave=interleave_relpe,
+                memory_length=memory_length,
+                causal=relmha_causal,
+                name="relpe",
+                dtype=self.dtype,
+            )
+        else:
+            self.relpe = SinusoidalPositionalEncoding(interleave=interleave_relpe, name="pe", dtype=self.dtype)
+
+        self.blocks = [
+            TransformerBlock(
+                dmodel=dmodel,
+                dff=dff,
                 num_heads=num_heads,
+                head_size=head_size,
                 mha_type=mha_type,
-                kernel_size=kernel_size,
-                depth_multiplier=depth_multiplier,
+                relmha_causal=relmha_causal,
+                norm_position=norm_position,
+                residual_factor=residual_factor,
+                pwffn_activation=pwffn_activation,
+                dropout=dropout,
+                memory_length=memory_length,
+                use_attention_bias=use_attention_bias,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
-                name=f"{name}_block_{i}",
+                name=f"block_{i}",
+                dtype=self.dtype,
             )
-            self.conformer_blocks.append(conformer_block)
+            for i in range(self._num_blocks)
+        ]
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        mask=None,
-        **kwargs,
-    ):
-        # input with shape [B, T, V1, V2]
-        outputs = self.conv_subsampling(inputs, training=training)
+        if mha_type == "relmha" and not use_attention_bias:
+            self.content_attention_bias = self.add_weight(
+                name="content_attention_bias",
+                shape=[num_heads, head_size],
+                trainable=True,
+                initializer="zeros",
+                regularizer=bias_regularizer,
+                dtype=self.variable_dtype,
+            )
+            self.positional_attention_bias = self.add_weight(
+                name="positional_attention_bias",
+                shape=[num_heads, head_size],
+                trainable=True,
+                initializer="zeros",
+                regularizer=bias_regularizer,
+                dtype=self.variable_dtype,
+            )
+        else:
+            self.content_attention_bias, self.positional_attention_bias = None, None
+
+    def reset_caching(self, batch_size):
+        if self._memory_length is None:
+            return None
+        # fmt: off
+        return [
+            tf.zeros(shape=(batch_size, self._memory_length, self._dmodel), dtype=self.dtype)
+            for _ in range(self._num_blocks)
+        ]
+        # fmt: on
+
+    def call(self, inputs, training=False):
+        outputs, outputs_length, caching = inputs
+        outputs, outputs_length = self.subsampling([outputs, outputs_length], training=training)
         outputs = self.linear(outputs, training=training)
-        pe = self.pe(outputs)
+        outputs, relative_position_encoding = self.relpe([outputs, outputs_length], training=training)
         outputs = self.do(outputs, training=training)
-        for cblock in self.conformer_blocks:
-            outputs = cblock([outputs, pe], training=training, mask=mask, **kwargs)
-        return outputs
-
-    def get_config(self):
-        conf = super(ConformerEncoder, self).get_config()
-        conf.update(self.conv_subsampling.get_config())
-        conf.update(self.linear.get_config())
-        conf.update(self.do.get_config())
-        conf.update(self.pe.get_config())
-        for cblock in self.conformer_blocks:
-            conf.update(cblock.get_config())
-        return conf
+        new_caching = None if self._memory_length is None else []
+        for i, block in enumerate(self.blocks):
+            outputs, new_cache = block(
+                [
+                    outputs,
+                    None if caching is None else caching[i],
+                    relative_position_encoding,
+                    self.content_attention_bias,
+                    self.positional_attention_bias,
+                ],
+                training=training,
+                use_causal_mask=self._use_attention_causal_mask,
+                use_auto_mask=self._use_attention_auto_mask,
+            )
+            if new_caching is not None:
+                new_caching.append(new_cache)
+        return outputs, outputs_length, new_caching
+
+    def call_next(self, features, features_length, *args, **kwargs):
+        """
+        Recognize function for encoder network
+
+        Parameters
+        ----------
+        features : tf.Tensor, shape [B, T, F, C]
+        features_length : tf.Tensor, shape [B]
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor, tf.Tensor], shape ([B, T, dmodel], [B], None)
+            Outputs, outputs_length, new_states
+        """
+        with tf.name_scope(f"{self.name}_call_next"):
+            outputs, outputs_length, _ = self.call((features, features_length, None), training=False)
+            return outputs, outputs_length, None
+
+    def compute_mask(self, inputs, mask=None):
+        *outputs, caching = inputs
+        return *self.subsampling.compute_mask(outputs, mask=mask), getattr(caching, "_keras_mask", None)
+
+    def compute_output_shape(self, input_shape):
+        output_shape, output_length_shape, caching_shape = input_shape
+        output_shape, output_length_shape = self.subsampling.compute_output_shape((output_shape, output_length_shape))
+        output_shape = self.linear.compute_output_shape(output_shape)
+        output_shape, relative_position_encoding_shape = self.relpe.compute_output_shape((output_shape, output_length_shape))
+        output_shape = self.do.compute_output_shape(output_shape)
+        for block in self.blocks:
+            output_shape, caching_shape = block.compute_output_shape((output_shape, caching_shape, relative_position_encoding_shape, None, None))
+        return output_shape, output_length_shape, caching_shape
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/encoders/contextnet.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/contextnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,250 +1,325 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Ref: https://github.com/iankur/ContextNet """
+""" http://arxiv.org/abs/2005.03191 """
 
 from typing import List
+
 import tensorflow as tf
 
+from tensorflow_asr.models.base_layer import Layer, Reshape
 from tensorflow_asr.utils import math_util
 
 L2 = tf.keras.regularizers.l2(1e-6)
 
 
 def get_activation(
     activation: str = "silu",
 ):
     activation = activation.lower()
     if activation in ["silu", "swish"]:
         return tf.nn.swish
-    elif activation == "relu":
+    if activation == "relu":
         return tf.nn.relu
-    elif activation == "linear":
+    if activation == "linear":
         return tf.keras.activations.linear
-    else:
-        raise ValueError("activation must be either 'silu', 'swish', 'relu' or 'linear'")
-
-
-class Reshape(tf.keras.layers.Layer):
-    def call(self, inputs):
-        return math_util.merge_two_last_dims(inputs)
+    raise ValueError("activation must be either 'silu', 'swish', 'relu' or 'linear'")
 
 
-class ConvModule(tf.keras.layers.Layer):
+class ConvModule(Layer):
     def __init__(
         self,
         kernel_size: int = 3,
         strides: int = 1,
         filters: int = 256,
         activation: str = "silu",
+        padding: str = "causal",
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(ConvModule, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.strides = strides
         self.conv = tf.keras.layers.SeparableConv1D(
             filters=filters,
             kernel_size=kernel_size,
             strides=strides,
-            padding="same",
+            padding=padding,
             depthwise_regularizer=kernel_regularizer,
             pointwise_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_conv",
+            name="conv",
+            dtype=self.dtype,
+        )
+        self.bn = tf.keras.layers.BatchNormalization(
+            name="bn", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
         )
-        self.bn = tf.keras.layers.BatchNormalization(name=f"{self.name}_bn")
         self.activation = get_activation(activation)
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        outputs = self.conv(inputs, training=training)
+    def call(self, inputs, training=False):
+        outputs, outputs_length = inputs
+        outputs = self.conv(outputs, training=training)
+        outputs_length = math_util.conv_output_length(
+            outputs_length, filter_size=self.conv.kernel_size[0], padding=self.conv.padding, stride=self.conv.strides[0]
+        )
         outputs = self.bn(outputs, training=training)
         outputs = self.activation(outputs)
-        return outputs
+        return outputs, outputs_length
+
+    def compute_mask(self, inputs, mask=None):
+        outputs, outputs_length = inputs
+        maxlen = tf.shape(outputs)[1]
+        maxlen, outputs_length = (
+            math_util.conv_output_length(length, filter_size=self.conv.kernel_size[0], padding=self.conv.padding, stride=self.conv.strides[0])
+            for length in (maxlen, outputs_length)
+        )
+        mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
+        return mask, None
+
+    def compute_output_shape(self, input_shape):
+        output_shape, output_length_shape = input_shape
+        output_shape = self.conv.compute_output_shape(output_shape)
+        return output_shape, output_length_shape
 
 
-class SEModule(tf.keras.layers.Layer):
+class SEModule(Layer):
     def __init__(
         self,
         kernel_size: int = 3,
         strides: int = 1,
         filters: int = 256,
         activation: str = "silu",
+        padding: str = "causal",
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(SEModule, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.conv = ConvModule(
             kernel_size=kernel_size,
             strides=strides,
             filters=filters,
             activation=activation,
+            padding=padding,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_conv_module",
+            name="conv_module",
+            dtype=self.dtype,
         )
+        self.global_avg_pool = tf.keras.layers.GlobalAveragePooling1D(keepdims=True, name="global_avg_pool", dtype=self.dtype)
         self.activation = get_activation(activation)
-        self.fc1 = tf.keras.layers.Dense(filters // 8, name=f"{self.name}_fc1")
-        self.fc2 = tf.keras.layers.Dense(filters, name=f"{self.name}_fc2")
+        self.fc1 = tf.keras.layers.Dense(
+            filters // 8,
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            name="fc1",
+            dtype=self.dtype,
+        )
+        self.fc2 = tf.keras.layers.Dense(
+            filters,
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            name="fc2",
+            dtype=self.dtype,
+        )
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        features, input_length = inputs
-        outputs = self.conv(features, training=training)
+    def call(self, inputs, training=False):
+        outputs, outputs_length = inputs
+        outputs, outputs_length = self.conv((outputs, outputs_length), training=training)  # [B, T, E]
 
-        se = tf.divide(tf.reduce_sum(outputs, axis=1), tf.expand_dims(tf.cast(input_length, dtype=outputs.dtype), axis=1))
+        se = self.global_avg_pool(outputs)  # [B, 1, E], mask auto populate
         se = self.fc1(se, training=training)
         se = self.activation(se)
         se = self.fc2(se, training=training)
-        se = self.activation(se)
         se = tf.nn.sigmoid(se)
-        se = tf.expand_dims(se, axis=1)
 
-        outputs = tf.multiply(outputs, se)
-        return outputs
+        se = tf.tile(se, [1, tf.shape(outputs)[1], 1])  # [B, 1, E] => [B, T, E]
+        outputs = tf.multiply(outputs, se)  # [B, T, E]
+        return outputs, outputs_length
 
+    def compute_mask(self, inputs, mask=None):
+        return self.conv.compute_mask(inputs, mask=mask)
 
-class ConvBlock(tf.keras.layers.Layer):
+    def compute_output_shape(self, input_shape):
+        return self.conv.compute_output_shape(input_shape)
+
+
+class ConvBlock(Layer):
     def __init__(
         self,
         nlayers: int = 3,
         kernel_size: int = 3,
         filters: int = 256,
         strides: int = 1,
         residual: bool = True,
         activation: str = "silu",
         alpha: float = 1.0,
+        padding: str = "causal",
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(ConvBlock, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-        self.dmodel = filters
         self.time_reduction_factor = strides
         filters = int(filters * alpha)
+        self.dmodel = filters
 
         self.convs = []
         for i in range(nlayers - 1):
             self.convs.append(
                 ConvModule(
                     kernel_size=kernel_size,
                     strides=1,
                     filters=filters,
                     activation=activation,
+                    padding=padding,
                     kernel_regularizer=kernel_regularizer,
                     bias_regularizer=bias_regularizer,
-                    name=f"{self.name}_conv_module_{i}",
+                    name=f"conv_module_{i}",
+                    dtype=self.dtype,
                 )
             )
 
         self.last_conv = ConvModule(
             kernel_size=kernel_size,
             strides=strides,
             filters=filters,
             activation=activation,
+            padding=padding,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_conv_module_{nlayers - 1}",
+            name=f"conv_module_{nlayers - 1}",
+            dtype=self.dtype,
         )
 
         self.se = SEModule(
             kernel_size=kernel_size,
             strides=1,
             filters=filters,
             activation=activation,
+            padding=padding,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
-            name=f"{self.name}_se",
+            name="se",
+            dtype=self.dtype,
         )
 
         self.residual = None
         if residual:
             self.residual = ConvModule(
                 kernel_size=kernel_size,
                 strides=strides,
                 filters=filters,
                 activation="linear",
+                padding=padding,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
-                name=f"{self.name}_residual",
+                name="residual",
+                dtype=self.dtype,
             )
 
         self.activation = get_activation(activation)
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        features, input_length = inputs
-        outputs = features
+    def call(self, inputs, training=False):
+        _inputs, _inputs_length = inputs
+        outputs, outputs_length = _inputs, _inputs_length
         for conv in self.convs:
-            outputs = conv(outputs, training=training)
-        outputs = self.last_conv(outputs, training=training)
-        input_length = math_util.get_reduced_length(input_length, self.last_conv.strides)
-        outputs = self.se([outputs, input_length], training=training)
+            outputs, outputs_length = conv((outputs, outputs_length), training=training)
+        outputs, outputs_length = self.last_conv((outputs, outputs_length), training=training)
+        outputs, outputs_length = self.se((outputs, outputs_length), training=training)
         if self.residual is not None:
-            res = self.residual(features, training=training)
+            res, _ = self.residual((_inputs, _inputs_length), training=training)
             outputs = tf.add(outputs, res)
         outputs = self.activation(outputs)
-        return outputs, input_length
+        return outputs, outputs_length
+
+    def compute_mask(self, inputs, mask=None):
+        return self.last_conv.compute_mask(inputs, mask=mask)
 
+    def compute_output_shape(self, input_shape):
+        output_shape = input_shape
+        for conv in self.convs:
+            output_shape = conv.compute_output_shape(output_shape)
+        output_shape = self.last_conv.compute_output_shape(output_shape)
+        output_shape = self.se.compute_output_shape(output_shape)
+        return output_shape
 
-class ContextNetEncoder(tf.keras.Model):
+
+class ContextNetEncoder(Layer):
     def __init__(
         self,
         blocks: List[dict] = [],
         alpha: float = 1.0,
         kernel_regularizer=None,
         bias_regularizer=None,
         **kwargs,
     ):
-        super(ContextNetEncoder, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
-        self.reshape = Reshape(name=f"{self.name}_reshape")
+        self.reshape = Reshape(name="reshape", dtype=self.dtype)
 
         self.blocks = []
+        self.time_reduction_factor = 1
         for i, config in enumerate(blocks):
-            self.blocks.append(
-                ConvBlock(
-                    **config,
-                    alpha=alpha,
-                    kernel_regularizer=kernel_regularizer,
-                    bias_regularizer=bias_regularizer,
-                    name=f"{self.name}_block_{i}",
-                )
+            block = ConvBlock(
+                **config,
+                alpha=alpha,
+                kernel_regularizer=kernel_regularizer,
+                bias_regularizer=bias_regularizer,
+                name=f"block_{i}",
+                dtype=self.dtype,
             )
+            self.blocks.append(block)
+            self.time_reduction_factor *= block.time_reduction_factor
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        outputs, input_length = inputs
-        outputs = self.reshape(outputs)
+        self.dmodel = self.blocks[-1].dmodel
+
+    def call(self, inputs, training=False):
+        outputs, outputs_length, caching = inputs
+        outputs, outputs_length = self.reshape((outputs, outputs_length))
+        for block in self.blocks:
+            outputs, outputs_length = block((outputs, outputs_length), training=training)
+        return outputs, outputs_length, caching
+
+    def call_next(self, features, features_length, *args, **kwargs):
+        """
+        Recognize function for encoder network
+
+        Parameters
+        ----------
+        features : tf.Tensor, shape [B, T, F, C]
+        features_length : tf.Tensor, shape [B]
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor, tf.Tensor], shape ([B, T, dmodel], [B], None)
+            Outputs, outputs_length, new_states
+        """
+        with tf.name_scope(f"{self.name}_call_next"):
+            outputs, outputs_length, _ = self.call((features, features_length, None), training=False)
+            return outputs, outputs_length, None
+
+    def compute_mask(self, inputs, mask=None):
+        outputs, outputs_length, caching = inputs
+        maxlen = tf.shape(outputs)[1]
+        maxlen, outputs_length = (math_util.get_reduced_length(length, self.time_reduction_factor) for length in (maxlen, outputs_length))
+        mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
+        return mask, None, getattr(caching, "_keras_mask", None)
+
+    def compute_output_shape(self, input_shape):
+        *output_shape, caching_shape = input_shape
+        output_shape = self.reshape.compute_output_shape(output_shape)
         for block in self.blocks:
-            outputs, input_length = block([outputs, input_length], training=training)
-        return outputs
+            output_shape = block.compute_output_shape(output_shape)
+        return *output_shape, caching_shape
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/layers/bnlstmcell.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/sequence_wise_bn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,71 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# pylint:disable=attribute-defined-outside-init
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import tensorflow as tf
-import tensorflow.keras.backend as K
-from tensorflow.python.ops import array_ops
 
 
-def ds2_rnn_batch_norm(
-    x_i,
-    x_f,
-    x_c,
-    x_o,
-    beta=None,
-    gamma=None,
-):
-    # x is input * weight with shape [batch_size, units * 4]
-    # Merge into single array of features
-    # https://www.tensorflow.org/api_docs/python/tf/nn/moments
-    x = tf.concat([x_i, x_f, x_c, x_o], axis=1)
-    mean, variance = tf.nn.moments(x, axes=[0, 1], keepdims=False)
-    x = tf.nn.batch_normalization(
-        x=x,
-        mean=mean,
-        variance=variance,
-        offset=beta,
-        scale=gamma,
-        variance_epsilon=K.epsilon(),
-    )
-    x_i, x_f, x_c, x_o = array_ops.split(x, num_or_size_splits=4, axis=1)
-    return x_i, x_f, x_c, x_o
+# https://arxiv.org/abs/1510.01378
+class SequenceBatchNorm(tf.keras.layers.Layer):
+    def __init__(self, name, time_major=False, gamma_regularizer=None, beta_regularizer=None, **kwargs):
+        super().__init__(name=name, **kwargs)
+        self.time_major = time_major
+        self.gamma_regularizer = tf.keras.regularizers.get(gamma_regularizer)
+        self.beta_regularizer = tf.keras.regularizers.get(beta_regularizer)
 
-
-# Frame-wise Batch Norm RNN
-class BNLSTMCell(tf.keras.layers.LSTMCell):
-    def __init__(
+    def build(
         self,
-        *args,
-        **kwargs,
+        input_shape,
     ):
-        super().__init__(*args, **kwargs)
         self.beta = self.add_weight(
-            shape=(self.units * 4,),
-            name="lstm_bn_beta",
+            shape=[input_shape[-1]],
+            name="beta",
             initializer="zeros",
-            regularizer=None,
+            regularizer=self.beta_regularizer,
             constraint=None,
             trainable=True,
+            dtype=self.variable_dtype,
         )
         self.gamma = self.add_weight(
-            shape=(self.units * 4,),
-            name="lstm_bn_gamma",
+            shape=[input_shape[-1]],
+            name="gamma",
             initializer="ones",
-            regularizer=None,
+            regularizer=self.gamma_regularizer,
             constraint=None,
             trainable=True,
+            dtype=self.variable_dtype,
         )
 
-    def _compute_carry_and_output(
+    def call(
         self,
-        x,
-        h_tm1,
-        c_tm1,
+        inputs,
+        **kwargs,
     ):
-        """Computes carry and output using split kernels."""
-        x_i, x_f, x_c, x_o = x
-        x_i, x_f, x_c, x_o = ds2_rnn_batch_norm(x_i, x_f, x_c, x_o, beta=self.beta, gamma=self.gamma)
-
-        h_tm1_i, h_tm1_f, h_tm1_c, h_tm1_o = h_tm1
-        i = self.recurrent_activation(x_i + K.dot(h_tm1_i, self.recurrent_kernel[:, : self.units]))
-        f = self.recurrent_activation(x_f + K.dot(h_tm1_f, self.recurrent_kernel[:, self.units : self.units * 2]))
-        c = f * c_tm1 + i * self.activation(x_c + K.dot(h_tm1_c, self.recurrent_kernel[:, self.units * 2 : self.units * 3]))
-        o = self.recurrent_activation(x_o + K.dot(h_tm1_o, self.recurrent_kernel[:, self.units * 3 :]))
-        return c, o
+        mean, variance = tf.nn.moments(inputs, axes=[0, 1], keepdims=False)
+        if self.time_major:
+            total_padded_frames = tf.cast(tf.shape(inputs)[0], tf.keras.backend.dtype(mean))
+            batch_size = tf.cast(tf.shape(inputs)[1], tf.keras.backend.dtype(mean))
+        else:
+            total_padded_frames = tf.cast(tf.shape(inputs)[1], tf.keras.backend.dtype(mean))
+            batch_size = tf.cast(tf.shape(inputs)[0], tf.keras.backend.dtype(mean))
+        total_unpadded_frames_batch = tf.math.count_nonzero(inputs, axis=[0, 1], keepdims=False, dtype=tf.keras.backend.dtype(mean))
+        mean = (mean * total_padded_frames * batch_size) / total_unpadded_frames_batch
+        variance = (variance * total_padded_frames * batch_size) / total_unpadded_frames_batch
+        return tf.nn.batch_normalization(
+            inputs,
+            mean=mean,
+            variance=variance,
+            offset=self.beta,
+            scale=self.gamma,
+            variance_epsilon=tf.keras.backend.epsilon(),
+        )
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/layers/embedding.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/residual.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,74 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2023 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Optional
+
 import tensorflow as tf
 
+from tensorflow_asr.models.base_layer import Layer
+
+
+class Residual(Layer):
+    """Applying residual addition to layers
+    - Normal addition with constant factor
+    - Rezero: which improves convergence speed. This implements the paper:
+    ReZero is All You Need: Fast Convergence at Large Depth.
+    (https://arxiv.org/pdf/2003.04887.pdf).
+    """
 
-class Embedding(tf.keras.layers.Layer):
     def __init__(
         self,
-        vocab_size,
-        embed_dim,
-        contraint=None,
-        regularizer=None,
-        initializer=None,
+        factor="rezero",
+        initializer: tf.keras.initializers.Initializer = "zeros",
+        regularizer: Optional[tf.keras.regularizers.Regularizer] = None,
+        name="residual",
         **kwargs,
     ):
-        super(Embedding, self).__init__(**kwargs)
-        self.vocab_size = vocab_size
-        self.embed_dim = embed_dim
-        self.contraint = tf.keras.constraints.get(contraint)
-        self.regularizer = tf.keras.regularizers.get(regularizer)
-        self.initializer = tf.keras.initializers.get(initializer)
+        super().__init__(name=name, **kwargs)
+        self._factor = factor
+        self._initializer = initializer
+        self._regularizer = regularizer
 
     def build(self, input_shape):
-        self.embeddings = self.add_weight(
-            name="embeddings",
-            dtype=tf.float32,
-            shape=[self.vocab_size, self.embed_dim],
-            initializer=self.initializer,
-            trainable=True,
-            regularizer=self.regularizer,
-            constraint=self.contraint,
-        )
-        self.built = True
+        if self._factor == "rezero":
+            self._alpha = self.add_weight(
+                name="alpha",
+                shape=[],
+                initializer=self._initializer,
+                regularizer=self._regularizer,
+                trainable=True,
+                dtype=self.variable_dtype,
+            )
+        else:
+            assert isinstance(self._factor, (int, float))
+            self._alpha = tf.convert_to_tensor(self._factor, dtype=self.compute_dtype)
+        return super().build(input_shape)
 
     def call(self, inputs):
-        outputs = tf.cast(inputs, dtype=tf.int32)
-        return tf.nn.embedding_lookup(self.embeddings, outputs)
-
-    def recognize_tflite(self, inputs):
-        outputs = tf.cast(tf.expand_dims(inputs, axis=-1), dtype=tf.int32)
-        return tf.gather_nd(self.embeddings, outputs)  # https://github.com/tensorflow/tensorflow/issues/42410
+        x, residual_x = inputs
+        alpha = tf.cast(self._alpha, residual_x.dtype)
+        x = x + alpha * residual_x
+        return x
 
     def get_config(self):
-        conf = super(Embedding, self).get_config()
-        conf.update(
-            {
-                "vocab_size": self.vocab_size,
-                "embed_dim": self.embed_dim,
-                "contraint": self.contraint,
-                "regularizer": self.regularizer,
-                "initializer": self.initializer,
-            }
-        )
-        return conf
+        config = {
+            "factor": self._factor,
+            "initializer": self._initializer,
+            "regularizer": self._regularizer,
+        }
+        base_config = super().get_config()
+        return dict(list(base_config.items()) + list(config.items()))
+
+    def compute_output_shape(self, input_shape):
+        return input_shape[0]
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/layers/positional_encoding.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/embedding.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,97 +10,83 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from tensorflow_asr.utils.shape_util import shape_list
+from tensorflow_asr.models.base_layer import Layer
 
 
-class PositionalEncoding(tf.keras.layers.Layer):
+class Embedding(tf.keras.layers.Embedding):
     def __init__(
         self,
-        alpha: int = 1,
-        beta: int = 0,
-        name="positional_encoding",
+        vocab_size,
+        embed_dim,
+        initializer="uniform",
+        regularizer=None,
+        contraint=None,
         **kwargs,
     ):
-        super().__init__(trainable=False, name=name, **kwargs)
-        self.alpha = alpha
-        self.beta = beta
-
-    def build(
-        self,
-        input_shape,
-    ):
-        dmodel = input_shape[-1]
-        assert dmodel % 2 == 0, f"Input last dim must be even: {dmodel}"
-
-    @staticmethod
-    def encode(
-        max_len,
-        dmodel,
-    ):
-        pos = tf.expand_dims(tf.range(max_len - 1, -1, -1.0, dtype=tf.float32), axis=1)
-        index = tf.expand_dims(tf.range(0, dmodel, dtype=tf.float32), axis=0)
-
-        pe = pos * (1 / tf.pow(10000.0, (2 * (index // 2)) / dmodel))
-
-        # Sin cos will be [max_len, size // 2]
-        # we add 0 between numbers by using padding and reshape
-        sin = tf.pad(tf.expand_dims(tf.sin(pe[:, 0::2]), -1), [[0, 0], [0, 0], [0, 1]], mode="CONSTANT", constant_values=0)
-        sin = tf.reshape(sin, [max_len, dmodel])
-        cos = tf.pad(tf.expand_dims(tf.cos(pe[:, 1::2]), -1), [[0, 0], [0, 0], [1, 0]], mode="CONSTANT", constant_values=0)
-        cos = tf.reshape(cos, [max_len, dmodel])
-        # Then add sin and cos, which results in [time, size]
-        pe = tf.add(sin, cos)
-        return tf.expand_dims(pe, axis=0)  # [1, time, size]
-
-    def call(
-        self,
-        inputs,
-        **kwargs,
-    ):
-        # inputs shape [B, T, V]
-        _, max_len, dmodel = shape_list(inputs)
-        pe = self.encode(max_len * self.alpha + self.beta, dmodel)
-        return tf.cast(pe, dtype=inputs.dtype)
-
-    def get_config(self):
-        conf = super().get_config()
-        conf.update({"alpha": self.alpha, "beta": self.beta})
-        return conf
-
-
-class PositionalEncodingConcat(PositionalEncoding):
-    def build(
-        self,
-        input_shape,
-    ):
-        dmodel = input_shape[-1]
-        assert dmodel % 2 == 0, f"Input last dim must be even: {dmodel}"
-
-    @staticmethod
-    def encode(
-        max_len,
-        dmodel,
-    ):
-        pos = tf.range(max_len - 1, -1, -1.0, dtype=tf.float32)
-
-        index = tf.range(0, dmodel, 2.0, dtype=tf.float32)
-        index = 1 / tf.pow(10000.0, (index / dmodel))
-
-        sinusoid = tf.einsum("i,j->ij", pos, index)
-        pos = tf.concat([tf.sin(sinusoid), tf.cos(sinusoid)], axis=-1)
-
-        return tf.expand_dims(pos, axis=0)
-
-    def call(
-        self,
-        inputs,
-        **kwargs,
-    ):
-        # inputs shape [B, T, V]
-        _, max_len, dmodel = shape_list(inputs)
-        pe = self.encode(max_len * self.alpha + self.beta, dmodel)
-        return tf.cast(pe, dtype=inputs.dtype)
+        super().__init__(
+            input_dim=vocab_size,
+            output_dim=embed_dim,
+            embeddings_initializer=initializer,
+            embeddings_regularizer=regularizer,
+            embeddings_constraint=contraint,
+            mask_zero=False,
+            **kwargs,
+        )
+        self.supports_masking = True
+
+    def call(self, inputs):
+        outputs, outputs_length = inputs
+        outputs = super().call(outputs)
+        return outputs, outputs_length
+
+    def call_next(self, inputs):
+        outputs = tf.cast(tf.expand_dims(inputs, axis=-1), dtype=tf.int32)
+        return tf.gather_nd(self.embeddings, outputs)  # https://github.com/tensorflow/tensorflow/issues/42410
+
+    def compute_mask(self, inputs, mask=None):
+        outputs, outputs_length = inputs
+        mask = tf.sequence_mask(outputs_length, maxlen=tf.shape(outputs)[1], dtype=tf.bool)
+        return mask, None
+
+    def compute_output_shape(self, input_shape):
+        output_shape, output_length_shape = input_shape
+        output_shape = super().compute_output_shape(output_shape)
+        return output_shape, output_length_shape
+
+
+class OneHotBlank(Layer):
+    """
+    https://arxiv.org/pdf/1211.3711.pdf
+    The inputs are encoded as one-hot vectors;
+    that is, if Y consists of K labels and yu = k, then y^u is a length K vector whose elements are all zero
+    except the k-th, which is one. ∅ is encoded as a length K vector of zeros
+    """
+
+    def __init__(self, blank, depth, name="one_hot_blank", **kwargs):
+        super().__init__(name=name, **kwargs)
+        self.blank = blank
+        self.depth = depth
+
+    def call(self, inputs):
+        outputs, outputs_length = inputs
+        minus_one_at_blank = tf.where(tf.equal(outputs, self.blank), -1, outputs)
+        outputs = tf.one_hot(minus_one_at_blank, depth=self.depth, dtype=self.dtype)
+        return outputs, outputs_length
+
+    def call_next(self, inputs):
+        outputs, _ = self.call((inputs, None))
+        return outputs
+
+    def compute_mask(self, inputs, mask=None):
+        outputs, outputs_length = inputs
+        mask = tf.sequence_mask(outputs_length, maxlen=tf.shape(outputs)[1], dtype=tf.bool)
+        return mask, None
+
+    def compute_output_shape(self, input_shape):
+        output_shape, output_length_shape = input_shape
+        output_shape = output_shape + (self.depth,)
+        return output_shape, output_length_shape
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/base_transducer.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/base_transducer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# pylint: disable=attribute-defined-outside-init,too-many-lines
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,944 +11,1049 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ https://arxiv.org/pdf/1811.06621.pdf """
 
 import collections
-from typing import Dict
+
 import tensorflow as tf
 
-from tensorflow_asr.featurizers.speech_featurizers import SpeechFeaturizer
-from tensorflow_asr.featurizers.text_featurizers import TextFeaturizer
+from tensorflow_asr import schemas
 from tensorflow_asr.losses.rnnt_loss import RnntLoss
-from tensorflow_asr.utils import data_util, layer_util, math_util, shape_util
+from tensorflow_asr.models.base_layer import Layer
 from tensorflow_asr.models.base_model import BaseModel
-from tensorflow_asr.models.layers.embedding import Embedding
+from tensorflow_asr.models.layers.embedding import Embedding, OneHotBlank
+from tensorflow_asr.utils import layer_util, shape_util
 
 Hypothesis = collections.namedtuple("Hypothesis", ("index", "prediction", "states"))
 
 BeamHypothesis = collections.namedtuple("BeamHypothesis", ("score", "indices", "prediction", "states"))
 
+JOINT_MODES = ["add", "mul"]
+
 
-class TransducerPrediction(tf.keras.Model):
+class TransducerPrediction(Layer):
     def __init__(
         self,
-        vocabulary_size: int,
-        embed_dim: int,
-        embed_dropout: float = 0,
+        blank: int,
+        vocab_size: int,
+        label_encoder_mode: str = "embedding",  # either "embedding" | "one_hot"
+        embed_dim: int = 0,
         num_rnns: int = 1,
         rnn_units: int = 512,
         rnn_type: str = "lstm",
         rnn_implementation: int = 2,
+        rnn_unroll: bool = False,
         layer_norm: bool = True,
         projection_units: int = 0,
         kernel_regularizer=None,
         bias_regularizer=None,
         name="transducer_prediction",
         **kwargs,
     ):
         super().__init__(name=name, **kwargs)
-        self.embed = Embedding(vocabulary_size, embed_dim, regularizer=kernel_regularizer, name=f"{name}_embedding")
-        self.do = tf.keras.layers.Dropout(embed_dropout, name=f"{name}_dropout")
+        assert label_encoder_mode in ("one_hot", "embedding"), "label_encode_mode must be either 'one_hot' or 'embedding'"
+        self.label_encoder = (
+            Embedding(vocab_size, embed_dim, regularizer=kernel_regularizer, name=label_encoder_mode, dtype=self.dtype)
+            if label_encoder_mode == "embedding"
+            else OneHotBlank(blank=blank, depth=vocab_size, name=label_encoder_mode, dtype=self.dtype)
+        )
         # Initialize rnn layers
-        RNN = layer_util.get_rnn(rnn_type)
+        RnnClass = layer_util.get_rnn(rnn_type)
         self.rnns = []
+        self.lns = []
+        self.projections = []
         for i in range(num_rnns):
-            rnn = RNN(
+            rnn = RnnClass(
                 units=rnn_units,
                 return_sequences=True,
-                name=f"{name}_{rnn_type}_{i}",
+                name=f"{rnn_type}_{i}",
                 return_state=True,
                 implementation=rnn_implementation,
+                unroll=rnn_unroll,
+                zero_output_for_mask=True,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
+                dtype=self.dtype,
             )
-            if layer_norm:
-                ln = tf.keras.layers.LayerNormalization(name=f"{name}_ln_{i}")
-            else:
-                ln = None
-            if projection_units > 0:
-                projection = tf.keras.layers.Dense(
+            ln = (
+                tf.keras.layers.LayerNormalization(
+                    name=f"ln_{i}", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
+                )
+                if layer_norm
+                else None
+            )
+            projection = (
+                tf.keras.layers.Dense(
                     projection_units,
-                    name=f"{name}_projection_{i}",
+                    name=f"projection_{i}",
                     kernel_regularizer=kernel_regularizer,
                     bias_regularizer=bias_regularizer,
+                    dtype=self.dtype,
                 )
-            else:
-                projection = None
-            self.rnns.append({"rnn": rnn, "ln": ln, "projection": projection})
+                if projection_units > 0
+                else None
+            )
+            self.rnns.append(rnn)
+            self.lns.append(ln)
+            self.projections.append(projection)
 
-    def get_initial_state(self):
-        """Get zeros states
+    def get_initial_state(self, batch_size: int):
+        """
+        Get zeros states
 
-        Returns:
-            tf.Tensor: states having shape [num_rnns, 1 or 2, B, P]
+        Returns
+        -------
+        tf.Tensor, shape [B, num_rnns, nstates, state_size]
+            Zero initialized states
         """
         states = []
         for rnn in self.rnns:
-            states.append(tf.stack(rnn["rnn"].get_initial_state(tf.zeros([1, 1, 1], dtype=tf.float32)), axis=0))
-        return tf.stack(states, axis=0)
+            states.append(tf.stack(rnn.get_initial_state(tf.zeros([batch_size, 1, 1], dtype=self.dtype)), axis=0))
+        return tf.transpose(tf.stack(states, axis=0), perm=[2, 0, 1, 3])
 
-    def call(self, inputs, training=False, **kwargs):
-        # inputs has shape [B, U]
-        # use tf.gather_nd instead of tf.gather for tflite conversion
-        outputs, prediction_length = inputs
-        outputs = self.embed(outputs, training=training)
-        outputs = self.do(outputs, training=training)
-        for rnn in self.rnns:
-            mask = tf.sequence_mask(prediction_length, maxlen=tf.shape(outputs)[1])
-            outputs = rnn["rnn"](outputs, training=training, mask=mask)
-            outputs = outputs[0]
-            if rnn["ln"] is not None:
-                outputs = rnn["ln"](outputs, training=training)
-            if rnn["projection"] is not None:
-                outputs = rnn["projection"](outputs, training=training)
-        return outputs
+    def call(self, inputs, training=False):
+        outputs, outputs_length = inputs
+        outputs, outputs_length = self.label_encoder((outputs, outputs_length), training=training)
+        for i, rnn in enumerate(self.rnns):
+            outputs, *_ = rnn(outputs, training=training)  # mask auto populate
+            if self.lns[i] is not None:
+                outputs = self.lns[i](outputs, training=training)
+            if self.projections[i] is not None:
+                outputs = self.projections[i](outputs, training=training)
+        return outputs, outputs_length
 
-    def recognize(self, inputs, states, tflite: bool = False):
-        """Recognize function for prediction network
+    def call_next(self, inputs, previous_decoder_states):
+        """
+        Recognize function for prediction network from the previous predicted tokens
 
-        Args:
-            inputs (tf.Tensor): shape [1, 1]
-            states (tf.Tensor): shape [num_lstms, 2, B, P]
-
-        Returns:
-            tf.Tensor: outputs with shape [1, 1, P]
-            tf.Tensor: new states with shape [num_lstms, 2, 1, P]
+        Parameters
+        ----------
+        inputs : tf.Tensor, shape [B, 1]
+        previous_decoder_states : tf.Tensor, shape [B, num_rnns, nstates, rnn_units]
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor], shapes ([B, 1, rnn_units], [B, num_rnns, nstates, rnn_units])
+            Outputs, new states
         """
-        if tflite:
-            outputs = self.embed.recognize_tflite(inputs)
-        else:
-            outputs = self.embed(inputs, training=False)
-        outputs = self.do(outputs, training=False)
-        new_states = []
+        with tf.name_scope(f"{self.name}_call_next"):
+            previous_decoder_states = tf.transpose(previous_decoder_states, perm=[1, 2, 0, 3])
+            outputs = self.label_encoder.call_next(inputs)
+            new_states = []
+            for i, rnn in enumerate(self.rnns):
+                outputs, *_states = rnn(outputs, training=False, initial_state=tf.unstack(previous_decoder_states[i], axis=0))
+                new_states.append(tf.stack(_states))
+                if self.lns[i] is not None:
+                    outputs = self.lns[i](outputs, training=False)
+                if self.projections[i] is not None:
+                    outputs = self.projections[i](outputs, training=False)
+            return outputs, tf.transpose(tf.stack(new_states, axis=0), perm=[2, 0, 1, 3])
+
+    def compute_mask(self, inputs, mask=None):
+        return self.label_encoder.compute_mask(inputs, mask=mask)
+
+    def compute_output_shape(self, input_shape):
+        output_shape, output_length_shape = input_shape
+        output_shape, output_length_shape = self.label_encoder.compute_output_shape((output_shape, output_length_shape))
         for i, rnn in enumerate(self.rnns):
-            outputs = rnn["rnn"](outputs, training=False, initial_state=tf.unstack(states[i], axis=0))
-            new_states.append(tf.stack(outputs[1:]))
-            outputs = outputs[0]
-            if rnn["ln"] is not None:
-                outputs = rnn["ln"](outputs, training=False)
-            if rnn["projection"] is not None:
-                outputs = rnn["projection"](outputs, training=False)
-        return outputs, tf.stack(new_states, axis=0)
-
-    def get_config(self):
-        conf = self.embed.get_config()
-        conf.update(self.do.get_config())
-        for rnn in self.rnns:
-            conf.update(rnn["rnn"].get_config())
-            if rnn["ln"] is not None:
-                conf.update(rnn["ln"].get_config())
-            if rnn["projection"] is not None:
-                conf.update(rnn["projection"].get_config())
-        return conf
-
-
-class TransducerJointReshape(tf.keras.layers.Layer):
-    def __init__(self, axis: int = 1, name="transducer_joint_reshape", **kwargs):
-        super().__init__(name=name, trainable=False, **kwargs)
-        self.axis = axis
-
-    def call(self, inputs, repeats=None, **kwargs):
-        outputs = tf.expand_dims(inputs, axis=self.axis)
-        return tf.repeat(outputs, repeats=repeats, axis=self.axis)
-
-    def get_config(self):
-        conf = super().get_config()
-        conf.update({"axis": self.axis})
-        return conf
+            output_shape = (
+                self.projections[i].compute_output_shape(output_shape)
+                if self.projections[i] is not None
+                else rnn.compute_output_shape(output_shape)[0]
+            )
+        return tuple(output_shape), tuple(output_length_shape)
+
+
+class TransducerJointMerge(Layer):
+    def __init__(self, joint_mode: str = "add", name="transducer_joint_merge", **kwargs):
+        super().__init__(name=name, **kwargs)
+        if joint_mode not in JOINT_MODES:
+            raise ValueError(f"joint_mode must in {JOINT_MODES}")
+        self.joint_mode = joint_mode
+
+    def compute_mask(self, inputs, mask=None):
+        enc_out, pred_out = inputs
+        enc_mask = mask[0] if mask else getattr(enc_out, "_keras_mask", None)  # BT
+        pred_mask = mask[1] if mask else getattr(pred_out, "_keras_mask", None)  # BU
+        auto_mask = None
+        if enc_mask is not None:
+            auto_mask = enc_mask[:, :, tf.newaxis]  # BT1
+        if pred_mask is not None:
+            if auto_mask is not None:
+                auto_mask = auto_mask & pred_mask[:, tf.newaxis, :]  # BT1 & B1U -> BTU
+            else:
+                auto_mask = pred_mask[:, tf.newaxis, :]
+        mask = auto_mask
+        return mask
+
+    def call(self, inputs):
+        enc_out, pred_out = inputs
+        enc_out = tf.expand_dims(enc_out, axis=2)  # [B, T, 1, V]
+        pred_out = tf.expand_dims(pred_out, axis=1)  # [B, 1, U, V]
+        if self.joint_mode == "add":
+            outputs = tf.add(enc_out, pred_out)  # broadcast operator
+        else:
+            outputs = tf.multiply(enc_out, pred_out)  # broadcast operator
+        return outputs  # [B, T, U, V]
+
+    def compute_output_shape(self, input_shape):
+        enc_shape, pred_shape = input_shape
+        return enc_shape[0], enc_shape[1], pred_shape[1], enc_shape[-1]
 
 
-class TransducerJoint(tf.keras.Model):
+class TransducerJoint(Layer):
     def __init__(
         self,
-        vocabulary_size: int,
+        vocab_size: int,
         joint_dim: int = 1024,
         activation: str = "tanh",
-        prejoint_linear: bool = True,
+        prejoint_encoder_linear: bool = True,
+        prejoint_prediction_linear: bool = True,
         postjoint_linear: bool = False,
         joint_mode: str = "add",
         kernel_regularizer=None,
         bias_regularizer=None,
         name="tranducer_joint",
         **kwargs,
     ):
         super().__init__(name=name, **kwargs)
 
-        activation = activation.lower()
-        if activation == "linear":
-            self.activation = tf.keras.layers.Activation(tf.keras.activation.linear, name=f"{name}_linear")
-        elif activation == "relu":
-            self.activation = tf.keras.layers.Activation(tf.nn.relu, name=f"{name}_relu")
-        elif activation == "tanh":
-            self.activation = tf.keras.layers.Activation(tf.nn.tanh, name=f"{name}_tanh")
-        else:
-            raise ValueError("activation must be either 'linear', 'relu' or 'tanh'")
-
-        self.prejoint_linear = prejoint_linear
+        self.prejoint_encoder_linear = prejoint_encoder_linear
+        self.prejoint_prediction_linear = prejoint_prediction_linear
         self.postjoint_linear = postjoint_linear
 
-        if self.prejoint_linear:
+        if self.prejoint_encoder_linear:
             self.ffn_enc = tf.keras.layers.Dense(
-                joint_dim, name=f"{name}_enc", kernel_regularizer=kernel_regularizer, bias_regularizer=bias_regularizer
+                joint_dim,
+                name="enc",
+                kernel_regularizer=kernel_regularizer,
+                bias_regularizer=bias_regularizer,
+                dtype=self.dtype,
             )
+        if self.prejoint_prediction_linear:
             self.ffn_pred = tf.keras.layers.Dense(
-                joint_dim, use_bias=False, name=f"{name}_pred", kernel_regularizer=kernel_regularizer
+                joint_dim,
+                use_bias=False,
+                name="pred",
+                kernel_regularizer=kernel_regularizer,
+                dtype=self.dtype,
             )
 
-        self.enc_reshape = TransducerJointReshape(axis=2, name=f"{name}_enc_reshape")
-        self.pred_reshape = TransducerJointReshape(axis=1, name=f"{name}_pred_reshape")
+        self.joint = TransducerJointMerge(joint_mode=joint_mode, name="merge", dtype=self.dtype)
 
-        if joint_mode == "add":
-            self.joint = tf.keras.layers.Add(name=f"{name}_add")
-        elif joint_mode == "concat":
-            self.joint = tf.keras.layers.Concatenate(name=f"{name}_concat")
-        else:
-            raise ValueError("joint_mode must be either 'add' or 'concat'")
+        activation = activation.lower()
+        self.activation = tf.keras.layers.Activation(activation, name=activation, dtype=self.dtype)
 
         if self.postjoint_linear:
             self.ffn = tf.keras.layers.Dense(
-                joint_dim, name=f"{name}_ffn", kernel_regularizer=kernel_regularizer, bias_regularizer=bias_regularizer
+                joint_dim,
+                name="ffn",
+                kernel_regularizer=kernel_regularizer,
+                bias_regularizer=bias_regularizer,
+                dtype=self.dtype,
             )
 
         self.ffn_out = tf.keras.layers.Dense(
-            vocabulary_size, name=f"{name}_vocab", kernel_regularizer=kernel_regularizer, bias_regularizer=bias_regularizer
+            vocab_size,
+            name="vocab",
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            dtype=self.dtype,
         )
 
-    def call(self, inputs, training=False, **kwargs):
+    def call(self, inputs, training=False):
         # enc has shape [B, T, E]
         # pred has shape [B, U, P]
         enc_out, pred_out = inputs
-        if self.prejoint_linear:
+        if self.prejoint_encoder_linear:
             enc_out = self.ffn_enc(enc_out, training=training)  # [B, T, E] => [B, T, V]
+        if self.prejoint_prediction_linear:
             pred_out = self.ffn_pred(pred_out, training=training)  # [B, U, P] => [B, U, V]
-        enc_out = self.enc_reshape(enc_out, repeats=tf.shape(pred_out)[1])
-        pred_out = self.pred_reshape(pred_out, repeats=tf.shape(enc_out)[1])
-        outputs = self.joint([enc_out, pred_out], training=training)
+        outputs = self.joint((enc_out, pred_out))  # => [B, T, U, V]
         if self.postjoint_linear:
             outputs = self.ffn(outputs, training=training)
-        outputs = self.activation(outputs, training=training)  # => [B, T, U, V]
+        outputs = self.activation(outputs, training=training)
         outputs = self.ffn_out(outputs, training=training)
         return outputs
 
-    def get_config(self):
-        conf = self.ffn_enc.get_config()
-        conf.update(self.ffn_pred.get_config())
-        conf.update(self.ffn_out.get_config())
-        conf.update(self.activation.get_config())
-        conf.update(self.joint.get_config())
-        conf.update({"prejoint_linear": self.prejoint_linear, "postjoint_linear": self.postjoint_linear})
-        return conf
+    def compute_mask(self, inputs, mask=None):
+        return self.joint.compute_mask(inputs, mask=mask)
+
+    def compute_output_shape(self, input_shape):
+        encoder_shape, prediction_shape = input_shape
+        batch_shape = encoder_shape[0]
+        encoder_time_shape, prediction_time_shape = encoder_shape[1], prediction_shape[1]
+        return batch_shape, encoder_time_shape, prediction_time_shape, self.ffn_out.units
 
 
 class Transducer(BaseModel):
     """Transducer Model Warper"""
 
     def __init__(
         self,
-        encoder: tf.keras.Model,
-        vocabulary_size: int,
-        embed_dim: int = 512,
-        embed_dropout: float = 0,
-        num_rnns: int = 1,
-        rnn_units: int = 320,
-        rnn_type: str = "lstm",
-        rnn_implementation: int = 2,
-        layer_norm: bool = True,
-        projection_units: int = 0,
+        blank: int,
+        vocab_size: int,
+        speech_config: dict,
+        encoder: tf.keras.layers.Layer,
+        prediction_label_encoder_mode: str = "embedding",
+        prediction_embed_dim: int = 512,
+        prediction_num_rnns: int = 1,
+        prediction_rnn_units: int = 320,
+        prediction_rnn_type: str = "lstm",
+        prediction_rnn_implementation: int = 2,
+        prediction_rnn_unroll: bool = False,
+        prediction_layer_norm: bool = True,
+        prediction_projection_units: int = 0,
         prediction_trainable: bool = True,
         joint_dim: int = 1024,
         joint_activation: str = "tanh",
-        prejoint_linear: bool = True,
-        postjoint_linear: bool = False,
         joint_mode: str = "add",
         joint_trainable: bool = True,
+        prejoint_encoder_linear: bool = True,
+        prejoint_prediction_linear: bool = True,
+        postjoint_linear: bool = False,
         kernel_regularizer=None,
         bias_regularizer=None,
         name="transducer",
         **kwargs,
     ):
-        super().__init__(name=name, **kwargs)
+        super().__init__(speech_config=speech_config, name=name, **kwargs)
+        self.blank = blank
         self.encoder = encoder
         self.predict_net = TransducerPrediction(
-            vocabulary_size=vocabulary_size,
-            embed_dim=embed_dim,
-            embed_dropout=embed_dropout,
-            num_rnns=num_rnns,
-            rnn_units=rnn_units,
-            rnn_type=rnn_type,
-            rnn_implementation=rnn_implementation,
-            layer_norm=layer_norm,
-            projection_units=projection_units,
+            blank=blank,
+            vocab_size=vocab_size,
+            label_encoder_mode=prediction_label_encoder_mode,
+            embed_dim=prediction_embed_dim,
+            num_rnns=prediction_num_rnns,
+            rnn_units=prediction_rnn_units,
+            rnn_type=prediction_rnn_type,
+            rnn_implementation=prediction_rnn_implementation,
+            rnn_unroll=prediction_rnn_unroll,
+            layer_norm=prediction_layer_norm,
+            projection_units=prediction_projection_units,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             trainable=prediction_trainable,
-            name=f"{name}_prediction",
+            name="prediction",
+            dtype=self.dtype,
         )
         self.joint_net = TransducerJoint(
-            vocabulary_size=vocabulary_size,
+            vocab_size=vocab_size,
             joint_dim=joint_dim,
             activation=joint_activation,
-            prejoint_linear=prejoint_linear,
+            prejoint_encoder_linear=prejoint_encoder_linear,
+            prejoint_prediction_linear=prejoint_prediction_linear,
             postjoint_linear=postjoint_linear,
             joint_mode=joint_mode,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             trainable=joint_trainable,
-            name=f"{name}_joint",
+            name="joint",
+            dtype=self.dtype,
         )
         self.time_reduction_factor = 1
 
-    def make(
-        self,
-        input_shape,
-        prediction_shape=[None],
-        batch_size=None,
-    ):
-        inputs = tf.keras.Input(shape=input_shape, batch_size=batch_size, dtype=tf.float32)
-        inputs_length = tf.keras.Input(shape=[], batch_size=batch_size, dtype=tf.int32)
-        predictions = tf.keras.Input(shape=prediction_shape, batch_size=batch_size, dtype=tf.int32)
-        predictions_length = tf.keras.Input(shape=[], batch_size=batch_size, dtype=tf.int32)
-        self(
-            data_util.create_inputs(
-                inputs=inputs,
-                inputs_length=inputs_length,
-                predictions=predictions,
-                predictions_length=predictions_length,
-            ),
-            training=False,
-        )
-
-    def summary(
-        self,
-        line_length=None,
-        **kwargs,
-    ):
-        if self.encoder is not None:
-            self.encoder.summary(line_length=line_length, **kwargs)
-        self.predict_net.summary(line_length=line_length, **kwargs)
-        self.joint_net.summary(line_length=line_length, **kwargs)
-        super().summary(line_length=line_length, **kwargs)
-
-    def add_featurizers(
-        self,
-        speech_featurizer: SpeechFeaturizer,
-        text_featurizer: TextFeaturizer,
-    ):
-        """
-        Function to add featurizer to model to convert to end2end tflite
-        Args:
-            speech_featurizer: SpeechFeaturizer instance
-            text_featurizer: TextFeaturizer instance
-            scorer: external language model scorer
-        """
-        self.speech_featurizer = speech_featurizer
-        self.text_featurizer = text_featurizer
+    def compile(self, optimizer, output_shapes=None, **kwargs):
+        loss = RnntLoss(blank=self.blank, output_shapes=output_shapes, name="rnnt_loss")
+        return super().compile(loss, optimizer, **kwargs)
+
+    def apply_gwn(self):
+        if self.gwn_config:
+            original_weights = {}
+            if self.gwn_config.get("encoder_step") is not None and self.gwn_config.get("encoder_stddev") is not None:
+                original_weights["encoder"] = tf.cond(
+                    tf.greater_equal(self.optimizer.iterations, self.gwn_config["encoder_step"]),
+                    lambda: layer_util.add_gwn(self.encoder.trainable_weights, stddev=self.gwn_config["encoder_stddev"]),
+                    lambda: self.encoder.trainable_weights,
+                )
+            if self.gwn_config.get("predict_net_step") is not None and self.gwn_config.get("predict_net_stddev") is not None:
+                original_weights["predict_net"] = tf.cond(
+                    tf.greater_equal(self.optimizer.iterations, self.gwn_config["predict_net_step"]),
+                    lambda: layer_util.add_gwn(self.predict_net.trainable_weights, stddev=self.gwn_config["predict_net_stddev"]),
+                    lambda: self.predict_net.trainable_weights,
+                )
+            if self.gwn_config.get("joint_net_step") is not None and self.gwn_config.get("joint_net_stddev") is not None:
+                original_weights["joint_net"] = tf.cond(
+                    tf.greater_equal(self.optimizer.iterations, self.gwn_config["joint_net_step"]),
+                    lambda: layer_util.add_gwn(self.joint_net.trainable_weights, stddev=self.gwn_config["joint_net_stddev"]),
+                    lambda: self.joint_net.trainable_weights,
+                )
+            return original_weights
+        return {}
 
-    def compile(
-        self,
-        optimizer,
-        global_batch_size,
-        blank=0,
-        run_eagerly=None,
-        **kwargs,
-    ):
-        loss = RnntLoss(blank=blank, global_batch_size=global_batch_size)
-        super().compile(loss=loss, optimizer=optimizer, run_eagerly=run_eagerly, **kwargs)
+    def remove_gwn(self, original_weights):
+        if self.gwn_config:
+            if original_weights.get("encoder") is not None:
+                tf.cond(
+                    tf.greater_equal(self.optimizer.iterations, self.gwn_config["encoder_step"]),
+                    lambda: layer_util.sub_gwn(original_weights["encoder"], self.encoder.trainable_weights),
+                    lambda: None,
+                )
+            if original_weights.get("predict_net") is not None:
+                tf.cond(
+                    tf.greater_equal(self.optimizer.iterations, self.gwn_config["predict_net_step"]),
+                    lambda: layer_util.sub_gwn(original_weights["predict_net"], self.predict_net.trainable_weights),
+                    lambda: None,
+                )
+            if original_weights.get("joint_net") is not None:
+                tf.cond(
+                    tf.greater_equal(self.optimizer.iterations, self.gwn_config["joint_net_step"]),
+                    lambda: layer_util.sub_gwn(original_weights["joint_net"], self.joint_net.trainable_weights),
+                    lambda: None,
+                )
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        enc = self.encoder(inputs["inputs"], training=training, **kwargs)
-        pred = self.predict_net([inputs["predictions"], inputs["predictions_length"]], training=training, **kwargs)
-        logits = self.joint_net([enc, pred], training=training, **kwargs)
-        return data_util.create_logits(
+    def call(self, inputs: schemas.TrainInput, training=False):
+        features, features_length = self.feature_extraction((inputs["inputs"], inputs["inputs_length"]), training=training)
+        enc, logits_length, caching = self.encoder((features, features_length, inputs.get("caching")), training=training)
+        pred, _ = self.predict_net((inputs["predictions"], inputs["predictions_length"]), training=training)
+        logits = self.joint_net((enc, pred), training=training)
+        return schemas.TrainOutput(
             logits=logits,
-            logits_length=math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor),
+            logits_length=logits_length,
+            caching=caching,
         )
 
-    # -------------------------------- INFERENCES -------------------------------------
-
-    def encoder_inference(
+    def call_next(
         self,
-        features: tf.Tensor,
+        current_frames: tf.Tensor,
+        previous_tokens: tf.Tensor,
+        previous_decoder_states: tf.Tensor,
     ):
-        """Infer function for encoder (or encoders)
-
-        Args:
-            features (tf.Tensor): features with shape [T, F, C]
-
-        Returns:
-            tf.Tensor: output of encoders with shape [T, E]
         """
-        with tf.name_scope(f"{self.name}_encoder"):
-            outputs = tf.expand_dims(features, axis=0)
-            outputs = self.encoder(outputs, training=False)
-            return tf.squeeze(outputs, axis=0)
-
-    def decoder_inference(
-        self,
-        encoded: tf.Tensor,
-        predicted: tf.Tensor,
-        states: tf.Tensor,
-        tflite: bool = False,
-    ):
-        """Infer function for decoder
+        Decode current frame given previous predicted token and states
 
-        Args:
-            encoded (tf.Tensor): output of encoder at each time step => shape [E]
-            predicted (tf.Tensor): last character index of predicted sequence => shape []
-            states (nested lists of tf.Tensor): states returned by rnn layers
-
-        Returns:
-            (ytu, new_states)
-        """
-        with tf.name_scope(f"{self.name}_decoder"):
-            encoded = tf.reshape(encoded, [1, 1, -1])  # [E] => [1, 1, E]
-            predicted = tf.reshape(predicted, [1, 1])  # [] => [1, 1]
-            y, new_states = self.predict_net.recognize(predicted, states, tflite=tflite)  # [1, 1, P], states
-            ytu = tf.nn.log_softmax(self.joint_net([encoded, y], training=False))  # [1, 1, V]
-            ytu = tf.reshape(ytu, shape=[-1])  # [1, 1, V] => [V]
+        Parameters
+        ----------
+        current_frames : tf.Tensor, shape [B, 1, E]
+            Output of the encoder network of the current frame
+        previous_tokens : tf.Tensor, shape [B, 1]
+            Predicted token of the previous frame
+        previous_decoder_states : tf.Tensor, shape [B, num_rnns, nstates, state_size]
+            States got from previous frame
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor], shapes ([B, 1, 1, V], [B, num_rnns, nstates, state_size])
+            Output of joint network of the current frame, new states of prediction network
+        """
+        with tf.name_scope(f"{self.name}_call_next"):
+            y, new_states = self.predict_net.call_next(previous_tokens, previous_decoder_states)
+            ytu = self.joint_net([current_frames, y], training=False)
+            ytu = tf.nn.log_softmax(ytu)
             return ytu, new_states
 
-    def get_config(self):
-        conf = self.encoder.get_config()
-        conf.update(self.predict_net.get_config())
-        conf.update(self.joint_net.get_config())
-        return conf
-
     # -------------------------------- GREEDY -------------------------------------
 
-    @tf.function
-    def recognize(
-        self,
-        inputs: Dict[str, tf.Tensor],
-    ):
+    def recognize(self, inputs: schemas.PredictInput, max_tokens_per_frame: int = 3, **kwargs):
         """
-        RNN Transducer Greedy decoding
-        Args:
-            features (tf.Tensor): a batch of extracted features
-            input_length (tf.Tensor): a batch of extracted features length
-
-        Returns:
-            tf.Tensor: a batch of decoded transcripts
-        """
-        encoded = self.encoder(inputs["inputs"], training=False)
-        encoded_length = math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor)
-        return self._perform_greedy_batch(encoded=encoded, encoded_length=encoded_length)
-
-    def recognize_tflite(
-        self,
-        signal,
-        predicted,
-        states,
-    ):
-        """
-        Function to convert to tflite using greedy decoding (default streaming mode)
-        Args:
-            signal: tf.Tensor with shape [None] indicating a single audio signal
-            predicted: last predicted character with shape []
-            states: lastest rnn states with shape [num_rnns, 1 or 2, 1, P]
-
-        Return:
-            transcript: tf.Tensor of Unicode Code Points with shape [None] and dtype tf.int32
-            predicted: last predicted character with shape []
-            states: lastest rnn states with shape [num_rnns, 1 or 2, 1, P]
-        """
-        features = self.speech_featurizer.tf_extract(signal)
-        encoded = self.encoder_inference(features)
-        hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, states, tflite=True)
-        transcript = self.text_featurizer.indices2upoints(hypothesis.prediction)
-        return transcript, hypothesis.index, hypothesis.states
-
-    def recognize_tflite_with_timestamp(
-        self,
-        signal,
-        predicted,
-        states,
-    ):
-        features = self.speech_featurizer.tf_extract(signal)
-        encoded = self.encoder_inference(features)
-        hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, states, tflite=True)
-        indices = self.text_featurizer.normalize_indices(hypothesis.prediction)
-        upoints = tf.gather_nd(self.text_featurizer.upoints, tf.expand_dims(indices, axis=-1))  # [None, max_subword_length]
-
-        num_samples = tf.cast(tf.shape(signal)[0], dtype=tf.float32)
-        total_time_reduction_factor = self.time_reduction_factor * self.speech_featurizer.frame_step
-
-        stime = tf.range(0, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
-        stime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
-
-        etime = tf.range(total_time_reduction_factor, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
-        etime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
-
-        non_blank = tf.where(tf.not_equal(upoints, 0))
-        non_blank_transcript = tf.gather_nd(upoints, non_blank)
-        non_blank_stime = tf.gather_nd(tf.repeat(tf.expand_dims(stime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
-        non_blank_etime = tf.gather_nd(tf.repeat(tf.expand_dims(etime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
+        Recognize greedy from input signals
 
-        return non_blank_transcript, non_blank_stime, non_blank_etime, hypothesis.index, hypothesis.states
-
-    def _perform_greedy_batch(
-        self,
-        encoded: tf.Tensor,
-        encoded_length: tf.Tensor,
-        parallel_iterations: int = 10,
-        swap_memory: bool = False,
-    ):
-        with tf.name_scope(f"{self.name}_perform_greedy_batch"):
-            total_batch = tf.shape(encoded)[0]
-            batch = tf.constant(0, dtype=tf.int32)
-
-            decoded = tf.TensorArray(
-                dtype=tf.int32,
-                size=total_batch,
-                dynamic_size=False,
-                clear_after_read=False,
-                element_shape=tf.TensorShape([None]),
+        Parameters
+        ----------
+        inputs : schemas.PredictInput
+
+        Returns
+        -------
+        named tuple of
+            (
+                tokens, will be feed to text_featurizer.detokenize or text_featurizer.detokenize_unicode_points,
+                next_encoder_states, if encoder does not have states, returns None, will be used to predict next chunk of audio,
+                next_tokens, will be used to predict next chunk of audio,
+                next_decoder_states, next states of predict_net, will be used to predict next chunk of audio,
             )
+        """
+        return tf.cond(
+            tf.equal(tf.shape(inputs.inputs_length)[0], 1),
+            lambda: self.recognize_single(inputs, max_tokens_per_frame=max_tokens_per_frame, **kwargs),
+            lambda: self.recognize_batch(inputs, **kwargs),
+        )
 
-            def condition(batch, _):
-                return tf.less(batch, total_batch)
-
-            def body(batch, decoded):
-                hypothesis = self._perform_greedy(
-                    encoded=encoded[batch],
-                    encoded_length=encoded_length[batch],
-                    predicted=tf.constant(self.text_featurizer.blank, dtype=tf.int32),
-                    states=self.predict_net.get_initial_state(),
-                    parallel_iterations=parallel_iterations,
-                    swap_memory=swap_memory,
+    def recognize_batch(self, inputs: schemas.PredictInput, **kwargs):
+        """
+        Ref: https://arxiv.org/pdf/1801.00841.pdf
+        This is a greedy decoding algorithm that greedily select the best token at each time step
+        Only apply for batch size > 1
+        """
+        with tf.name_scope(f"{self.name}_recognize"):
+            features, features_length = self.feature_extraction((inputs.inputs, inputs.inputs_length), training=False)
+            encoded, encoded_length, next_encoder_states = self.encoder.call_next(features, features_length, inputs.previous_encoder_states)
+
+            nframes = tf.expand_dims(encoded_length, axis=-1)  # [B, 1]
+            batch_size, max_frames, _ = shape_util.shape_list(encoded)
+            # The current indices of the output of encoder, shape [B, 1]
+            frame_indices = tf.zeros([batch_size, 1], dtype=tf.int32, name="frame_indices")
+            # Previous predicted tokens, initially are blanks, shape [B, 1]
+            previous_tokens = inputs.previous_tokens or tf.ones([batch_size, 1], dtype=tf.int32, name="previous_tokens") * self.blank
+            # Previous states of the prediction network, initially are zeros, shape [B, num_rnns, nstates, rnn_units]
+            previous_decoder_states = inputs.previous_decoder_states or self.predict_net.get_initial_state(batch_size)
+            # Assumption that number of tokens can not exceed (2 * the size of output of encoder + 1), this is for static runs like TPU or TFLite
+            max_tokens = max_frames * 2 + 1
+            # All of the tokens that are getting recognized, initially are blanks, shape [B, nframes * 2 + 1]
+            tokens = tf.ones([batch_size, max_tokens], dtype=tf.int32, name="tokens") * self.blank
+            # The current indices of the token that are currently being recognized, shape [B, 1], the tokens indices are started with 1 so that any
+            # blank token recognized got updated to index 0 to avoid affecting results
+            tokens_indices = tf.ones([batch_size, 1], dtype=tf.int32, name="tokens_indices")
+
+            def cond(_frame_indices, _previous_tokens, _previous_decoder_states, _tokens, _tokens_indices):
+                return tf.logical_not(  # Reversed so that the loop check and continue
+                    # One of the following condition met will terminate the loop
+                    tf.logical_or(
+                        # Stop when ALL of the indices of the output of the encoder reach the end
+                        tf.math.reduce_all(tf.greater_equal(_frame_indices, nframes - 1)),
+                        # Stop when ALL of the indices of recognized tokens reach the end
+                        tf.math.reduce_all(tf.greater_equal(_tokens_indices, max_tokens - 1)),
+                    )
                 )
-                decoded = decoded.write(batch, hypothesis.prediction)
-                return batch + 1, decoded
-
-            batch, decoded = tf.while_loop(
-                condition,
-                body,
-                loop_vars=[batch, decoded],
-                parallel_iterations=parallel_iterations,
-                swap_memory=True,
-            )
-
-            decoded = math_util.pad_prediction_tfarray(decoded, blank=self.text_featurizer.blank)
-            return self.text_featurizer.iextract(decoded.stack())
-
-    def _perform_greedy(
-        self,
-        encoded: tf.Tensor,
-        encoded_length: tf.Tensor,
-        predicted: tf.Tensor,
-        states: tf.Tensor,
-        parallel_iterations: int = 10,
-        swap_memory: bool = False,
-        tflite: bool = False,
-    ):
-        with tf.name_scope(f"{self.name}_greedy"):
-            time = tf.constant(0, dtype=tf.int32)
-            total = encoded_length
-
-            hypothesis = Hypothesis(
-                index=predicted,
-                prediction=tf.TensorArray(
-                    dtype=tf.int32,
-                    size=total,
-                    dynamic_size=False,
-                    clear_after_read=False,
-                    element_shape=tf.TensorShape([]),
-                ),
-                states=states,
-            )
 
-            def condition(_time, _hypothesis):
-                return tf.less(_time, total)
-
-            def body(_time, _hypothesis):
-                ytu, _states = self.decoder_inference(
-                    # avoid using [index] in tflite
-                    encoded=tf.gather_nd(encoded, tf.reshape(_time, shape=[1])),
-                    predicted=_hypothesis.index,
-                    states=_hypothesis.states,
-                    tflite=tflite,
+            def body(_frame_indices, _previous_tokens, _previous_decoder_states, _tokens, _tokens_indices):
+                _current_frames = tf.expand_dims(tf.gather_nd(encoded, tf.minimum(_frame_indices, nframes - 1), batch_dims=1), axis=1)  # [B, 1, E]
+                _log_softmax, _states = self.call_next(_current_frames, _previous_tokens, _previous_decoder_states)
+                _current_tokens = tf.reshape(tf.argmax(_log_softmax, axis=-1, output_type=tf.int32), [batch_size, 1])  # [B, 1, 1] -> [B, 1]
+                # conditions, blanks are ignored
+                _equal_blank = tf.equal(_current_tokens, self.blank)  # [B, 1]
+                # if the token index >= max tokens, it's already finished, set to blank to ignore
+                _equal_blank = tf.logical_or(_equal_blank, tf.greater_equal(_tokens_indices, max_tokens))
+                # if the frame index > nframes, it's already done, set to blank to ignore
+                _equal_blank = tf.logical_or(_equal_blank, tf.greater(_frame_indices, nframes))
+                # update results
+                _update_tokens = tf.reshape(tf.where(_equal_blank, self.blank, _current_tokens), [batch_size])  # [B]
+                _update_tokens_indices = tf.where(
+                    _equal_blank, 0, tf.minimum(tf.add(_tokens_indices, 1), max_tokens - 1)
+                )  # blanks are getting updated at index 0 to avoid affecting results
+                _tokens = tf.tensor_scatter_nd_update(
+                    tensor=_tokens,
+                    indices=tf.concat([tf.expand_dims(tf.range(batch_size, dtype=tf.int32), axis=-1), _update_tokens_indices], -1),  # [B, 2]
+                    updates=_update_tokens,  # [B]
                 )
-                _predict = tf.argmax(ytu, axis=-1, output_type=tf.int32)  # => argmax []
-
-                # something is wrong with tflite that drop support for tf.cond
-                # def equal_blank_fn(): return _hypothesis.index, _hypothesis.states
-                # def non_equal_blank_fn(): return _predict, _states  # update if the new prediction is a non-blank
-                # _index, _states = tf.cond(tf.equal(_predict, blank), equal_blank_fn, non_equal_blank_fn)
-
-                _equal = tf.equal(_predict, self.text_featurizer.blank)
-                _index = tf.where(_equal, _hypothesis.index, _predict)
-                _states = tf.where(_equal, _hypothesis.states, _states)
-
-                _prediction = _hypothesis.prediction.write(_time, _predict)
-                _hypothesis = Hypothesis(index=_index, prediction=_prediction, states=_states)
-
-                return _time + 1, _hypothesis
-
-            time, hypothesis = tf.while_loop(
-                condition,
-                body,
-                loop_vars=[time, hypothesis],
-                parallel_iterations=parallel_iterations,
-                swap_memory=swap_memory,
-            )
-
-            return Hypothesis(
-                index=hypothesis.index,
-                prediction=hypothesis.prediction.stack(),
-                states=hypothesis.states,
+                _tokens_indices = tf.where(_equal_blank, _tokens_indices, tf.minimum(tf.add(_tokens_indices, 1), max_tokens - 1))
+                # update states
+                _frame_indices = tf.where(_equal_blank, tf.add(_frame_indices, 1), _frame_indices)  # blank then next frames, else current frames
+                _previous_tokens = tf.where(_equal_blank, _previous_tokens, _current_tokens)  # blank then keep prev tokens, else next tokens
+                _previous_decoder_states = tf.where(
+                    tf.reshape(_equal_blank, [batch_size, 1, 1, 1]), _previous_decoder_states, _states
+                )  # blank then keep prev states, else next states # pylint: disable=line-too-long
+                return _frame_indices, _previous_tokens, _previous_decoder_states, _tokens, _tokens_indices
+
+            (
+                frame_indices,
+                next_tokens,
+                next_decoder_states,
+                tokens,
+                tokens_indices,
+            ) = tf.while_loop(cond, body, loop_vars=(frame_indices, previous_tokens, previous_decoder_states, tokens, tokens_indices))
+
+            return schemas.PredictOutput(
+                tokens=tokens,
+                next_tokens=next_tokens,
+                next_encoder_states=next_encoder_states,
+                next_decoder_states=next_decoder_states,
             )
 
-    def _perform_greedy_v2(
-        self,
-        encoded: tf.Tensor,
-        encoded_length: tf.Tensor,
-        predicted: tf.Tensor,
-        states: tf.Tensor,
-        parallel_iterations: int = 10,
-        swap_memory: bool = False,
-        tflite: bool = False,
-    ):
-        """Ref: https://arxiv.org/pdf/1801.00841.pdf"""
-        with tf.name_scope(f"{self.name}_greedy_v2"):
-            time = tf.constant(0, dtype=tf.int32)
-            total = encoded_length
-
-            hypothesis = Hypothesis(
-                index=predicted,
-                prediction=tf.TensorArray(
-                    dtype=tf.int32,
-                    size=0,
-                    dynamic_size=True,
-                    clear_after_read=False,
-                    element_shape=tf.TensorShape([]),
-                ),
-                states=states,
-            )
-
-            def condition(_time, _hypothesis):
-                return tf.less(_time, total)
-
-            def body(_time, _hypothesis):
-                ytu, _states = self.decoder_inference(
-                    # avoid using [index] in tflite
-                    encoded=tf.gather_nd(encoded, tf.reshape(_time, shape=[1])),
-                    predicted=_hypothesis.index,
-                    states=_hypothesis.states,
-                    tflite=tflite,
-                )
-                _predict = tf.argmax(ytu, axis=-1, output_type=tf.int32)  # => argmax []
-
-                _equal = tf.equal(_predict, self.text_featurizer.blank)
-                _index = tf.where(_equal, _hypothesis.index, _predict)
-                _states = tf.where(_equal, _hypothesis.states, _states)
-                _time = tf.where(_equal, _time + 1, _time)
-
-                _prediction = _hypothesis.prediction.write(_time, _predict)
-                _hypothesis = Hypothesis(index=_index, prediction=_prediction, states=_states)
-
-                return _time, _hypothesis
-
-            time, hypothesis = tf.while_loop(
-                condition,
-                body,
-                loop_vars=[time, hypothesis],
-                parallel_iterations=parallel_iterations,
-                swap_memory=swap_memory,
-            )
-
-            return Hypothesis(
-                index=hypothesis.index,
-                prediction=hypothesis.prediction.stack(),
-                states=hypothesis.states,
-            )
-
-    # -------------------------------- BEAM SEARCH -------------------------------------
-
-    @tf.function
-    def recognize_beam(
-        self,
-        inputs: Dict[str, tf.Tensor],
-        lm: bool = False,
-    ):
+    def recognize_single(self, inputs: schemas.PredictInput, max_tokens_per_frame: int = 3, **kwargs):
         """
-        RNN Transducer Beam Search
-        Args:
-            inputs (Dict[str, tf.Tensor]): Input dictionary containing "inputs" and "inputs_length"
-            lm (bool, optional): whether to use language model. Defaults to False.
-
-        Returns:
-            tf.Tensor: a batch of decoded transcripts
-        """
-        encoded = self.encoder(inputs["inputs"], training=False)
-        encoded_length = math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor)
-        return self._perform_beam_search_batch(
-            encoded=encoded,
-            encoded_length=encoded_length,
-            lm=lm,
-        )
-
-    def _perform_beam_search_batch(
-        self,
-        encoded: tf.Tensor,
-        encoded_length: tf.Tensor,
-        lm: bool = False,
-        parallel_iterations: int = 10,
-        swap_memory: bool = True,
-    ):
-        with tf.name_scope(f"{self.name}_perform_beam_search_batch"):
-            total_batch = tf.shape(encoded)[0]
-            batch = tf.constant(0, dtype=tf.int32)
-
-            decoded = tf.TensorArray(
+        Ref: https://arxiv.org/pdf/1801.00841.pdf
+        This is a greedy decoding algorithm that greedily select the best token at each time step
+        Only apply for batch size 1
+        """
+        with tf.name_scope(f"{self.name}_decode_greedy"):
+            features, features_length = self.feature_extraction((inputs.inputs, inputs.inputs_length), training=False)
+            encoded, encoded_length, next_encoder_states = self.encoder.call_next(features, features_length, inputs.previous_encoder_states)
+
+            frame = tf.zeros([1, 1], dtype=tf.int32)
+            nframes = encoded_length
+
+            previous_tokens = inputs.previous_tokens or tf.ones([1, 1], dtype=tf.int32) * self.blank
+            token_index = tf.ones([], dtype=tf.int32) * -1
+            tokens = tf.TensorArray(
                 dtype=tf.int32,
-                size=total_batch,
+                size=tf.reshape(nframes, shape=[]) * max_tokens_per_frame,
                 dynamic_size=False,
                 clear_after_read=False,
-                element_shape=None,
+                element_shape=tf.TensorShape([]),
             )
-
-            def condition(batch, _):
-                return tf.less(batch, total_batch)
-
-            def body(batch, decoded):
-                hypothesis = self._perform_beam_search(
-                    encoded[batch],
-                    encoded_length[batch],
-                    lm,
-                    parallel_iterations=parallel_iterations,
-                    swap_memory=swap_memory,
-                )
-                decoded = decoded.write(batch, hypothesis.prediction)
-                return batch + 1, decoded
-
-            batch, decoded = tf.while_loop(
-                condition,
-                body,
-                loop_vars=[batch, decoded],
-                parallel_iterations=parallel_iterations,
-                swap_memory=True,
+            num_tokens_per_frame = tf.TensorArray(
+                dtype=tf.int32,
+                size=tf.reshape(nframes, shape=[]),
+                dynamic_size=False,
+                clear_after_read=False,
+                element_shape=tf.TensorShape([]),
             )
 
-            decoded = math_util.pad_prediction_tfarray(decoded, blank=self.text_featurizer.blank)
-            return self.text_featurizer.iextract(decoded.stack())
+            previous_decoder_states = inputs.previous_decoder_states or self.predict_net.get_initial_state(1)
 
-    def _perform_beam_search(
-        self,
-        encoded: tf.Tensor,
-        encoded_length: tf.Tensor,
-        lm: bool = False,
-        parallel_iterations: int = 10,
-        swap_memory: bool = True,
-        tflite: bool = False,
-    ):
-        with tf.name_scope(f"{self.name}_beam_search"):
-            beam_width = tf.cond(
-                tf.less(self.text_featurizer.decoder_config.beam_width, self.text_featurizer.num_classes),
-                true_fn=lambda: self.text_featurizer.decoder_config.beam_width,
-                false_fn=lambda: self.text_featurizer.num_classes - 1,
-            )
-            total = encoded_length
-
-            def initialize_beam(dynamic=False):
-                return BeamHypothesis(
-                    score=tf.TensorArray(
-                        dtype=tf.float32,
-                        size=beam_width if not dynamic else 0,
-                        dynamic_size=dynamic,
-                        element_shape=tf.TensorShape([]),
-                        clear_after_read=False,
-                    ),
-                    indices=tf.TensorArray(
-                        dtype=tf.int32,
-                        size=beam_width if not dynamic else 0,
-                        dynamic_size=dynamic,
-                        element_shape=tf.TensorShape([]),
-                        clear_after_read=False,
-                    ),
-                    prediction=tf.TensorArray(
-                        dtype=tf.int32,
-                        size=beam_width if not dynamic else 0,
-                        dynamic_size=dynamic,
-                        element_shape=None,
-                        clear_after_read=False,
-                    ),
-                    states=tf.TensorArray(
-                        dtype=tf.float32,
-                        size=beam_width if not dynamic else 0,
-                        dynamic_size=dynamic,
-                        element_shape=tf.TensorShape(shape_util.shape_list(self.predict_net.get_initial_state())),
-                        clear_after_read=False,
-                    ),
-                )
-
-            B = initialize_beam()
-            B = BeamHypothesis(
-                score=B.score.write(0, 0.0),
-                indices=B.indices.write(0, self.text_featurizer.blank),
-                prediction=B.prediction.write(0, tf.ones([total], dtype=tf.int32) * self.text_featurizer.blank),
-                states=B.states.write(0, self.predict_net.get_initial_state()),
-            )
-
-            def condition(time, total, B):
-                return tf.less(time, total)
-
-            def body(time, total, B):
-                A = initialize_beam(dynamic=True)
-                A = BeamHypothesis(
-                    score=A.score.unstack(B.score.stack()),
-                    indices=A.indices.unstack(B.indices.stack()),
-                    prediction=A.prediction.unstack(
-                        math_util.pad_prediction_tfarray(B.prediction, blank=self.text_featurizer.blank).stack()
-                    ),
-                    states=A.states.unstack(B.states.stack()),
-                )
-                A_i = tf.constant(0, tf.int32)
-                B = initialize_beam()
-
-                encoded_t = tf.gather_nd(encoded, tf.expand_dims(time, axis=-1))
-
-                def beam_condition(beam, beam_width, A, A_i, B):
-                    return tf.less(beam, beam_width)
-
-                def beam_body(beam, beam_width, A, A_i, B):
-                    # get y_hat
-                    y_hat_score, y_hat_score_index = tf.math.top_k(A.score.stack(), k=1, sorted=True)
-                    y_hat_score = y_hat_score[0]
-                    y_hat_index = tf.gather_nd(A.indices.stack(), y_hat_score_index)
-                    y_hat_prediction = tf.gather_nd(
-                        math_util.pad_prediction_tfarray(A.prediction, blank=self.text_featurizer.blank).stack(),
-                        y_hat_score_index,
-                    )
-                    y_hat_states = tf.gather_nd(A.states.stack(), y_hat_score_index)
-
-                    # remove y_hat from A
-                    remain_indices = tf.range(0, tf.shape(A.score.stack())[0], dtype=tf.int32)
-                    remain_indices = tf.gather_nd(remain_indices, tf.where(tf.not_equal(remain_indices, y_hat_score_index[0])))
-                    remain_indices = tf.expand_dims(remain_indices, axis=-1)
-                    A = BeamHypothesis(
-                        score=A.score.unstack(tf.gather_nd(A.score.stack(), remain_indices)),
-                        indices=A.indices.unstack(tf.gather_nd(A.indices.stack(), remain_indices)),
-                        prediction=A.prediction.unstack(
-                            tf.gather_nd(
-                                math_util.pad_prediction_tfarray(A.prediction, blank=self.text_featurizer.blank).stack(),
-                                remain_indices,
-                            )
-                        ),
-                        states=A.states.unstack(tf.gather_nd(A.states.stack(), remain_indices)),
-                    )
-                    A_i = tf.cond(tf.equal(A_i, 0), true_fn=lambda: A_i, false_fn=lambda: A_i - 1)
-
-                    ytu, new_states = self.decoder_inference(
-                        encoded=encoded_t, predicted=y_hat_index, states=y_hat_states, tflite=tflite
-                    )
-
-                    def predict_condition(pred, A, A_i, B):
-                        return tf.less(pred, self.text_featurizer.num_classes)
-
-                    def predict_body(pred, A, A_i, B):
-                        new_score = y_hat_score + tf.gather_nd(ytu, tf.expand_dims(pred, axis=-1))
-
-                        def true_fn():
-                            return (
-                                B.score.write(beam, new_score),
-                                B.indices.write(beam, y_hat_index),
-                                B.prediction.write(beam, y_hat_prediction),
-                                B.states.write(beam, y_hat_states),
-                                A.score,
-                                A.indices,
-                                A.prediction,
-                                A.states,
-                                A_i,
-                            )
-
-                        def false_fn():
-                            scatter_index = math_util.count_non_blank(y_hat_prediction, blank=self.text_featurizer.blank)
-                            updated_prediction = tf.tensor_scatter_nd_update(
-                                y_hat_prediction,
-                                indices=tf.reshape(scatter_index, [1, 1]),
-                                updates=tf.expand_dims(pred, axis=-1),
-                            )
-                            return (
-                                B.score,
-                                B.indices,
-                                B.prediction,
-                                B.states,
-                                A.score.write(A_i, new_score),
-                                A.indices.write(A_i, pred),
-                                A.prediction.write(A_i, updated_prediction),
-                                A.states.write(A_i, new_states),
-                                A_i + 1,
-                            )
-
-                        b_score, b_indices, b_prediction, b_states, a_score, a_indices, a_prediction, a_states, A_i = tf.cond(
-                            tf.equal(pred, self.text_featurizer.blank), true_fn=true_fn, false_fn=false_fn
-                        )
-
-                        B = BeamHypothesis(score=b_score, indices=b_indices, prediction=b_prediction, states=b_states)
-                        A = BeamHypothesis(score=a_score, indices=a_indices, prediction=a_prediction, states=a_states)
-
-                        return pred + 1, A, A_i, B
-
-                    _, A, A_i, B = tf.while_loop(
-                        predict_condition,
-                        predict_body,
-                        loop_vars=[0, A, A_i, B],
-                        parallel_iterations=parallel_iterations,
-                        swap_memory=swap_memory,
-                    )
-
-                    return beam + 1, beam_width, A, A_i, B
+            def condition(
+                _frame,
+                _nframes,
+                _previous_tokens,
+                _token_index,
+                _tokens,
+                _num_tokens_per_frame,
+                _max_tokens_per_frame,
+                _previous_decoder_states,
+            ):
+                return tf.less(_frame, _nframes)
+
+            def body(
+                _frame,
+                _nframes,
+                _previous_tokens,
+                _token_index,
+                _tokens,
+                _num_tokens_per_frame,
+                _max_tokens_per_frame,
+                _previous_decoder_states,
+            ):
+                _current_frame = tf.expand_dims(tf.gather_nd(encoded, _frame, batch_dims=1), axis=1)  # [1, 1, E]
+                _log_softmax, _states = self.call_next(_current_frame, _previous_tokens, _previous_decoder_states)
+                _current_tokens = tf.reshape(tf.argmax(_log_softmax, axis=-1, output_type=tf.int32), [1, 1])  # [1, 1, 1] -> [1, 1]
+
+                ##################### conditions, blanks are ignored
+                _equal_blank = tf.equal(_current_tokens, self.blank)  # [1, 1]
+
+                ##################### step updates
+                __frame_index = tf.reshape(_frame, shape=[])
+                __equal_blank_index = tf.reshape(_equal_blank, shape=[])
+                # only non-blank tokens are counted in number of tokens per frame
+                _current_frame_num_tokens = tf.where(
+                    __equal_blank_index,
+                    _num_tokens_per_frame.read(__frame_index),
+                    tf.add(_num_tokens_per_frame.read(__frame_index), 1),
+                )
+                _num_tokens_per_frame = _num_tokens_per_frame.write(__frame_index, _current_frame_num_tokens)
+                # increase frame index if current tokens are blank or number of tokens per frame exceeds max tokens per frame
+                _frame = tf.where(
+                    tf.logical_or(_equal_blank, tf.greater_equal(_current_frame_num_tokens, _max_tokens_per_frame)),
+                    tf.add(_frame, 1),
+                    _frame,
+                )
+                # increase token index if current token is not blank, so that it can be appended to tokens array
+                _token_index = tf.where(__equal_blank_index, _token_index, tf.add(_token_index, 1))
 
-                _, _, A, A_i, B = tf.while_loop(
-                    beam_condition,
-                    beam_body,
-                    loop_vars=[0, beam_width, A, A_i, B],
-                    parallel_iterations=parallel_iterations,
-                    swap_memory=swap_memory,
+                ##################### content updates
+                # keep previous tokens if current tokens are blank
+                _current_tokens = tf.where(_equal_blank, _previous_tokens, _current_tokens)
+                # keep previous states if current tokens are blank
+                _states = tf.where(tf.reshape(_equal_blank, [1, 1, 1, 1]), _previous_decoder_states, _states)
+                # token_index initialized as -1, so that the first recognized token will be at index 0
+                # therefore only update (append) tokens when token_index >= 0
+                _tokens = tf.cond(
+                    tf.greater_equal(_token_index, 0),
+                    lambda: _tokens.write(_token_index, tf.reshape(_current_tokens, shape=[])),
+                    lambda: _tokens,
                 )
 
-                return time + 1, total, B
+                ##################### return
+                return (
+                    _frame,
+                    _nframes,
+                    _current_tokens,
+                    _token_index,
+                    _tokens,
+                    _num_tokens_per_frame,
+                    _max_tokens_per_frame,
+                    _states,
+                )
 
-            _, _, B = tf.while_loop(
+            (
+                frame,
+                nframes,
+                next_tokens,
+                token_index,
+                tokens,
+                num_tokens_per_frame,
+                max_tokens_per_frame,
+                next_decoder_states,
+            ) = tf.while_loop(
                 condition,
                 body,
-                loop_vars=[0, total, B],
-                parallel_iterations=parallel_iterations,
-                swap_memory=swap_memory,
+                loop_vars=(
+                    frame,
+                    nframes,
+                    previous_tokens,
+                    token_index,
+                    tokens,
+                    num_tokens_per_frame,
+                    max_tokens_per_frame,
+                    previous_decoder_states,
+                ),
+                back_prop=False,
             )
 
-            scores = B.score.stack()
-            prediction = math_util.pad_prediction_tfarray(B.prediction, blank=self.text_featurizer.blank).stack()
-            if self.text_featurizer.decoder_config.norm_score:
-                prediction_lengths = math_util.count_non_blank(prediction, blank=self.text_featurizer.blank, axis=1)
-                scores /= tf.cast(prediction_lengths, dtype=scores.dtype)
+            return schemas.PredictOutput(
+                tokens=tf.reshape(tokens.stack(), shape=[1, -1]),
+                next_tokens=next_tokens,
+                next_encoder_states=next_encoder_states,
+                next_decoder_states=next_decoder_states,
+            )
 
-            y_hat_score, y_hat_score_index = tf.math.top_k(scores, k=1)
-            y_hat_score = y_hat_score[0]
-            y_hat_index = tf.gather_nd(B.indices.stack(), y_hat_score_index)
-            y_hat_prediction = tf.gather_nd(prediction, y_hat_score_index)
-            y_hat_states = tf.gather_nd(B.states.stack(), y_hat_score_index)
+    # def recognize_tflite_with_timestamp(self, signal, predicted, states):
+    #     features = self.speech_featurizer.tf_extract(signal)
+    #     encoded = self.encoder_inference(features)
+    #     hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, states, tflite=True)
+    #     indices = self.text_featurizer.normalize_indices(hypothesis.prediction)
+    #     upoints = tf.gather_nd(self.text_featurizer.upoints, tf.expand_dims(indices, axis=-1))  # [None, max_subword_length]
+
+    #     num_samples = tf.cast(tf.shape(signal)[0], dtype=tf.float32)
+    #     total_time_reduction_factor = self.time_reduction_factor * self.speech_featurizer.frame_step
+
+    #     stime = tf.range(0, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
+    #     stime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
+
+    #     etime = tf.range(total_time_reduction_factor, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
+    #     etime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
+
+    #     non_blank = tf.where(tf.not_equal(upoints, 0))
+    #     non_blank_transcript = tf.gather_nd(upoints, non_blank)
+    #     non_blank_stime = tf.gather_nd(tf.repeat(tf.expand_dims(stime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
+    #     non_blank_etime = tf.gather_nd(tf.repeat(tf.expand_dims(etime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
+
+    #     return non_blank_transcript, non_blank_stime, non_blank_etime, hypothesis.index, hypothesis.states
+
+    # def _perform_greedy_batch(
+    #     self,
+    #     encoded: tf.Tensor,
+    #     encoded_length: tf.Tensor,
+    #     parallel_iterations: int = 10,
+    #     swap_memory: bool = False,
+    # ):
+    #     with tf.name_scope("perform_greedy_batch"):
+    #         total_batch = tf.shape(encoded)[0]
+    #         batch = tf.constant(0, dtype=tf.int32)
+
+    #         decoded = tf.TensorArray(
+    #             dtype=tf.int32,
+    #             size=total_batch,
+    #             dynamic_size=False,
+    #             clear_after_read=False,
+    #             element_shape=tf.TensorShape([None]),
+    #         )
+
+    #         def condition(batch, _):
+    #             return tf.less(batch, total_batch)
+
+    #         def body(batch, decoded):
+    #             hypothesis = self._perform_greedy_v2(
+    #                 encoded=encoded[batch],
+    #                 encoded_length=encoded_length[batch],
+    #                 predicted=tf.constant(self.text_featurizer.blank, dtype=tf.int32),
+    #                 states=self.predict_net.get_initial_state(),
+    #                 parallel_iterations=parallel_iterations,
+    #                 swap_memory=swap_memory,
+    #             )
+    #             decoded = decoded.write(batch, hypothesis.prediction)
+    #             return batch + 1, decoded
+
+    #         batch, decoded = tf.while_loop(
+    #             condition,
+    #             body,
+    #             loop_vars=[batch, decoded],
+    #             parallel_iterations=parallel_iterations,
+    #             swap_memory=swap_memory,
+    #         )
+
+    #         decoded = math_util.pad_tfarray(decoded, blank=self.text_featurizer.blank)
+    #         return self.text_featurizer.detokenize(decoded.stack())
+
+    # def _perform_greedy(
+    #     self,
+    #     encoded: tf.Tensor,
+    #     encoded_length: tf.Tensor,
+    #     predicted: tf.Tensor,
+    #     states: tf.Tensor,
+    #     tflite: bool = False,
+    # ):
+    #     """Ref: https://arxiv.org/pdf/1801.00841.pdf"""
+    #     with tf.name_scope("greedy_v2"):
+    #         time = tf.constant(0, dtype=tf.int32)
+    #         pred_index = tf.constant(0, dtype=tf.int32)
+    #         total = encoded_length
+
+    #         hypothesis = Hypothesis(
+    #             index=predicted,
+    #             prediction=tf.TensorArray(
+    #                 dtype=tf.int32,
+    #                 size=(2 * total),
+    #                 dynamic_size=False,
+    #                 clear_after_read=False,
+    #                 element_shape=tf.TensorShape([]),
+    #             ),
+    #             states=states,
+    #         )
+
+    #         def condition(_time, _pred_index, _hypothesis):
+    #             return tf.logical_and(tf.less(_time, total), tf.less(_pred_index, 2 * total - 1))
+
+    #         def body(_time, _pred_index, _hypothesis):
+    #             ytu, _states = self.decoder_inference(
+    #                 encoded=tf.gather_nd(encoded, tf.reshape(_time, shape=[1])),  # avoid using [index] in tflite
+    #                 predicted=_hypothesis.index,
+    #                 states=_hypothesis.states,
+    #                 tflite=tflite,
+    #             )
+    #             _predict = tf.argmax(ytu, axis=-1, output_type=tf.int32)  # => argmax []
+
+    #             _equal_blank = tf.equal(_predict, self.text_featurizer.blank)
+    #             _time = tf.where(_equal_blank, _time + 1, _time)
+    #             _index = tf.where(_equal_blank, _hypothesis.index, _predict)
+    #             _states = tf.where(_equal_blank, _hypothesis.states, _states)
+    #             _pred_index = tf.where(_equal_blank, _pred_index, _pred_index + 1)
+    #             _prediction = _hypothesis.prediction.write(_pred_index, _index)
+
+    #             _hypothesis = Hypothesis(index=_index, prediction=_prediction, states=_states)
+
+    #             return _time, _pred_index, _hypothesis
+
+    #         time, pred_index, hypothesis = tf.while_loop(condition, body, loop_vars=[time, pred_index, hypothesis])
+
+    #         return Hypothesis(
+    #             index=hypothesis.index,
+    #             prediction=hypothesis.prediction.stack(),
+    #             states=hypothesis.states,
+    #         )
 
-            return Hypothesis(index=y_hat_index, prediction=y_hat_prediction, states=y_hat_states)
+    # -------------------------------- BEAM SEARCH -------------------------------------
 
-    # -------------------------------- TFLITE -------------------------------------
+    def recognize_beam(self, inputs: schemas.PredictInput, **kwargs):
+        return self.recognize(inputs=inputs, **kwargs)
 
-    def make_tflite_function(
-        self,
-        timestamp: bool = False,
-    ):
-        tflite_func = self.recognize_tflite_with_timestamp if timestamp else self.recognize_tflite
-        return tf.function(
-            tflite_func,
-            input_signature=[
-                tf.TensorSpec([None], dtype=tf.float32),
-                tf.TensorSpec([], dtype=tf.int32),
-                tf.TensorSpec(self.predict_net.get_initial_state().get_shape(), dtype=tf.float32),
-            ],
-        )
+    # def _perform_beam_search_batch(
+    #     self,
+    #     encoded: tf.Tensor,
+    #     encoded_length: tf.Tensor,
+    #     lm: bool = False,
+    #     parallel_iterations: int = 10,
+    #     swap_memory: bool = True,
+    # ):
+    #     with tf.name_scope("perform_beam_search_batch"):
+    #         total_batch = tf.shape(encoded)[0]
+    #         batch = tf.constant(0, dtype=tf.int32)
+
+    #         decoded = tf.TensorArray(
+    #             dtype=tf.int32,
+    #             size=total_batch,
+    #             dynamic_size=False,
+    #             clear_after_read=False,
+    #             element_shape=None,
+    #         )
+
+    #         def condition(batch, _):
+    #             return tf.less(batch, total_batch)
+
+    #         def body(batch, decoded):
+    #             hypothesis = self._perform_beam_search(
+    #                 encoded[batch],
+    #                 encoded_length[batch],
+    #                 lm,
+    #                 parallel_iterations=parallel_iterations,
+    #                 swap_memory=swap_memory,
+    #             )
+    #             decoded = decoded.write(batch, hypothesis.prediction)
+    #             return batch + 1, decoded
+
+    #         batch, decoded = tf.while_loop(
+    #             condition,
+    #             body,
+    #             loop_vars=[batch, decoded],
+    #             parallel_iterations=parallel_iterations,
+    #             swap_memory=True,
+    #         )
+
+    #         decoded = math_util.pad_tfarray(decoded, blank=self.text_featurizer.blank)
+    #         return self.text_featurizer.detokenize(decoded.stack())
+
+    # def _perform_beam_search(
+    #     self,
+    #     encoded: tf.Tensor,
+    #     encoded_length: tf.Tensor,
+    #     lm: bool = False,
+    #     parallel_iterations: int = 10,
+    #     swap_memory: bool = True,
+    #     tflite: bool = False,
+    # ):
+    #     with tf.name_scope("beam_search"):
+    #         beam_width = tf.where(
+    #             tf.less(self.text_featurizer.decoder_config.beam_width, self.text_featurizer.num_classes),
+    #             self.text_featurizer.decoder_config.beam_width,
+    #             self.text_featurizer.num_classes - 1,
+    #         )
+    #         total = encoded_length
+
+    #         def initialize_beam(dynamic=False):
+    #             return BeamHypothesis(
+    #                 score=tf.TensorArray(
+    #                     dtype=tf.float32,
+    #                     size=beam_width if not dynamic else 0,
+    #                     dynamic_size=dynamic,
+    #                     element_shape=tf.TensorShape([]),
+    #                     clear_after_read=False,
+    #                 ),
+    #                 indices=tf.TensorArray(
+    #                     dtype=tf.int32,
+    #                     size=beam_width if not dynamic else 0,
+    #                     dynamic_size=dynamic,
+    #                     element_shape=tf.TensorShape([]),
+    #                     clear_after_read=False,
+    #                 ),
+    #                 prediction=tf.TensorArray(
+    #                     dtype=tf.int32,
+    #                     size=beam_width if not dynamic else 0,
+    #                     dynamic_size=dynamic,
+    #                     element_shape=None,
+    #                     clear_after_read=False,
+    #                 ),
+    #                 states=tf.TensorArray(
+    #                     dtype=tf.float32,
+    #                     size=beam_width if not dynamic else 0,
+    #                     dynamic_size=dynamic,
+    #                     element_shape=tf.TensorShape(shape_util.shape_list(self.predict_net.get_initial_state())),
+    #                     clear_after_read=False,
+    #                 ),
+    #             )
+
+    #         B = initialize_beam()
+    #         B = BeamHypothesis(
+    #             score=B.score.write(0, 0.0),
+    #             indices=B.indices.write(0, self.text_featurizer.blank),
+    #             prediction=B.prediction.write(0, tf.ones([total], dtype=tf.int32) * self.text_featurizer.blank),
+    #             states=B.states.write(0, self.predict_net.get_initial_state(4)),
+    #         )
+
+    #         def condition(time, total, B):
+    #             return tf.less(time, total)
+
+    #         def body(time, total, B):
+    #             A = initialize_beam(dynamic=True)
+    #             A = BeamHypothesis(
+    #                 score=A.score.unstack(B.score.stack()),
+    #                 indices=A.indices.unstack(B.indices.stack()),
+    #                 prediction=A.prediction.unstack(math_util.pad_tfarray(B.prediction, blank=self.text_featurizer.blank).stack()),
+    #                 states=A.states.unstack(B.states.stack()),
+    #             )
+    #             A_i = tf.constant(0, tf.int32)
+    #             B = initialize_beam()
+
+    #             encoded_t = tf.gather_nd(encoded, tf.expand_dims(time, axis=-1))
+
+    #             def beam_condition(beam, beam_width, A, A_i, B):
+    #                 return tf.less(beam, beam_width)
+
+    #             def beam_body(beam, beam_width, A, A_i, B):
+    #                 # get y_hat
+    #                 y_hat_score, y_hat_score_index = tf.math.top_k(A.score.stack(), k=1, sorted=True)
+    #                 y_hat_score = y_hat_score[0]
+    #                 y_hat_index = tf.gather_nd(A.indices.stack(), y_hat_score_index)
+    #                 y_hat_prediction = tf.gather_nd(
+    #                     math_util.pad_tfarray(A.prediction, blank=self.text_featurizer.blank).stack(),
+    #                     y_hat_score_index,
+    #                 )
+    #                 y_hat_states = tf.gather_nd(A.states.stack(), y_hat_score_index)
+
+    #                 # remove y_hat from A
+    #                 remain_indices = tf.range(0, tf.shape(A.score.stack())[0], dtype=tf.int32)
+    #                 remain_indices = tf.gather_nd(remain_indices, tf.where(tf.not_equal(remain_indices, y_hat_score_index[0])))
+    #                 remain_indices = tf.expand_dims(remain_indices, axis=-1)
+    #                 A = BeamHypothesis(
+    #                     score=A.score.unstack(tf.gather_nd(A.score.stack(), remain_indices)),
+    #                     indices=A.indices.unstack(tf.gather_nd(A.indices.stack(), remain_indices)),
+    #                     prediction=A.prediction.unstack(
+    #                         tf.gather_nd(
+    #                             math_util.pad_tfarray(A.prediction, blank=self.text_featurizer.blank).stack(),
+    #                             remain_indices,
+    #                         )
+    #                     ),
+    #                     states=A.states.unstack(tf.gather_nd(A.states.stack(), remain_indices)),
+    #                 )
+    #                 A_i = tf.where(tf.equal(A_i, 0), A_i, A_i - 1)
+
+    #                 ytu, new_states = self.decoder_inference(encoded=encoded_t, predicted=y_hat_index, states=y_hat_states, tflite=tflite)
+
+    #                 def predict_condition(pred, A, A_i, B):
+    #                     return tf.less(pred, self.text_featurizer.num_classes)
+
+    #                 def predict_body(pred, A, A_i, B):
+    #                     new_score = y_hat_score + tf.gather_nd(ytu, tf.expand_dims(pred, axis=-1))
+
+    #                     def true_fn():
+    #                         return (
+    #                             B.score.write(beam, new_score),
+    #                             B.indices.write(beam, y_hat_index),
+    #                             B.prediction.write(beam, y_hat_prediction),
+    #                             B.states.write(beam, y_hat_states),
+    #                             A.score,
+    #                             A.indices,
+    #                             A.prediction,
+    #                             A.states,
+    #                             A_i,
+    #                         )
+
+    #                     def false_fn():
+    #                         scatter_index = math_util.count_non_blank(y_hat_prediction, blank=self.text_featurizer.blank)
+    #                         updated_prediction = tf.tensor_scatter_nd_update(
+    #                             y_hat_prediction,
+    #                             indices=tf.reshape(scatter_index, [1, 1]),
+    #                             updates=tf.expand_dims(pred, axis=-1),
+    #                         )
+    #                         return (
+    #                             B.score,
+    #                             B.indices,
+    #                             B.prediction,
+    #                             B.states,
+    #                             A.score.write(A_i, new_score),
+    #                             A.indices.write(A_i, pred),
+    #                             A.prediction.write(A_i, updated_prediction),
+    #                             A.states.write(A_i, new_states),
+    #                             A_i + 1,
+    #                         )
+
+    #                     b_score, b_indices, b_prediction, b_states, a_score, a_indices, a_prediction, a_states, A_i = tf.cond(
+    #                         tf.equal(pred, self.text_featurizer.blank), true_fn=true_fn, false_fn=false_fn
+    #                     )
+
+    #                     B = BeamHypothesis(score=b_score, indices=b_indices, prediction=b_prediction, states=b_states)
+    #                     A = BeamHypothesis(score=a_score, indices=a_indices, prediction=a_prediction, states=a_states)
+
+    #                     return pred + 1, A, A_i, B
+
+    #                 _, A, A_i, B = tf.while_loop(
+    #                     predict_condition,
+    #                     predict_body,
+    #                     loop_vars=[0, A, A_i, B],
+    #                     parallel_iterations=parallel_iterations,
+    #                     swap_memory=swap_memory,
+    #                 )
+
+    #                 return beam + 1, beam_width, A, A_i, B
+
+    #             _, _, A, A_i, B = tf.while_loop(
+    #                 beam_condition,
+    #                 beam_body,
+    #                 loop_vars=[0, beam_width, A, A_i, B],
+    #                 parallel_iterations=parallel_iterations,
+    #                 swap_memory=swap_memory,
+    #             )
+
+    #             return time + 1, total, B
+
+    #         _, _, B = tf.while_loop(
+    #             condition,
+    #             body,
+    #             loop_vars=[0, total, B],
+    #             parallel_iterations=parallel_iterations,
+    #             swap_memory=swap_memory,
+    #         )
+
+    #         scores = B.score.stack()
+    #         prediction = math_util.pad_tfarray(B.prediction, blank=self.text_featurizer.blank).stack()
+    #         if self.text_featurizer.decoder_config.norm_score:
+    #             prediction_lengths = math_util.count_non_blank(prediction, blank=self.text_featurizer.blank, axis=1)
+    #             scores /= tf.cast(prediction_lengths, dtype=scores.dtype)
+
+    #         y_hat_score, y_hat_score_index = tf.math.top_k(scores, k=1)
+    #         y_hat_score = y_hat_score[0]
+    #         y_hat_index = tf.gather_nd(B.indices.stack(), y_hat_score_index)
+    #         y_hat_prediction = tf.gather_nd(prediction, y_hat_score_index)
+    #         y_hat_states = tf.gather_nd(B.states.stack(), y_hat_score_index)
+
+    #         return Hypothesis(index=y_hat_index, prediction=y_hat_prediction, states=y_hat_states)
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/conformer.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/transformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,128 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2023 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from tensorflow_asr.models.encoders.conformer import L2, ConformerEncoder
+import tensorflow as tf
+
+from tensorflow_asr.models.encoders.transformer import TransformerEncoder
 from tensorflow_asr.models.transducer.base_transducer import Transducer
 
 
-class Conformer(Transducer):
+@tf.keras.utils.register_keras_serializable("tensorflow_asr.models.transducer")
+class Transformer(Transducer):
     def __init__(
         self,
-        vocabulary_size: int,
+        blank: int,
+        vocab_size: int,
+        speech_config: dict,
         encoder_subsampling: dict,
-        encoder_positional_encoding: str = "sinusoid",
-        encoder_dmodel: int = 144,
-        encoder_num_blocks: int = 16,
-        encoder_head_size: int = 36,
+        encoder_dmodel: int = 512,
+        encoder_dff: int = 1024,
+        encoder_num_blocks: int = 6,
+        encoder_head_size: int = 128,
         encoder_num_heads: int = 4,
         encoder_mha_type: str = "relmha",
-        encoder_kernel_size: int = 32,
-        encoder_depth_multiplier: int = 1,
-        encoder_fc_factor: float = 0.5,
-        encoder_dropout: float = 0,
+        encoder_interleave_relpe: bool = True,
+        encoder_use_attention_causal_mask: bool = False,
+        encoder_use_attention_auto_mask: bool = True,
+        encoder_residual_factor: float = 1.0,
+        encoder_norm_position: str = "post",
+        encoder_pwffn_activation: str = "relu",
+        encoder_dropout: float = 0.1,
+        encoder_memory_length: int = None,
         encoder_trainable: bool = True,
+        prediction_label_encode_mode: str = "embedding",
         prediction_embed_dim: int = 512,
-        prediction_embed_dropout: int = 0,
         prediction_num_rnns: int = 1,
         prediction_rnn_units: int = 320,
         prediction_rnn_type: str = "lstm",
         prediction_rnn_implementation: int = 2,
+        prediction_rnn_unroll: bool = False,
         prediction_layer_norm: bool = True,
         prediction_projection_units: int = 0,
         prediction_trainable: bool = True,
         joint_dim: int = 1024,
         joint_activation: str = "tanh",
-        prejoint_linear: bool = True,
+        prejoint_encoder_linear: bool = True,
+        prejoint_prediction_linear: bool = True,
         postjoint_linear: bool = False,
         joint_mode: str = "add",
         joint_trainable: bool = True,
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name: str = "conformer",
+        kernel_regularizer=None,
+        bias_regularizer=None,
+        name: str = "transformer",
         **kwargs,
     ):
-        super(Conformer, self).__init__(
-            encoder=ConformerEncoder(
+        super().__init__(
+            speech_config=speech_config,
+            encoder=TransformerEncoder(
                 subsampling=encoder_subsampling,
-                positional_encoding=encoder_positional_encoding,
-                dmodel=encoder_dmodel,
                 num_blocks=encoder_num_blocks,
-                head_size=encoder_head_size,
+                dmodel=encoder_dmodel,
+                dff=encoder_dff,
                 num_heads=encoder_num_heads,
+                head_size=encoder_head_size,
                 mha_type=encoder_mha_type,
-                kernel_size=encoder_kernel_size,
-                depth_multiplier=encoder_depth_multiplier,
-                fc_factor=encoder_fc_factor,
+                norm_position=encoder_norm_position,
+                residual_factor=encoder_residual_factor,
+                interleave_relpe=encoder_interleave_relpe,
+                use_attention_causal_mask=encoder_use_attention_causal_mask,
+                use_attention_auto_mask=encoder_use_attention_auto_mask,
+                pwffn_activation=encoder_pwffn_activation,
                 dropout=encoder_dropout,
+                memory_length=encoder_memory_length,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
                 trainable=encoder_trainable,
-                name=f"{name}_encoder",
+                name="encoder",
             ),
-            vocabulary_size=vocabulary_size,
-            embed_dim=prediction_embed_dim,
-            embed_dropout=prediction_embed_dropout,
-            num_rnns=prediction_num_rnns,
-            rnn_units=prediction_rnn_units,
-            rnn_type=prediction_rnn_type,
-            rnn_implementation=prediction_rnn_implementation,
-            layer_norm=prediction_layer_norm,
-            projection_units=prediction_projection_units,
+            blank=blank,
+            vocab_size=vocab_size,
+            prediction_label_encoder_mode=prediction_label_encode_mode,
+            prediction_embed_dim=prediction_embed_dim,
+            prediction_num_rnns=prediction_num_rnns,
+            prediction_rnn_units=prediction_rnn_units,
+            prediction_rnn_type=prediction_rnn_type,
+            prediction_rnn_implementation=prediction_rnn_implementation,
+            prediction_rnn_unroll=prediction_rnn_unroll,
+            prediction_layer_norm=prediction_layer_norm,
+            prediction_projection_units=prediction_projection_units,
             prediction_trainable=prediction_trainable,
             joint_dim=joint_dim,
             joint_activation=joint_activation,
-            prejoint_linear=prejoint_linear,
+            prejoint_encoder_linear=prejoint_encoder_linear,
+            prejoint_prediction_linear=prejoint_prediction_linear,
             postjoint_linear=postjoint_linear,
             joint_mode=joint_mode,
             joint_trainable=joint_trainable,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             name=name,
             **kwargs,
         )
         self.dmodel = encoder_dmodel
-        self.time_reduction_factor = self.encoder.conv_subsampling.time_reduction_factor
+        self.time_reduction_factor = self.encoder.time_reduction_factor
+
+    def reset_caching(self):
+        return self.encoder.reset_caching(self._per_replica_batch_size)
+
+    def make(self, input_shape=[None], prediction_shape=[None], batch_size=None, **kwargs):
+        caching = (
+            None
+            if self.encoder._memory_length is None
+            else [
+                tf.keras.Input(shape=[self.encoder._memory_length, self.encoder._dmodel], batch_size=batch_size, dtype=tf.float32)
+                for _ in range(self.encoder._num_blocks)
+            ]
+        )
+        return super().make(input_shape, prediction_shape, batch_size, caching, **kwargs)
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/models/transducer/contextnet.py` & `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/rnnt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,200 +1,178 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+""" http://arxiv.org/abs/1811.06621 """
 
-from typing import Dict, List
 import tensorflow as tf
 
-from tensorflow_asr.utils import data_util, math_util
-from tensorflow_asr.models.encoders.contextnet import L2, ContextNetEncoder
+from tensorflow_asr.models.encoders.rnnt import RnnTransducerEncoder
 from tensorflow_asr.models.transducer.base_transducer import Transducer
 
 
-class ContextNet(Transducer):
+@tf.keras.utils.register_keras_serializable("tensorflow_asr.models.transducer")
+class RnnTransducer(Transducer):
     def __init__(
         self,
-        vocabulary_size: int,
-        encoder_blocks: List[dict],
-        encoder_alpha: float = 0.5,
+        blank: int,
+        vocab_size: int,
+        speech_config: dict,
+        encoder_reduction_factors: list = [6, 0, 0, 0, 0, 0, 0, 0],
+        encoder_dmodel: int = 640,
+        encoder_nlayers: int = 8,
+        encoder_rnn_type: str = "lstm",
+        encoder_rnn_units: int = 2048,
+        encoder_rnn_unroll: bool = False,
+        encoder_layer_norm: bool = False,
         encoder_trainable: bool = True,
-        prediction_embed_dim: int = 512,
-        prediction_embed_dropout: int = 0,
-        prediction_num_rnns: int = 1,
-        prediction_rnn_units: int = 320,
+        prediction_label_encode_mode: str = "embedding",
+        prediction_embed_dim: int = 320,
+        prediction_num_rnns: int = 2,
+        prediction_rnn_units: int = 2048,
         prediction_rnn_type: str = "lstm",
         prediction_rnn_implementation: int = 2,
-        prediction_layer_norm: bool = True,
-        prediction_projection_units: int = 0,
+        prediction_rnn_unroll: bool = False,
+        prediction_layer_norm: bool = False,
+        prediction_projection_units: int = 640,
         prediction_trainable: bool = True,
-        joint_dim: int = 1024,
+        joint_dim: int = 640,
         joint_activation: str = "tanh",
-        prejoint_linear: bool = True,
+        prejoint_encoder_linear: bool = True,
+        prejoint_prediction_linear: bool = True,
         postjoint_linear: bool = False,
         joint_mode: str = "add",
         joint_trainable: bool = True,
-        kernel_regularizer=L2,
-        bias_regularizer=L2,
-        name: str = "contextnet",
+        kernel_regularizer=None,
+        bias_regularizer=None,
+        name="rnn_transducer",
         **kwargs,
     ):
-        super(ContextNet, self).__init__(
-            encoder=ContextNetEncoder(
-                blocks=encoder_blocks,
-                alpha=encoder_alpha,
+        super().__init__(
+            speech_config=speech_config,
+            encoder=RnnTransducerEncoder(
+                reduction_factors=encoder_reduction_factors,
+                dmodel=encoder_dmodel,
+                nlayers=encoder_nlayers,
+                rnn_type=encoder_rnn_type,
+                rnn_units=encoder_rnn_units,
+                rnn_unroll=encoder_rnn_unroll,
+                layer_norm=encoder_layer_norm,
                 kernel_regularizer=kernel_regularizer,
                 bias_regularizer=bias_regularizer,
                 trainable=encoder_trainable,
-                name=f"{name}_encoder",
+                name="encoder",
             ),
-            vocabulary_size=vocabulary_size,
-            embed_dim=prediction_embed_dim,
-            embed_dropout=prediction_embed_dropout,
-            num_rnns=prediction_num_rnns,
-            rnn_units=prediction_rnn_units,
-            rnn_type=prediction_rnn_type,
-            rnn_implementation=prediction_rnn_implementation,
-            layer_norm=prediction_layer_norm,
+            blank=blank,
+            vocab_size=vocab_size,
+            prediction_label_encoder_mode=prediction_label_encode_mode,
+            prediction_embed_dim=prediction_embed_dim,
+            prediction_num_rnns=prediction_num_rnns,
+            prediction_rnn_units=prediction_rnn_units,
+            prediction_rnn_type=prediction_rnn_type,
+            prediction_layer_norm=prediction_layer_norm,
+            prediction_rnn_implementation=prediction_rnn_implementation,
+            prediction_rnn_unroll=prediction_rnn_unroll,
+            prediction_projection_units=prediction_projection_units,
             prediction_trainable=prediction_trainable,
-            projection_units=prediction_projection_units,
             joint_dim=joint_dim,
             joint_activation=joint_activation,
-            prejoint_linear=prejoint_linear,
+            prejoint_encoder_linear=prejoint_encoder_linear,
+            prejoint_prediction_linear=prejoint_prediction_linear,
             postjoint_linear=postjoint_linear,
             joint_mode=joint_mode,
             joint_trainable=joint_trainable,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             name=name,
             **kwargs,
         )
-        self.dmodel = self.encoder.blocks[-1].dmodel
-        self.time_reduction_factor = 1
-        for block in self.encoder.blocks:
-            self.time_reduction_factor *= block.time_reduction_factor
+        self.time_reduction_factor = self.encoder.time_reduction_factor
+        self.dmodel = encoder_dmodel
 
-    def call(
-        self,
-        inputs,
-        training=False,
-        **kwargs,
-    ):
-        enc = self.encoder([inputs["inputs"], inputs["inputs_length"]], training=training, **kwargs)
-        pred = self.predict_net([inputs["predictions"], inputs["predictions_length"]], training=training, **kwargs)
-        logits = self.joint_net([enc, pred], training=training, **kwargs)
-        return data_util.create_logits(
-            logits=logits, logits_length=math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor)
-        )
-
-    def encoder_inference(
-        self,
-        features: tf.Tensor,
-        input_length: tf.Tensor,
-    ):
-        with tf.name_scope(f"{self.name}_encoder"):
-            input_length = tf.expand_dims(tf.shape(features)[0], axis=0)
-            outputs = tf.expand_dims(features, axis=0)
-            outputs = self.encoder([outputs, input_length], training=False)
-            return tf.squeeze(outputs, axis=0)
+    # def encoder_inference(self, features: tf.Tensor, states: tf.Tensor):
+    #     """Infer function for encoder (or encoders)
 
-    # -------------------------------- GREEDY -------------------------------------
-
-    @tf.function
-    def recognize(
-        self,
-        inputs: Dict[str, tf.Tensor],
-    ):
-        """
-        RNN Transducer Greedy decoding
-        Args:
-            features (tf.Tensor): a batch of padded extracted features
-
-        Returns:
-            tf.Tensor: a batch of decoded transcripts
-        """
-        encoded = self.encoder([inputs["inputs"], inputs["inputs_length"]], training=False)
-        encoded_length = math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor)
-        return self._perform_greedy_batch(encoded=encoded, encoded_length=encoded_length)
-
-    def recognize_tflite(
-        self,
-        signal,
-        predicted,
-        prediction_states,
-    ):
-        """
-        Function to convert to tflite using greedy decoding (default streaming mode)
-        Args:
-            signal: tf.Tensor with shape [None] indicating a single audio signal
-            predicted: last predicted character with shape []
-            prediction_states: lastest prediction states with shape [num_rnns, 1 or 2, 1, P]
-
-        Return:
-            transcript: tf.Tensor of Unicode Code Points with shape [None] and dtype tf.int32
-            predicted: last predicted character with shape []
-            encoder_states: lastest encoder states with shape [num_rnns, 1 or 2, 1, P]
-            prediction_states: lastest prediction states with shape [num_rnns, 1 or 2, 1, P]
-        """
-        features = self.speech_featurizer.tf_extract(signal)
-        encoded = self.encoder_inference(features, tf.shape(features)[0])
-        hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, prediction_states)
-        transcript = self.text_featurizer.indices2upoints(hypothesis.prediction)
-        return transcript, hypothesis.index, hypothesis.states
-
-    def recognize_tflite_with_timestamp(
-        self,
-        signal,
-        predicted,
-        states,
-    ):
-        features = self.speech_featurizer.tf_extract(signal)
-        encoded = self.encoder_inference(features, tf.shape(features)[0])
-        hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, states)
-        indices = self.text_featurizer.normalize_indices(hypothesis.prediction)
-        upoints = tf.gather_nd(self.text_featurizer.upoints, tf.expand_dims(indices, axis=-1))  # [None, max_subword_length]
-
-        num_samples = tf.cast(tf.shape(signal)[0], dtype=tf.float32)
-        total_time_reduction_factor = self.time_reduction_factor * self.speech_featurizer.frame_step
-
-        stime = tf.range(0, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
-        stime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
-
-        etime = tf.range(total_time_reduction_factor, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
-        etime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
-
-        non_blank = tf.where(tf.not_equal(upoints, 0))
-        non_blank_transcript = tf.gather_nd(upoints, non_blank)
-        non_blank_stime = tf.gather_nd(tf.repeat(tf.expand_dims(stime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
-        non_blank_etime = tf.gather_nd(tf.repeat(tf.expand_dims(etime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
-
-        return non_blank_transcript, non_blank_stime, non_blank_etime, hypothesis.index, hypothesis.states
-
-    # -------------------------------- BEAM SEARCH -------------------------------------
-
-    @tf.function
-    def recognize_beam(
-        self,
-        inputs: Dict[str, tf.Tensor],
-        lm: bool = False,
-    ):
-        """
-        RNN Transducer Beam Search
-        Args:
-            features (tf.Tensor): a batch of padded extracted features
-            lm (bool, optional): whether to use language model. Defaults to False.
-
-        Returns:
-            tf.Tensor: a batch of decoded transcripts
-        """
-        encoded = self.encoder([inputs["inputs"], inputs["inputs_length"]], training=False)
-        encoded_length = math_util.get_reduced_length(inputs["inputs_length"], self.time_reduction_factor)
-        return self._perform_beam_search_batch(encoded=encoded, encoded_length=encoded_length, lm=lm)
+    #     Args:
+    #         features (tf.Tensor): features with shape [T, F, C]
+    #         states (tf.Tensor): previous states of encoders with shape [num_rnns, 1 or 2, 1, P]
+
+    #     Returns:
+    #         tf.Tensor: output of encoders with shape [T, E]
+    #         tf.Tensor: states of encoders with shape [num_rnns, 1 or 2, 1, P]
+    #     """
+    #     with tf.name_scope("encoder"):
+    #         outputs = tf.expand_dims(features, axis=0)
+    #         outputs, new_states = self.encoder.recognize(outputs, states)
+    #         return tf.squeeze(outputs, axis=0), new_states
+
+    # # -------------------------------- GREEDY -------------------------------------
+
+    # def recognize_tflite(self, signal, predicted, encoder_states, prediction_states):
+    #     """
+    #     Function to convert to tflite using greedy decoding (default streaming mode)
+    #     Args:
+    #         signal: tf.Tensor with shape [None] indicating a single audio signal
+    #         predicted: last predicted character with shape []
+    #         encoder_states: lastest encoder states with shape [num_rnns, 1 or 2, 1, P]
+    #         prediction_states: lastest prediction states with shape [num_rnns, 1 or 2, 1, P]
+
+    #     Return:
+    #         transcript: tf.Tensor of Unicode Code Points with shape [None] and dtype tf.int32
+    #         predicted: last predicted character with shape []
+    #         encoder_states: lastest encoder states with shape [num_rnns, 1 or 2, 1, P]
+    #         prediction_states: lastest prediction states with shape [num_rnns, 1 or 2, 1, P]
+    #     """
+    #     features = self.speech_featurizer.tf_extract(signal)
+    #     encoded, new_encoder_states = self.encoder_inference(features, encoder_states)
+    #     hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, prediction_states)
+    #     transcript = self.text_featurizer.detokenize_unicode_points(hypothesis.prediction)
+    #     return transcript, hypothesis.index, new_encoder_states, hypothesis.states
+
+    # def recognize_tflite_with_timestamp(self, signal, predicted, encoder_states, prediction_states):
+    #     features = self.speech_featurizer.tf_extract(signal)
+    #     encoded, new_encoder_states = self.encoder_inference(features, encoder_states)
+    #     hypothesis = self._perform_greedy(encoded, tf.shape(encoded)[0], predicted, prediction_states)
+    #     indices = self.text_featurizer.normalize_indices(hypothesis.prediction)
+    #     upoints = tf.gather_nd(self.text_featurizer.upoints, tf.expand_dims(indices, axis=-1))  # [None, max_subword_length]
+
+    #     num_samples = tf.cast(tf.shape(signal)[0], dtype=tf.float32)
+    #     total_time_reduction_factor = self.time_reduction_factor * self.speech_featurizer.frame_step
+
+    #     stime = tf.range(0, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
+    #     stime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
+
+    #     etime = tf.range(total_time_reduction_factor, num_samples, delta=total_time_reduction_factor, dtype=tf.float32)
+    #     etime /= tf.cast(self.speech_featurizer.sample_rate, dtype=tf.float32)
+
+    #     non_blank = tf.where(tf.not_equal(upoints, 0))
+    #     non_blank_transcript = tf.gather_nd(upoints, non_blank)
+    #     non_blank_stime = tf.gather_nd(tf.repeat(tf.expand_dims(stime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
+    #     non_blank_etime = tf.gather_nd(tf.repeat(tf.expand_dims(etime, axis=-1), tf.shape(upoints)[-1], axis=-1), non_blank)
+
+    #     return non_blank_transcript, non_blank_stime, non_blank_etime, hypothesis.index, new_encoder_states, hypothesis.states
+
+    # -------------------------------- TFLITE -------------------------------------
+
+    # def make_tflite_function(
+    #     self,
+    #     timestamp: bool = True,
+    # ):
+    #     tflite_func = self.recognize_tflite_with_timestamp if timestamp else self.recognize_tflite
+    #     return tf.function(
+    #         tflite_func,
+    #         input_signature=[
+    #             tf.TensorSpec([None], dtype=tf.float32),
+    #             tf.TensorSpec([], dtype=tf.int32),
+    #             tf.TensorSpec(self.encoder.get_initial_state().get_shape(), dtype=tf.float32),
+    #             tf.TensorSpec(self.predict_net.get_initial_state().get_shape(), dtype=tf.float32),
+    #         ],
+    #     )
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/optimizers/schedules.py` & `TensorFlowASR-2.0.0/tensorflow_asr/optimizers/schedules.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,56 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
-from tensorflow.keras.optimizers.schedules import ExponentialDecay
 
 
+@tf.keras.utils.register_keras_serializable("tensorflow_asr.optimizers.schedules")
 class TransformerSchedule(tf.keras.optimizers.schedules.LearningRateSchedule):
-    def __init__(self, d_model, warmup_steps=4000, max_lr=None):
-        super(TransformerSchedule, self).__init__()
-
-        self.d_model = d_model
-        self.d_model = tf.cast(self.d_model, tf.float32)
-        self.max_lr = max_lr
-        self.warmup_steps = warmup_steps
+    def __init__(self, dmodel, scale=1.0, warmup_steps=4000, max_lr=None, min_lr=None):
+        super().__init__()
+        self.dmodel = tf.convert_to_tensor(dmodel, dtype=tf.float32)
+        self.scale = tf.convert_to_tensor(scale, dtype=tf.float32)
+        self.warmup_steps = tf.convert_to_tensor(warmup_steps, dtype=tf.float32)
+        self.max_lr = eval(max_lr) if isinstance(max_lr, str) else max_lr
+        self.min_lr = eval(min_lr) if isinstance(min_lr, str) else min_lr
 
-    def __call__(self, step):
+    def __call__(self, current_step):
         # lr = (d_model^-0.5) * min(step^-0.5, step*(warm_up^-1.5))
-        step = tf.cast(step, dtype=tf.float32)
-        arg1 = tf.math.rsqrt(step)
-        arg2 = step * (self.warmup_steps ** -1.5)
-        lr = tf.math.rsqrt(self.d_model) * tf.math.minimum(arg1, arg2)
+        step = tf.cast(current_step, dtype=tf.float32)
+        lr = (self.dmodel**-0.5) * tf.math.minimum(step**-0.5, step * (self.warmup_steps**-1.5))
+        lr = self.scale * lr
         if self.max_lr is not None:
-            return tf.math.minimum(self.max_lr, lr)
+            lr = tf.math.minimum(self.max_lr, lr)
+        if self.min_lr is not None:
+            lr = tf.math.maximum(self.min_lr, lr)
         return lr
 
     def get_config(self):
         return {
-            "d_model": self.d_model,
+            "dmodel": self.dmodel,
+            "scale": self.scale,
             "warmup_steps": self.warmup_steps,
             "max_lr": self.max_lr,
+            "min_lr": self.min_lr,
         }
 
 
-class SANSchedule(tf.keras.optimizers.schedules.LearningRateSchedule):
-    def __init__(self, lamb, d_model, warmup_steps=4000):
-        super(SANSchedule, self).__init__()
-
-        self.lamb = tf.cast(lamb, tf.float32)
-        self.d_model = tf.cast(d_model, tf.float32)
-
-        self.warmup_steps = tf.cast(warmup_steps, tf.float32)
-
-    def __call__(self, step):
-        step = tf.cast(step, dtype=tf.float32)
-        arg1 = step / (self.warmup_steps ** 1.5)
-        arg2 = 1 / tf.math.sqrt(step)
-        return (self.lamb / tf.math.sqrt(self.d_model)) * tf.math.minimum(arg1, arg2)
-
-    def get_config(self):
-        return {
-            "lamb": self.lamb,
-            "d_model": self.d_model,
-            "warmup_steps": self.warmup_steps,
-        }
-
-
-class BoundExponentialDecay(ExponentialDecay):
-    def __init__(self, min_lr=0.0, **kwargs):
-        super().__init__(**kwargs)
-        self.min_lr = min_lr
-
-    def __call__(self, step):
-        with tf.name_scope(self.name or "ExponentialDecay") as name:
-            initial_learning_rate = tf.convert_to_tensor(self.initial_learning_rate, name="initial_learning_rate")
-            dtype = initial_learning_rate.dtype
-            decay_steps = tf.cast(self.decay_steps, dtype)
-            decay_rate = tf.cast(self.decay_rate, dtype)
-
-            global_step_recomp = tf.cast(step, dtype)
-            p = global_step_recomp / decay_steps
-            if self.staircase:
-                p = tf.math.floor(p)
-            new_lr = tf.multiply(initial_learning_rate, tf.pow(decay_rate, p), name=name)
-            return tf.maximum(self.min_lr, new_lr)
-
-
+@tf.keras.utils.register_keras_serializable("tensorflow_asr.optimizers.schedules")
 class CyclicTransformerSchedule(tf.keras.optimizers.schedules.LearningRateSchedule):
     """This callback implements a cyclical learning rate policy (CLR) to the square
     root decay generally used to train transformers.
     The method cycles the learning rate around the square root decay LR with an amplitude
     equal to the target LR with a given period.
     # Arguments
         d_model: The dimension of the transformer model.
@@ -98,45 +59,45 @@
         max_lr: Maximum value of the learning rate reachable.
         step_size: number of training iterations per
             half cycle. Authors suggest setting step_size
             2-8 x training iterations in epoch.
 
     It is inspired from the paper:
     # References
-      - [Cyclical Learning Rates for Training Neural Networks](
-      https://arxiv.org/abs/1506.01186)
+    - [Cyclical Learning Rates for Training Neural Networks](
+    https://arxiv.org/abs/1506.01186)
     """
 
-    def __init__(self, d_model, warmup_steps=4000, max_lr=None, step_size=None):
+    def __init__(self, dmodel, step_size, max_lr, warmup_steps=4000):
         """Applies triangular cyclic to the square root decay learning rate.
         Args:
         d_model: Model dimension
         warmup_steps: Warm up steps where the LR increases linearly.
         max_lr: The maximum LR.
         step_size: The size of the cyclic triangular half cycle.
         """
         super().__init__()
-
-        self.d_model = tf.cast(d_model, tf.float32)
-        self.warmup_steps = tf.cast(warmup_steps, tf.float32)
-        self.max_lr = tf.cast(max_lr, tf.float32)
-        self.step_size = tf.cast(step_size, tf.float32)
-
-    def __call__(self, step):
-        step = tf.cast(step, tf.float32)
-        warmup = step * (self.warmup_steps ** -1.5)
+        self.dmodel = tf.convert_to_tensor(dmodel, tf.float32)
+        self.warmup_steps = tf.convert_to_tensor(warmup_steps, tf.float32)
+        self.max_lr = eval(max_lr) if isinstance(max_lr, str) else max_lr
+        self.max_lr = tf.convert_to_tensor(self.max_lr, tf.float32)
+        self.step_size = tf.convert_to_tensor(step_size, tf.float32)
+
+    def __call__(self, current_step):
+        step = tf.cast(current_step, tf.float32)
+        warmup = step * (self.warmup_steps**-1.5)
         lr = 2 * tf.math.rsqrt(step)
-        lr = tf.math.rsqrt(self.d_model) * tf.math.minimum(lr, warmup)
+        lr = tf.math.rsqrt(self.dmodel) * tf.math.minimum(lr, warmup)
         lr = tf.math.minimum(self.max_lr, lr)
         cycle = tf.math.floor(1 + step / (2 * self.step_size))
         x = tf.math.abs(step / self.step_size - 2 * cycle + 1)
         lr = lr * (0.5 + tf.math.maximum(0.0, x))
         lr = tf.math.minimum(self.max_lr, tf.math.minimum(lr, warmup))
         return lr
 
     def get_config(self):
         return {
-            "d_model": self.d_model,
+            "dmodel": self.dmodel,
             "warmup_steps": self.warmup_steps,
             "max_lr": self.max_lr,
             "step_size": self.step_size,
         }
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/utils/feature_util.py` & `TensorFlowASR-2.0.0/tensorflow_asr/utils/feature_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/utils/file_util.py` & `TensorFlowASR-2.0.0/tensorflow_asr/utils/file_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,49 +14,52 @@
 
 import contextlib
 import os
 import re
 import tempfile
 from typing import List, Union
 
+import jinja2
 import tensorflow as tf
 import yaml
 
+ENABLE_PATH_PREPROCESS = True
+
 
 def load_yaml(
     path: str,
-) -> dict:
+    **kwargs,
+):
     # Fix yaml numbers https://stackoverflow.com/a/30462009/11037553
     loader = yaml.SafeLoader
     loader.add_implicit_resolver(
-        u"tag:yaml.org,2002:float",
+        "tag:yaml.org,2002:float",
         re.compile(
-            u"""^(?:
+            """^(?:
          [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?
         |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
         |\\.[0-9_]+(?:[eE][-+][0-9]+)?
         |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*
         |[-+]?\\.(?:inf|Inf|INF)
         |\\.(?:nan|NaN|NAN))$""",
             re.X,
         ),
-        list(u"-+0123456789."),
+        list("-+0123456789."),
     )
-    with open(path, "r", encoding="utf-8") as file:
-        return yaml.load(file, Loader=loader)
+    with tf.io.gfile.GFile(path, "r") as file:
+        return yaml.load(
+            jinja2.Environment(loader=jinja2.FileSystemLoader([kwargs["repodir"]])).from_string(file.read()).render(**kwargs),
+            Loader=loader,
+        )
 
 
 def is_hdf5_filepath(
     filepath: str,
 ) -> bool:
-    return (
-        filepath.endswith(".h5")
-        or filepath.endswith(".keras")
-        or filepath.endswith(".hdf5")
-    )
+    return filepath.endswith(".h5") or filepath.endswith(".keras") or filepath.endswith(".hdf5")
 
 
 def is_cloud_path(
     path: str,
 ) -> bool:
     """Check if the path is on cloud (which requires tf.io.gfile)
 
@@ -68,63 +71,67 @@
     """
     return bool(re.match(r"^[a-z]+://", path))
 
 
 def preprocess_paths(
     paths: Union[List[str], str],
     isdir: bool = False,
+    enabled: bool = True,
+    check_exists: bool = False,
 ) -> Union[List[str], str]:
     """Expand the path to the root "/" and makedirs
 
     Args:
         paths (Union[List, str]): A path or list of paths
 
     Returns:
         Union[List, str]: A processed path or list of paths, return None if it's not path
     """
-    if isinstance(paths, list):
-        paths = [
-            path if is_cloud_path(path) else os.path.abspath(os.path.expanduser(path))
-            for path in paths
-        ]
-        for path in paths:
-            dirpath = path if isdir else os.path.dirname(path)
-            if not tf.io.gfile.exists(dirpath):
-                tf.io.gfile.makedirs(dirpath)
+    if not (enabled and ENABLE_PATH_PREPROCESS):
         return paths
+    if isinstance(paths, (list, tuple)):
+        paths = [path if is_cloud_path(path) else os.path.abspath(os.path.expanduser(path)) for path in paths]
+        for i, path in enumerate(paths):
+            dirpath = path if isdir else os.path.dirname(path)
+            if not tf.io.gfile.exists(path):
+                if check_exists:
+                    paths[i] = None
+                else:
+                    if not tf.io.gfile.exists(dirpath):
+                        tf.io.gfile.makedirs(dirpath)
+        return list(filter(None, paths))
     if isinstance(paths, str):
-        paths = (
-            paths
-            if is_cloud_path(paths)
-            else os.path.abspath(os.path.expanduser(paths))
-        )
+        paths = paths if is_cloud_path(paths) else os.path.abspath(os.path.expanduser(paths))
         dirpath = paths if isdir else os.path.dirname(paths)
-        if not tf.io.gfile.exists(dirpath):
-            tf.io.gfile.makedirs(dirpath)
+        if not tf.io.gfile.exists(paths):
+            if check_exists:
+                return None
+            if not tf.io.gfile.exists(dirpath):
+                tf.io.gfile.makedirs(dirpath)
         return paths
     return None
 
 
 @contextlib.contextmanager
 def save_file(
     filepath: str,
 ):
-    if is_cloud_path(filepath) and is_hdf5_filepath(filepath):
+    if is_cloud_path(filepath):
         _, ext = os.path.splitext(filepath)
         with tempfile.NamedTemporaryFile(suffix=ext) as tmp:
             yield tmp.name
             tf.io.gfile.copy(tmp.name, filepath, overwrite=True)
     else:
         yield filepath
 
 
 @contextlib.contextmanager
 def read_file(
     filepath: str,
 ):
-    if is_cloud_path(filepath) and is_hdf5_filepath(filepath):
+    if is_cloud_path(filepath):
         _, ext = os.path.splitext(filepath)
         with tempfile.NamedTemporaryFile(suffix=ext) as tmp:
             tf.io.gfile.copy(filepath, tmp.name, overwrite=True)
             yield tmp.name
     else:
         yield filepath
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/utils/metric_util.py` & `TensorFlowASR-2.0.0/tensorflow_asr/utils/metric_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Tuple
+
 import tensorflow as tf
 from nltk.metrics import distance
 
 from tensorflow_asr.utils import math_util
 
 
 def execute_wer(
@@ -78,19 +79,41 @@
 
     Returns:
         tuple: a tuple of tf.Tensor of (edit distances, number of characters) of each text
     """
     return tf.numpy_function(execute_cer, inp=[decode, target], Tout=[tf.float32, tf.float32])
 
 
+def tf_wer(
+    decode: tf.Tensor,
+    target: tf.Tensor,
+) -> Tuple[tf.Tensor, tf.Tensor]:
+    """
+    Tensorflow Word Error Rate
+
+    Args:
+        decode (tf.Tensor): tensor shape [B]
+        target (tf.Tensor): tensor shape [B]
+
+    Returns:
+        tuple: a tuple of tf.Tensor of (edit distances, number of words) of each text
+    """
+    decode = tf.strings.split(decode)
+    target = tf.strings.split(target)
+    distances = tf.edit_distance(decode.to_sparse(), target.to_sparse(), normalize=False)  # [B]
+    lengths = tf.cast(target.row_lengths(axis=1), dtype=tf.float32)  # [B]
+    return tf.reduce_sum(distances), tf.reduce_sum(lengths)
+
+
 def tf_cer(
     decode: tf.Tensor,
     target: tf.Tensor,
 ) -> Tuple[tf.Tensor, tf.Tensor]:
-    """Tensorflwo Charactor Error rate
+    """
+    Tensorflow Charactor Error rate
 
     Args:
         decoder (tf.Tensor): tensor shape [B]
         target (tf.Tensor): tensor shape [B]
 
     Returns:
         tuple: a tuple of tf.Tensor of (edit distances, number of characters) of each text
```

### Comparing `TensorFlowASR-1.0.3/tensorflow_asr/utils/shape_util.py` & `TensorFlowASR-2.0.0/tensorflow_asr/utils/shape_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Huy Le Nguyen (@usimarit)
+# Copyright 2020 Huy Le Nguyen (@nglehuy)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,15 +18,26 @@
 def shape_list(x, out_type=tf.int32):
     """Deal with dynamic shape in tensorflow cleanly."""
     static = x.shape.as_list()
     dynamic = tf.shape(x, out_type=out_type)
     return [dynamic[i] if s is None else s for i, s in enumerate(static)]
 
 
+def shape_list_per_replica(x, per_replica_batch_size):
+    shapes = x.shape.as_list()
+    shapes[0] = int(per_replica_batch_size)
+    return shapes
+
+
 def get_shape_invariants(tensor):
     shapes = shape_list(tensor)
     return tf.TensorShape([i if isinstance(i, int) else None for i in shapes])
 
 
 def get_float_spec(tensor):
     shape = get_shape_invariants(tensor)
     return tf.TensorSpec(shape, dtype=tf.float32)
+
+
+def get_dim(tensor, i):
+    """Get value of tensor shape[i] preferring static value if available."""
+    return tf.compat.dimension_value(tensor.shape[i]) or tf.shape(tensor)[i]
```

