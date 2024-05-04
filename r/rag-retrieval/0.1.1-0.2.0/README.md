# Comparing `tmp/rag_retrieval-0.1.1.tar.gz` & `tmp/rag_retrieval-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_retrieval-0.1.1.tar", last modified: Sun Apr 14 16:43:15 2024, max compression
+gzip compressed data, was "rag_retrieval-0.2.0.tar", last modified: Sat May  4 09:15:10 2024, max compression
```

## Comparing `rag_retrieval-0.1.1.tar` & `rag_retrieval-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-04-14 16:43:15.901005 rag_retrieval-0.1.1/
--rw-r--r--   0 jcli       (501) staff       (20)     1055 2024-03-20 15:01:37.000000 rag_retrieval-0.1.1/LICENSE
--rw-r--r--   0 jcli       (501) staff       (20)     7263 2024-04-14 16:43:15.900807 rag_retrieval-0.1.1/PKG-INFO
--rw-r--r--   0 jcli       (501) staff       (20)     4829 2024-03-20 15:01:42.000000 rag_retrieval-0.1.1/README.md
--rw-r--r--   0 jcli       (501) staff       (20)     1413 2024-04-14 16:43:08.000000 rag_retrieval-0.1.1/pyproject.toml
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-04-14 16:43:15.897413 rag_retrieval-0.1.1/rag_retrieval/
--rw-r--r--   0 jcli       (501) staff       (20)       94 2024-04-14 16:19:19.000000 rag_retrieval-0.1.1/rag_retrieval/__init__.py
--rw-r--r--   0 jcli       (501) staff       (20)     2918 2024-04-14 16:27:51.000000 rag_retrieval-0.1.1/rag_retrieval/rag_retrieval.py
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-04-14 16:43:15.900027 rag_retrieval-0.1.1/rag_retrieval/reranker_models/
--rw-r--r--   0 jcli       (501) staff       (20)      694 2024-04-14 16:18:08.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/__init__.py
--rw-r--r--   0 jcli       (501) staff       (20)        0 2024-04-11 15:44:38.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/colbert_ranker.py
--rw-r--r--   0 jcli       (501) staff       (20)     8489 2024-04-14 16:12:38.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/cross_encoder_ranker.py
--rw-r--r--   0 jcli       (501) staff       (20)        0 2024-04-11 15:44:03.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/llm_rankers.py
--rw-r--r--   0 jcli       (501) staff       (20)      639 2024-04-13 14:51:56.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/ranker.py
--rw-r--r--   0 jcli       (501) staff       (20)     1482 2024-04-14 16:12:48.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/result.py
--rw-r--r--   0 jcli       (501) staff       (20)      389 2024-04-13 05:50:10.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/test.py
--rw-r--r--   0 jcli       (501) staff       (20)     1543 2024-04-14 16:43:02.000000 rag_retrieval-0.1.1/rag_retrieval/reranker_models/utils.py
--rw-r--r--   0 jcli       (501) staff       (20)      163 2024-04-13 14:58:00.000000 rag_retrieval-0.1.1/rag_retrieval/test.py
-drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-04-14 16:43:15.900297 rag_retrieval-0.1.1/rag_retrieval.egg-info/
--rw-r--r--   0 jcli       (501) staff       (20)     7263 2024-04-14 16:43:15.000000 rag_retrieval-0.1.1/rag_retrieval.egg-info/PKG-INFO
--rw-r--r--   0 jcli       (501) staff       (20)      641 2024-04-14 16:43:15.000000 rag_retrieval-0.1.1/rag_retrieval.egg-info/SOURCES.txt
--rw-r--r--   0 jcli       (501) staff       (20)        1 2024-04-14 16:43:15.000000 rag_retrieval-0.1.1/rag_retrieval.egg-info/dependency_links.txt
--rw-r--r--   0 jcli       (501) staff       (20)      114 2024-04-14 16:43:15.000000 rag_retrieval-0.1.1/rag_retrieval.egg-info/requires.txt
--rw-r--r--   0 jcli       (501) staff       (20)       14 2024-04-14 16:43:15.000000 rag_retrieval-0.1.1/rag_retrieval.egg-info/top_level.txt
--rw-r--r--   0 jcli       (501) staff       (20)       38 2024-04-14 16:43:15.901044 rag_retrieval-0.1.1/setup.cfg
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.563356 rag_retrieval-0.2.0/
+-rw-r--r--   0 jcli       (501) staff       (20)     1055 2024-03-20 15:01:37.000000 rag_retrieval-0.2.0/LICENSE
+-rw-r--r--   0 jcli       (501) staff       (20)     7263 2024-05-04 09:15:10.563154 rag_retrieval-0.2.0/PKG-INFO
+-rw-r--r--   0 jcli       (501) staff       (20)     4829 2024-03-20 15:01:42.000000 rag_retrieval-0.2.0/README.md
+-rw-r--r--   0 jcli       (501) staff       (20)     1419 2024-05-04 09:12:44.000000 rag_retrieval-0.2.0/pyproject.toml
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.558642 rag_retrieval-0.2.0/rag_retrieval/
+-rw-r--r--   0 jcli       (501) staff       (20)       89 2024-05-04 09:11:48.000000 rag_retrieval-0.2.0/rag_retrieval/__init__.py
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.557857 rag_retrieval-0.2.0/rag_retrieval/infer/
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.561770 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/
+-rw-r--r--   0 jcli       (501) staff       (20)      720 2024-05-04 08:58:48.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/__init__.py
+-rw-r--r--   0 jcli       (501) staff       (20)       28 2024-05-04 08:53:27.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/colbert_ranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)     8726 2024-05-04 08:53:42.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/cross_encoder_ranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)    14175 2024-05-04 08:53:50.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/llm_rankers.py
+-rw-r--r--   0 jcli       (501) staff       (20)      639 2024-04-13 14:51:56.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/ranker.py
+-rw-r--r--   0 jcli       (501) staff       (20)     1482 2024-04-14 16:12:48.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/result.py
+-rw-r--r--   0 jcli       (501) staff       (20)     1543 2024-04-14 16:43:02.000000 rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/utils.py
+-rw-r--r--   0 jcli       (501) staff       (20)     2978 2024-05-04 08:53:08.000000 rag_retrieval-0.2.0/rag_retrieval/reranker.py
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.562602 rag_retrieval-0.2.0/rag_retrieval.egg-info/
+-rw-r--r--   0 jcli       (501) staff       (20)     7263 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 jcli       (501) staff       (20)      640 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 jcli       (501) staff       (20)        1 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 jcli       (501) staff       (20)      114 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/requires.txt
+-rw-r--r--   0 jcli       (501) staff       (20)       14 2024-05-04 09:15:10.000000 rag_retrieval-0.2.0/rag_retrieval.egg-info/top_level.txt
+-rw-r--r--   0 jcli       (501) staff       (20)       38 2024-05-04 09:15:10.563397 rag_retrieval-0.2.0/setup.cfg
+drwxr-xr-x   0 jcli       (501) staff       (20)        0 2024-05-04 09:15:10.562240 rag_retrieval-0.2.0/tests/
+-rw-r--r--   0 jcli       (501) staff       (20)       99 2024-04-17 17:10:16.000000 rag_retrieval-0.2.0/tests/test_predict.py
```

### Comparing `rag_retrieval-0.1.1/LICENSE` & `rag_retrieval-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.1.1/PKG-INFO` & `rag_retrieval-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_retrieval
-Version: 0.1.1
+Version: 0.2.0
 Summary: A unified API for various RAG Retrieval  re-ranking models.
 Author-email: A grass in the car <suda.jcli@qq.com>
 Maintainer-email: A grass in the car <suda.jcli@qq.com>
 License: MIT License
         
         Copyright (c) 2024
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rag_retrieval Version: 0.1.1 Summary: A unified API
+Metadata-Version: 2.1 Name: rag_retrieval Version: 0.2.0 Summary: A unified API
 for various RAG Retrieval re-ranking models. Author-email: A grass in the car
 qq.com> Maintainer-email: A grass in the car
 qq.com> License: MIT License Copyright (c) 2024 Permission is hereby granted,
 free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `rag_retrieval-0.1.1/README.md` & `rag_retrieval-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.1.1/pyproject.toml` & `rag_retrieval-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 [build-system]
 requires = ["setuptools"] 
 build-backend = "setuptools.build_meta" 
 
 [tool.setuptools]
 packages = [
     "rag_retrieval",
-    "rag_retrieval.reranker_models",
+    "rag_retrieval.infer.reranker_models",
 ]
 
 [project]
 name = "rag_retrieval" 
 
 
-version = "0.1.1"
+version = "0.2.0"
 
 description = "A unified API for various RAG Retrieval  re-ranking models."
 
 readme = "README.md"
 
 requires-python = ">=3.8"
```

### Comparing `rag_retrieval-0.1.1/rag_retrieval/rag_retrieval.py` & `rag_retrieval-0.2.0/rag_retrieval/reranker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 
-from rag_retrieval.reranker_models import AVAILABLE_RANKERS
+from rag_retrieval.infer.reranker_models import AVAILABLE_RANKERS
 import os 
 
 os.environ.setdefault('TRANSFORMERS_NO_ADVISORY_WARNINGS', '1')
 
 
+
 DEFAULTS_MODEL_CLASS_TYPE={
     'CorssEncoderRanker',
     "ColBERTRanker",
     "LLMRanker"
 }
 
 DEFAULTS_MODEL_TYPE={
@@ -17,14 +18,15 @@
     "colbert",
     "cross-encoder"
 }
 
 DEPS_MAPPING = {
     "CorssEncoderRanker": "transformers",
     "ColBERTRanker": "transformers",
+    "LLMRanker":"transformers"
 }
 
 def _get_model_type(
     model_name: str, 
     model_type: Optional[str] = None,
     ):
 
@@ -55,14 +57,15 @@
 
 
 
 def Reranker(
     model_name: str,
     model_type: Optional[str] = None,
     verbose: int = 1,
+    **kwargs
     ):
 
     #Infer the model class of the reranker。（by model_name or model_type）
     model_class_type = _get_model_type(model_name,model_type)
     
     if model_class_type not in  DEFAULTS_MODEL_CLASS_TYPE:
         if model_type is not None:
@@ -75,15 +78,15 @@
             print(
                 "If your model is NOT intended to be ran as a one-label cross-encoder, please reload it and specify the model_type!",
                 "Otherwise, you may ignore this warning. You may specify `model_type='cross-encoder'` to suppress this warning in the future.",
             )
             model_class_type = "CorssEncoderRanker"
     try:
         print(f"Loading {model_class_type} model {model_name}")
-        return AVAILABLE_RANKERS[model_class_type](model_name, verbose=verbose)
+        return AVAILABLE_RANKERS[model_class_type](model_name, verbose=verbose,**kwargs)
     except KeyError:
         print(
             f"You don't have the necessary dependencies installed to use {model_class_type}."
         )
         print(
             f'Please install the necessary dependencies for {model_class_type} by running `pip install "rerankers[{DEPS_MAPPING[model_type]}]"`',
             'or `pip install "rerankers[all]" to install the dependencies for all reranker types.',
```

### Comparing `rag_retrieval-0.1.1/rag_retrieval/reranker_models/__init__.py` & `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 AVAILABLE_RANKERS = {}
 
 try:
-    from rag_retrieval.reranker_models.cross_encoder_ranker import CorssEncoderRanker
+    from rag_retrieval.infer.reranker_models.cross_encoder_ranker import CorssEncoderRanker
     AVAILABLE_RANKERS["CorssEncoderRanker"] = CorssEncoderRanker
 except Exception as e:
-    print(e)
     pass
 
-try:
-    from rag_retrieval.reranker_models.colbert_ranker import ColBERTRanker
-
-    AVAILABLE_RANKERS["ColBERTRanker"] = ColBERTRanker
-except ImportError:
-    pass
+# try:
+#     from rag_retrieval.reranker_models.colbert_ranker import ColBERTRanker
 
-try:
-    from rag_retrieval.reranker_models.api_rankers import APIRanker
-    AVAILABLE_RANKERS["APIRanker"] = APIRanker
-except ImportError:
-    pass
+#     AVAILABLE_RANKERS["ColBERTRanker"] = ColBERTRanker
+# except Exception as e:
+#     pass
+
+# try:
+#     from rag_retrieval.reranker_models.api_rankers import APIRanker
+#     AVAILABLE_RANKERS["APIRanker"] = APIRanker
+# except Exception as e:
+#     pass
 
 try:
-    from rag_retrieval.reranker_models.llm_rankers import LLMRanker
+    from rag_retrieval.infer.reranker_models.llm_rankers import LLMRanker
 
     AVAILABLE_RANKERS["LLMRanker"] = LLMRanker
-except ImportError:
+except Exception as e:
     pass
-
-
```

### Comparing `rag_retrieval-0.1.1/rag_retrieval/reranker_models/cross_encoder_ranker.py` & `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/cross_encoder_ranker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
+
 from typing import Union, List, Optional, Tuple
 from .ranker import BaseRanker
-
+from .result import RankedResults, Result
+from copy import deepcopy
 from .utils import get_device,get_dtype,vprint
 import tqdm
 
 import torch
 from transformers import AutoTokenizer, AutoModelForSequenceClassification
-from copy import deepcopy
-from .result import RankedResults, Result
 
 class CorssEncoderRanker(BaseRanker):
     def __init__(self, 
         model_name_or_path: str, 
         dtype: str = None,
         device: str = None,
         verbose: int = 1,
@@ -22,87 +22,94 @@
         self.device = get_device(device, verbose=self.verbose)
         self.dtype = get_dtype(dtype, device=self.device, verbose=self.verbose)
 
         self.model = AutoModelForSequenceClassification.from_pretrained(
             model_name_or_path, torch_dtype=self.dtype
         ).to(self.device)
 
+        vprint(f"Loaded model {self.model_name_or_path}", self.verbose)
+
         self.model.eval()
         self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
 
-        if device is not None and device.startswith('cuda:'):
-            self.num_gpus = torch.cuda.device_count()
-            if self.num_gpus > 1:
-                print(f"----------using {self.num_gpus}*GPUs----------")
-                self.model = torch.nn.DataParallel(self.model)
-        else:
-            self.num_gpus = 1
+        # if device is not None and device.startswith('cuda:'):
+        #     self.num_gpus = torch.cuda.device_count()
+        #     if self.num_gpus > 1:
+        #         vprint(f"----------using {self.num_gpus}*GPUs----------",self.verbose)
+        #         self.model = torch.nn.DataParallel(self.model)
+        # else:
+        #     self.num_gpus = 1
     
     @torch.no_grad()
     def compute_score(self, 
         sentence_pairs: Union[List[Tuple[str, str]], Tuple[str, str]],
         batch_size: int = 256,
         max_length: int = 512,
+        normalize: bool = False,
         enable_tqdm: bool = True,
     ):
-        if self.num_gpus > 0:
-            batch_size = batch_size * self.num_gpus
-        
+
+        # batch inference
+        # if self.num_gpus > 1:
+        #     batch_size = batch_size * self.num_gpus
+
         all_scores = []
         for start_index in tqdm.tqdm(range(0, len(sentence_pairs), batch_size), desc="Compute Scores",
                                     disable=not enable_tqdm):
             sentences_batch = sentence_pairs[start_index:start_index + batch_size]
             inputs = self.tokenizer(
                 sentences_batch,
                 padding=True,
                 truncation=True,
                 return_tensors='pt',
                 max_length=max_length,
             ).to(self.device)
 
             scores = self.model(**inputs).logits.view(-1, ).float()
-            if 'bce' in self.model_name_or_path:
+            if 'bce' in self.model_name_or_path or normalize:
                 scores = torch.sigmoid(scores)
             all_scores.extend(scores.cpu().numpy().tolist())
 
         if len(all_scores) == 1:
             return all_scores[0]
         return all_scores
 
     @torch.no_grad()
     def rerank(self, 
         query: str, 
         docs: Union[List[str], str] = None,
         batch_size: int = 256,
         max_length: int = 512,
+        normalize: bool = False,
         long_doc_process_strategy: str="max_score_slice",#['max_score_slice','max_length_truncation']
     ):  
         
         # remove invalid passages
         docs = [doc[:128000] for doc in docs if isinstance(doc, str) and 0 < len(doc)]
 
         if query is None or len(query) == 0 or len(docs) == 0:
             return {'rerank_passages': [], 'rerank_scores': []}
         
         vprint(f'long_doc_process_strategy is {long_doc_process_strategy}',self.verbose)
         if long_doc_process_strategy=='max_length_truncation':
-            return self.__max_length_truncation_rerank(query,docs,batch_size,max_length)
+            return self.__max_length_truncation_rerank(query,docs,batch_size,max_length,normalize)
         else:
-            return self.__max_score_slice_rerank(query,docs,batch_size,max_length)
+            return self.__max_score_slice_rerank(query,docs,batch_size,max_length,normalize)
 
     @torch.no_grad()
     def __max_length_truncation_rerank(self,
         query: str, 
         docs: Union[List[str], str] = None,
         batch_size: int = 256,
         max_length: int = 512,
+        normalize: bool = False,
     ):
         doc_ids = list(range(len(docs)))
         sentence_pairs=[ [query,doc]  for doc in docs]
-        all_scores = self.compute_score(sentence_pairs,batch_size,max_length,enable_tqdm=False)
+        all_scores = self.compute_score(sentence_pairs,batch_size,max_length,normalize=normalize,enable_tqdm=False)
 
         ranked_results = [
             Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
             for idx, (doc_id, doc, score) in enumerate(
                 sorted(zip(doc_ids, docs, all_scores), key=lambda x: x[2], reverse=True)
             )
         ]
@@ -110,48 +117,48 @@
 
     @torch.no_grad()
     def __max_score_slice_rerank(self,
         query: str, 
         docs: Union[List[str], str] = None,
         batch_size: int=256,
         max_length: int = 512,
+        normalize: bool = False,
         overlap_tokens_length: int=80,
     ):
 
         doc_ids = list(range(len(docs)))
         
         # preproc of tokenization
         sentence_pairs, sentence_pairs_idxs = self.__reranker_tokenize_preproc(
             query,
             docs, 
             max_length=max_length,
             overlap_tokens_length=overlap_tokens_length,
         )
 
         # batch inference
-        if self.num_gpus > 1:
-            batch_size = batch_size * self.num_gpus
+        # if self.num_gpus > 1:
+        #     batch_size = batch_size * self.num_gpus
 
         all_scores = []
         for start_index in range(0, len(sentence_pairs), batch_size):
             batch = self.tokenizer.pad(
                     sentence_pairs[start_index:start_index+batch_size],
                     padding=True,
                     max_length=None,
                     pad_to_multiple_of=None,
                     return_tensors="pt"
                 ).to(self.device)
-            #batch_on_device = {k: v.to(self.device) for k, v in batch.items()}
             scores = self.model(**batch).logits.view(-1,).float()
-            if 'bce' in self.model_name_or_path:
+            if 'bce' in self.model_name_or_path or normalize:
                 scores = torch.sigmoid(scores)
             all_scores.extend(scores.cpu().numpy().tolist())
 
         # ranking
-        merge_scores = [0 for _ in range(len(docs))]
+        merge_scores = [float("-inf") for _ in range(len(docs))]
         for idx, score in zip(sentence_pairs_idxs, all_scores):
             merge_scores[idx] = max(merge_scores[idx], score)
 
         ranked_results = [
             Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
             for idx, (doc_id, doc, score) in enumerate(
                 sorted(zip(doc_ids, docs, merge_scores), key=lambda x: x[2], reverse=True)
@@ -166,15 +173,14 @@
         overlap_tokens_length: int = 80,
     ):
 
         sep_id = self.tokenizer.sep_token_id
         def _merge_inputs(chunk1_raw, chunk2):
             chunk1 = deepcopy(chunk1_raw)
 
-            #add sep
             chunk1['input_ids'].append(sep_id)
             chunk1['input_ids'].extend(chunk2['input_ids'])
             chunk1['input_ids'].append(sep_id)
 
             chunk1['attention_mask'].append(chunk2['attention_mask'][0])
             chunk1['attention_mask'].extend(chunk2['attention_mask'])
             chunk1['attention_mask'].append(chunk2['attention_mask'][0])
```

### Comparing `rag_retrieval-0.1.1/rag_retrieval/reranker_models/ranker.py` & `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/ranker.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.1.1/rag_retrieval/reranker_models/result.py` & `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/result.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.1.1/rag_retrieval/reranker_models/utils.py` & `rag_retrieval-0.2.0/rag_retrieval/infer/reranker_models/utils.py`

 * *Files identical despite different names*

### Comparing `rag_retrieval-0.1.1/rag_retrieval.egg-info/PKG-INFO` & `rag_retrieval-0.2.0/rag_retrieval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag_retrieval
-Version: 0.1.1
+Version: 0.2.0
 Summary: A unified API for various RAG Retrieval  re-ranking models.
 Author-email: A grass in the car <suda.jcli@qq.com>
 Maintainer-email: A grass in the car <suda.jcli@qq.com>
 License: MIT License
         
         Copyright (c) 2024
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rag_retrieval Version: 0.1.1 Summary: A unified API
+Metadata-Version: 2.1 Name: rag_retrieval Version: 0.2.0 Summary: A unified API
 for various RAG Retrieval re-ranking models. Author-email: A grass in the car
 qq.com> Maintainer-email: A grass in the car
 qq.com> License: MIT License Copyright (c) 2024 Permission is hereby granted,
 free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

