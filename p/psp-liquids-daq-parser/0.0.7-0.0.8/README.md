# Comparing `tmp/psp_liquids_daq_parser-0.0.7.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.7.tar", last modified: Sun Apr 21 05:21:47 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.8.tar", last modified: Fri May  3 22:10:31 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.7.tar` & `psp_liquids_daq_parser-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 05:21:45.000000 psp_liquids_daq_parser-0.0.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/plotly_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:21:47.303653 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 05:21:47.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-04-21 05:21:42.000000 psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 22:10:29.000000 psp_liquids_daq_parser-0.0.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/plotly_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.py
```

### Comparing `psp_liquids_daq_parser-0.0.7/LICENSE` & `psp_liquids_daq_parser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.7/PKG-INFO` & `psp_liquids_daq_parser-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.7
+Version: 0.0.8
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psp_liquids_daq_parser-0.0.7/README.md` & `psp_liquids_daq_parser-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.7/pyproject.toml` & `psp_liquids_daq_parser-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.7/src/classes.py` & `psp_liquids_daq_parser-0.0.8/src/classes.py`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.7/src/helpers.py` & `psp_liquids_daq_parser-0.0.8/src/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from datetime import datetime
 import re
+
+import pytz
 from classes import AnalogChannelData, DigitalChannelData
 from nptdms import TdmsChannel
 import numpy as np
+import pandas as pd
 
 def compileChannels(
     channels: list[TdmsChannel],
 ) -> tuple[dict[str, AnalogChannelData], dict[str, DigitalChannelData]]:
     toReturn_AI = {}
     toReturn_DI = {}
 
@@ -53,7 +57,20 @@
     pattern: str = r"\(([^()]+)\)"
     match: re.Match = re.search(pattern, group_name)
     sample_rate: float = float(match.group(1)[:-3])
     dt: float = 1 / sample_rate
     addedtime = np.arange(0, samples * dt, dt) + (start_time_unix_ms/1000)
     time: list[float] = addedtime.tolist()
     return time
+
+
+def convertStringTimestamp(data, fromTimezone):
+    if (str(data) == "nan"):
+        return data
+    test_date = data.split("+")
+    thing = datetime.strptime(test_date[0], "%Y-%m-%d %H:%M:%S.%f")
+    old_timezone = pytz.timezone(fromTimezone)
+    new_timezone = pytz.timezone("US/Eastern")
+    localized_timestamp = old_timezone.localize(thing)
+    new_timezone_timestamp = localized_timestamp.astimezone(new_timezone)
+    ms = new_timezone_timestamp.timestamp()
+    return ms
```

### Comparing `psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.egg-info/PKG-INFO` & `psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.7
+Version: 0.0.8
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psp_liquids_daq_parser-0.0.7/src/psp_liquids_daq_parser.py` & `psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import tkinter as tk
 from tkinter import filedialog
 import os
 
 import pandas as pd
 from classes import AnalogChannelData, DigitalChannelData, SensorNetData
-from helpers import compileChannels, getTime
+from helpers import compileChannels, convertStringTimestamp, getTime
 
 def parseTDMS(
     dev_num: int, start_time_unix_ms: int, file_path_custom: str = "", dev_group: str = "Data (1000.000000 Hz)"
 ) -> dict[str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]]:
     """## Parse a TDMS file (or an equivalent pickle file)
     ### Arguments:
     - `dev_num` (Type: `int`): dev box number (i.e: the `5` or `6` in dev5 or dev6)
@@ -133,15 +133,15 @@
                     )
                 }
             )
 
     return (available_channels, df_list_constant)
 
 def parseCSV(
-    start_time_unix_ms: int, file_path_custom: str = ""
+    start_time_unix_ms: int = 0, file_path_custom: str = ""
 ) -> dict[str, SensorNetData]:
     """## Parse a CSV file (or an equivalent pickle file)
     ### Arguments:
     - `start_time_unix_ms` (Type: `int`): unix timestamp in milliseconds indicating recording start time. Only required if not reading from a pickle file.
     - (Optional) `file_path_custom` (Type: `str`): the dynamic file path to a `.TDMS` file (use this in case you don't want to keep selecting the tdms file to parse every time you run the script)
     ### Description
     If `file_path_custom` isn't specified, the file picker dialog comes up to select a reduced csv file from sensornet. Then, we check to see if there's an equivalent pickle file in the same directory as the chosen csv file.
@@ -170,14 +170,18 @@
     else:
         channel_data_map: dict[
             str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]
         ] = {}
 
         df: pd.DataFrame = pd.read_csv(filepath)
         channel_names: list[str] = df.columns.to_list()
+        print("converting timestamps...")
+        for channel_name in channel_names:
+            if "_time" in channel_name and "-" in str(df[channel_name][3]):
+                df[channel_name] = df[channel_name].apply(lambda x: convertStringTimestamp(x, "UTC"))
         df[channel_names] = df[channel_names].astype('float64')
         for i in range(1,len(channel_names),2):
             channel: str = channel_names[i]
             timeArray: NDArray[float64] = df.iloc[:,i-1].to_numpy() + (start_time_unix_ms/1000)
             dataArray: NDArray[float64] = df.iloc[:,i].to_numpy()
             channel_data_map[channel] = SensorNetData(channel, timeArray, dataArray)
```

