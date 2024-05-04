# Comparing `tmp/pcffont-0.0.6.tar.gz` & `tmp/pcffont-0.0.7.tar.gz`

## Comparing `pcffont-0.0.6.tar` & `pcffont-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,51 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.6/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/artwiz/anorexia.pcf
--rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/artwiz/kates.pcf
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/dweep/dweep.pcf
--rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/profont-x11/ProFont_r400-29.pcf
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/raize/raize-normal-19.pcf
--rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/sgi/rock36.pcf
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/trisk/trisk.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.6/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.6/examples/__init__.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pcffont-0.0.6/examples/create.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pcffont-0.0.6/examples/load.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/error.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/font.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/format.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/header.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/metric.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.6/src/pcffont/internal/util.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pcffont-0.0.6/tests/test_dump.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.6/tests/test_example.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pcffont-0.0.6/tests/test_load_save.py
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 pcffont-0.0.6/tests/test_reload.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.6/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.6/LICENSE
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 pcffont-0.0.6/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 pcffont-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pcffont-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/README.md
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-msbit-p2-u4.pcf
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-msbit-p4-u2.pcf
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-lsbit-p2-u4.pcf
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-lsbit-p4-u2.pcf
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-msbit-p2-u4.pcf
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-msbit-p4-u2.pcf
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo.bdf
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/LICENSE
+-rw-r--r--   0        0        0   230552 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-12x24.pcf
+-rw-r--r--   0        0        0   268184 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-16x32.pcf
+-rw-r--r--   0        0        0   392216 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-32x64.pcf
+-rw-r--r--   0        0        0   145220 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-5x8.pcf
+-rw-r--r--   0        0        0   158776 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-6x12.pcf
+-rw-r--r--   0        0        0   206164 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-8x16.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.7/examples/__init__.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 pcffont-0.0.7/examples/create.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pcffont-0.0.7/examples/load.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/error.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/font.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/format.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/header.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/metric.py
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_buffer.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_demo.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_example.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_load_save.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_reload.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.7/LICENSE
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 pcffont-0.0.7/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pcffont-0.0.7/PKG-INFO
```

### Comparing `pcffont-0.0.6/.github/workflows/publish.yml` & `pcffont-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/.github/workflows/test.yml` & `pcffont-0.0.7/.github/workflows/test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.11", "3.12"]
+        python-version: ["3.10", "3.11", "3.12"]
     steps:
     - name: Checkout
       uses: actions/checkout@v4
     - name: Setup Python
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `pcffont-0.0.6/assets/unifont/OFL.txt` & `pcffont-0.0.7/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.7/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/examples/create.py` & `pcffont-0.0.7/examples/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     font.bdf_encodings = encodings
     font.glyph_names = glyph_names
     font.metrics = metrics
     font.ink_metrics = metrics
     font.scalable_widths = scalable_widths
     font.bitmaps = bitmaps
 
-    accelerators = PcfAccelerators(PcfTableFormat.build(has_ink_bounds=True))
+    accelerators = PcfAccelerators(PcfTableFormat(has_ink_bounds=True))
     accelerators.no_overlap = True
     accelerators.ink_inside = True
     accelerators.ink_metrics = True
     accelerators.font_ascent = 14
     accelerators.font_descent = 2
     accelerators.min_bounds = metrics[0]
     accelerators.max_bounds = metrics[0]
```

### Comparing `pcffont-0.0.6/examples/load.py` & `pcffont-0.0.7/examples/load.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/src/pcffont/error.py` & `pcffont-0.0.7/src/pcffont/error.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 
 class PcfTableTypeError(PcfError):
     pass
 
 
 class PcfPropKeyError(PcfError):
     def __init__(self, key: str, reason: str):
+        super().__init__(f"'{key}': {reason}")
         self.key = key
         self.reason = reason
-        super().__init__(f"'{key}': {reason}")
 
 
 class PcfPropValueError(PcfError):
     def __init__(self, key: str, value: object, reason: str):
+        super().__init__(f"'{key}': '{value}': {reason}")
         self.key = key
         self.value = value
         self.reason = reason
-        super().__init__(f"'{key}': '{value}': {reason}")
 
 
 class PcfXlfdError(PcfError):
     def __init__(self, font_name: str, reason: str):
+        super().__init__(f"'{font_name}': {reason}")
         self.font_name = font_name
         self.reason = reason
-        super().__init__(f"'{font_name}': {reason}")
 
 
 class PcfOutOfRangeError(PcfError):
     pass
```

### Comparing `pcffont-0.0.6/src/pcffont/font.py` & `pcffont-0.0.7/src/pcffont/font.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 import os
 from collections import UserDict
 from typing import BinaryIO
 
 from pcffont.error import PcfParseError, PcfTableTypeError
 from pcffont.header import PcfTableType, PcfHeader
-from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.t_accelerators import PcfAccelerators
 from pcffont.t_bitmaps import PcfBitmaps
 from pcffont.t_encodings import PcfBdfEncodings
 from pcffont.t_glyph_names import PcfGlyphNames
 from pcffont.t_metrics import PcfMetrics
 from pcffont.t_properties import PcfProperties
 from pcffont.t_scalable_widths import PcfScalableWidths
 from pcffont.table import PcfTable
 
+_TABLE_TYPE_REGISTRY = {
+    PcfTableType.PROPERTIES: PcfProperties,
+    PcfTableType.ACCELERATORS: PcfAccelerators,
+    PcfTableType.METRICS: PcfMetrics,
+    PcfTableType.BITMAPS: PcfBitmaps,
+    PcfTableType.INK_METRICS: PcfMetrics,
+    PcfTableType.BDF_ENCODINGS: PcfBdfEncodings,
+    PcfTableType.SWIDTHS: PcfScalableWidths,
+    PcfTableType.GLYPH_NAMES: PcfGlyphNames,
+    PcfTableType.BDF_ACCELERATORS: PcfAccelerators,
+}
+
 
 class PcfFont(UserDict[PcfTableType, PcfTable]):
     @staticmethod
     def parse(stream: BinaryIO, strict_level: int = 1) -> 'PcfFont':
         buffer = Buffer(stream)
 
         headers = PcfHeader.parse(buffer)
 
-        tables = {}
+        font = PcfFont()
         for header in headers:
-            if header.table_type in tables and strict_level >= 1:
+            if header.table_type in font and strict_level >= 1:
                 raise PcfParseError(f"Duplicate table '{header.table_type.name}'")
-            table = util.parse_table(buffer, header, strict_level)
-            tables[header.table_type] = table
+            table = _TABLE_TYPE_REGISTRY[header.table_type].parse(buffer, font, header, strict_level)
+            font[header.table_type] = table
 
-        return PcfFont(tables)
+        return font
 
     @staticmethod
     def load(
             file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
             strict_level: int = 1,
     ) -> 'PcfFont':
         with open(file_path, 'rb') as file:
             return PcfFont.parse(file, strict_level)
 
-    def __init__(self, tables: dict[PcfTableType, PcfTable | None] = None):
-        super().__init__(tables)
-
     def __setitem__(self, table_type: PcfTableType, table: PcfTable | None):
         if table is None:
             self.pop(table_type, None)
         else:
-            if not isinstance(table, util.TABLE_TYPE_REGISTRY[table_type]):
+            if not isinstance(table, _TABLE_TYPE_REGISTRY[table_type]):
                 raise PcfTableTypeError(f"Mismatched table type: '{table_type.name}' -> '{type(table)}'")
             super().__setitem__(table_type, table)
 
     def __repr__(self) -> str:
         return object.__repr__(self)
 
     @property
@@ -128,15 +136,15 @@
 
     def dump(self, stream: BinaryIO):
         buffer = Buffer(stream)
 
         headers = []
         table_offset = 4 + 4 + (4 * 4) * len(self)
         for table_type, table in sorted(self.items()):
-            table_size = table.dump(buffer, table_offset)
+            table_size = table.dump(buffer, self, table_offset)
             headers.append(PcfHeader(table_type, table.table_format, table_size, table_offset))
             table_offset += table_size
 
         PcfHeader.dump(buffer, headers)
 
     def save(self, file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
         with open(file_path, 'wb') as file:
```

### Comparing `pcffont-0.0.6/src/pcffont/header.py` & `pcffont-0.0.7/src/pcffont/header.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import IntEnum
 
 from pcffont.error import PcfParseError
+from pcffont.format import PcfTableFormat
 from pcffont.internal.buffer import Buffer
 
 _FILE_VERSION = b'\x01fcp'
 
 
 class PcfTableType(IntEnum):
     PROPERTIES = 1 << 0
@@ -15,42 +16,62 @@
     BDF_ENCODINGS = 1 << 5
     SWIDTHS = 1 << 6
     GLYPH_NAMES = 1 << 7
     BDF_ACCELERATORS = 1 << 8
 
 
 class PcfHeader:
+    _TABLE_PARSE_ORDER = [
+        PcfTableType.PROPERTIES,
+        PcfTableType.ACCELERATORS,
+        PcfTableType.BDF_ACCELERATORS,
+        PcfTableType.GLYPH_NAMES,
+        PcfTableType.METRICS,
+        PcfTableType.INK_METRICS,
+        PcfTableType.SWIDTHS,
+        PcfTableType.BITMAPS,
+        PcfTableType.BDF_ENCODINGS,
+    ]
+
     @staticmethod
     def parse(buffer: Buffer) -> list['PcfHeader']:
         buffer.seek(0)
         if buffer.read(4) != _FILE_VERSION:
             raise PcfParseError('Not PCF format')
 
         tables_count = buffer.read_uint32()
 
         headers = []
         for _ in range(tables_count):
             table_type = PcfTableType(buffer.read_uint32())
-            table_format = buffer.read_uint32()
+            table_format = PcfTableFormat.parse(buffer.read_uint32())
             table_size = buffer.read_uint32()
             table_offset = buffer.read_uint32()
             headers.append(PcfHeader(table_type, table_format, table_size, table_offset))
+        headers.sort(key=lambda header: PcfHeader._TABLE_PARSE_ORDER.index(header.table_type))
 
         return headers
 
     @staticmethod
     def dump(buffer: Buffer, headers: list['PcfHeader']):
         buffer.seek(0)
         buffer.write(_FILE_VERSION)
 
         buffer.write_uint32(len(headers))
         for header in headers:
             buffer.write_uint32(header.table_type)
-            buffer.write_uint32(header.table_format)
+            buffer.write_uint32(header.table_format.value)
             buffer.write_uint32(header.table_size)
             buffer.write_uint32(header.table_offset)
 
-    def __init__(self, table_type: PcfTableType, table_format: int, table_size: int, table_offset: int):
+    def __init__(self, table_type: PcfTableType, table_format: PcfTableFormat, table_size: int, table_offset: int):
         self.table_type = table_type
         self.table_format = table_format
         self.table_size = table_size
         self.table_offset = table_offset
+
+    def read_and_check_table_format(self, buffer: Buffer, strict_level: int) -> 'PcfTableFormat':
+        buffer.seek(self.table_offset)
+        value = buffer.read_uint32()
+        if value != self.table_format.value and strict_level >= 2:
+            raise PcfParseError(f"The table format definition is inconsistent with the header: type '{self.table_type.name}', offset {self.table_offset}")
+        return self.table_format
```

### Comparing `pcffont-0.0.6/src/pcffont/metric.py` & `pcffont-0.0.7/src/pcffont/metric.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/src/pcffont/t_accelerators.py` & `pcffont-0.0.7/src/pcffont/t_accelerators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,43 @@
+import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
 
 class PcfAccelerators(PcfTable):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfAccelerators':
-        table_format = PcfTableFormat.read_and_check(buffer, header)
-        ms_byte_first = PcfTableFormat.ms_byte_first(table_format)
-        has_ink_bounds = PcfTableFormat.has_ink_bounds(table_format)
+    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfAccelerators':
+        table_format = header.read_and_check_table_format(buffer, strict_level)
 
         no_overlap = buffer.read_bool()
         constant_metrics = buffer.read_bool()
         terminal_font = buffer.read_bool()
         constant_width = buffer.read_bool()
         ink_inside = buffer.read_bool()
         ink_metrics = buffer.read_bool()
         draw_right_to_left = buffer.read_bool()
         buffer.skip(1)
-        font_ascent = buffer.read_int32(ms_byte_first)
-        font_descent = buffer.read_int32(ms_byte_first)
-        max_overlap = buffer.read_int32(ms_byte_first)
-
-        min_bounds = PcfMetric.parse(buffer, ms_byte_first, False)
-        max_bounds = PcfMetric.parse(buffer, ms_byte_first, False)
-
-        if has_ink_bounds:
-            ink_min_bounds = PcfMetric.parse(buffer, ms_byte_first, False)
-            ink_max_bounds = PcfMetric.parse(buffer, ms_byte_first, False)
+        font_ascent = buffer.read_int32(table_format.ms_byte_first)
+        font_descent = buffer.read_int32(table_format.ms_byte_first)
+        max_overlap = buffer.read_int32(table_format.ms_byte_first)
+
+        min_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
+        max_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
+
+        if table_format.has_ink_bounds:
+            ink_min_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
+            ink_max_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
         else:
             ink_min_bounds = None
             ink_max_bounds = None
 
-        # TODO
+        # Compat
         if header.table_size > buffer.tell() - header.table_offset:
             buffer.seek(header.table_offset + 4 + 8 + 4 * 3 + 2 * 6 * 2)
             _compat_chunk_start = buffer.tell() - header.table_offset
             _compat_chunk_size = header.table_size - _compat_chunk_start
             _compat_chunk = buffer.read(_compat_chunk_size)
             _compat_info = _compat_chunk_start, _compat_chunk_size, _compat_chunk
         else:
@@ -58,22 +57,22 @@
             max_overlap,
             min_bounds,
             max_bounds,
             ink_min_bounds,
             ink_max_bounds,
         )
 
-        # TODO
+        # Compat
         accelerators._compat_info = _compat_info
 
         return accelerators
 
     def __init__(
             self,
-            table_format: int = PcfTableFormat.build(),
+            table_format: PcfTableFormat = None,
             no_overlap: bool = False,
             constant_metrics: bool = False,
             terminal_font: bool = False,
             constant_width: bool = False,
             ink_inside: bool = False,
             ink_metrics: bool = False,
             draw_right_to_left: bool = False,
@@ -81,14 +80,16 @@
             font_descent: int = 0,
             max_overlap: int = 0,
             min_bounds: PcfMetric = None,
             max_bounds: PcfMetric = None,
             ink_min_bounds: PcfMetric = None,
             ink_max_bounds: PcfMetric = None,
     ):
+        if table_format is None:
+            table_format = PcfTableFormat()
         super().__init__(table_format)
         self.no_overlap = no_overlap
         self.constant_metrics = constant_metrics
         self.terminal_font = terminal_font
         self.constant_width = constant_width
         self.ink_inside = ink_inside
         self.ink_metrics = ink_metrics
@@ -96,44 +97,41 @@
         self.font_ascent = font_ascent
         self.font_descent = font_descent
         self.max_overlap = max_overlap
         self.min_bounds = min_bounds
         self.max_bounds = max_bounds
         self.ink_min_bounds = ink_min_bounds
         self.ink_max_bounds = ink_max_bounds
-        self._compat_info: tuple[int, int, bytes] | None = None  # TODO
-
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
-        ms_byte_first = PcfTableFormat.ms_byte_first(self.table_format)
-        has_ink_bounds = PcfTableFormat.has_ink_bounds(self.table_format)
+        self._compat_info: tuple[int, int, bytes] | None = None
 
+    def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         buffer.seek(table_offset)
-        buffer.write_uint32(self.table_format)
+        buffer.write_uint32(self.table_format.value)
         buffer.write_bool(self.no_overlap)
         buffer.write_bool(self.constant_metrics)
         buffer.write_bool(self.terminal_font)
         buffer.write_bool(self.constant_width)
         buffer.write_bool(self.ink_inside)
         buffer.write_bool(self.ink_metrics)
         buffer.write_bool(self.draw_right_to_left)
         buffer.write_nulls(1)
-        buffer.write_int32(self.font_ascent, ms_byte_first)
-        buffer.write_int32(self.font_descent, ms_byte_first)
-        buffer.write_int32(self.max_overlap, ms_byte_first)
-
-        self.min_bounds.dump(buffer, ms_byte_first, False)
-        self.max_bounds.dump(buffer, ms_byte_first, False)
-
-        if has_ink_bounds:
-            self.ink_min_bounds.dump(buffer, ms_byte_first, False)
-            self.ink_max_bounds.dump(buffer, ms_byte_first, False)
+        buffer.write_int32(self.font_ascent, self.table_format.ms_byte_first)
+        buffer.write_int32(self.font_descent, self.table_format.ms_byte_first)
+        buffer.write_int32(self.max_overlap, self.table_format.ms_byte_first)
+
+        self.min_bounds.dump(buffer, self.table_format.ms_byte_first, False)
+        self.max_bounds.dump(buffer, self.table_format.ms_byte_first, False)
+
+        if self.table_format.has_ink_bounds:
+            self.ink_min_bounds.dump(buffer, self.table_format.ms_byte_first, False)
+            self.ink_max_bounds.dump(buffer, self.table_format.ms_byte_first, False)
 
         table_size = buffer.tell() - table_offset
 
-        # TODO
+        # Compat
         if self._compat_info is not None:
             _compat_chunk_start, _compat_chunk_size, _compat_chunk = self._compat_info
             _compat_chunk = bytearray(_compat_chunk)
 
             ink_chunk_size = 2 * 6 * 2
             if table_size == _compat_chunk_start + ink_chunk_size:
                 _compat_chunk_start += ink_chunk_size
```

### Comparing `pcffont-0.0.6/src/pcffont/t_bitmaps.py` & `pcffont-0.0.7/src/pcffont/t_bitmaps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,118 @@
+import math
 from collections import UserList
 
-from pcffont.error import PcfError
+import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 
+def _swap_fragments(fragments: list[list[int]], scan_unit: int):
+    if scan_unit == 2:
+        for i in range(0, len(fragments), 2):
+            fragments[i], fragments[i + 1] = fragments[i + 1], fragments[i]
+    elif scan_unit == 4:
+        for i in range(0, len(fragments), 4):
+            fragments[i], fragments[i + 1], fragments[i + 2], fragments[i + 3] = fragments[i + 3], fragments[i + 2], fragments[i + 1], fragments[i]
+
+
 class PcfBitmaps(PcfTable, UserList[list[list[int]]]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBitmaps':
-        table_format = PcfTableFormat.read_and_check(buffer, header)
-        ms_byte_first = PcfTableFormat.ms_byte_first(table_format)
-        ms_bit_first = PcfTableFormat.ms_bit_first(table_format)
-
-        bitmap_pad_mode = PcfTableFormat.bitmap_pad_mode(table_format)
-        bitmap_row_size = [1, 2, 4, 8][bitmap_pad_mode]
-
-        # FIXME
-        bit_scan_mode = PcfTableFormat.bit_scan_mode(table_format)
-        if bit_scan_mode != 0:
-            raise PcfError(f'Table format not supported: {table_format:b}')
-
-        glyphs_count = buffer.read_uint32(ms_byte_first)
-        bitmap_offsets = [buffer.read_uint32(ms_byte_first) for _ in range(glyphs_count)]
-        size_configs = [buffer.read_uint32(ms_byte_first) for _ in range(4)]
+    def parse(buffer: Buffer, font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfBitmaps':
+        table_format = header.read_and_check_table_format(buffer, strict_level)
+
+        glyph_pad = [1, 2, 4, 8][table_format.glyph_pad_index]
+        scan_unit = [1, 2, 4][table_format.scan_unit_index]
+
+        glyphs_count = buffer.read_uint32(table_format.ms_byte_first)
+        bitmap_offsets = buffer.read_uint32_list(glyphs_count, table_format.ms_byte_first)
+        bitmaps_sizes = buffer.read_uint32_list(4, table_format.ms_byte_first)
         bitmaps_start = buffer.tell()
-        bitmaps_size = size_configs[bitmap_pad_mode]
 
         bitmaps = PcfBitmaps(table_format)
-        for i in range(glyphs_count):
-            bitmap_offset = bitmap_offsets[i]
-            if i < glyphs_count - 1:
-                bitmap_offset_next = bitmap_offsets[i + 1]
-            else:
-                bitmap_offset_next = bitmaps_size
-            bitmap_size = bitmap_offset_next - bitmap_offset
+        for glyph_index, bitmap_offset in enumerate(bitmap_offsets):
+            buffer.seek(bitmaps_start + bitmap_offset)
+            metric = font.metrics[glyph_index]
+            glyph_row_pad = math.ceil(metric.glyph_width / (glyph_pad * 8)) * glyph_pad
+
+            fragments = buffer.read_binary_list(glyph_row_pad * metric.glyph_height, table_format.ms_bit_first)
+            if table_format.ms_byte_first != table_format.ms_bit_first:
+                _swap_fragments(fragments, scan_unit)
 
             bitmap = []
-            buffer.seek(bitmaps_start + bitmap_offset)
-            for _ in range(bitmap_size // bitmap_row_size):
+            for _ in range(metric.glyph_height):
                 bitmap_row = []
-                for _ in range(bitmap_row_size):
-                    data = buffer.read(1)
-                    array = [int(c) for c in f'{ord(data):08b}']
-                    if not ms_bit_first:
-                        array.reverse()
-                    bitmap_row.extend(array)
+                for _ in range(glyph_row_pad):
+                    bitmap_row.extend(fragments.pop(0))
+                bitmap_row = bitmap_row[:metric.glyph_width]
                 bitmap.append(bitmap_row)
             bitmaps.append(bitmap)
 
-        # TODO
-        bitmaps._compat_size_configs = size_configs
+        # Compat
+        bitmaps._compat_info = bitmaps_sizes
 
         return bitmaps
 
     def __init__(
             self,
-            table_format: int = PcfTableFormat.build(),
+            table_format: PcfTableFormat = None,
             bitmaps: list[list[list[int]]] = None,
     ):
+        if table_format is None:
+            table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, bitmaps)
-        self._compat_size_configs: list[int] | None = None  # TODO
+        self._compat_info: list[int] | None = None
 
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
-        ms_byte_first = PcfTableFormat.ms_byte_first(self.table_format)
-        ms_bit_first = PcfTableFormat.ms_byte_first(self.table_format)
-
-        bitmap_pad_mode = PcfTableFormat.bitmap_pad_mode(self.table_format)
-        bitmap_row_size = [1, 2, 4, 8][bitmap_pad_mode]
-
-        # FIXME
-        bit_scan_mode = PcfTableFormat.bit_scan_mode(self.table_format)
-        if bit_scan_mode != 0:
-            raise PcfError(f'Table format not supported: {self.table_format:b}')
+    def _dump(self, buffer: Buffer, font: 'pcffont.PcfFont', table_offset: int) -> int:
+        glyph_pad = [1, 2, 4, 8][self.table_format.glyph_pad_index]
+        scan_unit = [1, 2, 4][self.table_format.scan_unit_index]
 
         glyphs_count = len(self)
 
         bitmaps_start = table_offset + 4 + 4 + 4 * glyphs_count + 4 * 4
         bitmaps_size = 0
         bitmap_offsets = []
         buffer.seek(bitmaps_start)
-        for bitmap in self:
+        for glyph_index, bitmap in enumerate(self):
             bitmap_offsets.append(bitmaps_size)
+            metric = font.metrics[glyph_index]
+            bitmap_row_width = math.ceil(metric.glyph_width / (glyph_pad * 8)) * glyph_pad * 8
+
+            fragments = []
             for bitmap_row in bitmap:
-                if len(bitmap_row) < 8 * bitmap_row_size:
-                    bitmap_row = bitmap_row + [0] * (8 * bitmap_row_size - len(bitmap_row))
-                for i in range(len(bitmap_row) // 8):
-                    array = bitmap_row[i * 8:(i + 1) * 8]
-                    if not ms_bit_first:
-                        array.reverse()
-                    bin_string = ''.join(map(str, array))
-                    data = int(bin_string, 2).to_bytes(1, 'big')
-                    bitmaps_size += buffer.write(data)
-
-        # TODO
-        if self._compat_size_configs is not None:
-            size_configs = list(self._compat_size_configs)
-            size_configs[bitmap_pad_mode] = bitmaps_size
+                if len(bitmap_row) < bitmap_row_width:
+                    bitmap_row = bitmap_row + [0] * (bitmap_row_width - len(bitmap_row))
+                elif len(bitmap_row) > bitmap_row_width:
+                    bitmap_row = bitmap_row[:bitmap_row_width]
+                for i in range(bitmap_row_width // 8):
+                    fragments.append(bitmap_row[i * 8:(i + 1) * 8])
+
+            if self.table_format.ms_byte_first != self.table_format.ms_bit_first:
+                _swap_fragments(fragments, scan_unit)
+
+            bitmaps_size += buffer.write_binary_list(fragments, self.table_format.ms_bit_first)
+
+        # Compat
+        if self._compat_info is not None:
+            bitmaps_sizes = list(self._compat_info)
+            bitmaps_sizes[self.table_format.glyph_pad_index] = bitmaps_size
         else:
-            unit_size_config = bitmaps_size // bitmap_row_size
-            size_configs = [
-                unit_size_config,
-                unit_size_config * 2,
-                unit_size_config * 4,
-                unit_size_config * 8,
+            unit_bitmaps_size = bitmaps_size // glyph_pad
+            bitmaps_sizes = [
+                unit_bitmaps_size,
+                unit_bitmaps_size * 2,
+                unit_bitmaps_size * 4,
+                unit_bitmaps_size * 8,
             ]
 
         buffer.seek(table_offset)
-        buffer.write_uint32(self.table_format)
-        buffer.write_uint32(glyphs_count, ms_byte_first)
-        for bitmap_offset in bitmap_offsets:
-            buffer.write_uint32(bitmap_offset, ms_byte_first)
-        for size_config in size_configs:
-            buffer.write_uint32(size_config, ms_byte_first)
+        buffer.write_uint32(self.table_format.value)
+        buffer.write_uint32(glyphs_count, self.table_format.ms_byte_first)
+        buffer.write_uint32_list(bitmap_offsets, self.table_format.ms_byte_first)
+        buffer.write_uint32_list(bitmaps_sizes, self.table_format.ms_byte_first)
         buffer.skip(bitmaps_size)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.6/src/pcffont/t_encodings.py` & `pcffont-0.0.7/src/pcffont/t_encodings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import UserDict
 
+import pcffont
 from pcffont.error import PcfOutOfRangeError
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 _MAX_CODE_POINT = 0xFFFF
@@ -12,46 +13,47 @@
 
 class PcfBdfEncodings(PcfTable, UserDict[int, int]):
     """
     code_point -> glyph_index
     """
 
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBdfEncodings':
-        table_format = PcfTableFormat.read_and_check(buffer, header)
-        ms_byte_first = PcfTableFormat.ms_byte_first(table_format)
-
-        min_byte_2 = buffer.read_uint16(ms_byte_first)
-        max_byte_2 = buffer.read_uint16(ms_byte_first)
-        min_byte_1 = buffer.read_uint16(ms_byte_first)
-        max_byte_1 = buffer.read_uint16(ms_byte_first)
-        default_char = buffer.read_uint16(ms_byte_first)
+    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfBdfEncodings':
+        table_format = header.read_and_check_table_format(buffer, strict_level)
+
+        min_byte_2 = buffer.read_uint16(table_format.ms_byte_first)
+        max_byte_2 = buffer.read_uint16(table_format.ms_byte_first)
+        min_byte_1 = buffer.read_uint16(table_format.ms_byte_first)
+        max_byte_1 = buffer.read_uint16(table_format.ms_byte_first)
+        default_char = buffer.read_uint16(table_format.ms_byte_first)
 
         glyphs_count = (max_byte_2 - min_byte_2 + 1) * (max_byte_1 - min_byte_1 + 1)
-        glyph_indices = [buffer.read_uint16(ms_byte_first) for _ in range(glyphs_count)]
+        glyph_indices = buffer.read_uint16_list(glyphs_count, table_format.ms_byte_first)
 
         encodings = PcfBdfEncodings(table_format, default_char)
         if min_byte_1 == max_byte_1 == 0:
             for code_point in range(min_byte_2, max_byte_2 + 1):
                 glyph_index = glyph_indices[code_point - min_byte_2]
                 encodings[code_point] = glyph_index
         else:
             for byte_1 in range(min_byte_1, max_byte_1 + 1):
                 for byte_2 in range(min_byte_2, max_byte_2 + 1):
-                    code_point = int.from_bytes(bytes([byte_1, byte_2]))
+                    code_point = int.from_bytes(bytes([byte_1, byte_2]), 'big')
                     glyph_index = glyph_indices[(byte_1 - min_byte_1) * (max_byte_2 - min_byte_2 + 1) + byte_2 - min_byte_2]
                     encodings[code_point] = glyph_index
         return encodings
 
     def __init__(
             self,
-            table_format: int = PcfTableFormat.build(),
+            table_format: PcfTableFormat = None,
             default_char: int = _NO_GLYPH_INDEX,
             encodings: dict[int, int] = None,
     ):
+        if table_format is None:
+            table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserDict.__init__(self, encodings)
         self.default_char = default_char
 
     def __setitem__(self, code_point: int, glyph_index: int | None):
         if code_point < 0 or code_point > _MAX_CODE_POINT:
             raise PcfOutOfRangeError(f'Code point must between [0, {_MAX_CODE_POINT}]')
@@ -59,48 +61,46 @@
             raise PcfOutOfRangeError(f'Glyph index must between [0, {_NO_GLYPH_INDEX}]')
 
         if glyph_index is None or glyph_index == _NO_GLYPH_INDEX:
             self.pop(code_point, None)
         else:
             super().__setitem__(code_point, glyph_index)
 
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
-        ms_byte_first = PcfTableFormat.ms_byte_first(self.table_format)
-
+    def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         min_byte_2 = 0xFF
         max_byte_2 = 0
         min_byte_1 = 0xFF
         max_byte_1 = 0
         for code_point in self:
-            bs = code_point.to_bytes(2)
+            bs = code_point.to_bytes(2, 'big')
             byte_1 = bs[0]
             byte_2 = bs[1]
             if byte_1 < min_byte_1:
                 min_byte_1 = byte_1
             if byte_1 > max_byte_1:
                 max_byte_1 = byte_1
             if byte_2 < min_byte_2:
                 min_byte_2 = byte_2
             if byte_2 > max_byte_2:
                 max_byte_2 = byte_2
 
         buffer.seek(table_offset)
-        buffer.write_uint32(self.table_format)
-        buffer.write_uint16(min_byte_2, ms_byte_first)
-        buffer.write_uint16(max_byte_2, ms_byte_first)
-        buffer.write_uint16(min_byte_1, ms_byte_first)
-        buffer.write_uint16(max_byte_1, ms_byte_first)
-        buffer.write_uint16(self.default_char, ms_byte_first)
+        buffer.write_uint32(self.table_format.value)
+        buffer.write_uint16(min_byte_2, self.table_format.ms_byte_first)
+        buffer.write_uint16(max_byte_2, self.table_format.ms_byte_first)
+        buffer.write_uint16(min_byte_1, self.table_format.ms_byte_first)
+        buffer.write_uint16(max_byte_1, self.table_format.ms_byte_first)
+        buffer.write_uint16(self.default_char, self.table_format.ms_byte_first)
 
         if min_byte_1 == max_byte_1 == 0:
             for code_point in range(min_byte_2, max_byte_2 + 1):
                 glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
-                buffer.write_uint16(glyph_index, ms_byte_first)
+                buffer.write_uint16(glyph_index, self.table_format.ms_byte_first)
         else:
             for byte_1 in range(min_byte_1, max_byte_1 + 1):
                 for byte_2 in range(min_byte_2, max_byte_2 + 1):
-                    code_point = int.from_bytes(bytes([byte_1, byte_2]))
+                    code_point = int.from_bytes(bytes([byte_1, byte_2]), 'big')
                     glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
-                    buffer.write_uint16(glyph_index, ms_byte_first)
+                    buffer.write_uint16(glyph_index, self.table_format.ms_byte_first)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.6/src/pcffont/t_metrics.py` & `pcffont-0.0.7/src/pcffont/t_metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 from collections import UserList
 
+import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
 
 class PcfMetrics(PcfTable, UserList[PcfMetric]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfMetrics':
-        table_format = PcfTableFormat.read_and_check(buffer, header)
-        ms_byte_first = PcfTableFormat.ms_byte_first(table_format)
-        is_compressed = PcfTableFormat.is_compressed_metrics(table_format)
+    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfMetrics':
+        table_format = header.read_and_check_table_format(buffer, strict_level)
 
-        if is_compressed:
-            glyphs_count = buffer.read_uint16(ms_byte_first)
+        if table_format.is_compressed_metrics:
+            glyphs_count = buffer.read_uint16(table_format.ms_byte_first)
         else:
-            glyphs_count = buffer.read_uint32(ms_byte_first)
+            glyphs_count = buffer.read_uint32(table_format.ms_byte_first)
 
         metrics = PcfMetrics(table_format)
         for _ in range(glyphs_count):
-            metric = PcfMetric.parse(buffer, ms_byte_first, is_compressed)
+            metric = PcfMetric.parse(buffer, table_format.ms_byte_first, table_format.is_compressed_metrics)
             metrics.append(metric)
         return metrics
 
     def __init__(
             self,
-            table_format: int = PcfTableFormat.build(is_compressed_metrics=True),
+            table_format: PcfTableFormat = None,
             metrics: list[PcfMetric] = None,
     ):
+        if table_format is None:
+            table_format = PcfTableFormat(is_compressed_metrics=True)
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, metrics)
 
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
-        ms_byte_first = PcfTableFormat.ms_byte_first(self.table_format)
-        is_compressed = PcfTableFormat.is_compressed_metrics(self.table_format)
-
+    def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         glyphs_count = len(self)
 
         buffer.seek(table_offset)
-        buffer.write_uint32(self.table_format)
-        if is_compressed:
-            buffer.write_uint16(glyphs_count, ms_byte_first)
+        buffer.write_uint32(self.table_format.value)
+        if self.table_format.is_compressed_metrics:
+            buffer.write_uint16(glyphs_count, self.table_format.ms_byte_first)
         else:
-            buffer.write_uint32(glyphs_count, ms_byte_first)
+            buffer.write_uint32(glyphs_count, self.table_format.ms_byte_first)
         for metric in self:
-            metric.dump(buffer, ms_byte_first, is_compressed)
+            metric.dump(buffer, self.table_format.ms_byte_first, self.table_format.is_compressed_metrics)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.6/src/pcffont/t_properties.py` & `pcffont-0.0.7/src/pcffont/t_properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from collections import UserDict
 
+import pcffont
 from pcffont.error import PcfError, PcfPropKeyError, PcfPropValueError, PcfXlfdError
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 _KEY_FOUNDRY = 'FOUNDRY'
@@ -105,29 +106,28 @@
         matched = re.search(r'[-?*,"]', value)
         if matched is not None:
             raise PcfPropValueError(key, value, f"contains illegal characters '{matched.group()}'")
 
 
 class PcfProperties(PcfTable, UserDict[str, str | int]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader, strict_level: int) -> 'PcfProperties':
-        table_format = PcfTableFormat.read_and_check(buffer, header)
-        ms_byte_first = PcfTableFormat.ms_byte_first(table_format)
+    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfProperties':
+        table_format = header.read_and_check_table_format(buffer, strict_level)
 
-        props_count = buffer.read_uint32(ms_byte_first)
+        props_count = buffer.read_uint32(table_format.ms_byte_first)
 
         prop_infos = []
         for _ in range(props_count):
-            key_offset = buffer.read_uint32(ms_byte_first)
+            key_offset = buffer.read_uint32(table_format.ms_byte_first)
             is_string_prop = buffer.read_bool()
             if is_string_prop:
-                value_offset = buffer.read_uint32(ms_byte_first)
+                value_offset = buffer.read_uint32(table_format.ms_byte_first)
                 prop_infos.append((key_offset, is_string_prop, value_offset))
             else:
-                value = buffer.read_int32(ms_byte_first)
+                value = buffer.read_int32(table_format.ms_byte_first)
                 prop_infos.append((key_offset, is_string_prop, value))
 
         # Pad to next int32 boundary
         padding = 3 - (((4 + 1 + 4) * props_count + 3) % 4)
         buffer.skip(padding)
 
         buffer.skip(4)  # strings_size
@@ -147,17 +147,19 @@
             except (PcfPropKeyError, PcfPropValueError) as e:
                 if strict_level >= 1:
                     raise e
         return properties
 
     def __init__(
             self,
-            table_format: int = PcfTableFormat.build(),
+            table_format: PcfTableFormat = None,
             properties: dict[str, str | int] = None,
     ):
+        if table_format is None:
+            table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserDict.__init__(self, properties)
 
     def __getitem__(self, key: str) -> str | int:
         key = key.upper()
         _check_key(key)
         return super().__getitem__(key)
@@ -352,17 +354,15 @@
             else:
                 if key in _XLFD_FONT_NAME_STR_VALUE_KEYS:
                     value = token
                 else:
                     value = int(token)
             self[key] = value
 
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
-        ms_byte_first = PcfTableFormat.ms_byte_first(self.table_format)
-
+    def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         props_count = len(self)
 
         # Pad to next int32 boundary
         padding = 3 - (((4 + 1 + 4) * props_count + 3) % 4)
 
         strings_start = table_offset + 4 + 4 + (4 + 1 + 4) * props_count + padding + 4
         strings_size = 0
@@ -373,23 +373,23 @@
             strings_size += buffer.write_string(key)
             value_offset = strings_size
             if isinstance(value, str):
                 strings_size += buffer.write_string(value)
             prop_infos.append((key, key_offset, value, value_offset))
 
         buffer.seek(table_offset)
-        buffer.write_uint32(self.table_format)
-        buffer.write_uint32(props_count, ms_byte_first)
+        buffer.write_uint32(self.table_format.value)
+        buffer.write_uint32(props_count, self.table_format.ms_byte_first)
         for key, key_offset, value, value_offset in prop_infos:
-            buffer.write_uint32(key_offset, ms_byte_first)
+            buffer.write_uint32(key_offset, self.table_format.ms_byte_first)
             if isinstance(value, str):
                 buffer.write_bool(True)
-                buffer.write_uint32(value_offset, ms_byte_first)
+                buffer.write_uint32(value_offset, self.table_format.ms_byte_first)
             else:
                 buffer.write_bool(False)
-                buffer.write_int32(value, ms_byte_first)
+                buffer.write_int32(value, self.table_format.ms_byte_first)
         buffer.write_nulls(padding)
-        buffer.write_uint32(strings_size, ms_byte_first)
+        buffer.write_uint32(strings_size, self.table_format.ms_byte_first)
         buffer.skip(strings_size)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.6/src/pcffont/t_scalable_widths.py` & `pcffont-0.0.7/src/pcffont/t_scalable_widths.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from collections import UserList
 
+import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 
 class PcfScalableWidths(PcfTable, UserList[int]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfScalableWidths':
-        table_format = PcfTableFormat.read_and_check(buffer, header)
-        ms_byte_first = PcfTableFormat.ms_byte_first(table_format)
-
-        glyphs_count = buffer.read_uint32(ms_byte_first)
-
-        scalable_widths = PcfScalableWidths(table_format)
-        for _ in range(glyphs_count):
-            scalable_widths.append(buffer.read_int32(ms_byte_first))
+    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfScalableWidths':
+        table_format = header.read_and_check_table_format(buffer, strict_level)
+
+        glyphs_count = buffer.read_uint32(table_format.ms_byte_first)
+
+        scalable_widths = PcfScalableWidths(
+            table_format,
+            buffer.read_int32_list(glyphs_count, table_format.ms_byte_first),
+        )
         return scalable_widths
 
     def __init__(
             self,
-            table_format: int = PcfTableFormat.build(),
+            table_format: PcfTableFormat = None,
             scalable_widths: list[int] = None,
     ):
+        if table_format is None:
+            table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, scalable_widths)
 
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
-        ms_byte_first = PcfTableFormat.ms_byte_first(self.table_format)
-
+    def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         glyphs_count = len(self)
 
         buffer.seek(table_offset)
-        buffer.write_uint32(self.table_format)
-        buffer.write_uint32(glyphs_count, ms_byte_first)
-        for scalable_width in self:
-            buffer.write_int32(scalable_width, ms_byte_first)
+        buffer.write_uint32(self.table_format.value)
+        buffer.write_uint32(glyphs_count, self.table_format.ms_byte_first)
+        buffer.write_int32_list(self, self.table_format.ms_byte_first)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.6/src/pcffont/table.py` & `pcffont-0.0.7/src/pcffont/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from abc import abstractmethod
 
+import pcffont
+from pcffont.format import PcfTableFormat
 from pcffont.internal.buffer import Buffer
 
 
 class PcfTable:
-    def __init__(self, table_format: int):
+    def __init__(self, table_format: PcfTableFormat):
         self.table_format = table_format
 
     def __repr__(self) -> str:
         return object.__repr__(self)
 
     @abstractmethod
-    def _dump(self, buffer: Buffer, table_offset: int) -> int:
+    def _dump(self, buffer: Buffer, font: 'pcffont.PcfFont', table_offset: int) -> int:
         raise NotImplementedError
 
-    def dump(self, buffer: Buffer, table_offset: int) -> int:
-        table_size = self._dump(buffer, table_offset)
+    def dump(self, buffer: Buffer, font: 'pcffont.PcfFont', table_offset: int) -> int:
+        table_size = self._dump(buffer, font, table_offset)
 
         # All tables begin on a 32bit boundary (and will be padded with zeroes).
         padding = 4 - table_size % 4
         if padding != 4:
             buffer.seek(table_offset + table_size)
             table_size += buffer.write_nulls(padding)
```

### Comparing `pcffont-0.0.6/tests/test_reload.py` & `pcffont-0.0.7/tests/test_reload.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 def test_reload(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'unifont', 'unifont-15.1.05.pcf')
     save_file_path = os.path.join(tmp_path, 'unifont-15.1.05.pcf')
     font = PcfFont.load(load_file_path)
     font.accelerators._compat_info = None
     font.bdf_accelerators._compat_info = None
-    font.bitmaps._compat_size_configs = None
+    font.bitmaps._compat_info = None
     font.save(save_file_path)
 
     font_1 = PcfFont.load(load_file_path)
     font_2 = PcfFont.load(save_file_path)
 
     assert len(font_1) == len(font_2)
     for table_type, table_1 in font_1.items():
         table_2 = font_2[table_type]
-        assert table_1.table_format == table_2.table_format
+        assert table_1.table_format.value == table_2.table_format.value
 
     assert len(font_1.properties) == len(font_2.properties)
     for key, value_1 in font_1.properties.items():
         value_2 = font_2.properties[key]
         assert value_1 == value_2
 
     assert font_1.accelerators.no_overlap == font_2.accelerators.no_overlap
```

### Comparing `pcffont-0.0.6/.gitignore` & `pcffont-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/LICENSE` & `pcffont-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.6/README.md` & `pcffont-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PcfFont
 
-[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pcffont)](https://pypi.org/project/pcffont/)
 
 PcfFont is a library for manipulating [Portable Compiled Format (PCF) Fonts](https://en.wikipedia.org/wiki/Portable_Compiled_Format).
 
 ## Installation
 
 ```shell
@@ -110,15 +110,15 @@
     font.bdf_encodings = encodings
     font.glyph_names = glyph_names
     font.metrics = metrics
     font.ink_metrics = metrics
     font.scalable_widths = scalable_widths
     font.bitmaps = bitmaps
 
-    accelerators = PcfAccelerators(PcfTableFormat.build(has_ink_bounds=True))
+    accelerators = PcfAccelerators(PcfTableFormat(has_ink_bounds=True))
     accelerators.no_overlap = True
     accelerators.ink_inside = True
     accelerators.ink_metrics = True
     accelerators.font_ascent = 14
     accelerators.font_descent = 2
     accelerators.min_bounds = metrics[0]
     accelerators.max_bounds = metrics[0]
@@ -155,20 +155,21 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## Test Fonts
 
 - [GNU Unifont Glyphs](https://unifoundry.com/unifont/index.html)
-- [bitmap-fonts](https://github.com/masaeedu/bitmap-fonts)
+- [Spleen](https://github.com/fcambus/spleen)
 
 ## References
 
 - [FreeType font driver for PCF fonts](https://github.com/freetype/freetype/tree/master/src/pcf)
 - [FontForge - The X11 PCF bitmap font file format](https://fontforge.org/docs/techref/pcf-format.html)
-- [pcf2bdf](https://github.com/ganaware/pcf2bdf)
+- [The X Font Library](https://www.x.org/releases/current/doc/libXfont/fontlib.html)
 - [bdftopcf](https://gitlab.freedesktop.org/xorg/util/bdftopcf)
+- [bdftopcf - docs](https://www.x.org/releases/current/doc/man/man1/bdftopcf.1.xhtml)
 - [X Logical Font Description Conventions - X Consortium Standard](https://www.x.org/releases/current/doc/xorg-docs/xlfd/xlfd.html)
 
 ## License
 
 Under the [MIT license](LICENSE).
```

### Comparing `pcffont-0.0.6/pyproject.toml` & `pcffont-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.6"
+version = "0.0.7"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
 maintainers = [
     { name = "TakWolf" },
 ]
 keywords = ["pcf", "font"]
```

### Comparing `pcffont-0.0.6/PKG-INFO` & `pcffont-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.3
 Name: pcffont
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for manipulating Portable Compiled Format (PCF) Fonts.
 Project-URL: homepage, https://github.com/TakWolf/pcffont
 Project-URL: source, https://github.com/TakWolf/pcffont
 Project-URL: issues, https://github.com/TakWolf/pcffont/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 License-File: LICENSE
 Keywords: font,pcf
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PcfFont
 
-[![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
+[![Python](https://img.shields.io/badge/python-3.10-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pcffont)](https://pypi.org/project/pcffont/)
 
 PcfFont is a library for manipulating [Portable Compiled Format (PCF) Fonts](https://en.wikipedia.org/wiki/Portable_Compiled_Format).
 
 ## Installation
 
 ```shell
@@ -128,15 +128,15 @@
     font.bdf_encodings = encodings
     font.glyph_names = glyph_names
     font.metrics = metrics
     font.ink_metrics = metrics
     font.scalable_widths = scalable_widths
     font.bitmaps = bitmaps
 
-    accelerators = PcfAccelerators(PcfTableFormat.build(has_ink_bounds=True))
+    accelerators = PcfAccelerators(PcfTableFormat(has_ink_bounds=True))
     accelerators.no_overlap = True
     accelerators.ink_inside = True
     accelerators.ink_metrics = True
     accelerators.font_ascent = 14
     accelerators.font_descent = 2
     accelerators.min_bounds = metrics[0]
     accelerators.max_bounds = metrics[0]
@@ -173,20 +173,21 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## Test Fonts
 
 - [GNU Unifont Glyphs](https://unifoundry.com/unifont/index.html)
-- [bitmap-fonts](https://github.com/masaeedu/bitmap-fonts)
+- [Spleen](https://github.com/fcambus/spleen)
 
 ## References
 
 - [FreeType font driver for PCF fonts](https://github.com/freetype/freetype/tree/master/src/pcf)
 - [FontForge - The X11 PCF bitmap font file format](https://fontforge.org/docs/techref/pcf-format.html)
-- [pcf2bdf](https://github.com/ganaware/pcf2bdf)
+- [The X Font Library](https://www.x.org/releases/current/doc/libXfont/fontlib.html)
 - [bdftopcf](https://gitlab.freedesktop.org/xorg/util/bdftopcf)
+- [bdftopcf - docs](https://www.x.org/releases/current/doc/man/man1/bdftopcf.1.xhtml)
 - [X Logical Font Description Conventions - X Consortium Standard](https://www.x.org/releases/current/doc/xorg-docs/xlfd/xlfd.html)
 
 ## License
 
 Under the [MIT license](LICENSE).
```

