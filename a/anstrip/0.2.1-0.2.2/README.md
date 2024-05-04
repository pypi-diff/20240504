# Comparing `tmp/anstrip-0.2.1.tar.gz` & `tmp/anstrip-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anstrip-0.2.1.tar", last modified: Mon Apr 15 22:39:48 2024, max compression
+gzip compressed data, was "anstrip-0.2.2.tar", last modified: Sat May  4 14:44:05 2024, max compression
```

## Comparing `anstrip-0.2.1.tar` & `anstrip-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:39:48.866291 anstrip-0.2.1/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1061 2024-04-14 10:56:07.000000 anstrip-0.2.1/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2416 2024-04-15 22:39:48.866291 anstrip-0.2.1/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      605 2024-04-15 22:39:42.000000 anstrip-0.2.1/README.md
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      588 2024-04-15 22:39:42.000000 anstrip-0.2.1/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-15 22:39:48.866291 anstrip-0.2.1/setup.cfg
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:39:48.862958 anstrip-0.2.1/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:39:48.862958 anstrip-0.2.1/src/anstrip/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3524 2024-04-15 22:39:42.000000 anstrip-0.2.1/src/anstrip/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2691 2024-04-15 22:37:07.000000 anstrip-0.2.1/src/anstrip/__init__.pyi
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 11:16:28.000000 anstrip-0.2.1/src/anstrip/py.typed
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-15 22:39:48.862958 anstrip-0.2.1/src/anstrip.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2416 2024-04-15 22:39:48.000000 anstrip-0.2.1/src/anstrip.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      276 2024-04-15 22:39:48.000000 anstrip-0.2.1/src/anstrip.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-15 22:39:48.000000 anstrip-0.2.1/src/anstrip.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-04-15 22:39:48.000000 anstrip-0.2.1/src/anstrip.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        8 2024-04-15 22:39:48.000000 anstrip-0.2.1/src/anstrip.egg-info/top_level.txt
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-05-04 14:44:05.780470 anstrip-0.2.2/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1061 2024-04-14 10:56:07.000000 anstrip-0.2.2/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2416 2024-05-04 14:44:05.780470 anstrip-0.2.2/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      605 2024-04-15 22:39:42.000000 anstrip-0.2.2/README.md
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      588 2024-05-04 14:44:02.000000 anstrip-0.2.2/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-05-04 14:44:05.780470 anstrip-0.2.2/setup.cfg
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-05-04 14:44:05.777137 anstrip-0.2.2/src/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-05-04 14:44:05.777137 anstrip-0.2.2/src/anstrip/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3610 2024-05-04 14:41:46.000000 anstrip-0.2.2/src/anstrip/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2691 2024-04-15 22:37:07.000000 anstrip-0.2.2/src/anstrip/__init__.pyi
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-04-14 11:16:28.000000 anstrip-0.2.2/src/anstrip/py.typed
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-05-04 14:44:05.780470 anstrip-0.2.2/src/anstrip.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2416 2024-05-04 14:44:05.000000 anstrip-0.2.2/src/anstrip.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      276 2024-05-04 14:44:05.000000 anstrip-0.2.2/src/anstrip.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-05-04 14:44:05.000000 anstrip-0.2.2/src/anstrip.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       58 2024-05-04 14:44:05.000000 anstrip-0.2.2/src/anstrip.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        8 2024-05-04 14:44:05.000000 anstrip-0.2.2/src/anstrip.egg-info/top_level.txt
```

### Comparing `anstrip-0.2.1/LICENSE` & `anstrip-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anstrip-0.2.1/PKG-INFO` & `anstrip-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anstrip
-Version: 0.2.1
+Version: 0.2.2
 Summary: anstrip is a minimal library to strip ANSI sequences from strings.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `anstrip-0.2.1/README.md` & `anstrip-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `anstrip-0.2.1/pyproject.toml` & `anstrip-0.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "anstrip"
 description = "anstrip is a minimal library to strip ANSI sequences from strings."
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 keywords = ["ansi", "escape sequence", "SGR", "ECMA", "strip"]
 requires-python = ">=3.10"
 
 
 [project.optional-dependencies]
 dev = ["pytest>=7.4", "coverage>=7.4", "pyright>=1.1", "build", "twine"]
```

### Comparing `anstrip-0.2.1/src/anstrip/__init__.py` & `anstrip-0.2.2/src/anstrip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 - `PATTERN`, the regex pattern used by the functions of anstrip
 - `strip`, a function to remove all the escape sequences from a string
 - `auto_strip`, a function that is similar to `strip`, except that it only removes if the output is a TTY
 - `print`, a function that is similar to the built-in `print` but with sequence auto-stripping
 - `printed_length`, a function that returns the length of the string as seen on the screen
 """
 
+import builtins as _builtins
 import collections.abc
 import functools
 import re
 import sys
 import typing
 
 __all__ = [
@@ -97,15 +98,21 @@
     Similar to the built-in function `print`, but ANSI escape sequences are
     automatically stripped if `file` is not a TTY.
     """
 
     def str_and_auto_strip(value: object) -> str:
         return typing.cast(str, auto_strip(str(value), output=file))
 
-    print(*map(str_and_auto_strip, values), sep=sep, end=end, file=file, flush=flush)
+    _builtins.print(
+        *map(str_and_auto_strip, values),
+        sep=sep,
+        end=end,
+        file=file,
+        flush=flush,
+    )
 
 
 def printed_length(string: str) -> int:
     """
     Return the length of the string without counting characters that are not
     actually visible (ANSI sequences).
```

### Comparing `anstrip-0.2.1/src/anstrip/__init__.pyi` & `anstrip-0.2.2/src/anstrip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `anstrip-0.2.1/src/anstrip.egg-info/PKG-INFO` & `anstrip-0.2.2/src/anstrip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anstrip
-Version: 0.2.1
+Version: 0.2.2
 Summary: anstrip is a minimal library to strip ANSI sequences from strings.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

