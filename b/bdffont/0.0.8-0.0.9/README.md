# Comparing `tmp/bdffont-0.0.8.tar.gz` & `tmp/bdffont-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.8.tar", last modified: Fri May 26 07:35:00 2023, max compression
+gzip compressed data, was "bdffont-0.0.9.tar", last modified: Wed May 31 09:56:03 2023, max compression
```

## Comparing `bdffont-0.0.8.tar` & `bdffont-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.775603 bdffont-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 07:34:46.000000 bdffont-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-26 07:35:00.775603 bdffont-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-26 07:34:46.000000 bdffont-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 07:34:46.000000 bdffont-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:35:00.775603 bdffont-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.771603 bdffont-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.771603 bdffont-0.0.8/src/bdffont/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.775603 bdffont-0.0.8/src/bdffont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.775603 bdffont-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-26 07:34:46.000000 bdffont-0.0.8/tests/test_damaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-26 07:34:46.000000 bdffont-0.0.8/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-26 07:34:46.000000 bdffont-0.0.8/tests/test_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:03.197701 bdffont-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-31 09:55:50.000000 bdffont-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-31 09:56:03.197701 bdffont-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-31 09:55:50.000000 bdffont-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-31 09:55:50.000000 bdffont-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:56:03.197701 bdffont-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:03.193701 bdffont-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:03.193701 bdffont-0.0.9/src/bdffont/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 09:55:50.000000 bdffont-0.0.9/src/bdffont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-31 09:55:50.000000 bdffont-0.0.9/src/bdffont/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-05-31 09:55:50.000000 bdffont-0.0.9/src/bdffont/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-31 09:55:50.000000 bdffont-0.0.9/src/bdffont/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-31 09:55:50.000000 bdffont-0.0.9/src/bdffont/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 09:55:50.000000 bdffont-0.0.9/src/bdffont/xlfd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:03.197701 bdffont-0.0.9/src/bdffont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-31 09:56:03.000000 bdffont-0.0.9/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 09:56:03.000000 bdffont-0.0.9/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:56:03.000000 bdffont-0.0.9/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 09:56:03.000000 bdffont-0.0.9/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:03.197701 bdffont-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-31 09:55:50.000000 bdffont-0.0.9/tests/test_damaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-31 09:55:50.000000 bdffont-0.0.9/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-31 09:55:50.000000 bdffont-0.0.9/tests/test_type.py
```

### Comparing `bdffont-0.0.8/LICENSE` & `bdffont-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.8/PKG-INFO` & `bdffont-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,98 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
 Keywords: bdf,font
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BdfFont
 
+[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/bdffont)](https://pypi.org/project/bdffont/)
 
 BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format).
 
 ## Installation
 
 ```commandline
 pip install bdffont
 ```
 
 ## Usage
 
+### Load
+
+```python
+import os
+
+from bdffont import BdfFont
+from examples import assets_dir, outputs_dir
+
+
+def main():
+    font = BdfFont.load(os.path.join(assets_dir, 'unifont-15.0.01.bdf'))
+    print(f'name: {font.name}')
+    print(f'size: {font.point_size}')
+    print(f'ascent: {font.properties.font_ascent}')
+    print(f'descent: {font.properties.font_descent}')
+    for glyph in font.get_orderly_glyphs():
+        print(f'glyph: {glyph.name} - {glyph.code_point:04X}')
+    font.save(os.path.join(outputs_dir, 'unifont-15.0.01.bdf'), optimize_bitmap=True)
+
+
+if __name__ == '__main__':
+    main()
+```
+
+### Create
+
 ```python
 import os
 
-from bdffont import BdfFont, BdfProperties, BdfGlyph
+from bdffont import BdfFont, BdfGlyph, xlfd
 from examples import outputs_dir
 
 
 def main():
     font = BdfFont(
-        name='my-font',
         point_size=16,
-        dpi_xy=(75, 75),
+        resolution_xy=(75, 75),
         bounding_box_size=(16, 16),
         bounding_box_offset=(0, -2),
-        properties=BdfProperties({
-            'PARAM_1': 1,
-            'PARAM_2': '2',
-        }),
-        comments=[
-            'This is a comment.',
-            'This is a comment, too.',
-        ],
     )
-    font.properties.font_version = '1.0.0'
-    font.properties.font_ascent = 7
+
+    font.properties.foundry = 'TakWolf Studio'
+    font.properties.family_name = 'Demo Pixel'
+    font.properties.add_style_name = xlfd.AddStyleName.SANS_SERIF
+    font.properties.pixel_size = 16
+    font.properties.point_size = 160
+    font.properties.spacing = xlfd.Spacing.PROPORTIONAL
+    font.setup_missing_xlfd_properties()
+
+    font.properties.default_char = -1
+    font.properties.font_ascent = 14
     font.properties.font_descent = 2
     font.properties.x_height = 5
     font.properties.cap_height = 7
+
+    font.properties.font_version = '1.0.0'
+    font.properties.copyright = 'Copyright (c) TakWolf'
+
     font.add_glyph(BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(500, 0),
         device_width=(8, 0),
         bounding_box_size=(8, 16),
         bounding_box_offset=(0, -2),
@@ -80,22 +111,29 @@
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
         ],
     ))
+
+    glyph_widths = [glyph.scalable_width_x for glyph in font.get_orderly_glyphs()]
+    font.properties.average_width = round(sum(glyph_widths) / font.get_glyphs_count())
+
+    font.generate_xlfd_font_name()
+
     font.save(os.path.join(outputs_dir, 'my-font.bdf'), optimize_bitmap=True)
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## References
 
 - [X11 - Bitmap Distribution Format - Version 2.1](https://www.x.org/docs/BDF/bdf.pdf)
 - [Adobe - Glyph Bitmap Distribution Format (BDF) Specification - Version 2.2](https://adobe-type-tools.github.io/font-tech-notes/pdfs/5005.BDF_Spec.pdf)
+- [X Logical Font Description Conventions - X Consortium Standard](https://www.x.org/releases/X11R7.6/doc/xorg-docs/specs/XLFD/xlfd.html)
 
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `bdffont-0.0.8/src/bdffont/glyph.py` & `bdffont-0.0.9/src/bdffont/glyph.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,47 +2,50 @@
 
 
 class BdfGlyph:
     def __init__(
             self,
             name: str,
             code_point: int,
-            scalable_width: tuple[int, int],
-            device_width: tuple[int, int],
-            bounding_box_size: tuple[int, int],
-            bounding_box_offset: tuple[int, int],
+            scalable_width: tuple[int, int] = (0, 0),
+            device_width: tuple[int, int] = (0, 0),
+            bounding_box_size: tuple[int, int] = (0, 0),
+            bounding_box_offset: tuple[int, int] = (0, 0),
             bitmap: list[list[int]] = None,
             comments: list[str] = None,
     ):
         """
         :param name:
-            Up to 14 characters (no blanks) of descriptive name of the glyph.
+            The name for the glyph, limited to a string of 14 characters. In base fonts, this should correspond to
+            the name in the PostScript language outline font's encoding vector. In a Composite font (Type 0), the
+            value may be a numeric offset or glyph ID.
         :param code_point:
-            Code point in Unicode.
+            The code point in Unicode. Could set -1 and optionally by another integer specifying the glyph index
+            for the non-standard encoding.
         :param scalable_width:
-            The scalable width in x and y of character. Scalable widths are in units of 1/1000th of the size of the
-            character. If the size of the character is p points, the width information must be scaled by p/1000 to
-            get the width of the character in printer’s points. This width information should be considered as a vector
-            indicating the position of the next character’s origin relative to the origin of this character.
-            To convert the scalable width to the width in device pixels, multiply scalable_width times p/1000 times
+            The scalable width in x and y of the glyph. The scalable width are in units of 1/1000th of the size of
+            the glyph and correspond to the width found in AFM files (for outline fonts). If the size of the glyph
+            is p points, the width information must be scaled by p/1000 to get the width of the glyph in printer's
+            points. This width information should be regarded as a vector indicating the position of the next glyph's
+            origin relative to the origin of this glyph.
+            To convert the scalable width to the width in device pixels, multiply scalable width times p/1000 times
             r/72, where r is the device resolution in pixels per inch. The result is a real number giving the ideal
-            print width in device pixels. The actual device width must of course be an integral number of device pixels
-            and is given in the next entry. The scalable_width y value should always be zero for a standard X font.
+            width in device pixels. The actual device width must be an integral number of device pixels and is given
+            by the device width entry.
+            The scalable width y value should always be zero for a standard X font.
         :param device_width:
-            The width in x and y of the character in device units. Like the scalable_width, this width information is
-            a vector indicating the position of the next character’s origin relative to the origin of this character.
-            Note that the device_width of a given "hand-tuned" WYSIWYG glyph may deviate slightly from its ideal
-            device-independent width given by scalable_width in order to improve its typographic characteristics on a
-            display. The device_width y value should always be zero for a standard X font.
+            The width in x and y of the glyph in device pixels. Like the scalable width, this width information is a
+            vector indicating the position of the next glyph's origin relative to the origin of this glyph.
+            The device width y value should always be zero for a standard X font.
         :param bounding_box_size:
-            The width in x, height in y of the character.
+            The width in x and height in y of the bitmap in integer pixel values.
         :param bounding_box_offset:
-            The x and y displacement of the lower left corner from the origin of the character.
+            The x and y displacement of the lower left corner from origin 0 of the bitmap in integer pixel values.
         :param bitmap:
-            The bitmap object.
+            The bitmap of the glyph.
         :param comments:
             The comments.
         """
         self.name = name
         self.code_point = code_point
         self.scalable_width_x, self.scalable_width_y = scalable_width
         self.device_width_x, self.device_width_y = device_width
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bdffont-0.0.8/src/bdffont.egg-info/PKG-INFO` & `bdffont-0.0.9/src/bdffont.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,98 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
 Keywords: bdf,font
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BdfFont
 
+[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/bdffont)](https://pypi.org/project/bdffont/)
 
 BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format).
 
 ## Installation
 
 ```commandline
 pip install bdffont
 ```
 
 ## Usage
 
+### Load
+
+```python
+import os
+
+from bdffont import BdfFont
+from examples import assets_dir, outputs_dir
+
+
+def main():
+    font = BdfFont.load(os.path.join(assets_dir, 'unifont-15.0.01.bdf'))
+    print(f'name: {font.name}')
+    print(f'size: {font.point_size}')
+    print(f'ascent: {font.properties.font_ascent}')
+    print(f'descent: {font.properties.font_descent}')
+    for glyph in font.get_orderly_glyphs():
+        print(f'glyph: {glyph.name} - {glyph.code_point:04X}')
+    font.save(os.path.join(outputs_dir, 'unifont-15.0.01.bdf'), optimize_bitmap=True)
+
+
+if __name__ == '__main__':
+    main()
+```
+
+### Create
+
 ```python
 import os
 
-from bdffont import BdfFont, BdfProperties, BdfGlyph
+from bdffont import BdfFont, BdfGlyph, xlfd
 from examples import outputs_dir
 
 
 def main():
     font = BdfFont(
-        name='my-font',
         point_size=16,
-        dpi_xy=(75, 75),
+        resolution_xy=(75, 75),
         bounding_box_size=(16, 16),
         bounding_box_offset=(0, -2),
-        properties=BdfProperties({
-            'PARAM_1': 1,
-            'PARAM_2': '2',
-        }),
-        comments=[
-            'This is a comment.',
-            'This is a comment, too.',
-        ],
     )
-    font.properties.font_version = '1.0.0'
-    font.properties.font_ascent = 7
+
+    font.properties.foundry = 'TakWolf Studio'
+    font.properties.family_name = 'Demo Pixel'
+    font.properties.add_style_name = xlfd.AddStyleName.SANS_SERIF
+    font.properties.pixel_size = 16
+    font.properties.point_size = 160
+    font.properties.spacing = xlfd.Spacing.PROPORTIONAL
+    font.setup_missing_xlfd_properties()
+
+    font.properties.default_char = -1
+    font.properties.font_ascent = 14
     font.properties.font_descent = 2
     font.properties.x_height = 5
     font.properties.cap_height = 7
+
+    font.properties.font_version = '1.0.0'
+    font.properties.copyright = 'Copyright (c) TakWolf'
+
     font.add_glyph(BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(500, 0),
         device_width=(8, 0),
         bounding_box_size=(8, 16),
         bounding_box_offset=(0, -2),
@@ -80,22 +111,29 @@
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
         ],
     ))
+
+    glyph_widths = [glyph.scalable_width_x for glyph in font.get_orderly_glyphs()]
+    font.properties.average_width = round(sum(glyph_widths) / font.get_glyphs_count())
+
+    font.generate_xlfd_font_name()
+
     font.save(os.path.join(outputs_dir, 'my-font.bdf'), optimize_bitmap=True)
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## References
 
 - [X11 - Bitmap Distribution Format - Version 2.1](https://www.x.org/docs/BDF/bdf.pdf)
 - [Adobe - Glyph Bitmap Distribution Format (BDF) Specification - Version 2.2](https://adobe-type-tools.github.io/font-tech-notes/pdfs/5005.BDF_Spec.pdf)
+- [X Logical Font Description Conventions - X Consortium Standard](https://www.x.org/releases/X11R7.6/doc/xorg-docs/specs/XLFD/xlfd.html)
 
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `bdffont-0.0.8/tests/test_damaged.py` & `bdffont-0.0.9/tests/test_damaged.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 
 import pytest
 
-import bdffont
-from bdffont.error import BdfMissingLine, BdfValueIncorrect
+from bdffont import BdfFont
+from bdffont.error import BdfMissingLine, BdfCountIncorrect
 from tests import assets_dir
 
 
 def load_damaged_bdf(file_name: str, strict_mode: bool = False):
     file_path = os.path.join(assets_dir, 'damaged', file_name)
-    bdffont.load_bdf(file_path, strict_mode=strict_mode)
+    BdfFont.load(file_path, strict_mode=strict_mode)
 
 
 def test_not_a_bdf():
     with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('not_a_bdf.bdf')
     assert info.value.word == 'STARTFONT'
 
@@ -80,17 +80,17 @@
     with pytest.raises(BdfMissingLine) as info:
         load_damaged_bdf('no_line_end_font.bdf')
     assert info.value.word == 'ENDFONT'
 
 
 def test_incorrect_properties_count():
     load_damaged_bdf('incorrect_properties_count.bdf')
-    with pytest.raises(BdfValueIncorrect) as info:
+    with pytest.raises(BdfCountIncorrect) as info:
         load_damaged_bdf('incorrect_properties_count.bdf', strict_mode=True)
     assert info.value.word == 'STARTPROPERTIES'
 
 
 def test_incorrect_chars_count():
     load_damaged_bdf('incorrect_chars_count.bdf')
-    with pytest.raises(BdfValueIncorrect) as info:
+    with pytest.raises(BdfCountIncorrect) as info:
         load_damaged_bdf('incorrect_chars_count.bdf', strict_mode=True)
     assert info.value.word == 'CHARS'
```

### Comparing `bdffont-0.0.8/tests/test_demo.py` & `bdffont-0.0.9/tests/test_demo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 import os
 
-import bdffont
 from bdffont import BdfFont
 from tests import assets_dir, outputs_dir
 
 
 def load_bdf(file_name: str) -> tuple[BdfFont, str]:
     file_path = os.path.join(assets_dir, file_name)
     with open(file_path, 'r', encoding='utf-8') as file:
         bdf_text = file.read()
-    font = bdffont.decode_bdf_str(bdf_text)
+    font = BdfFont.decode_str(bdf_text)
     return font, bdf_text
 
 
 def test_example():
     font, bdf_text = load_bdf('example.bdf')
     assert font.encode_str() == bdf_text
     assert font.encode_str(optimize_bitmap=True) == bdf_text
     assert font.spec_version == '2.1'
     assert font.name == '-Adobe-Helvetica-Bold-R-Normal--24-240-75-75-P-65-ISO8859-1'
     assert font.point_size == 24
-    assert font.dpi_x == 75
-    assert font.dpi_y == 75
-    assert font.dpi_xy == (75, 75)
+    assert font.resolution_x == 75
+    assert font.resolution_y == 75
+    assert font.resolution_xy == (75, 75)
     assert font.bounding_box_width == 9
     assert font.bounding_box_height == 24
     assert font.bounding_box_size == (9, 24)
     assert font.bounding_box_offset_x == -2
     assert font.bounding_box_offset_y == -6
     assert font.bounding_box_offset == (-2, -6)
     assert font.bounding_box == (9, 24, -2, -6)
     assert len(font.properties) == 19
     assert font.properties.foundry == 'Adobe'
-    assert font.properties['FAMILY'] == 'Helvetica'
+    assert font.properties.family_name == 'Helvetica'
     assert font.properties.weight_name == 'Bold'
     assert font.properties.slant == 'R'
-    assert font.properties['SETWIDTH_NAME'] == 'Normal'
-    assert font.properties['ADD_STYLE_NAME'] == ''
-    assert font.properties['PIXEL_SIZE'] == 24
+    assert font.properties.setwidth_name == 'Normal'
+    assert font.properties.add_style_name == ''
+    assert font.properties.pixel_size == 24
     assert font.properties.point_size == 240
     assert font.properties.resolution_x == 75
     assert font.properties.resolution_y == 75
-    assert font.properties['SPACING'] == 'P'
-    assert font.properties['AVERAGE_WIDTH'] == 65
-    assert font.properties['CHARSET_REGISTRY'] == 'ISO8859'
-    assert font.properties['CHARSET_ENCODING'] == '1'
+    assert font.properties.spacing == 'P'
+    assert font.properties.average_width == 65
+    assert font.properties.charset_registry == 'ISO8859'
+    assert font.properties.charset_encoding == '1'
     assert font.properties['MIN_SPACE'] == 4
     assert font.properties.font_ascent == 21
     assert font.properties.font_descent == 7
     assert font.properties.copyright == 'Copyright (c) 1987 Adobe Systems, Inc.'
     assert font.properties.notice == 'Helvetica is a registered trademark of Linotype Inc.'
     assert font.get_glyphs_count() == 2
     glyph = font.get_glyph(39)
```

### Comparing `bdffont-0.0.8/tests/test_type.py` & `bdffont-0.0.9/tests/test_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,87 @@
 import pytest
 
-from bdffont import BdfFont, BdfProperties, BdfGlyph
-from bdffont.error import BdfGlyphExists, BdfIllegalBitmap, BdfIllegalPropertiesKey, BdfIllegalPropertiesValue
+from bdffont import BdfFont, BdfProperties, BdfGlyph, xlfd
+from bdffont.error import BdfException, BdfGlyphExists, BdfIllegalBitmap, BdfIllegalPropertiesKey, BdfIllegalPropertiesValue, BdfIllegalXlfdFontName
 
 
 def test_font():
-    font = BdfFont(
-        name='',
-        point_size=0,
-        dpi_xy=(0, 0),
-        bounding_box_size=(0, 0),
-        bounding_box_offset=(0, 0),
-    )
+    font = BdfFont()
 
-    font.dpi_xy = 1, 2
-    assert font.dpi_xy == (1, 2)
-    assert font.dpi_x == 1
-    assert font.dpi_y == 2
+    font.resolution_xy = 1, 2
+    assert font.resolution_xy == (1, 2)
+    assert font.resolution_x == 1
+    assert font.resolution_y == 2
 
     font.bounding_box_size = 3, 4
     assert font.bounding_box_size == (3, 4)
     assert font.bounding_box_width == 3
     assert font.bounding_box_height == 4
 
     font.bounding_box_offset = 5, 6
     assert font.bounding_box_offset == (5, 6)
     assert font.bounding_box_offset_x == 5
     assert font.bounding_box_offset_y == 6
-
     assert font.bounding_box == (3, 4, 5, 6)
+
     font.bounding_box = 7, 8, 9, 10
     assert font.bounding_box == (7, 8, 9, 10)
     assert font.bounding_box_width == 7
     assert font.bounding_box_height == 8
     assert font.bounding_box_offset_x == 9
     assert font.bounding_box_offset_y == 10
 
+    font = BdfFont()
+
+    font.point_size = 16
+    font.resolution_xy = (75, 75)
+    font.properties.foundry = 'TakWolf Studio'
+    font.properties.family_name = 'Demo Pixel'
+    font.properties.add_style_name = xlfd.AddStyleName.SANS_SERIF
+    font.properties.pixel_size = 16
+    font.properties.point_size = 160
+    font.properties.spacing = xlfd.Spacing.PROPORTIONAL
+    font.properties.average_width = 80
+    font.setup_missing_xlfd_properties()
+    assert font.properties.weight_name == 'Medium'
+    assert font.properties.slant == 'R'
+    assert font.properties.setwidth_name == 'Normal'
+    assert font.properties.resolution_x == 75
+    assert font.properties.resolution_y == 75
+    assert font.properties.charset_registry == 'ISO10646'
+    assert font.properties.charset_encoding == '1'
+    font.generate_xlfd_font_name()
+    assert font.name == '-TakWolf Studio-Demo Pixel-Medium-R-Normal-Sans Serif-16-160-75-75-P-80-ISO10646-1'
+
+    font = BdfFont()
+
+    with pytest.raises(BdfException) as info:
+        font.update_by_name_as_xlfd_font_name()
+    assert info.value.args[0] == "Missing attribute 'name'"
+    font.name = '-Adobe-Times-Medium-R-Normal--14-100-100-100-P-74-ISO8859-1'
+    font.update_by_name_as_xlfd_font_name()
+    assert font.resolution_x == 100
+    assert font.resolution_y == 100
+    assert font.properties.foundry == 'Adobe'
+    assert font.properties.family_name == 'Times'
+    assert font.properties.weight_name == 'Medium'
+    assert font.properties.slant == 'R'
+    assert font.properties.setwidth_name == 'Normal'
+    assert font.properties.add_style_name is None
+    assert font.properties.pixel_size == 14
+    assert font.properties.point_size == 100
+    assert font.properties.resolution_x == 100
+    assert font.properties.resolution_y == 100
+    assert font.properties.spacing == 'P'
+    assert font.properties.average_width == 74
+    assert font.properties.charset_registry == 'ISO8859'
+    assert font.properties.charset_encoding == '1'
+
+    font = BdfFont()
+
     glyph_a = BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(500, 0),
         device_width=(3, 0),
         bounding_box_size=(2, 2),
         bounding_box_offset=(0, 0),
@@ -84,125 +126,218 @@
 
     font.add_glyph(glyph_b)
     font.add_glyph(glyph_a)
     glyphs = font.get_orderly_glyphs()
     assert glyphs[0] == glyph_a
     assert glyphs[1] == glyph_b
 
+    with pytest.raises(BdfException) as info:
+        font.encode()
+    assert info.value.args[0] == "Missing attribute 'name'"
+    font.name = 'my-font'
+    font.encode()
+
 
 def test_properties():
     properties = BdfProperties({
         'PARAM_1': 1,
-        'PARAM_2': '2',
+        'param_2': '2',
+        'PARAM_3': None,
     }, comments=[
         'This is a comment.',
         'This is a comment, too.',
     ])
+
     assert len(properties) == 2
-    assert properties['PARAM_1'] == 1
+    assert properties['param_1'] == 1
     assert properties['PARAM_2'] == '2'
     assert len(properties.comments) == 2
     assert properties.comments[0] == 'This is a comment.'
     assert properties.comments[1] == 'This is a comment, too.'
 
-    assert properties.default_char is None
-    properties.default_char = 1
-    assert properties.default_char == 1
-    assert 'DEFAULT_CHAR' in properties
-
-    assert properties.font_ascent is None
-    properties.font_ascent = 2
-    assert properties.font_ascent == 2
-    assert 'FONT_ASCENT' in properties
-
-    assert properties.font_descent is None
-    properties.font_descent = 3
-    assert properties.font_descent == 3
-    assert 'FONT_DESCENT' in properties
-
-    assert properties.cap_height is None
-    properties.cap_height = 4
-    assert properties.cap_height == 4
-    assert 'CAP_HEIGHT' in properties
+    properties.clear()
 
-    assert properties.x_height is None
-    properties.x_height = 5
-    assert properties.x_height == 5
-    assert 'X_HEIGHT' in properties
+    properties.foundry = 'TakWolf Studio'
+    assert properties.foundry == 'TakWolf Studio'
+    assert properties['FOUNDRY'] == 'TakWolf Studio'
+
+    properties.family_name = 'Demo Pixel'
+    assert properties.family_name == 'Demo Pixel'
+    assert properties['FAMILY_NAME'] == 'Demo Pixel'
+
+    properties.weight_name = xlfd.WeightName.MEDIUM
+    assert properties.weight_name == 'Medium'
+    assert properties['WEIGHT_NAME'] == 'Medium'
+
+    properties.slant = xlfd.Slant.ROMAN
+    assert properties.slant == 'R'
+    assert properties['SLANT'] == 'R'
+
+    properties.setwidth_name = xlfd.SetwidthName.NORMAL
+    assert properties.setwidth_name == 'Normal'
+    assert properties['SETWIDTH_NAME'] == 'Normal'
+
+    properties.add_style_name = xlfd.AddStyleName.SANS_SERIF
+    assert properties.add_style_name == 'Sans Serif'
+    assert properties['ADD_STYLE_NAME'] == 'Sans Serif'
+
+    properties.pixel_size = 16
+    assert properties.pixel_size == 16
+    assert properties['PIXEL_SIZE'] == 16
+
+    properties.point_size = 160
+    assert properties.point_size == 160
+    assert properties['POINT_SIZE'] == 160
+
+    properties.resolution_x = 75
+    assert properties.resolution_x == 75
+    assert properties['RESOLUTION_X'] == 75
+
+    properties.resolution_y = 240
+    assert properties.resolution_y == 240
+    assert properties['RESOLUTION_Y'] == 240
+
+    properties.spacing = xlfd.Spacing.MONOSPACED
+    assert properties.spacing == 'M'
+    assert properties['SPACING'] == 'M'
+
+    properties.average_width = 85
+    assert properties.average_width == 85
+    assert properties['AVERAGE_WIDTH'] == 85
+
+    properties.charset_registry = xlfd.CharsetRegistry.ISO8859
+    assert properties.charset_registry == 'ISO8859'
+    assert properties['CHARSET_REGISTRY'] == 'ISO8859'
+
+    properties.charset_encoding = '1'
+    assert properties.charset_encoding == '1'
+    assert properties['CHARSET_ENCODING'] == '1'
+
+    assert len(properties) == 14
+
+    font_name = '-TakWolf Studio-Demo Pixel-Medium-R-Normal-Sans Serif-16-160-75-240-M-85-ISO8859-1'
+    assert properties.to_xlfd_font_name() == font_name
+
+    font_name = '-Bitstream-Charter-Medium-R-Normal--12-120-75-75-P-68-ISO8859-1'
+    properties.update_by_xlfd_font_name(font_name)
+    assert properties.foundry == 'Bitstream'
+    assert properties.family_name == 'Charter'
+    assert properties.weight_name == 'Medium'
+    assert properties.slant == 'R'
+    assert properties.setwidth_name == 'Normal'
+    assert properties.add_style_name is None
+    assert properties.pixel_size == 12
+    assert properties.point_size == 120
+    assert properties.resolution_x == 75
+    assert properties.resolution_y == 75
+    assert properties.spacing == 'P'
+    assert properties.average_width == 68
+    assert properties.charset_registry == 'ISO8859'
+    assert properties.charset_encoding == '1'
 
+    font_name = '--------------'
+    properties.update_by_xlfd_font_name(font_name)
+    assert properties.foundry is None
+    assert properties.family_name is None
+    assert properties.weight_name is None
+    assert properties.slant is None
+    assert properties.setwidth_name is None
+    assert properties.add_style_name is None
+    assert properties.pixel_size is None
     assert properties.point_size is None
-    properties.point_size = 6
-    assert properties.point_size == 6
-    assert 'POINT_SIZE' in properties
-
     assert properties.resolution_x is None
-    properties.resolution_x = 7
-    assert properties.resolution_x == 7
-    assert 'RESOLUTION_X' in properties
-
     assert properties.resolution_y is None
-    properties.resolution_y = 8
-    assert properties.resolution_y == 8
-    assert 'RESOLUTION_Y' in properties
-
-    assert properties.face_name is None
-    properties.face_name = 'A'
-    assert properties.face_name == 'A'
-    assert 'FACE_NAME' in properties
-
-    assert properties.font is None
-    properties.font = 'B'
-    assert properties.font == 'B'
-    assert 'FONT' in properties
-
-    assert properties.font_version is None
-    properties.font_version = '1.2.3'
-    assert properties.font_version == '1.2.3'
-    assert 'FONT_VERSION' in properties
-
-    assert properties.family_name is None
-    properties.family_name = 'C'
-    assert properties.family_name == 'C'
-    assert 'FAMILY_NAME' in properties
-
-    assert properties.slant is None
-    properties.slant = 'D'
-    assert properties.slant == 'D'
-    assert 'SLANT' in properties
+    assert properties.spacing is None
+    assert properties.average_width is None
+    assert properties.charset_registry is None
+    assert properties.charset_encoding is None
+
+    font_name = 'Bitstream-Charter-Medium-R-Normal--12-120-75-75-P-68-ISO8859-1'
+    with pytest.raises(BdfIllegalXlfdFontName) as info:
+        properties.update_by_xlfd_font_name(font_name)
+    assert info.value.font_name == font_name
+    assert info.value.reason == "not starts with '-'"
+
+    font_name = '-Bitstream-Charter-Medium-R-Normal--12-120-75-75-P-68-ISO8859-1-'
+    with pytest.raises(BdfIllegalXlfdFontName) as info:
+        properties.update_by_xlfd_font_name(font_name)
+    assert info.value.font_name == font_name
+    assert info.value.reason == "there could only be 14 '-' in the name"
+
+    properties.clear()
+
+    properties.default_char = -1
+    assert properties.default_char == -1
+    assert properties['DEFAULT_CHAR'] == -1
+
+    properties.font_ascent = 14
+    assert properties.font_ascent == 14
+    assert properties['FONT_ASCENT'] == 14
+
+    properties.font_descent = 2
+    assert properties.font_descent == 2
+    assert properties['FONT_DESCENT'] == 2
 
-    assert properties.weight_name is None
-    properties.weight_name = 'E'
-    assert properties.weight_name == 'E'
-    assert 'WEIGHT_NAME' in properties
-
-    assert properties.foundry is None
-    properties.foundry = 'F'
-    assert properties.foundry == 'F'
-    assert 'FOUNDRY' in properties
-
-    assert properties.copyright is None
-    properties.copyright = 'G'
-    assert properties.copyright == 'G'
-    assert 'COPYRIGHT' in properties
-
-    assert properties.notice is None
-    properties.notice = 'H'
-    assert properties.notice == 'H'
-    assert 'NOTICE' in properties
-
-    assert len(properties) == 19
-
-    with pytest.raises(BdfIllegalPropertiesKey):
-        properties['abc'] = 'abc'
-
-    with pytest.raises(BdfIllegalPropertiesKey):
-        properties['ABC-DEF'] = 'abcdef'
+    properties.x_height = 5
+    assert properties.x_height == 5
+    assert properties['X_HEIGHT'] == 5
 
-    with pytest.raises(BdfIllegalPropertiesValue):
-        properties['TEST_KEY'] = float(1.2)
+    properties.cap_height = 8
+    assert properties.cap_height == 8
+    assert properties['CAP_HEIGHT'] == 8
+
+    assert len(properties) == 5
+    properties.clear()
+
+    properties.font_version = '1.0.0'
+    assert properties.font_version == '1.0.0'
+    assert properties['FONT_VERSION'] == '1.0.0'
+
+    properties.copyright = 'Copyright (c) TakWolf'
+    assert properties.copyright == 'Copyright (c) TakWolf'
+    assert properties['COPYRIGHT'] == 'Copyright (c) TakWolf'
+
+    properties.notice = 'This is a notice.'
+    assert properties.notice == 'This is a notice.'
+    assert properties['NOTICE'] == 'This is a notice.'
+
+    assert len(properties) == 3
+    properties.clear()
+
+    properties['abc'] = 'abc'
+    assert properties['ABC'] == 'abc'
+    assert properties['abc'] == 'abc'
+
+    with pytest.raises(BdfIllegalPropertiesKey) as info:
+        properties['abc-def'] = 'abcdef'
+    assert info.value.key == 'ABC-DEF'
+
+    properties['NONE_PARAM'] = None
+    assert 'NONE_PARAM' not in properties
+
+    with pytest.raises(BdfIllegalPropertiesValue) as info:
+        properties.foundry = 1
+    assert info.value.key == 'FOUNDRY'
+    assert info.value.value == 1
+
+    with pytest.raises(BdfIllegalPropertiesValue) as info:
+        properties.pixel_size = '1'
+    assert info.value.key == 'PIXEL_SIZE'
+    assert info.value.value == '1'
+
+    with pytest.raises(BdfIllegalPropertiesValue) as info:
+        # noinspection PyTypeChecker
+        properties['FLOAT_PARAM'] = 1.2
+    assert info.value.key == 'FLOAT_PARAM'
+    assert info.value.value == 1.2
+
+    with pytest.raises(BdfIllegalPropertiesValue) as info:
+        properties.family_name = 'Demo-Pixel'
+    assert info.value.key == 'FAMILY_NAME'
+    assert info.value.value == 'Demo-Pixel'
 
 
 def test_glyph():
     glyph = BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(0, 0),
```

