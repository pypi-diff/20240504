# Comparing `tmp/nnfasta-0.1.7.tar.gz` & `tmp/nnfasta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnfasta-0.1.7.tar", max compression
+gzip compressed data, was "nnfasta-0.1.8.tar", max compression
```

## Comparing `nnfasta-0.1.7.tar` & `nnfasta-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.7/LICENSE
--rw-r--r--   0        0        0     1118 2024-05-03 06:04:14.677648 nnfasta-0.1.7/README.md
--rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.7/nnfasta/__init__.py
--rw-r--r--   0        0        0     5094 2024-05-03 05:57:53.246317 nnfasta-0.1.7/nnfasta/fasta.py
--rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.7/nnfasta/py.typed
--rw-r--r--   0        0        0      368 2024-05-03 06:06:16.762719 nnfasta-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nnfasta-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-03 00:07:18.824495 nnfasta-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1130 2024-05-03 09:34:14.166752 nnfasta-0.1.8/README.md
+-rw-r--r--   0        0        0       70 2024-05-03 05:27:16.632116 nnfasta-0.1.8/nnfasta/__init__.py
+-rw-r--r--   0        0        0     5280 2024-05-03 09:23:50.781826 nnfasta-0.1.8/nnfasta/fasta.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:33:29.864485 nnfasta-0.1.8/nnfasta/py.typed
+-rw-r--r--   0        0        0      368 2024-05-03 09:34:42.490978 nnfasta-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 nnfasta-0.1.8/PKG-INFO
```

### Comparing `nnfasta-0.1.7/LICENSE` & `nnfasta-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nnfasta-0.1.7/README.md` & `nnfasta-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Install:
 
 ```bash
 pip install nnfasta
 ```
 
-There are **no** dependencies.
+**There are no dependencies.**
 
 ## Usage
 
 ```python
 from nnfasta import nnfastas 
 
 dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
@@ -50,7 +50,8 @@
     seq: str
     """Sequence stripped of whitespace and uppercased"""
 
     @property
     def name(self) -> str:
         return self.id
 ```
+Enjoy peps!
```

### Comparing `nnfasta-0.1.7/nnfasta/fasta.py` & `nnfasta-0.1.8/nnfasta/fasta.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 from typing import Iterator, overload
 
 
 @dataclass
 class Record:
+    """Mimics biopython Record"""
     id: str
     """Sequence ID"""
     description: str
     """Line prefixed by '>'"""
     seq: str
     """Sequence stripped of whitespace and uppercased"""
 
     @property
     def name(self) -> str:
+        """same as ID"""
         return self.id
 
 
 PREFIX = re.compile(b"(\n>|\r>|^>)", re.M)
 
 WHITE = re.compile(rb"\W+", re.I | re.M)
 EOL = re.compile(rb"\n|\r", re.I | re.M)
 
 
 def remove_white(s: bytes) -> bytes:
+    """remove whitespace from byte list"""
     return WHITE.sub(b"", s)
 
 
 def nnfastas(
     fasta_files: Sequence[os.PathLike | str], encoding: str | None = None
 ) -> Sequence[Record]:
     """Given a sequence of fasta files return an indexable (list like) Fasta object.
@@ -76,14 +79,15 @@
     def _find_pos(self) -> list[tuple[int, int]]:
         f = [(h.start(), h.end()) for h in PREFIX.finditer(self.fasta)]
         end, start = zip(*f)
         end = end[1:] + (len(self.fasta),)
         return list(zip(start, end))
 
     def get_idx(self, idx: int) -> Record:
+        """get Record for idx"""
         s, e = self.pos[idx]
         b = self.fasta[s:e]  # mmap go to disk
         m = EOL.search(b)
         if not m:
             raise ValueError(f"not a fasta file: {str(b)}")
         e = m.start()
         desc = b[0:e]
@@ -148,14 +152,15 @@
 
     def get_idx(self, idx: int) -> Record:
         """Given an integer ID return the Record"""
         i, rf = self._map_idx(idx)
         return rf.get_idx(i)
 
     def get_idxs(self, idxs: Sequence[int]) -> Iterator[Record]:
+        """get Records for sequence of integers"""
         for i, rf in self._map_idxs(idxs):
             yield rf.get_idx(i)
 
     @overload
     def __getitem__(self, idx: int) -> Record: ...
     @overload
     def __getitem__(self, idx: slice) -> list[Record]: ...
```

### Comparing `nnfasta-0.1.7/PKG-INFO` & `nnfasta-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnfasta
-Version: 0.1.7
+Version: 0.1.8
 Summary: Neural Net efficient Fasta
 License: MIT
 Author: arabidopsis
 Author-email: ian.castleden@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 Install:
 
 ```bash
 pip install nnfasta
 ```
 
-There are **no** dependencies.
+**There are no dependencies.**
 
 ## Usage
 
 ```python
 from nnfasta import nnfastas 
 
 dataset = nnfastas(['athaliana.fasta','triticum.fasta','zmays.fasta'])
@@ -67,8 +67,9 @@
     seq: str
     """Sequence stripped of whitespace and uppercased"""
 
     @property
     def name(self) -> str:
         return self.id
 ```
+Enjoy peps!
```

