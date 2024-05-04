# Comparing `tmp/wlr_layout_ui-1.6.7.tar.gz` & `tmp/wlr_layout_ui-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.6.7.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.6.8.tar", max compression
```

## Comparing `wlr_layout_ui-1.6.7.tar` & `wlr_layout_ui-1.6.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.7/LICENSE
--rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.7/README.md
--rw-r--r--   0        0        0      652 2024-05-02 18:28:20.817396 wlr_layout_ui-1.6.7/pyproject.toml
--rw-r--r--   0        0        0     2934 2024-05-02 18:21:25.240782 wlr_layout_ui-1.6.7/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.7/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.7/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    25016 2024-05-01 21:28:43.369353 wlr_layout_ui-1.6.7/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.7/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5575 2024-05-02 18:28:00.450250 wlr_layout_ui-1.6.7/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.7/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.7/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4529 2024-05-01 17:21:39.484459 wlr_layout_ui-1.6.7/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.7/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.8/LICENSE
+-rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.8/README.md
+-rw-r--r--   0        0        0      652 2024-05-03 20:54:30.131844 wlr_layout_ui-1.6.8/pyproject.toml
+-rw-r--r--   0        0        0     2934 2024-05-02 18:21:25.240782 wlr_layout_ui-1.6.8/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4331 2024-05-03 20:51:33.641760 wlr_layout_ui-1.6.8/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.8/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    25016 2024-05-01 21:28:43.369353 wlr_layout_ui-1.6.8/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.8/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5575 2024-05-02 18:28:00.450250 wlr_layout_ui-1.6.8/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.8/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.8/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4529 2024-05-01 17:21:39.484459 wlr_layout_ui-1.6.8/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.8/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.8/PKG-INFO
```

### Comparing `wlr_layout_ui-1.6.7/LICENSE` & `wlr_layout_ui-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/README.md` & `wlr_layout_ui-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/pyproject.toml` & `wlr_layout_ui-1.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.6.7"
+version = "1.6.8"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/displaywidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from pyglet.shapes import BorderedRectangle
 from pyglet.text import Label
 
 from .screens import Screen
 from .utils import Rect, brighten
 from .widgets import Widget
 
+ANIMATION_LENGTH = 8
+
 
 class GuiScreen(Widget):
     def __repr__(self):
         return "<Screen %s (%s) - %s>" % (self.rect, self.color, self.screen.name)
 
     __str__ = __repr__
 
@@ -72,18 +74,19 @@
         for var in ("x", "y", "width", "height"):
             cv = getattr(r, var)
             tv = getattr(t, var)
             if cv != tv:
                 if abs(tv - cv) <= 1:
                     setattr(r, var, tv)
                 else:
+                    tgt = (cv * ANIMATION_LENGTH + tv) / (ANIMATION_LENGTH + 1)
                     if cv < tv:
-                        setattr(r, var, min(tv, (cv + tv) / 2))
+                        setattr(r, var, min(tv, tgt))
                     elif cv > tv:
-                        setattr(r, var, max(tv, (cv + tv) / 2))
+                        setattr(r, var, max(tv, tgt))
 
     def set_position(self, x, y):
         self.rect.x = x
         self.target_rect.x = x
         self.rect.y = y
         self.target_rect.y = y
```

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/gui.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/screens.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/utils.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.6.8/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.7/PKG-INFO` & `wlr_layout_ui-1.6.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.6.7
+Version: 1.6.8
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

