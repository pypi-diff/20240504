# Comparing `tmp/byteforge_coinmarketcap-1.2.tar.gz` & `tmp/byteforge_coinmarketcap-1.3.tar.gz`

## Comparing `byteforge_coinmarketcap-1.2.tar` & `byteforge_coinmarketcap-1.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/MANIFEST
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/__init__.py
--rwxr-xr-x   0        0        0     3946 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/types/__init__.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/types/token_state.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/common.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/latest.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/v2/cryptocurrency/quotes/historical.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/doc/coinmarketcap.png
--rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/doc/coinmarketcap_original.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/tests/__init__.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/tests/test_coinmarketcap.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/.gitignore
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/LICENSE
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/README.md
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/pyproject.toml
--rw-r--r--   0        0        0    24601 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/MANIFEST
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/types/__init__.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/types/token_state.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/common.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/latest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/key/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/key/info.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v2/cryptocurrency/quotes/historical.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/doc/coinmarketcap.png
+-rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/doc/coinmarketcap_original.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/tests/__init__.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/tests/test_coinmarketcap.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/.gitignore
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/LICENSE
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/README.md
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/pyproject.toml
+-rw-r--r--   0        0        0    25988 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/PKG-INFO
```

### Comparing `byteforge_coinmarketcap-1.2/coinmarketcap/core.py` & `byteforge_coinmarketcap-1.3/coinmarketcap/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import requests_cache
 from typing import Optional, List
 
 from .types.token_state import TokenState, Quote
 from .v2.cryptocurrency.quotes.historical import _quotes_historical_v2
 from .v1.cryptocurrency.listings.latest import _listings_latest
 from .v1.cryptocurrency.listings.common import SortOption, AuxFields, SortDir, FilterOptions
+from .v1.key.info import _key_info
+from .v1.key.info import _calls_left_today
 
 class Market(object):
 
 	_session = None
 	_debug_mode = False
 	_api_key = None
 	__DEFAULT_BASE_URL = 'https://pro-api.coinmarketcap.com/'
@@ -85,27 +87,25 @@
 					start: int = 1, 
 					limit: int = 100, 
 					convert: List[str] = ['USD'],
 					aux_fields: AuxFields = None, 
 					filters: FilterOptions = None) -> List[TokenState]:
 		
 		return _listings_latest(self, sort_by, sort_dir, start, limit, convert, aux_fields, filters)
+	
 
-
-	# TODO - this should call global metrics endpoint
-	def stats(self, **kwargs):
-		"""
-		This endpoint displays the global data found at the top of coinmarketcap.com.
-
-		Optional parameters:
-		(string) convert - return pricing info in terms of another currency.
-		Valid fiat currency values are: "AUD", "BRL", "CAD", "CHF", "CLP", "CNY", "CZK",
-		"DKK", "EUR", "GBP", "HKD", "HUF", "IDR", "ILS", "INR", "JPY", "KRW", "MXN",
-		"MYR", "NOK", "NZD", "PHP", "PKR", "PLN", "RUB", "SEK", "SGD", "THB", "TRY",
-		"TWD", "ZAR"
-		Valid cryptocurrency values are: "BTC", "ETH" "XRP", "LTC", and "BCH"
+	def calls_left_today(self):
 		"""
+		Calculates how many API calls are left for today, based on the service plan's monthly call limit.
 
-		params = {}
-		params.update(kwargs)
-		response = self._request('global/', params)
-		return response
+		This function takes the user's API call limit and subtracts the number of calls used to date,
+		providing a simple ratio to estimate daily available calls until the reset date. Note that 
+		this is an approximation based on equal usage each day until the reset.
+
+		Parameters:
+			market (Market): An instance of the Market class, which handles the API communications.
+
+		Returns:
+			int: Approximate number of API calls left for the current day, based on daily usage 
+				till the reset date and a monthly limit.
+		"""		
+		return _calls_left_today(self)
```

### Comparing `byteforge_coinmarketcap-1.2/coinmarketcap/types/token_state.py` & `byteforge_coinmarketcap-1.3/coinmarketcap/types/token_state.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/common.py` & `byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/common.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/latest.py` & `byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/latest.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/coinmarketcap/v2/cryptocurrency/quotes/historical.py` & `byteforge_coinmarketcap-1.3/coinmarketcap/v2/cryptocurrency/quotes/historical.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/doc/coinmarketcap.png` & `byteforge_coinmarketcap-1.3/doc/coinmarketcap.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/doc/coinmarketcap_original.png` & `byteforge_coinmarketcap-1.3/doc/coinmarketcap_original.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/tests/test_coinmarketcap.py` & `byteforge_coinmarketcap-1.3/tests/test_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/LICENSE` & `byteforge_coinmarketcap-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.2/README.md` & `byteforge_coinmarketcap-1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -246,14 +246,39 @@
 - `m`: Retrieves a quote available every "m" minutes. Supported intervals: `5m`, `10m`, `15m`, `30m`, `45m`.
 - `h`: Retrieves a quote available every "h" hours. Supported intervals: `1h`, `2h`, `3h`, `4h`, `6h`, `12h`.
 - `d`: Retrieves a quote available every "d" days. Supported intervals: `1d`, `2d`, `3d`, `7d`, `14d`, `15d`, `30d`, `60d`, `90d`, `365d`.
 
 Please ensure to select the interval that best matches your data analysis needs.
 
 
+To include the new `calls_left_today` routine in your existing project documentation, add a section that explains its purpose, usage, and example code on how to call it. Below is a suggested format for including this information in your README:
+
+## Monitoring API Usage
+
+As you utilize the API, it's important to manage the number of requests to stay within your plan's limits. The `calls_left_today` function provides an easy way to monitor your daily API usage against your monthly limits.
+
+### Purpose
+
+The `calls_left_today` method estimates the number of API calls you can still make for the current day without exceeding your monthly limit. This is crucial for applications that need to manage request rates or distribute API calls evenly throughout a billing period.
+
+### Usage
+
+2. **Call the `calls_left_today` Method**:
+   Use the `calls_left_today` method to find out how many more API calls you can make today.
+
+```python
+remaining_calls = market.calls_left_today()
+print(f"You have {remaining_calls} API calls left for today.")
+```
+
+### Note
+
+- **Accuracy**: Please note that this function provides an approximation. If your daily API call volume varies significantly, consider implementing more detailed tracking mechanisms.
+- **Reset Timing**: Be aware of your API subscription details, especially when the monthly call count resets, as this will affect the calculations.
+
 
 ## License:
 
 ```
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `byteforge_coinmarketcap-1.2/pyproject.toml` & `byteforge_coinmarketcap-1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byteforge-coinmarketcap"
-version = "1.2"
+version = "1.3"
 description = "Python SDK for the coinmarketcap.com API."
 readme = "README.md"
 license = { file="LICENSE" }
 keywords = ["cryptocurrency", "API", "coinmarketcap", "BTC", "Bitcoin", "LTC", "Litecoin", "XRP", "Ripple", "ETH", "Ethereum"]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `byteforge_coinmarketcap-1.2/PKG-INFO` & `byteforge_coinmarketcap-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: byteforge-coinmarketcap
-Version: 1.2
+Version: 1.3
 Summary: Python SDK for the coinmarketcap.com API.
 Project-URL: Homepage, https://github.com/jmazzahacks/byteforge-coinmarketcap/
 Project-URL: Issues, https://github.com/jmazzahacks/byteforge-coinmarketcap/issues
 Author: Jason Byteforgia
 License:                              Apache License
                                Version 2.0, January 2004
                             http://www.apache.org/licenses/
@@ -465,14 +465,39 @@
 - `m`: Retrieves a quote available every "m" minutes. Supported intervals: `5m`, `10m`, `15m`, `30m`, `45m`.
 - `h`: Retrieves a quote available every "h" hours. Supported intervals: `1h`, `2h`, `3h`, `4h`, `6h`, `12h`.
 - `d`: Retrieves a quote available every "d" days. Supported intervals: `1d`, `2d`, `3d`, `7d`, `14d`, `15d`, `30d`, `60d`, `90d`, `365d`.
 
 Please ensure to select the interval that best matches your data analysis needs.
 
 
+To include the new `calls_left_today` routine in your existing project documentation, add a section that explains its purpose, usage, and example code on how to call it. Below is a suggested format for including this information in your README:
+
+## Monitoring API Usage
+
+As you utilize the API, it's important to manage the number of requests to stay within your plan's limits. The `calls_left_today` function provides an easy way to monitor your daily API usage against your monthly limits.
+
+### Purpose
+
+The `calls_left_today` method estimates the number of API calls you can still make for the current day without exceeding your monthly limit. This is crucial for applications that need to manage request rates or distribute API calls evenly throughout a billing period.
+
+### Usage
+
+2. **Call the `calls_left_today` Method**:
+   Use the `calls_left_today` method to find out how many more API calls you can make today.
+
+```python
+remaining_calls = market.calls_left_today()
+print(f"You have {remaining_calls} API calls left for today.")
+```
+
+### Note
+
+- **Accuracy**: Please note that this function provides an approximation. If your daily API call volume varies significantly, consider implementing more detailed tracking mechanisms.
+- **Reset Timing**: Be aware of your API subscription details, especially when the monthly call count resets, as this will affect the calculations.
+
 
 ## License:
 
 ```
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

