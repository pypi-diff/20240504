# Comparing `tmp/mptradelib-0.3.6.tar.gz` & `tmp/mptradelib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.6.tar", max compression
+gzip compressed data, was "mptradelib-0.3.7.tar", max compression
```

## Comparing `mptradelib-0.3.6.tar` & `mptradelib-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.6/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.6/mptradelib/__init__.py
--rw-r--r--   0        0        0     4572 2024-05-03 09:17:03.492484 mptradelib-0.3.6/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.6/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.6/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.6/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.6/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.6/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2338 2024-05-04 09:41:29.250845 mptradelib-0.3.6/mptradelib/cli/new.py
--rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.6/mptradelib/feed.py
--rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.6/mptradelib/livetrade.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.6/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.6/mptradelib/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2771 2024-05-04 09:39:02.808619 mptradelib-0.3.6/mptradelib/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.6/mptradelib/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.6/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.6/mptradelib/utils.py
--rw-r--r--   0        0        0      829 2024-05-04 09:42:16.840113 mptradelib-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.7/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4582 2024-05-04 11:45:49.548705 mptradelib-0.3.7/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.7/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.7/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.7/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.7/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.7/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2338 2024-05-04 09:41:29.250845 mptradelib-0.3.7/mptradelib/cli/new.py
+-rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.7/mptradelib/feed.py
+-rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.7/mptradelib/livetrade.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.7/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.7/mptradelib/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.3.7/mptradelib/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.7/mptradelib/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.7/mptradelib/test_renko.py
+-rw-r--r--   0        0        0     2748 2024-05-04 12:27:17.872441 mptradelib-0.3.7/mptradelib/utils.py
+-rw-r--r--   0        0        0      829 2024-05-04 12:27:28.517278 mptradelib-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.7/PKG-INFO
```

### Comparing `mptradelib-0.3.6/README.md` & `mptradelib-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/backtest.py` & `mptradelib-0.3.7/mptradelib/backtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,22 @@
 
 class Backtest:
     params: dict = {
         "sl": None,
         "tp": None
     }
 
-    __position: Order = None
-    __orders = []
-
     def __init__(self, data: pd.DataFrame, compute: Callable[[pd.DataFrame, dict], pd.DataFrame]=None, tp=2, sl=1, intraday=True):
         self.data = data
         self.compute = compute
         self.params['tp'] = tp
         self.params['sl'] = sl
         self.intraday = intraday
+        self.__orders = []
+        self.__position = None
 
     def run(self, **kwargs):
         self.params.update(kwargs)
 
         data = self.data.copy()
         
         data = self.compute(data, self.params)
```

### Comparing `mptradelib-0.3.6/mptradelib/broker/broker.py` & `mptradelib-0.3.7/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/broker/session.py` & `mptradelib-0.3.7/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/broker/ticker.py` & `mptradelib-0.3.7/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/cli/new.py` & `mptradelib-0.3.7/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/feed.py` & `mptradelib-0.3.7/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/livetrade.py` & `mptradelib-0.3.7/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/shoonya.py` & `mptradelib-0.3.7/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/templates/strategy/__init__.py.jinja` & `mptradelib-0.3.7/mptradelib/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.3.7/mptradelib/templates/strategy/backtest.ipynb.jinja`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9746428571428571%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(5, 'from mptradelib.utils import Tearsheet\\n')]}}, insert: "*

 * *            "[(4, OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', ['t = Tearsheet(out[0])\\n', "*

 * *            "'t.print()'])]))]}"}*

```diff
@@ -7,14 +7,15 @@
             "outputs": [],
             "source": [
                 "import pandas_ta as ta\n",
                 "import numpy as np\n",
                 "from mptradelib.backtest import Backtest\n",
                 "from mptradelib.broker.session import FyersSession\n",
                 "from mptradelib.broker.broker import Historical\n",
+                "from mptradelib.utils import Tearsheet\n",
                 "import datetime as dt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -77,14 +78,24 @@
                 "start = end - dt.timedelta(days=365*2)\n",
                 "df = h.historical(\"NSE:SBIN-EQ\", resolution=5, start=start, end=end)\n",
                 "\n",
                 "b = Backtest(df, compute, sl=1, tp=2, intraday=True)\n",
                 "out = b.run(**{k: int(v) for k, v in r[0].items()})\n",
                 "print(\"Profit: \", np.sum(out[0].profit))"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "t = Tearsheet(out[0])\n",
+                "t.print()"
+            ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python"
         }
     },
```

### Comparing `mptradelib-0.3.6/mptradelib/templates/strategy/livetrade.py.jinja` & `mptradelib-0.3.7/mptradelib/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/mptradelib/test_renko.py` & `mptradelib-0.3.7/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.6/pyproject.toml` & `mptradelib-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.3.6/PKG-INFO` & `mptradelib-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

