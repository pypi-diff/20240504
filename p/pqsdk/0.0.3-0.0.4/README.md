# Comparing `tmp/pqsdk-0.0.3.tar.gz` & `tmp/pqsdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqsdk-0.0.3.tar", last modified: Sat Apr 20 12:18:00 2024, max compression
+gzip compressed data, was "pqsdk-0.0.4.tar", last modified: Sat May  4 16:46:36 2024, max compression
```

## Comparing `pqsdk-0.0.3.tar` & `pqsdk-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.488684 pqsdk-0.0.3/
--rw-rw-rw-   0        0        0      766 2024-04-20 12:18:00.488137 pqsdk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.458501 pqsdk-0.0.3/pqsdk/
--rw-rw-rw-   0        0        0      169 2024-04-12 13:30:06.000000 pqsdk-0.0.3/pqsdk/__init__.py
--rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.3/pqsdk/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.469742 pqsdk-0.0.3/pqsdk/api/
--rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.3/pqsdk/api/__init__.py
--rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.3/pqsdk/api/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.475745 pqsdk-0.0.3/pqsdk/backtest/
--rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.3/pqsdk/backtest/__init__.py
--rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/backtest/analyzer.py
--rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/backtest/context.py
--rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/backtest/current_data.py
--rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/backtest/instrument.py
--rw-rw-rw-   0        0        0    14082 2024-04-20 12:07:11.000000 pqsdk-0.0.3/pqsdk/backtest/main.py
--rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.3/pqsdk/backtest/order.py
--rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/backtest/portfolio.py
--rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/backtest/position.py
--rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/backtest/run_info.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.476692 pqsdk-0.0.3/pqsdk/enums/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/enums/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.3/pqsdk/enums/orderStatus.py
--rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/faxconstant.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.482469 pqsdk-0.0.3/pqsdk/interface/
--rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/__init__.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/abstractInstrument.py
--rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.3/pqsdk/interface/abstractOrder.py
--rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/abstractPortfolio.py
--rw-rw-rw-   0        0        0     1677 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/abstractPosition.py
--rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/abstractRunInfo.py
--rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/abstractStrategyContext.py
--rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/interface/abstractTrader.py
--rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.3/pqsdk/interface/constant.py
--rw-rw-rw-   0        0        0     3520 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/logger.py
--rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.3/pqsdk/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.485849 pqsdk-0.0.3/pqsdk/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/utils/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/utils/dynamic_import.py
--rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/utils/file_util.py
--rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/utils/import_global_modules.py
--rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.3/pqsdk/utils/timer_factory.py
--rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.3/pqsdk/utils/value_type_util.py
--rw-rw-rw-   0        0        0      441 2024-04-20 12:17:53.000000 pqsdk-0.0.3/pqsdk/version.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.486815 pqsdk-0.0.3/pqsdk.egg-info/
--rw-rw-rw-   0        0        0      766 2024-04-20 12:18:00.000000 pqsdk-0.0.3/pqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2024-04-20 12:18:00.000000 pqsdk-0.0.3/pqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 12:18:00.000000 pqsdk-0.0.3/pqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-20 12:18:00.000000 pqsdk-0.0.3/pqsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      183 2024-04-20 12:18:00.000000 pqsdk-0.0.3/pqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-20 12:18:00.000000 pqsdk-0.0.3/pqsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 12:18:00.488684 pqsdk-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:18:00.486815 pqsdk-0.0.3/tests/
--rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.3/tests/test_backtest.py
--rw-rw-rw-   0        0        0     2059 2024-04-10 03:10:26.000000 pqsdk-0.0.3/tests/test_pqsdk_api.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.938639 pqsdk-0.0.4/
+-rw-rw-rw-   0        0        0      766 2024-05-04 16:46:36.937639 pqsdk-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.804405 pqsdk-0.0.4/pqsdk/
+-rw-rw-rw-   0        0        0      169 2024-04-12 13:30:06.000000 pqsdk-0.0.4/pqsdk/__init__.py
+-rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.4/pqsdk/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.825361 pqsdk-0.0.4/pqsdk/api/
+-rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.4/pqsdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.4/pqsdk/api/main.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.867334 pqsdk-0.0.4/pqsdk/backtest/
+-rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.4/pqsdk/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/backtest/analyzer.py
+-rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/backtest/context.py
+-rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/backtest/current_data.py
+-rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/backtest/instrument.py
+-rw-rw-rw-   0        0        0    14082 2024-04-20 12:07:11.000000 pqsdk-0.0.4/pqsdk/backtest/main.py
+-rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.4/pqsdk/backtest/order.py
+-rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/backtest/portfolio.py
+-rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/backtest/position.py
+-rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/backtest/run_info.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.871351 pqsdk-0.0.4/pqsdk/enums/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.4/pqsdk/enums/orderStatus.py
+-rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/faxconstant.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.910639 pqsdk-0.0.4/pqsdk/interface/
+-rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/interface/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/interface/abstractInstrument.py
+-rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.4/pqsdk/interface/abstractOrder.py
+-rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/interface/abstractPortfolio.py
+-rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.4/pqsdk/interface/abstractPosition.py
+-rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/interface/abstractRunInfo.py
+-rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/interface/abstractStrategyContext.py
+-rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/interface/abstractTrader.py
+-rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.4/pqsdk/interface/constant.py
+-rw-rw-rw-   0        0        0     4443 2024-05-04 16:44:11.000000 pqsdk-0.0.4/pqsdk/logger.py
+-rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.4/pqsdk/main.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.929639 pqsdk-0.0.4/pqsdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/utils/dynamic_import.py
+-rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/utils/file_util.py
+-rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/utils/import_global_modules.py
+-rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.4/pqsdk/utils/timer_factory.py
+-rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.4/pqsdk/utils/value_type_util.py
+-rw-rw-rw-   0        0        0      441 2024-05-04 16:44:57.000000 pqsdk-0.0.4/pqsdk/version.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.937639 pqsdk-0.0.4/pqsdk.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-04 16:46:36.000000 pqsdk-0.0.4/pqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2024-05-04 16:46:36.000000 pqsdk-0.0.4/pqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 16:46:36.000000 pqsdk-0.0.4/pqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-04 16:46:36.000000 pqsdk-0.0.4/pqsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2024-05-04 16:46:36.000000 pqsdk-0.0.4/pqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 16:46:36.000000 pqsdk-0.0.4/pqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 16:46:36.938639 pqsdk-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 16:46:36.936639 pqsdk-0.0.4/tests/
+-rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.4/tests/test_backtest.py
+-rw-rw-rw-   0        0        0     2059 2024-04-10 03:10:26.000000 pqsdk-0.0.4/tests/test_pqsdk_api.py
```

### Comparing `pqsdk-0.0.3/PKG-INFO` & `pqsdk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.3/pqsdk/__main__.py` & `pqsdk-0.0.4/pqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/api/__init__.py` & `pqsdk-0.0.4/pqsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/api/main.py` & `pqsdk-0.0.4/pqsdk/api/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/__init__.py` & `pqsdk-0.0.4/pqsdk/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/analyzer.py` & `pqsdk-0.0.4/pqsdk/backtest/analyzer.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/context.py` & `pqsdk-0.0.4/pqsdk/backtest/context.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/current_data.py` & `pqsdk-0.0.4/pqsdk/backtest/current_data.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/instrument.py` & `pqsdk-0.0.4/pqsdk/backtest/instrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/main.py` & `pqsdk-0.0.4/pqsdk/backtest/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/order.py` & `pqsdk-0.0.4/pqsdk/backtest/order.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/portfolio.py` & `pqsdk-0.0.4/pqsdk/backtest/portfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/position.py` & `pqsdk-0.0.4/pqsdk/backtest/position.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/backtest/run_info.py` & `pqsdk-0.0.4/pqsdk/backtest/run_info.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/enums/orderStatus.py` & `pqsdk-0.0.4/pqsdk/enums/orderStatus.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/faxconstant.py` & `pqsdk-0.0.4/pqsdk/faxconstant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/__init__.py` & `pqsdk-0.0.4/pqsdk/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractInstrument.py` & `pqsdk-0.0.4/pqsdk/interface/abstractInstrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractOrder.py` & `pqsdk-0.0.4/pqsdk/interface/abstractOrder.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractPortfolio.py` & `pqsdk-0.0.4/pqsdk/interface/abstractPortfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractPosition.py` & `pqsdk-0.0.4/pqsdk/interface/abstractPosition.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         """
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def init_date(self):
         """
-        减仓日期
+        建仓日期
         :return:
         """
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def transact_time(self):
```

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractRunInfo.py` & `pqsdk-0.0.4/pqsdk/interface/abstractRunInfo.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractStrategyContext.py` & `pqsdk-0.0.4/pqsdk/interface/abstractStrategyContext.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/abstractTrader.py` & `pqsdk-0.0.4/pqsdk/interface/abstractTrader.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/interface/constant.py` & `pqsdk-0.0.4/pqsdk/interface/constant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/main.py` & `pqsdk-0.0.4/pqsdk/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/utils/dynamic_import.py` & `pqsdk-0.0.4/pqsdk/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/utils/file_util.py` & `pqsdk-0.0.4/pqsdk/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/utils/timer_factory.py` & `pqsdk-0.0.4/pqsdk/utils/timer_factory.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk/utils/value_type_util.py` & `pqsdk-0.0.4/pqsdk/utils/value_type_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/pqsdk.egg-info/PKG-INFO` & `pqsdk-0.0.4/pqsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.3/pqsdk.egg-info/SOURCES.txt` & `pqsdk-0.0.4/pqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/setup.py` & `pqsdk-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.3/tests/test_pqsdk_api.py` & `pqsdk-0.0.4/tests/test_pqsdk_api.py`

 * *Files identical despite different names*

