# Comparing `tmp/searcharray-0.0.8.tar.gz` & `tmp/searcharray-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searcharray-0.0.8.tar", last modified: Wed Nov 22 02:14:26 2023, max compression
+gzip compressed data, was "searcharray-0.0.9.tar", last modified: Wed Nov 22 15:20:15 2023, max compression
```

## Comparing `searcharray-0.0.8.tar` & `searcharray-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 02:14:26.480872 searcharray-0.0.8/
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)    11307 2023-11-22 02:14:26.480739 searcharray-0.0.8/PKG-INFO
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)    10151 2023-11-21 23:01:56.000000 searcharray-0.0.8/README.md
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)      230 2023-11-13 14:13:22.000000 searcharray-0.0.8/pyproject.toml
-drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 02:14:26.476784 searcharray-0.0.8/searcharray/
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)        0 2023-11-13 14:18:52.000000 searcharray-0.0.8/searcharray/__init__.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)    32170 2023-11-22 02:09:07.000000 searcharray-0.0.8/searcharray/postings.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)      136 2023-11-18 14:29:51.000000 searcharray-0.0.8/searcharray/stemmers.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)     1193 2023-11-13 14:13:22.000000 searcharray-0.0.8/searcharray/term_dict.py
-drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 02:14:26.480293 searcharray-0.0.8/searcharray.egg-info/
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)    11307 2023-11-22 02:14:26.000000 searcharray-0.0.8/searcharray.egg-info/PKG-INFO
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)      467 2023-11-22 02:14:26.000000 searcharray-0.0.8/searcharray.egg-info/SOURCES.txt
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)        1 2023-11-22 02:14:26.000000 searcharray-0.0.8/searcharray.egg-info/dependency_links.txt
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)       39 2023-11-22 02:14:26.000000 searcharray-0.0.8/searcharray.egg-info/entry_points.txt
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)       66 2023-11-22 02:14:26.000000 searcharray-0.0.8/searcharray.egg-info/requires.txt
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)       12 2023-11-22 02:14:26.000000 searcharray-0.0.8/searcharray.egg-info/top_level.txt
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)       78 2023-11-22 02:14:26.481120 searcharray-0.0.8/setup.cfg
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)     7631 2023-11-22 02:11:39.000000 searcharray-0.0.8/setup.py
-drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 02:14:26.479590 searcharray-0.0.8/test/
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)     4494 2023-11-17 13:07:58.000000 searcharray-0.0.8/test/test_extension_array.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)     3291 2023-11-22 02:09:22.000000 searcharray-0.0.8/test/test_msmarco.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)     7445 2023-11-22 01:30:49.000000 searcharray-0.0.8/test/test_phrase_matches.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)     2526 2023-11-17 12:13:29.000000 searcharray-0.0.8/test/test_tmdb.py
--rw-r--r--   0 douglas.turnbull   (503) staff       (20)      383 2023-11-12 23:40:54.000000 searcharray-0.0.8/test/test_utils.py
+drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 15:20:15.210939 searcharray-0.0.9/
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)    11307 2023-11-22 15:20:15.210671 searcharray-0.0.9/PKG-INFO
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)    10151 2023-11-21 23:01:56.000000 searcharray-0.0.9/README.md
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)      230 2023-11-13 14:13:22.000000 searcharray-0.0.9/pyproject.toml
+drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 15:20:15.206246 searcharray-0.0.9/searcharray/
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)        0 2023-11-13 14:18:52.000000 searcharray-0.0.9/searcharray/__init__.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)    33954 2023-11-22 15:14:45.000000 searcharray-0.0.9/searcharray/postings.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)      136 2023-11-18 14:29:51.000000 searcharray-0.0.9/searcharray/stemmers.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)     1193 2023-11-13 14:13:22.000000 searcharray-0.0.9/searcharray/term_dict.py
+drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 15:20:15.210224 searcharray-0.0.9/searcharray.egg-info/
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)    11307 2023-11-22 15:20:15.000000 searcharray-0.0.9/searcharray.egg-info/PKG-INFO
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)      467 2023-11-22 15:20:15.000000 searcharray-0.0.9/searcharray.egg-info/SOURCES.txt
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)        1 2023-11-22 15:20:15.000000 searcharray-0.0.9/searcharray.egg-info/dependency_links.txt
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)       39 2023-11-22 15:20:15.000000 searcharray-0.0.9/searcharray.egg-info/entry_points.txt
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)       66 2023-11-22 15:20:15.000000 searcharray-0.0.9/searcharray.egg-info/requires.txt
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)       12 2023-11-22 15:20:15.000000 searcharray-0.0.9/searcharray.egg-info/top_level.txt
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)       78 2023-11-22 15:20:15.211192 searcharray-0.0.9/setup.cfg
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)     7631 2023-11-22 15:18:44.000000 searcharray-0.0.9/setup.py
+drwxr-xr-x   0 douglas.turnbull   (503) staff       (20)        0 2023-11-22 15:20:15.209589 searcharray-0.0.9/test/
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)     4494 2023-11-17 13:07:58.000000 searcharray-0.0.9/test/test_extension_array.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)     3291 2023-11-22 15:15:31.000000 searcharray-0.0.9/test/test_msmarco.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)     8124 2023-11-22 15:11:15.000000 searcharray-0.0.9/test/test_phrase_matches.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)     2526 2023-11-17 12:13:29.000000 searcharray-0.0.9/test/test_tmdb.py
+-rw-r--r--   0 douglas.turnbull   (503) staff       (20)      383 2023-11-12 23:40:54.000000 searcharray-0.0.9/test/test_utils.py
```

### Comparing `searcharray-0.0.8/PKG-INFO` & `searcharray-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searcharray
-Version: 0.0.8
+Version: 0.0.9
 Summary: Searchable pandas text extension arrays for prototyping search
 Home-page: https://github.com/softwaredoug/searcharray
 Author: Doug Turnbull
 Author-email: softwaredoug@gmail.com
 Keywords: sample,setuptools,development search
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `searcharray-0.0.8/README.md` & `searcharray-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `searcharray-0.0.8/searcharray/postings.py` & `searcharray-0.0.9/searcharray/postings.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,27 @@
 # handler = logging.StreamHandler(sys.stdout)
 # handler.setLevel(logging.INFO)
 # formatter = logging.Formatter('%(message)s')
 # handler.setFormatter(formatter)
 # root.addHandler(handler)
 
 
+def vstack_with_pad(arrays, width=10, pad=-100):
+    vstacked = np.zeros((len(arrays), width), dtype=arrays[0].dtype) + pad
+    for idx, array in enumerate(arrays):
+        # Resize if needed, padding with pad
+        if len(array) > width:
+            logging.info(f"Resizing from {width} to {len(array)}")
+            vstack_padded = np.pad(vstacked, ((0, 0), (0, len(array) - width)), constant_values=pad)
+            width = len(array)
+            vstacked = vstack_padded
+        vstacked[idx, :len(array)] = array
+    return vstacked
+
+
 class PostingsRow:
     """Wrapper around a row of a postings matrix.
 
     We can't easily directly use a dictionary as a cell type in pandas.
     See:
 
     https://github.com/pandas-dev/pandas/issues/17777
@@ -738,38 +751,71 @@
         masks = [self.match(term) for term in tokens]
         mask = np.array([True] * len(self))
         for curr_mask in masks:
             mask = mask & curr_mask
         return mask
 
     def phrase_freq(self, tokens, slop=1):
+        from time import perf_counter
+        start = perf_counter()
+
+        mask = self.and_query(tokens)
+
+        if np.sum(mask) == 0:
+            return mask
+
+        # Any identical terms, default to shitty algo for now
+        if len(tokens) != len(set(tokens)):
+            return self.phrase_freq_shitty(tokens, slop=slop)
+
+        # Iterate each phrase with its next term
+        prior_term = tokens[0]
+        prior_posns = self.positions(prior_term, mask)
+        phrase_freqs = np.zeros(len(self))
+        for term in tokens[1:]:
+            term_posns = self.positions(term, mask)
+
+            assert len(prior_posns) == len(term_posns)
+            # RIPE for optimization -> vectorize in C
+            bigram_freqs = np.zeros(len(term_posns))
+            cont_posns = []
+            term_start = perf_counter()
+            for idx in range(len(term_posns)):
+                # Find insert position of every next term in prior term's positions
+                # Intuition:
+                # https://colab.research.google.com/drive/1EeqHYuCiqyptd-awS67Re78pqVdTfH4A
+                ins_posns = np.searchsorted(prior_posns[idx], term_posns[idx], side='right')
+                prior_adjacents = prior_posns[idx][ins_posns - 1]
+                adjacents = term_posns[idx] - prior_adjacents
+                bigram_freqs[idx] = np.sum(adjacents <= slop)
+
+                cont_indices = np.argwhere(adjacents <= slop).flatten()
+                cont_posn = term_posns[idx][cont_indices]
+                cont_posns.append(cont_posn)
+            phrase_freqs[mask] = bigram_freqs
+            prior_term = term
+            prior_posns = cont_posns
+            logging.info(f"Term Time: {perf_counter() - term_start:.4f}s")
+
+        logging.info(f"Phrase Search Time: {perf_counter() - start:.4f}s")
+
+        return phrase_freqs
+
+    def phrase_freq_shitty(self, tokens, slop=1):
         """Return number of occurences of a phrase."""
         from time import perf_counter
         # Start with docs with all terms
         start = perf_counter()
-        pad = -1000
         mask = self.and_query(tokens)
         # For detailed documentation of this algorithm, see this ChatGPT4 discussion
         # https://chat.openai.com/share/31affaad-dc91-4757-b31c-e85bdb5a0eb6
 
         if np.sum(mask) == 0:
             return mask
 
-        def vstack_with_pad(arrays, width=10):
-            vstacked = np.zeros((len(arrays), width), dtype=arrays[0].dtype) + pad
-            for idx, array in enumerate(arrays):
-                # Resize if needed, padding with pad
-                if len(array) > width:
-                    logging.info(f"Resizing from {width} to {len(array)}")
-                    vstack_padded = np.pad(vstacked, ((0, 0), (0, len(array) - width)), constant_values=pad)
-                    width = len(array)
-                    vstacked = vstack_padded
-                vstacked[idx, :len(array)] = array
-            return vstacked
-
         # Pad for easy difference computation
         term_posns = []
         for term in tokens:
             as_array = self.positions(term, mask)
             as_array_time = perf_counter() - start
             logging.info(f"Arr Posns 1: {as_array_time:.2f}s")
             term_posns.append(vstack_with_pad(as_array, 5))
```

### Comparing `searcharray-0.0.8/searcharray/term_dict.py` & `searcharray-0.0.9/searcharray/term_dict.py`

 * *Files identical despite different names*

### Comparing `searcharray-0.0.8/searcharray.egg-info/PKG-INFO` & `searcharray-0.0.9/searcharray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searcharray
-Version: 0.0.8
+Version: 0.0.9
 Summary: Searchable pandas text extension arrays for prototyping search
 Home-page: https://github.com/softwaredoug/searcharray
 Author: Doug Turnbull
 Author-email: softwaredoug@gmail.com
 Keywords: sample,setuptools,development search
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `searcharray-0.0.8/setup.py` & `searcharray-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="searcharray",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.8",  # Required
+    version="0.0.9",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Searchable pandas text extension arrays for prototyping search",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `searcharray-0.0.8/test/test_extension_array.py` & `searcharray-0.0.9/test/test_extension_array.py`

 * *Files identical despite different names*

### Comparing `searcharray-0.0.8/test/test_msmarco.py` & `searcharray-0.0.9/test/test_msmarco.py`

 * *Files identical despite different names*

### Comparing `searcharray-0.0.8/test/test_phrase_matches.py` & `searcharray-0.0.9/test/test_phrase_matches.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,40 @@
     "many_docs_large_term_dict": {
         "docs": lambda: PostingsArray.index(["foo bar bar baz", "data2", "data3 bar", "bunny funny wunny",
                                              " ".join(random_strings(1000, 4, 10)),
                                              "la ma ta wa ga ao a b c d e f g a be ae i foo bar foo bar"] * 100000),
         "phrase": ["foo", "bar"],
         "expected": [True, False, False, False, False, True] * 100000,
     },
+    "many_docs_and_positions": {
+        "docs": lambda: PostingsArray.index([" ".join(["foo bar bar baz foo foo bar foo"] * 100),
+                                             " ".join(["what is the foo bar doing in the bar foo?"] * 100)] * 100000),
+        "phrase": ["foo", "bar"],
+        "expected": [True, True] * 100000
+    }
+
 }
 
 
 scenarios = {
     "length_one": {
         "docs": lambda: PostingsArray.index(["foo bar bar baz", "data2", "data3 bar", "bunny funny wunny"] * 25),
         "phrase": ["foo"],
         "expected": [1, 0, 0, 0] * 25,
     },
     "base": {
         "docs": lambda: PostingsArray.index(["foo bar bar baz", "data2", "data3 bar", "bunny funny wunny"] * 25),
         "phrase": ["foo", "bar"],
         "expected": [1, 0, 0, 0] * 25,
     },
+    "term_repeats": {
+        "docs": lambda: PostingsArray.index(["foo foo bar bar baz", "data2", "data3 bar", "bunny funny wunny"] * 25),
+        "phrase": ["foo", "bar"],
+        "expected": [1, 0, 0, 0] * 25,
+    },
     "multi_term_one_doc": {
         "docs": lambda: PostingsArray.index(["foo bar bar bar foo", "data2", "data3 bar", "bunny funny wunny"] * 25),
         "phrase": ["foo", "bar"],
         "expected": [1, 0, 0, 0] * 25,
     },
     "three_terms_match": {
         "docs": lambda: PostingsArray.index(["foo bar baz baz", "data2", "data3 bar", "bunny funny wunny"] * 25),
@@ -146,26 +158,29 @@
     docs = docs()
     docs_before = docs.copy()
     term_freqs = docs.term_freq(phrase)
     expected_matches = np.array(expected) > 0
     matches = docs.match(phrase)
     assert (term_freqs == expected).all()
     assert (matches == expected_matches).all()
+    if len(phrase) > 1:
+        phrase_matches = docs.phrase_freq(phrase)
+        assert (expected == phrase_matches).all()
     assert (docs == docs_before).all(), "The phrase_match method should not modify the original array"
     bm25 = docs.bm25(phrase)
     assert (np.argsort(bm25) == np.argsort(expected)).all()
 
 
 @pytest.mark.skip
 @w_scenarios(perf_scenarios)
 def test_phrase_performance(docs, phrase, expected):
     start = perf_counter()
     docs = docs()
     matches = docs.match(phrase)
-    print(f"phrase_match took {perf_counter() - start} seconds | {len(docs)} docs")
+    print(f"phrase_match 1 took {perf_counter() - start} seconds | {len(docs)} docs")
     assert (matches == expected).all()
 
 
 def test_positions():
     data = PostingsArray.index(["foo bar bar baz", "data2", "data3 bar", "bunny funny wunny"] * 25)
     positions = data.positions("bar")
     for idx, posn in enumerate(positions):
```

### Comparing `searcharray-0.0.8/test/test_tmdb.py` & `searcharray-0.0.9/test/test_tmdb.py`

 * *Files identical despite different names*

