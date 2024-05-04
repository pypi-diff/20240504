# Comparing `tmp/psp_liquids_daq_parser-0.0.8.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.8.tar", last modified: Fri May  3 22:10:31 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.9.tar", last modified: Sat May  4 18:26:12 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.8.tar` & `psp_liquids_daq_parser-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 22:10:29.000000 psp_liquids_daq_parser-0.0.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/plotly_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:10:31.123331 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 22:10:31.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-03 22:10:26.000000 psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:26:12.221604 psp_liquids_daq_parser-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-04 18:26:12.221604 psp_liquids_daq_parser-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:26:12.221604 psp_liquids_daq_parser-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:26:12.221604 psp_liquids_daq_parser-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 18:26:09.000000 psp_liquids_daq_parser-0.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/src/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/src/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/src/plotly_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:26:12.221604 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-04 18:26:12.000000 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 18:26:12.000000 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:26:12.000000 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-04 18:26:12.000000 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 18:26:12.000000 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-04 18:26:02.000000 psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.py
```

### Comparing `psp_liquids_daq_parser-0.0.8/LICENSE` & `psp_liquids_daq_parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.8/PKG-INFO` & `psp_liquids_daq_parser-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psp_liquids_daq_parser-0.0.8/README.md` & `psp_liquids_daq_parser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.8/pyproject.toml` & `psp_liquids_daq_parser-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.8/src/classes.py` & `psp_liquids_daq_parser-0.0.9/src/classes.py`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.8/src/helpers.py` & `psp_liquids_daq_parser-0.0.9/src/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 import re
+import time
 
 import pytz
 from classes import AnalogChannelData, DigitalChannelData
 from nptdms import TdmsChannel
 import numpy as np
 import pandas as pd
 
@@ -69,8 +70,14 @@
     test_date = data.split("+")
     thing = datetime.strptime(test_date[0], "%Y-%m-%d %H:%M:%S.%f")
     old_timezone = pytz.timezone(fromTimezone)
     new_timezone = pytz.timezone("US/Eastern")
     localized_timestamp = old_timezone.localize(thing)
     new_timezone_timestamp = localized_timestamp.astimezone(new_timezone)
     ms = new_timezone_timestamp.timestamp()
-    return ms
+    return ms
+
+def tdmsFilenameToSeconds(filename: str):
+    time_stamp_str = filename[8:25]
+    datetimeObj = datetime.strptime(time_stamp_str, "%Y-%m%d-%H%M-%S")
+    dateString = time.mktime(datetimeObj.timetuple())
+    return int(dateString)
```

### Comparing `psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.egg-info/PKG-INFO` & `psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psp_liquids_daq_parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Used to parse, convert, pickle, and pre-process TDMS files from BCLS or other NI daq boxes.
 Author-email: Rajan Phadnis <rajansd28@gmail.com>
 Project-URL: Homepage, https://github.com/Purdue-Space-Program/daq_parser
 Project-URL: Issues, https://github.com/Purdue-Space-Program/daq_parser/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psp_liquids_daq_parser-0.0.8/src/psp_liquids_daq_parser.py` & `psp_liquids_daq_parser-0.0.9/src/psp_liquids_daq_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import numpy as np
 import tkinter as tk
 from tkinter import filedialog
 import os
 
 import pandas as pd
 from classes import AnalogChannelData, DigitalChannelData, SensorNetData
-from helpers import compileChannels, convertStringTimestamp, getTime
+from helpers import compileChannels, convertStringTimestamp, getTime, tdmsFilenameToSeconds
 
 def parseTDMS(
-    dev_num: int, start_time_unix_ms: int, file_path_custom: str = "", dev_group: str = "Data (1000.000000 Hz)"
+    dev_num: int, start_time_unix_ms: int = 0, file_path_custom: str = "", dev_group: str = "Data (1000.000000 Hz)"
 ) -> dict[str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]]:
     """## Parse a TDMS file (or an equivalent pickle file)
     ### Arguments:
     - `dev_num` (Type: `int`): dev box number (i.e: the `5` or `6` in dev5 or dev6)
     - `start_time_unix_ms` (Type: `int`): unix timestamp in milliseconds indicating recording start time. Only required if not reading from a pickle file.
     - (Optional) `file_path_custom` (Type: `str`): the dynamic file path to a `.TDMS` file (use this in case you don't want to keep selecting the tdms file to parse every time you run the script)
     - (Optional) `dev_group` (Type: `str`): the TDMS group header. You usually don't have to touch this unless the data isn't high frequency sampling data
@@ -49,14 +49,16 @@
             str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]
         ] = {}
         tdms_file: TdmsFile = TdmsFile.read(filepath)
         group: TdmsGroup = tdms_file[dev_group]
         dev5_channels = compileChannels(group.channels())
         channel_data_map.update(dev5_channels[0])
         channel_data_map.update(dev5_channels[1])
+        if (start_time_unix_ms == 0):
+            start_time_unix_ms = tdmsFilenameToSeconds(os.path.basename(filepath)) * 1000
         channel_data_map["time"] = getTime(channel_data_map, dev_group, start_time_unix_ms)
         with open(pickle_filepath, "wb") as f:
             pickle.dump(channel_data_map, f, pickle.HIGHEST_PROTOCOL)
         print(
             f'conversion done!\n\n\nNext time you want to run the converter, consider calling the function with: "parseTDMS({dev_num}, file_path_custom={pickle_filepath[:-7] + ".tdms"})"'
         )
         return channel_data_map
@@ -94,51 +96,47 @@
 
     # get the length of the largest dataset
     total_length: int = 0
     for channel in available_channels:
         if channel != "time" and len(channel_data[channel].data) > total_length:
             total_length = len(channel_data[channel].data)
 
-    # for each channel, pad the end of that channel's dataset with some value to
-    # make all the channel's data the same length and simeltaneously convert it all to np arrays
-    df_list_constant = {}
-    time: list[float] = channel_data["time"]
-    df_list_constant.update(
-        {"time": np.pad(time, (0, total_length - len(time)), "edge")}
-    )
-    for channel in available_channels:
-        # for binary channels, make the padding value 0.5 to make it easy to identify which data is to be ignored
-        if channel.startswith(binary_channel_prefixes):
-            df_list_constant.update(
+    first_time: float = channel_data["time"][0]
+    last_time: float = channel_data["time"][-1]
+    available_channels = []
+    df = pd.DataFrame.from_dict({"time": channel_data["time"]})
+    for dataset in channel_data:
+        if dataset != "time":
+            new_data = np.array(channel_data[dataset].data.tolist())
+            temp_time = channel_data["time"][:len(new_data)]
+            if(hasattr(channel_data[dataset], "time")):
+                temp_time = np.array(channel_data[dataset].time.tolist())
+            new_df = pd.DataFrame.from_dict(
                 {
-                    channel: np.pad(
-                        channel_data[channel].data,
-                        (0, total_length - len(channel_data[channel].data)),
-                        "constant",
-                        constant_values=(
-                            0.5,
-                            0.5,
-                        ),
-                    )
+                    "temp_time": temp_time,
+                    dataset: new_data,
                 }
             )
-        # for all other channels, set the padding value to zero
-        elif channel != "time":
-            df_list_constant.update(
-                {
-                    channel: np.pad(
-                        channel_data[channel].data,
-                        (0, total_length - len(channel_data[channel].data)),
-                        "constant",
-                        constant_values=(0, 0),
-                    )
-                }
+            new_df.drop(new_df[new_df['temp_time'] < first_time].index, inplace=True)
+            new_df.drop(new_df[new_df['temp_time'] > last_time].index, inplace=True)
+            new_df.dropna(inplace=True)
+            merged_df = pd.merge_asof(
+                df.sort_values("time"),
+                new_df.sort_values("temp_time"),
+                left_on="time",
+                right_on="temp_time",
+                direction="nearest",
+                tolerance=5
             )
+            merged_df.drop("temp_time", axis=1, inplace=True)
+            df = merged_df
+            available_channels.append(dataset)
+            print("extended: " + dataset)
 
-    return (available_channels, df_list_constant)
+    return (available_channels, df.to_dict("list"))
 
 def parseCSV(
     start_time_unix_ms: int = 0, file_path_custom: str = ""
 ) -> dict[str, SensorNetData]:
     """## Parse a CSV file (or an equivalent pickle file)
     ### Arguments:
     - `start_time_unix_ms` (Type: `int`): unix timestamp in milliseconds indicating recording start time. Only required if not reading from a pickle file.
@@ -189,7 +187,14 @@
         with open(pickle_filepath, "wb") as f:
             pickle.dump(channel_data_map, f, pickle.HIGHEST_PROTOCOL)
         print(
             f'conversion done!\n\n\nNext time you want to run the converter, consider calling the function with: "parseCSV(file_path_custom=\"{pickle_filepath[:-7] + ".tdms"}\")"'
         )
         return channel_data_map
 
+def combineTDMSDatasets(existing: dict[str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]], to_add: dict[str, AnalogChannelData | DigitalChannelData | SensorNetData | list[float]]):
+    if (len(existing["time"]) > len(to_add["time"])):
+        to_add.update(existing)
+        return to_add
+    else:
+        existing.update(to_add)
+        return existing
```

