# Comparing `tmp/schwab-py-0.0.0a8.tar.gz` & `tmp/schwab-py-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a8.tar", last modified: Sun Apr 14 18:27:09 2024, max compression
+gzip compressed data, was "schwab-py-0.0.0a9.tar", last modified: Sun Apr 14 18:49:14 2024, max compression
```

## Comparing `schwab-py-0.0.0a8.tar` & `schwab-py-0.0.0a9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.045671 schwab-py-0.0.0a8/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a8/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:27:09.045597 schwab-py-0.0.0a8/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a8/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.043051 schwab-py-0.0.0a8/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a8/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a8/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.043558 schwab-py-0.0.0a8/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a8/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a8/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    27732 2024-04-14 18:26:28.000000 schwab-py-0.0.0a8/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a8/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a8/schwab/debug.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.044223 schwab-py-0.0.0a8/schwab/orders/
--rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a8/schwab/orders/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    11013 2024-04-14 17:35:12.000000 schwab-py-0.0.0a8/schwab/orders/common.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-04-14 17:35:34.000000 schwab-py-0.0.0a8/schwab/orders/equities.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    14184 2024-04-14 17:37:24.000000 schwab-py-0.0.0a8/schwab/orders/generic.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17394 2024-04-14 17:35:49.000000 schwab-py-0.0.0a8/schwab/orders/options.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a8/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-14 18:26:39.000000 schwab-py-0.0.0a8/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.045114 schwab-py-0.0.0a8/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-14 18:27:09.045986 schwab-py-0.0.0a8/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a8/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.044961 schwab-py-0.0.0a8/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a8/tests/test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.268338 schwab-py-0.0.0a9/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a9/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:49:14.268278 schwab-py-0.0.0a9/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a9/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.265801 schwab-py-0.0.0a9/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a9/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a9/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.266307 schwab-py-0.0.0a9/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a9/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a9/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    34237 2024-04-14 18:48:14.000000 schwab-py-0.0.0a9/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a9/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a9/schwab/debug.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.266969 schwab-py-0.0.0a9/schwab/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a9/schwab/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    11013 2024-04-14 17:35:12.000000 schwab-py-0.0.0a9/schwab/orders/common.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-04-14 17:35:34.000000 schwab-py-0.0.0a9/schwab/orders/equities.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14184 2024-04-14 17:37:24.000000 schwab-py-0.0.0a9/schwab/orders/generic.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17394 2024-04-14 17:35:49.000000 schwab-py-0.0.0a9/schwab/orders/options.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a9/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-14 18:48:56.000000 schwab-py-0.0.0a9/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.267805 schwab-py-0.0.0a9/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-14 18:49:14.268654 schwab-py-0.0.0a9/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a9/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.267657 schwab-py-0.0.0a9/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a9/tests/test.py
```

### Comparing `schwab-py-0.0.0a8/LICENSE` & `schwab-py-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/PKG-INFO` & `schwab-py-0.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a8/README.rst` & `schwab-py-0.0.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/auth.py` & `schwab-py-0.0.0a9/schwab/auth.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/client/asynchronous.py` & `schwab-py-0.0.0a9/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/client/base.py` & `schwab-py-0.0.0a9/schwab/client/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -688,7 +688,169 @@
                         'value of \'indicative\' must be either True or False')
             params['indicative'] = 'true' if indicative else 'false'
 
         path = '/marketdata/v1/quotes'
         return self._get_request(path, params)
 
 
+    ##########################################################################
+    # Option Chains
+
+    class Options:
+        class ContractType(Enum):
+            CALL = 'CALL'
+            PUT = 'PUT'
+            ALL = 'ALL'
+
+        class Strategy(Enum):
+            SINGLE = 'SINGLE'
+            ANALYTICAL = 'ANALYTICAL'
+            COVERED = 'COVERED'
+            VERTICAL = 'VERTICAL'
+            CALENDAR = 'CALENDAR'
+            STRANGLE = 'STRANGLE'
+            STRADDLE = 'STRADDLE'
+            BUTTERFLY = 'BUTTERFLY'
+            CONDOR = 'CONDOR'
+            DIAGONAL = 'DIAGONAL'
+            COLLAR = 'COLLAR'
+            ROLL = 'ROLL'
+
+        class StrikeRange(Enum):
+            IN_THE_MONEY = 'ITM'
+            NEAR_THE_MONEY = 'NTM'
+            OUT_OF_THE_MONEY = 'OTM'
+            STRIKES_ABOVE_MARKET = 'SAK'
+            STRIKES_BELOW_MARKET = 'SBK'
+            STRIKES_NEAR_MARKET = 'SNK'
+            ALL = 'ALL'
+
+        class Type(Enum):
+            STANDARD = 'S'
+            NON_STANDARD = 'NS'
+            ALL = 'ALL'
+
+        class ExpirationMonth(Enum):
+            JANUARY = 'JAN'
+            FEBRUARY = 'FEB'
+            MARCH = 'MAR'
+            APRIL = 'APR'
+            MAY = 'MAY'
+            JUNE = 'JUN'
+            JULY = 'JUL'
+            AUGUST = 'AUG'
+            SEPTEMBER = 'SEP'
+            OCTOBER = 'OCT'
+            NOVEMBER = 'NOV'
+            DECEMBER = 'DEC'
+
+        class Entitlement(Enum):
+            PAYING_PRO = 'PP'
+            NON_PRO = 'NP'
+            NON_PAYING_PRO = 'PN'
+
+    def get_option_chain(
+            self,
+            symbol,
+            *,
+            contract_type=None,
+            strike_count=None,
+            include_underlying_quote=None,
+            strategy=None,
+            interval=None,
+            strike=None,
+            strike_range=None,
+            from_date=None,
+            to_date=None,
+            volatility=None,
+            underlying_price=None,
+            interest_rate=None,
+            days_to_expiration=None,
+            exp_month=None,
+            option_type=None,
+            entitlement=None):
+        '''Get option chain for an optionable Symbol.
+
+        :param contract_type: Type of contracts to return in the chain. See
+                              :class:`Options.ContractType` for choices.
+        :param strike_count: The number of strikes to return above and below
+                             the at-the-money price.
+        :param include_underlying_quote: Include a quote for the underlying 
+                                         alongside the options chain?
+        :param strategy: If passed, returns a Strategy Chain. See
+                        :class:`Options.Strategy` for choices.
+        :param interval: Strike interval for spread strategy chains (see
+                         ``strategy`` param).
+        :param strike: Return options only at this strike price.
+        :param strike_range: Return options for the given range. See
+                             :class:`Options.StrikeRange` for choices.
+        :param from_date: Only return expirations after this date. For
+                          strategies, expiration refers to the nearest term
+                          expiration in the strategy. Accepts ``datetime.date``
+                          and ``datetime.datetime``.
+        :param to_date: Only return expirations before this date. For
+                        strategies, expiration refers to the nearest term
+                        expiration in the strategy. Accepts ``datetime.date``
+                        and ``datetime.datetime``.
+        :param volatility: Volatility to use in calculations. Applies only to
+                           ``ANALYTICAL`` strategy chains.
+        :param underlying_price: Underlying price to use in calculations.
+                                 Applies only to ``ANALYTICAL`` strategy chains.
+        :param interest_rate: Interest rate to use in calculations. Applies only
+                              to ``ANALYTICAL`` strategy chains.
+        :param days_to_expiration: Days to expiration to use in calculations.
+                                   Applies only to ``ANALYTICAL`` strategy
+                                   chains
+        :param exp_month: Return only options expiring in the specified month. See
+                          :class:`Options.ExpirationMonth` for choices.
+        :param option_type: Types of options to return. See
+                            :class:`Options.Type` for choices.
+        :param entitlement: Entitlement of the client.
+        '''
+        contract_type = self.convert_enum(
+            contract_type, self.Options.ContractType)
+        strategy = self.convert_enum(strategy, self.Options.Strategy)
+        strike_range = self.convert_enum(
+            strike_range, self.Options.StrikeRange)
+        option_type = self.convert_enum(option_type, self.Options.Type)
+        exp_month = self.convert_enum(exp_month, self.Options.ExpirationMonth)
+
+        params = {
+            'apikey': self.api_key,
+            'symbol': symbol,
+        }
+
+        if contract_type is not None:
+            params['contractType'] = contract_type
+        if strike_count is not None:
+            params['strikeCount'] = strike_count
+        if include_underlying_quote is not None:
+            params['includeUnderlyingQuote'] = include_underlying_quote
+        if strategy is not None:
+            params['strategy'] = strategy
+        if interval is not None:
+            params['interval'] = interval
+        if strike is not None:
+            params['strike'] = strike
+        if strike_range is not None:
+            params['range'] = strike_range
+        if from_date is not None:
+            params['fromDate'] = self._format_date('from_date', from_date)
+        if to_date is not None:
+            params['toDate'] = self._format_date('to_date', to_date)
+        if volatility is not None:
+            params['volatility'] = volatility
+        if underlying_price is not None:
+            params['underlyingPrice'] = underlying_price
+        if interest_rate is not None:
+            params['interestRate'] = interest_rate
+        if days_to_expiration is not None:
+            params['daysToExpiration'] = days_to_expiration
+        if exp_month is not None:
+            params['expMonth'] = exp_month
+        if option_type is not None:
+            params['optionType'] = option_type
+
+        path = '/marketdata/v1/chains'
+        return self._get_request(path, params)
+
+
```

### Comparing `schwab-py-0.0.0a8/schwab/client/synchronous.py` & `schwab-py-0.0.0a9/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/debug.py` & `schwab-py-0.0.0a9/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/orders/__init__.py` & `schwab-py-0.0.0a9/schwab/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/orders/common.py` & `schwab-py-0.0.0a9/schwab/orders/common.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/orders/equities.py` & `schwab-py-0.0.0a9/schwab/orders/equities.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/orders/generic.py` & `schwab-py-0.0.0a9/schwab/orders/generic.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/orders/options.py` & `schwab-py-0.0.0a9/schwab/orders/options.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab/utils.py` & `schwab-py-0.0.0a9/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a9/schwab_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a8/schwab_py.egg-info/SOURCES.txt` & `schwab-py-0.0.0a9/schwab_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/setup.cfg` & `schwab-py-0.0.0a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a8/setup.py` & `schwab-py-0.0.0a9/setup.py`

 * *Files identical despite different names*

