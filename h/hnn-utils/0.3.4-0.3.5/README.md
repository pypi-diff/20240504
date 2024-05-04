# Comparing `tmp/hnn_utils-0.3.4.tar.gz` & `tmp/hnn_utils-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnn_utils-0.3.4.tar", max compression
+gzip compressed data, was "hnn_utils-0.3.5.tar", max compression
```

## Comparing `hnn_utils-0.3.4.tar` & `hnn_utils-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1068 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/LICENSE
--rw-r--r--   0        0        0      137 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/README.md
--rw-r--r--   0        0        0        0 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/__init__.py
--rw-r--r--   0        0        0       48 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/callbacks/__init__.py
--rw-r--r--   0        0        0     6566 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/callbacks/ema.py
--rw-r--r--   0        0        0      178 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/__init__.py
--rw-r--r--   0        0        0     2219 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/guacamol.py
--rw-r--r--   0        0        0     3119 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/utils.py
--rw-r--r--   0        0        0     1730 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/vocab/guac.json
--rw-r--r--   0        0        0     1843 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/vocab/guac_random.json
--rw-r--r--   0        0        0     5297 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/vocab/zinc20.json
--rw-r--r--   0        0        0     3133 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/datasets/zinc.py
--rw-r--r--   0        0        0     1370 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/ALiBi.py
--rw-r--r--   0        0        0     1677 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/RotaryEmbedding.py
--rw-r--r--   0        0        0    15836 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/Transformer.py
--rw-r--r--   0        0        0      164 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/__init__.py
--rw-r--r--   0        0        0     1247 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/ffn.py
--rw-r--r--   0        0        0     2000 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/functional.py
--rw-r--r--   0        0        0      800 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/hnn_utils/nn/normalization.py
--rw-r--r--   0        0        0      517 2024-05-02 14:40:45.675921 hnn_utils-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 hnn_utils-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/LICENSE
+-rw-r--r--   0        0        0      137 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/callbacks/__init__.py
+-rw-r--r--   0        0        0     6566 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/callbacks/ema.py
+-rw-r--r--   0        0        0      178 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/__init__.py
+-rw-r--r--   0        0        0     2219 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/guacamol.py
+-rw-r--r--   0        0        0     3119 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/utils.py
+-rw-r--r--   0        0        0     1730 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/vocab/guac.json
+-rw-r--r--   0        0        0     1843 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/vocab/guac_random.json
+-rw-r--r--   0        0        0     5297 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/vocab/zinc20.json
+-rw-r--r--   0        0        0     3295 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/datasets/zinc.py
+-rw-r--r--   0        0        0     1370 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/ALiBi.py
+-rw-r--r--   0        0        0     1677 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/RotaryEmbedding.py
+-rw-r--r--   0        0        0    15836 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/Transformer.py
+-rw-r--r--   0        0        0      164 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/ffn.py
+-rw-r--r--   0        0        0     2000 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/functional.py
+-rw-r--r--   0        0        0      800 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/hnn_utils/nn/normalization.py
+-rw-r--r--   0        0        0      517 2024-05-04 21:17:25.080837 hnn_utils-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 hnn_utils-0.3.5/PKG-INFO
```

### Comparing `hnn_utils-0.3.4/LICENSE` & `hnn_utils-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/callbacks/ema.py` & `hnn_utils-0.3.5/hnn_utils/callbacks/ema.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/datasets/guacamol.py` & `hnn_utils-0.3.5/hnn_utils/datasets/guacamol.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/datasets/utils.py` & `hnn_utils-0.3.5/hnn_utils/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/datasets/vocab/guac.json` & `hnn_utils-0.3.5/hnn_utils/datasets/vocab/guac.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/datasets/vocab/guac_random.json` & `hnn_utils-0.3.5/hnn_utils/datasets/vocab/guac_random.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/datasets/vocab/zinc20.json` & `hnn_utils-0.3.5/hnn_utils/datasets/vocab/zinc20.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/datasets/zinc.py` & `hnn_utils-0.3.5/hnn_utils/datasets/zinc.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,89 +13,97 @@
 )
 
 DS_PATH = "haydn-jones/ZINC20"
 
 
 class ZINC20DataModule(L.LightningDataModule):
     def __init__(
-        self, batch_size: int, num_workers: int, randomize: Randomize = Randomize.NONE
+        self,
+        batch_size: int,
+        num_workers: int,
+        randomize: Randomize = Randomize.NONE,
+        seed: int = 42,
     ) -> None:
         super().__init__()
 
         self.batch_size = batch_size
         self.num_workers = num_workers
 
         self.vocab = json.load(
             pkg_resources.resource_stream(__name__, "vocab/zinc20.json")
         )
 
         self.randomize = randomize
+        self.seed = seed
 
     def prepare_data(self) -> None:
         datasets.load_dataset(DS_PATH, streaming=True, save_infos=True, split="train")
         datasets.load_dataset(DS_PATH, streaming=True, save_infos=True, split="val")
         datasets.load_dataset(DS_PATH, streaming=True, save_infos=True, split="test")
 
     def train_dataloader(self) -> DataLoader:
         ds = datasets.load_dataset(DS_PATH, streaming=True).select_columns("SELFIES")
-        ds = split_and_shuffle(ds, "train", self.trainer)
+        ds = split_and_shuffle(ds, "train", self.trainer, seed=self.seed)
 
         transform = build_transform(self.vocab, self.randomize)
 
         return DataLoader(
             ds,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=True,
             collate_fn=transform,
         )
 
     def val_dataloader(self) -> DataLoader:
         ds = datasets.load_dataset(DS_PATH, streaming=True).select_columns("SELFIES")
-        ds = split_and_shuffle(ds, "val", self.trainer)
+        ds = split_and_shuffle(ds, "val", self.trainer, seed=self.seed)
 
         transform = build_transform(self.vocab, self.randomize)
 
         return DataLoader(
             ds,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=True,
             collate_fn=transform,
         )
 
     def test_dataloader(self) -> DataLoader:
         ds = datasets.load_dataset(DS_PATH, streaming=True).select_columns("SELFIES")
-        ds = split_and_shuffle(ds, "test", self.trainer)
+        ds = split_and_shuffle(ds, "test", self.trainer, seed=self.seed)
 
         transform = build_transform(self.vocab, self.randomize)
 
         return DataLoader(
             ds,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
             pin_memory=True,
             collate_fn=transform,
         )
 
 
 def split_and_shuffle(
-    dataset: datasets.IterableDataset, split: str, trainer: Optional[L.Trainer]
+    dataset: datasets.IterableDataset,
+    split: str,
+    trainer: Optional[L.Trainer],
+    seed: int = 42,
 ) -> datasets.Dataset:
     dataset = dataset[split]
 
     # Split according to distributed setup
     if trainer is not None:
         dataset = split_dataset_by_node(
             dataset, rank=trainer.global_rank, world_size=trainer.world_size
         )
 
     # Shuffling an iterable dataset shuffles the *shards* and
     # creates a buffer of size `buffer_size` (in elements, not bytes)
     # which it randomly samples from. Larger buffer_size
     # means more memory usage but better shuffling.
-    dataset = dataset.shuffle(buffer_size=16384)
+    dataset = dataset.shuffle(buffer_size=16384, seed=seed)
 
     return dataset
```

### Comparing `hnn_utils-0.3.4/hnn_utils/nn/ALiBi.py` & `hnn_utils-0.3.5/hnn_utils/nn/ALiBi.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/nn/RotaryEmbedding.py` & `hnn_utils-0.3.5/hnn_utils/nn/RotaryEmbedding.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/nn/Transformer.py` & `hnn_utils-0.3.5/hnn_utils/nn/Transformer.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/nn/ffn.py` & `hnn_utils-0.3.5/hnn_utils/nn/ffn.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/nn/functional.py` & `hnn_utils-0.3.5/hnn_utils/nn/functional.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/hnn_utils/nn/normalization.py` & `hnn_utils-0.3.5/hnn_utils/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.4/pyproject.toml` & `hnn_utils-0.3.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hnn_utils"
-version = "0.3.4"
+version = "0.3.5"
 description = "Various utilities used throughout my research"
 authors = ["Haydn Jones <haydnjonest@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "hnn_utils" }]
 
 include = ["hnn_utils/datasets/vocab/*.json"]
```

### Comparing `hnn_utils-0.3.4/PKG-INFO` & `hnn_utils-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnn_utils
-Version: 0.3.4
+Version: 0.3.5
 Summary: Various utilities used throughout my research
 Author: Haydn Jones
 Author-email: haydnjonest@gmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

