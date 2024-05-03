# Comparing `tmp/nnfasta-0.1.8.tar.gz` & `tmp/nnfasta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.8.tar", max compression
+gzip compressed data, was "nnfasta-0.1.9.tar", max compression
```

## Comparing `nnfasta-0.1.8.tar` & `nnfasta-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.8/LICENSE
--rw-r--r--   0        0        0     1130 2024-05-03 09:34:14.166752 nnfasta-0.1.8/README.md
--rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.8/nnfasta/__init__.py
--rw-r--r--   0        0        0     5280 2024-05-03 09:23:50.781826 nnfasta-0.1.8/nnfasta/fasta.py
--rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.8/nnfasta/py.typed
--rw-r--r--   0        0        0      368 2024-05-03 09:34:42.490978 nnfasta-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 nnfasta-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1578 2024-05-03 22:50:58.632362 nnfasta-0.1.9/README.md
+-rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.9/nnfasta/__init__.py
+-rw-r--r--   0        0        0     6372 2024-05-03 22:55:18.949465 nnfasta-0.1.9/nnfasta/fasta.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.9/nnfasta/py.typed
+-rw-r--r--   0        0        0      368 2024-05-03 22:56:23.917756 nnfasta-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2153 1970-01-01 00:00:00.000000 nnfasta-0.1.9/PKG-INFO
```

### Comparing `nnfasta-0.1.8/LICENSE` & `nnfasta-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.8/README.md` & `nnfasta-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```
 
 **There are no dependencies.**
 
 ## Usage
 
 ```python
-from nnfasta import nnfastas 
+from nnfasta import nnfastas
 
 dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
 
 # display the number of sequences
 print(len(dataset))
 
 # get a particular record
@@ -50,8 +50,26 @@
     seq: str
     """Sequence stripped of whitespace and uppercased"""
 
     @property
     def name(self) -> str:
         return self.id
 ```
+
+## Test and Train Split best practice
+
+Use `LazyFasta`
+
+```python
+from nnfasta import nnfasta, LazyFasta
+from sklearn.model_selection import train_test_split
+
+dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
+train_idx, val_idx = train_test_split(range(len(dataset)),test_size=.1,shuffle=True)
+
+# these are still Sequence[Record] objects.
+train_data = LazyFasta(datset, train_idx)
+test_data = LazyFasta(datset, test_idx)
+
+```
+
 Enjoy peps!
```

### Comparing `nnfasta-0.1.8/nnfasta/fasta.py` & `nnfasta-0.1.9/nnfasta/fasta.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dataclasses import dataclass
 from typing import Iterator, overload
 
 
 @dataclass
 class Record:
     """Mimics biopython Record"""
+
     id: str
     """Sequence ID"""
     description: str
     """Line prefixed by '>'"""
     seq: str
     """Sequence stripped of whitespace and uppercased"""
 
@@ -170,7 +171,37 @@
         if isinstance(idx, int):
             return self.get_idx(idx)
         if isinstance(idx, list):
             return [self.get_idx(i) for i in idx]
         return list(
             self.get_idxs(range(idx.start, idx.stop or len(self), idx.step or 1))
         )
+
+
+class LazyFasta(Sequence[Record]):
+    """Return sequence records from a list of indicies"""
+
+    def __init__(self, dataset: Sequence[Record], indexes: Sequence[int]):
+        """Use index to create a new dataset from another"""
+        self._dataset = dataset
+        self._indexes = indexes
+        assert len(dataset) > max(self._indexes) and min(self._indexes) >= 0
+
+    def __len__(self) -> int:
+        return len(self._indexes)
+
+    @overload
+    def __getitem__(self, idx: int) -> Record: ...
+    @overload
+    def __getitem__(self, idx: slice) -> list[Record]: ...
+    @overload
+    def __getitem__(self, idx: list[int]) -> list[Record]: ...
+    def __getitem__(self, idx: int | slice | list[int]) -> Record | list[Record]:  # type: ignore
+        index = self._indexes
+        if isinstance(idx, int):
+            return self._dataset[index[idx]]
+        if isinstance(idx, list):
+            return [self._dataset[index[i]] for i in idx]
+        return [
+            self._dataset[index[i]]
+            for i in range(idx.start, idx.stop or len(self), idx.step or 1)
+        ]
```

### Comparing `nnfasta-0.1.8/PKG-INFO` & `nnfasta-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnfasta
-Version: 0.1.8
+Version: 0.1.9
 Summary: Neural Net efficient Fasta
 License: MIT
 Author: arabidopsis
 Author-email: ian.castleden@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 ```
 
 **There are no dependencies.**
 
 ## Usage
 
 ```python
-from nnfasta import nnfastas 
+from nnfasta import nnfastas
 
 dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
 
 # display the number of sequences
 print(len(dataset))
 
 # get a particular record
@@ -67,9 +67,27 @@
     seq: str
     """Sequence stripped of whitespace and uppercased"""
 
     @property
     def name(self) -> str:
         return self.id
 ```
+
+## Test and Train Split best practice
+
+Use `LazyFasta`
+
+```python
+from nnfasta import nnfasta, LazyFasta
+from sklearn.model_selection import train_test_split
+
+dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
+train_idx, val_idx = train_test_split(range(len(dataset)),test_size=.1,shuffle=True)
+
+# these are still Sequence[Record] objects.
+train_data = LazyFasta(datset, train_idx)
+test_data = LazyFasta(datset, test_idx)
+
+```
+
 Enjoy peps!
```

