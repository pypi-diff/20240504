# Comparing `tmp/pkscreener-0.44.20240504.327.tar.gz` & `tmp/pkscreener-0.44.20240504.328.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240504.327.tar", last modified: Sat May  4 03:40:45 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240504.328.tar", last modified: Sat May  4 04:04:09 2024, max compression
```

## Comparing `pkscreener-0.44.20240504.327.tar` & `pkscreener-0.44.20240504.328.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:45.378342 pkscreener-0.44.20240504.327/
--rw-rw-rw-   0        0        0     1086 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-04 03:40:45.378342 pkscreener-0.44.20240504.327/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:45.362717 pkscreener-0.44.20240504.327/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:45.378342 pkscreener-0.44.20240504.327/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7690 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20814 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82514 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-04 03:40:33.000000 pkscreener-0.44.20240504.327/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123857 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26414 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 03:40:45.362717 pkscreener-0.44.20240504.327/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-04 03:40:45.000000 pkscreener-0.44.20240504.327/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-04 03:40:45.000000 pkscreener-0.44.20240504.327/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 03:40:45.000000 pkscreener-0.44.20240504.327/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-04 03:40:45.000000 pkscreener-0.44.20240504.327/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 03:40:45.000000 pkscreener-0.44.20240504.327/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-04 03:40:45.000000 pkscreener-0.44.20240504.327/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-04 03:40:45.378342 pkscreener-0.44.20240504.327/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-04 03:35:24.000000 pkscreener-0.44.20240504.327/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/
+-rw-rw-rw-   0        0        0     1086 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.894486 pkscreener-0.44.20240504.328/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7690 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82514 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-04 04:04:00.000000 pkscreener-0.44.20240504.328/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124033 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26414 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.910085 pkscreener-0.44.20240504.328/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-04 03:58:48.000000 pkscreener-0.44.20240504.328/setup.py
```

### Comparing `pkscreener-0.44.20240504.327/LICENSE` & `pkscreener-0.44.20240504.328/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/LICENSE-Others` & `pkscreener-0.44.20240504.328/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/PKG-INFO` & `pkscreener-0.44.20240504.328/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.327
+Version: 0.44.20240504.328
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.327.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.328.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.327/README.md` & `pkscreener-0.44.20240504.328/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.327/pkscreener/__init__.py` & `pkscreener-0.44.20240504.328/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PKScanRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKGitFolderDownloader import downloadFolder
 from PKDevTools.classes.PKMultiProcessorClient import PKMultiProcessorClient
 from PKDevTools.classes.multiprocessing_logging import LogQueueReader
+from PKDevTools.classes.SuppressOutput import SuppressOutput
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.OutputControls import OutputControls
 # from PKDevTools.classes.PKJoinableQueue import PKJoinableQueue
 
@@ -281,15 +282,15 @@
                 )
 
         OutputControls().printOutput(colorText.END)
         if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options) and not userPassedArgs.options.upper().startswith("C"):
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
-            PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
+            PKScanRunner.terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
     def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
         tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
         sec_cache_file = cache_file if "intraday_" in cache_file else f"intraday_{cache_file}"
@@ -345,44 +346,46 @@
             sys.stdout.write(f"{round(time.time() - start_time)}.")
             worker.daemon = True
             worker.start()
         OutputControls().printOutput(f"Started all workers in {round(time.time() - start_time,4)}s")
         if OutputControls().enableMultipleLineOutput:
             sys.stdout.write("\x1b[1A")
 
-    def terminateAllWorkers(consumers, tasks_queue, testing=False):
-        # Exit all processes. Without this, it threw error in next screening session
-        for worker in consumers:
-            try:
-                if testing: # pragma: no cover
-                    if sys.platform.startswith("win"):
-                        import signal
-
-                        signal.signal(signal.SIGBREAK, PKScanRunner.shutdown)
-                        sleep(1)
-                    # worker.join()  # necessary so that the Process exists before the test suite exits (thus coverage is collected)
-                # else:
-                # try:
-                    # while worker.is_alive():
-                worker.terminate()
-                default_logger().debug("Worker terminated!")
-                # except:
-                #     continue
-            except OSError as e: # pragma: no cover
-                default_logger().debug(e, exc_info=True)
-                # if e.winerror == 5:
-                continue
-
-        # Flush the queue so depending processes will end
-        while True:
-            try:
-                _ = tasks_queue.get(False)
-            except Exception as e:  # pragma: no cover
-                # default_logger().debug(e, exc_info=True)
-                break
+    def terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing=False):
+        shouldSuppress = (userPassedArgs is None) or (userPassedArgs is not None and not userPassedArgs.log)
+        with SuppressOutput(suppress_stderr=shouldSuppress, suppress_stdout=shouldSuppress):
+            # Exit all processes. Without this, it threw error in next screening session
+            for worker in consumers:
+                try:
+                    if testing: # pragma: no cover
+                        if sys.platform.startswith("win"):
+                            import signal
+
+                            signal.signal(signal.SIGBREAK, PKScanRunner.shutdown)
+                            sleep(1)
+                        # worker.join()  # necessary so that the Process exists before the test suite exits (thus coverage is collected)
+                    # else:
+                    # try:
+                        # while worker.is_alive():
+                    worker.terminate()
+                    default_logger().debug("Worker terminated!")
+                    # except:
+                    #     continue
+                except OSError as e: # pragma: no cover
+                    default_logger().debug(e, exc_info=True)
+                    # if e.winerror == 5:
+                    continue
+
+            # Flush the queue so depending processes will end
+            while True:
+                try:
+                    _ = tasks_queue.get(False)
+                except Exception as e:  # pragma: no cover
+                    # default_logger().debug(e, exc_info=True)
+                    break
         PKScanRunner.tasks_queue = None
         PKScanRunner.results_queue = None
         PKScanRunner.scr = None
         PKScanRunner.consumers = None
 
     def shutdown(frame, signum):
         OutputControls().printOutput("Shutting down for test coverage")
```

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/classes/keys.py` & `pkscreener-0.44.20240504.328/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/courbd.ttf` & `pkscreener-0.44.20240504.328/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/globals.py` & `pkscreener-0.44.20240504.328/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,17 +640,17 @@
         options, False, False, defaultAnswer='Y'
     )
     listStockCodes = prepareStocksForScreening(testing=False, downloadOnly=False, listStockCodes=None,indexOption=indexOption)
     stockDictPrimary,stockDictSecondary = loadDatabaseOrFetch(downloadOnly=False, listStockCodes=listStockCodes, menuOption=menuOption,indexOption=indexOption)
     PKScanRunner.refreshDatabase(consumers,stockDictPrimary,stockDictSecondary)
 
 def closeWorkersAndExit():
-    global consumers, tasks_queue
+    global consumers, tasks_queue,userPassedArgs
     if consumers is not None:
-        PKScanRunner.terminateAllWorkers(consumers, tasks_queue)
+        PKScanRunner.terminateAllWorkers(userPassedArgs=userPassedArgs,consumers=consumers, tasks_queue=tasks_queue, testing=userPassedArgs.testbuild)
     
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
     global mp_manager, listStockCodes, screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDictPrimary, stockDictSecondary, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
     start_time = 0
@@ -2140,15 +2140,15 @@
     iterations,
     consumers,
     screenResults,
     saveResults,
     backtest_df,
     testing=False,
 ):
-    global selectedChoice, userPassedArgs, elapsed_time, start_time
+    global selectedChoice, userPassedArgs, elapsed_time, start_time,userPassedArgs
     result = None
     backtest_df = None
     reviewDate = getReviewDate(userPassedArgs)
     max_allowed = getMaxAllowedResultsCount(iterations, testing)
     try:
         originalNumberOfStocks = numStocks
         iterations, numStocksPerIteration = getIterationsAndStockCounts(numStocks, iterations)
@@ -2203,27 +2203,27 @@
             keyboardInterruptEventFired = True
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "\n[+] Terminating Script, Please wait..."
                 + colorText.END
             )
-            PKScanRunner.terminateAllWorkers(consumers=consumers, tasks_queue=tasks_queue,testing=testing)
+            PKScanRunner.terminateAllWorkers(userPassedArgs=userPassedArgs,consumers=consumers, tasks_queue=tasks_queue,testing=testing)
             logging.shutdown()
         except KeyboardInterrupt:
             pass
     except Exception as e:
         default_logger().debug(e, exc_info=True)
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
             + f"\nException:\n{e}\n[+] Terminating Script, Please wait..."
             + colorText.END
         )
-        PKScanRunner.terminateAllWorkers(consumers=consumers, tasks_queue=tasks_queue,testing=testing)
+        PKScanRunner.terminateAllWorkers(userPassedArgs=userPassedArgs,consumers=consumers, tasks_queue=tasks_queue,testing=testing)
         logging.shutdown()
 
     if result is not None and len(result) >=3 and "Date" not in saveResults.columns:
         temp_df = result[2].copy()
         temp_df.reset_index(inplace=True)
         temp_df = temp_df.tail(1)
         temp_df.rename(columns={"index": "Date"}, inplace=True)
```

### Comparing `pkscreener-0.44.20240504.327/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240504.328/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240504.328/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240504.328/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240504.328/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.327
+Version: 0.44.20240504.328
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.327.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.328.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240503.326/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.327/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240504.328/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.327/setup.py` & `pkscreener-0.44.20240504.328/setup.py`

 * *Files identical despite different names*

