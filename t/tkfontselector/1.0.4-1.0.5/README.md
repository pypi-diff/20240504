# Comparing `tmp/tkfontselector-1.0.4.tar.gz` & `tmp/tkfontselector-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkfontselector-1.0.4.tar", max compression
+gzip compressed data, was "tkfontselector-1.0.5.tar", max compression
```

## Comparing `tkfontselector-1.0.4.tar` & `tkfontselector-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0      979 2024-05-03 22:43:22.849760 tkfontselector-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.4/README.md
--rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.4/tkfontselector/__init__.py
--rw-r--r--   0        0        0     1507 2024-05-03 21:54:12.379453 tkfontselector-1.0.4/tkfontselector/ask_font.py
--rw-r--r--   0        0        0    18352 2024-05-03 22:42:53.380143 tkfontselector-1.0.4/tkfontselector/tkfontselector.py
--rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.4/tkfontselector/translations/__init__.py
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-03 18:38:10.067204 tkfontselector-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      979 2024-05-03 23:04:13.947917 tkfontselector-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2913 2024-05-03 21:12:12.176906 tkfontselector-1.0.5/README.md
+-rw-r--r--   0        0        0       72 2024-05-03 19:02:54.386237 tkfontselector-1.0.5/tkfontselector/__init__.py
+-rw-r--r--   0        0        0     1507 2024-05-03 21:54:12.379453 tkfontselector-1.0.5/tkfontselector/ask_font.py
+-rw-r--r--   0        0        0    18380 2024-05-03 23:02:58.284107 tkfontselector-1.0.5/tkfontselector/tkfontselector.py
+-rw-r--r--   0        0        0      861 2024-05-03 20:31:18.551933 tkfontselector-1.0.5/tkfontselector/translations/__init__.py
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tkfontselector-1.0.5/PKG-INFO
```

### Comparing `tkfontselector-1.0.4/LICENSE.txt` & `tkfontselector-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.4/pyproject.toml` & `tkfontselector-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkfontselector"
-version = "1.0.4"
+version = "1.0.5"
 description = "Tkinter Font Selector"
 authors = ["jlw4049 <jlw_4049@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "tkfontselector" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tkfontselector-1.0.4/README.md` & `tkfontselector-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.4/tkfontselector/ask_font.py` & `tkfontselector-1.0.5/tkfontselector/ask_font.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.4/tkfontselector/tkfontselector.py` & `tkfontselector-1.0.5/tkfontselector/tkfontselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,17 +191,17 @@
             self.list_size.selection_set(i)
             self.list_size.see(i)
         except ValueError:
             # size not in list
             pass
 
         self.entry_family.grid(
-            row=0, column=0, sticky="ews", pady=(10, 1), padx=(10, 0)
+            row=0, column=0, columnspan=2, sticky="ews", pady=(10, 1), padx=(10, 0)
         )
-        self.entry_size.grid(row=0, column=2, sticky="ews", pady=(10, 1), padx=(10, 0))
+        self.entry_size.grid(row=0, column=2, columnspan=2, sticky="ews", pady=(10, 1), padx=(10, 0))
         self.list_family.grid(
             row=1, column=0, sticky="nsew", pady=(1, 10), padx=(10, 0)
         )
         self.list_size.grid(row=1, column=2, sticky="nsew", pady=(1, 10), padx=(10, 0))
         scroll_family.grid(row=1, column=1, sticky="nsw", pady=(1, 10))
         scroll_size.grid(row=1, column=3, sticky="nsw", pady=(1, 10))
         options_frame.grid(
```

### Comparing `tkfontselector-1.0.4/tkfontselector/translations/__init__.py` & `tkfontselector-1.0.5/tkfontselector/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `tkfontselector-1.0.4/PKG-INFO` & `tkfontselector-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkfontselector
-Version: 1.0.4
+Version: 1.0.5
 Summary: Tkinter Font Selector
 License: MIT
 Author: jlw4049
 Author-email: jlw_4049@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

