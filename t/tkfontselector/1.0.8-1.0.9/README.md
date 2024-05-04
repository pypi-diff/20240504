# Comparing `tmp/tkfontselector-1.0.8.tar.gz` & `tmp/tkfontselector-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.8.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.9.tar", max compression
```

## Comparing `tkfontselector-1.0.8.tar` & `tkfontselector-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-04 06:22:23.693006 tkfontselector-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.8/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.8/tkfontselector/__init__.py
--rw-r--r--   0        0        0     2035 2024-05-04 04:24:14.225463 tkfontselector-1.0.8/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    19932 2024-05-04 06:22:15.882156 tkfontselector-1.0.8/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.8/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-04 17:21:35.536351 tkfontselector-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.9/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.9/tkfontselector/__init__.py
+-rw-r--r--   0        0        0     2180 2024-05-04 17:20:59.208687 tkfontselector-1.0.9/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    20145 2024-05-04 17:21:14.442860 tkfontselector-1.0.9/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-04 17:11:13.164073 tkfontselector-1.0.9/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-04 17:11:06.593335 tkfontselector-1.0.9/tkfontselector/translations/get_system_locale.py
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.9/PKG-INFO
```

### Comparing `tkfontselector-1.0.8/LICENSE.txt` & `tkfontselector-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.8/pyproject.toml` & `tkfontselector-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.8"
+version = "1.0.9"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.8/README.md` & `tkfontselector-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.8/tkfontselector/ask_font.py` & `tkfontselector-1.0.9/tkfontselector/ask_font.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 from tkinter import Tk, Toplevel
 
 
 def ask_font(
     master: Union[Tk, Toplevel, None] = None,
     text: str = "Abcd",
     title: str = "Font Selector",
-    fixed_only: bool = False,
+    fixed_only: Union[bool, None] = None,
     families_only: bool = False,
     font_args: dict = {},
 ) -> dict:
     """
     Open the Font Selector and return a dictionary of the font properties.
 
     General Arguments:
         master: Tk or Toplevel instance
             master window
         text: str
             sample text to be displayed in the Font Selector
         title: str
             dialog title
-        fixed_only: bool
-            Display fixed only families
+        fixed_only: (bool, None)
+            if set to `True` will display mono spaced fonts only, if set to `False`
+            will only show regular fonts, if set to `None` will show everything
         families_only: bool
             Will only display Families part of the UI
         font_dict: dict
             dictionary, like the one returned by the ``actual`` method of a ``Font`` object:
                 {'family': str,
                     'size': int,
                     'weight': 'bold'/'normal',
```

### Comparing `tkfontselector-1.0.8/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.9/tkfontselector/tkfontselector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 """
 Forked from https://github.com/j4321/tkFontChooser and improved. Was going to do a PR
 to clean some things up, but the repo hasn't been active for over 5 years.
 """
 
-import os
 from tkinter import Tk, Toplevel, Listbox, StringVar, BooleanVar, TclError
 from tkinter.ttk import Checkbutton, Frame, Label, Button, Scrollbar, Style, Entry
 from tkinter.font import families, Font
 from typing import Union, List
 
 from tkfontselector.translations import LANGUAGES
+from tkfontselector.translations.get_system_locale import system_locale
 
-try:
-    lang_code = os.environ.get("LANG").split("_")[0]
-    if lang_code in LANGUAGES:
-        TR = LANGUAGES[lang_code]
-    else:
-        TR = LANGUAGES["en"]
-except ValueError:
-    TR = LANGUAGES["en"]
+TR = LANGUAGES["en"]
+detect_language = system_locale()
+if detect_language and detect_language in LANGUAGES.keys():
+    TR = LANGUAGES[detect_language]
 
 
 class FontSelector(Toplevel):
     """Font Selector dialog."""
 
     def __init__(
         self,
         master: Union[Tk, Toplevel] = None,
         text: str = "Abcd",
         title: str = "Font Selector",
-        fixed_only: bool = False,
+        fixed_only: Union[bool, None] = None,
         families_only: bool = False,
         font_dict: dict = {},
         **kwargs
     ):
         """
         Create a new FontSelector instance.
         Arguments:
             master: Tk or Toplevel instance
                 master window
             text: str
                 text to be displayed in the preview label
             title: str
                 window title
-            fixed_only: bool
-                will display fixed (mono spaced) fonts only
+            fixed_only: (bool, None)
+                if set to `True` will display mono spaced fonts only, if set to `False`
+                will only show regular fonts, if set to `None` will show everything
             families_only: bool
                 will only display the family part of the UI
             font_dict: dict
                 dictionary, like the one returned by the ``actual`` method of a ``Font`` object:
                     {'family': str,
                      'size': int,
                      'weight': 'bold'/'normal',
@@ -71,15 +68,17 @@
         # --- variable storing the chosen font
         self.res = ""
 
         self.style = Style(self)
         self.style.configure("prev.TLabel", background="white")
 
         # --- family list
-        if fixed_only:
+        if fixed_only is None:
+            self.fonts = list(families())
+        elif fixed_only:
             self.fonts = self._get_fixed_families()
         else:
             self.fonts = self._get_non_fixed_families()
         self.fonts.append("TkDefaultFont")
         self.fonts.sort()
         for i in range(len(self.fonts)):
             self.fonts[i] = self.fonts[i].replace(" ", "\ ")
```

### Comparing `tkfontselector-1.0.8/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.9/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.8/PKG-INFO` & `tkfontselector-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

