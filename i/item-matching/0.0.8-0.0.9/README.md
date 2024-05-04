# Comparing `tmp/item_matching-0.0.8.tar.gz` & `tmp/item_matching-0.0.9.tar.gz`

## Comparing `item_matching-0.0.8.tar` & `item_matching-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 item_matching-0.0.8/.DS_Store
--rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 item_matching-0.0.8/examples/embed_bge.ipynb
--rw-r--r--   0        0        0    29136 2020-02-02 00:00:00.000000 item_matching-0.0.8/examples/embed_clip.ipynb
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 item_matching-0.0.8/examples/embed_tfidf.ipynb
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 item_matching-0.0.8/src/item_matching/__init__.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 item_matching-0.0.8/src/item_matching/main.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 item_matching-0.0.8/src/item_matching/build_index/func.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 item_matching-0.0.8/src/item_matching/build_index/matching.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 item_matching-0.0.8/src/item_matching/build_index/model.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 item_matching-0.0.8/test/download_images.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 item_matching-0.0.8/test/match_img.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 item_matching-0.0.8/test/match_text_by_df.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 item_matching-0.0.8/test/match_text_by_path.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 item_matching-0.0.8/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 item_matching-0.0.8/LICENSE
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 item_matching-0.0.8/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 item_matching-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 item_matching-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 item_matching-0.0.9/examples/embed_bge.ipynb
+-rw-r--r--   0        0        0    29136 2020-02-02 00:00:00.000000 item_matching-0.0.9/examples/embed_clip.ipynb
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 item_matching-0.0.9/examples/embed_tfidf.ipynb
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 item_matching-0.0.9/src/item_matching/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 item_matching-0.0.9/src/item_matching/main.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 item_matching-0.0.9/src/item_matching/build_index/func.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 item_matching-0.0.9/src/item_matching/build_index/matching.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 item_matching-0.0.9/src/item_matching/build_index/model.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 item_matching-0.0.9/test/download_images.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 item_matching-0.0.9/test/match_img.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 item_matching-0.0.9/test/match_text_by_df.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 item_matching-0.0.9/test/match_text_by_path.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 item_matching-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 item_matching-0.0.9/LICENSE
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 item_matching-0.0.9/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 item_matching-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 item_matching-0.0.9/PKG-INFO
```

### Comparing `item_matching-0.0.8/examples/embed_bge.ipynb` & `item_matching-0.0.9/examples/embed_bge.ipynb`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/examples/embed_clip.ipynb` & `item_matching-0.0.9/examples/embed_clip.ipynb`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/examples/embed_tfidf.ipynb` & `item_matching-0.0.9/examples/embed_tfidf.ipynb`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/src/item_matching/main.py` & `item_matching-0.0.9/src/item_matching/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
             self.df_db = check_file_type(self.file_database)
             self.df_q = check_file_type(self.file_query)
 
         # Database
         if clean_text:
             self.df_db = self.clean_text(self.df_db, 'db')
             self.df_q = self.clean_text(self.df_q, 'q')
-        json_stats.update({'database shape': self.df_db.shape})
-        json_stats.update({'query shape': self.df_q.shape})
+        json_stats.update({'database shape': self.df_db.shape[0]})
+        json_stats.update({'query shape': self.df_q.shape[0]})
         print(json_stats['database shape'])
         print(json_stats['query shape'])
 
         # Match
         be = BELargeScale(self.path, text_sparse=512)
         if match_mode == 'image':
             be = BELargeScale(self.path, img_dim=True)
```

### Comparing `item_matching-0.0.8/src/item_matching/build_index/func.py` & `item_matching-0.0.9/src/item_matching/build_index/func.py`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/src/item_matching/build_index/matching.py` & `item_matching-0.0.9/src/item_matching/build_index/matching.py`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/src/item_matching/build_index/model.py` & `item_matching-0.0.9/src/item_matching/build_index/model.py`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/test/download_images.py` & `item_matching-0.0.9/test/download_images.py`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/test/match_img.py` & `item_matching-0.0.9/test/match_img.py`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/.gitignore` & `item_matching-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/LICENSE` & `item_matching-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `item_matching-0.0.8/pyproject.toml` & `item_matching-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "item_matching"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Kevin Khang", email="kevinkhang2909@gmail.com" },
 ]
 description = "A name matching package"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `item_matching-0.0.8/PKG-INFO` & `item_matching-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: item_matching
-Version: 0.0.8
+Version: 0.0.9
 Summary: A name matching package
 Project-URL: Homepage, https://github.com/kevinkhang2909/item_matching
 Project-URL: Bug Tracker, https://github.com/kevinkhang2909/item_matching/issues
 Author-email: Kevin Khang <kevinkhang2909@gmail.com>
 License: Copyright (c) 2024 Kevin Khang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

