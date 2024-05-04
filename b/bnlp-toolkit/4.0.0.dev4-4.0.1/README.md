# Comparing `tmp/bnlp_toolkit-4.0.0.dev4.tar.gz` & `tmp/bnlp_toolkit-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlp_toolkit-4.0.0.dev4.tar", last modified: Mon Aug 14 11:32:03 2023, max compression
+gzip compressed data, was "bnlp_toolkit-4.0.1.tar", last modified: Sat May  4 18:52:26 2024, max compression
```

## Comparing `bnlp_toolkit-4.0.0.dev4.tar` & `bnlp_toolkit-4.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.507043 bnlp_toolkit-4.0.0.dev4/bnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.507043 bnlp_toolkit-4.0.0.dev4/bnlp/cleantext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/cleantext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/cleantext/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/cleantext/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/bnlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/corpus/_stopwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/corpus/corpus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/bnlp/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/embedding/doc2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/embedding/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/embedding/glove.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/embedding/word2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/token_classification_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/sentencepiece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/bnlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-14 11:31:53.000000 bnlp_toolkit-4.0.0.dev4/bnlp/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-14 11:32:03.000000 bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-14 11:32:03.000000 bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 11:32:03.000000 bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-14 11:32:03.000000 bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-14 11:32:03.000000 bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-14 11:32:03.511043 bnlp_toolkit-4.0.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-14 11:31:54.000000 bnlp_toolkit-4.0.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:26.000549 bnlp_toolkit-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-04 18:52:26.000549 bnlp_toolkit-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/cleantext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/cleantext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/cleantext/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/cleantext/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/corpus/_stopwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/corpus/corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/embedding/doc2vec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/embedding/glove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/embedding/word2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/token_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/token_classification/ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/token_classification/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/token_classification/token_classification_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/tokenizer/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/tokenizer/nltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/tokenizer/sentencepiece.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:25.996549 bnlp_toolkit-4.0.1/bnlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 18:52:21.000000 bnlp_toolkit-4.0.1/bnlp/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:26.000549 bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-04 18:52:25.000000 bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-04 18:52:25.000000 bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:52:25.000000 bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-04 18:52:25.000000 bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 18:52:25.000000 bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:52:26.000549 bnlp_toolkit-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-04 18:52:22.000000 bnlp_toolkit-4.0.1/setup.py
```

### Comparing `bnlp_toolkit-4.0.0.dev4/LICENSE` & `bnlp_toolkit-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/PKG-INFO` & `bnlp_toolkit-4.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-Metadata-Version: 2.1
-Name: bnlp_toolkit
-Version: 4.0.0.dev4
-Summary: BNLP is a natural language processing toolkit for Bengali Language
-Home-page: https://github.com/sagorbrur/bnlp
-Author: Sagor Sarker
-Author-email: sagorhem3532@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: fasttext
-License-File: LICENSE
-
 # Bengali Natural Language Processing(BNLP)
 
 [![PyPI version](https://img.shields.io/pypi/v/bnlp_toolkit)](https://pypi.org/project/bnlp-toolkit/)
-[![Downloads](https://pepy.tech/badge/bnlp-toolkit)](https://pepy.tech/project/bnlp-toolkit)
+[![Downloads](https://static.pepy.tech/badge/bnlp_toolkit)](https://pepy.tech/project/bnlp_toolkit)
 
 BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Bangla Text Cleaning** for Bengali NLP purposes.
 
 
 ## Features
 - Tokenization
    - [Basic Tokenizer](./docs/README.md#basic-tokenizer)
@@ -48,15 +32,15 @@
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
   ```
-  - Python: 3.6, 3.7, 3.8, 3.9, 3.10
+  - Python: 3.8, 3.9, 3.10, 3.11
   - OS: Linux, Windows, Mac
 
 ### Build from source
 ```
 git clone https://github.com/sagorbrur/bnlp.git
 cd bnlp
 python setup.py install
@@ -72,17 +56,17 @@
 raw_text = "আমি বাংলায় গান গাই।"
 tokens = tokenizer(raw_text)
 print(tokens)
 # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
 ```
 
 ## Documentation
-Full documentation are available [here](./docs/README.md)
+Full documentation are available [here](https://github.com/sagorbrur/bnlp/tree/master/docs)
 
-If you are using previous version of **bnlp** check the document [archive]()
+If you are using previous version of **bnlp** check the documentation [archive](https://github.com/sagorbrur/bnlp/tree/master/docs/archive)
 
 ## Contributor Guide
 
 Check [CONTRIBUTING.md](https://github.com/sagorbrur/bnlp/blob/master/CONTRIBUTING.md) page for details.
 
 
 ## Thanks To
```

### Comparing `bnlp_toolkit-4.0.0.dev4/README.md` & `bnlp_toolkit-4.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,38 @@
+Metadata-Version: 2.1
+Name: bnlp_toolkit
+Version: 4.0.1
+Summary: BNLP is a natural language processing toolkit for Bengali Language
+Home-page: https://github.com/sagorbrur/bnlp
+Author: Sagor Sarker
+Author-email: sagorhem3532@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sentencepiece==0.2.0
+Requires-Dist: gensim==4.3.2
+Requires-Dist: nltk==3.8.1
+Requires-Dist: numpy
+Requires-Dist: scipy==1.10.1
+Requires-Dist: sklearn-crfsuite==0.3.6
+Requires-Dist: tqdm==4.66.3
+Requires-Dist: ftfy==6.2.0
+Requires-Dist: emoji==1.7.0
+Requires-Dist: requests
+Provides-Extra: fasttext
+Requires-Dist: fasttext==0.9.2; extra == "fasttext"
+
 # Bengali Natural Language Processing(BNLP)
 
 [![PyPI version](https://img.shields.io/pypi/v/bnlp_toolkit)](https://pypi.org/project/bnlp-toolkit/)
-[![Downloads](https://pepy.tech/badge/bnlp-toolkit)](https://pepy.tech/project/bnlp-toolkit)
+[![Downloads](https://static.pepy.tech/badge/bnlp_toolkit)](https://pepy.tech/project/bnlp_toolkit)
 
 BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Bangla Text Cleaning** for Bengali NLP purposes.
 
 
 ## Features
 - Tokenization
    - [Basic Tokenizer](./docs/README.md#basic-tokenizer)
@@ -32,15 +59,15 @@
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
   ```
-  - Python: 3.6, 3.7, 3.8, 3.9, 3.10
+  - Python: 3.8, 3.9, 3.10, 3.11
   - OS: Linux, Windows, Mac
 
 ### Build from source
 ```
 git clone https://github.com/sagorbrur/bnlp.git
 cd bnlp
 python setup.py install
@@ -56,17 +83,17 @@
 raw_text = "আমি বাংলায় গান গাই।"
 tokens = tokenizer(raw_text)
 print(tokens)
 # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
 ```
 
 ## Documentation
-Full documentation are available [here](./docs/README.md)
+Full documentation are available [here](https://github.com/sagorbrur/bnlp/tree/master/docs)
 
-If you are using previous version of **bnlp** check the document [archive]()
+If you are using previous version of **bnlp** check the documentation [archive](https://github.com/sagorbrur/bnlp/tree/master/docs/archive)
 
 ## Contributor Guide
 
 Check [CONTRIBUTING.md](https://github.com/sagorbrur/bnlp/blob/master/CONTRIBUTING.md) page for details.
 
 
 ## Thanks To
```

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/__init__.py` & `bnlp_toolkit-4.0.1/bnlp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-__version__ = "4.0.0dev4"
 
+__version__ = "4.0.1"
 
 import os
 from bnlp.tokenizer.basic import BasicTokenizer
 from bnlp.tokenizer.nltk import NLTKTokenizer
 from bnlp.tokenizer.sentencepiece import (
     SentencepieceTokenizer, 
     SentencepieceTrainer,
 )
 
 from bnlp.embedding.word2vec import (
     BengaliWord2Vec,
     Word2VecTraining,
 )
 from bnlp.embedding.glove import BengaliGlove
+
 from bnlp.embedding.doc2vec import (
     BengaliDoc2vec, 
     BengaliDoc2vecTrainer,
 )
 
 from bnlp.token_classification.pos import BengaliPOS
 from bnlp.token_classification.ner import BengaliNER
```

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/cleantext/clean.py` & `bnlp_toolkit-4.0.1/bnlp/cleantext/clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     return remove_substrings(text, UNICODE_EMOJI["en"])
 
 def remove_number_or_digit(text, replace_with=""):
     return re.sub(constants.BANGLA_DIGIT_REGEX, replace_with, text)
 
 def remove_punctuations(text, replace_with=""):
     for punc in corpus.punctuations:
-        print(punc)
         text = text.replace(punc, replace_with)
     
     return text
 
 class CleanText(object):
     def __init__(
         self,
```

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/cleantext/constants.py` & `bnlp_toolkit-4.0.1/bnlp/cleantext/constants.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/corpus/_stopwords.py` & `bnlp_toolkit-4.0.1/bnlp/corpus/_stopwords.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/corpus/corpus.py` & `bnlp_toolkit-4.0.1/bnlp/corpus/corpus.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/embedding/doc2vec.py` & `bnlp_toolkit-4.0.1/bnlp/embedding/doc2vec.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/embedding/fasttext.py` & `bnlp_toolkit-4.0.1/bnlp/embedding/fasttext.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/embedding/glove.py` & `bnlp_toolkit-4.0.1/bnlp/embedding/glove.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/embedding/word2vec.py` & `bnlp_toolkit-4.0.1/bnlp/embedding/word2vec.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/ner.py` & `bnlp_toolkit-4.0.1/bnlp/token_classification/ner.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/pos.py` & `bnlp_toolkit-4.0.1/bnlp/token_classification/pos.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/token_classification/token_classification_trainer.py` & `bnlp_toolkit-4.0.1/bnlp/token_classification/token_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/basic.py` & `bnlp_toolkit-4.0.1/bnlp/tokenizer/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         return self.tokenize(text)
 
     def tokenize(self, text: str) -> List[str]:
         """Tokenizes a piece of text."""
         text = convert_to_unicode(text)
         # handle (.) in bangla text
         text = text.replace('.', DUMMYTOKEN)
-
         orig_tokens = whitespace_tokenize(text)
         split_tokens = []
         for token in orig_tokens:
             split_tokens.extend(self._run_split_on_punc(token))
 
         output_tokens = whitespace_tokenize(" ".join(split_tokens))
         # get (.) back in output tokens
```

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/nltk.py` & `bnlp_toolkit-4.0.1/bnlp/tokenizer/nltk.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 try:
     nltk.data.find("tokenizers/punkt")
 except LookupError:
     print("punkt not found. downloading...")
     nltk.download("punkt")
 
+DUMMYTOKEN = "XTEMPTOKEN"
 
 DUMMYTOKEN = "XTEMPDOT"
 
 class NLTKTokenizer:
     def word_tokenize(self, text: str) -> List[str]:
         text = text.replace(".", DUMMYTOKEN)  # to deal with abbreviations
         text = text.replace("।", ".")
```

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/tokenizer/sentencepiece.py` & `bnlp_toolkit-4.0.1/bnlp/tokenizer/sentencepiece.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/utils/config.py` & `bnlp_toolkit-4.0.1/bnlp/utils/config.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/utils/downloader.py` & `bnlp_toolkit-4.0.1/bnlp/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp/utils/utils.py` & `bnlp_toolkit-4.0.1/bnlp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/PKG-INFO` & `bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 Metadata-Version: 2.1
-Name: bnlp-toolkit
-Version: 4.0.0.dev4
+Name: bnlp_toolkit
+Version: 4.0.1
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: fasttext
 License-File: LICENSE
+Requires-Dist: sentencepiece==0.2.0
+Requires-Dist: gensim==4.3.2
+Requires-Dist: nltk==3.8.1
+Requires-Dist: numpy
+Requires-Dist: scipy==1.10.1
+Requires-Dist: sklearn-crfsuite==0.3.6
+Requires-Dist: tqdm==4.66.3
+Requires-Dist: ftfy==6.2.0
+Requires-Dist: emoji==1.7.0
+Requires-Dist: requests
+Provides-Extra: fasttext
+Requires-Dist: fasttext==0.9.2; extra == "fasttext"
 
 # Bengali Natural Language Processing(BNLP)
 
 [![PyPI version](https://img.shields.io/pypi/v/bnlp_toolkit)](https://pypi.org/project/bnlp-toolkit/)
-[![Downloads](https://pepy.tech/badge/bnlp-toolkit)](https://pepy.tech/project/bnlp-toolkit)
+[![Downloads](https://static.pepy.tech/badge/bnlp_toolkit)](https://pepy.tech/project/bnlp_toolkit)
 
 BNLP is a natural language processing toolkit for Bengali Language. This tool will help you to **tokenize Bengali text**, **Embedding Bengali words**, **Embedding Bengali Document**, **Bengali POS Tagging**, **Bengali Name Entity Recognition**, **Bangla Text Cleaning** for Bengali NLP purposes.
 
 
 ## Features
 - Tokenization
    - [Basic Tokenizer](./docs/README.md#basic-tokenizer)
@@ -48,15 +59,15 @@
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
   ```
-  - Python: 3.6, 3.7, 3.8, 3.9, 3.10
+  - Python: 3.8, 3.9, 3.10, 3.11
   - OS: Linux, Windows, Mac
 
 ### Build from source
 ```
 git clone https://github.com/sagorbrur/bnlp.git
 cd bnlp
 python setup.py install
@@ -72,17 +83,17 @@
 raw_text = "আমি বাংলায় গান গাই।"
 tokens = tokenizer(raw_text)
 print(tokens)
 # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
 ```
 
 ## Documentation
-Full documentation are available [here](./docs/README.md)
+Full documentation are available [here](https://github.com/sagorbrur/bnlp/tree/master/docs)
 
-If you are using previous version of **bnlp** check the document [archive]()
+If you are using previous version of **bnlp** check the documentation [archive](https://github.com/sagorbrur/bnlp/tree/master/docs/archive)
 
 ## Contributor Guide
 
 Check [CONTRIBUTING.md](https://github.com/sagorbrur/bnlp/blob/master/CONTRIBUTING.md) page for details.
 
 
 ## Thanks To
```

### Comparing `bnlp_toolkit-4.0.0.dev4/bnlp_toolkit.egg-info/SOURCES.txt` & `bnlp_toolkit-4.0.1/bnlp_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-4.0.0.dev4/setup.py` & `bnlp_toolkit-4.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 import setuptools
 
 
 setuptools.setup(
     name="bnlp_toolkit",
-    version="4.0.0dev4",
+    version="4.0.1",
     author="Sagor Sarker",
     author_email="sagorhem3532@gmail.com",
     description="BNLP is a natural language processing toolkit for Bengali Language",
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sagorbrur/bnlp",
     license="MIT",
@@ -16,22 +16,22 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
-        "sentencepiece",
-        "gensim",
-        "nltk",
+        "sentencepiece==0.2.0",
+        "gensim==4.3.2",
+        "nltk==3.8.1",
         "numpy",
-        "scipy",
-        "sklearn-crfsuite",
-        "tqdm",
-        "ftfy",
+        "scipy==1.10.1",
+        "sklearn-crfsuite==0.3.6",
+        "tqdm==4.66.3",
+        "ftfy==6.2.0",
         "emoji==1.7.0",
         "requests",
     ],
     extras_require={
         "fasttext": ["fasttext==0.9.2"],
     },
 )
```

