# Comparing `tmp/tkfontselector-1.0.2.tar.gz` & `tmp/tkfontselector-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.2.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.3.tar", max compression
```

## Comparing `tkfontselector-1.0.2.tar` & `tkfontselector-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-03 21:47:43.240510 tkfontselector-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.2/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.2/tkfontselector/__init__.py
--rw-r--r--   0        0        0       22 2024-05-03 21:12:57.402449 tkfontselector-1.0.2/tkfontselector/_version.py
--rw-r--r--   0        0        0     1404 2024-05-03 21:10:32.587835 tkfontselector-1.0.2/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    18418 2024-05-03 21:13:43.402212 tkfontselector-1.0.2/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.2/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-03 21:53:30.259261 tkfontselector-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.3/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.3/tkfontselector/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-03 21:53:36.027245 tkfontselector-1.0.3/tkfontselector/_version.py
+-rw-r--r--   0        0        0     1507 2024-05-03 21:54:12.379453 tkfontselector-1.0.3/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    18418 2024-05-03 21:13:43.402212 tkfontselector-1.0.3/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.3/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.3/PKG-INFO
```

### Comparing `tkfontselector-1.0.2/LICENSE.txt` & `tkfontselector-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.2/pyproject.toml` & `tkfontselector-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.2"
+version = "1.0.3"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.2/README.md` & `tkfontselector-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.2/tkfontselector/ask_font.py` & `tkfontselector-1.0.3/tkfontselector/ask_font.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Union
 from tkfontselector.tkfontselector import FontSelector
+from tkinter import Tk, Toplevel
 
 
 def ask_font(
-    master=None,
-    text="Abcd",
-    title="Font Selector",
+    master: Union[Tk, Toplevel, None] = None,
+    text: str = "Abcd",
+    title: str = "Font Selector",
     fixed_only: bool = False,
     **font_args
 ) -> dict:
     """
     Open the Font Selector and return a dictionary of the font properties.
 
     General Arguments:
```

### Comparing `tkfontselector-1.0.2/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.3/tkfontselector/tkfontselector.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.2/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.3/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.2/PKG-INFO` & `tkfontselector-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

