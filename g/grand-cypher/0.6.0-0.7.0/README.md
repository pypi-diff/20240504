# Comparing `tmp/grand-cypher-0.6.0.tar.gz` & `tmp/grand-cypher-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grand-cypher-0.6.0.tar", last modified: Mon Feb 19 15:50:56 2024, max compression
+gzip compressed data, was "grand-cypher-0.7.0.tar", last modified: Sat May  4 14:00:17 2024, max compression
```

## Comparing `grand-cypher-0.6.0.tar` & `grand-cypher-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-02-19 15:50:56.766416 grand-cypher-0.6.0/
--rw-r--r--   0 mateljk1   (501) staff       (20)    10173 2024-02-13 16:24:47.000000 grand-cypher-0.6.0/LICENSE
--rw-r--r--   0 mateljk1   (501) staff       (20)     4360 2024-02-19 15:50:56.766276 grand-cypher-0.6.0/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)     3969 2024-02-13 16:27:18.000000 grand-cypher-0.6.0/README.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-02-19 15:50:56.764519 grand-cypher-0.6.0/grand_cypher.egg-info/
--rw-r--r--   0 mateljk1   (501) staff       (20)     4360 2024-02-19 15:50:56.000000 grand-cypher-0.6.0/grand_cypher.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)      284 2024-02-19 15:50:56.000000 grand-cypher-0.6.0/grand_cypher.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-02-19 15:50:56.000000 grand-cypher-0.6.0/grand_cypher.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       30 2024-02-19 15:50:56.000000 grand-cypher-0.6.0/grand_cypher.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       12 2024-02-19 15:50:56.000000 grand-cypher-0.6.0/grand_cypher.egg-info/top_level.txt
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-02-19 15:50:56.765400 grand-cypher-0.6.0/grandcypher/
--rw-r--r--   0 mateljk1   (501) staff       (20)    25998 2024-02-18 19:45:21.000000 grand-cypher-0.6.0/grandcypher/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)      531 2024-02-13 16:24:47.000000 grand-cypher-0.6.0/grandcypher/test_parser.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    33029 2024-02-18 19:45:21.000000 grand-cypher-0.6.0/grandcypher/test_queries.py
--rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-02-19 15:50:56.766487 grand-cypher-0.6.0/setup.cfg
--rw-r--r--   0 mateljk1   (501) staff       (20)      701 2024-02-18 19:45:21.000000 grand-cypher-0.6.0/setup.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-04 14:00:17.204058 grand-cypher-0.7.0/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10173 2024-02-13 16:24:47.000000 grand-cypher-0.7.0/LICENSE
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4516 2024-05-04 14:00:17.203883 grand-cypher-0.7.0/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4125 2024-05-04 13:52:54.000000 grand-cypher-0.7.0/README.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-04 14:00:17.202916 grand-cypher-0.7.0/grand_cypher.egg-info/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4516 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)      284 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       30 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       12 2024-05-04 14:00:17.000000 grand-cypher-0.7.0/grand_cypher.egg-info/top_level.txt
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-04 14:00:17.203561 grand-cypher-0.7.0/grandcypher/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    30112 2024-05-04 13:59:06.000000 grand-cypher-0.7.0/grandcypher/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      531 2024-02-13 16:24:47.000000 grand-cypher-0.7.0/grandcypher/test_parser.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    40941 2024-05-04 13:52:54.000000 grand-cypher-0.7.0/grandcypher/test_queries.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-05-04 14:00:17.204128 grand-cypher-0.7.0/setup.cfg
+-rw-r--r--   0 mateljk1   (501) staff       (20)      701 2024-05-04 13:59:22.000000 grand-cypher-0.7.0/setup.py
```

### Comparing `grand-cypher-0.6.0/LICENSE` & `grand-cypher-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grand-cypher-0.6.0/PKG-INFO` & `grand-cypher-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grand-cypher
-Version: 0.6.0
+Version: 0.7.0
 Summary: Query Grand graphs using Cypher
 Home-page: https://github.com/aplbrain/grandcypher
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -88,14 +88,16 @@
 | Anonymous `()` nodes                       | ✅ Thanks @khoale88! |     |
 | Undirected `()-[]-()` edges                | ✅ Thanks @khoale88! |     |
 | Boolean Arithmetic (`AND`/`OR`)            | ✅ Thanks @khoale88! |     |
 | `OPTIONAL MATCH`                           | 🛣                    |     |
 | `(:Type)` node-labels                      | ✅ Thanks @khoale88! |     |
 | `[:Type]` edge-labels                      | ✅ Thanks @khoale88! |     |
 | Graph mutations (e.g. `DELETE`, `SET`,...) | 🛣                    |     |
+| `DISTINCT`                                 | ✅ Thanks @jackboyla! |     |
+| `ORDER BY`                                 | ✅ Thanks @jackboyla! |     |
 
 |                |                |                  |
 | -------------- | -------------- | ---------------- |
 | ✅ = Supported | 🛣 = On Roadmap | 🔴 = Not Planned |
 
 ## Citing
```

### Comparing `grand-cypher-0.6.0/README.md` & `grand-cypher-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 | Anonymous `()` nodes                       | ✅ Thanks @khoale88! |     |
 | Undirected `()-[]-()` edges                | ✅ Thanks @khoale88! |     |
 | Boolean Arithmetic (`AND`/`OR`)            | ✅ Thanks @khoale88! |     |
 | `OPTIONAL MATCH`                           | 🛣                    |     |
 | `(:Type)` node-labels                      | ✅ Thanks @khoale88! |     |
 | `[:Type]` edge-labels                      | ✅ Thanks @khoale88! |     |
 | Graph mutations (e.g. `DELETE`, `SET`,...) | 🛣                    |     |
+| `DISTINCT`                                 | ✅ Thanks @jackboyla! |     |
+| `ORDER BY`                                 | ✅ Thanks @jackboyla! |     |
 
 |                |                |                  |
 | -------------- | -------------- | ---------------- |
 | ✅ = Supported | 🛣 = On Roadmap | 🔴 = Not Planned |
 
 ## Citing
```

### Comparing `grand-cypher-0.6.0/grand_cypher.egg-info/PKG-INFO` & `grand-cypher-0.7.0/grand_cypher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grand-cypher
-Version: 0.6.0
+Version: 0.7.0
 Summary: Query Grand graphs using Cypher
 Home-page: https://github.com/aplbrain/grandcypher
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -88,14 +88,16 @@
 | Anonymous `()` nodes                       | ✅ Thanks @khoale88! |     |
 | Undirected `()-[]-()` edges                | ✅ Thanks @khoale88! |     |
 | Boolean Arithmetic (`AND`/`OR`)            | ✅ Thanks @khoale88! |     |
 | `OPTIONAL MATCH`                           | 🛣                    |     |
 | `(:Type)` node-labels                      | ✅ Thanks @khoale88! |     |
 | `[:Type]` edge-labels                      | ✅ Thanks @khoale88! |     |
 | Graph mutations (e.g. `DELETE`, `SET`,...) | 🛣                    |     |
+| `DISTINCT`                                 | ✅ Thanks @jackboyla! |     |
+| `ORDER BY`                                 | ✅ Thanks @jackboyla! |     |
 
 |                |                |                  |
 | -------------- | -------------- | ---------------- |
 | ✅ = Supported | 🛣 = On Roadmap | 🔴 = Not Planned |
 
 ## Citing
```

### Comparing `grand-cypher-0.6.0/grandcypher/__init__.py` & `grand-cypher-0.7.0/grandcypher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 You can use this tool to search Python graph data-structures by
 data/attribute or by structure, using the same language you'd use
 to search in a much larger graph database.
 
 """
 
 from typing import Dict, List, Callable, Tuple
+from collections import OrderedDict
 import random
 import string
 from functools import lru_cache
 import networkx as nx
 
 import grandiso
 
@@ -35,16 +36,16 @@
 }
 
 
 _GrandCypherGrammar = Lark(
     r"""
 start               : query
 
-query               : many_match_clause where_clause return_clause
-                    | many_match_clause return_clause
+query               : many_match_clause where_clause return_clause order_clause? skip_clause? limit_clause?
+                    | many_match_clause return_clause order_clause? skip_clause? limit_clause?
 
 
 many_match_clause   : (match_clause)+
 
 
 match_clause        : "match"i path_clause? node_match (edge_match node_match)*
 
@@ -76,22 +77,30 @@
                     | "in"i -> op_in
                     | "contains"i -> op_contains
                     | "starts with"i -> op_starts_with
                     | "ends with"i -> op_ends_with
 
 
 
-return_clause       : "return"i entity_id ("," entity_id)*
-                    | "return"i entity_id ("," entity_id)* limit_clause
-                    | "return"i entity_id ("," entity_id)* skip_clause
-                    | "return"i entity_id ("," entity_id)* skip_clause limit_clause
+return_clause       : "return"i distinct_return? entity_id ("," entity_id)*
 
+distinct_return     : "DISTINCT"i
 limit_clause        : "limit"i NUMBER
 skip_clause         : "skip"i NUMBER
 
+order_clause        : "order"i "by"i order_items
+
+order_items         : order_item ("," order_item)*
+
+order_item          : entity_id order_direction?
+
+order_direction     : "ASC"i -> asc
+                    | "DESC"i -> desc
+                    | -> no_direction
+
 
 ?entity_id          : CNAME
                     | CNAME "." CNAME
 
 node_match          : "(" (CNAME)? (json_dict)? ")"
                     | "(" (CNAME)? ":" TYPE (json_dict)? ")"
 
@@ -142,15 +151,15 @@
 COMMENT: "//" /[^\n]/*
 %ignore COMMENT
 
 """,
     start="start",
 )
 
-__version__ = "0.5.0"
+__version__ = "0.7.0"
 
 
 _ALPHABET = string.ascii_lowercase + string.digits
 
 
 def shortuuid(k=4) -> str:
     return "".join(random.choices(_ALPHABET, k=k))
@@ -315,14 +324,17 @@
         self._paths = []
         self._where_condition: CONDITION = None
         self._motif = nx.DiGraph()
         self._matches = None
         self._matche_paths = None
         self._return_requests = []
         self._return_edges = {}
+        self._distinct = False
+        self._order_by = None
+        self._order_by_attributes = set()
         self._limit = limit
         self._skip = 0
         self._max_hop = 100
 
     def _lookup(self, data_paths: List[str], offset_limit) -> Dict[str, List]:
         if not data_paths:
             return {}
@@ -387,37 +399,121 @@
                     # Get the correct entity from the target host graph,
                     # and then return the attribute:
                     ret = (r.get(entity_attribute, None) for r in ret)
 
             result[data_path] = list(ret)[offset_limit]
 
         return result
-
-    def return_clause(self, clause):
+    
+    def return_clause(self, clause):        
+        # collect all entity identifiers to be returned
         for item in clause:
             if item:
                 if not isinstance(item, str):
                     item = str(item.value)
                 self._return_requests.append(item)
 
+
+    def order_clause(self, order_clause):
+        self._order_by = []
+        for item in order_clause[0].children:
+            field = str(item.children[0])  # assuming the field name is the first child
+            # Default to 'ASC' if not specified
+            if len(item.children) > 1 and str(item.children[1].data).lower() != 'desc':
+                direction = 'ASC'
+            else:
+                direction = 'DESC'
+            
+            self._order_by.append((field, direction))   # [('n.age', 'DESC'), ...]
+            self._order_by_attributes.add(field)
+
+    def distinct_return(self, distinct):
+        self._distinct = True
+
     def limit_clause(self, limit):
         limit = int(limit[-1])
         self._limit = limit
 
     def skip_clause(self, skip):
         skip = int(skip[-1])
         self._skip = skip
 
     def returns(self, ignore_limit=False):
-        if self._limit and ignore_limit is False:
-            offset_limit = slice(self._skip, self._skip + self._limit)
-        else:
-            offset_limit = slice(self._skip, None)
 
-        return self._lookup(self._return_requests, offset_limit=offset_limit)
+        results = self._lookup(
+            self._return_requests + list(self._order_by_attributes), 
+            offset_limit=slice(0, None)
+        )
+        if self._order_by:
+            results = self._apply_order_by(results)
+        if self._distinct:
+            results = self._apply_distinct(results)
+        results = self._apply_pagination(results, ignore_limit)
+
+
+        # Exclude order-by-only attributes from the final results
+        results = {
+            key: values for key, values in results.items() if key in self._return_requests
+        }
+
+        return results
+    
+    def _apply_order_by(self, results):
+        if self._order_by:
+            sort_lists = [(results[field], direction) for field, direction in self._order_by if field in results]
+
+            if sort_lists:
+                # Generate a list of indices sorted by the specified fields
+                indices = range(len(next(iter(results.values()))))  # Safe because all lists are assumed to be of the same length
+                for sort_list, direction in reversed(sort_lists):  # reverse to ensure the first sort key is primary
+                    indices = sorted(indices, key=lambda i: sort_list[i], reverse=(direction == 'DESC'))
+
+                # Reorder all lists in results using sorted indices
+                for key in results:
+                    results[key] = [results[key][i] for i in indices]
+        
+        return results
+    
+    def _apply_distinct(self, results):
+        if self._order_by:
+            assert self._order_by_attributes.issubset(self._return_requests), "In a WITH/RETURN with DISTINCT or an aggregation, it is not possible to access variables declared before the WITH/RETURN"
+
+        # ordered dict to maintain the first occurrence of each unique tuple based on return requests
+        unique_rows = OrderedDict()
+        
+        # Iterate over each 'row' by index
+        for i in range(len(next(iter(results.values())))):  # assume all columns are of the same length
+            # create a tuple key of all the values from return requests for this row
+            row_key = tuple(results[key][i] for key in self._return_requests if key in results)
+            
+            if row_key not in unique_rows:
+                unique_rows[row_key] = i  # store the index of the first occurrence of this unique row
+        
+        # construct the results based on unique indices collected
+        distinct_results = {key: [] for key in self._return_requests}
+        for row_key, index in unique_rows.items():
+            for _, key in enumerate(self._return_requests):
+                distinct_results[key].append(results[key][index])
+        
+        return distinct_results
+    
+    def _apply_pagination(self, results, ignore_limit):
+        # apply LIMIT and SKIP (if set) after ordering
+        if self._limit is not None and not ignore_limit:
+            start_index = self._skip
+            end_index = start_index + self._limit
+            for key in results.keys():
+                results[key] = results[key][start_index:end_index]
+        # else just apply SKIP (if set)
+        else:
+            for key in results.keys():
+                start_index = self._skip
+                results[key] = results[key][start_index:]
+        
+        return results
 
     def _get_true_matches(self):
         if not self._matches:
             self_matches = []
             self_matche_paths = []
             complete = False
 
@@ -450,16 +546,16 @@
                         # Check if match matches where condition and add
                         if not self._where_condition or self._where_condition(
                             match, self._target_graph, self._return_edges
                         ):
                             self_matches.append(match)
                             self_matche_paths.append(edge_hop_map)
 
-                            # Check if limit reached
-                            if self._is_limit(len(self_matches)):
+                            # Check if limit reached; stop ONLY IF we are not ordering
+                            if self._is_limit(len(self_matches)) and not self._order_by:
                                 complete = True
                                 break
 
             self._matches = self_matches
             self._matche_paths = self_matche_paths
 
         return list(zip(self._matches, self._matche_paths))
```

### Comparing `grand-cypher-0.6.0/grandcypher/test_parser.py` & `grand-cypher-0.7.0/grandcypher/test_parser.py`

 * *Files identical despite different names*

### Comparing `grand-cypher-0.6.0/grandcypher/test_queries.py` & `grand-cypher-0.7.0/grandcypher/test_queries.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import networkx as nx
+import pytest
 
 from . import _GrandCypherGrammar, _GrandCypherTransformer, GrandCypher
 
 
 class TestWorking:
     def test_simple_structural_match(self):
         tree = _GrandCypherGrammar.parse(
@@ -584,14 +585,250 @@
         """
         res = GrandCypher(host).run(qry)
         assert len(res) == 2
         assert res["A"] == ["x", "y"]
         assert res["B"] == ["y", "z"]
 
 
+class TestDistinct:
+    def test_basic_distinct1(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice")
+        host.add_node("b", name="Bob")
+        host.add_node("c", name="Alice")  # duplicate name
+
+        qry = """
+        MATCH (n)
+        RETURN DISTINCT n.name
+        """
+        res = GrandCypher(host).run(qry)
+        assert len(res["n.name"]) == 2  # should return "Alice" and "Bob" only once
+        assert "Alice" in res["n.name"] and "Bob" in res["n.name"]
+
+    def test_basic_distinct2(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=25)
+        host.add_node("c", name="Carol", age=21)
+        host.add_node("d", name="Alice", age=25)
+        host.add_node("e", name="Greg", age=32)
+
+        qry = """
+        MATCH (n)
+        RETURN DISTINCT n.name
+        """
+        res = GrandCypher(host).run(qry)
+        assert len(res["n.name"]) == 4  # should return "Alice" and "Bob" only once
+        assert "Alice" in res["n.name"] and "Bob" in res["n.name"] and "Carol" in res["n.name"] and "Greg" in res["n.name"]
+
+
+    def test_distinct_with_relationships(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice")
+        host.add_node("b", name="Bob")
+        host.add_node("c", name="Alice")  # duplicate name
+        host.add_edge("a", "b")
+        host.add_edge("c", "b")
+
+        qry = """
+        MATCH (n)-[]->(b)
+        RETURN DISTINCT n.name
+        """
+        res = GrandCypher(host).run(qry)
+        assert len(res["n.name"]) == 1  # should return "Alice" only once
+        assert res["n.name"] == ["Alice"]
+
+
+    def test_distinct_with_limit_and_skip(self):
+        host = nx.DiGraph()
+        for i in range(5):
+            host.add_node(f"a{i}", name="Alice")
+            host.add_node(f"b{i}", name="Bob")
+
+        qry = """
+        MATCH (n)
+        RETURN DISTINCT n.name SKIP 1 LIMIT 1
+        """
+        res = GrandCypher(host).run(qry)
+        assert len(res["n.name"]) == 1  # only one name should be returned
+        assert res["n.name"] == ["Bob"]  # assuming alphabetical order
+
+
+    def test_distinct_on_complex_graph(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice")
+        host.add_node("b", name="Bob")
+        host.add_node("c", name="Carol")
+        host.add_node("d", name="Alice")  # duplicate name
+        host.add_edge("a", "b")
+        host.add_edge("b", "c")
+        host.add_edge("c", "d")
+
+        qry = """
+        MATCH (n)-[]->(m)
+        RETURN DISTINCT n.name, m.name
+        """
+        res = GrandCypher(host).run(qry)
+        assert len(res["n.name"]) == 3  # should account for paths without considering duplicate names
+        assert "Alice" in res["n.name"] and "Bob" in res["n.name"] and "Carol" in res["n.name"]
+        assert len(res["m.name"]) == 3  # should account for paths without considering duplicate names
+
+    def test_distinct_with_attributes(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Alice", age=30)  # same name, different attribute
+        host.add_node("c", name="Bob", age=25)
+
+        qry = """
+        MATCH (n)
+        WHERE n.age > 20
+        RETURN DISTINCT n.name
+        """
+        res = GrandCypher(host).run(qry)
+        assert len(res["n.name"]) == 2  # "Alice" and "Bob" should be distinct
+        assert "Alice" in res["n.name"] and "Bob" in res["n.name"]
+
+
+class TestOrderBy:
+    def test_order_by_single_field_ascending(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=20)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name 
+        ORDER BY n.age ASC
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ["Carol", "Alice", "Bob"]
+
+    def test_order_by_single_field_descending(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=20)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name 
+        ORDER BY n.age DESC
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ["Bob", "Alice", "Carol"]
+
+    def test_order_by_single_field_no_direction_provided(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=20)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name 
+        ORDER BY n.age
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ["Carol", "Alice", "Bob"]
+
+    def test_order_by_multiple_fields(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=25)
+        host.add_node("d", name="Dave", age=25)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name 
+        ORDER BY n.age ASC, n.name DESC
+        """
+        res = GrandCypher(host).run(qry)
+        # names sorted in descending order where ages are the same
+        assert res["n.name"] == ["Dave", "Carol", "Alice", "Bob"]
+
+    def test_order_by_with_limit(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=20)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name 
+        ORDER BY n.age ASC LIMIT 2
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ["Carol", "Alice"]
+
+    def test_order_by_with_skip(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=20)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name 
+        ORDER BY n.age ASC SKIP 1
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ["Alice", "Bob"]
+
+    def test_order_by_with_distinct(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=25)
+        host.add_node("d", name="Alice", age=25)
+        host.add_node("e", name="Greg", age=32)
+
+        qry = """
+        MATCH (n)
+        RETURN DISTINCT n.name, n.age
+        ORDER BY n.age DESC
+        """
+        res = GrandCypher(host).run(qry)
+        # Distinct names, ordered by age where available
+        assert res["n.name"] == ['Greg', 'Bob', 'Alice', 'Carol']
+        assert res["n.age"] == [32, 30, 25, 25]
+
+    def test_error_on_order_by_with_distinct_and_non_returned_field(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=25)
+        host.add_node("d", name="Alice", age=25)
+        host.add_node("e", name="Greg", age=32)
+
+        qry = """
+        MATCH (n)
+        RETURN DISTINCT n.name
+        ORDER BY n.age DESC
+        """
+        # Expect an error since 'n.age' is not included in the RETURN clause but used in ORDER BY
+        with pytest.raises(Exception):
+            res = GrandCypher(host).run(qry)
+
+    def test_order_by_with_non_returned_field(self):
+        host = nx.DiGraph()
+        host.add_node("a", name="Alice", age=25)
+        host.add_node("b", name="Bob", age=30)
+        host.add_node("c", name="Carol", age=20)
+
+        qry = """
+        MATCH (n)
+        RETURN n.name ORDER BY n.age ASC
+        """
+        res = GrandCypher(host).run(qry)
+        assert res["n.name"] == ["Carol", "Alice", "Bob"]
+
+
 class TestVariableLengthRelationship:
     def test_single_variable_length_relationship(self):
         host = nx.DiGraph()
         host.add_node("x", foo=12)
         host.add_node("y", foo=13)
         host.add_node("z", foo=16)
         host.add_edge("x", "y", bar="1")
```

### Comparing `grand-cypher-0.6.0/setup.py` & `grand-cypher-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="grand-cypher",
-    version="0.6.0",
+    version="0.7.0",
     author="Jordan Matelsky",
     author_email="opensource@matelsky.com",
     description="Query Grand graphs using Cypher",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aplbrain/grandcypher",
     packages=setuptools.find_packages(),
```

