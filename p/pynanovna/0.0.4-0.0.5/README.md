# Comparing `tmp/pynanovna-0.0.4.tar.gz` & `tmp/pynanovna-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynanovna-0.0.4.tar", last modified: Fri Apr 26 15:59:09 2024, max compression
+gzip compressed data, was "pynanovna-0.0.5.tar", last modified: Sat May  4 14:42:23 2024, max compression
```

## Comparing `pynanovna-0.0.4.tar` & `pynanovna-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 15:59:09.451468 pynanovna-0.0.4/
--rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.4/LICENCE
--rw-r--r--   0 teo        (501) staff       (20)     1089 2024-04-26 15:59:09.450571 pynanovna-0.0.4/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      432 2024-04-26 13:34:36.000000 pynanovna-0.0.4/README.md
--rw-r--r--   0 teo        (501) staff       (20)      637 2024-04-26 15:59:02.000000 pynanovna-0.0.4/pyproject.toml
--rw-r--r--   0 teo        (501) staff       (20)       38 2024-04-26 15:59:09.451604 pynanovna-0.0.4/setup.cfg
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 15:59:09.428486 pynanovna-0.0.4/src/
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 15:59:09.435413 pynanovna-0.0.4/src/pynanovna/
--rw-r--r--   0 teo        (501) staff       (20)    16118 2024-04-25 06:18:47.000000 pynanovna-0.0.4/src/pynanovna/Calibration.py
--rw-r--r--   0 teo        (501) staff       (20)     9117 2024-04-25 06:12:43.000000 pynanovna-0.0.4/src/pynanovna/CalibrationGuide.py
--rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.4/src/pynanovna/RFTools.py
--rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.4/src/pynanovna/SITools.py
--rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.4/src/pynanovna/Sweep.py
--rw-r--r--   0 teo        (501) staff       (20)    11225 2024-04-26 15:31:08.000000 pynanovna-0.0.4/src/pynanovna/SweepWorker.py
--rw-r--r--   0 teo        (501) staff       (20)     9655 2024-04-26 14:30:43.000000 pynanovna-0.0.4/src/pynanovna/Touchstone.py
--rw-r--r--   0 teo        (501) staff       (20)       80 2024-04-26 13:14:50.000000 pynanovna-0.0.4/src/pynanovna/__init__.py
--rw-r--r--   0 teo        (501) staff       (20)      236 2024-04-26 13:49:13.000000 pynanovna-0.0.4/src/pynanovna/example.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 15:59:09.449292 pynanovna-0.0.4/src/pynanovna/hardware/
--rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/AVNA.py
--rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/Hardware.py
--rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/JNCRadio_VNA_3G.py
--rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA.py
--rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA_F.py
--rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA_F_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA_H.py
--rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA_H4.py
--rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/SV4401A.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/SV6301A.py
--rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/Serial.py
--rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/TinySA.py
--rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/VNA.py
--rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.4/src/pynanovna/hardware/Version.py
--rw-r--r--   0 teo        (501) staff       (20)     9051 2024-04-26 15:57:41.000000 pynanovna-0.0.4/src/pynanovna/pynanovna.py
--rw-r--r--   0 teo        (501) staff       (20)     5906 2024-04-25 11:38:52.000000 pynanovna-0.0.4/src/pynanovna/vis.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-04-26 15:59:09.449967 pynanovna-0.0.4/src/pynanovna.egg-info/
--rw-r--r--   0 teo        (501) staff       (20)     1089 2024-04-26 15:59:09.000000 pynanovna-0.0.4/src/pynanovna.egg-info/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)     1033 2024-04-26 15:59:09.000000 pynanovna-0.0.4/src/pynanovna.egg-info/SOURCES.txt
--rw-r--r--   0 teo        (501) staff       (20)        1 2024-04-26 15:59:09.000000 pynanovna-0.0.4/src/pynanovna.egg-info/dependency_links.txt
--rw-r--r--   0 teo        (501) staff       (20)       60 2024-04-26 15:59:09.000000 pynanovna-0.0.4/src/pynanovna.egg-info/requires.txt
--rw-r--r--   0 teo        (501) staff       (20)       10 2024-04-26 15:59:09.000000 pynanovna-0.0.4/src/pynanovna.egg-info/top_level.txt
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.060435 pynanovna-0.0.5/
+-rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.5/LICENCE
+-rw-r--r--   0 teo        (501) staff       (20)     1333 2024-05-04 14:42:23.059227 pynanovna-0.0.5/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)      676 2024-05-04 14:41:16.000000 pynanovna-0.0.5/README.md
+-rw-r--r--   0 teo        (501) staff       (20)      637 2024-05-04 14:21:36.000000 pynanovna-0.0.5/pyproject.toml
+-rw-r--r--   0 teo        (501) staff       (20)       38 2024-05-04 14:42:23.060787 pynanovna-0.0.5/setup.cfg
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.035294 pynanovna-0.0.5/src/
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.043606 pynanovna-0.0.5/src/pynanovna/
+-rw-r--r--   0 teo        (501) staff       (20)    16095 2024-05-04 11:44:22.000000 pynanovna-0.0.5/src/pynanovna/Calibration.py
+-rw-r--r--   0 teo        (501) staff       (20)     8952 2024-05-04 11:44:22.000000 pynanovna-0.0.5/src/pynanovna/CalibrationGuide.py
+-rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.5/src/pynanovna/RFTools.py
+-rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.5/src/pynanovna/SITools.py
+-rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.5/src/pynanovna/Sweep.py
+-rw-r--r--   0 teo        (501) staff       (20)    11096 2024-05-04 13:32:02.000000 pynanovna-0.0.5/src/pynanovna/SweepWorker.py
+-rw-r--r--   0 teo        (501) staff       (20)     8824 2024-05-04 11:44:22.000000 pynanovna-0.0.5/src/pynanovna/Touchstone.py
+-rw-r--r--   0 teo        (501) staff       (20)      101 2024-05-04 14:14:44.000000 pynanovna-0.0.5/src/pynanovna/__init__.py
+-rw-r--r--   0 teo        (501) staff       (20)      653 2024-05-04 14:20:41.000000 pynanovna-0.0.5/src/pynanovna/example.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.057460 pynanovna-0.0.5/src/pynanovna/hardware/
+-rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/AVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/Hardware.py
+-rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/JNCRadio_VNA_3G.py
+-rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_F.py
+-rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_F_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_H.py
+-rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_H4.py
+-rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/SV4401A.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/SV6301A.py
+-rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/Serial.py
+-rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/TinySA.py
+-rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/VNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/Version.py
+-rw-r--r--   0 teo        (501) staff       (20)    10060 2024-05-04 13:34:06.000000 pynanovna-0.0.5/src/pynanovna/pynanovna.py
+-rw-r--r--   0 teo        (501) staff       (20)     3973 2024-05-04 14:02:01.000000 pynanovna-0.0.5/src/pynanovna/vis.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.058238 pynanovna-0.0.5/src/pynanovna.egg-info/
+-rw-r--r--   0 teo        (501) staff       (20)     1333 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)     1033 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/SOURCES.txt
+-rw-r--r--   0 teo        (501) staff       (20)        1 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/dependency_links.txt
+-rw-r--r--   0 teo        (501) staff       (20)       60 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/requires.txt
+-rw-r--r--   0 teo        (501) staff       (20)       10 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/top_level.txt
```

### Comparing `pynanovna-0.0.4/LICENCE` & `pynanovna-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/PKG-INFO` & `pynanovna-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,12 +16,24 @@
 Requires-Dist: pyserial>=3.5
 Requires-Dist: scipy>=1.13.0
 
 # pynanovna
 This is a python module for using a NanoVNA.
 
 ## Installation
-Install with `pip install pynanovna` or `pip3 install pynanovna`
+Install with `pip install pynanovna` or `pip3 install pynanovna`.
+
+## Example
+```
+import pynanovna
+
+worker = pynanovna.NanoVNAWorker()
+stream = worker.stream_data(datafile)
+for sweep in stream:
+    print(sweep)
+```
+
+See `src/pynanovna/example.py` for a more detailed example on some use cases of the project.
+
 
 ## History
 Originally this was the fork [nanovna-saver-headless](https://github.com/PICC-Group/nanovna-saver-headless) from [nanovna-saver](https://github.com/NanoVNA-Saver/nanovna-saver) but when that project no longer shared much code with the original we decided to create a new project.
-
```

### Comparing `pynanovna-0.0.4/pyproject.toml` & `pynanovna-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pynanovna"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name = "Teo Bergkvist", email = "bergkvist.teo@protonmail.com" },
 ]
 description = "A package to use a NanoVNA"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `pynanovna-0.0.4/src/pynanovna/Calibration.py` & `pynanovna-0.0.5/src/pynanovna/Calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,16 +319,15 @@
             try:
                 self._calc_port_1(freq, caldata)
                 if self.isValid2Port():
                     self._calc_port_2(freq, caldata)
             except ZeroDivisionError as exc:
                 self.isCalculated = False
                 print(
-                    "Division error - did you use the same measurement"
-                    " for two of short, open and load?"
+                    "Division error - did you use the same measurement for two of short, open and load?"
                 )
                 raise ValueError(
                     f"Two of short, open and load returned the same"
                     f" values at frequency {freq}Hz."
                 ) from exc
 
         self.gen_interpolation()
```

### Comparing `pynanovna-0.0.4/src/pynanovna/CalibrationGuide.py` & `pynanovna-0.0.5/src/pynanovna/CalibrationGuide.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,26 +111,19 @@
             print("Save failed: ", e)
             return False
 
     def automaticCalibration(self):
         response = input(
             """Calibration assistant,
             
-                This calibration assistant will help you create a calibration\n
-                in the NanoVNASaver application. It will sweep the\n
-                standards for you and guide you through the process.<br><br>\n
-                Before starting, ensure you have Open, Short and Load\n
-                standards available and the cables you wish to have\n
-                calibrated connected to the device.<br><br>\n
+                This calibration assistant will help you create a calibration in the NanoVNASaver application. It will sweep the standards for you and guide you through the process.\n
+                Before starting, ensure you have Open, Short and Load standards available and the cables you wish to have calibrated connected to the device.\n
                 Make sure sweep is NOT in continuous mode.\n
-                If you want a 2-port calibration, also have a through\n
-                connector on hand.<br><br>\n
-                <b>The best results are achieved by having the NanoVNA\n
-                calibrated on-device for the full span of interest and stored\n
-                in save slot 0 before starting.</b><br><br>\n\n
+                If you want a 2-port calibration, also have a through connector on hand.\n
+                The best results are achieved by having the NanoVNA calibrated on-device for the full span of interest and stored in save slot 0 before starting.\n\n
                 Once you are ready to proceed, press enter. (q to quit)."""
         )
 
         if response.lower() == "q":
             return False
         print("Starting automatic calibration assistant.")
         if not self.vna.connected():
```

### Comparing `pynanovna-0.0.4/src/pynanovna/RFTools.py` & `pynanovna-0.0.5/src/pynanovna/RFTools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/SITools.py` & `pynanovna-0.0.5/src/pynanovna/SITools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/Sweep.py` & `pynanovna-0.0.5/src/pynanovna/Sweep.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/SweepWorker.py` & `pynanovna-0.0.5/src/pynanovna/SweepWorker.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .RFTools import Datapoint
 
 
 def truncate(values: list[list[tuple]], count: int, verbose=False) -> list[list[tuple]]:
     """truncate drops extrema from data list if averaging is active"""
     keep = len(values) - count
     if verbose:
-        print("Truncating from %d values to %d", len(values), keep)
+        print(f"Truncating from {len(values)} values to {keep}")
     if count < 1 or keep < 1:
         if verbose:
             print("Not doing illegal truncate")
         return values
     truncated = []
     for valueset in np.swapaxes(values, 0, 1).tolist():
         avg = complex(*np.average(valueset, 0))
@@ -52,15 +52,15 @@
             if self.s21att > 0:
                 self.data.s21 = corr_att_data(self.data.s21, self.s21att)
 
     def run(self) -> None:
         try:
             self._run()
         except BaseException as exc:
-            print("%s", exc)
+            print(exc)
             print(f"ERROR during sweep\n\nStopped\n\n{exc}")
             if self.verbose:
                 raise exc
 
     def _run(self) -> None:
         if self.verbose:
             print("Initializing SweepWorker")
@@ -81,34 +81,34 @@
 
         self._run_loop()
 
         if sweep.segments > 1:
             start = sweep.start
             end = sweep.end
             if self.verbose:
-                print("Resetting NanoVNA sweep to full range: %d to %d", start, end)
+                print(f"Resetting NanoVNA sweep to full range: {start} to {end}")
             self.vna.resetSweep(start, end)
 
         self.percentage = 100
         if self.verbose:
             print("Sweep is finished.")
         self.running = False
 
     def _run_loop(self) -> None:
         sweep = self.sweep
         averages = (
             sweep.properties.averages[0] if sweep.properties.mode == "AVERAGE" else 1
         )
         if self.verbose:
-            print("%d averages", averages)
+            print("Averages: ", averages)
 
         while True:
             for i in range(sweep.segments):
                 if self.verbose:
-                    print("Sweep segment no %d", i)
+                    print(f"Sweep segment no {i}")
                 if not self.running:
                     if self.verbose:
                         print("Stopping sweeping as signalled")
                     break
                 start, stop = sweep.get_index_range(i)
 
                 freq, values11, values21 = self.readAveragedSegment(
@@ -126,45 +126,43 @@
         self.rawData21 = []
         for freq in self.sweep.get_frequencies():
             self.data11.append(Datapoint(freq, 0.0, 0.0))
             self.data21.append(Datapoint(freq, 0.0, 0.0))
             self.rawData11.append(Datapoint(freq, 0.0, 0.0))
             self.rawData21.append(Datapoint(freq, 0.0, 0.0))
         if self.verbose:
-            print("Init data length: %s", len(self.data11))
+            print("Init data length: ", len(self.data11))
 
     def updateData(self, frequencies, values11, values21, index):
         # Update the data from (i*101) to (i+1)*101
         if self.verbose:
-            print("Calculating data and inserting in existing data at index %d", index)
+            print(f"Calculating data and inserting in existing data at index {index}")
         offset = self.sweep.points * index
 
         raw_data11 = [
             Datapoint(freq, values11[i][0], values11[i][1])
             for i, freq in enumerate(frequencies)
         ]
         raw_data21 = [
             Datapoint(freq, values21[i][0], values21[i][1])
             for i, freq in enumerate(frequencies)
         ]
 
         data11, data21 = self.applyCalibration(raw_data11, raw_data21)
         if self.verbose:
-            print("update Freqs: %s, Offset: %s", len(frequencies), offset)
+            print(f"update Freqs: {len(frequencies)}, Offset: {offset}")
         for i in range(len(frequencies)):
             self.data11[offset + i] = data11[i]
             self.data21[offset + i] = data21[i]
             self.rawData11[offset + i] = raw_data11[i]
             self.rawData21[offset + i] = raw_data21[i]
 
         if self.verbose:
             print(
-                "Saving data to application (%d and %d points)",
-                len(self.data11),
-                len(self.data21),
+                f"Saving data to application ({len(self.data11)} and {len(self.data21)} points)"
             )
         self.saveData(self.data11, self.data21)
 
     def applyCalibration(
         self, raw_data11: list[Datapoint], raw_data21: list[Datapoint]
     ) -> tuple[list[Datapoint], list[Datapoint]]:
         data11: list[Datapoint] = []
@@ -197,115 +195,113 @@
         return data11, data21
 
     def readAveragedSegment(self, start, stop, averages=1):
         values11 = []
         values21 = []
         freq = []
         if self.verbose:
-            print("Reading from %d to %d. Averaging %d values", start, stop, averages)
+            print(f"Reading from {start} to {stop}. Averaging {averages} values")
         for i in range(averages):
             if not self.running:
                 if self.verbose:
                     print("Stopping averaging as signalled.")
                 if averages == 1:
                     break
                 if self.verbose:
                     print("Stop during average. Discarding sweep result.")
                 return [], [], []
             if self.verbose:
-                print("Reading average no %d / %d", i + 1, averages)
+                print(f"Reading average no {i + 1} / {averages}")
             retry = 0
             tmp11 = []
             tmp21 = []
             while not tmp11 and retry < 5:
                 sleep(0.5 * retry)
                 retry += 1
                 freq, tmp11, tmp21 = self.readSegment(start, stop)
                 if retry > 1:
                     if self.verbose:
-                        print("retry %s readSegment(%s,%s)", retry, start, stop)
+                        print(f"retry {retry} readSegment({start}, {stop})")
                     sleep(0.5)
             values11.append(tmp11)
             values21.append(tmp21)
             self.percentage += 100 / (self.sweep.segments * averages)
 
         if not values11:
             raise IOError("Invalid data during swwep")
 
         truncates = self.sweep.properties.averages[1]
         if truncates > 0 and averages > 1:
             if self.verbose:
-                print("Truncating %d values by %d", len(values11), truncates)
+                print(f"Truncating {len(values11)} values by {truncates}")
             values11 = truncate(values11, truncates)
             values21 = truncate(values21, truncates)
 
         if self.verbose:
-            print("Averaging %d values", len(values11))
+            print(f"Averaging {len(values11)} values")
         values11 = np.average(values11, 0).tolist()
         values21 = np.average(values21, 0).tolist()
 
         return freq, values11, values21
 
     def readSegment(self, start, stop):
         if self.verbose:
-            print("Setting sweep range to %d to %d", start, stop)
+            print(f"Setting sweep range to {start} to {stop}")
         self.vna.setSweep(start, stop)
 
         frequencies = self.vna.readFrequencies()
         if self.verbose:
-            print("Read %s frequencies", len(frequencies))
+            print(f"Read {len(frequencies)} frequencies")
         values11 = self.readData("data 0")
         values21 = self.readData("data 1")
         if not len(frequencies) == len(values11) == len(values21):
             if self.verbose:
                 print("No valid data during this run")
             return [], [], []
         return frequencies, values11, values21
 
     def readData(self, data):
         if self.verbose:
-            print("Reading %s", data)
+            print("Reading ", data)
         done = False
         returndata = []
         count = 0
         while not done:
             done = True
             returndata = []
             tmpdata = self.vna.readValues(data)
             if self.verbose:
-                print("Read %d values", len(tmpdata))
+                print(f"Read {len(tmpdata)} values")
             for d in tmpdata:
                 a, b = d.split(" ")
                 try:
                     if self.vna.validateInput and (
                         abs(float(a)) > 9.5 or abs(float(b)) > 9.5
                     ):
                         if self.verbose:
-                            print("Got a non plausible data value: (%s)", d)
+                            print("Got a non plausible data value: ", d)
                         done = False
                         break
                     returndata.append((float(a), float(b)))
                 except ValueError as exc:
-                    print("An exception occurred reading %s: %s", data, exc)
+                    print(f"An exception occurred reading {data}: {exc}", data, exc)
                     done = False
             if not done:
                 if self.verbose:
-                    print("Re-reading %s", data)
+                    print("Re-reading ", data)
                 sleep(0.2)
                 count += 1
                 if count == 5:
                     if self.verbose:
-                        print("Tried and failed to read %s %d times.", data, count)
+                        print(f"Tried and failed to read {data} {count} times.")
                     if self.verbose:
                         print("trying to reconnect")
                     self.vna.reconnect()
                 if count >= 10:
-                    print(
-                        "Tried and failed to read %s %d times. Giving up.", data, count
-                    )
+                    print(f"Tried and failed to read {data} {count} times. Giving up.")
                     raise IOError(
                         f"Failed reading {data} {count} times.\n"
                         f"Data outside expected valid ranges,"
                         f" or in an unexpected format.\n\n"
                         f"You can disable data validation on the"
                         f"device settings screen."
                     )
```

### Comparing `pynanovna-0.0.4/src/pynanovna/Touchstone.py` & `pynanovna-0.0.5/src/pynanovna/Touchstone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-#  NanoVNASaver
-#
-#  A python program to view and export Touchstone data from a NanoVNA
-#  Copyright (C) 2019, 2020  Rune B. Broberg
-#  Copyright (C) 2020,2021 NanoVNA-Saver Authors
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
 import math
 import cmath
 import io
 from operator import attrgetter
 
 from scipy.interpolate import interp1d
```

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/AVNA.py` & `pynanovna-0.0.5/src/pynanovna/hardware/AVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/Hardware.py` & `pynanovna-0.0.5/src/pynanovna/hardware/Hardware.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/JNCRadio_VNA_3G.py` & `pynanovna-0.0.5/src/pynanovna/hardware/JNCRadio_VNA_3G.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA.py` & `pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/NanoVNA_V2.py` & `pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_V2.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/SV4401A.py` & `pynanovna-0.0.5/src/pynanovna/hardware/SV4401A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/SV6301A.py` & `pynanovna-0.0.5/src/pynanovna/hardware/SV6301A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/Serial.py` & `pynanovna-0.0.5/src/pynanovna/hardware/Serial.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/TinySA.py` & `pynanovna-0.0.5/src/pynanovna/hardware/TinySA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/VNA.py` & `pynanovna-0.0.5/src/pynanovna/hardware/VNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/hardware/Version.py` & `pynanovna-0.0.5/src/pynanovna/hardware/Version.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.4/src/pynanovna/pynanovna.py` & `pynanovna-0.0.5/src/pynanovna/pynanovna.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             self.iface = hw.get_interfaces()[vna_index]
         except IndexError:
             print("NanoVNA not found, is it connected? Entering playback mode.")
             self.playback_mode = True
         if not self.playback_mode:
             self.vna = hw.get_VNA(self.iface)
             self.calibration = Calibration()
-            self.touchstone = Touchstone("./output") #  Fix this.
+            self.touchstone = Touchstone("./output")  #  Fix this.
             self.worker = SweepWorker(
                 self.vna, self.calibration, self.touchstone, verbose=verbose
             )
             self.CalibrationGuide = CalibrationGuide(
                 self.calibration, self.worker, verbose
             )
             if self.verbose:
@@ -102,22 +102,27 @@
         """
         if not data_file:
             self._stream_data()
         sleep(2)
         try:
             if not data_file:
                 if self.playback_mode:
-                    print("Cannot stream data from NanoVNA in playback mode. Connect NanoVNA and restart.")
+                    print(
+                        "Cannot stream data from NanoVNA in playback mode. Connect NanoVNA and restart."
+                    )
                     return
                 stream = self._access_data()
             else:
                 stream = self._csv_streamer(data_file)
 
             for data in stream:
                 yield data  # Yield each piece of data as it comes
+
+        except KeyboardInterrupt:
+            self._stop_worker()
         except Exception as e:
             if self.verbose:
                 print("Exception in data stream: ", e)
         finally:
             if self.verbose:
                 print("Stopping worker.")
             self._stop_worker()
@@ -125,43 +130,57 @@
     def _stream_data(self):
         """Starts a thread for the sweep workers run function."""
         self.worker.sweep.set_mode("CONTINOUS")
         # Start the worker in a new thread
         self.worker_thread = threading.Thread(target=self.worker.run)
         self.worker_thread.start()
 
-    def _csv_streamer(self, filename, data_points=5):
+    def _csv_streamer(self, filename, sweepdivider="Sweepno"):
         """Stream previously recorded data from a csv file.
 
         Args:
             filename (string): Path to the csv file.
-            data_points (int): Number of lines that each sweep is stored as. Defaults to 5.
+            sweepdivider (string): Used to identify where sweeps end and start in the csv file.
 
         Yields:
-            list: [refl_re, refl_im, thru_re, thru_im, freq]
+            tuple: ([s11], [s21])
         """
         try:
             with open(filename) as f:
                 data = f.readlines()
+                package = ([], [])
                 for i, line in enumerate(data):
                     if i != 0:
-                        data_vals = [float(val) for val in line.split(",")]
-                        s11 = Datapoint(data_vals[-1], complex(data_vals[0]).real, complex(data_vals[0]).imag)
-                        s12 = Datapoint(data_vals[-1], complex(data_vals[1]).real, complex(data_vals[1]).imag)
-                        yield (s11, s12)
+                        if sweepdivider in line:
+                            if package != ([], []):
+                                yield package
+                            package = ([], [])
+                            continue
+                        data_vals = [complex(val) for val in line.split(",")]
+                        package[0].append(Datapoint(
+                            data_vals[-1].real,
+                            data_vals[0].real,
+                            data_vals[0].imag,
+                        ))
+                        package[1].append(Datapoint(
+                            data_vals[-1].real,
+                            data_vals[1].real,
+                            data_vals[1].imag,
+                        ))
+        except KeyboardInterrupt:
+            return
         except Exception as e:
             print(e)
 
     def _access_data(self):
         """Fetches the data from the sweep worker as long as it is running a sweep.
 
         Yields:
             list: List of data from the latest sweep.
         """
-        # Access data while the worker is running
         while self.worker.running:
             yield self._get_data()
 
     def _stop_worker(self):
         """Stop the sweep worker and kill the stream."""
         if self.verbose:
             print("NanoVNASaverHeadless is stopping sweepworker now.")
@@ -173,15 +192,15 @@
         """Get data from the sweep worker.
 
         Returns:
             list: Real Reflection, Imaginary Reflection, Real Through, Imaginary Through, Frequency
         """
         return self.worker.data11, self.worker.data21
 
-    def save_csv(self, filename, skip_start=5):
+    def save_csv(self, filename, skip_start=5, sweepdivider="Sweepno"):
         """Function to save the stream to a csv file.
 
         Args:
             filename (str): The filename to save to.
             nr_sweeps (int): Number of sweeps to run. Defaults to 10.
             skip_start (int): The NanoVNA usually gives bad data in the beginning, therefore this data can be skipped. Defaults to 5.
 
@@ -194,26 +213,39 @@
         try:
             if not isinstance(filename, str):
                 raise TypeError("Filename must be a string")
             if not filename.endswith(".csv"):
                 filename += ".csv"
             file_path = filename
             old_data = [[Datapoint(1, 1.0, 1.0)]]
-            counter = 0 #  Counter because NanoVNA sends out incorrect data the first few times.
+            counter = 0  #  Counter because NanoVNA sends out incorrect data the first few times.
             with open(file_path, mode="w", newline="") as file:
                 writer = csv.writer(file)
                 writer.writerow(["Refl", "Thru", "Freq"])
                 data_stream = self.stream_data()
                 for new_data in data_stream:
                     if new_data[0][0].im != old_data[0][0].im:
+                        writer.writerow([sweepdivider, counter])
                         counter += 1  # Increment counter when new_data is different
                         if counter > skip_start:
-                            for data_index in range(len(new_data)):
-                                writer.writerow([new_data[0][data_index].z, new_data[1][data_index].z, new_data[0][data_index].freq])
-                    old_data = (new_data[0].copy(), new_data[1].copy()) # Update old_data every iteration to the latest data
+                            for data_index in range(len(new_data[0])):
+                                writer.writerow(
+                                    [
+                                        new_data[:][0][data_index].z,
+                                        new_data[:][1][data_index].z,
+                                        new_data[:][0][data_index].freq,
+                                    ]
+                                )
+                    old_data = (
+                        new_data[0].copy(),
+                        new_data[1].copy(),
+                    )  # Update old_data every iteration to the latest data
+
+        except KeyboardInterrupt:
+            return
 
         except Exception as e:
             print("An error occurred: ", e)
 
     def kill(self):
         """Disconnect the NanoVNA.
```

### Comparing `pynanovna-0.0.4/src/pynanovna.egg-info/PKG-INFO` & `pynanovna-0.0.5/src/pynanovna.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -16,12 +16,24 @@
 Requires-Dist: pyserial>=3.5
 Requires-Dist: scipy>=1.13.0
 
 # pynanovna
 This is a python module for using a NanoVNA.
 
 ## Installation
-Install with `pip install pynanovna` or `pip3 install pynanovna`
+Install with `pip install pynanovna` or `pip3 install pynanovna`.
+
+## Example
+```
+import pynanovna
+
+worker = pynanovna.NanoVNAWorker()
+stream = worker.stream_data(datafile)
+for sweep in stream:
+    print(sweep)
+```
+
+See `src/pynanovna/example.py` for a more detailed example on some use cases of the project.
+
 
 ## History
 Originally this was the fork [nanovna-saver-headless](https://github.com/PICC-Group/nanovna-saver-headless) from [nanovna-saver](https://github.com/NanoVNA-Saver/nanovna-saver) but when that project no longer shared much code with the original we decided to create a new project.
-
```

### Comparing `pynanovna-0.0.4/src/pynanovna.egg-info/SOURCES.txt` & `pynanovna-0.0.5/src/pynanovna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

