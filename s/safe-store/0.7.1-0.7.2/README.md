# Comparing `tmp/safe_store-0.7.1.tar.gz` & `tmp/safe_store-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_store-0.7.1.tar", last modified: Sat Apr 20 01:04:55 2024, max compression
+gzip compressed data, was "safe_store-0.7.2.tar", last modified: Sat May  4 15:21:24 2024, max compression
```

## Comparing `safe_store-0.7.1.tar` & `safe_store-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 01:04:55.880758 safe_store-0.7.1/
--rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     7409 2024-04-20 01:04:55.879752 safe_store-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 01:04:55.857623 safe_store-0.7.1/safe_store/
--rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.7.1/safe_store/BM25Vectorizer.py
--rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.7.1/safe_store/__init__.py
--rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.7.1/safe_store/document_decomposer.py
--rw-rw-rw-   0        0        0    10919 2024-04-19 23:55:54.000000 safe_store-0.7.1/safe_store/generic_data_loader.py
--rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.7.1/safe_store/knowledge_base.py
--rw-rw-rw-   0        0        0    23889 2024-04-20 01:03:00.000000 safe_store-0.7.1/safe_store/text_vectorizer.py
--rw-rw-rw-   0        0        0     2569 2024-04-20 00:44:17.000000 safe_store-0.7.1/safe_store/tf_idf_vectorizer.py
--rw-rw-rw-   0        0        0      896 2024-04-20 01:00:58.000000 safe_store-0.7.1/safe_store/tfidf_loader.py
--rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.7.1/safe_store/utils.py
--rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.7.1/safe_store/word2vec.py
-drwxrwxrwx   0        0        0        0 2024-04-20 01:04:55.878744 safe_store-0.7.1/safe_store.egg-info/
--rw-rw-rw-   0        0        0     7409 2024-04-20 01:04:55.000000 safe_store-0.7.1/safe_store.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2024-04-20 01:04:55.000000 safe_store-0.7.1/safe_store.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 01:04:55.000000 safe_store-0.7.1/safe_store.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-04-20 01:04:55.000000 safe_store-0.7.1/safe_store.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-20 01:04:55.000000 safe_store-0.7.1/safe_store.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 01:04:55.880758 safe_store-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1601 2024-04-20 01:04:53.000000 safe_store-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:21:24.792459 safe_store-0.7.2/
+-rw-rw-rw-   0        0        0    11558 2024-01-25 22:10:12.000000 safe_store-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     7409 2024-05-04 15:21:24.791459 safe_store-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6333 2024-02-10 19:31:37.000000 safe_store-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 15:21:24.775642 safe_store-0.7.2/safe_store/
+-rw-rw-rw-   0        0        0     3941 2024-01-25 22:10:12.000000 safe_store-0.7.2/safe_store/BM25Vectorizer.py
+-rw-rw-rw-   0        0        0      203 2024-01-25 22:10:12.000000 safe_store-0.7.2/safe_store/__init__.py
+-rw-rw-rw-   0        0        0     3113 2024-01-25 22:10:12.000000 safe_store-0.7.2/safe_store/document_decomposer.py
+-rw-rw-rw-   0        0        0    10919 2024-04-19 23:55:54.000000 safe_store-0.7.2/safe_store/generic_data_loader.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.7.2/safe_store/knowledge_base.py
+-rw-rw-rw-   0        0        0    23889 2024-04-20 01:03:00.000000 safe_store-0.7.2/safe_store/text_vectorizer.py
+-rw-rw-rw-   0        0        0     2569 2024-04-20 00:44:17.000000 safe_store-0.7.2/safe_store/tf_idf_vectorizer.py
+-rw-rw-rw-   0        0        0      884 2024-05-04 12:44:04.000000 safe_store-0.7.2/safe_store/tfidf_loader.py
+-rw-rw-rw-   0        0        0      502 2024-01-25 22:10:12.000000 safe_store-0.7.2/safe_store/utils.py
+-rw-rw-rw-   0        0        0        0 2024-01-25 22:10:12.000000 safe_store-0.7.2/safe_store/word2vec.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:21:24.790161 safe_store-0.7.2/safe_store.egg-info/
+-rw-rw-rw-   0        0        0     7409 2024-05-04 15:21:24.000000 safe_store-0.7.2/safe_store.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-05-04 15:21:24.000000 safe_store-0.7.2/safe_store.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 15:21:24.000000 safe_store-0.7.2/safe_store.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-05-04 15:21:24.000000 safe_store-0.7.2/safe_store.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 15:21:24.000000 safe_store-0.7.2/safe_store.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 15:21:24.793461 safe_store-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2024-05-04 15:21:03.000000 safe_store-0.7.2/setup.py
```

### Comparing `safe_store-0.7.1/LICENSE` & `safe_store-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/PKG-INFO` & `safe_store-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `safe_store-0.7.1/README.md` & `safe_store-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/safe_store/BM25Vectorizer.py` & `safe_store-0.7.2/safe_store/BM25Vectorizer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/safe_store/document_decomposer.py` & `safe_store-0.7.2/safe_store/document_decomposer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/safe_store/generic_data_loader.py` & `safe_store-0.7.2/safe_store/generic_data_loader.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/safe_store/text_vectorizer.py` & `safe_store-0.7.2/safe_store/text_vectorizer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/safe_store/tf_idf_vectorizer.py` & `safe_store-0.7.2/safe_store/tf_idf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `safe_store-0.7.1/safe_store/tfidf_loader.py` & `safe_store-0.7.2/safe_store/tfidf_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from safe_store.tf_idf_vectorizer import TfidfVectorizer
 
 class TFIDFLoader:
     @staticmethod
     def create_vectorizer_from_dict(tfidf_info):
         vectorizer = TfidfVectorizer(**tfidf_info['params'])
         vectorizer.ngram_range = tuple(vectorizer.ngram_range)
-        vectorizer.vocabulary_ = tfidf_info['vocabulary']
-        vectorizer.idf_ = tfidf_info['idf_values']
+        vectorizer.vocab = tfidf_info['vocabulary']
+        vectorizer.idf = tfidf_info['idf_values']
         dt = vectorizer.dtype[8:-2]
         vectorizer.dtype = eval(dt)
         return vectorizer
 
     @staticmethod
     def create_dict_from_vectorizer(vectorizer):
         tfidf_info = {
-            "vocabulary": vectorizer.vocabulary_,
-            "idf_values": vectorizer.idf_,# dict(zip(vectorizer.get_feature_names(), )),
+            "vocabulary": vectorizer.vocab,
+            "idf_values": vectorizer.idf,# dict(zip(vectorizer.get_feature_names(), )),
             "params": vectorizer.get_params()
         }
         tfidf_info["params"]["dtype"]=str(tfidf_info["params"]["dtype"])
 
-        return tfidf_info
+        return tfidf_info
```

### Comparing `safe_store-0.7.1/safe_store.egg-info/PKG-INFO` & `safe_store-0.7.2/safe_store.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe_store
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library for safe document storage and vectorization.
 Home-page: https://github.com/ParisNeo/safe_store
 Author: ALOUI Saifeddine (ParisNeo)
 Author-email: aloui.seifeddine@email.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `safe_store-0.7.1/setup.py` & `safe_store-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Package metadata
 NAME = 'safe_store'
 DESCRIPTION = 'A library for safe document storage and vectorization.'
 URL = 'https://github.com/ParisNeo/safe_store'
 AUTHOR = 'ALOUI Saifeddine (ParisNeo)'
 AUTHOR_EMAIL = 'aloui.seifeddine@email.com'
 LICENSE = 'Apache 2.0'
-VERSION = '0.7.1'
+VERSION = '0.7.2'
 
 # Read dependencies from requirements.txt
 with open('requirements.txt', 'r') as req_file:
     INSTALL_REQUIRES = req_file.read().splitlines()
 
 # Packages to include (find_packages() automatically discovers and includes sub-packages)
 PACKAGES = find_packages()
```

