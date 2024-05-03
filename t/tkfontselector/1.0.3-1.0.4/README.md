# Comparing `tmp/tkfontselector-1.0.3.tar.gz` & `tmp/tkfontselector-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.3.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.4.tar", max compression
```

## Comparing `tkfontselector-1.0.3.tar` & `tkfontselector-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-03 21:53:30.259261 tkfontselector-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.3/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.3/tkfontselector/__init__.py
--rw-r--r--   0        0        0       22 2024-05-03 21:53:36.027245 tkfontselector-1.0.3/tkfontselector/_version.py
--rw-r--r--   0        0        0     1507 2024-05-03 21:54:12.379453 tkfontselector-1.0.3/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    18418 2024-05-03 21:13:43.402212 tkfontselector-1.0.3/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.3/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-03 22:43:22.849760 tkfontselector-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.4/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.4/tkfontselector/__init__.py
+-rw-r--r--   0        0        0     1507 2024-05-03 21:54:12.379453 tkfontselector-1.0.4/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    18352 2024-05-03 22:42:53.380143 tkfontselector-1.0.4/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.4/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.4/PKG-INFO
```

### Comparing `tkfontselector-1.0.3/LICENSE.txt` & `tkfontselector-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.3/pyproject.toml` & `tkfontselector-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.3"
+version = "1.0.4"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.3/README.md` & `tkfontselector-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.3/tkfontselector/ask_font.py` & `tkfontselector-1.0.4/tkfontselector/ask_font.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.3/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.4/tkfontselector/tkfontselector.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,37 +51,37 @@
             title: str
                 window title
             kwargs: dict
                 additional keyword arguments to be passed to ``Toplevel.__init__``
         """
         super().__init__(master, **kwargs)
         self.title(title)
-        self.resizable(False, False)
         self.protocol("WM_DELETE_WINDOW", self.quit)
         self._validate_family = self.register(self.validate_font_family)
         self._validate_size = self.register(self.validate_font_size)
 
+        self.grid_columnconfigure((0, 2), weight=1)
+        self.grid_rowconfigure(0, weight=1)
+        self.grid_rowconfigure(1, weight=500)
+
         # --- variable storing the chosen font
         self.res = ""
 
         style = Style(self)
         style.configure("prev.TLabel", background="white")
-        bg = style.lookup("TLabel", "background")
-        self.configure(bg=bg)
 
         # --- family list
         if fixed_only:
             self.fonts = self._get_fixed_families()
         else:
             self.fonts = self._get_non_fixed_families()
         self.fonts.append("TkDefaultFont")
         self.fonts.sort()
         for i in range(len(self.fonts)):
             self.fonts[i] = self.fonts[i].replace(" ", "\ ")
-        max_length = int(2.5 * max([len(font) for font in self.fonts])) // 3
         self.sizes = ["%i" % i for i in (list(range(6, 17)) + list(range(18, 32, 2)))]
         # --- font default
         font_dict["weight"] = font_dict.get("weight", "normal")
         font_dict["slant"] = font_dict.get("slant", "roman")
         font_dict["underline"] = font_dict.get("underline", False)
         font_dict["overstrike"] = font_dict.get("overstrike", False)
         font_dict["family"] = font_dict.get("family", self.fonts[0].replace("\ ", " "))
@@ -124,15 +124,14 @@
             command=self.toggle_overstrike,
         )
         b_overstrike.grid(row=3, sticky="w", padx=4, pady=(2, 4))
         # ------ Size and family
         self.var_size = StringVar(self)
         self.entry_family = Entry(
             self,
-            width=max_length,
             validate="key",
             validatecommand=(self._validate_family, "%d", "%S", "%i", "%s", "%V"),
         )
         self.entry_size = Entry(
             self,
             width=4,
             validate="key",
@@ -141,23 +140,21 @@
         )
         self.list_family = Listbox(
             self,
             selectmode="browse",
             listvariable=self.font_family,
             highlightthickness=0,
             exportselection=False,
-            width=max_length,
         )
         self.list_size = Listbox(
             self,
             selectmode="browse",
             listvariable=self.font_size,
             highlightthickness=0,
             exportselection=False,
-            width=4,
         )
         scroll_family = Scrollbar(
             self, orient="vertical", command=self.list_family.yview
         )
         scroll_size = Scrollbar(self, orient="vertical", command=self.list_size.yview)
         self.preview_font = Font(self, **font_dict)
         if len(text) > 30:
@@ -193,23 +190,27 @@
             self.list_size.selection_clear(0, "end")
             self.list_size.selection_set(i)
             self.list_size.see(i)
         except ValueError:
             # size not in list
             pass
 
-        self.entry_family.grid(row=0, column=0, sticky="ew", pady=(10, 1), padx=(10, 0))
-        self.entry_size.grid(row=0, column=2, sticky="ew", pady=(10, 1), padx=(10, 0))
+        self.entry_family.grid(
+            row=0, column=0, sticky="ews", pady=(10, 1), padx=(10, 0)
+        )
+        self.entry_size.grid(row=0, column=2, sticky="ews", pady=(10, 1), padx=(10, 0))
         self.list_family.grid(
             row=1, column=0, sticky="nsew", pady=(1, 10), padx=(10, 0)
         )
         self.list_size.grid(row=1, column=2, sticky="nsew", pady=(1, 10), padx=(10, 0))
-        scroll_family.grid(row=1, column=1, sticky="ns", pady=(1, 10))
-        scroll_size.grid(row=1, column=3, sticky="ns", pady=(1, 10))
-        options_frame.grid(row=0, column=4, rowspan=2, padx=10, pady=10, ipadx=10)
+        scroll_family.grid(row=1, column=1, sticky="nsw", pady=(1, 10))
+        scroll_size.grid(row=1, column=3, sticky="nsw", pady=(1, 10))
+        options_frame.grid(
+            row=0, column=4, rowspan=2, padx=10, pady=10, ipadx=10, sticky="nsew"
+        )
 
         self.preview.grid(
             row=2,
             column=0,
             columnspan=5,
             sticky="eswn",
             padx=10,
@@ -218,18 +219,18 @@
             ipady=4,
         )
 
         button_frame = Frame(self)
         button_frame.grid(row=3, column=0, columnspan=5, pady=(0, 10), padx=10)
 
         Button(button_frame, text="Ok", command=self.ok).grid(
-            row=0, column=0, padx=4, sticky="ew"
+            row=0, column=0, padx=14, sticky="ew"
         )
         Button(button_frame, text=TR["Cancel"], command=self.quit).grid(
-            row=0, column=1, padx=4, sticky="ew"
+            row=0, column=1, padx=14, sticky="ew"
         )
         self.list_family.bind("<<ListboxSelect>>", self.update_entry_family)
         self.list_size.bind("<<ListboxSelect>>", self.update_entry_size, add=True)
         self.list_family.bind("<KeyPress>", self.keypress)
         self.entry_family.bind("<Return>", self.change_font_family)
         self.entry_family.bind("<Tab>", self.tab)
         self.entry_size.bind("<Return>", self.change_font_size)
```

### Comparing `tkfontselector-1.0.3/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.4/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.3/PKG-INFO` & `tkfontselector-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

