# Comparing `tmp/kfsconfig-1.2.0.tar.gz` & `tmp/kfsconfig-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsconfig-1.2.0.tar", max compression
+gzip compressed data, was "kfsconfig-2.0.0.tar", max compression
```

## Comparing `kfsconfig-1.2.0.tar` & `kfsconfig-2.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7245 2024-04-20 12:50:38.852606 kfsconfig-1.2.0/KFSconfig/KFSconfig.py
--rw-r--r--   0        0        0      515 2024-04-20 12:50:38.852606 kfsconfig-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      668 2024-04-20 12:50:38.852606 kfsconfig-1.2.0/readme.md
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 kfsconfig-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13919 2024-05-04 17:44:24.287002 kfsconfig-2.0.0/KFSconfig/KFSconfig.py
+-rw-r--r--   0        0        0      514 2024-05-04 17:44:24.287002 kfsconfig-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-04 17:44:24.287002 kfsconfig-2.0.0/readme.md
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kfsconfig-2.0.0/PKG-INFO
```

### Comparing `kfsconfig-1.2.0/pyproject.toml` & `kfsconfig-2.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 authors     = ["9FS <pray4spam@googlemail.com>"]
 description = ""
 license     = "MIT"
 name        = "KFSconfig"
 packages    = [{ include = "KFSconfig" }]
 readme      = "readme.md"
 repository  = "https://github.com/9-FS/2023-09-20-KFSconfig"
-version     = "1.2.0"
+version     = "2.0.0"
 
 [tool.poetry.dependencies]
 KFSlog = "^1.0.0"
-python = "^3.11.0"
+python = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies]
-hypothesis = "^6.87.0"
-pytest     = "^7.4.2"
+hypothesis = "^6.0.0"
+pytest     = "^7.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires      = ["poetry-core"]
```

### Comparing `kfsconfig-1.2.0/readme.md` & `kfsconfig-2.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `kfsconfig-1.2.0/PKG-INFO` & `kfsconfig-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: KFSconfig
-Version: 1.2.0
+Version: 2.0.0
 Summary: 
 Home-page: https://github.com/9-FS/2023-09-20-KFSconfig
 License: MIT
 Author: 9FS
 Author-email: pray4spam@googlemail.com
-Requires-Python: >=3.11.0,<4.0.0
+Requires-Python: >=3.12.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: KFSlog (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/9-FS/2023-09-20-KFSconfig
 Description-Content-Type: text/markdown
 
 ---
 Topic: "KFSconfig"
```

