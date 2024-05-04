# Comparing `tmp/wlr_layout_ui-1.6.8.tar.gz` & `tmp/wlr_layout_ui-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.6.8.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.6.9.tar", max compression
```

## Comparing `wlr_layout_ui-1.6.8.tar` & `wlr_layout_ui-1.6.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.8/LICENSE
--rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.8/README.md
--rw-r--r--   0        0        0      652 2024-05-03 20:54:30.131844 wlr_layout_ui-1.6.8/pyproject.toml
--rw-r--r--   0        0        0     2934 2024-05-02 18:21:25.240782 wlr_layout_ui-1.6.8/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4331 2024-05-03 20:51:33.641760 wlr_layout_ui-1.6.8/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.8/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    25016 2024-05-01 21:28:43.369353 wlr_layout_ui-1.6.8/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.8/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5575 2024-05-02 18:28:00.450250 wlr_layout_ui-1.6.8/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.8/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.8/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4529 2024-05-01 17:21:39.484459 wlr_layout_ui-1.6.8/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.8/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.9/LICENSE
+-rw-r--r--   0        0        0     1318 2024-05-04 11:28:23.880948 wlr_layout_ui-1.6.9/README.md
+-rw-r--r--   0        0        0      652 2024-05-04 11:30:52.297224 wlr_layout_ui-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2934 2024-05-02 18:21:25.240782 wlr_layout_ui-1.6.9/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4484 2024-05-03 21:48:54.542765 wlr_layout_ui-1.6.9/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.9/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    24937 2024-05-03 21:53:52.385793 wlr_layout_ui-1.6.9/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.9/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5575 2024-05-02 18:28:00.450250 wlr_layout_ui-1.6.9/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.9/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.9/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4848 2024-05-03 21:31:37.151204 wlr_layout_ui-1.6.9/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12998 2024-05-01 18:51:08.232951 wlr_layout_ui-1.6.9/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.9/PKG-INFO
```

### Comparing `wlr_layout_ui-1.6.8/LICENSE` & `wlr_layout_ui-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.8/pyproject.toml` & `wlr_layout_ui-1.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.6.8"
+version = "1.6.9"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/displaywidget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import random
 
-import pyglet
 from pyglet.shapes import BorderedRectangle
 from pyglet.text import Label
 
 from .screens import Screen
-from .utils import Rect, brighten
+from .utils import Rect, brighten, simplify_model_name
 from .widgets import Widget
 
 ANIMATION_LENGTH = 8
 
 
+def limit_size(text):
+    if len(text) > 15:
+        return text[:12] + "..."
+    return text
+
+
 class GuiScreen(Widget):
     def __repr__(self):
         return "<Screen %s (%s) - %s>" % (self.rect, self.color, self.screen.name)
 
     __str__ = __repr__
 
     all_colors: tuple[tuple[int, int, int], ...] = (
@@ -113,38 +118,38 @@
             border=9 if self.highlighted else 2,
             color=color,
             border_color=border_color,
         ).draw()
         # Render the screen uid as text
         tx, ty = self.rect.center
         Label(
-            self.screen.uid,
+            limit_size(simplify_model_name(self.screen.name)),
             anchor_x="center",
             anchor_y="center",
             x=tx,
             y=ty,
             font_size=16,
             color=(240, 240, 240, 255),
         ).draw()
 
         # Second caption line
         if self.screen.active:
             assert self.screen.mode
-            label = f"{self.screen.mode.width}x{self.screen.mode.height}"
+            label = f"{self.screen.mode.width}x{self.screen.mode.height}@{int(self.screen.mode.freq)}"
             Label(
-                label,
+                self.screen.uid,
                 anchor_x="center",
                 anchor_y="center",
                 x=tx,
                 y=ty + 20,
                 color=txt_color,
                 bold=self.screen.active,
             ).draw()
             Label(
-                f"{self.screen.mode.freq}Hz",
+                label,
                 anchor_x="center",
                 anchor_y="center",
                 x=tx,
                 y=ty - 20,
                 color=txt_color,
                 bold=self.screen.active,
             ).draw()
```

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     UI_RATIO,
     WINDOW_MARGIN,
     reload_pre_commands,
 )
 from .utils import (
     Rect,
     compute_bounding_box,
+    simplify_model_name,
     config,
     find_matching_mode,
     make_command,
     sorted_frequencies,
     sorted_resolutions,
     trim_rects_flip_y,
 )
 from .widgets import Button, Dropdown, HBox, Style, VBox, Widget, Spacer
 
-hex_re = re.compile("^[0-9x]+$")
 
 CONFIRM_DELAY = 20
 
 
 def get_closest_match(float_list, value):
     return min(float_list, key=lambda x: abs(x - value))
 
@@ -137,31 +137,32 @@
             ref_rect.copy(),
             label="Rate",
             options=[],
             onchange=self.action_update_mode,
             # invert=True,
         )
 
+        ref_rect.width = but_w
         self.rotation = Dropdown(
             ref_rect.copy(),
-            label="Rotation",
+            label="Transform",
             options=[
-                {"name": "0", "value": 0},
-                {"name": "90", "value": 1},
-                {"name": "180", "value": 2},
-                {"name": "270", "value": 3},
+                {"name": "original", "value": 0},
+                {"name": "rot 90°", "value": 1},
+                {"name": "rot 180°", "value": 2},
+                {"name": "rot 270°", "value": 3},
                 {"name": "flip", "value": 4},
-                {"name": "flip 90", "value": 5},
-                {"name": "flip 180", "value": 6},
-                {"name": "flip 270", "value": 7},
+                {"name": "rot 90° flip", "value": 5},
+                {"name": "rot 180° flip", "value": 6},
+                {"name": "rot 270° flip", "value": 7},
             ],
             onchange=self.action_update_rotation,
             # invert=True,
         )
-        ref_rect.width = int(ref_rect.width * 0.8)
+        ref_rect.width = but_w // 1.5
         self.scale_ratio = Dropdown(
             ref_rect.copy(),
             label="Scale",
             options=[
                 {"name": "100%", "value": 1},
                 {"name": "90%", "value": 0.833333},
                 {"name": "80%", "value": 0.666667},
@@ -366,19 +367,15 @@
 
     # }}}
     # Gui getters & properties  {{{
     def get_status_text(self):
         if self.text_input is not None:
             return f'Press ENTER to validate "{self.text_input}"'
         elif self.selected_item:
-            words = []
-            for word in self.selected_item.screen.name.split():
-                if not hex_re.match(word):
-                    words.append(word)
-            return " ".join(words)
+            return simplify_model_name(self.selected_item.screen.name)
         else:
             return "Select a monitor to edit its settings"
 
     # }}}
     # Event handler methods {{{
     def on_text(self, text):
         if self.text_input is not None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/screens.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,24 @@
+import re
 from dataclasses import dataclass
 
 config = {"hyprland": False}
 
+hex_re = re.compile("^[0-9x]+$")
+
+
+def simplify_model_name(name):
+    words = []
+    for word in name.split():
+        if not hex_re.match(word):
+            words.append(word)
+    # remove duplicate words keeping order (comparing lowercase)
+    words = list(dict.fromkeys(words))
+    return " ".join(words)
+
 
 def make_command(screens, rects, wayland=True):
     if wayland and config.get("hyprland"):
         return make_command_hyprland(screens, rects)
     return make_command_legacy(screens, rects, wayland)
```

### Comparing `wlr_layout_ui-1.6.8/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.6.9/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.8/PKG-INFO` & `wlr_layout_ui-1.6.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.6.8
+Version: 1.6.9
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,32 +22,50 @@
 # Wlr layout UI
 
 An simple GUI to setup the screens layout on wlroots based systems and X11 (using xrandr), Hyprland is the first class user.
 
 ## Features
 
 - Load and save profiles
+- No grid snapping, but anchors in a smart way on overlap
 - Set the screen settings
-  - Layout: position, rotation and scale
+  - Layout: position, rotation, scale and flipping
   - Resolution
   - Refresh rate
+- Makes clean, easy to understand layouts, with no negative values of random offsets `</monk>`
 
 > [!note]
 > Non Hyprland should work without screen rotation or scaling support
 
 ## Video / Demo
 
 A bit outdated, but still relevant.
 
 [![Video](https://img.youtube.com/vi/bJxVIu9cMzg/0.jpg)](https://www.youtube.com/watch?v=bJxVIu9cMzg)
 
 ## Requires
 
 - wlr-randr (if not using Hyprland >= 0.37)
-- Python: pyglet, tomli
+- Python: pyglet, tomli, tomli-w
+
+## Installation
+
+### Archlinux
+
+`yay wlr-layout-ui-git`
+
+### Other distros
+
+```
+python -m venv myenv
+./myenv/bin/pip install wlr-layout-ui
+```
+
+This will create a "myenv" folder with the app installed.
+You will need to run the app with the full path to it.
 
 ## Usage
 
 ### Start the GUI
 
 ```
 wlrlui
```

