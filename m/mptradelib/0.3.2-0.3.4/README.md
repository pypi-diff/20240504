# Comparing `tmp/mptradelib-0.3.2.tar.gz` & `tmp/mptradelib-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.2.tar", max compression
+gzip compressed data, was "mptradelib-0.3.4.tar", max compression
```

## Comparing `mptradelib-0.3.2.tar` & `mptradelib-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.2/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.2/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.2/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.2/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.2/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.2/mptradelib/feed.py
--rw-r--r--   0        0        0     1866 2024-05-02 08:01:45.468179 mptradelib-0.3.2/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.2/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.2/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.2/mptradelib/utils.py
--rw-r--r--   0        0        0     4193 2024-05-02 14:00:12.492668 mptradelib-0.3.2/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-05-03 03:52:20.749789 mptradelib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.4/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4572 2024-05-03 09:17:03.492484 mptradelib-0.3.4/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.4/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.4/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.4/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.4/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.4/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2330 2024-05-03 13:17:36.227537 mptradelib-0.3.4/mptradelib/cli/new.py
+-rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.4/mptradelib/feed.py
+-rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.4/mptradelib/livetrade.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.4/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.4/mptradelib/templates/strategy/__init__.jinja
+-rw-r--r--   0        0        0     1187 2024-05-03 13:10:47.542853 mptradelib-0.3.4/mptradelib/templates/strategy/backtest.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.4/mptradelib/templates/strategy/livetrade.jinja
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.4/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.4/mptradelib/utils.py
+-rw-r--r--   0        0        0      829 2024-05-03 13:07:16.260293 mptradelib-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.4/PKG-INFO
```

### Comparing `mptradelib-0.3.2/README.md` & `mptradelib-0.3.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# Installation
+Create a virtualenv.
+```
+pip install mptradelib
+```
+**Install `pandas_ta` as extra.
+
+# Create strategy
+```
+mpt create <strategy_name>
+```
+
 # Backtest
 
 ### Prepare data (example)
 ```
 import pandas as pd
 import numpy as np
 
@@ -97,42 +109,38 @@
     def next(self, symbol, data):
         ema_fast = ta.ema(data.df.close, self.ema_fast)
         ema_slow = ta.ema(data.df.close, self.ema_slow)
         ema_trend = ta.ema(data.df.close, self.ema_trend)
 
         self.b.buy()
 
-r = redis.Redis(
-    host='127.0.0.1',
-    port=6379,
-    decode_responses=True # <-- this will ensure that binary data is decoded
-)
-
-
-f = FyersSession()
-feed = LiveTicker(f, r, "ticks")
-
-end_date = dt.datetime.now()
-start_date = end_date - dt.timedelta(days=7)
-h = HistoricalV2(f)
-hd = h.historical("MCX", "CRUDEOILM24MAYFUT", 1, start_date, end_date)
-
-def producer():
-    feed.run()
-
-    if feed.is_live:
-        feed.subscribe(["MCX:CRUDEOILM24MAYFUT"])
-
-def consumer():
-    datas = Datas(r)
-    datas.load("MCX:CRUDEOILM24MAYFUT", hd.to_dict('records'))
-    l = LiveTrading(MyStrategy)
-    l.set_datas(datas)
-    l.run(ema_fast=20, ema_slow=50, ema_trend=200, sl=1, tp=2)
-    
-
-t = threading.Thread(target=producer)
-t.start()
+```
 
-consumer()
+### Run
+```
+mpt runlive <strategy_name> --symbols NSE:SBIN-EQ,NSE:CANB-EQ --param {}
+```
 
-```
+### Param
+Param can be in two formats-
+```
+pars = {
+        "NSE:SBIN-EQ": {
+            "ema_fast": 20,
+            "ema_slow": 50,
+            "ema_trend": 200,
+            "sl": 1,
+            "tp": 2
+        }
+    }
+```
+OR
+```
+{
+    "ema_fast": 20,
+    "ema_slow": 50,
+    "ema_trend": 200,
+    "sl": 1,
+    "tp": 2
+}
+```
+In later case, same params are used for all symbols.
```

### Comparing `mptradelib-0.3.2/mptradelib/broker/broker.py` & `mptradelib-0.3.4/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/broker/session.py` & `mptradelib-0.3.4/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/broker/ticker.py` & `mptradelib-0.3.4/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/feed.py` & `mptradelib-0.3.4/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/livetrading.py` & `mptradelib-0.3.4/mptradelib/livetrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pydantic
 import copy
 
 class BaseStrategy(pydantic.BaseModel):
     def next(self, symbol: str, data: Series) -> None:
         raise NotImplementedError
 
-class LiveTrading:
+class LiveTrade:
     _datas: Datas = None
     _s: BaseStrategy
     b: BaseBroker
     _p: dict = {}
 
     def __init__(self, s: BaseStrategy.__class__) -> None:
         self._s = s()
```

### Comparing `mptradelib-0.3.2/mptradelib/shoonya.py` & `mptradelib-0.3.4/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/test_renko.py` & `mptradelib-0.3.4/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/utils.py` & `mptradelib-0.3.4/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.2/mptradelib/vectorised_backtest.py` & `mptradelib-0.3.4/mptradelib/backtest.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,16 +94,27 @@
             elif self.__position.direction == -1:
                 if row.close >= self.__position.sl or row.close <= self.__position.tp:
                     self._exit_position(row)
 
         if row.entries != 0 and self.__position is None and self._in_intraday_window(row):
             self.__position = Order(entry_time=row.trade_time, entry_price=row.entry_price, sl=row.sl, tp=row.tp, direction=row.entries)
 
+    def _define_space(self, params):
+        space = {}
+        for k, v in params.items():
+            if isinstance(v.step, int):
+                space[k] = scope.int(hp.quniform(k, v.start, v.stop, v.step))
+            elif isinstance(v.step, float):
+                space[k] = hp.quniform(k, v.start, v.stop, v.step)
+            else:
+                raise ValueError(f"step of {k} can not be {type(v.step)}")
+        return space
+
     def _optimizer(self, **kwargs):
-        space = { k: scope.int(hp.quniform(k, v.start, v.stop, v.step)) for k, v in kwargs.items()}
+        space = self._define_space(kwargs)
         
         def objective(params):
             r = self.run(**params)
             return {'loss': -np.sum(r[0].profit), 'status': STATUS_OK}
         
         best = fmin(
             fn=objective,
```

### Comparing `mptradelib-0.3.2/pyproject.toml` & `mptradelib-0.3.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.2"
+version = "0.3.4"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
 requests = "2.31.0"
 fyers-apiv3 = "3.0.6"
 retry = "0.9.2"
 pyotp = "2.9.0"
+jinja2 = "^3.1.3"
+click = "^8.1.7"
+jinja2-strcase = "^0.0.2"
+redis = "^5.0.4"
+pandas-ta = "^0.3.14b0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 
-[tool.poetry.group.extra]
-optional = true
+pandas_ta = { version = "^0.3.14b", optional = true }
+pandas = { version = "^2.1.4", optional = true }
+hyperopt = { version = "^0.2.7", optional = true }
 
-[tool.poetry.group.extra.dependencies]
-pandas = "^2.1.4"
-hyperopt = "^0.2.7"
-redis = "^5.0.4"
+[tool.poetry.extras]
+pandasta = ["pandas_ta"]
+pandas = ["pandas"]
+hyperopt = ["hyperopt"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+mpt = 'mptradelib.cli.new:commands'
```

