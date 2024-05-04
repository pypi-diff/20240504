# Comparing `tmp/tasksflow-0.1.0.tar.gz` & `tmp/tasksflow-0.2.1.tar.gz`

## Comparing `tasksflow-0.1.0.tar` & `tasksflow-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,28 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.1.0/.python-version
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tasksflow-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.1.0/requirements.lock
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tasksflow-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tasksflow-0.1.0/docs/dev.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.1.0/src/tasksflow/__init__.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 tasksflow-0.1.0/src/tasksflow/cache.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tasksflow-0.1.0/src/tasksflow/common.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 tasksflow-0.1.0/src/tasksflow/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tasksflow-0.1.0/tests/cache_test.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 tasksflow-0.1.0/tests/dev_test.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tasksflow-0.1.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.1.0/LICENSE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tasksflow-0.1.0/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tasksflow-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tasksflow-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.python-version
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.2.1/Dockerfile.ci
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tasksflow-0.2.1/README_zh_CN.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tasksflow-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.2.1/requirements.lock
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/dev.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/demo/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/demo/demo1.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/demo/requirements.txt
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.2.1/scripts/entrypoint
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/cache.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/common.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/executer.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/pool.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/cache_test.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/cpu_intensive_test.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/http_test.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/normal_test.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.2.1/LICENSE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tasksflow-0.2.1/README.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tasksflow-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tasksflow-0.2.1/PKG-INFO
```

### Comparing `tasksflow-0.1.0/LICENSE` & `tasksflow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tasksflow-0.1.0/pyproject.toml` & `tasksflow-0.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [project]
 name = "tasksflow"
-version = "0.1.0"
+version = "0.2.1"
 description = "Supporting complex processes through tasks"
-authors = [
-    { name = "117503445", email = "t117503445@gmail.com" }
-]
-dependencies = [
-    "loguru>=0.7.2",
-]
+authors = [{ name = "117503445", email = "t117503445@gmail.com" }]
+dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "pytest>=8.1.1",
+    "aiohttp>=3.9.5",
+    "pytest-asyncio>=0.23.6",
+    "fastapi>=0.110.2",
+    "requests>=2.31.0",
+    "uvicorn>=0.29.0",
+    "types-requests>=2.31.0.20240406",
+    "ruff>=0.4.1",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/tasksflow"]
 
 [tool.hatch.build]
-exclude = [
-    ".vscode",
-    ".gitignore",
-    "docker-compose.yml",
-    "Dockerfile.dev",
-]
+exclude = [".vscode", ".gitignore", "docker-compose.yml", "Dockerfile.dev"]
```

