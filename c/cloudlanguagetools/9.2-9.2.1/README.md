# Comparing `tmp/cloudlanguagetools-9.2.tar.gz` & `tmp/cloudlanguagetools-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-9.2.tar", last modified: Sat Mar  9 10:05:57 2024, max compression
+gzip compressed data, was "cloudlanguagetools-9.2.1.tar", last modified: Sat Mar  9 10:22:34 2024, max compression
```

## Comparing `cloudlanguagetools-9.2.tar` & `cloudlanguagetools-9.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2024-03-09 10:05:57.389817 cloudlanguagetools-9.2/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      591 2024-03-09 10:05:57.389817 cloudlanguagetools-9.2/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2024-03-09 10:05:57.388817 cloudlanguagetools-9.2/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23979 2024-03-09 10:04:38.000000 cloudlanguagetools-9.2/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17838 2023-07-22 00:24:24.000000 cloudlanguagetools-9.2/cloudlanguagetools/chatapi.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2147 2024-03-06 22:51:32.000000 cloudlanguagetools-9.2/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-9.2/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8251 2024-02-10 08:22:00.000000 cloudlanguagetools-9.2/cloudlanguagetools/elevenlabs.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13385 2024-01-15 07:13:28.000000 cloudlanguagetools-9.2/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-12-13 14:06:23.000000 cloudlanguagetools-9.2/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-9.2/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    14218 2024-03-06 22:51:32.000000 cloudlanguagetools-9.2/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2899 2023-08-16 01:07:51.000000 cloudlanguagetools-9.2/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    21916 2024-01-15 10:16:56.000000 cloudlanguagetools-9.2/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7658 2024-01-15 10:16:56.000000 cloudlanguagetools-9.2/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18543 2023-08-16 01:07:51.000000 cloudlanguagetools-9.2/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-9.2/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-9.2/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2024-03-09 02:10:08.000000 cloudlanguagetools-9.2/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5546 2023-08-16 01:07:51.000000 cloudlanguagetools-9.2/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2024-03-09 10:05:57.388817 cloudlanguagetools-9.2/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      591 2024-03-09 10:05:57.000000 cloudlanguagetools-9.2/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1430 2024-03-09 10:05:57.000000 cloudlanguagetools-9.2/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2024-03-09 10:05:57.000000 cloudlanguagetools-9.2/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       22 2024-03-09 10:05:57.000000 cloudlanguagetools-9.2/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2024-03-09 10:05:57.000000 cloudlanguagetools-9.2/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2024-03-09 10:05:57.389817 cloudlanguagetools-9.2/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      817 2024-03-09 10:05:54.000000 cloudlanguagetools-9.2/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2024-03-09 10:22:34.771459 cloudlanguagetools-9.2.1/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      593 2024-03-09 10:22:34.771459 cloudlanguagetools-9.2.1/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2024-03-09 10:22:34.770460 cloudlanguagetools-9.2.1/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23979 2024-03-09 10:04:38.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17838 2023-07-22 00:24:24.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/chatapi.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2147 2024-03-06 22:51:32.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8251 2024-02-10 08:22:00.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13385 2024-01-15 07:13:28.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-12-13 14:06:23.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    14218 2024-03-06 22:51:32.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2899 2023-08-16 01:07:51.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    21916 2024-01-15 10:16:56.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7658 2024-01-15 10:16:56.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18543 2023-08-16 01:07:51.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2024-03-09 02:10:08.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5546 2023-08-16 01:07:51.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-9.2.1/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2024-03-09 10:22:34.771459 cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      593 2024-03-09 10:22:34.000000 cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1430 2024-03-09 10:22:34.000000 cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2024-03-09 10:22:34.000000 cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       22 2024-03-09 10:22:34.000000 cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2024-03-09 10:22:34.000000 cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2024-03-09 10:22:34.771459 cloudlanguagetools-9.2.1/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      819 2024-03-09 10:22:31.000000 cloudlanguagetools-9.2.1/setup.py
```

### Comparing `cloudlanguagetools-9.2/LICENSE` & `cloudlanguagetools-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/PKG-INFO` & `cloudlanguagetools-9.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 9.2
+Version: 9.2.1
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/amazon.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/azure.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/chatapi.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/chatapi.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/constants.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/constants.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/deepl.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/elevenlabs.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/encryption.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/epitran.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/forvo.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/fptai.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/google.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/keys.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/keys.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/languages.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/naver.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/openai.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/servicemanager.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/spacy.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/test_services.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/voicen.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/watson.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-9.2.1/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 9.2
+Version: 9.2.1
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `cloudlanguagetools-9.2/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-9.2.1/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-9.2/setup.py` & `cloudlanguagetools-9.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='9.2',
+      version='9.2.1',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.11',
```

