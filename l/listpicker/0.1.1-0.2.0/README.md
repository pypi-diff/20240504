# Comparing `tmp/listpicker-0.1.1.tar.gz` & `tmp/listpicker-0.2.0.tar.gz`

## Comparing `listpicker-0.1.1.tar` & `listpicker-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 listpicker-0.1.1/src/listpicker/__init__.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 listpicker-0.1.1/src/listpicker/keyboard.py
--rw-r--r--   0        0        0    20641 2020-02-02 00:00:00.000000 listpicker-0.1.1/src/listpicker/listpicker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 listpicker-0.1.1/src/listpicker/py.typed
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 listpicker-0.1.1/src/listpicker/util.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 listpicker-0.1.1/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 listpicker-0.1.1/LICENSE
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 listpicker-0.1.1/README.md
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 listpicker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 listpicker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/__init__.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/keyboard.py
+-rw-r--r--   0        0        0    20641 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/listpicker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/py.typed
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 listpicker-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 listpicker-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 listpicker-0.2.0/README.md
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 listpicker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 listpicker-0.2.0/PKG-INFO
```

### Comparing `listpicker-0.1.1/src/listpicker/__init__.py` & `listpicker-0.2.0/src/listpicker/__init__.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.1.1/src/listpicker/keyboard.py` & `listpicker-0.2.0/src/listpicker/keyboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     bytes_to_int(0x1B, ord("["), ord("7"), ord("~")): "Home",  # vt
     bytes_to_int(0x1B, ord("["), ord("8"), ord("~")): "End",  # vt
     bytes_to_int(0x1B, ord("["), ord("1"), ord("1"), ord("~")): "F1",
     bytes_to_int(0x1B, ord("O"), ord("P")): "F1",
 }
 
 
-class NonCanonicalModeTerminalWrapper:
+class NonCanonicalModeTerminalInput:
     _file: TextIO
     _old_attrs: list[Any]
 
     def __init__(self, file: TextIO):
         if not file.isatty():
             raise ValueError(f"file is not a tty: ${file!r}")
 
@@ -64,18 +64,19 @@
         fd = self._file.fileno()
         self._old_attrs = termios.tcgetattr(fd)
         tty.setcbreak(fd, termios.TCSAFLUSH)
         return self._file
 
     def __exit__(self, *_args: object) -> None:
         termios.tcsetattr(self._file.fileno(), termios.TCSAFLUSH, self._old_attrs)
+        self._old_attrs.clear()
 
 
 def getkey(file: TextIO) -> Optional[str]:
-    with NonCanonicalModeTerminalWrapper(file) as f:
+    with NonCanonicalModeTerminalInput(file) as f:
         ch = f.read(1)
 
         if ch == "\x1b":
             ch = f.read(1)
 
             if ch in ("[", "O"):
                 # The subset of escape sequences we accept end in a capital letter or tilde
```

### Comparing `listpicker-0.1.1/src/listpicker/listpicker.py` & `listpicker-0.2.0/src/listpicker/listpicker.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.1.1/src/listpicker/util.py` & `listpicker-0.2.0/src/listpicker/util.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.1.1/LICENSE` & `listpicker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `listpicker-0.1.1/README.md` & `listpicker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `listpicker-0.1.1/pyproject.toml` & `listpicker-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "listpicker"
 description = "Interactive list selection and multiselect for POSIX terminals (non-curses)"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
     {name = "Sung Pae", email = "self@sungpae.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `listpicker-0.1.1/PKG-INFO` & `listpicker-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: listpicker
-Version: 0.1.1
+Version: 0.2.0
 Summary: Interactive list selection and multiselect for POSIX terminals (non-curses)
 Project-URL: Homepage, https://github.com/guns/python-listpicker
 Project-URL: Repository, https://github.com/guns/python-listpicker.git
 Author-email: Sung Pae <self@sungpae.com>
 License: The MIT License (MIT)
         
         Copyright © 2024 Sung Pae <self@sungpae.com>
```

