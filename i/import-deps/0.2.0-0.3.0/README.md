# Comparing `tmp/import_deps-0.2.0.tar.gz` & `tmp/import_deps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "import_deps-0.2.0.tar", last modified: Sun Jan 16 19:51:09 2022, max compression
+gzip compressed data, was "import_deps-0.3.0.tar", last modified: Sat May  4 03:44:08 2024, max compression
```

## Comparing `import_deps-0.2.0.tar` & `import_deps-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-01-16 19:51:09.337582 import_deps-0.2.0/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4836 2022-01-16 19:51:09.337582 import_deps-0.2.0/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2889 2022-01-16 19:43:12.000000 import_deps-0.2.0/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-01-16 19:51:09.337582 import_deps-0.2.0/import_deps/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5124 2022-01-16 19:45:02.000000 import_deps-0.2.0/import_deps/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      358 2020-05-24 12:45:00.000000 import_deps-0.2.0/import_deps/__main__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-01-16 19:51:09.337582 import_deps-0.2.0/import_deps.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4836 2022-01-16 19:51:09.000000 import_deps-0.2.0/import_deps.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      288 2022-01-16 19:51:09.000000 import_deps-0.2.0/import_deps.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2022-01-16 19:51:09.000000 import_deps-0.2.0/import_deps.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       59 2022-01-16 19:51:09.000000 import_deps-0.2.0/import_deps.egg-info/entry_points.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       18 2022-01-16 19:51:09.000000 import_deps-0.2.0/import_deps.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2022-01-16 19:51:09.337582 import_deps-0.2.0/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1218 2022-01-16 19:45:20.000000 import_deps-0.2.0/setup.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-01-16 19:51:09.337582 import_deps-0.2.0/tests/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2020-05-24 12:45:00.000000 import_deps-0.2.0/tests/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6545 2022-01-16 19:20:57.000000 import_deps-0.2.0/tests/test_import_deps.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-05-04 03:44:08.102291 import_deps-0.3.0/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1087 2020-05-24 12:45:00.000000 import_deps-0.3.0/LICENSE
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4001 2024-05-04 03:44:08.102291 import_deps-0.3.0/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2981 2024-05-04 03:37:04.000000 import_deps-0.3.0/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-05-04 03:44:08.098291 import_deps-0.3.0/import_deps/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5124 2024-05-04 03:37:04.000000 import_deps-0.3.0/import_deps/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      739 2024-05-04 03:37:04.000000 import_deps-0.3.0/import_deps/__main__.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-05-04 03:44:08.098291 import_deps-0.3.0/import_deps.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4001 2024-05-04 03:44:08.000000 import_deps-0.3.0/import_deps.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      296 2024-05-04 03:44:08.000000 import_deps-0.3.0/import_deps.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-05-04 03:44:08.000000 import_deps-0.3.0/import_deps.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       59 2024-05-04 03:44:08.000000 import_deps-0.3.0/import_deps.egg-info/entry_points.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       18 2024-05-04 03:44:08.000000 import_deps-0.3.0/import_deps.egg-info/top_level.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-05-04 03:44:08.102291 import_deps-0.3.0/setup.cfg
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1318 2024-05-04 03:37:04.000000 import_deps-0.3.0/setup.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-05-04 03:44:08.102291 import_deps-0.3.0/tests/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2020-05-24 12:45:00.000000 import_deps-0.3.0/tests/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     6545 2022-01-16 19:20:57.000000 import_deps-0.3.0/tests/test_import_deps.py
```

### Comparing `import_deps-0.2.0/README.md` & `import_deps-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 ## Install
 
 ```
 pip install import_deps
 ```
 
-## Usage
 
+## Usage
 
 `import_deps` is designed to track only imports within a known set of package and modules.
 
 Given a package with the modules:
 
 - `foo/__init__.py`
 - `foo/foo_a.py`
@@ -31,14 +31,24 @@
 Where `foo_a.py` has the following imports:
 
 ```python3
 from . import foo_b
 from .foo_c import obj_c
 ```
 
+## Usage (CLI)
+
+```bash
+> import_deps foo/foo_a.py
+foo.foo_b
+foo.foo_c
+```
+
+
+## Usage (lib)
 
 ```python3
 import pathlib
 from import_deps import ModuleSet
 
 # First initialise a ModuleSet instance with a list str of modules to track
 pkg_paths = pathlib.Path('foo').glob('**/*.py')
```

### Comparing `import_deps-0.2.0/import_deps/__init__.py` & `import_deps-0.3.0/import_deps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = (0, 2, 0)
+__version__ = (0, 3, 0)
 
 import ast
 import pathlib
 
 
 class _ImportsFinder(ast.NodeVisitor):
     """find all imports
```

### Comparing `import_deps-0.2.0/setup.py` & `import_deps-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="import_deps",
-    version="0.2.0",
+    version="0.3.0",
     author = 'Eduardo Naufel Schettino',
     author_email = 'schettino72@gmail.com',
     url = 'https://github.com/schettino72/import-deps',
     description='find python module imports',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
@@ -20,14 +20,16 @@
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Quality Assurance',
     ),
     keywords = "import graph quality",
 
     entry_points = {
         'console_scripts': [
```

### Comparing `import_deps-0.2.0/tests/test_import_deps.py` & `import_deps-0.3.0/tests/test_import_deps.py`

 * *Files identical despite different names*

