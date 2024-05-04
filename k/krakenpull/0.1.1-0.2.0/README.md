# Comparing `tmp/krakenpull-0.1.1.tar.gz` & `tmp/krakenpull-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakenpull-0.1.1.tar", max compression
+gzip compressed data, was "krakenpull-0.2.0.tar", max compression
```

## Comparing `krakenpull-0.1.1.tar` & `krakenpull-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1362 2024-04-20 20:15:10.421813 krakenpull-0.1.1/README.md
--rw-r--r--   0        0        0     1793 2024-04-20 20:15:10.421813 krakenpull-0.1.1/krakenpull/__init__.py
--rw-r--r--   0        0        0     7276 2024-04-20 20:15:10.421813 krakenpull-0.1.1/krakenpull/client.py
--rw-r--r--   0        0        0     1386 2024-04-20 20:15:10.421813 krakenpull-0.1.1/krakenpull/env.py
--rw-r--r--   0        0        0     2465 2024-04-20 20:15:10.421813 krakenpull-0.1.1/krakenpull/models.py
--rw-r--r--   0        0        0      276 2024-04-20 20:15:10.421813 krakenpull-0.1.1/krakenpull/utils.py
--rw-r--r--   0        0        0      492 2024-04-20 20:15:10.421813 krakenpull-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 krakenpull-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1362 2024-05-04 18:05:55.119321 krakenpull-0.2.0/README.md
+-rw-r--r--   0        0        0     1793 2024-05-04 18:05:55.119321 krakenpull-0.2.0/krakenpull/__init__.py
+-rw-r--r--   0        0        0     7728 2024-05-04 18:05:55.123321 krakenpull-0.2.0/krakenpull/client.py
+-rw-r--r--   0        0        0     1386 2024-05-04 18:05:55.123321 krakenpull-0.2.0/krakenpull/env.py
+-rw-r--r--   0        0        0     2478 2024-05-04 18:05:55.123321 krakenpull-0.2.0/krakenpull/models.py
+-rw-r--r--   0        0        0      531 2024-05-04 18:05:55.123321 krakenpull-0.2.0/krakenpull/utils.py
+-rw-r--r--   0        0        0      492 2024-05-04 18:05:55.123321 krakenpull-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 krakenpull-0.2.0/PKG-INFO
```

### Comparing `krakenpull-0.1.1/README.md` & `krakenpull-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `krakenpull-0.1.1/krakenpull/__init__.py` & `krakenpull-0.2.0/krakenpull/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 
-VERSION = "0.1.1"
+VERSION = "0.2.0"
 
 
 if typing.TYPE_CHECKING:
     # import of virtually everything is supported via `__getattr__` below,
     # but we need them here for type checking and IDE support
     from .models import (
         NonfiatCurrency,
```

### Comparing `krakenpull-0.1.1/krakenpull/client.py` & `krakenpull-0.2.0/krakenpull/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from krakenpull.models import (
     CurrencyPair,
     ClosedTransaction,
     Currency,
     TickerInfo,
     JSON,
 )
+from krakenpull.utils import get_unique_tickers
 
 BASE_URL = "https://api.kraken.com/0"
 
 
 class AbstractKraken(abc.ABC):
     @abc.abstractmethod
     def __init__(self, key: str, private_key: str):
@@ -40,19 +41,35 @@
     def get_closed_orders(self, trades: bool = False) -> list[ClosedTransaction]:
         raise NotImplementedError
 
     def get_ticker_info(
         self, currency_pairs: list[CurrencyPair] | CurrencyPair
     ) -> list[TickerInfo]:
         url, _ = self._return_url_endpoint(endpoint="Ticker")
-        pairs = currency_pairs if isinstance(currency_pairs, list) else [currency_pairs]
+        pairs = get_unique_tickers(
+            currency_pairs if isinstance(currency_pairs, list) else [currency_pairs]
+        )
+
+        usd_ticker = []
+        if (Currency.ZUSD, Currency.USD) in pairs:
+            index = pairs.index((Currency.ZUSD, Currency.USD))
+            pairs.pop(index)
+            usd_ticker = [
+                TickerInfo(
+                    pair=(Currency.ZUSD, Currency.USD),
+                    price=1,
+                    low=1,
+                    high=1,
+                )
+            ]
+
         stringed_pairs = ["".join(c.value for c in pair) for pair in pairs]
         res = requests.post(f"{url}?pair={','.join(stringed_pairs)}")
         result = self._get_result(res, op="get ticker info")
-        return [
+        return usd_ticker + [
             TickerInfo.model_validate(
                 {
                     "pair": pair_id,
                     "price": data["a"][0],
                     "low": data["l"][0],
                     "high": data["h"][0],
                 },
@@ -123,18 +140,14 @@
     def get_closed_orders(self, trades: bool = False) -> list[ClosedTransaction]:
         return self._transactions
 
     def _get_server_time_unix(self) -> int:
         return int(time.time() * 1000)
 
 
-# FIXME
-# get_env_variables().KRAKEN_API_KEY
-
-
 class Kraken(AbstractKraken):
     def __init__(self, key: str, private_key: str):
         super().__init__(key, private_key)
         self.api_key = key
         self.private_key = private_key
 
     def get_order_book(self, currency_pair: CurrencyPair) -> JSON:
```

### Comparing `krakenpull-0.1.1/krakenpull/env.py` & `krakenpull-0.2.0/krakenpull/env.py`

 * *Files identical despite different names*

### Comparing `krakenpull-0.1.1/krakenpull/models.py` & `krakenpull-0.2.0/krakenpull/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,32 +43,31 @@
 
 
 class TransactionType(Enum):
     buy = "buy"
     sell = "sell"
 
 
-# FIXME
-# OrderType = Literal['limit', 'market', 'stop-loss', 'take-profit']
-
-
 class OrderType(Enum):
     limit = "limit"
     market = "market"
     stop_loss = "stop-loss"
     take_profit = "take-profit"
 
 
 class BaseTickerInfo(BaseModel):
     pair: CurrencyPair
     price: float
 
     @field_validator("pair", mode="before")
     @classmethod
-    def parse_pair(cls, v: str) -> tuple[Currency, Currency]:
+    def parse_pair(cls, v: str | tuple) -> tuple[Currency, Currency]:
+        if isinstance(v, tuple):
+            return Currency(v[0]), Currency(v[1])
+
         if v == "USDZUSD" or v == "USDTZUSD":
             return Currency.USDT, Currency.USD
 
         try:
             currency1 = Currency(v[:3])
         except ValueError:
             try:
```

### Comparing `krakenpull-0.1.1/PKG-INFO` & `krakenpull-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krakenpull
-Version: 0.1.1
+Version: 0.2.0
 Summary: A user friendly Kraken API client using pydantic 🐙
 Author: marc
 Author-email: marc@mawaie.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

