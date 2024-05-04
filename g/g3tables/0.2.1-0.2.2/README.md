# Comparing `tmp/g3tables-0.2.1.tar.gz` & `tmp/g3tables-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3tables-0.2.1.tar", last modified: Mon Apr 29 14:34:40 2024, max compression
+gzip compressed data, was "g3tables-0.2.2.tar", last modified: Sat May  4 20:13:16 2024, max compression
```

## Comparing `g3tables-0.2.1.tar` & `g3tables-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.838334 g3tables-0.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3tables-0.2.1/LICENCE
--rw-rw-rw-   0        0        0     1325 2024-04-29 14:34:40.836331 g3tables-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-02-05 12:26:13.000000 g3tables-0.2.1/README.md
--rw-rw-rw-   0        0        0     1679 2024-04-29 14:33:37.000000 g3tables-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 14:34:40.839331 g3tables-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.368334 g3tables-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.407332 g3tables-0.2.1/src/g3tables/
--rw-rw-rw-   0        0        0      550 2024-04-17 13:30:09.000000 g3tables-0.2.1/src/g3tables/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.621329 g3tables-0.2.1/src/g3tables/plc_composition_io_table/
--rw-rw-rw-   0        0        0      361 2024-01-30 11:09:40.000000 g3tables-0.2.1/src/g3tables/plc_composition_io_table/__init__.py
--rw-rw-rw-   0        0        0    14539 2024-04-17 23:31:56.000000 g3tables-0.2.1/src/g3tables/plc_composition_io_table/_extend_table.py
--rw-rw-rw-   0        0        0    21360 2024-04-23 15:47:17.000000 g3tables-0.2.1/src/g3tables/plc_composition_io_table/_table.py
--rw-rw-rw-   0        0        0     5535 2023-10-09 09:10:14.000000 g3tables-0.2.1/src/g3tables/plc_composition_io_table/io_signals.json
--rw-rw-rw-   0        0        0        0 2023-11-09 12:06:31.000000 g3tables-0.2.1/src/g3tables/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.652332 g3tables-0.2.1/src/g3tables/sw_definition_table/
--rw-rw-rw-   0        0        0      182 2024-01-23 16:58:13.000000 g3tables-0.2.1/src/g3tables/sw_definition_table/__init__.py
--rw-rw-rw-   0        0        0    54470 2024-04-24 09:59:15.000000 g3tables-0.2.1/src/g3tables/sw_definition_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.786334 g3tables-0.2.1/src/g3tables/system_config/
--rw-rw-rw-   0        0        0      225 2024-02-06 12:11:24.000000 g3tables-0.2.1/src/g3tables/system_config/__init__.py
--rw-rw-rw-   0        0        0    15259 2024-04-26 09:28:53.000000 g3tables-0.2.1/src/g3tables/system_config/_cli.py
--rw-rw-rw-   0        0        0    22338 2024-04-29 14:30:55.000000 g3tables-0.2.1/src/g3tables/system_config/_g3core_updater.py
--rw-rw-rw-   0        0        0      972 2024-04-25 15:08:07.000000 g3tables-0.2.1/src/g3tables/system_config/_hw_connections.py
--rw-rw-rw-   0        0        0     8599 2024-04-23 15:46:30.000000 g3tables-0.2.1/src/g3tables/system_config/_iomap_updater.py
--rw-rw-rw-   0        0        0       74 2024-04-17 13:09:47.000000 g3tables-0.2.1/src/g3tables/system_config/_logger.py
--rw-rw-rw-   0        0        0     7326 2024-04-20 10:49:38.000000 g3tables-0.2.1/src/g3tables/system_config/_sw_system_dict_wrapper.py
--rw-rw-rw-   0        0        0     4132 2024-04-25 15:08:14.000000 g3tables-0.2.1/src/g3tables/system_config/_system_config_processor.py
--rw-rw-rw-   0        0        0     1192 2024-04-17 13:14:39.000000 g3tables-0.2.1/src/g3tables/system_config/type_hinting.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.800333 g3tables-0.2.1/src/g3tables/utils/
--rw-rw-rw-   0        0        0      146 2024-02-05 13:19:52.000000 g3tables-0.2.1/src/g3tables/utils/__init__.py
--rw-rw-rw-   0        0        0     1552 2024-01-03 13:08:04.000000 g3tables-0.2.1/src/g3tables/utils/_d2nd.py
--rw-rw-rw-   0        0        0     3706 2023-10-25 21:45:04.000000 g3tables-0.2.1/src/g3tables/utils/_interval.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.810331 g3tables-0.2.1/src/g3tables/utils/gdrive/
--rw-rw-rw-   0        0        0      365 2024-03-10 17:32:39.000000 g3tables-0.2.1/src/g3tables/utils/gdrive/__init__.py
--rw-rw-rw-   0        0        0     5172 2024-04-17 14:08:11.000000 g3tables-0.2.1/src/g3tables/utils/gdrive/_gdrive.py
--rw-rw-rw-   0        0        0     1263 2024-03-10 16:29:47.000000 g3tables-0.2.1/src/g3tables/utils/gdrive/_update_creds.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.821331 g3tables-0.2.1/src/g3tables/visualization_table/
--rw-rw-rw-   0        0        0      207 2024-01-23 16:54:08.000000 g3tables-0.2.1/src/g3tables/visualization_table/__init__.py
--rw-rw-rw-   0        0        0    14811 2024-04-17 20:18:51.000000 g3tables-0.2.1/src/g3tables/visualization_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:34:40.824333 g3tables-0.2.1/src/g3tables.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-04-29 14:34:40.000000 g3tables-0.2.1/src/g3tables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-04-29 14:34:40.000000 g3tables-0.2.1/src/g3tables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:34:40.000000 g3tables-0.2.1/src/g3tables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-04-29 14:34:40.000000 g3tables-0.2.1/src/g3tables.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-04-29 14:34:40.000000 g3tables-0.2.1/src/g3tables.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 14:34:40.000000 g3tables-0.2.1/src/g3tables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.488160 g3tables-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.2/LICENCE
+-rw-rw-rw-   0        0        0     1325 2024-05-04 20:13:16.488160 g3tables-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1679 2024-05-02 05:59:12.000000 g3tables-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:13:16.488160 g3tables-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.387880 g3tables-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.403516 g3tables-0.2.2/src/g3tables/
+-rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.434757 g3tables-0.2.2/src/g3tables/plc_composition_io_table/
+-rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/__init__.py
+-rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/_extend_table.py
+-rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/_table.py
+-rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/io_signals.json
+-rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.434757 g3tables-0.2.2/src/g3tables/sw_definition_table/
+-rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/sw_definition_table/__init__.py
+-rw-rw-rw-   0        0        0    54470 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/sw_definition_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.450378 g3tables-0.2.2/src/g3tables/system_config/
+-rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/__init__.py
+-rw-rw-rw-   0        0        0    15259 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_cli.py
+-rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_g3core_updater.py
+-rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_hw_connections.py
+-rw-rw-rw-   0        0        0     8599 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_iomap_updater.py
+-rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/_logger.py
+-rw-rw-rw-   0        0        0     7326 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_sw_system_dict_wrapper.py
+-rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/_system_config_processor.py
+-rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/type_hinting.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.472517 g3tables-0.2.2/src/g3tables/utils/
+-rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/__init__.py
+-rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/_d2nd.py
+-rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/_interval.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.472517 g3tables-0.2.2/src/g3tables/utils/gdrive/
+-rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/gdrive/__init__.py
+-rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/gdrive/_gdrive.py
+-rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/gdrive/_update_creds.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.472517 g3tables-0.2.2/src/g3tables/visualization_table/
+-rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/visualization_table/__init__.py
+-rw-rw-rw-   0        0        0    14819 2024-04-30 13:14:34.000000 g3tables-0.2.2/src/g3tables/visualization_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.488160 g3tables-0.2.2/src/g3tables.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/top_level.txt
```

### Comparing `g3tables-0.2.1/LICENCE` & `g3tables-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/PKG-INFO` & `g3tables-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.1
+Version: 0.2.2
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.1/pyproject.toml` & `g3tables-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3tables"
-version = "0.2.1"
+version = "0.2.2"
 description = "G3 SW Definition, HW and PLC components, and Visualisation tables parser"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3tables-0.2.1/src/g3tables/__init__.py` & `g3tables-0.2.2/src/g3tables/__init__.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/plc_composition_io_table/_extend_table.py` & `g3tables-0.2.2/src/g3tables/plc_composition_io_table/_extend_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/plc_composition_io_table/_table.py` & `g3tables-0.2.2/src/g3tables/plc_composition_io_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/sw_definition_table/_table.py` & `g3tables-0.2.2/src/g3tables/sw_definition_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/_cli.py` & `g3tables-0.2.2/src/g3tables/system_config/_cli.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/_g3core_updater.py` & `g3tables-0.2.2/src/g3tables/system_config/_g3core_updater.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/_hw_connections.py` & `g3tables-0.2.2/src/g3tables/system_config/_hw_connections.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/_iomap_updater.py` & `g3tables-0.2.2/src/g3tables/system_config/_iomap_updater.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/_sw_system_dict_wrapper.py` & `g3tables-0.2.2/src/g3tables/system_config/_sw_system_dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/_system_config_processor.py` & `g3tables-0.2.2/src/g3tables/system_config/_system_config_processor.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/system_config/type_hinting.py` & `g3tables-0.2.2/src/g3tables/system_config/type_hinting.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/utils/_d2nd.py` & `g3tables-0.2.2/src/g3tables/utils/_d2nd.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/utils/_interval.py` & `g3tables-0.2.2/src/g3tables/utils/_interval.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/utils/gdrive/_gdrive.py` & `g3tables-0.2.2/src/g3tables/utils/gdrive/_gdrive.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/utils/gdrive/_update_creds.py` & `g3tables-0.2.2/src/g3tables/utils/gdrive/_update_creds.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.1/src/g3tables/visualization_table/_table.py` & `g3tables-0.2.2/src/g3tables/visualization_table/_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,36 +16,36 @@
     "Gate": "Gate_G3",
     "Route": "Route_G3",
     "Zone.Track": "Track",
     "Detector.TrackCircuit": "TC_G3",
     "Detector.Pantograph": "PD_G3",
     "Detector.MassDetector": "MD_G3",
     "Detector.UltrasonicSensor": "US_G3",
-    "Detector.VirtualDetector": "US_G3",
+    "Detector.VirtualDetector": "VD_G3",
     "PointMachine.PME": "PME_G3",
     "PointMachine.PMM": "PMM_G3",
     "Signal": "Signal_G3",
     "Signal.Symbol": "SignalSymbol_G3",
     "DoorDisplay7": "DoorDisplay7_G3",
     "Requestor.Digital": "RequestorDigital",
     "Requestor.RoutingTable": "RoutingTable_G3",
     "Requestor.Vecom": "VecomController_G3",
     "Requestor.Vecom.Loop": "VecomLoop_G3",
     "Requestor.DRR": "DRRController_G3",
     "Requestor.DRR.Transceiver": "DRRTransceiver_G3",
     "Requestor.SPIE": "SPIEController_G3",
     "Requestor.SPIE.Loop": "SPIELoop_G3",
     "Requestor.Vetra": "Vetra_G3",
-    "Requestor.Digital.AWA": "AWA_G3",
+    "Requestor.AWA": "AWA_G3",
     "Cabinet": "Cabinet_G3",
     "Cabinet.UPS": "CabinetUps_G3",
     "Cabinet.RFID": "CabinetRFID_G3",
     "Cabinet.Fuse": "CabinetFuse_G3",
     "Cabinet.Convertor": "CabinetConvertor_G3",
-    "Cabinet.MonitoringModule": "",
+    "Cabinet.MonitoringModule": "CabinetModule_G3",
     "Heating": "Heating_G3",
     "Heating.Contactor": "HeatingContactor_G3",
     "Heating.Contactor.Rod": "HeatingRod_G3",
     "Matrix": "MPS_G3",
     "GPIO": "GPIO_G3"
 }
```

### Comparing `g3tables-0.2.1/src/g3tables.egg-info/PKG-INFO` & `g3tables-0.2.2/src/g3tables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.1
+Version: 0.2.2
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.1/src/g3tables.egg-info/SOURCES.txt` & `g3tables-0.2.2/src/g3tables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

