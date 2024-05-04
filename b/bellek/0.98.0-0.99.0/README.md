# Comparing `tmp/bellek-0.98.0.tar.gz` & `tmp/bellek-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.98.0.tar", last modified: Wed Apr 24 20:00:54 2024, max compression
+gzip compressed data, was "bellek-0.99.0.tar", last modified: Wed Apr 24 20:11:12 2024, max compression
```

## Comparing `bellek-0.98.0.tar` & `bellek-0.99.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.130186 bellek-0.98.0/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.98.0/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.98.0/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-24 20:00:54.129402 bellek-0.98.0/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.98.0/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.098225 bellek-0.98.0/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    55622 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.103315 bellek-0.98.0/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.104086 bellek-0.98.0/bellek/hf/datasets/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/hf/datasets/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/datasets/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.106665 bellek-0.98.0/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    12968 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/llama2.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/llama3.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.109657 bellek-0.98.0/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/eval.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.110688 bellek-0.98.0/bellek/jerx/fewshot/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/fewshot/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9537 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/fewshot/llm.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.112076 bellek-0.98.0/bellek/jerx/offline/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/offline/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      984 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/offline/llm.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4108 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.113238 bellek-0.98.0/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.114724 bellek-0.98.0/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.116105 bellek-0.98.0/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.117608 bellek-0.98.0/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.118580 bellek-0.98.0/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.119337 bellek-0.98.0/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-24 20:00:50.000000 bellek-0.98.0/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.119775 bellek-0.98.0/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.120807 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.126556 bellek-0.98.0/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.127330 bellek-0.98.0/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.128575 bellek-0.98.0/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-24 20:00:51.000000 bellek-0.98.0/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:00:54.102599 bellek-0.98.0/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1807 2024-04-24 20:00:54.000000 bellek-0.98.0/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.98.0/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-24 20:00:53.000000 bellek-0.98.0/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-24 20:00:20.000000 bellek-0.98.0/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-24 20:00:54.130316 bellek-0.98.0/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.98.0/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.738212 bellek-0.99.0/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.99.0/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.99.0/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-24 20:11:12.737505 bellek-0.99.0/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.99.0/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.643111 bellek-0.99.0/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    55625 2024-04-24 20:11:09.000000 bellek-0.99.0/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.648110 bellek-0.99.0/bellek/hf/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.648951 bellek-0.99.0/bellek/hf/datasets/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/datasets/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1193 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/datasets/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.653525 bellek-0.99.0/bellek/hf/transformers/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/transformers/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    12992 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/transformers/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2039 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/transformers/llama2.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      790 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/transformers/llama3.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/hf/transformers/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.656384 bellek-0.99.0/bellek/jerx/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/eval.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.660120 bellek-0.99.0/bellek/jerx/fewshot/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/fewshot/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9537 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/fewshot/llm.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.661052 bellek-0.99.0/bellek/jerx/offline/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/offline/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      984 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/offline/llm.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4108 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/prompt.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.662128 bellek-0.99.0/bellek/jerx/reward/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/reward/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/reward/gpt.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1186 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/jerx/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.663820 bellek-0.99.0/bellek/lang/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/lang/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1575 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/lang/dataset.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/lang/qdecomp.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.665637 bellek-0.99.0/bellek/langchain/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/langchain/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/langchain/cache.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/langchain/obs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.667278 bellek-0.99.0/bellek/llama_index/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.668307 bellek-0.99.0/bellek/llama_index/data_structs/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/data_structs/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/data_structs/data_structs.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.669347 bellek-0.99.0/bellek/llama_index/graph_stores/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/graph_stores/kuzu.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.673118 bellek-0.99.0/bellek/llama_index/indices/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/indices/__init__.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.675008 bellek-0.99.0/bellek/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/llms.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/llama_index/obs.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/logging.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.731960 bellek-0.99.0/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/ml/vision.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.733409 bellek-0.99.0/bellek/musique/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/musique/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/musique/eval.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/testing.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.736547 bellek-0.99.0/bellek/text/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/text/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/text/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/utils.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-24 20:11:08.000000 bellek-0.99.0/bellek/wandb.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-24 20:11:12.647521 bellek-0.99.0/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-24 20:11:12.000000 bellek-0.99.0/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1807 2024-04-24 20:11:12.000000 bellek-0.99.0/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-24 20:11:12.000000 bellek-0.99.0/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-24 20:11:12.000000 bellek-0.99.0/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.99.0/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-24 20:11:12.000000 bellek-0.99.0/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-24 20:11:12.000000 bellek-0.99.0/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1316 2024-04-24 20:10:51.000000 bellek-0.99.0/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-24 20:11:12.740237 bellek-0.99.0/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.99.0/setup.py
```

### Comparing `bellek-0.98.0/LICENSE` & `bellek-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/PKG-INFO` & `bellek-0.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.98.0
+Version: 0.99.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.98.0/bellek/_modidx.py` & `bellek-0.99.0/bellek/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
                                                                                                                  'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.evaluate_': ( 'hf.transformers.experiment.html#evaluate_',
                                                                                                     'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.fine_tune': ( 'hf.transformers.experiment.html#fine_tune',
                                                                                                     'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.flat_pipeline': ( 'hf.transformers.experiment.html#flat_pipeline',
                                                                                                         'bellek/hf/transformers/experiment.py'),
+                                                   'bellek.hf.transformers.experiment.generate': ( 'hf.transformers.experiment.html#generate',
+                                                                                                   'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.make_datacollator': ( 'hf.transformers.experiment.html#make_datacollator',
                                                                                                             'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.make_pipeline': ( 'hf.transformers.experiment.html#make_pipeline',
                                                                                                         'bellek/hf/transformers/experiment.py'),
-                                                   'bellek.hf.transformers.experiment.predict': ( 'hf.transformers.experiment.html#predict',
-                                                                                                  'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.prepare_config_for_fp': ( 'hf.transformers.experiment.html#prepare_config_for_fp',
                                                                                                                 'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.prepare_model_for_inference': ( 'hf.transformers.experiment.html#prepare_model_for_inference',
                                                                                                                       'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.prepare_model_for_training': ( 'hf.transformers.experiment.html#prepare_model_for_training',
                                                                                                                      'bellek/hf/transformers/experiment.py'),
                                                    'bellek.hf.transformers.experiment.preprocess_config': ( 'hf.transformers.experiment.html#preprocess_config',
```

### Comparing `bellek-0.98.0/bellek/hf/datasets/utils.py` & `bellek-0.99.0/bellek/hf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/hf/transformers/experiment.py` & `bellek-0.99.0/bellek/hf/transformers/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/hf.transformers.experiment.ipynb.
 
 # %% auto 0
 __all__ = ['log', 'prepare_config_for_fp', 'preprocess_config', 'make_datacollator', 'prepare_model_for_training',
            'calculate_token_counts', 'fine_tune', 'prepare_model_for_inference', 'make_pipeline', 'flat_pipeline',
-           'predict', 'evaluate_']
+           'generate', 'evaluate_']
 
 # %% ../../../nbs/hf.transformers.experiment.ipynb 3
 from copy import deepcopy
 from math import ceil
 from typing import Any, Callable
 
 import torch
@@ -239,32 +239,22 @@
 def flat_pipeline(pipe):
     def func(inputs, **kwargs) -> list[str]:
         return [result[0]["generated_text"] for result in tqdm(pipe(inputs, **kwargs))]
 
     return func
 
 
-def predict(
+def generate(
     pipe,
     dataset,
-    *,
-    output_parse_fn: Callable[[str], Any] | None = None,
     **generation_kwargs,
 ):
-    output_parse_fn = output_parse_fn or (lambda x: x)
-
     # Setup generation parameters
     generation_kwargs["return_full_text"] = False
 
-    if "max_new_tokens" not in generation_kwargs:
-        tokenized_outputs = dataset.map(lambda examples: pipe.tokenizer(examples["output"]), batched=True)
-        token_counts = [len(input_ids) for input_ids in tokenized_outputs["input_ids"]]
-        log.info(f"Output token counts: min={min(token_counts)}, max={max(token_counts)}")
-        generation_kwargs["max_new_tokens"] = ceil(max(token_counts) / 8) * 8
-
     terminators = generation_kwargs.pop("terminators", [])
     eos_token_ids = {pipe.tokenizer.eos_token_id}
     for terminator in terminators:
         if isinstance(terminator, int):
             eos_token_ids.add(terminator)
         elif isinstance(terminator, str):
             eos_token_ids.add(pipe.tokenizer.convert_tokens_to_ids(terminator))
@@ -272,23 +262,17 @@
             raise ValueError(f"Invalid terminator token {terminator}.")
     generation_kwargs["eos_token_id"] = sorted(eos_token_ids)
 
     # Generate text
     log.info(f"Running pipeline on dataset with {len(dataset)} samples...")
     generations = flat_pipeline(pipe)(dataset["input"], **generation_kwargs)
 
-    # Parse outputs
-    predictions = [output_parse_fn(text) for text in generations]
-    references = [output_parse_fn(text) for text in dataset["output"]]
-
     # Create dataframe
     dataf = dataset.to_pandas()
     dataf["generation"] = generations
-    dataf["prediction"] = predictions
-    dataf["reference"] = references
 
     return dataf
 
 
 def evaluate_(
     config,
     *,
@@ -300,36 +284,54 @@
     import evaluate
 
     # Load validation dataset
     dataset_config = config.at("dataset.validation")
     assert dataset_config, "Validation dataset is not provided!"
     dataset = load_datasets(dataset_config)
     assert len(dataset) > 0, "Validation dataset is empty!"
-    
+
     # Ensure the dataset has input/output columns
     cols = dataset[0].keys()
     if "input" not in cols or "output" not in cols:
         if "messages" not in dataset.column_names:
             raise ValueError("Dataset must have 'messages' column if 'input' and 'output' columns are not provided.")
         dataset = dataset.map(
             lambda x: {"input": x["messages"][:-1], "output": x["messages"][-1]["content"]}
         ).remove_columns("messages")
 
     # Prepare text generation pipeline
     if tokenizer is None or model is None:
         tokenizer, model = _load_tokenizer_model(config)
 
+    # Set up pipeline
+    generation_params = config.at("evaluation.generation_params", {})
+    if "max_new_tokens" not in generation_params:
+        tokenized_outputs = dataset.map(lambda examples: tokenizer(examples["output"]), batched=True)
+        token_counts = [len(input_ids) for input_ids in tokenized_outputs["input_ids"]]
+        log.info(f"Output token counts: min={min(token_counts)}, max={max(token_counts)}")
+        generation_params["max_new_tokens"] = ceil(max(token_counts) / 8) * 8
+
     pipe = make_pipeline(config, tokenizer, model)
 
-    dataf = predict(
+    # Generate
+    dataf = generate(
         pipe,
         dataset,
-        output_parse_fn=output_parse_fn,
-        **config.at("evaluation.generation_params", {}),
+        **generation_params,
     )
 
-    # Compute metrics
+    # Parse outputs
+    assert set(dataf.columns).issuperset({"input", "output", "generation"}), "Dataframe is missing columns."
+    output_parse_fn = output_parse_fn or (lambda x: x)
+    dataf["prediction"] = dataf["generation"].map(output_parse_fn)
+    dataf["reference"] = dataf["output"].map(output_parse_fn)
+
+    # Compute scores
     metric = evaluate.load(config.at("evaluation.metric"))
     metric_kwargs = metric_kwargs or {}
-    scores = metric.compute(predictions=dataf["prediction"].values, references=dataf["reference"].values, **metric_kwargs)
+    scores = metric.compute(
+        predictions=dataf["prediction"].values,
+        references=dataf["reference"].values,
+        **metric_kwargs,
+    )
 
     return scores, dataf
```

### Comparing `bellek-0.98.0/bellek/hf/transformers/llama2.py` & `bellek-0.99.0/bellek/hf/transformers/llama2.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/hf/transformers/llama3.py` & `bellek-0.99.0/bellek/hf/transformers/llama3.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/hf/transformers/utils.py` & `bellek-0.99.0/bellek/hf/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/dataset.py` & `bellek-0.99.0/bellek/jerx/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/eval.py` & `bellek-0.99.0/bellek/jerx/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/fewshot/llm.py` & `bellek-0.99.0/bellek/jerx/fewshot/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/offline/llm.py` & `bellek-0.99.0/bellek/jerx/offline/llm.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/prompt.py` & `bellek-0.99.0/bellek/jerx/prompt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/reward/gpt.py` & `bellek-0.99.0/bellek/jerx/reward/gpt.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/jerx/utils.py` & `bellek-0.99.0/bellek/jerx/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/lang/dataset.py` & `bellek-0.99.0/bellek/lang/dataset.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/lang/qdecomp.py` & `bellek-0.99.0/bellek/lang/qdecomp.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/langchain/cache.py` & `bellek-0.99.0/bellek/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/langchain/obs.py` & `bellek-0.99.0/bellek/langchain/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/llama_index/data_structs/data_structs.py` & `bellek-0.99.0/bellek/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/llama_index/graph_stores/kuzu.py` & `bellek-0.99.0/bellek/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/base.py` & `bellek-0.99.0/bellek/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/llama_index/indices/knowledge_graph/retrievers.py` & `bellek-0.99.0/bellek/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/llama_index/llms.py` & `bellek-0.99.0/bellek/llama_index/llms.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/llama_index/obs.py` & `bellek-0.99.0/bellek/llama_index/obs.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/logging.py` & `bellek-0.99.0/bellek/logging.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/clip.py` & `bellek-0.99.0/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/coop.py` & `bellek-0.99.0/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/data.py` & `bellek-0.99.0/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/evaluation.py` & `bellek-0.99.0/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/experiment.py` & `bellek-0.99.0/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/layer.py` & `bellek-0.99.0/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/loss.py` & `bellek-0.99.0/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/mcd.py` & `bellek-0.99.0/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/ml/vision.py` & `bellek-0.99.0/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/musique/eval.py` & `bellek-0.99.0/bellek/musique/eval.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/testing.py` & `bellek-0.99.0/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/utils.py` & `bellek-0.99.0/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek/wandb.py` & `bellek-0.99.0/bellek/wandb.py`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/bellek.egg-info/PKG-INFO` & `bellek-0.99.0/bellek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.98.0
+Version: 0.99.0
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bellek-0.98.0/bellek.egg-info/SOURCES.txt` & `bellek-0.99.0/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.98.0/settings.ini` & `bellek-0.99.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.98.0
+version = 0.99.0
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `bellek-0.98.0/setup.py` & `bellek-0.99.0/setup.py`

 * *Files identical despite different names*

