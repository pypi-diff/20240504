# Comparing `tmp/latentscope-0.2.0.tar.gz` & `tmp/latentscope-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latentscope-0.2.0.tar", last modified: Wed May  1 21:55:19 2024, max compression
+gzip compressed data, was "latentscope-0.2.1.tar", last modified: Fri May  3 22:31:04 2024, max compression
```

## Comparing `latentscope-0.2.0.tar` & `latentscope-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.358158 latentscope-0.2.0/
--rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.0/LICENSE
--rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-01 21:55:19.357919 latentscope-0.2.0/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)    12893 2024-05-01 21:43:52.000000 latentscope-0.2.0/README.md
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.349647 latentscope-0.2.0/latentscope/
--rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/__version__.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.350807 latentscope-0.2.0/latentscope/models/
--rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.0/latentscope/models/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.2.0/latentscope/models/chat_models.json
--rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.2.0/latentscope/models/embedding_models.json
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.351907 latentscope-0.2.0/latentscope/models/providers/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.0/latentscope/models/providers/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.0/latentscope/models/providers/base.py
--rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.0/latentscope/models/providers/cohereai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.0/latentscope/models/providers/mistralai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.0/latentscope/models/providers/nltk.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.2.0/latentscope/models/providers/openai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.0/latentscope/models/providers/togetherai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.2.0/latentscope/models/providers/transformers.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.0/latentscope/models/providers/voyageai.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.352945 latentscope-0.2.0/latentscope/scripts/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.0/latentscope/scripts/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.0/latentscope/scripts/cluster-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.0/latentscope/scripts/cluster.py
--rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.0/latentscope/scripts/embed.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/scripts/ingest.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.2.0/latentscope/scripts/label_clusters.py
--rw-r--r--   0 enjalot    (501) staff       (20)     5930 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/scripts/scope.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.0/latentscope/scripts/umapper-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.0/latentscope/scripts/umapper.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.353780 latentscope-0.2.0/latentscope/server/
--rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.0/latentscope/server/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.0/latentscope/server/app.py
--rw-r--r--   0 enjalot    (501) staff       (20)     5099 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/bulk.py
--rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/datasets.py
--rw-r--r--   0 enjalot    (501) staff       (20)    13747 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/jobs.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.0/latentscope/server/search.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.0/latentscope/server/tags.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.354036 latentscope-0.2.0/latentscope/util/
--rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.0/latentscope/util/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.0/latentscope/util/configuration.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-01 21:55:19.350399 latentscope-0.2.0/latentscope.egg-info/
--rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/SOURCES.txt
--rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/dependency_links.txt
--rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/entry_points.txt
--rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/requires.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-01 21:55:19.000000 latentscope-0.2.0/latentscope.egg-info/top_level.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-01 21:55:19.358234 latentscope-0.2.0/setup.cfg
--rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.0/setup.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.982173 latentscope-0.2.1/
+-rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.1/LICENSE
+-rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-03 22:31:04.981852 latentscope-0.2.1/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)    12893 2024-05-01 21:43:52.000000 latentscope-0.2.1/README.md
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.972285 latentscope-0.2.1/latentscope/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-05-02 18:24:50.000000 latentscope-0.2.1/latentscope/__version__.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.973663 latentscope-0.2.1/latentscope/models/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.1/latentscope/models/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.2.1/latentscope/models/chat_models.json
+-rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.2.1/latentscope/models/embedding_models.json
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.975321 latentscope-0.2.1/latentscope/models/providers/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.1/latentscope/models/providers/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.1/latentscope/models/providers/base.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.1/latentscope/models/providers/cohereai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.1/latentscope/models/providers/mistralai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.1/latentscope/models/providers/nltk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.2.1/latentscope/models/providers/openai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.1/latentscope/models/providers/togetherai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.2.1/latentscope/models/providers/transformers.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.1/latentscope/models/providers/voyageai.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.976654 latentscope-0.2.1/latentscope/scripts/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.1/latentscope/scripts/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.1/latentscope/scripts/cluster-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.1/latentscope/scripts/cluster.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.1/latentscope/scripts/embed.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/scripts/ingest.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.2.1/latentscope/scripts/label_clusters.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6306 2024-05-02 18:45:04.000000 latentscope-0.2.1/latentscope/scripts/scope.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.1/latentscope/scripts/umapper-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.1/latentscope/scripts/umapper.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.977505 latentscope-0.2.1/latentscope/server/
+-rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.1/latentscope/server/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.1/latentscope/server/app.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     5645 2024-05-02 18:44:22.000000 latentscope-0.2.1/latentscope/server/bulk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/server/datasets.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    13927 2024-05-02 18:50:28.000000 latentscope-0.2.1/latentscope/server/jobs.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.1/latentscope/server/search.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/server/tags.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.977744 latentscope-0.2.1/latentscope/util/
+-rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.1/latentscope/util/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.1/latentscope/util/configuration.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.973299 latentscope-0.2.1/latentscope.egg-info/
+-rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/SOURCES.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/dependency_links.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/entry_points.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/requires.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/top_level.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-03 22:31:04.982235 latentscope-0.2.1/setup.cfg
+-rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.1/setup.py
```

### Comparing `latentscope-0.2.0/LICENSE` & `latentscope-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/PKG-INFO` & `latentscope-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.26.1
```

### Comparing `latentscope-0.2.0/README.md` & `latentscope-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/__init__.py` & `latentscope-0.2.1/latentscope/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/__init__.py` & `latentscope-0.2.1/latentscope/models/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/chat_models.json` & `latentscope-0.2.1/latentscope/models/chat_models.json`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/embedding_models.json` & `latentscope-0.2.1/latentscope/models/embedding_models.json`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/base.py` & `latentscope-0.2.1/latentscope/models/providers/base.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/cohereai.py` & `latentscope-0.2.1/latentscope/models/providers/cohereai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/mistralai.py` & `latentscope-0.2.1/latentscope/models/providers/mistralai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/nltk.py` & `latentscope-0.2.1/latentscope/models/providers/nltk.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/openai.py` & `latentscope-0.2.1/latentscope/models/providers/openai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/togetherai.py` & `latentscope-0.2.1/latentscope/models/providers/togetherai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/transformers.py` & `latentscope-0.2.1/latentscope/models/providers/transformers.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/models/providers/voyageai.py` & `latentscope-0.2.1/latentscope/models/providers/voyageai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/cluster-1d.py` & `latentscope-0.2.1/latentscope/scripts/cluster-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/cluster.py` & `latentscope-0.2.1/latentscope/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/embed.py` & `latentscope-0.2.1/latentscope/scripts/embed.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/ingest.py` & `latentscope-0.2.1/latentscope/scripts/ingest.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/label_clusters.py` & `latentscope-0.2.1/latentscope/scripts/label_clusters.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/scope.py` & `latentscope-0.2.1/latentscope/scripts/scope.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,9 +124,16 @@
     with open(file_path, 'w') as f:
         json.dump(scope, f, indent=2)
     
     transactions_file_path = os.path.join(directory, id + "-transactions.json")
     if not os.path.exists(transactions_file_path):
         with open(transactions_file_path, 'w') as f:
             json.dump([], f)
+    
+    input_df = pd.read_parquet(os.path.join(DATA_DIR, dataset_id, "input.parquet"))
+    input_df.reset_index(inplace=True)
+    input_df = input_df[input_df['index'].isin(scope_parquet['ls_index'])]
+    combined_df = input_df.join(scope_parquet.set_index('ls_index'), on='index', rsuffix='_ls')
+    combined_df.to_parquet(os.path.join(directory, id + "-input.parquet"))
+
+    print("wrote scope", id)
 
-    print("wrote scope", id)
```

### Comparing `latentscope-0.2.0/latentscope/scripts/umapper-1d.py` & `latentscope-0.2.1/latentscope/scripts/umapper-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/scripts/umapper.py` & `latentscope-0.2.1/latentscope/scripts/umapper.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/server/__init__.py` & `latentscope-0.2.1/latentscope/server/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/server/app.py` & `latentscope-0.2.1/latentscope/server/app.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/server/bulk.py` & `latentscope-0.2.1/latentscope/server/bulk.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,15 @@
   new_label = clusters[new_cluster]
   # change the cluster of the rows
   df.loc[df['ls_index'].isin(row_ids), "cluster"] = new_cluster
   df.loc[df['ls_index'].isin(row_ids), "label"] = new_label["label"]
 
   # write the parquet
   df.to_parquet(scope_file)
+  update_combined(df, dataset_id, scope_id)
 
   # recalculate the hulls
   for c in clusters:
       indices = df[df['cluster'] == c["cluster"]]["ls_index"].tolist()
       label_points = df[df['cluster'] == c["cluster"]][['x', 'y']].values
       if(len(label_points) > 0):
         hull = ConvexHull(label_points)
@@ -100,14 +101,17 @@
   clusters = scope_meta["cluster_labels_lookup"]
   updated = clusters[cluster]
   updated["label"] = new_label
 
   # update the label column in the parquet
   df[df['cluster'] == cluster]['label'] = new_label
   df.to_parquet(scope_file)
+
+  update_combined(df, dataset_id, scope_id)
+
   #write the scope meta to file
   with open(scope_meta_file, "w") as f:
     json.dump(scope_meta, f, indent=2)
 
   write_transaction(dataset_id, scope_id, "change_cluster_name", {
     "cluster": cluster,
     "new_label": new_label
@@ -127,14 +131,16 @@
   scope_file = os.path.join(DATA_DIR, dataset_id, "scopes", scope_id + ".parquet")
   df = pd.read_parquet(scope_file)
   df = df[~df['ls_index'].isin(row_ids)]
   df.reset_index(drop=True, inplace=True)
 
   df.to_parquet(scope_file)
 
+  update_combined(df, dataset_id, scope_id)
+
   # recalculate hulls
   scope_meta_file = os.path.join(DATA_DIR, dataset_id, "scopes", scope_id + ".json")
   with open(scope_meta_file) as f:
     scope_meta = json.load(f)
   clusters = scope_meta["cluster_labels_lookup"]
   for c in clusters:
     indices = df[df['cluster'] == c["cluster"]]["ls_index"].tolist()
@@ -152,7 +158,13 @@
     json.dump(scope_meta, f, indent=2)
 
   write_transaction(dataset_id, scope_id, "delete_rows", {
     "row_ids": row_ids
   })
   return jsonify({"success": True})
 
+def update_combined(df, dataset_id, scope_id):
+  input_df = pd.read_parquet(os.path.join(DATA_DIR, dataset_id, "input.parquet"))
+  input_df.reset_index(inplace=True)
+  input_df = input_df[input_df['index'].isin(df['ls_index'])]
+  combined_df = input_df.join(df.set_index('ls_index'), on='index', rsuffix='_ls')
+  combined_df.to_parquet(os.path.join(DATA_DIR, dataset_id, "scopes", scope_id + "-input.parquet"))
```

### Comparing `latentscope-0.2.0/latentscope/server/datasets.py` & `latentscope-0.2.1/latentscope/server/datasets.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/server/jobs.py` & `latentscope-0.2.1/latentscope/server/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,16 @@
             with open(os.path.join(umap_dir, file), 'r') as f:
                 umap_data = json.load(f)
             if umap_data.get('embedding_id') == embedding_id:
                 umaps_to_delete.append(file.replace('.json', ''))
     
 
     job_id = str(uuid.uuid4())
-    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "embeddings", f"{embedding_id}*")}"'
+    path = os.path.join(DATA_DIR, dataset, "embeddings", f"{embedding_id}*").replace(" ", "\\ ")
+    command = f'rm -rf {path}'
     for umap in umaps_to_delete:
         delete_umap(dataset, umap)
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/umap')
 def run_umap():
@@ -280,18 +281,20 @@
             with open(os.path.join(cluster_dir, file), 'r') as f:
                 cluster_data = json.load(f)
             if cluster_data.get('umap_id') == umap_id:
                 clusters_to_delete.append(file.replace('.json', ''))
     
 
     job_id = str(uuid.uuid4())
-    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "umaps", f"{umap_id}*")}"'
+    path = os.path.join(DATA_DIR, dataset, "umaps", f"{umap_id}*").replace(" ", "\\ ")
+    command = f'rm -rf {path}'
     # Create the rm -rf commands from the clusters_to_delete list
     for cluster in clusters_to_delete:
-        command += f'; rm "{os.path.join(DATA_DIR, dataset, "clusters", f"{cluster}*")}"'
+        cpath = os.path.join(DATA_DIR, dataset, "clusters", f"{cluster}*").replace(" ", "\\ ")
+        command += f'; rm -rf {cpath}'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/cluster')
 def run_cluster():
     dataset = request.args.get('dataset')
     umap_id = request.args.get('umap_id')
@@ -306,15 +309,16 @@
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/delete/cluster')
 def delete_cluster():
     dataset = request.args.get('dataset')
     cluster_id = request.args.get('cluster_id')
     job_id = str(uuid.uuid4())
-    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "clusters", f"{cluster_id}*")}"'
+    path = os.path.join(DATA_DIR, dataset, "clusters", f"{cluster_id}*").replace(" ", "\\ ")
+    command = f'rm -rf {path}'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
 
 @jobs_write_bp.route('/cluster_label')
 def run_cluster_label():
     dataset = request.args.get('dataset')
     chat_id = request.args.get('chat_id')
@@ -350,11 +354,12 @@
 
 @jobs_write_bp.route('/delete/scope')
 def delete_scope():
     dataset = request.args.get('dataset')
     scope_id = request.args.get('scope_id')
 
     job_id = str(uuid.uuid4())
-    command = f'rm -rf "{os.path.join(DATA_DIR, dataset, "scopes", f"{scope_id}*")}"'
+    path = os.path.join(DATA_DIR, dataset, "scopes", f"{scope_id}*").replace(" ", "\\ ")
+    command = f'rm -rf {path}'
     threading.Thread(target=run_job, args=(dataset, job_id, command)).start()
     return jsonify({"job_id": job_id})
```

### Comparing `latentscope-0.2.0/latentscope/server/search.py` & `latentscope-0.2.1/latentscope/server/search.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/server/tags.py` & `latentscope-0.2.1/latentscope/server/tags.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope/util/configuration.py` & `latentscope-0.2.1/latentscope/util/configuration.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope.egg-info/PKG-INFO` & `latentscope-0.2.1/latentscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.26.1
```

### Comparing `latentscope-0.2.0/latentscope.egg-info/SOURCES.txt` & `latentscope-0.2.1/latentscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope.egg-info/entry_points.txt` & `latentscope-0.2.1/latentscope.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/latentscope.egg-info/requires.txt` & `latentscope-0.2.1/latentscope.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.0/setup.py` & `latentscope-0.2.1/setup.py`

 * *Files identical despite different names*

