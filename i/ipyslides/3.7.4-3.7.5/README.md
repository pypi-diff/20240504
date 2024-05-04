# Comparing `tmp/ipyslides-3.7.4.tar.gz` & `tmp/ipyslides-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.7.4.tar", last modified: Thu May  2 19:50:55 2024, max compression
+gzip compressed data, was "ipyslides-3.7.5.tar", last modified: Sat May  4 01:25:45 2024, max compression
```

## Comparing `ipyslides-3.7.4.tar` & `ipyslides-3.7.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.851592 ipyslides-3.7.4/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.7.4/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-02 19:50:55.850591 ipyslides-3.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.811317 ipyslides-3.7.4/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.7.4/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-02 18:51:45.000000 ipyslides-3.7.4/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.844320 ipyslides-3.7.4/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.7.4/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    40549 2024-05-02 17:36:10.000000 ipyslides-3.7.4/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.7.4/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    32956 2024-05-02 18:42:52.000000 ipyslides-3.7.4/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.7.4/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.7.4/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    11523 2024-05-02 17:07:46.000000 ipyslides-3.7.4/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.7.4/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.844320 ipyslides-3.7.4/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.7.4/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.7.4/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.7.4/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.7.4/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.7.4/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    22978 2024-05-02 19:12:44.000000 ipyslides-3.7.4/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28848 2024-05-02 18:42:52.000000 ipyslides-3.7.4/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28254 2024-03-06 23:50:13.000000 ipyslides-3.7.4/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15531 2024-05-02 19:13:37.000000 ipyslides-3.7.4/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.7.4/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    49800 2024-05-02 19:49:43.000000 ipyslides-3.7.4/ipyslides/core.py
--rw-rw-rw-   0        0        0    17494 2024-02-24 17:41:41.000000 ipyslides-3.7.4/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.7.4/ipyslides/source.py
--rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.7.4/ipyslides/utils.py
--rw-rw-rw-   0        0        0    13884 2024-03-09 15:23:53.000000 ipyslides-3.7.4/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.7.4/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.832824 ipyslides-3.7.4/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 19:50:55.851592 ipyslides-3.7.4/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:25:45.264321 ipyslides-3.7.5/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.7.5/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-04 01:25:45.263319 ipyslides-3.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.7.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 01:25:45.222808 ipyslides-3.7.5/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.7.5/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-04 01:17:54.000000 ipyslides-3.7.5/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:25:45.259379 ipyslides-3.7.5/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.7.5/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41172 2024-05-04 01:13:38.000000 ipyslides-3.7.5/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.7.5/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    32956 2024-05-02 18:42:52.000000 ipyslides-3.7.5/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.7.5/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.7.5/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-03 23:26:00.000000 ipyslides-3.7.5/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.7.5/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:25:45.262339 ipyslides-3.7.5/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.7.5/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.7.5/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.7.5/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.7.5/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.7.5/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    21960 2024-05-04 00:50:24.000000 ipyslides-3.7.5/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28848 2024-05-02 18:42:52.000000 ipyslides-3.7.5/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28254 2024-03-06 23:50:13.000000 ipyslides-3.7.5/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15593 2024-05-03 23:26:48.000000 ipyslides-3.7.5/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.7.5/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    49083 2024-05-04 01:11:39.000000 ipyslides-3.7.5/ipyslides/core.py
+-rw-rw-rw-   0        0        0    17494 2024-02-24 17:41:41.000000 ipyslides-3.7.5/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.7.5/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.7.5/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    13884 2024-03-09 15:23:53.000000 ipyslides-3.7.5/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.7.5/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-04 01:25:45.242838 ipyslides-3.7.5/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-04 01:25:44.000000 ipyslides-3.7.5/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-04 01:25:45.000000 ipyslides-3.7.5/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 01:25:44.000000 ipyslides-3.7.5/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-04 01:25:44.000000 ipyslides-3.7.5/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 01:25:44.000000 ipyslides-3.7.5/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 01:25:45.264321 ipyslides-3.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.7.5/setup.py
```

### Comparing `ipyslides-3.7.4/LICENSE` & `ipyslides-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/PKG-INFO` & `ipyslides-3.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.7.4
+Version: 3.7.5
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.7.4/README.md` & `ipyslides-3.7.5/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/_layout_css.py` & `ipyslides-3.7.5/ipyslides/_base/_layout_css.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,18 +662,34 @@
                 ).css,
             },
             ".Source-Btn": {
                 ".fa.fa-plus": Icon(
                     "code", color=accent_color, size=_icons_size
                 ).css,
             },
+            ".Home-Btn": {
+                ".fa.fa-plus": Icon(
+                    "arrow-bar", color=accent_color, size=_icons_size, rotation=180,
+                ).css,
+            },
+            ".End-Btn": {
+                ".fa.fa-plus": Icon(
+                    "arrow-bar", color=accent_color, size=_icons_size
+                ).css,
+            },
+            ".Info-Btn": {
+                ".fa.fa-plus": Icon(
+                    "info", color=accent_color, size=_icons_size,
+                ).css,
+            },
             "<.Scroll-Btn": { # top level
                 "color": "var(--jp-brand-color1,skyblue) !important",
                 "background": "transparent !important",
-                "^:hover": {"font-weight": "bold !important",},
+                "font-size": "0.8em !important",
+                "^:hover": {"font-weight": "bold !important","font-size": "0.9em !important",},
                 "^:hover, ^:focus, ^:active, ^.mod-active" : {
                     "box-shadow": "none !important",
                     "outline": "none !important",
                 },
             },
             "@media print": { # Needs modification
                 ".SlidesWrapper": {
```

### Comparing `ipyslides-3.7.4/ipyslides/_base/_widgets.py` & `ipyslides-3.7.5/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/base.py` & `ipyslides-3.7.5/ipyslides/_base/base.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/export_html.py` & `ipyslides-3.7.5/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/export_template.py` & `ipyslides-3.7.5/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/icons.py` & `ipyslides-3.7.5/ipyslides/_base/icons.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,19 @@
             <circle stroke="none" cx="3" cy="21" r="3"/>
             <line x1="8" y1="5" x2="24" y2="5"/>
             <line x1="8" y1="13" x2="24" y2="13" />
             <line x1="8" y1="21" x2="24" y2="21"/>
         </svg>''',
     'arrow': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke="{color}" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" transform="rotate({rotation})">
-            <line x1="4" y1="13" x2="21" y2="13" />
-            <path fill="none" d="M13 4L21 13L13 21" />
+            <path fill="none" d="M13 4L21 13L13 21M4 13L21 13" />
+        </svg>''',
+    'arrow-bar': '''
+        <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke="{color}" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" transform="rotate({rotation})">
+            <path fill="none" d="M13 4L21 13L13 21M4 13L21 13M22 4L22 21"/>
         </svg>''',
     'close': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke="{color}" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" transform="rotate({rotation})">
             <line x1="4" y1="4" x2="21" y2="21" />
             <line x1="4" y1="21" x2="21" y2="4" />
         </svg>''',
     'dots': '''
@@ -79,14 +82,20 @@
                 <animateTransform attributeName="transform" type="rotate" from="0 25 25" to="360 25 25" dur="0.2s" repeatCount="indefinite"/>
             </path>
         </svg>''',
     'circle': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg">
             <circle cx="13" cy="13" r="11" fill="none" stroke="{color}" stroke-width="2"/>
         </svg>''',
+    'info': '''
+        <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg">
+            <circle cx="13" cy="13" r="11" fill="none" stroke="{color}" stroke-width="2"/>
+            <line x1="13" y1="21" x2="13" y2="12" stroke="{color}" stroke-width="5"/>
+            <circle cx="13" cy="7.5" r="3" fill="{color}" stroke="none"/>
+        </svg>''',
     'refresh': '''
         <svg height="{size}" viewBox="0 0 40 40" xmlns="http://www.w3.org/2000/svg">
             <path d=" M 37 18.8 A 17 17 4.2 1 1 32.2 8.2" stroke="{color}" stroke-width="3.5" fill="none"/>
             <path d="M36 11L30 0L24 10" fill="{color}" stroke="none"/>
         </svg>''',
     'laser': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg">
```

### Comparing `ipyslides-3.7.4/ipyslides/_base/intro.py` & `ipyslides-3.7.5/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/js/interaction.js` & `ipyslides-3.7.5/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/js/notes.js` & `ipyslides-3.7.5/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/navigation.py` & `ipyslides-3.7.5/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/notes.py` & `ipyslides-3.7.5/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/screenshot.py` & `ipyslides-3.7.5/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/settings.py` & `ipyslides-3.7.5/ipyslides/_base/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 Author Notes: Classes in this module should only be instantiated in Slides class or it's parent class
 and then provided to other classes via composition, not inheritance.
 """
 
 import os
 import math
 
-from inspect import signature
-
 from IPython.display import Image
 
 from ..formatters import fix_ipy_image, code_css
 from ..xmd import parse
 from ..utils import html, today, format_html, _sub_doc, _css_docstring
 from . import intro, styles, _layout_css
 
@@ -98,45 +96,14 @@
             "timeout": 120000 # 2 minutes
         })
 
     @property
     def widgets(self):
         return self._widgets  # To avoid breaking code by user
 
-    def set(self, **kwargs):
-        """Add multiple settings at once. keys in kwargs should be name of a function after `Slides.settings.set_`
-        and values should be dictionary or tuple of arguments for that function. See examples below.
-        ```python
-        Slides.settings.set(
-            bg_image = dict(src='image_src'),
-            css = ({},), # note trailing comma to make it tuple
-            layout = dict(scroll=True),
-        )
-        ```
-        """
-        for k, v in kwargs.items():
-            if not isinstance(v, (dict, tuple)):
-                raise TypeError(f"values in kwargs should be dict or tuple, got {v!r}")
-            func = getattr(self, f"set_{k}", False)
-            if func is False:
-                funcs = ', '.join(k for k in self.__dir__() if k.startswith('set_'))
-                raise AttributeError(f"No such function '{k}' -> 'set_{k}' in settings. Available functions are: \n{funcs}")
-            
-            # Test parameters and give hints
-            sig = signature(func)
-            param_keys = tuple(sig.parameters.keys())
-            if isinstance(v,dict):
-                for key in v.keys():
-                    if key not in param_keys:
-                        raise ValueError(f"function '{k}' -> 'set_{k}' expects these parameters: {str(sig)}")
-                    
-            func(**v) if isinstance(v, dict) else func(
-                *v
-            )  # Call function with arguments
-
     def _toggle_nav_gui(self, change):
         if change["new"]:  # It's checked then hide
             self.show_nav_gui(True)
         else:
             self.show_nav_gui(False)
 
     def _toggle_proxy_buttons(self, change):
@@ -156,53 +123,56 @@
         ):
         for name, value in ({
             'navgui': nav_gui,
             'reflow': reflow_content,
             'notes': notes,
             'toast': notifications,
             'proxy': proxy_buttons,
-            'scroll': scroll_buttons,
             'focus': auto_focus,
         }).items():
             if (widget := getattr(self.widgets.checks,name, None)):
                 widget.value = value # if condition for future additions check
+        return self # for chaining set_methods
 
     def set_animation(self, main="slide_h", frame="appear"):
         "Set animation for slides and frames."
         if len(self._slides[:]) >= 1:
             self._slides[0]._set_overall_animation(main=main, frame=frame)
         else:
             raise RuntimeError("No slides yet to set animation.")
+        return self # for chaining set_methods
 
     @_sub_doc(colors=styles.theme_colors["Light"])
     def set_theme_colors(self, colors={}):
         """Set theme colors. Only take effect when using custom theme.
         colors must be a dictionary with exactly like this:
         ```python
         Slides.settings.set_theme_colors({colors})
         ```
         """
         styles._validate_colors(colors)  # Validate colors before using and setting
         self._custom_colors = colors
         self.theme_dd.value = "Custom"  # Trigger theme update
         self._update_theme({'owner':self.theme_dd}) # This chnage is important to update layout theme as well
+        return self # for chaining set_methods
 
     @_sub_doc(css_docstring=_css_docstring)
     def set_css(self, css_dict={}):
         """Set CSS for all slides. This loads on slides navigation, so you can include keyframes animations as well.
         Individual slide's CSS set by `slides[index].set_css` will override this.
         {css_docstring}
         """
         if len(self._slides[:]) >= 1:
             self._slides[0]._set_overall_css(css_dict=css_dict)
         else:
             raise RuntimeError("No slides yet to set CSS.")
+        return self # for chaining set_methods
 
 
-    def set_bg_image(self, src, opacity=0.25, blur_radius=None):
+    def set_bg_image(self, src=None, opacity=0.25, blur_radius=None):
         "Adds glassmorphic effect to the background with image. `src` can be a url or a local image path."
         if not src:
             self.widgets.htmls.glass.value = ""  # clear
             self._bg_image = ""
             return
 
         if not os.path.isfile(src):
@@ -211,14 +181,15 @@
         self._bg_image = f"""
             <style>
                 {_layout_css.glass_css(opacity= 1 - opacity, blur_radius=blur_radius)}
             </style>
             {self._slides.image(src,width='100%')}
             <div class="Front"></div>""" # opacity of layer would be opposite to supplied
         self.widgets.htmls.glass.value = self._bg_image
+        return self # for chaining set_methods
 
     def set_code_theme(
         self,
         style="default",
         color=None,
         background=None,
         hover_color="var(--hover-bg)",
@@ -229,40 +200,43 @@
         self.widgets.htmls.hilite.value = code_css(
             style,
             color=color,
             background=background,
             lineno=lineno,
             hover_color=hover_color,
         )
+        return self # for chaining set_methods
 
     def set_font_family(self, text=None, code=None):
         "Set main fonts for text and code."
         if text:
             self._font_family["text"] = text
         if code:
             self._font_family["code"] = code
 
         self._update_theme()  # Changes Finally
+        return self # for chaining set_methods
 
-    def set_font_size(self, value, update_range=False):
+    def set_font_size(self, value = 20, update_range=False):
         """Set font scale to increase or decrease text size. 1 is default. 
         You can update min/max if value is not in [8,64] interval by setting update_range = True"""
         if (not isinstance(value, int)) or (value < 1):
             raise TypeError("font size should be positive integer")
         
         if (value < self.fontsize_slider.min) or (value > self.fontsize_slider.max):
             if not update_range:
                 raise ValueError(f"Given {value} is out of range. Use update_range = True to extend range as well")
             else:
                 self.fontsize_slider.max = max(value, self.fontsize_slider.max)
                 self.fontsize_slider.min = min(value, self.fontsize_slider.min)
         
         self.fontsize_slider.value = value
+        return self # for chaining set_methods
 
-    def set_logo(self, src, width=60, top=0, right=0):
+    def set_logo(self, src=None, width=60, top=0, right=0):
         "`src` should be PNG/JPEG file name or SVG string or None. width, top, right can be given as int or in valid CSS units, e.g. '16px'."
         if not src: # give as None, '' etc
             self.widgets.htmls.logo.value = ''
             return None
         
         kwargs = {k:v for k,v in locals().items() if k not in ('self','src')}
         for k,v in kwargs.items():
@@ -274,14 +248,15 @@
                 image = src
             else:
                 image = fix_ipy_image(
                     Image(src, width=width), width=width
                 ).value  
             self.widgets.htmls.logo.layout = dict(**kwargs, height='max-content')
             self.widgets.htmls.logo.value = image 
+        return self # for chaining set_methods
 
     def set_footer(self, text="", numbering=True, date="today"):
         "Set footer text. `text` should be string. `date` should be 'today' or string of date. To skip date, set it to None or ''"
         self._footer_kws.update({"numbering": numbering, "date": date})
         if text is None or text == "":
             self._footer_kws["text"] = ""  # assign to text
         elif text and isinstance(text, str):
@@ -289,14 +264,15 @@
         else:
             raise TypeError(f"text should be string or None, not {type(text)}")
 
         if self._slides.current:
             self.get_footer(
                 self._slides.current, update_widget=True
             )  # Update footer immediately if slide there
+        return self # for chaining set_methods
 
     def get_footer(self, slide, update_widget=False):
         "Get footer text. `slide` is a slide object."
         if (type(slide).__name__ != "Slide") and (
             type(slide).__module__.split(".")[0] != "ipyslides"
         ):
             raise TypeError(f"slide should be Slide object, not {type(slide)}")
@@ -331,14 +307,15 @@
         """
         if (not isinstance(width, int)) or (width not in range(101)):
             raise ValueError("width should be int in range [0,100]")
         if not isinstance(aspect, (int,float)):
             raise TypeError("aspect should be int/float of ratio width/height.")
         self._layout = {'cwidth':width, 'scroll': scroll, 'centered': center, 'aspect': aspect, 'ncol_refs': ncol_refs}
         self._update_size(change = None) # will reset theme and send RESCALE message
+        return self # for chaining set_methods
 
     def show_nav_gui(self, visible = True):
         """Show/Hide navigation GUI, keyboard or touch still work. Hover on left-bottom corner to acess settings."""
         self.widgets.controls.layout.visibility = "visible" if visible else "hidden"
         self.widgets.checks.navgui.value = True if visible else False
         self.widgets.iw.msg_tojs = 'RESCALE' # sets padding etc
```

### Comparing `ipyslides-3.7.4/ipyslides/_base/slide.py` & `ipyslides-3.7.5/ipyslides/_base/slide.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/styles.py` & `ipyslides-3.7.5/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/_base/widgets.py` & `ipyslides-3.7.5/ipyslides/_base/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     """
     prev    =  Button(icon='chevron-left',layout= Layout(width='auto',height='auto'),tooltip='Previous Slide [<, Shift + Space]').add_class('Arrows').add_class('Prev-Btn')
     next    =  Button(icon='chevron-right',layout= Layout(width='auto',height='auto'),tooltip='Next Slide [>, Space]').add_class('Arrows').add_class('Next-Btn')
     setting =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Open Settings [G]').add_class('Menu-Item').add_class('Settings-Btn')
     toc     =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Toggle Table of Contents').add_class('Menu-Item').add_class('Toc-Btn')
     refresh =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'),tooltip='Refresh Dynamic Content').add_class('Menu-Item').add_class('Refresh-Btn')
     source  =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Edit Source Cell [E]').add_class('Menu-Item').add_class('Source-Btn')
-    home    =  Button(description= '⇤',layout= Layout(width='auto',height='auto'), tooltip='Go to Title Page').add_class('Menu-Item')
-    end     =  Button(description= '⇥',layout= Layout(width='auto',height='auto'), tooltip='Go To End of Slides').add_class('Menu-Item')
-    info    =  Button(description= 'ℹ️',layout= Layout(width='auto',height='auto'), tooltip='Information').add_class('Menu-Item')
+    home    =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Go to Title Page').add_class('Menu-Item').add_class('Home-Btn')
+    end     =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Go To End of Slides').add_class('Menu-Item').add_class('End-Btn')
+    info    =  Button(icon='plus',layout= Layout(width='auto',height='auto'), tooltip='Information').add_class('Menu-Item').add_class('Info-Btn')
     capture =  Button(icon='camera',layout= Layout(width='auto',height='auto'),
                 tooltip='Take Screen short in full screen. Order of multiple shots in a slide is preserved! [S]',
                 ).add_class('Screenshot-Btn').add_class('Menu-Item')
     pdf     = Button(description='Save PDF',layout= Layout(width='auto',height='auto'))
     png     = Button(description='Save PNG',layout= Layout(width='auto',height='auto'))
     cap_all = Button(description='Capture All',layout= Layout(width='auto',height='auto'))
     export  = Button(description="Export to HTML",layout= Layout(width='auto',height='auto'))
@@ -218,15 +218,15 @@
         
         self.tocbox = VBox([],layout = Layout(width='30%',min_width='400px',height='0',overflow='auto')).add_class('TOC')
         
         self.slidebox = Box([
             # Slides are added here dynamically
         ],layout= Layout(min_width='100%',min_height='100%', overflow='hidden')).add_class('SlideBox') 
         
-        self.quick_menu = VBox([HBox([self.buttons.home, self.buttons.end, self.buttons.info, self.toggles.menu]),*_many_btns[::-1]],layout= dict(width='auto', height='0')).add_class('TopBar').add_class('Outside')
+        self.quick_menu = VBox([HBox([self.buttons.home, self.buttons.end, self.buttons.info, self.buttons.source, self.toggles.menu]),*_many_btns[::-1]],layout= dict(width='auto', height='0')).add_class('TopBar').add_class('Outside')
 
         def close_quick_menu(change):
             self.toggles.menu.value = False
 
         for btn in self.quick_menu.children: # All buttons should close menu
             if hasattr(btn, 'on_click'):
                 btn.on_click(close_quick_menu)
```

### Comparing `ipyslides-3.7.4/ipyslides/_demo.py` & `ipyslides-3.7.5/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/core.py` & `ipyslides-3.7.5/ipyslides/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         return output
     
     def _post_run_cell(self, result):
         self._unregister_postrun_cell() # it will be initialized from next building slides
         if result.error_before_exec or result.error_in_exec:
             return  # Do not display if there is an error
 
-        scroll_btn = ipw.Button(description= 'Scroll to Slides', icon= 'scroll').add_class('Scroll-Btn')
+        scroll_btn = ipw.Button(description= 'View Slides', icon= 'scroll').add_class('Scroll-Btn')
         
         for slide in self._slides_per_cell:
             slide._scroll_btn = scroll_btn
         
         self._slides_per_cell.clear() # empty it
         scroll_btn.on_click(lambda btn: self._box.focus()) # only need to go there, no slide switching 
         display(scroll_btn)
@@ -1084,25 +1084,28 @@
 
 class Slides:
     _version = (
         _private_instance.version
     )  # This is for initial use, and will be overwritten by property version
     __doc__ = textwrap.dedent(
         """
-    Interactive Slides in IPython Notebook. Only one instance can exist. 
-    
-    All arguments and kwargs are passed to corresponding methods in submodules, that you can tweak later as well.
+    Interactive Slides in IPython Notebook. Only one instance can exist.
+    `auto_focus` can be reset from settings and enable jumping back to slides after a cell is excuted. 
     
     To suppress unwanted print from other libraries/functions, use:
     ```python
     with slides.suppress_stdout():
         some_function_that_prints() # This will not be printed
         print('This will not be printed either')
         display('Something') # This will be printed
     ```
+    ::: note-info
+        The methods under settings starting with `Slides.settings.set_` returns settings back to enable chaining 
+        without extra typing, like `Slides.settings.set_animation().set_layout()...` .
+    
     ::: note-tip
         - Use `Slides.instance()` class method to keep older settings. `Slides()` apply default settings every time.
         - Run `slides.demo()` to see a demo of some features.
         - Run `slides.docs()` to see documentation.
         - Instructions in left settings panel are always on your fingertips.
         - Creating slides in a batch using `Slides.create` is much faster than adding them one by one.
         - In JupyterLab, right click on the slides and select `Create New View for Output` for optimized display.
@@ -1113,39 +1116,17 @@
     def instance(cls):
         "Access current instnace without changing the settings."
         return _private_instance
 
     def __new__(
         cls,
         extensions=[],
-        auto_focus = True, 
-        layout = dict(center=True, scroll=True, width=100, aspect=16/9, ncol_refs = 2),
-        footer = dict(
-            text='IPySlides | <a style="color:blue;" href="https://github.com/massgh/ipyslides">github-link</a>',
-            numbering = True, 
-            date="today",
-        ),
-        logo = dict(src=get_logo(), width=60),
-        font_family = dict(text = "Roboto", code = "var(--jp-code-font-family)"),
-        code_theme = dict(style="default",lineno=True),
-        animation = dict(main="slide_h", frame = "appear"),
-        **kwargs
-    ):
+        auto_focus = True,
+        ):
         "Returns Same instance each time after applying given settings. Encapsulation."
         instance = cls.instance()
         instance.__doc__ = cls.__doc__  # copy docstring
-        instance.extender.extend(extensions)
-        instance.settings.set(
-            layout = layout,
-            footer = footer,
-            logo = logo,
-            font_family = font_family,
-            code_theme = code_theme,
-            **kwargs
-        )
-        instance.widgets.checks.focus.value = auto_focus # after other settings
-
-        with suppress(BaseException):  # Avoid error if no slides exist
-            instance.settings.set_animation(**animation)
+        instance.extender.extend(extensions) # globally once
+        instance.widgets.checks.focus.value = auto_focus # useful
         return instance
 
     # No need to define __init__, __new__ is enough to show signature and docs
```

### Comparing `ipyslides-3.7.4/ipyslides/formatters.py` & `ipyslides-3.7.5/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/source.py` & `ipyslides-3.7.5/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/utils.py` & `ipyslides-3.7.5/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/writer.py` & `ipyslides-3.7.5/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides/xmd.py` & `ipyslides-3.7.5/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.7.5/ipyslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.7.4
+Version: 3.7.5
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.7.4/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.7.5/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.4/setup.py` & `ipyslides-3.7.5/setup.py`

 * *Files identical despite different names*

