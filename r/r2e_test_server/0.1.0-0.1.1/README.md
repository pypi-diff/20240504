# Comparing `tmp/r2e_test_server-0.1.0.tar.gz` & `tmp/r2e_test_server-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2e_test_server-0.1.0.tar", max compression
+gzip compressed data, was "r2e_test_server-0.1.1.tar", max compression
```

## Comparing `r2e_test_server-0.1.0.tar` & `r2e_test_server-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1060 2024-04-28 20:41:54.434892 r2e_test_server-0.1.0/LICENSE
--rw-r--r--   0        0        0      976 2024-05-01 04:26:51.498941 r2e_test_server-0.1.0/README.md
--rw-r--r--   0        0        0      601 2024-05-01 03:57:32.993005 r2e_test_server-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-28 20:41:54.435374 r2e_test_server-0.1.0/r2e_test_server/ast/__init__.py
--rw-r--r--   0        0        0     3062 2024-05-01 03:57:32.993170 r2e_test_server-0.1.0/r2e_test_server/ast/transformer.py
--rw-r--r--   0        0        0      757 2024-05-01 03:57:32.993270 r2e_test_server-0.1.0/r2e_test_server/cli.py
--rw-r--r--   0        0        0      130 2024-05-01 03:57:32.993445 r2e_test_server-0.1.0/r2e_test_server/instrument/__init__.py
--rw-r--r--   0        0        0     7416 2024-04-28 20:41:54.435695 r2e_test_server-0.1.0/r2e_test_server/instrument/arguments.py
--rw-r--r--   0        0        0     1824 2024-05-01 03:57:32.993657 r2e_test_server-0.1.0/r2e_test_server/instrument/base.py
--rw-r--r--   0        0        0        0 2024-04-28 20:41:54.435866 r2e_test_server-0.1.0/r2e_test_server/modules/__init__.py
--rw-r--r--   0        0        0     4767 2024-04-28 20:41:54.435990 r2e_test_server-0.1.0/r2e_test_server/modules/explorer.py
--rw-r--r--   0        0        0     4292 2024-05-01 03:57:32.993872 r2e_test_server-0.1.0/r2e_test_server/server.py
--rw-r--r--   0        0        0     2094 2024-04-28 20:41:54.436221 r2e_test_server-0.1.0/r2e_test_server/testing/cleaner.py
--rw-r--r--   0        0        0     5052 2024-05-01 03:57:32.994105 r2e_test_server-0.1.0/r2e_test_server/testing/codecov.py
--rw-r--r--   0        0        0     2466 2024-05-01 03:57:32.994279 r2e_test_server-0.1.0/r2e_test_server/testing/loader.py
--rw-r--r--   0        0        0     9512 2024-05-01 03:57:32.994676 r2e_test_server-0.1.0/r2e_test_server/testing/r2e_testprogram.py
--rw-r--r--   0        0        0     2947 2024-04-28 20:41:54.436633 r2e_test_server-0.1.0/r2e_test_server/testing/result.py
--rw-r--r--   0        0        0      354 2024-04-28 20:41:54.436717 r2e_test_server-0.1.0/r2e_test_server/testing/runner.py
--rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 r2e_test_server-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-27 00:14:08.782149 r2e_test_server-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1020 2024-05-02 05:33:55.087500 r2e_test_server-0.1.1/README.md
+-rw-r--r--   0        0        0      601 2024-05-04 20:58:53.322507 r2e_test_server-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/ast/__init__.py
+-rw-r--r--   0        0        0     3062 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/ast/transformer.py
+-rw-r--r--   0        0        0      757 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/cli.py
+-rw-r--r--   0        0        0      130 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/instrument/__init__.py
+-rw-r--r--   0        0        0     7431 2024-05-04 20:52:36.474257 r2e_test_server-0.1.1/r2e_test_server/instrument/arguments.py
+-rw-r--r--   0        0        0     1824 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/instrument/base.py
+-rw-r--r--   0        0        0        0 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/modules/__init__.py
+-rw-r--r--   0        0        0     4767 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/modules/explorer.py
+-rw-r--r--   0        0        0     4286 2024-05-04 20:52:36.474257 r2e_test_server-0.1.1/r2e_test_server/server.py
+-rw-r--r--   0        0        0     2094 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/testing/cleaner.py
+-rw-r--r--   0        0        0     5052 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/testing/codecov.py
+-rw-r--r--   0        0        0     2466 2024-04-29 00:05:15.445367 r2e_test_server-0.1.1/r2e_test_server/testing/loader.py
+-rw-r--r--   0        0        0     9549 2024-05-04 20:52:36.474257 r2e_test_server-0.1.1/r2e_test_server/testing/r2e_testprogram.py
+-rw-r--r--   0        0        0     2947 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/testing/result.py
+-rw-r--r--   0        0        0      354 2024-04-28 05:56:33.718445 r2e_test_server-0.1.1/r2e_test_server/testing/runner.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 r2e_test_server-0.1.1/PKG-INFO
```

### Comparing `r2e_test_server-0.1.0/LICENSE` & `r2e_test_server-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/README.md` & `r2e_test_server-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # R2E Test Server
 
-This is the test server for the [R2E framework](https://github.com/r2e-project). R2E turns any GitHub repository into an executable programming agent environment. More information about the project and framework can be found @ [r2e.github.io](https://r2e-project.github.io).
+This is the test server for the [R2E framework](https://github.com/r2e-project). R2E turns any GitHub repository into an executable programming agent environment. More information about the project and framework can be found at our [webpage](https://r2e-project.github.io).
 
 
 This server provides a [rPyC](https://rpyc.readthedocs.io/en/latest/) (remote Python call) interface to the R2E testing framework. The server is used to execute code and tests for the agent in a pre-built environment for the repository and return the results. More on how this integrates with the R2E framework can be found in the [R2E Repository](https://github.com/r2e-project/r2e).
 
 
 ## Installation
 
-Install the server using pip or any other package manager:
+Install the server using [pip](https://pypi.org/project/r2e_test_server/) or any other package manager:
 
 ```bash
-pip install r2e-test-server
+pip install r2e_test_server
 ```
 
 ## Usage
 
 To start the server, run the following command:
 
 ```bash
```

### Comparing `r2e_test_server-0.1.0/pyproject.toml` & `r2e_test_server-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r2e_test_server"
-version = "0.1.0"
+version = "0.1.1"
 description = "Test Server For R2E"
 authors = ["Naman Jain <naman_jain@berkeley.com>", "Manish Shetty <manishs@berkeley.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/r2e-project/r2e-test-server"
 
 [tool.poetry.dependencies]
```

### Comparing `r2e_test_server-0.1.0/r2e_test_server/ast/transformer.py` & `r2e_test_server-0.1.1/r2e_test_server/ast/transformer.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/cli.py` & `r2e_test_server-0.1.1/r2e_test_server/cli.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/instrument/arguments.py` & `r2e_test_server-0.1.1/r2e_test_server/instrument/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     def serialize_numpy(obj):
         try:
             import numpy as np  # type: ignore
 
             if isinstance(obj, np.ndarray):  # type: ignore
                 if obj.size > 25:
                     return f"np.ndarray(shape={obj.shape}, dtype={obj.dtype})"
-                return obj.round(2)
+                return f"np-array: {obj.round(2)}"
         except:
             pass
         return None
 
     @staticmethod
     def serialize_torch(obj):
         try:
```

### Comparing `r2e_test_server-0.1.0/r2e_test_server/instrument/base.py` & `r2e_test_server-0.1.1/r2e_test_server/instrument/base.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/modules/explorer.py` & `r2e_test_server-0.1.1/r2e_test_server/modules/explorer.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/server.py` & `r2e_test_server-0.1.1/r2e_test_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     @rpyc.exposed
     def stop_server(self):
         server_stop_event.set()
 
     @rpyc.exposed
     def setup_repo(self, data: str):
         data_dict = json.loads(data)
-        self.repo_name: str = data_dict["repo_name"]
+        self.repo_id: str = data_dict["repo_id"]
         self.repo_path: str = data_dict["repo_path"]
 
     @rpyc.exposed
     def setup_function(self, data: str):
         data_dict = json.loads(data)
         self.funclass_names: list[str] = data_dict["funclass_names"]
         self.file_path = data_dict["file_path"]
@@ -67,15 +67,15 @@
     @rpyc.exposed
     def init(self):
         try:
             stdout_buffer = StringIO()
             stderr_buffer = StringIO()
             with CaptureOutput(stdout=stdout_buffer, stderr=stderr_buffer):
                 self.r2e_test_program = R2ETestProgram(
-                    self.repo_name,
+                    self.repo_id,
                     self.repo_path,
                     self.funclass_names,
                     self.file_path,
                     self.generated_tests,
                     self.codegen_mode,
                 )
```

### Comparing `r2e_test_server-0.1.0/r2e_test_server/testing/cleaner.py` & `r2e_test_server-0.1.1/r2e_test_server/testing/cleaner.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/testing/codecov.py` & `r2e_test_server-0.1.1/r2e_test_server/testing/codecov.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/testing/loader.py` & `r2e_test_server-0.1.1/r2e_test_server/testing/loader.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/r2e_test_server/testing/r2e_testprogram.py` & `r2e_test_server-0.1.1/r2e_test_server/testing/r2e_testprogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 import sys
 import json
+import coverage
 import importlib
 import importlib.util
-import coverage
-from typing import Any
 from copy import deepcopy
+from typing import Any, Union
 from types import ModuleType, FunctionType
 
 
 from r2e_test_server.testing.loader import R2ETestLoader
 from r2e_test_server.testing.runner import R2ETestRunner
 from r2e_test_server.ast.transformer import NameReplacer
 from r2e_test_server.testing.codecov import R2ECodeCoverage
@@ -23,23 +23,23 @@
     Args:
         fid (str): identifier for function under test.
         codegen (bool): Whether the function under test is generated code.
     """
 
     def __init__(
         self,
-        repo_name: str,
+        repo_id: str,
         repo_path: str,
         funclass_names: list[str],
         file_path: str,
         generated_tests: dict[str, str],
         codegen_mode: bool = False,
     ):
-        self.repo_name = repo_name
-        self.repo_path = repo_path
+        self.repo_id = repo_id
+        self.repo_path = f"/repos/{repo_id}"
         self.funclass_names = funclass_names
         self.file_path = file_path
         self.generated_tests = generated_tests
         self.codegen_mode = codegen_mode
 
         with open(file_path, "r") as file:
             self.orig_file_content = file.read()
@@ -228,19 +228,21 @@
             raise
         except Exception as e:
             print("[ERROR] Bug in the imported FUT module?")
             raise
 
         return fut_module, fut_module_deps
 
-    def get_funclass_object(self, name: str) -> FunctionType | type:
+    def get_funclass_object(self, name: str) -> Union[FunctionType, type]:
         """Get the function or class object from the module by name."""
         return getattr(self.fut_module, name)
 
-    def get_funclass_ast(self, funclass_name: str) -> ast.FunctionDef | ast.ClassDef:
+    def get_funclass_ast(
+        self, funclass_name: str
+    ) -> Union[ast.FunctionDef, ast.ClassDef]:
         """Get the function or class AST node from the original file by name."""
         for node in self.orig_file_ast.body:
             if isinstance(node, ast.ClassDef) or isinstance(node, ast.FunctionDef):
                 if node.name == funclass_name:
                     return node
         raise ValueError(f"Function or class {funclass_name} not found in the file.")
```

### Comparing `r2e_test_server-0.1.0/r2e_test_server/testing/result.py` & `r2e_test_server-0.1.1/r2e_test_server/testing/result.py`

 * *Files identical despite different names*

### Comparing `r2e_test_server-0.1.0/PKG-INFO` & `r2e_test_server-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2e_test_server
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test Server For R2E
 Home-page: https://github.com/r2e-project/r2e-test-server
 License: MIT
 Author: Naman Jain
 Author-email: naman_jain@berkeley.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,26 +18,26 @@
 Requires-Dist: rpyc (>=6.0.0,<7.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/r2e-project/r2e-test-server
 Description-Content-Type: text/markdown
 
 # R2E Test Server
 
-This is the test server for the [R2E framework](https://github.com/r2e-project). R2E turns any GitHub repository into an executable programming agent environment. More information about the project and framework can be found @ [r2e.github.io](https://r2e-project.github.io).
+This is the test server for the [R2E framework](https://github.com/r2e-project). R2E turns any GitHub repository into an executable programming agent environment. More information about the project and framework can be found at our [webpage](https://r2e-project.github.io).
 
 
 This server provides a [rPyC](https://rpyc.readthedocs.io/en/latest/) (remote Python call) interface to the R2E testing framework. The server is used to execute code and tests for the agent in a pre-built environment for the repository and return the results. More on how this integrates with the R2E framework can be found in the [R2E Repository](https://github.com/r2e-project/r2e).
 
 
 ## Installation
 
-Install the server using pip or any other package manager:
+Install the server using [pip](https://pypi.org/project/r2e_test_server/) or any other package manager:
 
 ```bash
-pip install r2e-test-server
+pip install r2e_test_server
 ```
 
 ## Usage
 
 To start the server, run the following command:
 
 ```bash
```

