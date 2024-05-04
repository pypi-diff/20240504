# Comparing `tmp/tkfontselector-1.0.5.tar.gz` & `tmp/tkfontselector-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.5.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.6.tar", max compression
```

## Comparing `tkfontselector-1.0.5.tar` & `tkfontselector-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-03 23:04:13.947917 tkfontselector-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.5/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.5/tkfontselector/__init__.py
--rw-r--r--   0        0        0     1507 2024-05-03 21:54:12.379453 tkfontselector-1.0.5/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    18380 2024-05-03 23:02:58.284107 tkfontselector-1.0.5/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.5/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-04 04:26:34.871849 tkfontselector-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.6/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.6/tkfontselector/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-04 04:24:14.225463 tkfontselector-1.0.6/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    19274 2024-05-04 04:29:03.193623 tkfontselector-1.0.6/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.6/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.6/PKG-INFO
```

### Comparing `tkfontselector-1.0.5/LICENSE.txt` & `tkfontselector-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.5/pyproject.toml` & `tkfontselector-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.5"
+version = "1.0.6"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.5/README.md` & `tkfontselector-1.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,22 +41,24 @@
     'overstrike': bool}
 ```
 
 ## General arguments
 
 `master`: Tk, Toplevel, or None (Optional)
 
-`font_dict`: dict (Optional) _font dictionary like an actual Font object_
-
 `text`: str (Optional) _text to show in the font selection window_
 
 `title`: str (Optional) _changes the title of the window_
 
 `fixed_only`: bool (Optional), _if set to `True` will only show `Fixed (mono spaced)` fonts_
 
+`families_only`: bool (Optional), _if set to `True` will only show Font Families part of the UI_
+
+`font_dict`: dict (Optional) _font dictionary like an actual Font object_
+
 `**kwargs`: (Optional) _pass any other args that might be accepted_
 
 ## Font Arguments
 
 `family`: str
 
 `size`: int
@@ -68,14 +70,25 @@
 `underline`: bool
 
 `overstrike`: bool
 
 ## Example
 
 ```python
+EXAMPLE_FONT_FAMILY = {
+    "family": "Comic Sans MS",
+    "size": 10,
+    "weight": "normal",
+    "slant": "roman",
+    "underline": 0,
+    "overstrike": 0,
+}
+
+
+if __name__ == "__main__":
     """Example Usage"""
     root = Tk()
     style = ttk.Style(root)
     if "win" == platform[:3]:
         style.theme_use("vista")
     elif "darwin" in platform:
         style.theme_use("clam")
@@ -83,15 +96,15 @@
         style.theme_use("clam")
     bg = style.lookup("TLabel", "background")
     root.configure(bg=bg)
     label = ttk.Label(root, text="Chosen font: ")
     label.pack(padx=10, pady=(10, 4))
 
     def callback():
-        font = ask_font(root, title="Choose a font")
+        font = ask_font(root, title="Choose a font", font_args=EXAMPLE_FONT_FAMILY)
         if font:
             # spaces in the family name need to be escaped
             font["family"] = font["family"].replace(" ", "\ ")
             font_str = "%(family)s %(size)i %(weight)s %(slant)s" % font
             if font["underline"]:
                 font_str += " underline"
             if font["overstrike"]:
```

### Comparing `tkfontselector-1.0.5/tkfontselector/ask_font.py` & `tkfontselector-1.0.6/tkfontselector/ask_font.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,40 @@
 
 
 def ask_font(
     master: Union[Tk, Toplevel, None] = None,
     text: str = "Abcd",
     title: str = "Font Selector",
     fixed_only: bool = False,
-    **font_args
+    families_only: bool = False,
+    font_args: dict = {},
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
         fixed_only: bool
             Display fixed only families
+        families_only: bool
+            Will only display Families part of the UI
+        font_dict: dict
+            dictionary, like the one returned by the ``actual`` method of a ``Font`` object:
+                {'family': str,
+                    'size': int,
+                    'weight': 'bold'/'normal',
+                    'slant': 'italic'/'roman',
+                    'underline': bool,
+                    'overstrike': bool}
+        kwargs: dict
 
     Font arguments:
         family: str
             font family
         size: int
             font size
         slant: str
@@ -44,10 +56,10 @@
              'size': int,
              'weight': 'bold'/'normal',
              'slant': 'italic'/'roman',
              'underline': bool,
              'overstrike': bool}
 
     """
-    chooser = FontSelector(master, font_args, text, title, fixed_only)
+    chooser = FontSelector(master, text, title, fixed_only, families_only, font_args)
     chooser.wait_window(chooser)
     return chooser.get_res()
```

### Comparing `tkfontselector-1.0.5/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.6/tkfontselector/tkfontselector.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,37 +23,42 @@
 
 class FontSelector(Toplevel):
     """Font Selector dialog."""
 
     def __init__(
         self,
         master: Union[Tk, Toplevel] = None,
-        font_dict: dict = {},
         text: str = "Abcd",
         title: str = "Font Selector",
         fixed_only: bool = False,
+        families_only: bool = False,
+        font_dict: dict = {},
         **kwargs
     ):
         """
         Create a new FontSelector instance.
         Arguments:
             master: Tk or Toplevel instance
                 master window
+            text: str
+                text to be displayed in the preview label
+            title: str
+                window title
+            fixed_only: bool
+                will display fixed (mono spaced) fonts only
+            families_only: bool
+                will only display the family part of the UI
             font_dict: dict
                 dictionary, like the one returned by the ``actual`` method of a ``Font`` object:
                     {'family': str,
                      'size': int,
                      'weight': 'bold'/'normal',
                      'slant': 'italic'/'roman',
                      'underline': bool,
                      'overstrike': bool}
-            text: str
-                text to be displayed in the preview label
-            title: str
-                window title
             kwargs: dict
                 additional keyword arguments to be passed to ``Toplevel.__init__``
         """
         super().__init__(master, **kwargs)
         self.title(title)
         self.protocol("WM_DELETE_WINDOW", self.quit)
         self._validate_family = self.register(self.validate_font_family)
@@ -85,59 +90,59 @@
         font_dict["underline"] = font_dict.get("underline", False)
         font_dict["overstrike"] = font_dict.get("overstrike", False)
         font_dict["family"] = font_dict.get("family", self.fonts[0].replace("\ ", " "))
         font_dict["size"] = font_dict.get("size", 10)
 
         # --- creation of the widgets
         # ------ style parameters (bold, italic ...)
-        options_frame = Frame(self, relief="groove", borderwidth=2)
+        self.options_frame = Frame(self, relief="groove", borderwidth=2)
         self.font_family = StringVar(self, " ".join(self.fonts))
         self.font_size = StringVar(self, " ".join(self.sizes))
         self.var_bold = BooleanVar(self, font_dict["weight"] == "bold")
         b_bold = Checkbutton(
-            options_frame,
+            self.options_frame,
             text=TR["Bold"],
             command=self.toggle_bold,
             variable=self.var_bold,
         )
         b_bold.grid(row=0, sticky="w", padx=4, pady=(4, 2))
         self.var_italic = BooleanVar(self, font_dict["slant"] == "italic")
         b_italic = Checkbutton(
-            options_frame,
+            self.options_frame,
             text=TR["Italic"],
             command=self.toggle_italic,
             variable=self.var_italic,
         )
         b_italic.grid(row=1, sticky="w", padx=4, pady=2)
         self.var_underline = BooleanVar(self, font_dict["underline"])
         b_underline = Checkbutton(
-            options_frame,
+            self.options_frame,
             text=TR["Underline"],
             command=self.toggle_underline,
             variable=self.var_underline,
         )
         b_underline.grid(row=2, sticky="w", padx=4, pady=2)
         self.var_overstrike = BooleanVar(self, font_dict["overstrike"])
         b_overstrike = Checkbutton(
-            options_frame,
+            self.options_frame,
             text=TR["Overstrike"],
             variable=self.var_overstrike,
             command=self.toggle_overstrike,
         )
         b_overstrike.grid(row=3, sticky="w", padx=4, pady=(2, 4))
         # ------ Size and family
         self.var_size = StringVar(self)
         self.entry_family = Entry(
             self,
             validate="key",
             validatecommand=(self._validate_family, "%d", "%S", "%i", "%s", "%V"),
         )
         self.entry_size = Entry(
             self,
-            width=4,
+            width=8,
             validate="key",
             textvariable=self.var_size,
             validatecommand=(self._validate_size, "%d", "%P", "%V"),
         )
         self.list_family = Listbox(
             self,
             selectmode="browse",
@@ -147,34 +152,37 @@
         )
         self.list_size = Listbox(
             self,
             selectmode="browse",
             listvariable=self.font_size,
             highlightthickness=0,
             exportselection=False,
+            width=8,
         )
-        scroll_family = Scrollbar(
+        self.scroll_family = Scrollbar(
             self, orient="vertical", command=self.list_family.yview
         )
-        scroll_size = Scrollbar(self, orient="vertical", command=self.list_size.yview)
+        self.scroll_size = Scrollbar(
+            self, orient="vertical", command=self.list_size.yview
+        )
         self.preview_font = Font(self, **font_dict)
         if len(text) > 30:
             text = text[:30]
         self.preview = Label(
             self,
             relief="groove",
             style="prev.TLabel",
             text=text,
             font=self.preview_font,
             anchor="center",
         )
 
         # --- widget configuration
-        self.list_family.configure(yscrollcommand=scroll_family.set)
-        self.list_size.configure(yscrollcommand=scroll_size.set)
+        self.list_family.configure(yscrollcommand=self.scroll_family.set)
+        self.list_size.configure(yscrollcommand=self.scroll_size.set)
 
         self.entry_family.insert(0, font_dict["family"])
         self.entry_family.selection_clear()
         self.entry_family.icursor("end")
         self.entry_size.insert(0, font_dict["size"])
 
         try:
@@ -190,27 +198,18 @@
             self.list_size.selection_clear(0, "end")
             self.list_size.selection_set(i)
             self.list_size.see(i)
         except ValueError:
             # size not in list
             pass
 
-        self.entry_family.grid(
-            row=0, column=0, columnspan=2, sticky="ews", pady=(10, 1), padx=(10, 0)
-        )
-        self.entry_size.grid(row=0, column=2, columnspan=2, sticky="ews", pady=(10, 1), padx=(10, 0))
-        self.list_family.grid(
-            row=1, column=0, sticky="nsew", pady=(1, 10), padx=(10, 0)
-        )
-        self.list_size.grid(row=1, column=2, sticky="nsew", pady=(1, 10), padx=(10, 0))
-        scroll_family.grid(row=1, column=1, sticky="nsw", pady=(1, 10))
-        scroll_size.grid(row=1, column=3, sticky="nsw", pady=(1, 10))
-        options_frame.grid(
-            row=0, column=4, rowspan=2, padx=10, pady=10, ipadx=10, sticky="nsew"
-        )
+        if families_only:
+            self._families_only()
+        else:
+            self._full_ui()
 
         self.preview.grid(
             row=2,
             column=0,
             columnspan=5,
             sticky="eswn",
             padx=10,
@@ -245,14 +244,42 @@
         self.bind_class("TEntry", "<Control-a>", self.select_all)
 
         self.wait_visibility(self)
         self.grab_set()
         self.entry_family.focus_set()
         self.lift()
 
+    def _families_only(self):
+        self.entry_family.grid(
+            row=0, column=0, columnspan=4, sticky="ews", pady=(10, 1), padx=(10, 10)
+        )
+        self.list_family.grid(
+            row=1, column=0, columnspan=3, sticky="nsew", pady=(1, 10), padx=(10, 0)
+        )
+        self.scroll_family.grid(
+            row=1, column=3, sticky="nsw", pady=(1, 10), padx=(0, 10)
+        )
+
+    def _full_ui(self):
+        self.entry_family.grid(
+            row=0, column=0, columnspan=2, sticky="ews", pady=(10, 1), padx=(10, 0)
+        )
+        self.entry_size.grid(
+            row=0, column=2, columnspan=2, sticky="ews", pady=(10, 1), padx=(10, 0)
+        )
+        self.list_family.grid(
+            row=1, column=0, sticky="nsew", pady=(1, 10), padx=(10, 0)
+        )
+        self.list_size.grid(row=1, column=2, sticky="nsew", pady=(1, 10), padx=(10, 0))
+        self.scroll_family.grid(row=1, column=1, sticky="nsw", pady=(1, 10))
+        self.scroll_size.grid(row=1, column=3, sticky="nsw", pady=(1, 10))
+        self.options_frame.grid(
+            row=0, column=4, rowspan=2, padx=10, pady=10, ipadx=10, sticky="nsew"
+        )
+
     def select_all(self, event):
         """Select all entry content."""
         event.widget.selection_range(0, "end")
 
     def keypress(self, event):
         """Select the first font whose name begin by the key pressed."""
         key = event.char.lower()
```

### Comparing `tkfontselector-1.0.5/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.6/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.5/PKG-INFO` & `tkfontselector-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -68,22 +68,24 @@
     'overstrike': bool}
 ```
 
 ## General arguments
 
 `master`: Tk, Toplevel, or None (Optional)
 
-`font_dict`: dict (Optional) _font dictionary like an actual Font object_
-
 `text`: str (Optional) _text to show in the font selection window_
 
 `title`: str (Optional) _changes the title of the window_
 
 `fixed_only`: bool (Optional), _if set to `True` will only show `Fixed (mono spaced)` fonts_
 
+`families_only`: bool (Optional), _if set to `True` will only show Font Families part of the UI_
+
+`font_dict`: dict (Optional) _font dictionary like an actual Font object_
+
 `**kwargs`: (Optional) _pass any other args that might be accepted_
 
 ## Font Arguments
 
 `family`: str
 
 `size`: int
@@ -95,14 +97,25 @@
 `underline`: bool
 
 `overstrike`: bool
 
 ## Example
 
 ```python
+EXAMPLE_FONT_FAMILY = {
+    "family": "Comic Sans MS",
+    "size": 10,
+    "weight": "normal",
+    "slant": "roman",
+    "underline": 0,
+    "overstrike": 0,
+}
+
+
+if __name__ == "__main__":
     """Example Usage"""
     root = Tk()
     style = ttk.Style(root)
     if "win" == platform[:3]:
         style.theme_use("vista")
     elif "darwin" in platform:
         style.theme_use("clam")
@@ -110,15 +123,15 @@
         style.theme_use("clam")
     bg = style.lookup("TLabel", "background")
     root.configure(bg=bg)
     label = ttk.Label(root, text="Chosen font: ")
     label.pack(padx=10, pady=(10, 4))
 
     def callback():
-        font = ask_font(root, title="Choose a font")
+        font = ask_font(root, title="Choose a font", font_args=EXAMPLE_FONT_FAMILY)
         if font:
             # spaces in the family name need to be escaped
             font["family"] = font["family"].replace(" ", "\ ")
             font_str = "%(family)s %(size)i %(weight)s %(slant)s" % font
             if font["underline"]:
                 font_str += " underline"
             if font["overstrike"]:
```

