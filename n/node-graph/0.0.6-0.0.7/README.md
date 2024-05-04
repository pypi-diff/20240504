# Comparing `tmp/node_graph-0.0.6.tar.gz` & `tmp/node_graph-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node_graph-0.0.6.tar", last modified: Mon Apr 22 09:20:07 2024, max compression
+gzip compressed data, was "node_graph-0.0.7.tar", last modified: Sat May  4 08:37:54 2024, max compression
```

## Comparing `node_graph-0.0.6.tar` & `node_graph-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.6/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     1468 2024-04-22 09:20:07.867761 node_graph-0.0.6/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1027 2024-04-22 09:09:57.000000 node_graph-0.0.6/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/node_graph/
--rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/analysis.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13072 2024-04-22 09:09:57.000000 node_graph-0.0.6/node_graph/collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    10311 2024-04-22 09:19:56.000000 node_graph-0.0.6/node_graph/decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/link.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    18403 2024-04-22 09:09:57.000000 node_graph-0.0.6/node_graph/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/node_graph.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/node_graph/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/nodes/test_nodes.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/node_graph/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/properties/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3331 2024-04-22 09:09:57.000000 node_graph-0.0.6/node_graph/property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/serializer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.6/node_graph/socket.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/node_graph/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/sockets/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/sockets/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.6/node_graph/version.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/node_graph.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     1468 2024-04-22 09:20:07.000000 node_graph-0.0.6/node_graph.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-04-22 09:20:07.000000 node_graph-0.0.6/node_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-22 09:20:07.000000 node_graph-0.0.6/node_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-04-22 09:20:07.000000 node_graph-0.0.6/node_graph.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-04-22 09:20:07.000000 node_graph-0.0.6/node_graph.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-04-22 09:20:07.000000 node_graph-0.0.6/node_graph.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-22 09:20:07.867761 node_graph-0.0.6/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-04-22 09:19:56.000000 node_graph-0.0.6/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 09:20:07.867761 node_graph-0.0.6/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2231 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_entry_point.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.6/tests/test_hooks.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_socket.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.6/tests/test_yaml.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.311802 node_graph-0.0.7/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.7/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     1468 2024-05-04 08:37:54.311802 node_graph-0.0.7/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1027 2024-04-22 09:09:57.000000 node_graph-0.0.7/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/analysis.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13072 2024-04-26 12:04:23.000000 node_graph-0.0.7/node_graph/collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10339 2024-05-04 08:37:08.000000 node_graph-0.0.7/node_graph/decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/link.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    18403 2024-04-22 09:09:57.000000 node_graph-0.0.7/node_graph/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/node_graph.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/nodes/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/nodes/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/nodes/test_nodes.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/properties/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/properties/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/properties/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3331 2024-04-22 09:09:57.000000 node_graph-0.0.7/node_graph/property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/serializer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.7/node_graph/socket.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/sockets/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/sockets/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/version.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     1468 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-05-04 08:37:54.311802 node_graph-0.0.7/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-05-04 08:37:17.000000 node_graph-0.0.7/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2231 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_entry_point.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.7/tests/test_hooks.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_socket.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_yaml.py
```

### Comparing `node_graph-0.0.6/LICENSE` & `node_graph-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/PKG-INFO` & `node_graph-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `node_graph-0.0.6/README.md` & `node_graph-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/analysis.py` & `node_graph-0.0.7/node_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/collection.py` & `node_graph-0.0.7/node_graph/collection.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/decorator.py` & `node_graph-0.0.7/node_graph/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,21 @@
         if parameter.kind == inspect.Parameter.POSITIONAL_ONLY:
             if parameter.annotation is not inspect.Parameter.empty:
                 arg = [name, parameter.annotation]
             else:
                 arg = [name, None]
             args.append(arg)
         elif parameter.kind == inspect.Parameter.POSITIONAL_OR_KEYWORD:
-            kwargs[name] = {"type": parameter.annotation}
             if parameter.default is not inspect.Parameter.empty:
-                kwargs[name]["default"] = parameter.default
+                kwargs[name] = {
+                    "type": parameter.annotation,
+                    "default": parameter.default,
+                }
             else:
-                kwargs[name]["default"] = None
+                args.append([name, None])
         elif parameter.kind == inspect.Parameter.VAR_POSITIONAL:
             var_args = name
         elif parameter.kind == inspect.Parameter.VAR_KEYWORD:
             var_kwargs = name
 
     return args, kwargs, var_args, var_kwargs
```

### Comparing `node_graph-0.0.6/node_graph/link.py` & `node_graph-0.0.7/node_graph/link.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/node.py` & `node_graph-0.0.7/node_graph/node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/node_graph.py` & `node_graph-0.0.7/node_graph/node_graph.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/nodes/test_nodes.py` & `node_graph-0.0.7/node_graph/nodes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/properties/builtin.py` & `node_graph-0.0.7/node_graph/properties/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/property.py` & `node_graph-0.0.7/node_graph/property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/serializer.py` & `node_graph-0.0.7/node_graph/serializer.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/socket.py` & `node_graph-0.0.7/node_graph/socket.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/sockets/builtin.py` & `node_graph-0.0.7/node_graph/sockets/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph/utils.py` & `node_graph-0.0.7/node_graph/utils.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/node_graph.egg-info/PKG-INFO` & `node_graph-0.0.7/node_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `node_graph-0.0.6/node_graph.egg-info/SOURCES.txt` & `node_graph-0.0.7/node_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/setup.py` & `node_graph-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="node_graph",
-    version="0.0.6",
+    version="0.0.7",
     description="Create node-based workflow",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/scinode/node-graph",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
```

### Comparing `node_graph-0.0.6/tests/test_collection.py` & `node_graph-0.0.7/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/tests/test_decorator.py` & `node_graph-0.0.7/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/tests/test_hooks.py` & `node_graph-0.0.7/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/tests/test_node.py` & `node_graph-0.0.7/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/tests/test_nodetree.py` & `node_graph-0.0.7/tests/test_nodetree.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/tests/test_property.py` & `node_graph-0.0.7/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.6/tests/test_socket.py` & `node_graph-0.0.7/tests/test_socket.py`

 * *Files identical despite different names*

