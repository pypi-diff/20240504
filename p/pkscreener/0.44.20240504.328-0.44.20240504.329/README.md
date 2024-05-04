# Comparing `tmp/pkscreener-0.44.20240504.328.tar.gz` & `tmp/pkscreener-0.44.20240504.329.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240504.328.tar", last modified: Sat May  4 04:04:09 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240504.329.tar", last modified: Sat May  4 04:56:08 2024, max compression
```

## Comparing `pkscreener-0.44.20240504.328.tar` & `pkscreener-0.44.20240504.329.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/
--rw-rw-rw-   0        0        0     1086 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.894486 pkscreener-0.44.20240504.328/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7690 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82514 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-04 04:04:00.000000 pkscreener-0.44.20240504.328/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124033 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26414 2024-05-04 03:58:47.000000 pkscreener-0.44.20240504.328/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:04:09.910085 pkscreener-0.44.20240504.328/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-04 04:04:09.000000 pkscreener-0.44.20240504.328/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-04 04:04:09.925712 pkscreener-0.44.20240504.328/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-04 03:58:48.000000 pkscreener-0.44.20240504.328/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/
+-rw-rw-rw-   0        0        0     1086 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.620517 pkscreener-0.44.20240504.329/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7690 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17459 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82649 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-04 04:55:58.000000 pkscreener-0.44.20240504.329/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124033 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26414 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.620517 pkscreener-0.44.20240504.329/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-04 04:51:37.000000 pkscreener-0.44.20240504.329/setup.py
```

### Comparing `pkscreener-0.44.20240504.328/LICENSE` & `pkscreener-0.44.20240504.329/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/LICENSE-Others` & `pkscreener-0.44.20240504.329/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/PKG-INFO` & `pkscreener-0.44.20240504.329/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.328
+Version: 0.44.20240504.329
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.328.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.329.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.328/README.md` & `pkscreener-0.44.20240504.329/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.328/pkscreener/__init__.py` & `pkscreener-0.44.20240504.329/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Pktalib.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
 from PKDevTools.classes.ColorText import colorText
 
 from pkscreener import Imports
 
 if Imports["talib"]:
-    import talib
+    try:
+        import talib
+    except:
+        print("[+] TA-Lib is not installed. For best results, please install 'TA-Lib' ! Installation failed!")
+        pass
 else:
     try:
         import pandas_ta as talib
 
         print(
             colorText.BOLD
             + colorText.FAIL
```

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 import pytz
 from genericpath import isfile
 from PKDevTools.classes.log import default_logger
 
 from pkscreener import Imports
 
 if Imports["keras"]:
-    import keras
+    try:
+        import keras
+    except:
+        print("The installation will fail. Please install 'keras' library on your machine!")
+        pass
 
 import warnings
 from time import sleep
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
 import pandas as pd
```

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/classes/keys.py` & `pkscreener-0.44.20240504.329/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/courbd.ttf` & `pkscreener-0.44.20240504.329/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/globals.py` & `pkscreener-0.44.20240504.329/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240504.329/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240504.329/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240504.329/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240504.329/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.328
+Version: 0.44.20240504.329
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.328.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.329.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.327/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.328/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240504.329/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.328/setup.py` & `pkscreener-0.44.20240504.329/setup.py`

 * *Files identical despite different names*

