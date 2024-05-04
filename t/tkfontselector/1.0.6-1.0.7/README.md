# Comparing `tmp/tkfontselector-1.0.6.tar.gz` & `tmp/tkfontselector-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.6.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.7.tar", max compression
```

## Comparing `tkfontselector-1.0.6.tar` & `tkfontselector-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-04 04:26:34.871849 tkfontselector-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.6/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.6/tkfontselector/__init__.py
--rw-r--r--   0        0        0     2035 2024-05-04 04:24:14.225463 tkfontselector-1.0.6/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    19274 2024-05-04 04:29:03.193623 tkfontselector-1.0.6/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.6/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-04 05:48:07.718543 tkfontselector-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3244 2024-05-04 04:26:16.286001 tkfontselector-1.0.7/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.7/tkfontselector/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-04 04:24:14.225463 tkfontselector-1.0.7/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    19933 2024-05-04 05:47:17.178753 tkfontselector-1.0.7/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.7/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 tkfontselector-1.0.7/PKG-INFO
```

### Comparing `tkfontselector-1.0.6/LICENSE.txt` & `tkfontselector-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.6/pyproject.toml` & `tkfontselector-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.6"
+version = "1.0.7"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.6/README.md` & `tkfontselector-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.6/tkfontselector/ask_font.py` & `tkfontselector-1.0.7/tkfontselector/ask_font.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.6/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.7/tkfontselector/tkfontselector.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         self.grid_columnconfigure((0, 2), weight=1)
         self.grid_rowconfigure(0, weight=1)
         self.grid_rowconfigure(1, weight=500)
 
         # --- variable storing the chosen font
         self.res = ""
 
-        style = Style(self)
-        style.configure("prev.TLabel", background="white")
+        self.style = Style(self)
+        self.style.configure("prev.TLabel", background="white")
 
         # --- family list
         if fixed_only:
             self.fonts = self._get_fixed_families()
         else:
             self.fonts = self._get_non_fixed_families()
         self.fonts.append("TkDefaultFont")
@@ -86,53 +86,53 @@
         self.sizes = ["%i" % i for i in (list(range(6, 17)) + list(range(18, 32, 2)))]
         # --- font default
         font_dict["weight"] = font_dict.get("weight", "normal")
         font_dict["slant"] = font_dict.get("slant", "roman")
         font_dict["underline"] = font_dict.get("underline", False)
         font_dict["overstrike"] = font_dict.get("overstrike", False)
         font_dict["family"] = font_dict.get("family", self.fonts[0].replace("\ ", " "))
-        font_dict["size"] = font_dict.get("size", 10)
+        self.passed_size = font_dict["size"] = font_dict.get("size", 10)
 
         # --- creation of the widgets
         # ------ style parameters (bold, italic ...)
         self.options_frame = Frame(self, relief="groove", borderwidth=2)
         self.font_family = StringVar(self, " ".join(self.fonts))
         self.font_size = StringVar(self, " ".join(self.sizes))
         self.var_bold = BooleanVar(self, font_dict["weight"] == "bold")
-        b_bold = Checkbutton(
+        self.b_bold = Checkbutton(
             self.options_frame,
             text=TR["Bold"],
             command=self.toggle_bold,
             variable=self.var_bold,
         )
-        b_bold.grid(row=0, sticky="w", padx=4, pady=(4, 2))
+        self.b_bold.grid(row=0, sticky="w", padx=4, pady=(4, 2))
         self.var_italic = BooleanVar(self, font_dict["slant"] == "italic")
-        b_italic = Checkbutton(
+        self.b_italic = Checkbutton(
             self.options_frame,
             text=TR["Italic"],
             command=self.toggle_italic,
             variable=self.var_italic,
         )
-        b_italic.grid(row=1, sticky="w", padx=4, pady=2)
+        self.b_italic.grid(row=1, sticky="w", padx=4, pady=2)
         self.var_underline = BooleanVar(self, font_dict["underline"])
-        b_underline = Checkbutton(
+        self.b_underline = Checkbutton(
             self.options_frame,
             text=TR["Underline"],
             command=self.toggle_underline,
             variable=self.var_underline,
         )
-        b_underline.grid(row=2, sticky="w", padx=4, pady=2)
+        self.b_underline.grid(row=2, sticky="w", padx=4, pady=2)
         self.var_overstrike = BooleanVar(self, font_dict["overstrike"])
-        b_overstrike = Checkbutton(
+        self.b_overstrike = Checkbutton(
             self.options_frame,
             text=TR["Overstrike"],
             variable=self.var_overstrike,
             command=self.toggle_overstrike,
         )
-        b_overstrike.grid(row=3, sticky="w", padx=4, pady=(2, 4))
+        self.b_overstrike.grid(row=3, sticky="w", padx=4, pady=(2, 4))
         # ------ Size and family
         self.var_size = StringVar(self)
         self.entry_family = Entry(
             self,
             validate="key",
             validatecommand=(self._validate_family, "%d", "%S", "%i", "%s", "%V"),
         )
@@ -217,20 +217,18 @@
             ipadx=4,
             ipady=4,
         )
 
         button_frame = Frame(self)
         button_frame.grid(row=3, column=0, columnspan=5, pady=(0, 10), padx=10)
 
-        Button(button_frame, text="Ok", command=self.ok).grid(
-            row=0, column=0, padx=14, sticky="ew"
-        )
-        Button(button_frame, text=TR["Cancel"], command=self.quit).grid(
-            row=0, column=1, padx=14, sticky="ew"
-        )
+        self.okay_btn = Button(button_frame, text="Ok", command=self.ok)
+        self.okay_btn.grid(row=0, column=0, padx=14, sticky="ew")
+        self.cancel_btn = Button(button_frame, text=TR["Cancel"], command=self.quit)
+        self.cancel_btn.grid(row=0, column=1, padx=14, sticky="ew")
         self.list_family.bind("<<ListboxSelect>>", self.update_entry_family)
         self.list_size.bind("<<ListboxSelect>>", self.update_entry_size, add=True)
         self.list_family.bind("<KeyPress>", self.keypress)
         self.entry_family.bind("<Return>", self.change_font_family)
         self.entry_family.bind("<Tab>", self.tab)
         self.entry_size.bind("<Return>", self.change_font_size)
 
@@ -239,19 +237,37 @@
 
         self.entry_family.bind("<Up>", self.up_family)
         self.entry_size.bind("<Up>", self.up_size)
 
         # bind Ctrl+A to select all instead of go to beginning
         self.bind_class("TEntry", "<Control-a>", self.select_all)
 
+        self._update_widget_font_sizes()
+
         self.wait_visibility(self)
         self.grab_set()
         self.entry_family.focus_set()
         self.lift()
 
+    def _update_widget_font_sizes(self):
+        self._update_tk_widget_font_size()
+        self._update_ttk_widget_font_size()
+
+    def _update_tk_widget_font_size(self):
+        for widget in (
+            self.entry_family,
+            self.entry_size,
+            self.list_family,
+            self.list_size,
+        ):
+            widget.configure(font=(None, self.passed_size))
+
+    def _update_ttk_widget_font_size(self):
+        self.style.configure(".", font=(None, self.passed_size))
+
     def _families_only(self):
         self.entry_family.grid(
             row=0, column=0, columnspan=4, sticky="ews", pady=(10, 1), padx=(10, 10)
         )
         self.list_family.grid(
             row=1, column=0, columnspan=3, sticky="nsew", pady=(1, 10), padx=(10, 0)
         )
```

### Comparing `tkfontselector-1.0.6/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.7/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.6/PKG-INFO` & `tkfontselector-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

