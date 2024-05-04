# Comparing `tmp/konfuzio_sdk-0.3.4.dev20240418152335.tar.gz` & `tmp/konfuzio_sdk-0.3.4.dev20240502164651.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240418152335.tar", last modified: Fri Apr 19 03:26:53 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240502164651.tar", last modified: Fri May  3 03:29:52 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.4.dev20240418152335.tar` & `konfuzio_sdk-0.3.4.dev20240502164651.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.628459 konfuzio_sdk-0.3.4.dev20240418152335/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-19 03:26:53.628459 konfuzio_sdk-0.3.4.dev20240418152335/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.620459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.620459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.624459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.624459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:26:53.628459 konfuzio_sdk-0.3.4.dev20240418152335/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.624459 konfuzio_sdk-0.3.4.dev20240418152335/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.530389 konfuzio_sdk-0.3.4.dev20240502164651/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-03 03:29:52.530389 konfuzio_sdk-0.3.4.dev20240502164651/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.518389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207592 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.522389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.522389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.526389 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 03:29:52.000000 konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:29:52.530389 konfuzio_sdk-0.3.4.dev20240502164651/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:29:52.526389 konfuzio_sdk-0.3.4.dev20240502164651/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168877 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-03 03:29:43.000000 konfuzio_sdk-0.3.4.dev20240502164651/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/LICENSE.md` & `konfuzio_sdk-0.3.4.dev20240502164651/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240502164651/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240418152335
+Version: 0.3.4.dev20240502164651
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/README.md` & `konfuzio_sdk-0.3.4.dev20240502164651/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from konfuzio_sdk.regex import get_best_regex, merge_regex, regex_matches, suggest_regex_for_string
 from konfuzio_sdk.urls import get_annotation_view_url
 from konfuzio_sdk.utils import (
     amend_file_name,
     convert_to_bio_scheme,
     exception_or_log_error,
     get_file_type_and_extension,
+    get_merged_bboxes,
     get_missing_offsets,
     is_file,
     sdk_isinstance,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -690,14 +691,27 @@
         return self.page.image_height - self.y1 * (self.page.image_height / self.page.height)
 
     @property
     def y1_image(self):
         """Get the y1 coordinate in the context of the Page image, in a top-down coordinate system."""
         return self.page.image_height - self.y0 * (self.page.image_height / self.page.height)
 
+    @property
+    def dict_format(self) -> Dict:
+        """Obtain Bbox data as a dictionary."""
+        return {
+            'page_index': self.page.index,
+            'top': self.page.height - self.y1,
+            'bottom': self.page.height - self.y0,
+            'x0': self.x0,
+            'x1': self.x1,
+            'y0': self.y0,
+            'y1': self.y1,
+        }
+
 
 class AnnotationSet(Data):
     """
     An Annotation Set is a group of Annotations. The Labels of those Annotations refer to the same Label Set.
 
     For more details see https://dev.konfuzio.com/sdk/explanations.html#annotation-set-concept
     """
@@ -2161,14 +2175,17 @@
         offset_string: str = None,
         *args,
         **kwargs,
     ):
         """
         Initialize the Annotation.
 
+        An Annotation can be created either using Spans or using Bboxes. Make sure that Bboxes supplied actually contain
+        text inside; supplying empty Bboxes will cause an error.
+
         :param label: ID of the Annotation
         :param is_correct: If the Annotation is correct or not (bool)
         :param revised: If the Annotation is revised or not (bool)
         :param id_: ID of the Annotation (int)
         :param accuracy: Accuracy of the Annotation (float) which is the Confidence
         :param document: Document to annotate
         :param annotation: Annotation Set of the Document where the Label belongs
@@ -2279,34 +2296,33 @@
                 self.selection_bbox['x0'],
                 self.selection_bbox['x1'],
                 self.selection_bbox['y0'],
                 self.selection_bbox['y1'],
             )
             self.selection_bbox = Bbox(x0=x0, x1=x1, y0=y0, y1=y1, page=page)
 
+        # a variable to access Document Bboxes in case an Annotation is Bbox-based
+        self._document_bboxes = None
+
         # TODO START LEGACY to support multiline Annotations
-        bboxes = kwargs.get('bboxes', None)
-        if bboxes and len(bboxes) > 0:
-            for bbox in bboxes:
-                if 'start_offset' in bbox.keys() and 'end_offset' in bbox.keys():
-                    Span(start_offset=bbox['start_offset'], end_offset=bbox['end_offset'], annotation=self)
-                else:
-                    raise ValueError(f'SDK cannot read bbox of Annotation {self.id_} in {self.document}: {bbox}')
+        input_bbox_dicts = kwargs.get('bboxes', None)
+        if input_bbox_dicts and len(input_bbox_dicts) > 0:
+            self._add_annotation_from_bbox_dicts(input_bbox_dicts=input_bbox_dicts)
         elif (
-            bboxes is None
+            input_bbox_dicts is None
             and kwargs.get('start_offset', None) is not None
             and kwargs.get('end_offset', None) is not None
         ):
             # Legacy support for creating Annotations with a single offset
             bbox = kwargs.get('bbox', {})
             _ = Span(start_offset=kwargs.get('start_offset'), end_offset=kwargs.get('end_offset'), annotation=self)
             logger.warning(f'{self} is empty')
 
         self.top = None
-        self.top = None
+        self.bottom = None
         self.x0 = None
         self.x1 = None
         self.y0 = None
         self.y1 = None
 
         # todo: remove this Annotation single Bbox
         bbox = kwargs.get('bbox')
@@ -2350,15 +2366,15 @@
             return f'Annotation ({self.get_link()}) {self.label.name} {span_str}'
         elif self.label:
             return f'Annotation ({self.get_link()}) {self.label.name} ({self.spans})'
         else:
             return f'Annotation ({self.get_link()}) without Label ({self.start_offset}, {self.end_offset})'
 
     def __eq__(self, other):
-        """We compare an Annotation based on it's Label, Label-Sets if it's online otherwise on the id_local."""
+        """We compare an Annotation based on its Label, Label Sets if it's online otherwise on the id_local."""
         return (
             (self._spans.keys() == other._spans.keys())
             and self.label
             and other.label
             and (self.label == other.label)
             and self.document
             and other.document
@@ -2421,14 +2437,68 @@
         return [span.eval_dict() for span in self.spans]
 
     @property
     def label_set(self) -> LabelSet:
         """Return Label Set of Annotation."""
         return self.annotation_set.label_set
 
+    def _add_annotation_from_bbox_dicts(self, input_bbox_dicts: list) -> None:
+        """
+        Based on a list of dictionaries where each contains metadata for a bbox, this method adds Annotations to the Document.
+        If the dictionary has the fields "start_offset" and "end_offset", the method creates a Span based on such fields.
+        If not, it parses the bbox coordinates from the dictionary keys and based on them, looks for Spans
+        that could be contained within such bbox. If no Span was found, a `KeyError` is raised.
+
+        :param input_bbox_dicts: List of dictionaries, each containing metadata such as bbox coordinates
+        or Span's start_offset & end_offset used to create an Annotation.
+        Note: either (start_offset, end_offset) or (x0, x1, y0, y1, page_index) should be provided in each item of `input_bbox_dicts`.
+        """
+        for input_bbox_dict in input_bbox_dicts:
+            if 'start_offset' in input_bbox_dict.keys() and 'end_offset' in input_bbox_dict.keys():
+                Span(
+                    start_offset=input_bbox_dict['start_offset'],
+                    end_offset=input_bbox_dict['end_offset'],
+                    annotation=self,
+                )
+            elif (
+                'x0' in input_bbox_dict.keys()
+                and 'x1' in input_bbox_dict.keys()
+                and 'y0' in input_bbox_dict.keys()
+                and 'y1' in input_bbox_dict.keys()
+                and 'page_index' in input_bbox_dict.keys()
+            ):
+                page = self.document.get_page_by_index(input_bbox_dict['page_index'])
+                if not self._document_bboxes:
+                    self._document_bboxes = self.document.bbox_dict
+                input_bbox_dict['top'] = page.height - input_bbox_dict['y1']
+                input_bbox_dict['bottom'] = page.height - input_bbox_dict['y0']
+                # checking that Bboxes provided as input contain text inside
+                merged_bboxes = get_merged_bboxes(
+                    doc_bbox=self._document_bboxes, bboxes=[input_bbox_dict], doc_text=self.document.text
+                )
+                for merged_bbox in merged_bboxes:
+                    try:
+                        span = Span(start_offset=merged_bbox['start_offset'], end_offset=merged_bbox['end_offset'])
+                        self.add_span(span)
+                        _ = Bbox(
+                            page=self.document.get_page_by_index(merged_bbox['page_index']),
+                            x0=merged_bbox['x0'],
+                            x1=merged_bbox['x1'],
+                            y0=merged_bbox['y0'],
+                            y1=merged_bbox['y1'],
+                        )
+                    except KeyError:
+                        raise KeyError(
+                            f'Cannot add {self} because Bbox {input_bbox_dict} does not have any text inside and '
+                            f'it is not possible create Spans from the selected area. Please provide Bboxes'
+                            f'that have text inside them or Spans to create an Annotation.'
+                        )
+            else:
+                raise ValueError(f'SDK cannot read Bbox of Annotation {self.id_} in {self.document}: {input_bbox_dict}')
+
     def add_span(self, span: Span):
         """Add a Span to an Annotation incl. a duplicate check per Annotation."""
         if (span.start_offset, span.end_offset) not in self._spans:
             # add the Span first to make sure to bea able to do a duplicate check
             self._spans[(span.start_offset, span.end_offset)] = span  # one Annotation can span multiple Spans
             if span.annotation is not None and self != span.annotation:
                 raise ValueError(f'{span} should be added to {self} but relates to {span.annotation}.')
@@ -2473,24 +2543,30 @@
         new_annotation_added = False
 
         if self.is_online:
             raise ValueError(f'You cannot update Annotations once saved online: {self.get_link()}')
             # update_annotation(id_=self.id_, document_id=self.document.id_, project_id=self.project.id_)
 
         if not self.is_online:
+            if self.spans:
+                spans_bboxes = self.spans
+            elif self.bboxes:
+                spans_bboxes = self.bboxes
+            else:
+                raise ValueError('Cannot save an Annotation without Spans and Bboxes.')
             response = post_document_annotation(
                 document_id=self.document.id_,
                 label_id=self.label.id_,
                 label_set_id=label_set_id,
                 confidence=self.confidence,
                 is_correct=self.is_correct,
                 revised=self.revised,
                 annotation_set_id=annotation_set_id,
                 session=self.document.project.session,
-                spans=self.spans,
+                spans=spans_bboxes,
             )
             if response.status_code == 201:
                 json_response = json.loads(response.text)
                 self.id_ = json_response['id']
                 new_annotation_added = True
             elif response.status_code == 403:
                 logger.error(response.text)
@@ -2598,22 +2674,21 @@
                 logger.warning(
                     f'Could not delete annotation with key {(tuple(sorted(self._spans.keys())), self.label.name)} in {self.document}: {e}'
                 )
                 # See also: https://git.konfuzio.com/konfuzio/objectives/-/issues/12402
 
     def bbox(self) -> Bbox:
         """Get Bbox encompassing all Annotation Spans."""
-        if self._bbox is None:
-            self._bbox = Bbox(
-                x0=min([span.bbox().x0 for span in self.spans]),
-                x1=max([span.bbox().x1 for span in self.spans]),
-                y0=min([span.bbox().y0 for span in self.spans]),
-                y1=max([span.bbox().y1 for span in self.spans]),
-                page=self.page,
-            )
+        self._bbox = Bbox(
+            x0=min([span.bbox().x0 for span in self.spans]),
+            x1=max([span.bbox().x1 for span in self.spans]),
+            y0=min([span.bbox().y0 for span in self.spans]),
+            y1=max([span.bbox().y1 for span in self.spans]),
+            page=self.page,
+        )
         return self._bbox
 
     @property
     def spans(self) -> List[Span]:
         """Return default entry to get all Spans of the Annotation."""
         return [self._spans[k] for k in sorted(self._spans.keys())]
 
@@ -3256,20 +3331,20 @@
                     # filter by start and end offset, include Annotations that extend into the offset
                     if start_offset is not None and end_offset is not None:  # if the start and end offset are specified
                         latest_start = max(span.start_offset, start_offset)
                         earliest_end = min(span.end_offset, end_offset)
                         is_overlapping = latest_start - earliest_end < 0
                     else:
                         is_overlapping = True
-
                     if label is not None:  # filter by Label
                         if label == annotation.label and is_overlapping:
                             add = True
                     elif is_overlapping:
                         add = True
+
             # as multiline Annotations will be added twice
             if add:
                 annotations.append(annotation)
                 add = False
 
         if fill:
             # todo: we cannot assure that the Document has a Category, so Annotations must not require label_set
@@ -4010,14 +4085,33 @@
             if original:
                 raise IndexError(f'Page id {page_id} was not found in {self}.')
             else:
                 if not page.id_ and page.copy_of_id == page_id:
                     logger.warning(f'Page id {page_id} was not found in {self}, only a Page copy.')
                     return page
 
+    @property
+    def bbox_dict(self) -> Dict:
+        """Get a dictionary of Document's character-level Bboxes."""
+        return {
+            key: {
+                'x0': value['x0'],
+                'x1': value['x1'],
+                'y0': value['y0'],
+                'y1': value['y1'],
+                'page_index': value['page_index'],
+                'page_number': value['page_index'] + 1,
+                'line_index': value['line_index'],
+                'text': value['text'],
+                'top': self.get_page_by_index(value['page_index']).height - value['y1'],
+                'bottom': self.get_page_by_index(value['page_index']).height - value['y0'],
+            }
+            for key, value in self.get_bbox().items()
+        }
+
 
 class Project(Data):
     """
     Access the information of a Project.
 
     For more details see https://dev.konfuzio.com/sdk/explanations.html#project-concept
     """
```

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240418152335
+Version: 0.3.4.dev20240502164651
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.4.dev20240502164651/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/setup.py` & `konfuzio_sdk-0.3.4.dev20240502164651/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_api.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         data = get_document_details(document_id=TEST_DOCUMENT_ID)
         assert set(data.keys()) == {
             'id',
             'project',
             'document_set',
             'number_of_pages',
             'data_file_name',
+            'data_file_producer',
             'file_url',
             'thumbnail_url',
             'ocr_time',
             'categorization_time',
             'extraction_time',
             'processing_time',
             'extraction_url',
@@ -188,14 +189,15 @@
         data = get_document_details(document_id=216836)
         assert set(data.keys()) == {
             'id',
             'project',
             'document_set',
             'number_of_pages',
             'data_file_name',
+            'data_file_producer',
             'file_url',
             'thumbnail_url',
             'ocr_time',
             'categorization_time',
             'extraction_time',
             'processing_time',
             'extraction_url',
@@ -360,14 +362,39 @@
         annotations = get_document_annotations(TEST_DOCUMENT_ID)['results']
         assert annotation['id'] in [annotation['id'] for annotation in annotations]
         # delete the annotation, i.e. change its status from feedback required to negative
         negative_id = delete_document_annotation(annotation['id'])
         # delete it a second time to remove this Annotation from the feedback stored as negative
         assert delete_document_annotation(negative_id, delete_from_database=True).status_code == 204
 
+    def post_document_annotation_as_bboxes(self):
+        """Test creating an Annotation that is based only on Bbox coordinates."""
+        label_id = 862
+        label_set_id = 64
+
+        bboxes = [
+            {'page_index': 0, 'x0': 198, 'x1': 300, 'y0': 508, 'y1': 517},
+        ]
+        document = Project(id_=TEST_PROJECT_ID, strict_data_validation=False).get_document_by_id(TEST_DOCUMENT_ID + 11)
+        document.update()
+
+        response = post_document_annotation(
+            document_id=TEST_DOCUMENT_ID + 11,
+            confidence=0.01,
+            label_id=label_id,
+            label_set_id=label_set_id,
+            revised=False,
+            is_correct=True,
+            spans=bboxes,
+        )
+
+        assert response.status_code == 201
+        annotation = json.loads(response.text)
+        assert delete_document_annotation(annotation['id'])
+
     def test_change_annotation(self):
         """Test modifying an existing Annotation."""
         r = change_document_annotation(annotation_id=4420022, label=860)
         assert r.status_code == 200
 
     def test_get_project_labels(self):
         """Download Labels from API for a Project."""
```

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_cli.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_data.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,58 @@
         doc.update()  # redownload Document information to check that the Annotation was not deleted online
         assert annotation in doc.get_annotations()
 
         # Test3: delete the Annotation from the Document online.
         annotation.delete()  # doc.update() performed internally when delete_online=True, which is default
         assert annotation not in doc.get_annotations()
 
+    def test_create_bbox_annotation(self):
+        """Test creating a Bbox-based Annotation."""
+        doc = self.project.get_document_by_id(TEST_DOCUMENT_ID)
+        doc.status = 2
+        doc.get_bbox()
+        label = self.project.get_label_by_id(862)
+        bbox = {'page_index': 0, 'x0': 198, 'x1': 300, 'y0': 508, 'y1': 517}
+        annotation_set = AnnotationSet(document=doc, label_set=self.project.get_label_set_by_id(64))
+        annotation = Annotation(
+            document=doc,
+            annotation_set=annotation_set,
+            label=label,
+            label_set_id=64,
+            accuracy=1.0,
+            is_correct=True,
+            bboxes=[bbox],
+        )
+        annotation.save(label_set_id=64)
+        assert annotation in doc.annotations()
+        doc.update()
+        assert annotation in doc.annotations()
+        assert round(annotation.bbox().x0) == 199
+        assert round(annotation.bbox().x1) == 287
+        assert round(annotation.bbox().y0) == 509
+        assert round(annotation.bbox().y1) == 517
+        annotation.delete(delete_online=True)
+
+    def test_create_empty_bbox_annotation(self):
+        """Test creating an empty Annotation using empty Bbox is impossible."""
+        doc = self.project.get_document_by_id(TEST_DOCUMENT_ID)
+        label = self.project.get_label_by_id(862)
+        bbox = {'page_index': 0, 'x0': 1, 'x1': 4, 'y0': 1, 'y1': 4}
+        annotation_set = AnnotationSet(document=doc, label_set=self.project.get_label_set_by_id(64))
+        with pytest.raises(NotImplementedError):
+            Annotation(
+                document=doc,
+                annotation_set=annotation_set,
+                label=label,
+                label_set_id=64,
+                accuracy=1.0,
+                is_correct=True,
+                bboxes=[bbox],
+            )
+
     def test_get_sentence_spans_from_bbox(self):
         """Test to get sentence Spans in a bounding box."""
         document = self.project.get_document_by_id(5679477)
         document = WhitespaceTokenizer().tokenize(deepcopy(document))
         page = document.get_page_by_index(0)
 
         bbox = Bbox(x0=39, y0=728, x1=512, y1=742, page=page)
@@ -1115,15 +1159,15 @@
         page = Page(id_=None, document=document, start_offset=0, end_offset=4, number=1, original_size=(12, 6))
         document_bbox = {'1': Bbox(x0=0, x1=1, y0=0, y1=1, page=page)}
         document.set_bboxes(document_bbox)
         # An Annotation can be created by providing a list of Spans or a list of bboxes.
         # In the latter case, the minimum information required is the start and end offsets corresponding
         # to the characters of each bbox.
         annotation_bboxes = [{'start_offset': 0, 'end_offset': 1}, {'start_offset': 3}]
-        with pytest.raises(ValueError, match='cannot read bbox'):
+        with pytest.raises(ValueError, match='cannot read Bbox'):
             Annotation(document=document, bboxes=annotation_bboxes, label=self.label, label_set=self.label_set)
 
     def test_add_annotation_with_label_set_none(self):
         """Test to add an Annotation to a Document where the LabelSet is None."""
         project = Project(id_=None)
         category = Category(project=project)
         label_set = LabelSet(project=project, categories=[category])
```

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_evaluate.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_extras.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_normalize.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_regex.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_samples.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_urls.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_utils.py` & `konfuzio_sdk-0.3.4.dev20240502164651/tests/test_utils.py`

 * *Files identical despite different names*

