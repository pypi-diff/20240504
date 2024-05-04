# Comparing `tmp/dekvenv-0.1.8.tar.gz` & `tmp/dekvenv-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekvenv-0.1.8.tar", last modified: Sat Feb 17 12:35:01 2024, max compression
+gzip compressed data, was "dekvenv-0.1.9.tar", last modified: Sat Feb 17 13:09:50 2024, max compression
```

## Comparing `dekvenv-0.1.8.tar` & `dekvenv-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1075 2024-02-17 12:34:59.481775 dekvenv-0.1.8/LICENSE
--rw-r--r--   0        0        0      125 2024-02-17 12:34:59.481775 dekvenv-0.1.8/README.md
--rw-r--r--   0        0        0       49 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/__entry__.py
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/__init__.py
--rw-r--r--   0        0        0      359 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/active.py
--rw-r--r--   0        0        0      403 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/command.py
--rw-r--r--   0        0        0      101 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/constants.py
--rw-r--r--   0        0        0       71 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/dekshellplugin/__init__.py
--rw-r--r--   0        0        0       79 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/dekshellplugin/contexts/__init__.py
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/main/__init__.py
--rw-r--r--   0        0        0     2530 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/main/command.py
--rw-r--r--   0        0        0      200 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/main/core.py
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pdm/__init__.py
--rw-r--r--   0        0        0     1005 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pdm/command.py
--rw-r--r--   0        0        0     3697 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pdm/core.py
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pipconf/__init__.py
--rw-r--r--   0        0        0      775 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pipconf/command.py
--rw-r--r--   0        0        0     3502 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pipconf/core.py
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pypirc/__init__.py
--rw-r--r--   0        0        0      944 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pypirc/command.py
--rw-r--r--   0        0        0     2897 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/pypirc/core.py
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/script/__init__.py
--rw-r--r--   0        0        0     6858 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/script/command.py
--rw-r--r--   0        0        0      888 2024-02-17 12:34:59.481775 dekvenv-0.1.8/dekvenv/script/core.py
--rw-r--r--   0        0        0      128 2024-02-17 12:34:59.485775 dekvenv-0.1.8/dekvenv/script/res/pyproject.toml-tpl
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.485775 dekvenv-0.1.8/dekvenv/utils/__init__.py
--rw-r--r--   0        0        0     2355 2024-02-17 12:34:59.485775 dekvenv-0.1.8/dekvenv/utils/common.py
--rw-r--r--   0        0        0      611 2024-02-17 12:35:01.329809 dekvenv-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-17 12:34:59.485775 dekvenv-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      127 2024-02-17 12:34:59.485775 dekvenv-0.1.8/tests/test_main.py
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 dekvenv-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-02-17 13:09:48.143266 dekvenv-0.1.9/LICENSE
+-rw-r--r--   0        0        0      125 2024-02-17 13:09:48.143266 dekvenv-0.1.9/README.md
+-rw-r--r--   0        0        0       49 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/__entry__.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/__init__.py
+-rw-r--r--   0        0        0      359 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/active.py
+-rw-r--r--   0        0        0      403 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/command.py
+-rw-r--r--   0        0        0      101 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/constants.py
+-rw-r--r--   0        0        0       71 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/dekshellplugin/__init__.py
+-rw-r--r--   0        0        0       79 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/dekshellplugin/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/main/__init__.py
+-rw-r--r--   0        0        0     2530 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/main/command.py
+-rw-r--r--   0        0        0      200 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/main/core.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pdm/__init__.py
+-rw-r--r--   0        0        0     1390 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pdm/command.py
+-rw-r--r--   0        0        0     3697 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pipconf/__init__.py
+-rw-r--r--   0        0        0      775 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pipconf/command.py
+-rw-r--r--   0        0        0     3502 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pipconf/core.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pypirc/__init__.py
+-rw-r--r--   0        0        0      944 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pypirc/command.py
+-rw-r--r--   0        0        0     2897 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/pypirc/core.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/script/__init__.py
+-rw-r--r--   0        0        0     6858 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/script/command.py
+-rw-r--r--   0        0        0      888 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/script/core.py
+-rw-r--r--   0        0        0      128 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/script/res/pyproject.toml-tpl
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/utils/__init__.py
+-rw-r--r--   0        0        0     2355 2024-02-17 13:09:48.143266 dekvenv-0.1.9/dekvenv/utils/common.py
+-rw-r--r--   0        0        0      611 2024-02-17 13:09:49.991265 dekvenv-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-17 13:09:48.143266 dekvenv-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      127 2024-02-17 13:09:48.143266 dekvenv-0.1.9/tests/test_main.py
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 dekvenv-0.1.9/PKG-INFO
```

### Comparing `dekvenv-0.1.8/LICENSE` & `dekvenv-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/main/command.py` & `dekvenv-0.1.9/dekvenv/main/command.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/pdm/core.py` & `dekvenv-0.1.9/dekvenv/pdm/core.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/pipconf/command.py` & `dekvenv-0.1.9/dekvenv/pipconf/command.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/pipconf/core.py` & `dekvenv-0.1.9/dekvenv/pipconf/core.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/pypirc/command.py` & `dekvenv-0.1.9/dekvenv/pypirc/command.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/pypirc/core.py` & `dekvenv-0.1.9/dekvenv/pypirc/core.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/script/command.py` & `dekvenv-0.1.9/dekvenv/script/command.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/script/core.py` & `dekvenv-0.1.9/dekvenv/script/core.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/dekvenv/utils/common.py` & `dekvenv-0.1.9/dekvenv/utils/common.py`

 * *Files identical despite different names*

### Comparing `dekvenv-0.1.8/pyproject.toml` & `dekvenv-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dekvenv"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = [
     { name = "sanzenwin", email = "sanzenwin@gmail.com" },
 ]
 dependencies = [
     "virtualenv<21.0.0",
     "build<=0.10.0",
```

