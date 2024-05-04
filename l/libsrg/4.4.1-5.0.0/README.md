# Comparing `tmp/libsrg-4.4.1.tar.gz` & `tmp/libsrg-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg-4.4.1.tar", max compression
+gzip compressed data, was "libsrg-5.0.0.tar", max compression
```

## Comparing `libsrg-4.4.1.tar` & `libsrg-5.0.0.tar`

### file list

```diff
@@ -1,46 +1,77 @@
--rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-4.4.1/LICENSE.txt
--rw-r--r--   0        0        0     2776 2022-03-19 14:34:49.085595 libsrg-4.4.1/README.md
--rw-r--r--   0        0        0     1442 2024-05-03 01:24:32.649128 libsrg-4.4.1/libsrg/AppTemplate.py
--rw-r--r--   0        0        0    11308 2024-05-03 01:24:32.641128 libsrg-4.4.1/libsrg/Config.py
--rwxr-xr-x   0        0        0     2580 2024-05-03 01:24:32.631128 libsrg-4.4.1/libsrg/ElapsedTime.py
--rwxr-xr-x   0        0        0     7980 2024-05-03 01:24:32.617128 libsrg-4.4.1/libsrg/Info.py
--rwxr-xr-x   0        0        0     3532 2023-01-31 15:26:05.068010 libsrg-4.4.1/libsrg/LevelBanner.py
--rwxr-xr-x   0        0        0     1492 2023-01-18 20:30:11.250572 libsrg-4.4.1/libsrg/LoggerGUIProxy.py
--rwxr-xr-x   0        0        0     6113 2024-04-12 20:43:07.275560 libsrg-4.4.1/libsrg/LoggingAppBase.py
--rwxr-xr-x   0        0        0     7082 2024-04-17 20:14:51.858892 libsrg-4.4.1/libsrg/LoggingCounter.py
--rwxr-xr-x   0        0        0      413 2023-01-31 15:26:05.056010 libsrg-4.4.1/libsrg/LoggingUtils.py
--rwxr-xr-x   0        0        0     1376 2023-01-08 15:03:07.096718 libsrg-4.4.1/libsrg/LoggingWatcher.py
--rwxr-xr-x   0        0        0     2680 2023-01-31 15:30:47.587267 libsrg-4.4.1/libsrg/NagiosBase.py
--rwxr-xr-x   0        0        0     7125 2024-05-03 01:24:32.658128 libsrg-4.4.1/libsrg/Runner.py
--rwxr-xr-x   0        0        0     4100 2024-04-09 15:09:14.504097 libsrg-4.4.1/libsrg/Runner2.py
--rw-r--r--   0        0        0     4508 2024-04-21 12:42:50.283800 libsrg-4.4.1/libsrg/Statistics/ADStatsBase.py
--rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-4.4.1/libsrg/Statistics/AnalogStatsBase.py
--rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-4.4.1/libsrg/Statistics/AnalogStatsCumulative.py
--rw-r--r--   0        0        0     2300 2024-04-08 17:02:20.939118 libsrg-4.4.1/libsrg/Statistics/AnalogStatsFading.py
--rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-4.4.1/libsrg/Statistics/AnalogStatsSlidingWindow.py
--rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-4.4.1/libsrg/Statistics/DiscreteStatsBase.py
--rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-4.4.1/libsrg/Statistics/DiscreteStatsCumulative.py
--rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-4.4.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py
--rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-4.4.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py
--rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
--rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
--rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
--rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
--rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-4.4.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
--rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-4.4.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-4.4.1/libsrg/Statistics/UnitTests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-4.4.1/libsrg/Statistics/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-4.4.1/libsrg/TKGUI/GuiBase.py
--rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-4.4.1/libsrg/TKGUI/GuiRequest.py
--rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-4.4.1/libsrg/TKGUI/GuiRequestQueue.py
--rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-4.4.1/libsrg/TKGUI/LoggerGUI.py
--rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-4.4.1/libsrg/TKGUI/__init__.py
--rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-4.4.1/libsrg/UnitTests/Config_test.py
--rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-4.4.1/libsrg/UnitTests/RolloverTest_filename.py
--rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-4.4.1/libsrg/UnitTests/RolloverTest_logfile.py
--rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-4.4.1/libsrg/UnitTests/Sample.env
--rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-4.4.1/libsrg/UnitTests/Sample.ini
--rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-4.4.1/libsrg/UnitTests/Sample.json
--rwxr-xr-x   0        0        0        0 2023-01-31 16:52:02.998067 libsrg-4.4.1/libsrg/__init__.py
--rw-r--r--   0        0        0     1054 2024-05-03 01:29:35.764371 libsrg-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 libsrg-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.0.0/README.md
+-rw-r--r--   0        0        0     1464 2024-05-03 23:47:01.853721 libsrg-5.0.0/libsrg/AppTemplate.py
+-rw-r--r--   0        0        0    11392 2024-05-04 13:48:11.572363 libsrg-5.0.0/libsrg/Config.py
+-rwxr-xr-x   0        0        0     2603 2024-05-04 14:04:12.419228 libsrg-5.0.0/libsrg/ElapsedTime.py
+-rwxr-xr-x   0        0        0     8002 2024-05-03 23:47:01.863721 libsrg-5.0.0/libsrg/Info.py
+-rwxr-xr-x   0        0        0     4027 2024-05-03 23:47:01.866721 libsrg-5.0.0/libsrg/LevelBanner.py
+-rwxr-xr-x   0        0        0     1514 2024-05-03 23:47:01.870721 libsrg-5.0.0/libsrg/LoggerGUIProxy.py
+-rwxr-xr-x   0        0        0     6135 2024-05-03 23:47:01.873721 libsrg-5.0.0/libsrg/LoggingAppBase.py
+-rwxr-xr-x   0        0        0     8167 2024-05-03 23:47:01.876721 libsrg-5.0.0/libsrg/LoggingCounter.py
+-rwxr-xr-x   0        0        0      593 2024-05-03 23:47:01.880721 libsrg-5.0.0/libsrg/LoggingUtils.py
+-rwxr-xr-x   0        0        0     1854 2024-05-03 23:47:01.884721 libsrg-5.0.0/libsrg/LoggingWatcher.py
+-rwxr-xr-x   0        0        0     3644 2024-05-03 23:47:01.888721 libsrg-5.0.0/libsrg/NagiosBase.py
+-rwxr-xr-x   0        0        0     7209 2024-05-04 13:52:43.434938 libsrg-5.0.0/libsrg/Runner.py
+-rwxr-xr-x   0        0        0     4903 2024-05-03 23:47:01.898721 libsrg-5.0.0/libsrg/Runner2.py
+-rw-r--r--   0        0        0     4508 2024-04-21 12:42:50.283800 libsrg-5.0.0/libsrg/Statistics/ADStatsBase.py
+-rw-r--r--   0        0        0     2275 2024-04-11 13:40:23.574158 libsrg-5.0.0/libsrg/Statistics/AnalogStatsBase.py
+-rw-r--r--   0        0        0     1436 2024-04-08 17:02:20.928118 libsrg-5.0.0/libsrg/Statistics/AnalogStatsCumulative.py
+-rw-r--r--   0        0        0     2300 2024-04-08 17:02:20.939118 libsrg-5.0.0/libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--   0        0        0     1590 2024-04-12 18:46:46.468186 libsrg-5.0.0/libsrg/Statistics/AnalogStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1593 2024-04-11 13:40:23.559158 libsrg-5.0.0/libsrg/Statistics/DiscreteStatsBase.py
+-rw-r--r--   0        0        0      774 2024-04-08 17:02:20.912118 libsrg-5.0.0/libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--   0        0        0     1583 2024-04-11 13:02:36.159113 libsrg-5.0.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py
+-rw-r--r--   0        0        0     1839 2024-04-11 13:46:23.627270 libsrg-5.0.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py
+-rw-r--r--   0        0        0     2784 2024-04-17 20:08:12.373031 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+-rw-r--r--   0        0        0     2344 2024-04-11 13:56:04.322214 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+-rw-r--r--   0        0        0     3915 2024-04-11 13:59:27.002140 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--   0        0        0     2933 2024-04-12 18:46:46.483186 libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0     1605 2024-04-09 15:09:14.481097 libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--   0        0        0     2607 2024-04-11 00:45:26.519787 libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:48:22.511124 libsrg-5.0.0/libsrg/Statistics/UnitTests/__init__.py
+-rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
+-rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     4175 2024-04-24 16:16:17.492580 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.0.0/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-07 19:48:22.512123 libsrg-5.0.0/libsrg/Statistics/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-21 12:42:50.605797 libsrg-5.0.0/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
+-rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.0.0/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0     4439 2024-04-11 13:40:23.886156 libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.0.0/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-04-08 17:02:46.932966 libsrg-5.0.0/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2222 2024-04-09 15:09:14.520097 libsrg-5.0.0/libsrg/TKGUI/GuiBase.py
+-rw-r--r--   0        0        0      448 2024-04-09 15:09:14.568096 libsrg-5.0.0/libsrg/TKGUI/GuiRequest.py
+-rw-r--r--   0        0        0     3424 2024-04-09 15:09:14.527097 libsrg-5.0.0/libsrg/TKGUI/GuiRequestQueue.py
+-rw-r--r--   0        0        0    10694 2024-04-09 15:09:14.560097 libsrg-5.0.0/libsrg/TKGUI/LoggerGUI.py
+-rw-r--r--   0        0        0        1 2023-01-31 17:16:02.479077 libsrg-5.0.0/libsrg/TKGUI/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
+-rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
+-rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.0.0/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
+-rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.0.0/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
+-rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.0.0/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5498 2024-04-17 20:14:51.866892 libsrg-5.0.0/libsrg/UnitTests/Config_test.py
+-rw-r--r--   0        0        0     1259 2024-04-17 20:14:51.874892 libsrg-5.0.0/libsrg/UnitTests/RolloverTest_filename.py
+-rw-r--r--   0        0        0     1309 2024-04-17 20:14:51.850892 libsrg-5.0.0/libsrg/UnitTests/RolloverTest_logfile.py
+-rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.0.0/libsrg/UnitTests/Sample.env
+-rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.0.0/libsrg/UnitTests/Sample.ini
+-rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.0.0/libsrg/UnitTests/Sample.json
+-rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.0.0/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
+-rwxr-xr-x   0        0        0      114 2024-05-03 23:47:01.900721 libsrg-5.0.0/libsrg/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-04 14:33:28.588647 libsrg-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.0.0/PKG-INFO
```

### Comparing `libsrg-4.4.1/LICENSE.txt` & `libsrg-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/README.md` & `libsrg-5.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -70,12 +70,8 @@
 My intention is to keep this library small. It is not expected to evolve into an all-purpose framework. 
 Output is geared towards developers, not end users. 
 
 ## License
 MIT
 
 ## Project status
-Core functionality appears solid, but naming and packaging may be fluid for a while.
-
-This is my first attempt at publishing to pypi, so there may be surprises. 
-
-I will bump version to 1.x when out of beta.
+Pulled extraneous applications out into libsrg_apps
```

### Comparing `libsrg-4.4.1/libsrg/AppTemplate.py` & `libsrg-5.0.0/libsrg/AppTemplate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# 2024 Steven Goncalo
 import logging
 
 from libsrg.LoggingAppBase import LoggingAppBase
 
 """
 This module is a sample application template for libsrg application logging
 """
```

### Comparing `libsrg-4.4.1/libsrg/Config.py` & `libsrg-5.0.0/libsrg/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import re
 from collections import ChainMap
 from pathlib import Path
 from typing import Any, Self, Optional, Tuple, TypeAlias
 
 from jinja2 import Template
 
-"""FileName can be a str, bytes or a pathlib.Path."""
 FileName: TypeAlias = str | bytes | os.PathLike
-"""ConfigSource can be a ChainMap, a dict, or a FileName as defined above."""
+"""FileName can be a str, bytes or a pathlib.Path."""
+
 ConfigSource: TypeAlias = ChainMap[str, Any] | dict[str, Any] | FileName
+"""ConfigSource can be a ChainMap, a dict, or a FileName as defined above."""
 
 
 class Config(ChainMap):
     """
     The Config class extends the ChainMap class to provide access to config files.
 
     From outside, a Config looks like a series of python dictionaries which get searched in
@@ -27,121 +28,75 @@
 
     The Config class maintains one special Config instance which contains secrets. These can be usernames,
     passwords, api keys, or anything else that should not normally be kept in publicly accessible
     configuration files. One file of secrets can be read from a secure location and referenced by items
     in the normal config files.
 
     """
-    _secret_config: Self | None = None
 
-    @classmethod
-    def set_secrets(cls, *args: ConfigSource) -> None:
-        """
-        Sets the secret config held by this class.
-        :param args: zero or more Config, ChainMap, dict[str, Any], Path
-        :return: None
-        """
-        cls._secret_config = cls(*args)
+    _secret_config: Self | None = None
+    """Holds a secret config instance for usernames, passwords, api keys, etc."""
 
     def __init__(self, *args: ConfigSource):
         """
         Constructs a new Config object.
         :param args: zero or more Config, ChainMap, dict[str, Any], Path
         """
         args2 = self.process_args(*args)
         super().__init__(*args2)
 
-    @classmethod
-    def process_args(cls, *args: ConfigSource) -> list[dict[str, Any]]:
+    def apply_templates_to_strings(self, data: Any, config: Optional[Self] = None,
+                                   secrets: bool = False) -> Any:
         """
-        Processes a mixed list of Config like inputs to a list of dictionaries.
-        * Paths or str filenames are opened and loaded from disk.
-        * Config or ChainMap inputs are split into their internal maps (preserving order)
-        :param args: zero or more Config, ChainMap, dict[str, Any], Path
-        :return: an ordered list of dict objects
+        apply templates to strings in data (applies to str or list of str, else return unchanged
+          * if data is a str, apply templates
+          * if data is a list containing ONLY str, apply recursively for one level only
+          * anything else returns unmodified
+        :param data: data to be processed
+        :param config: defaults to self, if caller has already appended secrets, that can be passed here
+        :param secrets: append secrets before templates
+        :return: result
         """
-        pending: list[Any] = list(args)
-        out: list[dict[str, Any]] = []
-        while len(pending) > 0:
-            candidate = pending.pop(0)
-
-            # for ChainMap/Config inputs, add the individual maps
-            if isinstance(candidate, ChainMap):
-                maps = candidate.maps.copy()  # dont consume the source!
-                while len(maps) > 0:
-                    amap = maps.pop(-1)
-                    pending.insert(0, amap)
-                continue
-
-            # assume string argument is a pathname
-            if isinstance(candidate, str):
-                candidate = Path(candidate)
-
-            # open path arguments
-            if isinstance(candidate, Path):
-                with open(candidate, "r") as f:
-                    text = f.read()
-                # noinspection PyBroadException
-                candidate = cls.text_to_dict(text)
-
-            # only valid choice is dict here
-            if isinstance(candidate, dict):
-                out.append(candidate)
-            else:
-                raise TypeError(f"{type(candidate)} unexpected at {candidate}")
-        return out
+        if config is None:
+            config = self
+        if secrets:
+            config = ChainMap(config, self._secret_config)
+        if isinstance(data, str):
+            template = Template(data)
+            val = template.render(config)
+            return val
+        if isinstance(data, list):
+            # only apply to list of str, not list of Any
+            if all([isinstance(x, str) for x in data]):
+                return [self.apply_templates_to_strings(x, config=config, secrets=False) for x in data]
+        return data
 
     @classmethod
-    def text_to_dict(cls, text: str) -> dict[str, Any]:
-        """
-        Converts a string into a dict. Content type is determined using a few heuristics.
-        * convert from json if a line starting with "{" is found
-        * convert from yaml if a line starting with "---" is found  TODO #36
-        * convert from ini/configparser if a line starting with "[" is found
-          * note first level in dict will be sections, not items
-        * convert from env/bash name=value  otherwise
-        :param text:
-        :return: ict[str, Any]
+    def config_to_list(cls, config: Self) -> list[tuple[str, Any, int]]:
+        """Finds and alphabetizes all config items in config
+        :param config: Config instance
+        :return: Ordered list of tuples (name, value, depth)
         """
-        text = cls.strip_comments(text)
-        json_pat = re.compile(r"^\s*\{", re.MULTILINE)
-        if json_pat.match(text):
-            out = json.loads(text)
-            return out
-        ini_pat = re.compile(r"^\s*\[", re.MULTILINE)
-        if ini_pat.match(text):
-            cp = configparser.ConfigParser()
-            cp.read_string(text)
-            # reformat ini data as native dict of dicts
-            out = {name: {k: v for k, v in cp[name].items()} for name in cp.sections()}
-            return out
-        # fallback to flat env like file w/o [inisection]
-        cp = configparser.ConfigParser()
-        cp.read_string("[qqq]\n" + text)
-        out = {k: v for k, v in cp["qqq"].items()}
-        return out
-
-    @classmethod
-    def text_to_config(cls, text: str) -> Self:
-        """Create a Config instance from a string (see text_to_dict)."""
-        return cls(cls.text_to_dict(text))
+        names = list(config.keys())
+        names.sort()
+        lst = []
+        for name in names:
+            depth, val = config.find_item_depth(name)
+            lst.append((name, val, depth))
+        return lst
 
-    @classmethod
-    def strip_comments(cls, text: str, markers: Tuple[str] = None) -> str:
-        """
-        Strips line comments starting with markers
-        :param markers: tuple of line markers, defaults to ("#", ";", "//")
-        :param text: input text
-        :return: output text with line comments removed
+    def find_item_depth(self, item: str) -> Tuple[Optional[int], Any]:
+        """Looks for item in maps
+        :param item: item name
+        :return: (depth, value) if found tuple with depth and value, else (None,None)
         """
-        if markers is None:
-            markers = ("#", ";", "//")
-        lines = text.split("\n")
-        new_lines = [line for line in lines if not line.strip(" \t").startswith(markers)]
-        return "\n".join(new_lines)
+        for depth, dct in enumerate(self.maps):
+            if item in dct:
+                return depth, dct[item]
+        return None, None
 
     def get_item(self, *item_names: str, default=None, allow_none=False,
                  secrets: bool = False, jinja=True) -> Any:
         """
         get an argument from self.merged_args
         :param item_names: one or more alternate names, first found used
         :param default: if none of the names are found return this value
@@ -168,117 +123,165 @@
         if isinstance(val, Exception):
             raise val
         if jinja or secrets:
             # config already has secrets if enabled
             val = self.apply_templates_to_strings(val, config=config, secrets=False)
         return val
 
-    def apply_templates_to_strings(self, data: Any, config: Optional[Self] = None,
-                                   secrets: bool = False) -> Any:
+    @classmethod
+    def process_args(cls, *args: ConfigSource) -> list[dict[str, Any]]:
         """
-        apply templates to strings in data (applies to str or list of str, else return unchanged
-          * if data is a str, apply templates
-          * if data is a list containing ONLY str, apply recursively for one level only
-          * anything else returns unmodified
-        :param data: data to be processed
-        :param config: defaults to self, if caller has already appended secrets, that can be passed here
-        :param secrets: append secrets before templates
-        :return: result
+        Processes a mixed list of Config like inputs to a list of dictionaries.
+        * Paths or str filenames are opened and loaded from disk.
+        * Config or ChainMap inputs are split into their internal maps (preserving order)
+        :param args: zero or more Config, ChainMap, dict[str, Any], Path
+        :return: an ordered list of dict objects
         """
-        if config is None:
-            config = self
-        if secrets:
-            config = ChainMap(config, self._secret_config)
-        if isinstance(data, str):
-            template = Template(data)
-            val = template.render(config)
-            return val
-        if isinstance(data, list):
-            # only apply to list of str, not list of Any
-            if all([isinstance(x, str) for x in data]):
-                return [self.apply_templates_to_strings(x, config=config, secrets=False) for x in data]
-        return data
+        pending: list[Any] = list(args)
+        out: list[dict[str, Any]] = []
+        while len(pending) > 0:
+            candidate = pending.pop(0)
 
-    def set_item_if_missing(self, key: str, val: Any) -> None:
-        """
-        Convenience method for set_item which prevents overwriting existing item value
-        :param key: name of item
-        :param val: value of item
-        :return: None
-        """
-        self.set_item(key, val, overwrite=False)
+            # for ChainMap/Config inputs, add the individual maps
+            if isinstance(candidate, ChainMap):
+                maps = candidate.maps.copy()  # dont consume the source!
+                while len(maps) > 0:
+                    amap = maps.pop(-1)
+                    pending.insert(0, amap)
+                continue
+
+            # assume string argument is a pathname
+            if isinstance(candidate, str):
+                candidate = Path(candidate)
+
+            # open path arguments
+            if isinstance(candidate, Path):
+                with open(candidate, "r") as f:
+                    text = f.read()
+                # noinspection PyBroadException
+                candidate = cls.text_to_dict(text)
+
+            # only valid choice is dict here
+            if isinstance(candidate, dict):
+                out.append(candidate)
+            else:
+                raise TypeError(f"{type(candidate)} unexpected at {candidate}")
+        return out
 
     def set_item(self, key: str, value: Any, overwrite=True, ) -> None:
         """
         Set one item in config
         :param key: item name
         :param value: item value
         :param overwrite: Allow overwriting existing item (defaults True)
         :return: None
         """
         if key not in self or overwrite:
             self[key] = value
 
+    def set_item_if_missing(self, key: str, val: Any) -> None:
+        """
+        Convenience method for set_item which prevents overwriting existing item value
+        :param key: name of item
+        :param val: value of item
+        :return: None
+        """
+        self.set_item(key, val, overwrite=False)
+
     def set_items(self, overwrite: bool = True, **key_value_pairs) -> None:
         """Set one or more items in config using key/value pairs
         :param overwrite: Allow overwriting existing item (defaults True)
         :param key_value_pairs: key/value pairs to be set
         :return: None
         """
         for key, val in key_value_pairs.items():
             self.set_item(key, val, overwrite=overwrite)
 
-    def find_item_depth(self, item: str) -> Tuple[Optional[int], Any]:
-        """Looks for item in maps
-        :param item: item name
-        :return: (depth, value) if found tuple with depth and value, else (None,None)
+    @classmethod
+    def set_secrets(cls, *args: ConfigSource) -> None:
         """
-        for depth, dct in enumerate(self.maps):
-            if item in dct:
-                return depth, dct[item]
-        return None, None
+        Sets the secret config held by this class.
+        :param args: zero or more Config, ChainMap, dict[str, Any], Path
+        :return: None
+        """
+        cls._secret_config = cls(*args)
 
-    def to_list(self) -> list[tuple[str, Any, int]]:
-        """Finds and alphabetizes all config items in config
-        :return: Ordered list of tuples (name, value, depth)
+    @classmethod
+    def strip_comments(cls, text: str, markers: Tuple[str] = None) -> str:
         """
-        return self.config_to_list(self)
+        Strips line comments starting with markers
+        :param markers: tuple of line markers, defaults to ("#", ";", "//")
+        :param text: input text
+        :return: output text with line comments removed
+        """
+        if markers is None:
+            markers = ("#", ";", "//")
+        lines = text.split("\n")
+        new_lines = [line for line in lines if not line.strip(" \t").startswith(markers)]
+        return "\n".join(new_lines)
 
     @classmethod
-    def config_to_list(cls, config: Self) -> list[tuple[str, Any, int]]:
-        """Finds and alphabetizes all config items in config
-        :param config: Config instance
-        :return: Ordered list of tuples (name, value, depth)
+    def text_to_config(cls, text: str) -> Self:
+        """Create a Config instance from a string (see text_to_dict)."""
+        return cls(cls.text_to_dict(text))
+
+    @classmethod
+    def text_to_dict(cls, text: str) -> dict[str, Any]:
         """
-        names = list(config.keys())
-        names.sort()
-        lst = []
-        for name in names:
-            depth, val = config.find_item_depth(name)
-            lst.append((name, val, depth))
-        return lst
+        Converts a string into a dict. Content type is determined using a few heuristics.
+        * convert from json if a line starting with "{" is found
+        * convert from yaml if a line starting with "---" is found  TODO #36
+        * convert from ini/configparser if a line starting with "[" is found
+          * note first level in dict will be sections, not items
+        * convert from env/bash name=value  otherwise
+        :param text:
+        :return: ict[str, Any]
+        """
+        text = cls.strip_comments(text)
+        json_pat = re.compile(r"^\s*\{", re.MULTILINE)
+        if json_pat.match(text):
+            out = json.loads(text)
+            return out
+        ini_pat = re.compile(r"^\s*\[", re.MULTILINE)
+        if ini_pat.match(text):
+            cp = configparser.ConfigParser()
+            cp.read_string(text)
+            # reformat ini data as native dict of dicts
+            out = {name: {k: v for k, v in cp[name].items()} for name in cp.sections()}
+            return out
+        # fallback to flat env like file w/o [inisection]
+        cp = configparser.ConfigParser()
+        cp.read_string("[qqq]\n" + text)
+        out = {k: v for k, v in cp["qqq"].items()}
+        return out
 
-    def to_json_str(self, **kwargs) -> str:
+    def to_flat_dict(self, ) -> dict[str, Any]:
         """
-        Produces a flat dict from a Config and converts to JSON string.
-        :param kwargs: Keyword arguments pased to json.dump
-        :return: JSON string of Config
+        Produces a flat dict from a Config.
+        :return: dict contents of Config
         """
-        return json.dumps(self.to_flat_dict(), **kwargs)
+        return dict(self)
 
     def to_json_file(self, file: FileName, **kwargs):
         """
         Produces a flat dict from a Config and converts to JSON file.
         :param file: str or Path instance
         :param kwargs: keyword arguments pased to json.dump
         :return: None
         """
         txt = self.to_json_str(**kwargs)
         with open(file, 'w') as f:
             f.write(txt)
 
-    def to_flat_dict(self, ) -> dict[str, Any]:
+    def to_json_str(self, **kwargs) -> str:
         """
-        Produces a flat dict from a Config.
-        :return: dict contents of Config
+        Produces a flat dict from a Config and converts to JSON string.
+        :param kwargs: Keyword arguments pased to json.dump
+        :return: JSON string of Config
         """
-        return dict(self)
+        return json.dumps(self.to_flat_dict(), **kwargs)
+
+    def to_list(self) -> list[tuple[str, Any, int]]:
+        """Finds and alphabetizes all config items in config
+        :return: Ordered list of tuples (name, value, depth)
+        """
+        return self.config_to_list(self)
```

### Comparing `libsrg-4.4.1/libsrg/ElapsedTime.py` & `libsrg-5.0.0/libsrg/ElapsedTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# 2024 Steven Goncalo
 """
 ElapsedTime is a class to measure elapsed time between start and stop events.
 It can be operated directly using start and stop methods, or it can
 act as a context manager in a "with" statement block.
 """
 import logging
 from datetime import timedelta
@@ -9,14 +10,15 @@
 
 
 class ElapsedTime:
 
     def __init__(self, name=None):
         """
         Constructs ElapsedTime object, started
+
         :param name: Name of ElapsedTime
         """
         self.logger = logging.getLogger(self.__class__.__name__)
         if name:
             self.name = name
         else:
             self.name = repr(self)
```

### Comparing `libsrg-4.4.1/libsrg/Info.py` & `libsrg-5.0.0/libsrg/Info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #! /usr/bin/env python3
+# 2024 Steven Goncalo
 import configparser
 import logging
 import os
 import platform
 import sys
 from importlib.metadata import version
```

### Comparing `libsrg-4.4.1/libsrg/LevelBanner.py` & `libsrg-5.0.0/libsrg/LevelBanner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env  python3
+# 2024 Steven Goncalo
 
 import logging
 
 from libsrg.LoggingUtils import level2int
 from libsrg.Runner import Runner
 
 banner_DEBUG = """
@@ -71,35 +72,48 @@
     'WARNING': banner_WARNING,
     'ERROR': banner_ERROR,
     'CRITICAL': banner_CRITICAL,
 }
 
 
 class LevelBanner:
+    """
+    The LevelBanner class maintains a set of large print banners listing the python logging levels.
+    """
     levs = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
     levmap = {'CRITICAL': 50, 'FATAL': 50, 'ERROR': 40, 'WARN': 30, 'WARNING': 30, 'INFO': 20, 'DEBUG': 10, 'NOTSET': 0}
 
     # logging.getLevelNamesMapping()  # levmap[int]->str
     # {'CRITICAL': 50, 'FATAL': 50, 'ERROR': 40, 'WARN': 30, 'WARNING': 30, 'INFO': 20, 'DEBUG': 10, 'NOTSET': 0}
 
     @classmethod
     def find(cls, name: str, threshold=None) -> str:
+        """
+        Find a LevelBanner instance by name.
+        :param name: Uppercase ascii name of logging level
+        :param threshold: return empty string for levels below threshold
+        :return: block character string
+        """
         iname = level2int(name)
         if not threshold:
             threshold = logging.WARNING
         if iname < threshold:
             return ""  # f"All logging below {threshold=}"
         if name in banners:
             return banners[name]
         else:
             return f"Unknown level {name}"
 
     @classmethod
-    def generate(cls):
-        # this method used the system banner utility to generate the text arrays pasted above
+    def generate(cls) ->None:
+        """
+        This method runs the system banner utility to generate the text arrays pasted above.
+
+        It is not needed at run time, just preserves how the banners were generated.
+        """
         for lev in cls.levs:
             print(f'banner_{lev}="""')
             r = Runner(["banner", lev])
             print("\n".join(r.so_lines))
             print('"""')
             print()
         print("banners:dict[str,str]={")
```

### Comparing `libsrg-4.4.1/libsrg/LoggerGUIProxy.py` & `libsrg-5.0.0/libsrg/LoggerGUIProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# 2024 Steven Goncalo
 import logging
 
 GUI_NEW_LINE = "GUI_NEW_LINE"
 GUI_FREEZE_LINE = "GUI_FREEZE_LINE"
 GUI_CONFIGURE = "GUI_CONFIGURE"
```

### Comparing `libsrg-4.4.1/libsrg/LoggingAppBase.py` & `libsrg-5.0.0/libsrg/LoggingAppBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env  python3
+# 2024 Steven Goncalo
 
 import argparse
 import logging
 from importlib.metadata import version
 from typing import Optional
 
 from libsrg.LoggingCounter import LoggingCounter
```

### Comparing `libsrg-4.4.1/libsrg/LoggingCounter.py` & `libsrg-5.0.0/libsrg/LoggingCounter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env  python3
+# 2024 Steven Goncalo
 
 import atexit
 import logging
 import sys
 import time
 from collections import Counter
 from importlib.metadata import version
@@ -26,37 +27,57 @@
     """
 
     __instance: "LoggingCounter" = None
 
     __rotating_file_handler: RotatingFileHandler = None
 
     def __init__(self, *args, **kwargs):
+        """
+        Constructor registers the logging counter instance.
+
+        It will throw an exception if another instance is already created.
+
+        :param args: passed to logging.Handler
+        :param kwargs: passed to logging.Handler
+        """
         super(LoggingCounter, self).__init__(*args, **kwargs)
         if self.__instance is not None:
             log.critical("Constructor called on existing singleton")
             raise Exception("LoggingCounter is designed as a singleton")
         self.__class__.__instance = self
         # index is name of level, not numeric value
         self.count_at_level_name = Counter()
         self.frozen = False
         self.runtime = ElapsedTime("Runtime")
 
     def emit(self, record):
+        """
+        When handler is told to emit a record, it counts the number of logs performed at each level.
+        :param record:
+        """
         if not self.frozen:
             lev = record.levelname
             # if lev not in self.count_at_level_name:
             #     self.count_at_level_name[lev] = 0
             self.count_at_level_name[lev] += 1
 
     def count_for_level(self, lev) -> int:
-        """lev can be passed as string or numeric level, but index is based on string """
+        """
+        Returns count of logs performed at given level
+        :param lev: level name or numeric level
+        """
         lev_str: str = level2str(lev)
         return self.count_at_level_name[lev_str]
 
     def __log_atexit(self, logger: logging.Logger = None, log_level=logging.INFO):
+        """
+        At Exit routine to print logging and runtime summary
+        :param logger: logger to use for printing
+        :param log_level: level at which to print summary
+        """
         if logger is None:
             logger = log
         self.frozen = True
         self.runtime.stop()
         ver = version('libsrg')
         olist: List[str] = [f"\n\n{sys.argv[0]} Using libsrg {ver} from {libsrg_version()}", "Logging Summary:"]
         lasttag = None
@@ -106,31 +127,51 @@
             log.critical("Looks like a LoggingCounter was already created? Good luck with that...")
         else:
             # log.info("Logging system configured")
             atexit.register(cls.log_counters)
         return handler
 
     @classmethod
-    def rotate_files(cls):
+    def rotate_files(cls)->None:
+        """
+        Rotates all log files
+        :return:
+        """
         if cls.__rotating_file_handler is not None:
             cls.__rotating_file_handler.doRollover()
 
     @classmethod
     def get_instance(cls):
+        """
+        Returns the LoggingCounter instance
+        :return:
+        """
         if cls.__instance is None:
             cls.__instance = LoggingCounter()
         return cls.__instance
 
     @classmethod
     def log_counters(cls, logger: logging.Logger = None, log_level=logging.INFO):
+        """
+        Logs the number of logs performed at each level (same as __log_atexit)
+        :param logger:
+        :param log_level:
+        :return:
+        """
         cls.get_instance().__log_atexit(logger, log_level)
-        # atexit.unregister(cls.log_counters)
 
     @classmethod
     def add_logfile(cls, filename, tgt_logger=None, **kwargs):
+        """
+        Adds a new logfile
+        :param filename:
+        :param tgt_logger:
+        :param kwargs:
+        :return:
+        """
         if tgt_logger is None:
             tgt_logger = logging.getLogger()
 
         kwargs.setdefault("maxBytes", 10 * 1024 * 1024)
         kwargs.setdefault("backupCount", 5)
         h = RotatingFileHandler(filename, **kwargs)
         fmt = logging.getLogger().handlers[0].formatter
```

### Comparing `libsrg-4.4.1/libsrg/NagiosBase.py` & `libsrg-5.0.0/libsrg/NagiosBase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 #!/usr/bin/env  python3
+# 2024 Steven Goncalo
 
 # from optparse import OptionParser
 import sys
 from enum import Enum
 
 from libsrg.LoggingAppBase import LoggingAppBase
 
 
 class NagiosReturn(Enum):
+    """
+    Enum class to represent Nagios return codes.
+    """
     NOCALL = -1
     OK = 0
     WARNING = 1
     CRITICAL = 2
     UNKNOWN = 3
 
 
 # noinspection PyPep8Naming
 class NagiosBase(LoggingAppBase):
-
+    """
+    Base class for Nagios applications.
+    """
     def __init__(self):
-
+        """
+        Constructor. Initializes logging and sets up default command line arguments.
+        """
         super().__init__()
 
         self.curReturn = NagiosReturn.NOCALL
         self.curReturnStr = "nocall?"
         self.defReturn = NagiosReturn.UNKNOWN
         self.defReturnStr = "no status reported?"
         try:
@@ -32,14 +40,21 @@
         except Exception as e:
             self.logger.critical(f"Unexpected error: {e}")
         finally:
             self.report()
 
     # noinspection PyPep8Naming
     def createParser(self):
+        """
+        Creates command line parser.
+        * host address
+        * username
+        * verbose flag
+        :return:
+        """
 
         self.parser.add_argument("-H", "--hostaddress",
                                  action="store", dest="host", default="nas0.home.goncalo.name",
                                  help="FQDN or IP of host to check via ssh")
         self.parser.add_argument("-U", "--user",
                                  action="store", dest="user", default="root",
                                  help="username at hostaddress")
@@ -48,35 +63,59 @@
         # self.parser.add_argument('--log-file', nargs=1, help='file to log to (default = stdout)', dest='logfile',
         #                          type=str, default=None)
 
         self.extendParser()
         self.perform_parse()
 
     def nocallResult(self, retCode, retStr):
+        """
+        Sets return code directly to Nagios return code.
+        :param retCode:
+        :param retStr:
+        :return:
+        """
         self.defReturn = retCode
         self.defReturnStr = retStr
 
     def setResult(self, retCode, retStr):
+        """
+        Sets return code to worse of given and previous codes
+        :param retCode:
+        :param retStr:
+        :return:
+        """
         if retCode.value > self.curReturn.value:
             self.curReturn = retCode
             self.curReturnStr = retStr
 
     def report(self):
+        """
+        Prints worst case return code and message at end of test
+        :return:
+        """
         if self.curReturn == NagiosReturn.NOCALL:
             self.logger.error("using nocall result")
             self.curReturn = self.defReturn
             self.curReturnStr = self.defReturnStr
         self.logger.info(f"{self.curReturn.name}={self.curReturn.value} {self.curReturnStr}")
         print(self.curReturn.name, " - ", self.curReturnStr)
         sys.exit(self.curReturn.value)
 
     # these need to be overriden in the subclass
     def extendParser(self):
+        """
+        Extends command line parser.
+        :return:
+        """
         self.logger.error("createSubclassParser should be overridden in Subclass")
 
     def runTest(self):
+        """
+        This is where the actual test is executed.
+        :return:
+        """
         self.logger.error("runTest should be overridden in Subclass")
 
 
 if __name__ == '__main__':
     print("This module cannot be run standalone")
     sys.exit(-1)
```

### Comparing `libsrg-4.4.1/libsrg/Runner.py` & `libsrg-5.0.0/libsrg/Runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,50 @@
+# 2024 Steven Goncalo
+"""
+Module before includes
+"""
 import logging
 import os
 import subprocess
 from pathlib import Path
 from typing import List, Optional, Union, Dict
 
 from libsrg.ElapsedTime import ElapsedTime
 
-
+"""
+Module after includes
+"""
 class Runner:
-    """
-    Runner is a utility class to run a command as a subprocess and return results
-    * command is passed as a list of program followed by zero or more arguments
-      * if provided as a single string, it calls split to make it a list
-    * Runner objects are single use
-      * command executed by constructor
-      * results returned as fields of object
-    * stdout and stderr are captured and returned as lists of utf-8 strings
-      * one list element per line
-      * end of line chars removed
-      * empty list if no output captured
-    * return code as integer
-    * any exception raised is caught
-      * returned in caught field
-      * logged as an error
-      * optionally rethrown if rethrow is set True
-    * success field is true if no exceptions caught and return code is zero
-    * exception raised if throw is True and success is false
-    """
-
     def __init__(self, cmd: Union[List[str], str], timeout=None, rethrow=False, verbose=False, throw=False,
                  cwd: Optional[Union[str, Path]] = None,
                  userat: Optional[str] = None,
                  env: Optional[Dict[str, str]] = None,
                  inherit_env: bool = False,
                  logger: Optional[logging.Logger] = None,
                  retries: int = 0,
                  silent: bool = False,
                  ):
         """
-        Run the given command and return results
+        Runner is a utility class to run a command as a subprocess and return results
+        * command is passed as a list of program followed by zero or more arguments
+          * if provided as a single string, it calls split to make it a list
+        * Runner objects are single use
+          * command executed by constructor
+          * results returned as fields of object
+        * stdout and stderr are captured and returned as lists of utf-8 strings
+          * one list element per line
+          * end of line chars removed
+          * empty list if no output captured
+        * return code as integer
+        * any exception raised is caught
+          * returned in caught field
+          * logged as an error
+          * optionally rethrown if rethrow is set True
+        * success field is true if no exceptions caught and return code is zero
+        * exception raised if throw is True and success is false
 
         :param cmd: A list of strings, or a single string which Runner will str.split()
         :param timeout: If positive, number of seconds before a timeout exception is raised
         :param rethrow: If true, rethrow any exceptions caught, else success set False
         :param verbose: If true, log the command before execution
         :param cwd: If set, run in this location on local node
         :param userat: Prepend ssh to cammand with this user@remote.node string
```

### Comparing `libsrg-4.4.1/libsrg/Runner2.py` & `libsrg-5.0.0/libsrg/Runner2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+# 2024 Steven Goncalo
 import logging
 import subprocess
 from typing import List, Optional, Union
 
 from libsrg.LoggingAppBase import LoggingAppBase
 
 """
-Runner2 is a utility class to run a command as a subprocess and return results
+Runner2 is a utility class to run a pair of commands as a subprocess and return results.
+
+The output of cmd1 is piped into the input of cmd2. Primary usage is intended for zfs send/receive commands, 
+where either or both ends of the pipeline may be on remote nodes.
+
 * command is passed as a list of program followed by zero or more arguments
 * Runner2 objects are single use
   * command executed by constructor
   * results returned as fields of object
 * stdout and stderr are captured and returned as lists of utf-8 strings
   * one list element per line
   * end of line chars removed
@@ -24,14 +29,23 @@
 
 
 class Runner2:
 
     def __init__(self, cmd1: Union[List[str], str], cmd2: Union[List[str], str], timeout=None, rethrow=False,
                  userat1=None,
                  userat2=None):
+        """
+        Forms a pipeline where cmd1 runs in one subprocess feeding into cmd2 in another subprocess
+        :param cmd1: first command
+        :param cmd2: second command
+        :param timeout: overall timeout in seconds
+        :param rethrow: rethrow any caught exception
+        :param userat1: run cmd1 as ssh at this user1@host1
+        :param userat2: run cmd2 as ssh at this user2@host2
+        """
         self.logger = logging.getLogger(self.__class__.__name__)
         # cmd2 is a list of program name and zero or mor eorguments
         # timeout (if specified) is a timeout to communicate in seconds
         if isinstance(cmd1, str):
             self.cmd1 = cmd1.split()
         else:
             self.cmd1 = cmd1
@@ -52,17 +66,21 @@
         self.so_lines: List[str] = []
         self.se_lines: List[str] = []
         self.caught: Optional[Exception] = None
         self.p1 = None
         self.p2 = None
         self.rethrow = rethrow
         self.timeout = timeout
-        self.execute()
+        self._execute()
 
-    def execute(self):
+    def _execute(self):
+        """
+        inner routine to execute piped commands
+        :return:
+        """
         try:
             self.logger.info(f'{" ".join(self.cmd1)} | {" ".join(self.cmd2)}')
             self.p2 = subprocess.Popen(self.cmd2, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE)
             # self.p2 = subprocess.Popen(self.cmd2,stdin=subprocess.PIPE)
             self.p1 = subprocess.Popen(self.cmd1, stdout=self.p2.stdin)
 
             (self.so_bytes, self.se_bytes) = self.p2.communicate()  # @UnusedVariable
@@ -77,14 +95,18 @@
             self.logger.error(ex)
             self.success = False
             self.caught = ex
             if self.rethrow:
                 raise ex
 
     def __str__(self):
+        """
+        Single line summary of the object.
+        :return:
+        """
         # noinspection PyPep8
         return (
                 f'Runner2 success={self.success} ret1={self.ret1}' +
                 f' ret2={self.ret2} cmd1={self.cmd1}  cmd2={self.cmd2}  so_lines={self.so_lines}'
         )
```

### Comparing `libsrg-4.4.1/libsrg/Statistics/ADStatsBase.py` & `libsrg-5.0.0/libsrg/Statistics/ADStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/AnalogStatsBase.py` & `libsrg-5.0.0/libsrg/Statistics/AnalogStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/AnalogStatsCumulative.py` & `libsrg-5.0.0/libsrg/Statistics/AnalogStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/AnalogStatsFading.py` & `libsrg-5.0.0/libsrg/Statistics/AnalogStatsFading.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/AnalogStatsSlidingWindow.py` & `libsrg-5.0.0/libsrg/Statistics/AnalogStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/DiscreteStatsBase.py` & `libsrg-5.0.0/libsrg/Statistics/DiscreteStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/DiscreteStatsCumulative.py` & `libsrg-5.0.0/libsrg/Statistics/DiscreteStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py` & `libsrg-5.0.0/libsrg/Statistics/DiscreteStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/ADStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py` & `libsrg-5.0.0/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/TKGUI/GuiBase.py` & `libsrg-5.0.0/libsrg/TKGUI/GuiBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/TKGUI/GuiRequestQueue.py` & `libsrg-5.0.0/libsrg/TKGUI/GuiRequestQueue.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/TKGUI/LoggerGUI.py` & `libsrg-5.0.0/libsrg/TKGUI/LoggerGUI.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/UnitTests/Config_test.py` & `libsrg-5.0.0/libsrg/UnitTests/Config_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/UnitTests/RolloverTest_filename.py` & `libsrg-5.0.0/libsrg/UnitTests/RolloverTest_filename.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/libsrg/UnitTests/RolloverTest_logfile.py` & `libsrg-5.0.0/libsrg/UnitTests/RolloverTest_logfile.py`

 * *Files identical despite different names*

### Comparing `libsrg-4.4.1/pyproject.toml` & `libsrg-5.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg"
-version = "4.4.1"
+version = "5.0.0"
 description = "Utility lib logging, statistics, subprocesses"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -25,10 +25,12 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
 Homepage = "https://gitlab.com/SRG_gitlab/libsrg"
 Issues = "https://gitlab.com/SRG_gitlab/libsrg/-/issues"
+API = "https://srg_gitlab.gitlab.io/libsrg/index.html"
+Wiki = "https://gitlab.com/SRG_gitlab/libsrg/-/wikis/home"
 
 [tool.poetry.extras]
 doc = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon"]
```

### Comparing `libsrg-4.4.1/PKG-INFO` & `libsrg-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 4.4.1
+Version: 5.0.0
 Summary: Utility lib logging, statistics, subprocesses
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -95,12 +95,8 @@
 My intention is to keep this library small. It is not expected to evolve into an all-purpose framework. 
 Output is geared towards developers, not end users. 
 
 ## License
 MIT
 
 ## Project status
-Core functionality appears solid, but naming and packaging may be fluid for a while.
-
-This is my first attempt at publishing to pypi, so there may be surprises. 
-
-I will bump version to 1.x when out of beta.
+Pulled extraneous applications out into libsrg_apps
```

