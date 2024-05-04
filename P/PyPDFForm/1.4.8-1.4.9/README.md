# Comparing `tmp/PyPDFForm-1.4.8.tar.gz` & `tmp/PyPDFForm-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.4.8.tar", last modified: Sat Feb 10 03:30:49 2024, max compression
+gzip compressed data, was "PyPDFForm-1.4.9.tar", last modified: Wed Feb 14 00:19:09 2024, max compression
```

## Comparing `PyPDFForm-1.4.8.tar` & `PyPDFForm-1.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.593141 PyPDFForm-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-10 03:30:49.593141 PyPDFForm-1.4.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.585141 PyPDFForm-1.4.8/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.589141 PyPDFForm-1.4.8/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.589141 PyPDFForm-1.4.8/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/middleware/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.593141 PyPDFForm-1.4.8/PyPDFForm/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/widgets/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.593141 PyPDFForm-1.4.8/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-10 03:30:49.000000 PyPDFForm-1.4.8/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-10 03:30:49.000000 PyPDFForm-1.4.8/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 03:30:49.000000 PyPDFForm-1.4.8/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-10 03:30:49.000000 PyPDFForm-1.4.8/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-10 03:30:49.000000 PyPDFForm-1.4.8/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 03:30:49.593141 PyPDFForm-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 03:30:49.593141 PyPDFForm-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/tests/test_create_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/tests/test_dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/tests/test_fill_max_length_text_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/tests/test_paragraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-10 03:30:34.000000 PyPDFForm-1.4.8/tests/test_preview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.414088 PyPDFForm-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-14 00:19:09.410088 PyPDFForm-1.4.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.406088 PyPDFForm-1.4.9/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.410088 PyPDFForm-1.4.9/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.410088 PyPDFForm-1.4.9/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/middleware/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.410088 PyPDFForm-1.4.9/PyPDFForm/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/widgets/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.410088 PyPDFForm-1.4.9/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-02-14 00:19:09.000000 PyPDFForm-1.4.9/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-14 00:19:09.000000 PyPDFForm-1.4.9/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 00:19:09.000000 PyPDFForm-1.4.9/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-14 00:19:09.000000 PyPDFForm-1.4.9/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 00:19:09.000000 PyPDFForm-1.4.9/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 00:19:09.414088 PyPDFForm-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:19:09.410088 PyPDFForm-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/tests/test_create_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/tests/test_dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/tests/test_fill_max_length_text_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/tests/test_paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-14 00:18:38.000000 PyPDFForm-1.4.9/tests/test_preview.py
```

### Comparing `PyPDFForm-1.4.8/LICENSE` & `PyPDFForm-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PKG-INFO` & `PyPDFForm-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.4.8
+Version: 1.4.9
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.4.8 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.4.9 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/constants.py` & `PyPDFForm-1.4.9/PyPDFForm/core/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 DEFAULT_RADIO_STYLE = "\u25CF"
 BUTTON_STYLES = {
     "4": "\u2713",
     "5": "\u00D7",
     "l": "\u25CF",
 }
 
-COORDINATE_GRID_MARGIN = 100
+COORDINATE_GRID_FONT_SIZE_MARGIN_RATIO = DEFAULT_FONT_SIZE / 100
```

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/coordinate.py` & `PyPDFForm-1.4.9/PyPDFForm/core/coordinate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from copy import deepcopy
 from typing import List, Tuple, Union
 
 from pypdf import PdfReader
 from reportlab.pdfbase.pdfmetrics import stringWidth
 
 from ..middleware.text import Text
-from .constants import (ANNOTATION_RECTANGLE_KEY, COORDINATE_GRID_MARGIN,
-                        DEFAULT_FONT, DEFAULT_FONT_SIZE)
+from .constants import (ANNOTATION_RECTANGLE_KEY,
+                        COORDINATE_GRID_FONT_SIZE_MARGIN_RATIO, DEFAULT_FONT)
 from .template import (get_char_rect_width, get_widget_alignment,
                        is_text_multiline)
 from .utils import stream_to_io
 from .watermark import create_watermarks_and_draw, merge_watermarks_with_pdf
 
 
 def get_draw_checkbox_radio_coordinates(
@@ -154,15 +154,17 @@
             result.append(get_draw_text_coordinates(widget, _widget)[0])
 
         return result
 
     return None
 
 
-def generate_coordinate_grid(pdf: bytes, color: Tuple[float, float, float]) -> bytes:
+def generate_coordinate_grid(
+    pdf: bytes, color: Tuple[float, float, float], margin: float
+) -> bytes:
     """Creates a grid view for the coordinates of a PDF."""
 
     pdf_file = PdfReader(stream_to_io(pdf))
     lines_by_page = {}
     texts_by_page = {}
     watermarks = []
 
@@ -170,42 +172,43 @@
         lines_by_page[i + 1] = []
         texts_by_page[i + 1] = []
         width = float(page.mediabox[2])
         height = float(page.mediabox[3])
 
         r, g, b = color
 
-        current = COORDINATE_GRID_MARGIN
+        current = margin
         while current < width:
             lines_by_page[i + 1].append([current, 0, current, height, r, g, b])
-            current += COORDINATE_GRID_MARGIN
+            current += margin
 
-        current = COORDINATE_GRID_MARGIN
+        current = margin
         while current < height:
             lines_by_page[i + 1].append([0, current, width, current, r, g, b])
-            current += COORDINATE_GRID_MARGIN
+            current += margin
 
-        x = COORDINATE_GRID_MARGIN
+        x = margin
         while x < width:
-            y = COORDINATE_GRID_MARGIN
+            y = margin
             while y < height:
                 value = f"({x}, {y})"
+                font_size = margin * COORDINATE_GRID_FONT_SIZE_MARGIN_RATIO
                 text = Text("new_coordinate", value)
                 text.font = DEFAULT_FONT
-                text.font_size = DEFAULT_FONT_SIZE
+                text.font_size = font_size
                 text.font_color = color
                 texts_by_page[i + 1].append(
                     [
                         text,
-                        x - stringWidth(value, DEFAULT_FONT, DEFAULT_FONT_SIZE),
-                        y - DEFAULT_FONT_SIZE,
+                        x - stringWidth(value, DEFAULT_FONT, font_size),
+                        y - font_size,
                     ]
                 )
-                y += COORDINATE_GRID_MARGIN
-            x += COORDINATE_GRID_MARGIN
+                y += margin
+            x += margin
 
     for page, lines in lines_by_page.items():
         watermarks.append(
             create_watermarks_and_draw(pdf, page, "line", lines)[page - 1]
         )
 
     result = merge_watermarks_with_pdf(pdf, watermarks)
```

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/filler.py` & `PyPDFForm-1.4.9/PyPDFForm/core/filler.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/font.py` & `PyPDFForm-1.4.9/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/image.py` & `PyPDFForm-1.4.9/PyPDFForm/core/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
     image = Image.open(buff)
 
     if image.format == "JPEG":
         buff.close()
         return image_stream
 
-    rgb_image = image.convert("RGB")
+    rgb_image = Image.new("RGB", image.size, (255, 255, 255))
+    rgb_image.paste(image, mask=image.split()[3])
+
     with BytesIO() as _file:
         rgb_image.save(_file, format="JPEG")
         _file.seek(0)
         result = _file.read()
 
     buff.close()
     return result
```

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/patterns.py` & `PyPDFForm-1.4.9/PyPDFForm/core/patterns.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/template.py` & `PyPDFForm-1.4.9/PyPDFForm/core/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/utils.py` & `PyPDFForm-1.4.9/PyPDFForm/core/utils.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/core/watermark.py` & `PyPDFForm-1.4.9/PyPDFForm/core/watermark.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/constants.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/constants.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/template.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/text.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/text.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/middleware/widget.py` & `PyPDFForm-1.4.9/PyPDFForm/middleware/widget.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/widgets/base.py` & `PyPDFForm-1.4.9/PyPDFForm/widgets/base.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/PyPDFForm/wrapper.py` & `PyPDFForm-1.4.9/PyPDFForm/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,23 +133,24 @@
                     },
                 ),
                 widget_rect_watermarks(self.read()),
             )
         )
 
     def generate_coordinate_grid(
-        self, color: Tuple[float, float, float] = (1, 0, 0)
+        self, color: Tuple[float, float, float] = (1, 0, 0), margin: float = 100
     ) -> PdfWrapper:
         """Inspects a coordinate grid of the PDF."""
 
         self.stream = generate_coordinate_grid(
             merge_watermarks_with_pdf(
                 remove_all_widgets(self.read()), widget_rect_watermarks(self.read())
             ),
             color,
+            margin,
         )
 
         return self
 
     def fill(
         self,
         data: Dict[str, Union[str, bool, int]],
```

### Comparing `PyPDFForm-1.4.8/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.4.9/PyPDFForm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.4.8
+Version: 1.4.9
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.4.8 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.4.9 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `PyPDFForm-1.4.8/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.4.9/PyPDFForm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/README.md` & `PyPDFForm-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/setup.py` & `PyPDFForm-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/tests/test_create_widget.py` & `PyPDFForm-1.4.9/tests/test_create_widget.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/tests/test_dropdown.py` & `PyPDFForm-1.4.9/tests/test_dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/tests/test_fill_max_length_text_field.py` & `PyPDFForm-1.4.9/tests/test_fill_max_length_text_field.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/tests/test_functional.py` & `PyPDFForm-1.4.9/tests/test_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,37 @@
         if os.name == "nt":
             request.config.results["expected_path"] = expected_path
             request.config.results["stream"] = obj.read()
             assert len(obj.stream) == len(expected)
             assert obj.stream == expected
 
 
+def test_draw_transparent_png_image_on_one_page(
+    template_stream, image_samples, pdf_samples, request
+):
+    expected_path = os.path.join(pdf_samples, "sample_pdf_with_transparent_png.pdf")
+    with open(expected_path, "rb+") as f:
+        obj = PdfWrapper(template_stream).draw_image(
+            os.path.join(image_samples, "sample_transparent_png.png"),
+            1,
+            100,
+            100,
+            400,
+            225,
+        )
+
+        expected = f.read()
+
+        if os.name == "nt":
+            request.config.results["expected_path"] = expected_path
+            request.config.results["stream"] = obj.read()
+            assert len(obj.stream) == len(expected)
+            assert obj.stream == expected
+
+
 def test_addition_operator_3_times(template_stream, pdf_samples, data_dict, request):
     expected_path = os.path.join(pdf_samples, "sample_added_3_copies.pdf")
     with open(expected_path, "rb+") as f:
         result = PdfWrapper()
 
         for _ in range(3):
             result += PdfWrapper(template_stream).fill(data_dict)
@@ -508,8 +531,24 @@
 
         request.config.results["expected_path"] = expected_path
         request.config.results["stream"] = obj.read()
 
         expected = f.read()
 
         assert len(obj.read()) == len(expected)
+        assert obj.stream == expected
+
+
+def test_generate_coordinate_grid_margin_50(template_stream, pdf_samples, request):
+    expected_path = os.path.join(
+        pdf_samples, "test_generate_coordinate_grid_margin_50.pdf"
+    )
+    with open(expected_path, "rb+") as f:
+        obj = PdfWrapper(template_stream).generate_coordinate_grid((1, 0, 1), margin=50)
+
+        request.config.results["expected_path"] = expected_path
+        request.config.results["stream"] = obj.read()
+
+        expected = f.read()
+
+        assert len(obj.read()) == len(expected)
         assert obj.stream == expected
```

### Comparing `PyPDFForm-1.4.8/tests/test_paragraph.py` & `PyPDFForm-1.4.9/tests/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.4.8/tests/test_preview.py` & `PyPDFForm-1.4.9/tests/test_preview.py`

 * *Files identical despite different names*

