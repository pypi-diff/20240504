# Comparing `tmp/tkfontselector-1.0.7.tar.gz` & `tmp/tkfontselector-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.7.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.8.tar", max compression
```

## Comparing `tkfontselector-1.0.7.tar` & `tkfontselector-1.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.7/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-04 05:48:07.718543 tkfontselector-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.7/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.7/tkfontselector/__init__.py
--rw-r--r--   0        0        0     2035 2024-05-04 04:24:14.225463 tkfontselector-1.0.7/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    19933 2024-05-04 05:47:17.178753 tkfontselector-1.0.7/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.7/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-04 06:22:23.693006 tkfontselector-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.8/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.8/tkfontselector/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-04 04:24:14.225463 tkfontselector-1.0.8/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    19932 2024-05-04 06:22:15.882156 tkfontselector-1.0.8/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.8/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.8/PKG-INFO
```

### Comparing `tkfontselector-1.0.7/LICENSE.txt` & `tkfontselector-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.7/pyproject.toml` & `tkfontselector-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.7"
+version = "1.0.8"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.7/README.md` & `tkfontselector-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.7/tkfontselector/ask_font.py` & `tkfontselector-1.0.8/tkfontselector/ask_font.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.7/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.8/tkfontselector/tkfontselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Forked from https://github.com/j4321/tkFontChooser and improved. Was going to do a PR
 to clean some things up, but the repo hasn't been active for over 5 years.
 """
 
+import os
 from tkinter import Tk, Toplevel, Listbox, StringVar, BooleanVar, TclError
 from tkinter.ttk import Checkbutton, Frame, Label, Button, Scrollbar, Style, Entry
 from tkinter.font import families, Font
-from locale import getlocale
 from typing import Union, List
 
 from tkfontselector.translations import LANGUAGES
 
 try:
-    lang_code = getlocale()[0][:2]
+    lang_code = os.environ.get("LANG").split("_")[0]
     if lang_code in LANGUAGES:
         TR = LANGUAGES[lang_code]
     else:
         TR = LANGUAGES["en"]
 except ValueError:
     TR = LANGUAGES["en"]
```

### Comparing `tkfontselector-1.0.7/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.8/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.7/PKG-INFO` & `tkfontselector-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

