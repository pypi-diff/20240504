# Comparing `tmp/tiny_dag-0.0.8.tar.gz` & `tmp/tiny_dag-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_dag-0.0.8.tar", last modified: Wed May  1 10:19:54 2024, max compression
+gzip compressed data, was "tiny_dag-0.0.9.tar", last modified: Wed May  1 11:57:24 2024, max compression
```

## Comparing `tiny_dag-0.0.8.tar` & `tiny_dag-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.8/LICENSE
--rw-r--r--   0 ossi      (1000) ossi      (1000)     2683 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     2145 2024-05-01 10:18:21.000000 tiny_dag-0.0.8/README.md
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.8/pyproject.toml
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/setup.cfg
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.051933 tiny_dag-0.0.8/src/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/src/tiny_dag.egg-info/
--rw-r--r--   0 ossi      (1000) ossi      (1000)     2683 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      312 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/SOURCES.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/dependency_links.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/requires.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/top_level.txt
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/src/tinydag/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.8/src/tinydag/__init__.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      147 2024-05-01 10:15:23.000000 tiny_dag-0.0.8/src/tinydag/exceptions.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     9709 2024-05-01 10:15:23.000000 tiny_dag-0.0.8/src/tinydag/graph.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1522 2024-05-01 10:15:23.000000 tiny_dag-0.0.8/src/tinydag/node.py
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 11:57:24.804042 tiny_dag-0.0.9/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.9/LICENSE
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     2715 2024-05-01 11:57:24.804042 tiny_dag-0.0.9/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     2177 2024-05-01 11:38:17.000000 tiny_dag-0.0.9/README.md
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.9/pyproject.toml
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-05-01 11:57:24.804042 tiny_dag-0.0.9/setup.cfg
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 11:57:24.800042 tiny_dag-0.0.9/src/
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 11:57:24.800042 tiny_dag-0.0.9/src/tiny_dag.egg-info/
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     2715 2024-05-01 11:57:24.000000 tiny_dag-0.0.9/src/tiny_dag.egg-info/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      333 2024-05-01 11:57:24.000000 tiny_dag-0.0.9/src/tiny_dag.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-05-01 11:57:24.000000 tiny_dag-0.0.9/src/tiny_dag.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-05-01 11:57:24.000000 tiny_dag-0.0.9/src/tiny_dag.egg-info/requires.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-05-01 11:57:24.000000 tiny_dag-0.0.9/src/tiny_dag.egg-info/top_level.txt
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 11:57:24.800042 tiny_dag-0.0.9/src/tinydag/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.9/src/tinydag/__init__.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      147 2024-05-01 10:15:23.000000 tiny_dag-0.0.9/src/tinydag/exceptions.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)    11481 2024-05-01 11:56:36.000000 tiny_dag-0.0.9/src/tinydag/graph.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1522 2024-05-01 10:15:23.000000 tiny_dag-0.0.9/src/tinydag/node.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      300 2024-05-01 11:43:13.000000 tiny_dag-0.0.9/src/tinydag/utils.py
```

### Comparing `tiny_dag-0.0.8/LICENSE` & `tiny_dag-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_dag-0.0.8/PKG-INFO` & `tiny_dag-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.8
+Version: 0.0.9
 Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: graphviz
 
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
 User provides a graph structure (nodes) and input data for graph. The graph executes every node in the graph and returns 
-output of every node as the result. The library supports multiple outputs.
+output of every node as the result. The library supports multiple outputs and caching of the node results.
 
 # Requirements
 
 - Python >= 3.6
 - graphviz (optional)
 
 # Installation
```

### Comparing `tiny_dag-0.0.8/README.md` & `tiny_dag-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
 User provides a graph structure (nodes) and input data for graph. The graph executes every node in the graph and returns 
-output of every node as the result. The library supports multiple outputs.
+output of every node as the result. The library supports multiple outputs and caching of the node results.
 
 # Requirements
 
 - Python >= 3.6
 - graphviz (optional)
 
 # Installation
```

### Comparing `tiny_dag-0.0.8/setup.cfg` & `tiny_dag-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiny-dag
-version = 0.0.8
+version = 0.0.9
 author = Ossi Myllymäki
 author_email = omyllymaki@gmail.com
 description = Minimal DAG implementation with Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/omyllymaki/tiny-dag
 project_urls =
```

### Comparing `tiny_dag-0.0.8/src/tiny_dag.egg-info/PKG-INFO` & `tiny_dag-0.0.9/src/tiny_dag.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.8
+Version: 0.0.9
 Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: graphviz
 
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
 User provides a graph structure (nodes) and input data for graph. The graph executes every node in the graph and returns 
-output of every node as the result. The library supports multiple outputs.
+output of every node as the result. The library supports multiple outputs and caching of the node results.
 
 # Requirements
 
 - Python >= 3.6
 - graphviz (optional)
 
 # Installation
```

### Comparing `tiny_dag-0.0.8/src/tinydag/graph.py` & `tiny_dag-0.0.9/src/tinydag/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
+import os
 import time
 from copy import copy
-from typing import List, Callable, Union, Optional, Any
+from os.path import join
+from typing import List, Callable, Union, Optional
 
 from tinydag.exceptions import InvalidGraphError, MissingInputError, InvalidNodeFunctionOutput
 from tinydag.node import Node
+from tinydag.utils import load_pickle, save_pickle
 
 logger = logging.getLogger(__name__)
 
 try:
     import graphviz as graphviz
     from graphviz import Digraph
 except ImportError:
@@ -44,36 +47,37 @@
     x, y -> add1
     x, z -> add_subtract
     add1/output, x -> add2
     add1/output, add2/output -> mul
     mul/output, add_subtract/add_output -> div
 
     User needs to provide x, y and z as input data for this graph when doing calculation.
+
+    Cache can be used to save and load cached results.
     """
 
     def __init__(self,
                  nodes: List[Node],
-                 wrappers: Optional[List[Callable]] = None) -> None:
+                 wrappers: Optional[List[Callable]] = None,
+                 cache_dir="cache") -> None:
         """
         :param nodes: List of nodes defining the graph.
         :param wrappers: Optional wrapper functions that will be used to wrap all the node functions.
+        :param cache_dir: Directory to save and read cached files.
         :raises InvalidGraphError if the node names are not unique.
         """
         self._check_node_names_are_unique(nodes)
         self.nodes = nodes
         self.wrappers = wrappers
         self.required_user_inputs = self._get_required_user_inputs()
         logger.debug(f"Required user input: {self.required_user_inputs}")
 
-    def _get_required_user_inputs(self) -> List[str]:
-        required_inputs, node_outputs = [], []
-        for node in self.nodes:
-            required_inputs += node.inputs
-            node_outputs += node.outputs
-        return list(set(required_inputs) - set(node_outputs))
+        if not os.path.exists(cache_dir):
+            os.makedirs(cache_dir)
+        self.cache_dir = cache_dir
 
     def render(self,
                path: str = "graph.gv",
                view: bool = True) -> Optional["Digraph"]:
         """
         Render graph. This will only work if graphviz is available.
         :param path: Path to save fig.
@@ -104,32 +108,76 @@
         """
         Check if the graph structure is valid.
         :raises InvalidGraphError if the graph structure is not valid.
         """
         input_data = {name: None for name in self.required_user_inputs}
         self._execute(input_data, False)
 
-    def calculate(self, input_data: Optional[dict] = None) -> dict:
+    def calculate(self,
+                  input_data: Optional[dict] = None,
+                  from_cache: Optional[List[str]] = None,
+                  to_cache: Optional[List[str]] = None) -> dict:
         """
         Execute every node in the graph.
         :param input_data: Input data for the graph, where keys are names used in the graph definition.
-        :return: Output of every node, with node names as keys.
+        :param from_cache: List of node names to read from cache.
+        :param to_cache: List of node names to save to cache.
+        :return: Output of every node, with node outputs as keys.
         :raises MissingInputError if the input_data doesn't contain all the required data.
         :raises InvalidGraphError if the graph structure is not valid.
+        :raises InvalidNodeFunctionOutput if the node function output is not valid.
+        :raises FileNotFoundError if cache file we want to read doesn't exist.
         """
         self._check_input_data(input_data)
-        return self._execute(input_data)
+        return self._execute(input_data, True, from_cache, to_cache)
+
+    def __add__(self, nodes: Union[List[Node], Node]) -> "Graph":
+        if isinstance(nodes, list):
+            nodes = self.nodes + nodes
+        else:
+            nodes = self.nodes + [nodes]
+        return Graph(nodes, self.wrappers)
+
+    def __repr__(self) -> str:
+        repr_str = "\n"
+        for node in self.nodes:
+            name = node.name
+            repr_str += f"Node: {name}\n"
+            repr_str += "├─ Inputs:\n"
+            for input_node in node.inputs:
+                repr_str += f"│  ├─ {input_node}\n"
+            repr_str += "└─ Outputs:\n"
+            for output_node in node.outputs:
+                repr_str += f"   ├─ {output_node}\n"
+        return repr_str
 
     def _check_input_data(self, input_data):
         if len(self.required_user_inputs) > 0:
             for item in self.required_user_inputs:
                 if item not in input_data:
                     raise MissingInputError(f"Input data is missing {item}")
 
-    def _execute(self, input_data: Optional[dict] = None, run: Optional[bool] = True) -> dict:
+    def _get_required_user_inputs(self) -> List[str]:
+        required_inputs, node_outputs = [], []
+        for node in self.nodes:
+            required_inputs += node.inputs
+            node_outputs += node.outputs
+        return list(set(required_inputs) - set(node_outputs))
+
+    def _execute(self,
+                 input_data: Optional[dict] = None,
+                 run: Optional[bool] = True,
+                 from_cache=None,
+                 to_cache=None) -> dict:
+
+        if from_cache is None:
+            from_cache = []
+        if to_cache is None:
+            to_cache = []
+
         # Container where all the node inputs will be stored
         # This will be updated when the nodes are executed
         inputs = copy(input_data) if input_data is not None else {}
 
         nodes_to_execute = [i for i in range(len(self.nodes))]
         t_graph_start = time.time()
 
@@ -142,16 +190,15 @@
             for node_index in nodes_to_execute:
                 node = self.nodes[node_index]
                 logger.debug(f"Executing node {node}")
                 node_input_data = self._get_node_input_data(node, inputs)
                 if len(node_input_data) < len(node.inputs):
                     continue  # All the input data cannot be found for this node yet, so skip this node
                 if run:
-                    results = self._run_node(node, node_input_data)
-                    self._check_node_output(results, node)
+                    results = self._get_node_results(node, node_input_data, from_cache, to_cache)
                     if results is not None:
                         for key, val in results.items():
                             inputs[node.name + "/" + key] = val
                 else:
                     for output in node.outputs:
                         inputs[output] = None
                 nodes_executed.append(node_index)
@@ -165,65 +212,62 @@
             for node_index in nodes_executed:
                 nodes_to_execute.remove(node_index)
 
         logger.debug("All nodes executed successfully")
         t_graph_end = time.time()
         logger.debug(f"Graph execution took {1000 * (t_graph_end - t_graph_start): 0.2f} ms")
 
+        results = self._create_output(inputs)
+
+        return results
+
+    def _create_output(self, inputs: dict) -> dict:
         results = {}
         for node in self.nodes:
             for output in node.outputs:
                 results[output] = inputs[output]
+        return results
 
+    def _get_node_results(self, node: Node, node_input_data: list, from_cache: List[str], to_cache: List[str]) -> dict:
+        path = join(self.cache_dir, node.name)
+        if node.name in from_cache:
+            results = load_pickle(path)
+            logger.info(f"Node {node.name} results read from cache: {path}")
+        else:
+            results = self._run_node(node, node_input_data)
+        self._check_node_output(results, node)
+        if node.name in to_cache:
+            save_pickle(path, results)
+            logger.info(f"Node {node.name} results wrote to cache: {path}")
         return results
 
-    def _run_node(self, node: Node, data: list) -> Any:
+    def _run_node(self, node: Node, data: list) -> dict:
         func = self._wrap_node_func(node.function)
         t_node_start = time.time()
         output = func(*data)
         t_node_end = time.time()
         logger.debug(f"Node {node} execution took {1000 * (t_node_end - t_node_start): 0.3f} ms")
         return output
 
     @staticmethod
-    def _check_node_output(output, node):
+    def _check_node_output(output: dict, node: Node) -> None:
         if output is not None:
             if not isinstance(output, dict):
                 raise InvalidNodeFunctionOutput(f"Node {node.name} output is not a dict!")
         for item in node.outputs:
             item = item.replace(f"{node.name}/", "")
             if item not in output:
                 raise InvalidNodeFunctionOutput(f"Node {node.name} output doesn't contain required item {item}!")
 
-    def _wrap_node_func(self, func):
+    def _wrap_node_func(self, func: Callable) -> Callable:
         if self.wrappers is not None:
             for wrapper in self.wrappers:
                 func = wrapper(func)
         return func
 
-    def __add__(self, nodes: Union[List[Node], Node]) -> "Graph":
-        if isinstance(nodes, list):
-            nodes = self.nodes + nodes
-        else:
-            nodes = self.nodes + [nodes]
-        return Graph(nodes, self.wrappers)
-
-    def __repr__(self) -> str:
-        repr_str = "\n"
-        for node in self.nodes:
-            name = node.name
-            repr_str += f"Node: {name}\n"
-            repr_str += "├─ Inputs:\n"
-            for input_node in node.inputs:
-                repr_str += f"│  ├─ {input_node}\n"
-            repr_str += "└─ Outputs:\n"
-            for output_node in node.outputs:
-                repr_str += f"   ├─ {output_node}\n"
-        return repr_str
-
     @staticmethod
     def _check_node_names_are_unique(nodes: List[Node]) -> None:
         node_names = [n.name for n in nodes]
         if len(set(node_names)) < len(node_names):
             raise InvalidGraphError("All the nodes need to have unique name!")
 
     @staticmethod
```

### Comparing `tiny_dag-0.0.8/src/tinydag/node.py` & `tiny_dag-0.0.9/src/tinydag/node.py`

 * *Files identical despite different names*

