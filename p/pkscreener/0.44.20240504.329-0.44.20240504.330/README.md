# Comparing `tmp/pkscreener-0.44.20240504.329.tar.gz` & `tmp/pkscreener-0.44.20240504.330.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240504.329.tar", last modified: Sat May  4 04:56:08 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240504.330.tar", last modified: Sat May  4 06:45:46 2024, max compression
```

## Comparing `pkscreener-0.44.20240504.329.tar` & `pkscreener-0.44.20240504.330.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/
--rw-rw-rw-   0        0        0     1086 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.620517 pkscreener-0.44.20240504.329/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25810 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7690 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29461 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17459 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82649 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-04 04:55:58.000000 pkscreener-0.44.20240504.329/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124033 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26414 2024-05-04 04:51:36.000000 pkscreener-0.44.20240504.329/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:56:08.620517 pkscreener-0.44.20240504.329/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-04 04:56:08.000000 pkscreener-0.44.20240504.329/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-04 04:56:08.636144 pkscreener-0.44.20240504.329/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-05-04 04:51:37.000000 pkscreener-0.44.20240504.329/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:45:46.405489 pkscreener-0.44.20240504.330/
+-rw-rw-rw-   0        0        0     1086 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-04 06:45:46.405489 pkscreener-0.44.20240504.330/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 06:45:46.389872 pkscreener-0.44.20240504.330/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:45:46.405489 pkscreener-0.44.20240504.330/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7690 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29461 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119213 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    80741 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-04 06:45:36.000000 pkscreener-0.44.20240504.330/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   124033 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    26410 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-04 06:45:46.389872 pkscreener-0.44.20240504.330/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-04 06:45:46.000000 pkscreener-0.44.20240504.330/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-04 06:45:46.000000 pkscreener-0.44.20240504.330/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 06:45:46.000000 pkscreener-0.44.20240504.330/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-04 06:45:46.000000 pkscreener-0.44.20240504.330/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 06:45:46.000000 pkscreener-0.44.20240504.330/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-04 06:45:46.000000 pkscreener-0.44.20240504.330/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-04 06:45:46.405489 pkscreener-0.44.20240504.330/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-04 06:40:42.000000 pkscreener-0.44.20240504.330/setup.py
```

### Comparing `pkscreener-0.44.20240504.329/LICENSE` & `pkscreener-0.44.20240504.330/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/LICENSE-Others` & `pkscreener-0.44.20240504.330/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/PKG-INFO` & `pkscreener-0.44.20240504.330/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.329
+Version: 0.44.20240504.330
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.329.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.330.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.329/README.md` & `pkscreener-0.44.20240504.330/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.329/pkscreener/__init__.py` & `pkscreener-0.44.20240504.330/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Pktalib.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,40 @@
 
 from pkscreener import Imports
 
 if Imports["talib"]:
     try:
         import talib
     except:
-        print("[+] TA-Lib is not installed. For best results, please install 'TA-Lib' ! Installation failed!")
+        print(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] 'TA-Lib' library is not installed. For best results, please install 'TA-Lib'! You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
+                + colorText.END
+            )
+        try:
+            import pandas_ta as talib
+            print(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] TA-Lib is not installed. Falling back on pandas_ta.\n[+] For full coverage(candle patterns), you may wish to follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
+                + colorText.END
+            )
+        except:
+            print(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] pandas_ta is not installed. Falling back on pandas_ta also failed.\n[+] For full coverage(candle patterns), you may wish to follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
+                + colorText.END
+            )
+            pass
         pass
 else:
     try:
         import pandas_ta as talib
-
         print(
             colorText.BOLD
             + colorText.FAIL
             + "[+] TA-Lib is not installed. Falling back on pandas_ta.\n[+] For full coverage(candle patterns), you may wish to follow instructions from\n[+] https://github.com/ta-lib/ta-lib-python"
             + colorText.END
         )
         sleep(3)
```

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/Utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import copy
 import datetime
 import glob
 import math
 import os
 import sys
 import textwrap
+import random
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 os.environ["AUTOGRAPH_VERBOSITY"] = "0"
 
 import pickle
 import platform
 import tempfile
@@ -47,14 +48,20 @@
 from pkscreener import Imports
 
 if Imports["keras"]:
     try:
         import keras
     except:
         print("The installation will fail. Please install 'keras' library on your machine!")
+        print(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] 'Keras' library is not installed. You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
+                + colorText.END
+            )
         pass
 
 import warnings
 from time import sleep
 
 warnings.simplefilter("ignore", DeprecationWarning)
 warnings.simplefilter("ignore", FutureWarning)
@@ -75,38 +82,23 @@
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
 from pkscreener.classes.PKTask import PKTask
 from pkscreener.classes.MarketStatus import MarketStatus
 from pkscreener.classes.PKScheduler import PKScheduler
 from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.Utils import random_user_agent
 
+from pkscreener.classes.ArtTexts import getArtText
+
 configManager = ConfigManager.tools()
 configManager.getConfig(ConfigManager.parser)
 nseFetcher = nseStockDataFetcher()
 fetcher = Fetcher.screenerStockDataFetcher()
 
-artText = """
-PPPPPPPPPPPPPPPPP   KKKKKKKKK    KKKKKKK   SSSSSSSSSSSSSSS                                                                                                                                         TM
-UPI:8007162973@APL  K:::::::K    K:::::K SS:::::::::::::::S
-P::::::PPPPPP:::::P K:::::::K    K:::::KS:::::SSSSSS::::::S
-PP:::::P     P:::::PK:::::::K   K::::::KS:::::S     SSSSSSS
-  P::::P     P:::::P K::::::K  K:::::K  S:::::S                ccccccccccccccccrrrrr   rrrrrrrrr       eeeeeeeeeeee        eeeeeeeeeeee    nnnn  nnnnnnnn        eeeeeeeeeeee    rrrrr   rrrrrrrrr
-  P::::P     P:::::P  K:::::K K:::::K   S:::::S              cc::::MADE:::::::cr::::rrr::WITH::::r    ee::::LOVE::::ee    ee:::::IN:::::ee  n:::nn:INDIA:nn    ee::::::::::::ee  r::::rrr:::::::::r
-  P::::PPPPPP:::::P   K::::::K:::::K     S::::SSSS          c:::::::::::::::::cr:::::::::::::::::r  e::::::eeeee:::::ee e::::::eeeee:::::een::::::::::::::nn  e::::::eeeee:::::eer::::©PKJMESRA::::r
-  P:::::::::::::PP    K:::::::::::K       SS::::::SSSSS    c:::::::cccccc:::::crr::::::rrrrr::::::re::::::e     e:::::ee::::::e     e:::::enn:::::::::::::::ne::::::e     e:::::err::::::rrrrr::::::r
-  P::::PPPPPPPPP      K:::::::::::K         SSS::::::::SS  c::::::c     ccccccc r:::::r     r:::::re:::::::eeeee::::::ee:::::::eeeee::::::e  n:::::nnnn:::::ne:::::::eeeee::::::e r:::::r     r:::::r
-  P::::P              K::::::K:::::K           SSSSSS::::S c:::::c              r:::::r     rrrrrrre:::::::::::::::::e e:::::::::::::::::e   n::::n    n::::ne:::::::::::::::::e  r:::::r     rrrrrrr
-  P::::P              K:::::K K:::::K               S:::::Sc:::::c              r:::::r            e::::::eeeeeeeeeee  e::::::eeeeeeeeeee    n::::n    n::::ne::::::eeeeeeeeeee   r:::::r
-  P::::P              K:::::K  K:::::K              S:::::Sc::::::c     ccccccc r:::::r            e:::::::e           e:::::::e             n::::n    n::::ne:::::::e            r:::::r
-PP::::::PP            K:::::K   K::::::KSSSSSSS     S:::::Sc:::::::cccccc:::::c r:::::r            e::::::::e          e::::::::e            n::::n    n::::ne::::::::e           r:::::r
-P::::::::P            K:::::K    K:::::KS::::::SSSSSS:::::S c:::::::::::::::::c r:::::r             e::::::::eeeeeeee   e::::::::eeeeeeee    n::::n    n::::n e::::::::eeeeeeee   r:::::r
-P::::::::P            K:::::K    K:::::KS:::::::::::::::S    cc:::::::::::::::c r:::::r              ee:::::::::::::e    ee:::::::::::::e    n::::n    n::::n  ee:::::::::::::e   r:::::r
-PPPPPPPPPP            KKKKKKK    KKKKKKK SSSSSSSSSSSSSSS       cccccccccccccccc rrrrrrr                eeeeeeeeeeeeee      eeeeeeeeeeeeee    nnnnnn    nnnnnn    eeeeeeeeeeeeee   rrrrrrr
-"""
-artText = f"{artText}\nv{VERSION}"
+
+artText = f"{getArtText()}\nv{VERSION}"
 
 STD_ENCODING=sys.stdout.encoding if sys.stdout is not None else 'utf-8'
 
 def marketStatus():
     # task = PKTask("Nifty 50 Market Status",MarketStatus().getMarketStatus)
     lngStatus = MarketStatus().marketStatus
     # scheduleTasks(tasksList=[task])
@@ -693,17 +685,18 @@
         for ii in word_list[:-1]:
             legendText_new = legendText_new + ii + "\n"
         legendText_new += word_list[-1]
         legendText = legendText_new
         return legendText
 
     def getDefaultColors():
+        artColors = ["violet", "indigo", "blue", "lightgreen", "yellow", "orange", "red"]
         bgColor = "white" if PKDateUtilities.currentDateTime().day % 2 == 0 else "black"
         gridColor = "black" if bgColor == "white" else "white"
-        artColor = "lightgreen" if bgColor == "black" else "blue"
+        artColor = random.choice(artColors[3:]) if bgColor == "black" else random.choice(artColors[:3])
         menuColor = "red"
         return bgColor,gridColor,artColor,menuColor
 
     def setupReportFont():
         fontURL = "https://raw.githubusercontent.com/pkjmesra/pkscreener/main/pkscreener/courbd.ttf"
         fontFile = fontURL.split("/")[-1]
         bData, fontPath, _ = Archiver.findFile(fontFile)
@@ -1515,14 +1508,21 @@
                 model = keras.models.load_model(files[0]) if Imports["keras"] else None
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             os.remove(files[0])
             os.remove(files[1])
             if not retrial:
                 tools.getNiftyModel(retrial=True)
+        if model is None:
+            print(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] 'Keras' library is not installed. Prediction failed! You may wish to follow instructions from\n[+] https://github.com/pkjmesra/PKScreener/"
+                + colorText.END
+            )
         return model, pkl
 
     def getSigmoidConfidence(x):
         out_min, out_max = 0, 100
         if x > 0.5:
             in_min = 0.50001
             in_max = 1
```

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/classes/keys.py` & `pkscreener-0.44.20240504.330/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/courbd.ttf` & `pkscreener-0.44.20240504.330/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/globals.py` & `pkscreener-0.44.20240504.330/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240504.330/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240504.330/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240504.329/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240504.330/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
                 OutputControls().printOutput(
                     "[+] RuntimeError with 'multiprocessing'.\n[+] Please contact the Developer, if this does not work!"
                 )
                 OutputControls().printOutput(e)
                 traceback.print_exc()
             pass
 
-        OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
+    OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
         
     configManager.getConfig(ConfigManager.parser)
     # configManager.restartRequestsCache()
     # args.monitor = configManager.defaultMonitorOptions
     if args.monitor is not None:
         MarketMonitor(monitors=args.monitor.split(",") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split(","),maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow)
```

### Comparing `pkscreener-0.44.20240504.329/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240504.330/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240504.329
+Version: 0.44.20240504.330
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.329.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240504.330.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.328/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240504.329/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240504.329/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240504.330/pkscreener.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pkscreener/pkscreenercli.py
 pkscreener.egg-info/PKG-INFO
 pkscreener.egg-info/SOURCES.txt
 pkscreener.egg-info/dependency_links.txt
 pkscreener.egg-info/entry_points.txt
 pkscreener.egg-info/not-zip-safe
 pkscreener.egg-info/top_level.txt
+pkscreener/classes/ArtTexts.py
 pkscreener/classes/Backtest.py
 pkscreener/classes/Barometer.py
 pkscreener/classes/CandlePatterns.py
 pkscreener/classes/Changelog.py
 pkscreener/classes/ConfigManager.py
 pkscreener/classes/Fetcher.py
 pkscreener/classes/MarketMonitor.py
```

### Comparing `pkscreener-0.44.20240504.329/setup.py` & `pkscreener-0.44.20240504.330/setup.py`

 * *Files identical despite different names*

