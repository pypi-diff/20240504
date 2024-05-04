# Comparing `tmp/UliEngineering-0.4.8.tar.gz` & `tmp/UliEngineering-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UliEngineering-0.4.8.tar", last modified: Sat Sep 23 02:08:46 2023, max compression
+gzip compressed data, was "UliEngineering-0.4.9.tar", last modified: Sat Sep 23 02:34:55 2023, max compression
```

## Comparing `UliEngineering-0.4.8.tar` & `UliEngineering-0.4.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.548989 UliEngineering-0.4.8/
--rw-rw-r--   0 uli       (1000) uli       (1000)    11342 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/LICENSE
--rw-rw-r--   0 uli       (1000) uli       (1000)     1038 2023-09-23 02:08:46.548989 UliEngineering-0.4.8/PKG-INFO
--rw-rw-r--   0 uli       (1000) uli       (1000)     7000 2023-09-17 22:55:14.000000 UliEngineering-0.4.8/README.md
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.532989 UliEngineering-0.4.8/UliEngineering/
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.536989 UliEngineering-0.4.8/UliEngineering/Economics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     3661 2022-02-21 16:48:03.000000 UliEngineering-0.4.8/UliEngineering/Economics/Interest.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-02-21 16:48:03.000000 UliEngineering-0.4.8/UliEngineering/Economics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.540989 UliEngineering-0.4.8/UliEngineering/Electronics/
--rwxr-xr-x   0 uli       (1000) uli       (1000)     1798 2021-09-18 02:45:54.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Capacitors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     5427 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Crystal.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1124 2023-09-23 00:50:53.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Filter.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     7882 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Hysteresis.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)      753 2021-09-18 02:45:54.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Inductors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2663 2023-07-29 15:48:40.000000 UliEngineering-0.4.8/UliEngineering/Electronics/LED.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)     2669 2023-09-17 01:42:26.000000 UliEngineering-0.4.8/UliEngineering/Electronics/MOSFET.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     7077 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Microstrip.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1637 2023-09-17 22:36:55.000000 UliEngineering-0.4.8/UliEngineering/Electronics/OpAmp.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      873 2022-06-19 16:15:14.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Power.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Electronics/PowerFactor.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)      786 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Reactance.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     6498 2023-07-29 15:48:40.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Resistors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6543 2022-06-19 16:15:55.000000 UliEngineering-0.4.8/UliEngineering/Electronics/TemperatureCoefficient.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      884 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Electronics/Tolerance.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     5948 2022-02-21 16:48:03.000000 UliEngineering-0.4.8/UliEngineering/Electronics/VoltageDivider.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Electronics/__init__.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)    21499 2022-06-19 16:45:11.000000 UliEngineering-0.4.8/UliEngineering/EngineerIO.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      534 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Exceptions.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.540989 UliEngineering-0.4.8/UliEngineering/Filesystem/
--rw-rw-r--   0 uli       (1000) uli       (1000)     4122 2023-07-29 15:48:40.000000 UliEngineering-0.4.8/UliEngineering/Filesystem/Hash.py
--rw-rw-r--   0 uli       (1000) uli       (1000)       22 2023-07-28 16:52:38.000000 UliEngineering-0.4.8/UliEngineering/Filesystem/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2622 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Length.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.540989 UliEngineering-0.4.8/UliEngineering/Math/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1890 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Math/Coordinates.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2885 2023-03-13 04:42:02.000000 UliEngineering-0.4.8/UliEngineering/Math/Decibel.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.540989 UliEngineering-0.4.8/UliEngineering/Math/Geometry/
--rw-rw-r--   0 uli       (1000) uli       (1000)      591 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Math/Geometry/Circle.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3668 2023-07-28 16:51:33.000000 UliEngineering-0.4.8/UliEngineering/Math/Geometry/Cylinder.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1588 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Math/Geometry/Polygon.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1113 2022-09-15 15:07:11.000000 UliEngineering-0.4.8/UliEngineering/Math/Geometry/Sphere.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Math/Geometry/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Math/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.540989 UliEngineering-0.4.8/UliEngineering/Mechanics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1493 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Mechanics/Threads.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Mechanics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.544989 UliEngineering-0.4.8/UliEngineering/Physics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1968 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/Acceleration.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3378 2023-07-28 16:51:33.000000 UliEngineering-0.4.8/UliEngineering/Physics/Density.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      953 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/Frequency.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)     1835 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/Physics/JohnsonNyquistNoise.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)     1023 2022-06-19 16:44:08.000000 UliEngineering-0.4.8/UliEngineering/Physics/Light.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      991 2023-02-04 03:03:35.000000 UliEngineering-0.4.8/UliEngineering/Physics/MagneticResonance.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1451 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/NTC.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)     1012 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/Physics/NoiseDensity.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1355 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/Pressure.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)     2234 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/Physics/RF.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     4945 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/RTD.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2175 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/Rotation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2489 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/Temperature.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Physics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.544989 UliEngineering-0.4.8/UliEngineering/SignalProcessing/
--rw-rw-r--   0 uli       (1000) uli       (1000)     8963 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Chunks.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      492 2022-06-19 16:20:02.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Correlation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1747 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/DateTime.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)    12299 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/FFT.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    11911 2023-07-29 15:48:40.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Filter.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3030 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Normalize.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     9022 2022-02-21 16:48:04.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Resampling.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    19078 2022-06-19 16:20:22.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Selection.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)     2446 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Simulation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     9831 2022-02-21 16:48:04.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Utils.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1710 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Weight.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3332 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/Window.py
--rw-rw-r--   0 uli       (1000) uli       (1000)       22 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/SignalProcessing/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2081 2022-02-21 16:48:02.000000 UliEngineering-0.4.8/UliEngineering/Units.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.548989 UliEngineering-0.4.8/UliEngineering/Utils/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1145 2023-07-28 17:30:02.000000 UliEngineering-0.4.8/UliEngineering/Utils/Compression.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      662 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/Concurrency.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    11944 2023-07-28 16:51:33.000000 UliEngineering-0.4.8/UliEngineering/Utils/Date.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6193 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/Files.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3687 2022-02-21 16:48:04.000000 UliEngineering-0.4.8/UliEngineering/Utils/Iterable.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      606 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/JSON.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6972 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/NumPy.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      664 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/Parser.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1806 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/Range.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      286 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/Slice.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1348 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/String.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2372 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/Temporary.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2621 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/ZIP.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      104 2021-12-18 02:10:48.000000 UliEngineering-0.4.8/UliEngineering/Utils/__init__.py
--rwxr-xr-x   0 uli       (1000) uli       (1000)       23 2021-09-18 02:45:55.000000 UliEngineering-0.4.8/UliEngineering/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:08:46.536989 UliEngineering-0.4.8/UliEngineering.egg-info/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1038 2023-09-23 02:08:46.000000 UliEngineering-0.4.8/UliEngineering.egg-info/PKG-INFO
--rw-rw-r--   0 uli       (1000) uli       (1000)     3063 2023-09-23 02:08:46.000000 UliEngineering-0.4.8/UliEngineering.egg-info/SOURCES.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)        1 2023-09-23 02:08:46.000000 UliEngineering-0.4.8/UliEngineering.egg-info/dependency_links.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)       56 2023-09-23 02:08:46.000000 UliEngineering-0.4.8/UliEngineering.egg-info/requires.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)       15 2023-09-23 02:08:46.000000 UliEngineering-0.4.8/UliEngineering.egg-info/top_level.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)      100 2023-09-23 02:08:46.548989 UliEngineering-0.4.8/setup.cfg
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1578 2023-09-23 02:08:21.000000 UliEngineering-0.4.8/setup.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.487879 UliEngineering-0.4.9/
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11342 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/LICENSE
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1038 2023-09-23 02:34:55.487879 UliEngineering-0.4.9/PKG-INFO
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7000 2023-09-17 22:55:14.000000 UliEngineering-0.4.9/README.md
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.475879 UliEngineering-0.4.9/UliEngineering/
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.479879 UliEngineering-0.4.9/UliEngineering/Economics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3661 2022-02-21 16:48:03.000000 UliEngineering-0.4.9/UliEngineering/Economics/Interest.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-02-21 16:48:03.000000 UliEngineering-0.4.9/UliEngineering/Economics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.479879 UliEngineering-0.4.9/UliEngineering/Electronics/
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1798 2021-09-18 02:45:54.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Capacitors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     5427 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Crystal.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2130 2023-09-23 02:34:10.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Filter.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7882 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Hysteresis.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)      753 2021-09-18 02:45:54.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Inductors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2663 2023-07-29 15:48:40.000000 UliEngineering-0.4.9/UliEngineering/Electronics/LED.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     2669 2023-09-17 01:42:26.000000 UliEngineering-0.4.9/UliEngineering/Electronics/MOSFET.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7077 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Microstrip.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1637 2023-09-17 22:36:55.000000 UliEngineering-0.4.9/UliEngineering/Electronics/OpAmp.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      873 2022-06-19 16:15:14.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Power.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Electronics/PowerFactor.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)      786 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Reactance.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     6498 2023-07-29 15:48:40.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Resistors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6543 2022-06-19 16:15:55.000000 UliEngineering-0.4.9/UliEngineering/Electronics/TemperatureCoefficient.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      884 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Electronics/Tolerance.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     5948 2022-02-21 16:48:03.000000 UliEngineering-0.4.9/UliEngineering/Electronics/VoltageDivider.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Electronics/__init__.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)    21499 2022-06-19 16:45:11.000000 UliEngineering-0.4.9/UliEngineering/EngineerIO.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      534 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Exceptions.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.479879 UliEngineering-0.4.9/UliEngineering/Filesystem/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     4122 2023-07-29 15:48:40.000000 UliEngineering-0.4.9/UliEngineering/Filesystem/Hash.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)       22 2023-07-28 16:52:38.000000 UliEngineering-0.4.9/UliEngineering/Filesystem/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2622 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Length.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.479879 UliEngineering-0.4.9/UliEngineering/Math/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1890 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Math/Coordinates.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2885 2023-03-13 04:42:02.000000 UliEngineering-0.4.9/UliEngineering/Math/Decibel.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.483879 UliEngineering-0.4.9/UliEngineering/Math/Geometry/
+-rw-rw-r--   0 uli       (1000) uli       (1000)      591 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Math/Geometry/Circle.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3668 2023-07-28 16:51:33.000000 UliEngineering-0.4.9/UliEngineering/Math/Geometry/Cylinder.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1588 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Math/Geometry/Polygon.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1113 2022-09-15 15:07:11.000000 UliEngineering-0.4.9/UliEngineering/Math/Geometry/Sphere.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Math/Geometry/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Math/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.483879 UliEngineering-0.4.9/UliEngineering/Mechanics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1493 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Mechanics/Threads.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Mechanics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.483879 UliEngineering-0.4.9/UliEngineering/Physics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1968 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/Acceleration.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3378 2023-07-28 16:51:33.000000 UliEngineering-0.4.9/UliEngineering/Physics/Density.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      953 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/Frequency.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1835 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/Physics/JohnsonNyquistNoise.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1023 2022-06-19 16:44:08.000000 UliEngineering-0.4.9/UliEngineering/Physics/Light.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      991 2023-02-04 03:03:35.000000 UliEngineering-0.4.9/UliEngineering/Physics/MagneticResonance.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1451 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/NTC.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     1012 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/Physics/NoiseDensity.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1355 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/Pressure.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     2234 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/Physics/RF.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     4945 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/RTD.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2175 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/Rotation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2489 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/Temperature.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Physics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.487879 UliEngineering-0.4.9/UliEngineering/SignalProcessing/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     8963 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Chunks.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      492 2022-06-19 16:20:02.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Correlation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1747 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/DateTime.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)    12299 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/FFT.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11911 2023-07-29 15:48:40.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Filter.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3030 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Normalize.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     9022 2022-02-21 16:48:04.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Resampling.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    19078 2022-06-19 16:20:22.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Selection.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)     2446 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Simulation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     9831 2022-02-21 16:48:04.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Utils.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1710 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Weight.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3332 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/Window.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)       22 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/SignalProcessing/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2081 2022-02-21 16:48:02.000000 UliEngineering-0.4.9/UliEngineering/Units.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.487879 UliEngineering-0.4.9/UliEngineering/Utils/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1145 2023-07-28 17:30:02.000000 UliEngineering-0.4.9/UliEngineering/Utils/Compression.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      662 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/Concurrency.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11944 2023-07-28 16:51:33.000000 UliEngineering-0.4.9/UliEngineering/Utils/Date.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6193 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/Files.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3687 2022-02-21 16:48:04.000000 UliEngineering-0.4.9/UliEngineering/Utils/Iterable.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      606 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/JSON.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6972 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/NumPy.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      664 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/Parser.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1806 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/Range.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      286 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/Slice.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1348 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/String.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2372 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/Temporary.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2621 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/ZIP.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      104 2021-12-18 02:10:48.000000 UliEngineering-0.4.9/UliEngineering/Utils/__init__.py
+-rwxr-xr-x   0 uli       (1000) uli       (1000)       23 2021-09-18 02:45:55.000000 UliEngineering-0.4.9/UliEngineering/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-09-23 02:34:55.475879 UliEngineering-0.4.9/UliEngineering.egg-info/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1038 2023-09-23 02:34:55.000000 UliEngineering-0.4.9/UliEngineering.egg-info/PKG-INFO
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3063 2023-09-23 02:34:55.000000 UliEngineering-0.4.9/UliEngineering.egg-info/SOURCES.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)        1 2023-09-23 02:34:55.000000 UliEngineering-0.4.9/UliEngineering.egg-info/dependency_links.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)       56 2023-09-23 02:34:55.000000 UliEngineering-0.4.9/UliEngineering.egg-info/requires.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)       15 2023-09-23 02:34:55.000000 UliEngineering-0.4.9/UliEngineering.egg-info/top_level.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)      100 2023-09-23 02:34:55.491879 UliEngineering-0.4.9/setup.cfg
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1578 2023-09-23 02:34:37.000000 UliEngineering-0.4.9/setup.py
```

### Comparing `UliEngineering-0.4.8/LICENSE` & `UliEngineering-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/PKG-INFO` & `UliEngineering-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UliEngineering
-Version: 0.4.8
+Version: 0.4.9
 Summary: Computational tools for electronics engineering
 Home-page: https://techoverflow.net/
 Author: Uli Köhler
 Author-email: ukoehler@techoverflow.net
 License: Apache License v2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `UliEngineering-0.4.8/README.md` & `UliEngineering-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Economics/Interest.py` & `UliEngineering-0.4.9/UliEngineering/Economics/Interest.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Capacitors.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Capacitors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Crystal.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Crystal.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Hysteresis.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Hysteresis.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Inductors.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Inductors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/LED.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/LED.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/MOSFET.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/MOSFET.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Microstrip.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Microstrip.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/OpAmp.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/OpAmp.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Power.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Power.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/PowerFactor.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/PowerFactor.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Reactance.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Reactance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Resistors.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Resistors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/TemperatureCoefficient.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/TemperatureCoefficient.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/Tolerance.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/Tolerance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Electronics/VoltageDivider.py` & `UliEngineering-0.4.9/UliEngineering/Electronics/VoltageDivider.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/EngineerIO.py` & `UliEngineering-0.4.9/UliEngineering/EngineerIO.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Exceptions.py` & `UliEngineering-0.4.9/UliEngineering/Exceptions.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Filesystem/Hash.py` & `UliEngineering-0.4.9/UliEngineering/Filesystem/Hash.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Length.py` & `UliEngineering-0.4.9/UliEngineering/Length.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Math/Coordinates.py` & `UliEngineering-0.4.9/UliEngineering/Math/Coordinates.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Math/Decibel.py` & `UliEngineering-0.4.9/UliEngineering/Math/Decibel.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Math/Geometry/Circle.py` & `UliEngineering-0.4.9/UliEngineering/Math/Geometry/Circle.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Math/Geometry/Cylinder.py` & `UliEngineering-0.4.9/UliEngineering/Math/Geometry/Cylinder.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Math/Geometry/Polygon.py` & `UliEngineering-0.4.9/UliEngineering/Math/Geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Math/Geometry/Sphere.py` & `UliEngineering-0.4.9/UliEngineering/Math/Geometry/Sphere.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Mechanics/Threads.py` & `UliEngineering-0.4.9/UliEngineering/Mechanics/Threads.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Acceleration.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Acceleration.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Density.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Density.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Frequency.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Frequency.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/JohnsonNyquistNoise.py` & `UliEngineering-0.4.9/UliEngineering/Physics/JohnsonNyquistNoise.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Light.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Light.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/MagneticResonance.py` & `UliEngineering-0.4.9/UliEngineering/Physics/MagneticResonance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/NTC.py` & `UliEngineering-0.4.9/UliEngineering/Physics/NTC.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/NoiseDensity.py` & `UliEngineering-0.4.9/UliEngineering/Physics/NoiseDensity.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Pressure.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Pressure.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/RF.py` & `UliEngineering-0.4.9/UliEngineering/Physics/RF.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/RTD.py` & `UliEngineering-0.4.9/UliEngineering/Physics/RTD.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Rotation.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Rotation.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Physics/Temperature.py` & `UliEngineering-0.4.9/UliEngineering/Physics/Temperature.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Chunks.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Chunks.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/DateTime.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/DateTime.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/FFT.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/FFT.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Filter.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Filter.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Normalize.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Normalize.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Resampling.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Resampling.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Selection.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Selection.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Simulation.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Simulation.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Utils.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Utils.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Weight.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Weight.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/SignalProcessing/Window.py` & `UliEngineering-0.4.9/UliEngineering/SignalProcessing/Window.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Units.py` & `UliEngineering-0.4.9/UliEngineering/Units.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Compression.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Compression.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Concurrency.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Concurrency.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Date.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Date.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Files.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Files.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Iterable.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Iterable.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/JSON.py` & `UliEngineering-0.4.9/UliEngineering/Utils/JSON.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/NumPy.py` & `UliEngineering-0.4.9/UliEngineering/Utils/NumPy.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Parser.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Parser.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Range.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Range.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/String.py` & `UliEngineering-0.4.9/UliEngineering/Utils/String.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/Temporary.py` & `UliEngineering-0.4.9/UliEngineering/Utils/Temporary.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering/Utils/ZIP.py` & `UliEngineering-0.4.9/UliEngineering/Utils/ZIP.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/UliEngineering.egg-info/PKG-INFO` & `UliEngineering-0.4.9/UliEngineering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UliEngineering
-Version: 0.4.8
+Version: 0.4.9
 Summary: Computational tools for electronics engineering
 Home-page: https://techoverflow.net/
 Author: Uli Köhler
 Author-email: ukoehler@techoverflow.net
 License: Apache License v2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `UliEngineering-0.4.8/UliEngineering.egg-info/SOURCES.txt` & `UliEngineering-0.4.9/UliEngineering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.8/setup.py` & `UliEngineering-0.4.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 0):
     print('ERROR: UliEngineering currently requires at least Python 3.0 to run.')
     sys.exit(1)
 
 setup(name='UliEngineering',
-      version='0.4.8',
+      version='0.4.9',
       description='Computational tools for electronics engineering',
       author='Uli Köhler',
       author_email='ukoehler@techoverflow.net',
       url='https://techoverflow.net/',
       license='Apache License v2.0',
       packages=find_packages(exclude=['tests*']),
       include_package_data=True,
```

