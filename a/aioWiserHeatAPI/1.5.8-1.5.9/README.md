# Comparing `tmp/aioWiserHeatAPI-1.5.8.tar.gz` & `tmp/aioWiserHeatAPI-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioWiserHeatAPI-1.5.8.tar", last modified: Fri Mar  1 12:45:39 2024, max compression
+gzip compressed data, was "aioWiserHeatAPI-1.5.9.tar", last modified: Fri Mar  1 14:46:33 2024, max compression
```

## Comparing `aioWiserHeatAPI-1.5.8.tar` & `aioWiserHeatAPI-1.5.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:45:39.055677 aioWiserHeatAPI-1.5.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-01 12:45:39.055677 aioWiserHeatAPI-1.5.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     5800 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:45:39.051677 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/heating.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/heating_actuator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:45:39.055677 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/extra_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/opentherm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/special_times.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/zigbee.py
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/hot_water.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/pte.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/rest_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    27455 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/roomstat.py
--rw-r--r--   0 runner    (1001) docker     (127)    42257 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/smartplug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/smartvalve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/smokealarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16816 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/ufh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/wiserhub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:45:39.055677 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-01 12:45:39.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-01 12:45:39.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 12:45:39.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-01 12:45:39.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-01 12:45:39.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-01 12:45:39.000000 aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-01 12:45:39.055677 aioWiserHeatAPI-1.5.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1540 2024-03-01 12:45:33.000000 aioWiserHeatAPI-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:46:33.627797 aioWiserHeatAPI-1.5.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1068 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-01 14:46:33.627797 aioWiserHeatAPI-1.5.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5856 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:46:33.623796 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/heating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/heating_actuator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:46:33.627797 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/extra_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/opentherm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/special_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/zigbee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/hot_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/pte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/rest_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27455 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/roomstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42257 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/smartplug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/smartvalve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/smokealarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16816 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/ufh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/wiserhub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 14:46:33.627797 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-01 14:46:33.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-01 14:46:33.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 14:46:33.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-01 14:46:33.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-01 14:46:33.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-01 14:46:33.000000 aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-01 14:46:33.627797 aioWiserHeatAPI-1.5.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1540 2024-03-01 14:46:28.000000 aioWiserHeatAPI-1.5.9/setup.py
```

### Comparing `aioWiserHeatAPI-1.5.8/LICENSE` & `aioWiserHeatAPI-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/PKG-INFO` & `aioWiserHeatAPI-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.5.8
+Version: 1.5.9
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
@@ -68,14 +68,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.5.9
+
+* Force schedules endpoint to use http/1.0
+
 ### v1.5.8
 
 * Handle chunked encoding if sent by the hub
 
 ### v1.5.7
 
 * Fixed issue whereby lower target temp for passive mode was not being set correctly
```

### Comparing `aioWiserHeatAPI-1.5.8/README.md` & `aioWiserHeatAPI-1.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.5.9
+
+* Force schedules endpoint to use http/1.0
+
 ### v1.5.8
 
 * Handle chunked encoding if sent by the hub
 
 ### v1.5.7
 
 * Fixed issue whereby lower target temp for passive mode was not being set correctly
```

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/cli.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/cli.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/const.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/const.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/devices.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/devices.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/discovery.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/discovery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/heating.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/heating.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/heating_actuator.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/heating_actuator.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/automations.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/automations.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/battery.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/battery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/capabilities.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/capabilities.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/cloud.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/device.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/device.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/equipment.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/equipment.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/extra_config.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/extra_config.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/firmware.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/firmware.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/network.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/network.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/opentherm.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/opentherm.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/signal.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/signal.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/special_times.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/special_times.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/status.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/status.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/temp.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/temp.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/helpers/zigbee.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/helpers/zigbee.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/hot_water.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/hot_water.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/light.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/light.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/moments.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/moments.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/pte.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/pte.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/rest_controller.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/rest_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     ):
         """
         Send patch update to hub and raise errors if fails
         param url: url of hub rest api endpoint
         param patchData: json object containing command and values to set
         return: boolean
         """
-        if url in [WISERHUBDOMAIN, WISERHUBSCHEDULES]:
+        if url in [WISERHUBDOMAIN]:
             http_version = aiohttp.HttpVersion11
         else:
             http_version = aiohttp.HttpVersion10
 
         url = url.format(
             self._wiser_connection_info.host,
             self._wiser_connection_info.port,
```

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/room.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/room.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/roomstat.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/roomstat.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/schedule.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/shutter.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/shutter.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/smartplug.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/smartplug.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/smartvalve.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/smartvalve.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/smokealarm.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/smokealarm.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/system.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/system.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/ufh.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/ufh.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI/wiserhub.py` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI/wiserhub.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/PKG-INFO` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.5.8
+Version: 1.5.9
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
@@ -68,14 +68,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.5.9
+
+* Force schedules endpoint to use http/1.0
+
 ### v1.5.8
 
 * Handle chunked encoding if sent by the hub
 
 ### v1.5.7
 
 * Fixed issue whereby lower target temp for passive mode was not being set correctly
```

### Comparing `aioWiserHeatAPI-1.5.8/aioWiserHeatAPI.egg-info/SOURCES.txt` & `aioWiserHeatAPI-1.5.9/aioWiserHeatAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.5.8/setup.py` & `aioWiserHeatAPI-1.5.9/setup.py`

 * *Files identical despite different names*

