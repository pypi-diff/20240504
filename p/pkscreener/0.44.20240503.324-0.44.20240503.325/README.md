# Comparing `tmp/pkscreener-0.44.20240503.324.tar.gz` & `tmp/pkscreener-0.44.20240503.325.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240503.324.tar", last modified: Fri May  3 10:34:00 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240503.325.tar", last modified: Fri May  3 10:53:23 2024, max compression
```

## Comparing `pkscreener-0.44.20240503.324.tar` & `pkscreener-0.44.20240503.325.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/
--rw-rw-rw-   0        0        0     1086 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.852244 pkscreener-0.44.20240503.324/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7690 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20814 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8126 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82304 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-03 10:33:51.000000 pkscreener-0.44.20240503.324/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123825 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26382 2024-05-03 10:29:29.000000 pkscreener-0.44.20240503.324/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:34:00.852244 pkscreener-0.44.20240503.324/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 10:34:00.000000 pkscreener-0.44.20240503.324/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-03 10:34:00.867843 pkscreener-0.44.20240503.324/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-03 10:29:30.000000 pkscreener-0.44.20240503.324/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:53:23.622660 pkscreener-0.44.20240503.325/
+-rw-rw-rw-   0        0        0     1086 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-03 10:53:23.622660 pkscreener-0.44.20240503.325/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 10:53:23.607034 pkscreener-0.44.20240503.325/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:53:23.622660 pkscreener-0.44.20240503.325/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7690 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20814 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82514 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-03 10:53:10.000000 pkscreener-0.44.20240503.325/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-03 10:48:30.000000 pkscreener-0.44.20240503.325/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-03 10:48:31.000000 pkscreener-0.44.20240503.325/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123857 2024-05-03 10:48:31.000000 pkscreener-0.44.20240503.325/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-03 10:48:31.000000 pkscreener-0.44.20240503.325/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-03 10:48:31.000000 pkscreener-0.44.20240503.325/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26414 2024-05-03 10:48:31.000000 pkscreener-0.44.20240503.325/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:53:23.607034 pkscreener-0.44.20240503.325/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-03 10:53:23.000000 pkscreener-0.44.20240503.325/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-03 10:53:23.000000 pkscreener-0.44.20240503.325/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 10:53:23.000000 pkscreener-0.44.20240503.325/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-03 10:53:23.000000 pkscreener-0.44.20240503.325/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 10:53:23.000000 pkscreener-0.44.20240503.325/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 10:53:23.000000 pkscreener-0.44.20240503.325/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-03 10:53:23.622660 pkscreener-0.44.20240503.325/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-03 10:48:31.000000 pkscreener-0.44.20240503.325/setup.py
```

### Comparing `pkscreener-0.44.20240503.324/LICENSE` & `pkscreener-0.44.20240503.325/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/LICENSE-Others` & `pkscreener-0.44.20240503.325/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/PKG-INFO` & `pkscreener-0.44.20240503.325/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240503.324
+Version: 0.44.20240503.325
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.324.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.325.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `pkscreener-0.44.20240503.324/README.md` & `pkscreener-0.44.20240503.325/README.md`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/__init__.py` & `pkscreener-0.44.20240503.325/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PKScheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 from concurrent.futures import ProcessPoolExecutor
 from rich.progress import Progress, BarColumn, TimeRemainingColumn, TimeElapsedColumn
 from rich.console import Console
 from rich.control import Control
 from rich.segment import ControlType
 from pkscreener.classes.PKTask import PKTask
 
-multiprocessing.freeze_support()
+if __name__ == '__main__':
+    multiprocessing.freeze_support()
 
 # def long_running_fn(*args, **kwargs):
 #     len_of_task = random.randint(3, 20000)  # take some random length of time
 #     task = args[0]
 #     progress = task.progressStatusDict
 #     task_id = task.taskId
 #     for n in range(0, len_of_task):
```

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 import pandas as pd
 from alive_progress import alive_bar
 from PIL import Image, ImageDraw, ImageFont
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.Committer import Committer
+from PKDevTools.classes.SuppressOutput import SuppressOutput
 from tabulate import tabulate
 
 import pkscreener.classes.ConfigManager as ConfigManager
 import pkscreener.classes.Fetcher as Fetcher
 from pkscreener.classes import VERSION, Changelog
 from pkscreener.classes.MenuOptions import menus
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
@@ -822,18 +823,20 @@
             task.userData = stocks
             if len(stocks) > 0:
                 tasksList.append(task)
             queueCounter += 1
         
         processedStocks = []
         if len(tasksList) > 0:
-            PKScheduler.scheduleTasks(tasksList=tasksList, 
-                                      label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",
-                                      timeout=(5+2.5*configManager.longTimeout*(4 if downloadOnly else 1)), # 5 sec additional time for multiprocessing setup
-                                      minAcceptableCompletionPercentage=(100 if downloadOnly else 100))
+            # Suppress any multiprocessing errors/warnings
+            with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
+                PKScheduler.scheduleTasks(tasksList=tasksList, 
+                                        label=f"Downloading latest data [{configManager.period},{configManager.duration}] (Total={len(stockCodes)} records in {len(tasksList)} batches){'Be Patient!' if len(stockCodes)> 2000 else ''}",
+                                        timeout=(5+2.5*configManager.longTimeout*(4 if downloadOnly else 1)), # 5 sec additional time for multiprocessing setup
+                                        minAcceptableCompletionPercentage=(100 if downloadOnly else 100))
             for task in tasksList:
                 if task.result is not None:
                     for stock in task.userData:
                         taskResult = task.result.get(f"{stock}{exchangeSuffix}")
                         if taskResult is not None:
                             stockDict[stock] = taskResult.to_dict("split")
                             processedStocks.append(stock)
```

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/classes/keys.py` & `pkscreener-0.44.20240503.325/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/courbd.ttf` & `pkscreener-0.44.20240503.325/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/globals.py` & `pkscreener-0.44.20240503.325/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 from pkscreener.classes.OtaUpdater import OTAUpdater
 from pkscreener.classes.Portfolio import PortfolioCollection
 from pkscreener.classes.PKTask import PKTask
 from pkscreener.classes.PKScheduler import PKScheduler
 from pkscreener.classes.PKScanRunner import PKScanRunner
 from pkscreener.classes.PKMarketOpenCloseAnalyser import PKMarketOpenCloseAnalyser
 
-multiprocessing.freeze_support()
+if __name__ == '__main__':
+    multiprocessing.freeze_support()
 # import dataframe_image as dfi
 # import df2img
 # Try Fixing bug with this symbol
 TEST_STKCODE = "SBIN"
 # Constants
 np.seterr(divide="ignore", invalid="ignore")
```

### Comparing `pkscreener-0.44.20240503.324/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240503.325/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240503.325/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240503.325/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from pkscreener import Imports
 from PKDevTools.classes.OutputControls import OutputControls
 from pkscreener.classes.MarketMonitor import MarketMonitor
 import pkscreener.classes.ConfigManager as ConfigManager
 
-multiprocessing.freeze_support()
+if __name__ == '__main__':
+    multiprocessing.freeze_support()
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 os.environ["AUTOGRAPH_VERBOSITY"] = "0"
 
 printenabled=False
 originalStdOut=None
 original__stdout=None
 cron_runs=0
```

### Comparing `pkscreener-0.44.20240503.324/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240503.325/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240503.324
+Version: 0.44.20240503.325
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.324.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240503.325.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `pkscreener-0.44.20240503.324/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240503.325/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240503.324/setup.py` & `pkscreener-0.44.20240503.325/setup.py`

 * *Files identical despite different names*

