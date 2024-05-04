# Comparing `tmp/fiftyl_toolkit-0.1.2.tar.gz` & `tmp/fiftyl_toolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyl_toolkit-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fiftyl_toolkit-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fiftyl_toolkit-0.1.2.tar` & `fiftyl_toolkit-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      583 2023-10-23 15:57:30.490862 fiftyl_toolkit-0.1.2/README.md
--rw-r--r--   0        0        0       21 2023-10-23 14:43:57.802838 fiftyl_toolkit-0.1.2/fiftyl_toolkit/__init__.py
--rw-r--r--   0        0        0       28 2023-10-23 14:43:57.849504 fiftyl_toolkit-0.1.2/fiftyl_toolkit/io/__init__.py
--rw-r--r--   0        0        0     5851 2023-11-23 13:45:10.777183 fiftyl_toolkit-0.1.2/fiftyl_toolkit/io/extractor.py
--rw-r--r--   0        0        0      670 2023-11-23 13:45:58.590524 fiftyl_toolkit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 fiftyl_toolkit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-10-23 15:57:30.490862 fiftyl_toolkit-0.1.3/README.md
+-rw-r--r--   0        0        0     1289 2024-05-04 11:01:59.636333 fiftyl_toolkit-0.1.3/fiftyl_toolkit/ChannelMaps.py
+-rw-r--r--   0        0        0       21 2023-10-23 14:43:57.802838 fiftyl_toolkit-0.1.3/fiftyl_toolkit/__init__.py
+-rw-r--r--   0        0        0       28 2023-10-23 14:43:57.849504 fiftyl_toolkit-0.1.3/fiftyl_toolkit/io/__init__.py
+-rw-r--r--   0        0        0     5583 2024-05-04 11:11:04.980463 fiftyl_toolkit-0.1.3/fiftyl_toolkit/io/extractor.py
+-rw-r--r--   0        0        0      670 2024-05-04 11:12:01.583522 fiftyl_toolkit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 fiftyl_toolkit-0.1.3/PKG-INFO
```

### Comparing `fiftyl_toolkit-0.1.2/README.md` & `fiftyl_toolkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fiftyl_toolkit-0.1.2/fiftyl_toolkit/io/extractor.py` & `fiftyl_toolkit-0.1.3/fiftyl_toolkit/io/extractor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+from ..ChannelMaps import CHANNEL_MAPS
+
 from datetime import datetime
 from functools import singledispatchmethod
 import os
 
 import numpy as np
 
 import daqdataformats
 from hdf5libs import HDF5RawDataFile
 from rawdatautils.unpack.wibeth import np_array_adc
 
 class Data:
     _dt_format = "%Y%m%dT%H%M%S" # datetime format from hdf5 files.
     _channels_per_link = 64
-    _channel_map = np.array([112, 113, 115, 116, 118, 119, 120, 121, 123, 124, 126, 127, 64, 65, 67, 68, 70, 71, 72, 73, 75, 76, 78, 79, 48, 49, 51, 52, 54, 55, 56, 57, 59, 60, 62, 63, 0, 1, 3, 4, 6, 7, 8, 9, 11, 12, 14, 15, 50, 53, 58, 61, 2, 5, 10, 13, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 114, 117, 122, 125, 66, 69, 74, 77])
 
-    def __init__(self, filename: str):
+    def __init__(self, filename: str, map_version: int=0):
         self._filename = os.path.expanduser(filename)
         self._h5_file = HDF5RawDataFile(self._filename)
         self._records = self._h5_file.get_all_record_ids()
         self._last_extracted_record = None
 
         self._datetime = datetime.strptime(self._filename.split("_")[-1].split(".")[0], self._dt_format)
         self.run_id = int(self._filename.split('/')[-1].split('_')[1][3:])
         self.sub_run_id = int(self._filename.split('/')[-1].split('_')[2])
+        self.set_channel_map(map_version)
+
+    def set_channel_map(self, map_version: int=0) -> None:
+        """
+        Set the channel map version.
+        """
+        self._channel_map = CHANNEL_MAPS[map_version]
+        return
 
     def get_run_id(self) -> int:
         """
         Return the run ID integer.
         """
         return self.run_id
```

### Comparing `fiftyl_toolkit-0.1.2/pyproject.toml` & `fiftyl_toolkit-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fiftyl_toolkit"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{ name = "Alejandro Oranday", email = "alejandro@oran.day" }
 ]
 description = "50L data toolkit"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fiftyl_toolkit-0.1.2/PKG-INFO` & `fiftyl_toolkit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyl_toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: 50L data toolkit
 Author-email: Alejandro Oranday <alejandro@oran.day>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

