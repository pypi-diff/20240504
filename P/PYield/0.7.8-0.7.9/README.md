# Comparing `tmp/pyield-0.7.8.tar.gz` & `tmp/pyield-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.8.tar", last modified: Sat Apr 27 14:04:14 2024, max compression
+gzip compressed data, was "pyield-0.7.9.tar", last modified: Sun Apr 28 10:53:08 2024, max compression
```

## Comparing `pyield-0.7.8.tar` & `pyield-0.7.9.tar`

### file list

```diff
@@ -1,31 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.8/LICENSE
--rw-r--r--   0        0        0     6508 2024-04-26 00:32:17.834190 pyield-0.7.8/README.md
--rw-r--r--   0        0        0       22 2024-04-27 11:56:16.299935 pyield-0.7.8/pyield/__about__.py
--rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.8/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.8/pyield/bday.py
--rw-r--r--   0        0        0     6268 2024-04-27 13:08:29.971193 pyield-0.7.8/pyield/data_access.py
--rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.8/pyield/data_analysis.py
--rw-r--r--   0        0        0        0 2024-04-25 23:39:41.039220 pyield-0.7.8/pyield/futures/__init__.py
--rw-r--r--   0        0        0      169 2024-04-27 12:39:19.772667 pyield-0.7.8/pyield/futures/historical/__init__.py
--rw-r--r--   0        0        0     9277 2024-04-27 12:35:06.344046 pyield-0.7.8/pyield/futures/historical/common.py
--rw-r--r--   0        0        0     2121 2024-04-27 12:38:36.571050 pyield-0.7.8/pyield/futures/historical/dap.py
--rw-r--r--   0        0        0     2717 2024-04-26 08:19:58.862579 pyield-0.7.8/pyield/futures/historical/ddi.py
--rw-r--r--   0        0        0     3095 2024-04-27 13:03:13.689638 pyield-0.7.8/pyield/futures/historical/di.py
--rw-r--r--   0        0        0    11501 2024-04-27 13:47:29.988597 pyield-0.7.8/pyield/futures/historical/di_xml.py
--rw-r--r--   0        0        0     2175 2024-04-26 08:20:47.784608 pyield-0.7.8/pyield/futures/historical/frc.py
--rw-r--r--   0        0        0       71 2024-04-26 17:05:33.986164 pyield-0.7.8/pyield/futures/intraday/__init__.py
--rw-r--r--   0        0        0     3595 2024-04-26 09:06:08.639852 pyield-0.7.8/pyield/futures/intraday/trading_data.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.8/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.8/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.8/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.8/pyield/holidays/core.py
--rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.8/pyield/indicators.py
--rw-r--r--   0        0        0     3500 2024-04-25 00:22:37.836841 pyield-0.7.8/pyield/projections.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.8/pyield/py.typed
--rw-r--r--   0        0        0     6622 2024-04-27 13:46:18.187573 pyield-0.7.8/pyield/treasuries.py
--rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.8/pyield/utils.py
--rw-r--r--   0        0        0     1203 2024-04-27 14:04:14.278968 pyield-0.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.8/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.8/tests/test_bday.py
--rw-r--r--   0        0        0     1225 2024-04-27 13:28:21.555207 pyield-0.7.8/tests/test_futures.py
--rw-r--r--   0        0        0     8571 1970-01-01 00:00:00.000000 pyield-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.9/LICENSE
+-rw-r--r--   0        0        0     6508 2024-04-26 00:32:17.834190 pyield-0.7.9/README.md
+-rw-r--r--   0        0        0       22 2024-04-28 10:38:58.291333 pyield-0.7.9/pyield/__about__.py
+-rw-r--r--   0        0        0      417 2024-04-28 10:11:00.205906 pyield-0.7.9/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.9/pyield/bday.py
+-rw-r--r--   0        0        0     7381 2024-04-28 10:51:14.510995 pyield-0.7.9/pyield/data_access.py
+-rw-r--r--   0        0        0      140 2024-04-28 10:31:40.116585 pyield-0.7.9/pyield/futures/__init__.py
+-rw-r--r--   0        0        0    12106 2024-04-28 10:44:29.678697 pyield-0.7.9/pyield/futures/historical.py
+-rw-r--r--   0        0        0     3598 2024-04-28 10:31:04.134126 pyield-0.7.9/pyield/futures/intraday.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.9/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.9/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.9/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.9/pyield/holidays/core.py
+-rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.9/pyield/indicators.py
+-rw-r--r--   0        0        0     3500 2024-04-25 00:22:37.836841 pyield-0.7.9/pyield/projections.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.9/pyield/py.typed
+-rw-r--r--   0        0        0     2378 2024-04-28 10:30:56.245025 pyield-0.7.9/pyield/spreads.py
+-rw-r--r--   0        0        0     4321 2024-04-28 10:03:46.441528 pyield-0.7.9/pyield/treasuries.py
+-rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.9/pyield/utils.py
+-rw-r--r--   0        0        0     1203 2024-04-28 10:53:08.081451 pyield-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.9/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.9/tests/test_bday.py
+-rw-r--r--   0        0        0     1225 2024-04-27 13:28:21.555207 pyield-0.7.9/tests/test_futures.py
+-rw-r--r--   0        0        0    11525 2024-04-28 10:36:11.897142 pyield-0.7.9/tests/xml.py
+-rw-r--r--   0        0        0     8571 1970-01-01 00:00:00.000000 pyield-0.7.9/PKG-INFO
```

### Comparing `pyield-0.7.8/LICENSE` & `pyield-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/README.md` & `pyield-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/bday.py` & `pyield-0.7.9/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/futures/historical/common.py` & `pyield-0.7.9/pyield/futures/historical.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import io
 
 import pandas as pd
 import requests
 
-from ... import bday
+from .. import bday
+
+COUNT_CONVENTIONS = {
+    "DAP": 252,
+    "DI1": 252,
+    "DDI": 360,
+    "FRC": None,
+    "DOL": None,
+    "WDO": None,
+    "IND": None,
+    "WIN": None,
+}
 
 
 def get_expiration_date(expiration_code: str) -> pd.Timestamp:
     """
     Converts an expiration code into its corresponding expiration date.
 
     This function translates an expiration code into a specific expiration date based on
@@ -137,20 +148,25 @@
     """
     Internal function to convert DI futures prices to rates.
 
     Args:
         prices (pd.Series): The futures prices to be converted.
         days_to_expiration (pd.Series): The number of days to expiration for each price.
         count_convention (int): The count convention for the DI futures contract.
-            Normally, it is 252 business days or 360 calendar days.
+            Can be 252 business days or 360 calendar days.
 
     Returns:
         pd.Series: A pd.Series containing the futures rates.
     """
-    rates = (100_000 / prices) ** (count_convention / days_to_expiration) - 1
+    if count_convention == 252:
+        rates = (100_000 / prices) ** (252 / days_to_expiration) - 1
+    elif count_convention == 360:
+        rates = (100_000 / prices - 1) * (360 / days_to_expiration)
+    else:
+        raise ValueError("Invalid count_convention. Must be 252 or 360.")
 
     # Round to 5 (3 in %) dec. places (contract's current max. precision)
     return rates.round(5)
 
 
 def fetch_raw_df(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
@@ -194,14 +210,24 @@
     # Force "AJUSTE CORRIG. (4)" to be float, since it can be also read as int
     if "AJUSTE CORRIG. (4)" in df.columns:
         df["AJUSTE CORRIG. (4)"] = df["AJUSTE CORRIG. (4)"].astype(pd.Float64Dtype())
 
     return df
 
 
+def _adjust_older_contracts_rates(df: pd.DataFrame, rate_cols: list) -> pd.DataFrame:
+    for col in rate_cols:
+        df[col] = convert_prices_to_rates(df[col], df["BDaysToExp"], 252)
+
+    # Invert low and high prices
+    df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
+
+    return df
+
+
 def rename_columns(df: pd.DataFrame) -> pd.DataFrame:
     all_columns = {
         "VENCTO": "ExpirationCode",
         "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
         "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
         "NÚM. NEGOC.": "TradeCount",
         "CONTR. NEGOC.": "TradeVolume",
@@ -220,40 +246,69 @@
         "ÚLT.OF. COMPRA": "CloseAskRate",
         "ÚLT.OF. VENDA": "CloseBidRate",
     }
     rename_dict = {c: all_columns[c] for c in all_columns if c in df.columns}
     return df.rename(columns=rename_dict)
 
 
-def process_raw_df(
-    df: pd.DataFrame, trade_date: pd.Timestamp, asset_code: str
+def process_df(
+    df: pd.DataFrame,
+    trade_date: pd.Timestamp,
+    asset_code: str,
 ) -> pd.DataFrame:
-    df = rename_columns(df)
-
     df["TradeDate"] = trade_date
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
 
     df["TickerSymbol"] = asset_code + df["ExpirationCode"]
 
     # Contract code format was changed in 22/05/2006
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
             get_old_expiration_date, args=(trade_date,)
         )
     else:
         df["ExpirationDate"] = df["ExpirationCode"].apply(get_expiration_date)
 
+    df["DaysToExp"] = (df["ExpirationDate"] - trade_date).dt.days
+    # Convert to nullable integer, since it is the default type in the library
+    df["DaysToExp"] = df["DaysToExp"].astype(pd.Int64Dtype())
+    # Remove expired contracts
+    df.query("DaysToExp > 0", inplace=True)
+
+    df["BDaysToExp"] = bday.count_bdays(trade_date, df["ExpirationDate"])
+
     # Columns where 0 means NaN
     cols_with_nan = [col for col in df.columns if "Rate" in col]
     if "SettlementPrice" in df.columns:
         cols_with_nan.append("SettlementPrice")
     # Replace 0 with NaN in these columns
     df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
 
+    rate_cols = [col for col in df.columns if "Rate" in col]
+    # Prior to 17/01/2002 (inclusive), DI prices were not converted to rates
+    if trade_date <= pd.Timestamp("2002-01-17") and asset_code == "DI1":
+        df = _adjust_older_contracts_rates(df, rate_cols)
+    else:
+        # Remove % and round to 5 (3 in %) dec. places in rate columns
+        df[rate_cols] = df[rate_cols].div(100).round(5)
+
+    if COUNT_CONVENTIONS[asset_code] == 252:
+        df["SettlementRate"] = convert_prices_to_rates(
+            prices=df["SettlementPrice"],
+            days_to_expiration=df["BDaysToExp"],
+            count_convention=252,
+        )
+    elif COUNT_CONVENTIONS[asset_code] == 360:
+        df["SettlementRate"] = convert_prices_to_rates(
+            prices=df["SettlementPrice"],
+            days_to_expiration=df["DaysToExp"],
+            count_convention=360,
+        )
+
     return df
 
 
 def reorder_columns(df: pd.DataFrame):
     all_columns = [
         "TradeDate",
         "TickerSymbol",
@@ -275,7 +330,35 @@
         "MaxRate",
         "CloseAskRate",
         "CloseBidRate",
         "CloseRate",
     ]
     reordered_columns = [col for col in all_columns if col in df.columns]
     return df[reordered_columns]
+
+
+def fetch_historical_df(
+    asset_code: str,
+    trade_date: pd.Timestamp,
+) -> pd.DataFrame:
+    """
+    Fetchs the futures data for a given date from B3.
+
+    This function fetches and processes the futures data from B3 for a specific
+    trade date. It's the primary external interface for accessing futures data.
+
+    Args:
+        asset_code (str): The asset code to fetch the futures data.
+        trade_date (pd.Timestamp): The trade date to fetch the futures data.
+        count_convention (int): The count convention for the DI futures contract.
+            Can be 252 business days or 360 calendar days.
+
+    Returns:
+        pd.DataFrame: A Pandas pd.DataFrame containing processed futures data.
+    """
+    df_raw = fetch_raw_df(asset_code=asset_code, trade_date=trade_date)
+    if df_raw.empty:
+        return df_raw
+    df = rename_columns(df_raw)
+    df = process_df(df, trade_date, asset_code)
+    df = reorder_columns(df)
+    return df
```

### Comparing `pyield-0.7.8/pyield/futures/historical/di_xml.py` & `pyield-0.7.9/tests/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 
 import pandas as pd
 import requests
 from lxml import etree
 from pandas import DataFrame, Timestamp
 
-from ... import bday
-from . import common as cm
+from ..pyield import bday
+from ..pyield.futures import historical as ht
 
 
 def _get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
     """
     Types of XML files available:
     Full Price Report (all assets)
         - aprox. 5 MB zipped file;
@@ -225,15 +225,15 @@
 
 
 def _process_di_df(df_raw: DataFrame) -> DataFrame:
     df = df_raw.copy()
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradDt"] = df["TradDt"].astype("datetime64[ns]")
 
-    expiration = df["TckrSymb"].str[3:].apply(cm.get_expiration_date)
+    expiration = df["TckrSymb"].str[3:].apply(ht.get_expiration_date)
     df.insert(2, "ExpirationDate", expiration)
 
     business_days = bday.count_bdays(df["TradDt"], df["ExpirationDate"])
     df.insert(3, "BDaysToExp", business_days)
 
     # Convert to nullable integer, since other columns use this data type
     df["BDaysToExp"] = df["BDaysToExp"].astype(pd.Int64Dtype())
```

### Comparing `pyield-0.7.8/pyield/futures/intraday/trading_data.py` & `pyield-0.7.9/pyield/futures/intraday.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     rate_cols = [col for col in df.columns if "Rate" in col]
     df[rate_cols] = df[rate_cols] / 100
 
     # Reorder columns based on the order of the dictionary
     return df[rename_dict.values()]
 
 
-def fetch_intraday(future_code: str) -> pd.DataFrame:
+def fetch_intraday_df(future_code: str) -> pd.DataFrame:
     """
     Fetch the latest DI futures data from B3.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing the latest DI futures data.
     """
     raw_df = _fetch_raw_df(future_code)
```

### Comparing `pyield-0.7.8/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.9/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.9/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/holidays/core.py` & `pyield-0.7.9/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/indicators.py` & `pyield-0.7.9/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/projections.py` & `pyield-0.7.9/pyield/projections.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyield/utils.py` & `pyield-0.7.9/pyield/utils.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/pyproject.toml` & `pyield-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "beautifulsoup4",
     "html5lib",
     "lxml",
     "python-calamine>=0.2.0",
     "requests>=2.31.0",
 ]
 dynamic = []
-version = "0.7.8"
+version = "0.7.9"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.8/tests/test_bday.py` & `pyield-0.7.9/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/tests/test_futures.py` & `pyield-0.7.9/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.8/PKG-INFO` & `pyield-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
```

