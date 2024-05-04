# Comparing `tmp/rollercoaster-2.1.3.tar.gz` & `tmp/rollercoaster-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rollercoaster-2.1.3.tar", max compression
+gzip compressed data, was "rollercoaster-2.1.4.tar", max compression
```

## Comparing `rollercoaster-2.1.3.tar` & `rollercoaster-2.1.4.tar`

### file list

```diff
@@ -1,387 +1,272 @@
--rw-r--r--   0        0        0     1654 2024-04-17 00:36:01.519814 rollercoaster-2.1.3/pyproject.toml
--rwxr-xr-x   0        0        0     2102 2024-04-04 23:37:49.640824 rollercoaster-2.1.3/readme.md
--rwxr-xr-x   0        0        0     1312 2024-04-16 18:04:08.058879 rollercoaster-2.1.3/venue.S.HTML
--rw-r--r--   0        0        0       74 2024-04-08 20:59:40.730227 rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/itinerary - aspirations.S.HTML
--rwxr-xr-x   0        0        0      635 2024-04-09 00:03:01.343222 rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      574 2024-04-08 21:03:27.655704 rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/sequentials/sequentials.S.HTML
--rwxr-xr-x   0        0        0    51873 2024-03-17 02:26:50.689331 rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/sporatic/TradingView Screen.png
--rwxr-xr-x   0        0        0      381 2024-03-31 19:05:52.370949 rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/sporatic/itinerary.S.HTML
--rwxr-xr-x   0        0        0      384 2024-04-05 03:51:30.492335 rollercoaster-2.1.3/venues/stages/rollercoaster/__bin/rollercoaster_1
--rw-r--r--   0        0        0      630 2024-04-09 02:16:03.303817 rollercoaster-2.1.3/venues/stages/rollercoaster/__data_nodes/moon/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      225 2024-04-09 02:15:48.675989 rollercoaster-2.1.3/venues/stages/rollercoaster/__data_nodes/moon/clique.py
--rwxr-xr-x   0        0        0   845985 2024-04-05 04:00:12.449831 rollercoaster-2.1.3/venues/stages/rollercoaster/__data_nodes/moon/listing_status.csv
--rwxr-xr-x   0        0        0      508 2024-04-05 04:00:10.553855 rollercoaster-2.1.3/venues/stages/rollercoaster/__data_nodes/moon/mongo.S.HTML
--rwxr-xr-x   0        0        0       45 2024-04-04 18:35:08.441995 rollercoaster-2.1.3/venues/stages/rollercoaster/__init__.py
--rwxr-xr-x   0        0        0     1960 2024-04-09 02:16:01.627837 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/__init__.py
--rw-r--r--   0        0        0     2314 2024-04-09 02:16:03.227818 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.090558 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/group/__init__.py
--rwxr-xr-x   0        0        0      764 2024-02-28 18:16:04.681273 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0       53 2024-03-31 19:15:22.692288 rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/sanic_trails/strails.S.HTML
--rwxr-xr-x   0        0        0   227295 2024-04-17 00:35:50.355960 rollercoaster-2.1.3/venues/stages/rollercoaster/_status/DB/records.json
--rw-r--r--   0        0        0      337 2024-04-16 18:04:33.514601 rollercoaster-2.1.3/venues/stages/rollercoaster/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1314 2024-04-17 00:35:43.012056 rollercoaster-2.1.3/venues/stages/rollercoaster/_status/clouds_status.proc.py
--rwxr-xr-x   0        0        0     1193 2024-04-17 00:35:40.616088 rollercoaster-2.1.3/venues/stages/rollercoaster/_status/status.proc.py
--rwxr-xr-x   0        0        0      114 2024-03-17 06:14:54.911123 rollercoaster-2.1.3/venues/stages/rollercoaster/_status/status_1.py
--rwxr-xr-x   0        0        0      129 2024-01-26 16:01:45.729782 rollercoaster-2.1.3/venues/stages/rollercoaster/charts/charts.s.HTML
--rwxr-xr-x   0        0        0      821 2024-03-17 23:24:26.718972 rollercoaster-2.1.3/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML
--rwxr-xr-x   0        0        0      661 2024-03-31 20:40:53.750991 rollercoaster-2.1.3/venues/stages/rollercoaster/climate/__init__.py
--rwxr-xr-x   0        0        0      913 2024-03-31 20:40:56.818964 rollercoaster-2.1.3/venues/stages/rollercoaster/climate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1182 2023-12-19 04:09:04.651687 rollercoaster-2.1.3/venues/stages/rollercoaster/climate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      170 2024-04-04 19:34:53.736179 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/AV/AV.s.HTML
--rwxr-xr-x   0        0        0      276 2024-03-17 21:13:24.014422 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/Alpaca.s.HTML
--rw-r--r--   0        0        0      160 2024-04-09 00:53:14.647459 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/_data_API/data.S.HTML
--rw-r--r--   0        0        0      989 2024-04-09 02:18:01.710435 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/_data_API/v2/stock/symbol/__pycache__/bars.cpython-310.pyc
--rw-r--r--   0        0        0      798 2024-04-09 02:17:59.726458 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py
--rwxr-xr-x   0        0        0     2427 2023-12-03 20:14:57.298037 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1229 2024-03-17 20:49:06.769841 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/__pycache__/retrieve.cpython-310.pyc
--rwxr-xr-x   0        0        0     1569 2023-12-19 04:15:27.365826 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/__pycache__/retrieve.cpython-311.pyc
--rwxr-xr-x   0        0        0     1764 2024-04-04 18:31:50.349295 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/__pycache__/structure_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2850 2023-12-19 04:15:27.362825 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/__pycache__/structure_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      764 2024-04-04 18:30:31.938755 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py
--rwxr-xr-x   0        0        0      448 2024-04-04 18:32:49.240261 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/crypto.S.HTML
--rwxr-xr-x   0        0        0      980 2024-03-17 20:48:31.394211 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py
--rwxr-xr-x   0        0        0     1764 2024-04-04 18:31:47.681343 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py
--rwxr-xr-x   0        0        0       83 2024-04-04 20:04:06.732691 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/options/options.S.HTML
--rwxr-xr-x   0        0        0      390 2024-03-22 18:49:35.640871 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_one.py
--rwxr-xr-x   0        0        0      982 2024-03-22 18:48:12.109972 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py
--rwxr-xr-x   0        0        0      107 2024-03-17 18:08:13.242881 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Bybit/Bybit.S.HTML
--rwxr-xr-x   0        0        0      174 2024-03-18 17:15:52.070050 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/CCXT.s.HTML
--rwxr-xr-x   0        0        0     1039 2024-02-28 18:15:51.229428 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py
--rwxr-xr-x   0        0        0        4 2024-02-15 22:17:12.783549 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.202558 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2210 2024-01-03 02:13:34.497200 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__pycache__/candles.cpython-311.pyc
--rwxr-xr-x   0        0        0     1594 2024-02-28 18:15:51.249428 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py
--rwxr-xr-x   0        0        0        4 2024-02-15 22:17:12.843548 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.242558 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML
--rwxr-xr-x   0        0        0     2513 2024-02-28 18:15:51.265428 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py
--rwxr-xr-x   0        0        0     2371 2024-01-06 05:51:10.856125 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML
--rwxr-xr-x   0        0        0        3 2023-12-28 22:53:18.327445 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/__init__.py
--rwxr-xr-x   0        0        0      221 2024-03-18 17:17:05.853679 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      242 2023-12-31 03:44:11.213732 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0       62 2023-12-28 22:54:25.050671 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/coinbase/coinbase.s.HTML
--rwxr-xr-x   0        0        0      640 2024-03-18 17:17:05.853679 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/symbols/__pycache__/array.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-01-05 04:24:31.370747 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/symbols/__pycache__/array.cpython-311.pyc
--rwxr-xr-x   0        0        0      362 2024-02-28 18:15:51.285428 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/symbols/array.py
--rwxr-xr-x   0        0        0      331 2024-04-05 17:46:08.984778 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Clouds Crypto.S.HTML
--rwxr-xr-x   0        0        0     1030 2024-04-09 00:30:02.259836 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML
--rwxr-xr-x   0        0        0      597 2024-03-31 19:49:32.345940 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Clouds.S.HTML
--rwxr-xr-x   0        0        0     2726 2024-02-28 18:15:51.305427 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py
--rwxr-xr-x   0        0        0        4 2024-02-15 22:17:12.943547 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.310557 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3378 2024-01-05 23:56:15.810515 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/__pycache__/build_JWT.cpython-311.pyc
--rwxr-xr-x   0        0        0      717 2024-02-28 18:15:51.321427 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py
--rwxr-xr-x   0        0        0     1256 2024-01-05 03:42:55.233275 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2042 2024-02-28 18:15:51.341427 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py
--rwxr-xr-x   0        0        0     1798 2024-01-06 03:51:56.607140 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/orders/__pycache__/order_IDs.cpython-311.pyc
--rwxr-xr-x   0        0        0     1260 2024-02-28 18:15:51.361427 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py
--rwxr-xr-x   0        0        0        4 2024-02-15 22:17:13.067546 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/products/__pycache__/candles.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.378557 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/products/__pycache__/candles.cpython-311.pyc
--rwxr-xr-x   0        0        0     3281 2024-02-28 18:15:51.381427 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py
--rwxr-xr-x   0        0        0      978 2024-02-28 18:15:51.397426 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py
--rwxr-xr-x   0        0        0      699 2024-02-28 18:15:51.417426 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML
--rwxr-xr-x   0        0        0     1573 2024-01-05 02:24:04.987422 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/orders/__pycache__/place.cpython-311.pyc
--rwxr-xr-x   0        0        0     1543 2024-02-28 18:15:51.437426 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py
--rwxr-xr-x   0        0        0      614 2023-11-25 04:03:55.921174 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML
--rwxr-xr-x   0        0        0        0 2024-03-17 22:41:32.234375 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Finnhub/Finnhub.S.HTML
--rwxr-xr-x   0        0        0       47 2024-03-24 04:04:49.775241 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Finviz.com/Finviz.com.S.HTML
--rwxr-xr-x   0        0        0      193 2023-11-25 19:05:12.524729 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/LedgerX/LedgerX.s.HTML
--rwxr-xr-x   0        0        0       10 2023-12-12 05:12:16.566568 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/MQL5/MQL5.s.HTML
--rwxr-xr-x   0        0        0      226 2023-11-20 05:36:28.995516 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Robinhood/Robinhood.s.HTML
--rwxr-xr-x   0        0        0       80 2024-03-17 22:16:54.374127 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tiingo/Tiingo.S.HTML
--rwxr-xr-x   0        0        0      129 2024-03-31 18:42:05.191819 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/Tradier.s.HTML
--rwxr-xr-x   0        0        0      534 2024-04-04 18:44:17.394615 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py
--rwxr-xr-x   0        0        0       36 2024-04-04 19:14:12.097804 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/__init__.py
--rwxr-xr-x   0        0        0      122 2024-04-04 19:13:46.242103 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/exchanges.S.HTML
--rwxr-xr-x   0        0        0     2253 2023-10-12 00:49:49.793232 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1737 2024-04-04 19:00:57.079626 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/__pycache__/combine.cpython-310.pyc
--rwxr-xr-x   0        0        0     2438 2023-12-19 04:09:04.643687 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/__pycache__/combine.cpython-311.pyc
--rwxr-xr-x   0        0        0     1351 2024-04-04 19:00:55.635642 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py
--rwxr-xr-x   0        0        0   220164 2023-11-21 17:07:07.643477 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON
--rwxr-xr-x   0        0        0      212 2023-10-19 20:16:35.898645 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/uo_tradier_api.s.HTML
--rwxr-xr-x   0        0        0     1134 2024-04-04 19:45:42.235028 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py
--rwxr-xr-x   0        0        0     1350 2024-04-04 19:45:44.039013 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1234 2024-04-04 19:24:22.482995 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py
--rwxr-xr-x   0        0        0     1151 2023-10-12 00:26:56.418921 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__pycache__/PARSE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1427 2024-04-04 19:32:27.285751 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1857 2023-12-19 04:09:04.649687 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      963 2024-04-04 20:05:06.540108 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__pycache__/parse_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1189 2023-11-16 22:27:55.629712 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__pycache__/parse_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1769 2024-04-04 20:05:04.392129 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py
--rwxr-xr-x   0        0        0      634 2024-02-28 18:15:51.513425 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py
--rwxr-xr-x   0        0        0      876 2024-03-31 18:50:23.775072 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1179 2023-12-19 04:09:04.647687 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      216 2024-03-18 04:26:59.460093 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/TV.s.HTML
--rw-r--r--   0        0        0       80 2024-04-08 21:18:57.873149 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/fluctuators/fluctuators.S.HTML
--rwxr-xr-x   0        0        0      300 2023-12-12 05:03:24.406023 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/sensors/__init__.py
--rwxr-xr-x   0        0        0      237 2024-03-22 19:42:45.277679 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/sensors/sensors.S.HTML
--rwxr-xr-x   0        0        0     3458 2024-03-17 05:35:01.529000 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine
--rwxr-xr-x   0        0        0      163 2024-03-17 05:34:46.185162 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/indicators.S.HTML
--rwxr-xr-x   0        0        0     3836 2024-03-24 04:00:45.321327 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py
--rwxr-xr-x   0        0        0     2991 2024-03-31 19:18:13.894470 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1514 2024-03-31 20:03:17.529323 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py
--rwxr-xr-x   0        0        0     1990 2024-03-31 20:03:27.649271 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      952 2024-03-22 19:48:18.298003 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/__pycache__/print_symbols_table.cpython-310.pyc
--rwxr-xr-x   0        0        0     1630 2024-03-22 19:48:18.298003 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/__pycache__/scan_symbol.cpython-310.pyc
--rwxr-xr-x   0        0        0      813 2024-03-22 19:47:25.962582 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
--rwxr-xr-x   0        0        0     1829 2024-03-22 19:46:48.770994 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
--rwxr-xr-x   0        0        0      495 2024-03-28 00:15:40.797119 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/IRS/IRA/IRA.S.HTML
--rwxr-xr-x   0        0        0      410 2024-03-27 18:27:21.899277 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/IRS/taxes/income/__init__.py
--rwxr-xr-x   0        0        0       60 2023-11-10 17:23:06.947404 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/6K/__init__.py
--rwxr-xr-x   0        0        0      496 2023-11-10 17:40:32.497079 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/__init__.py
--rwxr-xr-x   0        0        0       18 2023-11-10 17:15:04.345938 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/balance_sheets.s.HTML
--rwxr-xr-x   0        0        0      198 2023-11-10 17:28:03.521299 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/equity/__init__.py
--rwxr-xr-x   0        0        0      420 2023-11-10 17:53:32.039501 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/income/__init__.py
--rwxr-xr-x   0        0        0       51 2023-11-10 17:34:28.536151 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/income/income.s.HTML
--rwxr-xr-x   0        0        0        0 2023-11-09 20:40:55.437403 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/USA/SEC/statements.s.HTML
--rwxr-xr-x   0        0        0      212 2023-11-14 04:12:06.841989 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/Yahoo.s.HTML
--rwxr-xr-x   0        0        0     1370 2024-03-18 19:45:48.829834 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/__pycache__/retrieve.cpython-310.pyc
--rwxr-xr-x   0        0        0     1252 2024-03-22 19:39:29.131830 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/__pycache__/retrieve_change.cpython-310.pyc
--rwxr-xr-x   0        0        0     1824 2024-03-18 19:45:43.465891 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py
--rwxr-xr-x   0        0        0      934 2024-03-22 19:39:27.891844 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py
--rwxr-xr-x   0        0        0       32 2023-11-14 05:19:00.214473 rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/twelve_data/twelve_data.s.HTML
--rwxr-xr-x   0        0        0       16 2024-03-24 03:14:51.054648 rollercoaster-2.1.3/venues/stages/rollercoaster/emojis.MD
--rwxr-xr-x   0        0        0     2589 2023-11-14 05:42:13.790956 rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/bt/strategies/example_1.py
--rwxr-xr-x   0        0        0      130 2024-04-08 20:48:05.178188 rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/fluctuators - itinerary.s.HTML
--rwxr-xr-x   0        0        0      787 2024-04-08 20:48:43.589745 rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/fluctuators.S.HTML
--rwxr-xr-x   0        0        0      121 2023-11-28 03:26:29.420655 rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/lumi/lumi.s.HTML
--rwxr-xr-x   0        0        0      100 2023-12-19 04:49:40.656260 rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/rover_1/rover_1.s.HTML
--rwxr-xr-x   0        0        0      687 2023-11-09 17:06:20.957059 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/__pycache__/RATIO.cpython-311.pyc
--rwxr-xr-x   0        0        0      514 2024-02-28 18:16:05.705262 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/__pycache__/ratio.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.518556 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/__pycache__/ratio.cpython-311.pyc
--rwxr-xr-x   0        0        0      446 2024-02-28 18:15:51.581424 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/clock/UTC/ISO.py
--rw-r--r--   0        0        0      555 2024-04-09 02:17:45.162628 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/clock/UTC/__pycache__/current.cpython-310.pyc
--rw-r--r--   0        0        0      352 2024-04-09 02:17:43.626646 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/clock/UTC/current.py
--rwxr-xr-x   0        0        0      984 2024-02-28 18:15:51.565425 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py
--rwxr-xr-x   0        0        0      288 2024-04-09 02:03:24.336835 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/clock/clock.s.HTML
--rwxr-xr-x   0        0        0      620 2023-11-09 20:46:40.432504 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/format_percentage.py
--rwxr-xr-x   0        0        0      151 2023-11-23 05:19:27.179399 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/math/slope/__init__.py
--rwxr-xr-x   0        0        0       79 2024-01-10 05:54:37.773115 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/DF.s.HTML
--rwxr-xr-x   0        0        0      517 2024-02-28 18:16:04.701273 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/__pycache__/from_list.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.566556 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/__pycache__/from_list.cpython-311.pyc
--rwxr-xr-x   0        0        0      477 2024-03-18 05:14:19.393182 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/__pycache__/to_list.cpython-310.pyc
--rwxr-xr-x   0        0        0      601 2024-01-06 05:10:56.564933 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/__pycache__/to_list.cpython-311.pyc
--rw-r--r--   0        0        0      796 2024-04-16 18:04:33.462601 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/_status/__pycache__/status_from_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      519 2024-02-28 18:15:51.653423 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py
--rwxr-xr-x   0        0        0      252 2024-02-28 18:15:51.673423 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/from_list.py
--rwxr-xr-x   0        0        0      326 2024-03-17 21:21:47.633007 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/to_list.py
--rwxr-xr-x   0        0        0      690 2024-01-13 06:12:46.871796 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML
--rwxr-xr-x   0        0        0      402 2024-02-28 18:15:51.689423 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/ratio.py
--rwxr-xr-x   0        0        0      457 2024-02-28 18:15:51.709423 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/__init__.py
--rwxr-xr-x   0        0        0      768 2024-02-28 18:16:04.685273 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.650555 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      709 2024-04-16 18:04:33.438601 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      377 2024-02-28 18:15:51.761422 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/status_1.py
--rwxr-xr-x   0        0        0    18282 2023-12-28 23:17:20.176165 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/summation.svg
--rwxr-xr-x   0        0        0      100 2024-04-09 02:03:10.212995 rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/tools.s.HTML
--rwxr-xr-x   0        0        0     2102 2024-04-04 20:32:10.597520 rollercoaster-2.1.3/venues/stages/rollercoaster/home.MD
--rwxr-xr-x   0        0        0     1081 2024-04-09 00:01:58.996000 rollercoaster-2.1.3/venues/stages/rollercoaster/home.s.HTML
--rw-r--r--   0        0        0      425 2024-04-09 02:33:16.647876 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/rides - formats.S.HTML
--rw-r--r--   0        0        0      319 2024-04-08 17:38:46.213186 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/rides - itinerary.S.HTML
--rwxr-xr-x   0        0        0     1334 2024-04-08 20:50:23.708590 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/rides.S.HTML
--rwxr-xr-x   0        0        0      489 2023-12-31 05:03:05.192136 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/ATR.s.HTML
--rwxr-xr-x   0        0        0     2944 2024-03-18 04:08:14.882175 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
--rwxr-xr-x   0        0        0     1591 2024-03-18 04:08:14.838176 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py
--rwxr-xr-x   0        0        0     1192 2024-03-18 05:14:19.113184 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.902554 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1191 2024-04-16 18:04:33.610599 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1242 2024-03-18 04:08:14.866176 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py
--rwxr-xr-x   0        0        0     1731 2024-01-02 03:23:31.042432 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/AO.pine
--rwxr-xr-x   0        0        0      134 2023-12-01 02:49:14.211328 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/Andean.r.HTML
--rwxr-xr-x   0        0        0      273 2023-12-31 06:36:06.223233 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/EMA/EMA.s.HTML
--rwxr-xr-x   0        0        0       82 2023-11-14 05:05:08.114737 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/EMA/__init__.py
--rwxr-xr-x   0        0        0     4821 2024-01-02 03:23:31.085431 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/HHLL/indicator.pine
--rwxr-xr-x   0        0        0       72 2023-12-03 22:10:44.686991 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/MA/MA.r.HTML
--rwxr-xr-x   0        0        0       91 2023-12-12 04:16:31.428608 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/MACD/MACD.s.HTML
--rwxr-xr-x   0        0        0       48 2023-12-02 00:37:47.807470 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/QQE/QQE.r.HTML
--rwxr-xr-x   0        0        0      201 2023-12-03 02:58:48.769709 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/RSI/RSI.r.HTML
--rwxr-xr-x   0        0        0      782 2024-03-18 04:08:14.894175 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.970554 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/RSI/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      250 2024-01-02 06:36:59.547427 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/SMA/__init__.py
--rwxr-xr-x   0        0        0      397 2024-01-02 03:23:31.177430 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/TR.s.HTML
--rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/True Range.svg
--rwxr-xr-x   0        0        0     1628 2024-03-18 04:08:14.978174 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/__init__.py
--rwxr-xr-x   0        0        0      778 2024-03-18 05:14:18.929185 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.066553 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      749 2024-04-16 18:04:33.578600 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      921 2024-04-16 18:04:33.466601 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/_status/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      523 2024-03-18 04:08:14.994174 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py
--rwxr-xr-x   0        0        0      792 2024-03-18 04:08:15.006173 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py
--rwxr-xr-x   0        0        0      254 2023-11-29 18:25:15.058846 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TV.r.HTML
--rwxr-xr-x   0        0        0       46 2023-11-21 16:46:45.097491 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/VWAP/VWAP.r.HTML
--rwxr-xr-x   0        0        0      593 2024-03-18 04:08:15.014173 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.030173 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/VWAP/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0       47 2023-11-21 16:46:17.697805 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/VWMA/VWMA.r.HTML
--rwxr-xr-x   0        0        0       24 2023-11-14 04:28:20.239207 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/bolinger_bands/bolinger_bands.r.html
--rwxr-xr-x   0        0        0        0 2023-11-30 18:13:51.268620 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/chandlier_exit/chandelier exit.r.HTML
--rwxr-xr-x   0        0        0      546 2024-02-28 18:15:52.105418 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML
--rwxr-xr-x   0        0        0     1266 2024-01-02 03:23:31.097431 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML
--rwxr-xr-x   0        0        0       28 2023-11-21 16:43:07.835981 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/relative_volume/relative volume.r.HTML
--rwxr-xr-x   0        0        0     2832 2024-03-18 04:08:14.950174 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:14.966174 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1098 2024-03-18 04:08:14.910175 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py
--rwxr-xr-x   0        0        0     1103 2024-03-18 05:14:19.101184 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.010553 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1213 2024-04-16 18:04:33.638599 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1243 2024-03-18 04:08:14.942175 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py
--rwxr-xr-x   0        0        0      358 2024-01-06 00:03:10.850549 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/pandas_ta/__init__.py
--rwxr-xr-x   0        0        0      225 2023-12-03 02:59:17.552392 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/supertrend.s.HTML
--rwxr-xr-x   0        0        0        0 2024-01-02 03:30:08.272935 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend2/__init__.py
--rwxr-xr-x   0        0        0     1215 2024-03-18 04:08:15.046173 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py
--rwxr-xr-x   0        0        0     1169 2024-03-18 05:14:19.105183 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.134553 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1185 2024-04-16 18:04:33.418602 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1230 2024-03-18 04:08:15.066173 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py
--rwxr-xr-x   0        0        0      334 2024-01-06 07:25:23.819962 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/AS.s.HTML
--rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/AS.svg
--rwxr-xr-x   0        0        0     1544 2024-03-18 04:08:15.074173 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/__init__.py
--rwxr-xr-x   0        0        0      741 2024-03-18 05:14:18.901185 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.174553 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      743 2024-04-16 18:04:33.414602 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      916 2024-04-16 18:04:33.442601 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/_status/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      511 2024-03-18 04:08:15.094172 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/_status/status_1.py
--rwxr-xr-x   0        0        0      783 2024-03-18 04:08:15.106172 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py
--rwxr-xr-x   0        0        0     1093 2024-01-06 07:15:37.995569 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py
--rwxr-xr-x   0        0        0     1350 2024-03-18 04:08:15.118172 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.130172 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/pecdency/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     4116 2024-03-18 04:08:15.278170 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/ST/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.294169 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/ST/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      433 2024-03-18 04:08:15.362168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/VDA/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.370168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/VDA/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-03-18 04:08:15.382168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.394168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/VSA/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      334 2024-01-09 01:54:38.423714 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/AS.s.HTML
--rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/AS.svg
--rwxr-xr-x   0        0        0     1557 2024-03-18 04:08:15.146171 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py
--rwxr-xr-x   0        0        0      747 2024-03-18 05:14:18.877185 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.242552 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      775 2024-04-16 18:04:33.450601 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      959 2024-04-16 18:04:33.458601 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/_status/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      522 2024-03-18 04:08:15.166171 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py
--rwxr-xr-x   0        0        0      790 2024-03-18 04:08:15.178171 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py
--rwxr-xr-x   0        0        0     1183 2024-03-18 04:08:15.190171 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py
--rwxr-xr-x   0        0        0     1202 2024-03-18 05:14:18.953184 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.294552 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1239 2024-04-16 18:04:33.462601 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1248 2024-03-18 04:08:15.210171 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py
--rwxr-xr-x   0        0        0     3688 2024-03-18 04:08:15.222170 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.238170 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3586 2024-03-18 04:08:15.250170 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.270170 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3862 2024-03-18 04:08:15.306169 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.386552 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.410551 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/__pycache__/shares_trading.cpython-311.pyc
--rwxr-xr-x   0        0        0     1759 2024-03-18 04:08:15.322169 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py
--rwxr-xr-x   0        0        0      961 2024-03-18 04:08:15.334169 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-18 04:08:15.346169 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/supertrend/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1825 2024-03-18 04:08:15.406168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/AO/__init__.py
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.494551 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/AO/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5968 2024-04-11 03:49:19.489710 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/KernelFunctions.ps
--rw-r--r--   0        0        0    36151 2024-04-11 03:49:38.505474 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps
--rw-r--r--   0        0        0    18799 2024-04-11 03:48:20.246452 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/MLExtensions.ps
--rwxr-xr-x   0        0        0     3926 2024-03-18 04:08:15.418168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/__init__.py
--rwxr-xr-x   0        0        0        4 2024-02-15 22:17:14.703527 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.530551 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0       13 2024-02-01 15:34:15.615610 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/superb.s.HTML
--rwxr-xr-x   0        0        0        4 2024-02-15 22:17:14.739527 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/win_rates/__pycache__/shares_trading.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:19.554551 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/win_rates/__pycache__/shares_trading.cpython-311.pyc
--rwxr-xr-x   0        0        0     1786 2024-03-18 04:08:15.430168 rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py
--rwxr-xr-x   0        0        0      800 2024-04-04 18:22:28.656860 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     4000 2024-04-04 17:03:41.281223 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/ETF.py
--rwxr-xr-x   0        0        0        2 2024-04-04 18:06:03.015402 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/REIT.py
--rwxr-xr-x   0        0        0     2162 2024-04-04 18:22:34.680804 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/TV.py
--rwxr-xr-x   0        0        0     3279 2024-04-04 17:04:11.753289 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/__pycache__/ETF.cpython-310.pyc
--rwxr-xr-x   0        0        0     2374 2024-04-04 18:22:36.056791 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/__pycache__/TV.cpython-310.pyc
--rwxr-xr-x   0        0        0     1871 2024-04-04 17:36:53.704312 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/__pycache__/currency.cpython-310.pyc
--rwxr-xr-x   0        0        0     1411 2024-04-04 17:36:52.196339 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/currency.py
--rwxr-xr-x   0        0        0       42 2024-04-04 18:06:43.814870 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/penny_stocks.py
--rwxr-xr-x   0        0        0      415 2024-04-04 18:22:24.940895 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/clique.py
--rwxr-xr-x   0        0        0      180 2024-04-15 19:29:36.357014 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/screeners.S.HTML
--rwxr-xr-x   0        0        0      119 2024-03-31 19:49:32.365940 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/symbol/__init__.py
--rwxr-xr-x   0        0        0      941 2024-04-15 19:25:57.778780 rollercoaster-2.1.3/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML
--rw-r--r--   0        0        0       84 2024-04-08 20:53:48.054233 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/VHLOC/MACD/MACD.S.HTML
--rw-r--r--   0        0        0      105 2024-04-08 20:51:20.623934 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/VHLOC/MACD/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 20:53:19.026568 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/VHLOC/MACD/procedure.ps
--rwxr-xr-x   0        0        0     1675 2024-04-05 03:53:30.742814 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     5120 2024-04-04 18:12:45.242647 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py
--rwxr-xr-x   0        0        0     3118 2024-04-04 18:13:14.090339 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.842554 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1958 2024-03-31 19:02:25.517446 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML
--rw-r--r--   0        0        0      952 2024-04-16 18:04:33.554600 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1599 2024-04-16 18:04:33.614599 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/1.JSON
--rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/2.JSON
--rwxr-xr-x   0        0        0      593 2024-02-28 18:15:51.993420 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py
--rwxr-xr-x   0        0        0     1860 2024-02-28 18:15:52.009419 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py
--rwxr-xr-x   0        0        0     2905 2024-03-31 18:52:09.009522 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py
--rwxr-xr-x   0        0        0     1780 2024-03-31 18:52:44.509015 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.742555 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1398 2024-04-16 18:04:33.574600 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1082 2024-04-16 18:04:33.630599 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     2290 2023-12-04 02:47:32.197228 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/0.JSON
--rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/1.JSON
--rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/2.JSON
--rwxr-xr-x   0        0        0     1508 2024-02-28 18:15:51.849421 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py
--rwxr-xr-x   0        0        0      794 2024-02-28 18:15:51.869421 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py
--rwxr-xr-x   0        0        0     1000 2024-04-05 04:05:45.569767 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML
--rwxr-xr-x   0        0        0        0 2024-03-31 19:07:37.005708 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/clique.py
--rwxr-xr-x   0        0        0      892 2024-02-28 18:15:51.889421 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py
--rwxr-xr-x   0        0        0      988 2024-02-28 18:16:05.309266 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/show/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-02-07 17:33:18.806555 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/show/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1599 2024-03-31 18:39:18.393448 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML
--rwxr-xr-x   0        0        0     1427 2024-04-05 03:53:28.182846 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/clique.py
--rwxr-xr-x   0        0        0      311 2024-04-05 04:21:31.280203 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/option_priceyness/option_priceyness.S.HTML
--rwxr-xr-x   0        0        0      562 2024-04-05 04:33:13.144392 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/stats.s.HTML
--rwxr-xr-x   0        0        0      352 2024-04-05 04:38:34.656724 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/the_multiplier/__init__.py
--rwxr-xr-x   0        0        0      570 2024-04-05 04:37:33.069429 rollercoaster-2.1.3/venues/stages/rollercoaster/stats/the_multiplier/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      911 2024-03-17 21:11:40.987538 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML
--rw-r--r--   0        0        0       89 2024-04-08 22:27:54.205084 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/contracts/contracts.S.HTML
--rw-r--r--   0        0        0      339 2024-04-13 19:27:27.156565 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/crypto/L1/L1.S.HTML
--rw-r--r--   0        0        0      725 2024-04-13 19:19:01.872575 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/crypto/crypto.S.HTML
--rw-r--r--   0        0        0       61 2024-04-13 19:26:04.032669 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/crypto/crypto_rust.S.HTML
--rw-r--r--   0        0        0      641 2024-04-13 19:19:32.260629 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/crypto/crypto_usual_features.S.HTML
--rwxr-xr-x   0        0        0       29 2023-11-21 17:46:09.752570 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/forex/forex.s.HTML
--rwxr-xr-x   0        0        0       75 2024-01-30 00:33:10.380046 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/futures/futures.s.HTML
--rw-r--r--   0        0        0      177 2024-04-16 18:07:20.864815 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/gems/gems.S.HTML
--rw-r--r--   0        0        0       48 2024-04-08 17:11:40.338334 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/greeks/greeks.S.HTML
--rwxr-xr-x   0        0        0     1565 2024-02-28 18:15:52.809410 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py
--rwxr-xr-x   0        0        0     1366 2023-11-23 04:51:27.721538 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/movement_calculator/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1167 2023-11-23 05:20:06.387999 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML
--rwxr-xr-x   0        0        0     2572 2024-04-05 05:24:21.970535 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/multipliers/__init__.py
--rwxr-xr-x   0        0        0     2148 2024-04-05 05:24:24.374510 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/multipliers/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      358 2024-04-08 17:12:06.086114 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/options.s.HTML
--rwxr-xr-x   0        0        0     1498 2024-02-28 18:15:52.809410 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py
--rwxr-xr-x   0        0        0     1299 2024-04-04 18:49:27.431033 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2548 2023-12-19 04:10:22.041108 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      489 2023-11-21 17:09:02.275163 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/shapes/shape_1/shape_1.s.HTML
--rw-r--r--   0        0        0      147 2024-04-08 21:43:35.583640 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/__init__.py
--rw-r--r--   0        0        0      156 2024-04-08 23:27:06.857428 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/loans.S.HTML
--rw-r--r--   0        0        0      431 2024-04-08 21:38:29.659326 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/constant.py
--rw-r--r--   0        0        0       95 2024-04-08 21:54:20.848024 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/insurance/insurance.S.HTML
--rw-r--r--   0        0        0      587 2024-04-08 22:05:05.892491 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML
--rw-r--r--   0        0        0     1202 2024-04-08 22:40:59.788117 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan.S.HTML
--rw-r--r--   0        0        0     1463 2024-04-09 00:50:23.861466 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/sources/sources.S.HTML
--rwxr-xr-x   0        0        0      414 2024-04-08 22:42:58.322845 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/real_estate.S.HTML
--rw-r--r--   0        0        0      437 2024-04-08 21:43:11.491928 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/sends.S.HTML
--rw-r--r--   0        0        0      127 2024-04-08 21:37:42.099907 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/tax/__init__.py
--rw-r--r--   0        0        0       97 2024-04-08 21:48:11.608365 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/tax/tax.S.HTML
--rw-r--r--   0        0        0     2434 2024-04-08 22:08:51.961985 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/varieties/varieties.S.HTML
--rwxr-xr-x   0        0        0     1190 2024-03-31 19:49:32.365940 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML
--rwxr-xr-x   0        0        0      114 2023-11-15 06:29:25.238807 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/comprehensive/comprehensive.s.HTML
--rwxr-xr-x   0        0        0       42 2023-11-15 06:37:06.461104 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/sectors/airlines/airlines.r.HTML
--rwxr-xr-x   0        0        0       45 2023-11-15 06:38:49.083268 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/sectors/electronics/semiconductors.r.HTML
--rwxr-xr-x   0        0        0       81 2023-11-15 06:34:55.671168 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/sectors/farming/farming.r.HTML
--rwxr-xr-x   0        0        0       84 2023-11-15 06:37:33.924880 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/sectors/real estate/real estate.r.HTML
--rwxr-xr-x   0        0        0      157 2024-03-17 04:50:30.861349 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/sectors/sectors.S.HTML
--rwxr-xr-x   0        0        0       14 2023-11-15 06:36:56.273187 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/sectors/vehicles/vehicles.r.HTML
--rwxr-xr-x   0        0        0        7 2024-03-24 04:01:12.905095 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/__init__.py
--rwxr-xr-x   0        0        0       13 2023-11-15 06:11:36.293215 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/companies/companies.s.HTML
--rwxr-xr-x   0        0        0       11 2023-11-21 16:53:15.238020 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/__init__.py
--rwxr-xr-x   0        0        0      135 2023-11-21 16:52:53.862265 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/shape_1.s.HTML
--rwxr-xr-x   0        0        0      106 2024-04-08 19:07:13.173774 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/shares.s.HTML
--rwxr-xr-x   0        0        0       43 2023-11-17 19:16:25.824071 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/splits.s.HTML
--rwxr-xr-x   0        0        0       90 2024-04-08 19:06:53.069998 rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/treasures.s.HTML
--rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 rollercoaster-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1654 2024-05-04 03:01:39.540494 rollercoaster-2.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0     2102 2024-04-04 23:37:49.640824 rollercoaster-2.1.4/readme.md
+-rwxr-xr-x   0        0        0      956 2024-05-04 03:05:41.090270 rollercoaster-2.1.4/venue.S.HTML
+-rw-r--r--   0        0        0       74 2024-04-08 20:59:40.730227 rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/itinerary - aspirations.S.HTML
+-rwxr-xr-x   0        0        0      825 2024-05-04 03:01:40.080489 rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      574 2024-04-08 21:03:27.655704 rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/sequentials/sequentials.S.HTML
+-rwxr-xr-x   0        0        0    51873 2024-03-17 02:26:50.689331 rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/sporatic/TradingView Screen.png
+-rwxr-xr-x   0        0        0      381 2024-03-31 19:05:52.370949 rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/sporatic/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      225 2024-04-09 02:15:48.675989 rollercoaster-2.1.4/venues/stages/rollercoaster/__data_nodes/moon/clique.py
+-rwxr-xr-x   0        0        0   845985 2024-04-05 04:00:12.449831 rollercoaster-2.1.4/venues/stages/rollercoaster/__data_nodes/moon/listing_status.csv
+-rwxr-xr-x   0        0        0      508 2024-05-04 03:01:39.960490 rollercoaster-2.1.4/venues/stages/rollercoaster/__data_nodes/moon/mongo.S.HTML
+-rwxr-xr-x   0        0        0      384 2024-05-04 03:01:40.148488 rollercoaster-2.1.4/venues/stages/rollercoaster/__glossary/rollercoaster_1
+-rwxr-xr-x   0        0        0       45 2024-04-04 18:35:08.441995 rollercoaster-2.1.4/venues/stages/rollercoaster/__init__.py
+-rwxr-xr-x   0        0        0     1960 2024-05-04 03:01:40.132488 rollercoaster-2.1.4/venues/stages/rollercoaster/_interfaces/clique/__init__.py
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 rollercoaster-2.1.4/venues/stages/rollercoaster/_interfaces/clique/group/__init__.py
+-rwxr-xr-x   0        0        0       53 2024-03-31 19:15:22.692288 rollercoaster-2.1.4/venues/stages/rollercoaster/_interfaces/sanic_trails/strails.S.HTML
+-rwxr-xr-x   0        0        0   234954 2024-05-04 03:04:33.266896 rollercoaster-2.1.4/venues/stages/rollercoaster/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1314 2024-04-17 00:35:43.012056 rollercoaster-2.1.4/venues/stages/rollercoaster/_status/clouds_status.proc.py
+-rwxr-xr-x   0        0        0     1193 2024-04-17 00:35:40.616088 rollercoaster-2.1.4/venues/stages/rollercoaster/_status/status.proc.py
+-rwxr-xr-x   0        0        0      114 2024-03-17 06:14:54.911123 rollercoaster-2.1.4/venues/stages/rollercoaster/_status/status_1.py
+-rw-r--r--   0        0        0       53 2024-04-26 00:14:43.452870 rollercoaster-2.1.4/venues/stages/rollercoaster/adventures/adventures.S.HTML
+-rw-r--r--   0        0        0      568 2024-04-26 01:07:20.514284 rollercoaster-2.1.4/venues/stages/rollercoaster/adventures/meter/meter.S.HTML
+-rwxr-xr-x   0        0        0      129 2024-01-26 16:01:45.729782 rollercoaster-2.1.4/venues/stages/rollercoaster/charts/charts.s.HTML
+-rwxr-xr-x   0        0        0      821 2024-03-17 23:24:26.718972 rollercoaster-2.1.4/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML
+-rwxr-xr-x   0        0        0      661 2024-05-04 03:01:39.992490 rollercoaster-2.1.4/venues/stages/rollercoaster/climate/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-25 23:54:45.286945 rollercoaster-2.1.4/venues/stages/rollercoaster/climate/climate.S.HTML
+-rwxr-xr-x   0        0        0      170 2024-04-04 19:34:53.736179 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/AV/AV.s.HTML
+-rwxr-xr-x   0        0        0      276 2024-03-17 21:13:24.014422 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/Alpaca.s.HTML
+-rw-r--r--   0        0        0      160 2024-04-09 00:53:14.647459 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/_data_API/data.S.HTML
+-rw-r--r--   0        0        0      798 2024-05-04 03:01:40.212488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py
+-rwxr-xr-x   0        0        0      764 2024-05-04 03:01:40.216488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py
+-rwxr-xr-x   0        0        0      448 2024-05-04 03:01:40.216488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/crypto.S.HTML
+-rwxr-xr-x   0        0        0      980 2024-05-04 03:01:40.216488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py
+-rwxr-xr-x   0        0        0     1764 2024-05-04 03:01:40.212488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py
+-rwxr-xr-x   0        0        0       83 2024-04-04 20:04:06.732691 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/options/options.S.HTML
+-rwxr-xr-x   0        0        0      390 2024-03-22 18:49:35.640871 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_one.py
+-rwxr-xr-x   0        0        0      982 2024-05-04 03:01:40.208488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py
+-rwxr-xr-x   0        0        0      107 2024-03-17 18:08:13.242881 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Bybit/Bybit.S.HTML
+-rwxr-xr-x   0        0        0      174 2024-05-04 03:01:40.192488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/CCXT.s.HTML
+-rwxr-xr-x   0        0        0     1039 2024-05-04 03:01:40.188488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py
+-rwxr-xr-x   0        0        0     1594 2024-05-04 03:01:40.188488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py
+-rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML
+-rwxr-xr-x   0        0        0     2513 2024-05-04 03:01:40.188488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py
+-rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML
+-rwxr-xr-x   0        0        0        3 2023-12-28 22:53:18.327445 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/__init__.py
+-rwxr-xr-x   0        0        0       62 2023-12-28 22:54:25.050671 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/coinbase/coinbase.s.HTML
+-rwxr-xr-x   0        0        0      362 2024-05-04 03:01:40.196488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/symbols/array.py
+-rwxr-xr-x   0        0        0      331 2024-04-05 17:46:08.984778 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Clouds Crypto.S.HTML
+-rwxr-xr-x   0        0        0     1030 2024-05-04 03:01:40.228488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML
+-rwxr-xr-x   0        0        0      597 2024-03-31 19:49:32.345940 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Clouds.S.HTML
+-rwxr-xr-x   0        0        0     2726 2024-05-04 03:01:40.200488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py
+-rwxr-xr-x   0        0        0      717 2024-05-04 03:01:40.200488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py
+-rwxr-xr-x   0        0        0     2042 2024-05-04 03:01:40.204488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py
+-rwxr-xr-x   0        0        0     1260 2024-05-04 03:01:40.204488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py
+-rwxr-xr-x   0        0        0     3281 2024-05-04 03:01:40.200488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py
+-rwxr-xr-x   0        0        0      978 2024-05-04 03:01:40.200488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py
+-rwxr-xr-x   0        0        0      699 2024-05-04 03:01:40.208488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML
+-rwxr-xr-x   0        0        0     1543 2024-05-04 03:01:40.208488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py
+-rwxr-xr-x   0        0        0      614 2023-11-25 04:03:55.921174 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-17 22:41:32.234375 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Finnhub/Finnhub.S.HTML
+-rwxr-xr-x   0        0        0       47 2024-03-24 04:04:49.775241 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Finviz.com/Finviz.com.S.HTML
+-rwxr-xr-x   0        0        0      193 2023-11-25 19:05:12.524729 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/LedgerX/LedgerX.s.HTML
+-rwxr-xr-x   0        0        0       10 2023-12-12 05:12:16.566568 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/MQL5/MQL5.s.HTML
+-rwxr-xr-x   0        0        0      226 2023-11-20 05:36:28.995516 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Robinhood/Robinhood.s.HTML
+-rwxr-xr-x   0        0        0       80 2024-03-17 22:16:54.374127 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tiingo/Tiingo.S.HTML
+-rwxr-xr-x   0        0        0      129 2024-05-04 03:01:40.172488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/Tradier.s.HTML
+-rwxr-xr-x   0        0        0      534 2024-05-04 03:01:40.176488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py
+-rwxr-xr-x   0        0        0       36 2024-04-04 19:14:12.097804 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/__init__.py
+-rwxr-xr-x   0        0        0      122 2024-04-04 19:13:46.242103 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/exchanges.S.HTML
+-rwxr-xr-x   0        0        0     1351 2024-05-04 03:01:40.156488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py
+-rwxr-xr-x   0        0        0   220164 2023-11-21 17:07:07.643477 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON
+-rwxr-xr-x   0        0        0      212 2023-10-19 20:16:35.898645 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/uo_tradier_api.s.HTML
+-rwxr-xr-x   0        0        0     1134 2024-05-04 03:01:40.164488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py
+-rwxr-xr-x   0        0        0     1234 2024-05-04 03:01:40.168488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py
+-rwxr-xr-x   0        0        0     1769 2024-04-04 20:05:04.392129 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py
+-rwxr-xr-x   0        0        0      634 2024-05-04 03:01:40.168488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py
+-rwxr-xr-x   0        0        0      216 2024-03-18 04:26:59.460093 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/TV.s.HTML
+-rw-r--r--   0        0        0       80 2024-05-04 03:01:40.228488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/fluctuators/fluctuators.S.HTML
+-rwxr-xr-x   0        0        0      300 2023-12-12 05:03:24.406023 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/sensors/__init__.py
+-rwxr-xr-x   0        0        0      237 2024-03-22 19:42:45.277679 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/sensors/sensors.S.HTML
+-rwxr-xr-x   0        0        0     3458 2024-03-17 05:35:01.529000 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine
+-rwxr-xr-x   0        0        0      163 2024-03-17 05:34:46.185162 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/indicators.S.HTML
+-rwxr-xr-x   0        0        0     3836 2024-05-04 03:01:40.224487 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py
+-rwxr-xr-x   0        0        0     1514 2024-05-04 03:01:40.220487 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py
+-rwxr-xr-x   0        0        0      813 2024-03-22 19:47:25.962582 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
+-rwxr-xr-x   0        0        0     1829 2024-03-22 19:46:48.770994 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
+-rwxr-xr-x   0        0        0      495 2024-03-28 00:15:40.797119 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/IRS/IRA/IRA.S.HTML
+-rwxr-xr-x   0        0        0      410 2024-05-04 03:01:40.180488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/IRS/taxes/income/__init__.py
+-rwxr-xr-x   0        0        0       60 2023-11-10 17:23:06.947404 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/6K/__init__.py
+-rwxr-xr-x   0        0        0      496 2023-11-10 17:40:32.497079 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/__init__.py
+-rwxr-xr-x   0        0        0       18 2023-11-10 17:15:04.345938 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/balance_sheets.s.HTML
+-rwxr-xr-x   0        0        0      198 2023-11-10 17:28:03.521299 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/equity/__init__.py
+-rwxr-xr-x   0        0        0      420 2023-11-10 17:53:32.039501 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/income/__init__.py
+-rwxr-xr-x   0        0        0       51 2023-11-10 17:34:28.536151 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/income/income.s.HTML
+-rwxr-xr-x   0        0        0        0 2023-11-09 20:40:55.437403 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/USA/SEC/statements.s.HTML
+-rwxr-xr-x   0        0        0      212 2023-11-14 04:12:06.841989 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Yahoo/Yahoo.s.HTML
+-rwxr-xr-x   0        0        0     1824 2024-05-04 03:01:40.176488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py
+-rwxr-xr-x   0        0        0      934 2024-05-04 03:01:40.176488 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py
+-rwxr-xr-x   0        0        0       32 2023-11-14 05:19:00.214473 rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/twelve_data/twelve_data.s.HTML
+-rwxr-xr-x   0        0        0       16 2024-03-24 03:14:51.054648 rollercoaster-2.1.4/venues/stages/rollercoaster/emojis.MD
+-rwxr-xr-x   0        0        0     2589 2023-11-14 05:42:13.790956 rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/bt/strategies/example_1.py
+-rwxr-xr-x   0        0        0      130 2024-04-08 20:48:05.178188 rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/fluctuators - itinerary.s.HTML
+-rwxr-xr-x   0        0        0      787 2024-04-08 20:48:43.589745 rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/fluctuators.S.HTML
+-rwxr-xr-x   0        0        0      121 2023-11-28 03:26:29.420655 rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/lumi/lumi.s.HTML
+-rwxr-xr-x   0        0        0      100 2023-12-19 04:49:40.656260 rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/rover_1/rover_1.s.HTML
+-rwxr-xr-x   0        0        0      446 2024-05-04 03:01:40.004490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/clock/UTC/ISO.py
+-rw-r--r--   0        0        0      352 2024-05-04 03:01:40.008489 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/clock/UTC/current.py
+-rwxr-xr-x   0        0        0      984 2024-05-04 03:01:40.008489 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py
+-rwxr-xr-x   0        0        0      288 2024-04-09 02:03:24.336835 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/clock/clock.s.HTML
+-rwxr-xr-x   0        0        0      620 2023-11-09 20:46:40.432504 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/format_percentage.py
+-rwxr-xr-x   0        0        0      151 2023-11-23 05:19:27.179399 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/math/slope/__init__.py
+-rwxr-xr-x   0        0        0       79 2024-01-10 05:54:37.773115 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/DF/DF.s.HTML
+-rwxr-xr-x   0        0        0      519 2024-05-04 03:01:40.000490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py
+-rwxr-xr-x   0        0        0      252 2024-05-04 03:01:40.000490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/DF/from_list.py
+-rwxr-xr-x   0        0        0      326 2024-05-04 03:01:39.996490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/DF/to_list.py
+-rwxr-xr-x   0        0        0      690 2024-01-13 06:12:46.871796 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML
+-rwxr-xr-x   0        0        0      402 2024-05-04 03:01:40.004490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/ratio.py
+-rwxr-xr-x   0        0        0      457 2024-05-04 03:01:39.992490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/summation/__init__.py
+-rwxr-xr-x   0        0        0      377 2024-05-04 03:01:39.992490 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/summation/status_1.py
+-rwxr-xr-x   0        0        0    18282 2023-12-28 23:17:20.176165 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/summation/summation.svg
+-rwxr-xr-x   0        0        0      100 2024-04-09 02:03:10.212995 rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/tools.s.HTML
+-rwxr-xr-x   0        0        0     2102 2024-05-04 03:01:40.152488 rollercoaster-2.1.4/venues/stages/rollercoaster/home.MD
+-rwxr-xr-x   0        0        0     1081 2024-05-04 03:01:40.228488 rollercoaster-2.1.4/venues/stages/rollercoaster/home.s.HTML
+-rw-r--r--   0        0        0      305 2024-04-26 00:08:58.840689 rollercoaster-2.1.4/venues/stages/rollercoaster/platforms/accounts/accounts.S.HTML
+-rw-r--r--   0        0        0      142 2024-04-26 01:32:14.574003 rollercoaster-2.1.4/venues/stages/rollercoaster/platforms/biorecon/biorecon.S.HTML
+-rw-r--r--   0        0        0      503 2024-04-26 00:27:03.696837 rollercoaster-2.1.4/venues/stages/rollercoaster/platforms/platforms.S.HTML
+-rw-r--r--   0        0        0      425 2024-04-09 02:33:16.647876 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/rides - formats.S.HTML
+-rw-r--r--   0        0        0      115 2024-04-27 16:24:01.727436 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/rides - objectives possibilities.S.HTML
+-rw-r--r--   0        0        0      321 2024-04-27 16:19:46.237010 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/rides - objectives.S.HTML
+-rwxr-xr-x   0        0        0     1398 2024-04-27 16:19:53.860942 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/rides.S.HTML
+-rwxr-xr-x   0        0        0      489 2023-12-31 05:03:05.192136 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/ATR.s.HTML
+-rwxr-xr-x   0        0        0     2944 2024-05-04 03:01:40.072489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
+-rwxr-xr-x   0        0        0     1591 2024-05-04 03:01:40.072489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py
+-rwxr-xr-x   0        0        0     1242 2024-05-04 03:01:40.076489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py
+-rwxr-xr-x   0        0        0     1731 2024-01-02 03:23:31.042432 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/AO.pine
+-rwxr-xr-x   0        0        0      134 2023-12-01 02:49:14.211328 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/Andean.r.HTML
+-rwxr-xr-x   0        0        0      273 2023-12-31 06:36:06.223233 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/EMA/EMA.s.HTML
+-rwxr-xr-x   0        0        0       82 2023-11-14 05:05:08.114737 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/EMA/__init__.py
+-rwxr-xr-x   0        0        0     4821 2024-01-02 03:23:31.085431 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/HHLL/indicator.pine
+-rwxr-xr-x   0        0        0       72 2023-12-03 22:10:44.686991 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/MA/MA.r.HTML
+-rwxr-xr-x   0        0        0       91 2023-12-12 04:16:31.428608 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/MACD/MACD.s.HTML
+-rwxr-xr-x   0        0        0       48 2023-12-02 00:37:47.807470 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/QQE/QQE.r.HTML
+-rwxr-xr-x   0        0        0      201 2023-12-03 02:58:48.769709 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/RSI/RSI.r.HTML
+-rwxr-xr-x   0        0        0      782 2024-05-04 03:01:40.056489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py
+-rwxr-xr-x   0        0        0      250 2024-01-02 06:36:59.547427 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/SMA/__init__.py
+-rwxr-xr-x   0        0        0      397 2024-01-02 03:23:31.177430 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/TR.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/True Range.svg
+-rwxr-xr-x   0        0        0     1628 2024-05-04 03:01:40.060489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/__init__.py
+-rwxr-xr-x   0        0        0      523 2024-05-04 03:01:40.064489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py
+-rwxr-xr-x   0        0        0      792 2024-05-04 03:01:40.064489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py
+-rwxr-xr-x   0        0        0      254 2023-11-29 18:25:15.058846 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TV.r.HTML
+-rwxr-xr-x   0        0        0       46 2023-11-21 16:46:45.097491 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/VWAP/VWAP.r.HTML
+-rwxr-xr-x   0        0        0      593 2024-05-04 03:01:40.052489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py
+-rwxr-xr-x   0        0        0       47 2023-11-21 16:46:17.697805 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/VWMA/VWMA.r.HTML
+-rwxr-xr-x   0        0        0       24 2023-11-14 04:28:20.239207 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/bolinger_bands/bolinger_bands.r.html
+-rwxr-xr-x   0        0        0        0 2023-11-30 18:13:51.268620 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/chandlier_exit/chandelier exit.r.HTML
+-rwxr-xr-x   0        0        0      546 2024-05-04 03:01:40.048489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML
+-rwxr-xr-x   0        0        0     1266 2024-01-02 03:23:31.097431 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML
+-rwxr-xr-x   0        0        0       28 2023-11-21 16:43:07.835981 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/relative_volume/relative volume.r.HTML
+-rwxr-xr-x   0        0        0     2832 2024-05-04 03:01:40.068489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
+-rwxr-xr-x   0        0        0     1098 2024-05-04 03:01:40.064489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py
+-rwxr-xr-x   0        0        0     1243 2024-05-04 03:01:40.068489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py
+-rwxr-xr-x   0        0        0      358 2024-01-06 00:03:10.850549 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/pandas_ta/__init__.py
+-rwxr-xr-x   0        0        0      225 2023-12-03 02:59:17.552392 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/supertrend.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-01-02 03:30:08.272935 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend2/__init__.py
+-rwxr-xr-x   0        0        0     1215 2024-05-04 03:01:40.016489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py
+-rwxr-xr-x   0        0        0     1230 2024-05-04 03:01:40.020489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py
+-rwxr-xr-x   0        0        0      334 2024-01-06 07:25:23.819962 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/AS.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/AS.svg
+-rwxr-xr-x   0        0        0     1544 2024-05-04 03:01:40.008489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/__init__.py
+-rwxr-xr-x   0        0        0      511 2024-05-04 03:01:40.012489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/_status/status_1.py
+-rwxr-xr-x   0        0        0      783 2024-05-04 03:01:40.016489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py
+-rwxr-xr-x   0        0        0     1093 2024-01-06 07:15:37.995569 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py
+-rwxr-xr-x   0        0        0     1350 2024-05-04 03:01:40.016489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py
+-rwxr-xr-x   0        0        0     4116 2024-05-04 03:01:40.020489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/ST/__init__.py
+-rwxr-xr-x   0        0        0      433 2024-05-04 03:01:40.036489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/VDA/__init__.py
+-rwxr-xr-x   0        0        0      567 2024-05-04 03:01:40.028489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py
+-rwxr-xr-x   0        0        0      334 2024-01-09 01:54:38.423714 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/AS.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/AS.svg
+-rwxr-xr-x   0        0        0     1557 2024-05-04 03:01:40.032489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py
+-rwxr-xr-x   0        0        0      522 2024-05-04 03:01:40.032489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py
+-rwxr-xr-x   0        0        0      790 2024-05-04 03:01:40.036489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py
+-rwxr-xr-x   0        0        0     1183 2024-05-04 03:01:40.024489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py
+-rwxr-xr-x   0        0        0     1248 2024-05-04 03:01:40.024489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py
+-rwxr-xr-x   0        0        0     3688 2024-05-04 03:01:40.036489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py
+-rwxr-xr-x   0        0        0     3586 2024-05-04 03:01:40.024489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py
+-rwxr-xr-x   0        0        0     3862 2024-05-04 03:01:40.028489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py
+-rwxr-xr-x   0        0        0     1759 2024-05-04 03:01:40.028489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py
+-rwxr-xr-x   0        0        0      961 2024-05-04 03:01:40.024489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py
+-rwxr-xr-x   0        0        0     1825 2024-05-04 03:01:40.044489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/AO/__init__.py
+-rw-r--r--   0        0        0     5968 2024-04-11 03:49:19.489710 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/KernelFunctions.ps
+-rw-r--r--   0        0        0    36151 2024-04-11 03:49:38.505474 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps
+-rw-r--r--   0        0        0    18799 2024-04-11 03:48:20.246452 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/MLExtensions.ps
+-rwxr-xr-x   0        0        0     3926 2024-05-04 03:01:40.040489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/superb/__init__.py
+-rwxr-xr-x   0        0        0       13 2024-02-01 15:34:15.615610 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/superb/superb.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-05-04 03:01:40.044489 rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py
+-rwxr-xr-x   0        0        0     4000 2024-05-04 03:01:39.952490 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/ETF.py
+-rwxr-xr-x   0        0        0        2 2024-04-04 18:06:03.015402 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/REIT.py
+-rwxr-xr-x   0        0        0     2162 2024-05-04 03:01:39.956490 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/TV.py
+-rwxr-xr-x   0        0        0     1411 2024-05-04 03:01:39.956490 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/currency.py
+-rwxr-xr-x   0        0        0       42 2024-04-04 18:06:43.814870 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/penny_stocks.py
+-rwxr-xr-x   0        0        0      415 2024-05-04 03:01:39.956490 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/clique.py
+-rwxr-xr-x   0        0        0      180 2024-04-15 19:29:36.357014 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/screeners.S.HTML
+-rwxr-xr-x   0        0        0      119 2024-05-04 03:01:39.960490 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/symbol/__init__.py
+-rwxr-xr-x   0        0        0      941 2024-05-04 03:01:39.960490 rollercoaster-2.1.4/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML
+-rw-r--r--   0        0        0       84 2024-04-08 20:53:48.054233 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/VHLOC/MACD/MACD.S.HTML
+-rw-r--r--   0        0        0      105 2024-05-04 03:01:40.084489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/VHLOC/MACD/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:53:19.026568 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/VHLOC/MACD/procedure.ps
+-rwxr-xr-x   0        0        0     5120 2024-05-04 03:01:40.108489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py
+-rwxr-xr-x   0        0        0     1958 2024-05-04 03:01:40.124488 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML
+-rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/1.JSON
+-rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/2.JSON
+-rwxr-xr-x   0        0        0      593 2024-05-04 03:01:40.108489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py
+-rwxr-xr-x   0        0        0     1860 2024-05-04 03:01:40.124488 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py
+-rwxr-xr-x   0        0        0     2905 2024-05-04 03:01:40.088489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py
+-rwxr-xr-x   0        0        0     2290 2023-12-04 02:47:32.197228 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/0.JSON
+-rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/1.JSON
+-rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/2.JSON
+-rwxr-xr-x   0        0        0     1508 2024-05-04 03:01:40.092489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-05-04 03:01:40.104489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py
+-rwxr-xr-x   0        0        0     1000 2024-05-04 03:01:40.092489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-31 19:07:37.005708 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/clique.py
+-rwxr-xr-x   0        0        0      892 2024-05-04 03:01:40.088489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py
+-rwxr-xr-x   0        0        0     1599 2024-03-31 18:39:18.393448 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML
+-rwxr-xr-x   0        0        0     1427 2024-05-04 03:01:40.108489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/clique.py
+-rwxr-xr-x   0        0        0      311 2024-04-05 04:21:31.280203 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/option_priceyness/option_priceyness.S.HTML
+-rwxr-xr-x   0        0        0      562 2024-04-05 04:33:13.144392 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/stats.s.HTML
+-rwxr-xr-x   0        0        0      352 2024-05-04 03:01:40.084489 rollercoaster-2.1.4/venues/stages/rollercoaster/stats/the_multiplier/__init__.py
+-rwxr-xr-x   0        0        0      911 2024-03-17 21:11:40.987538 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML
+-rw-r--r--   0        0        0       89 2024-04-08 22:27:54.205084 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/contracts/contracts.S.HTML
+-rw-r--r--   0        0        0      339 2024-04-13 19:27:27.156565 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/crypto/L1/L1.S.HTML
+-rw-r--r--   0        0        0      725 2024-04-13 19:19:01.872575 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/crypto/crypto.S.HTML
+-rw-r--r--   0        0        0       61 2024-04-13 19:26:04.032669 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/crypto/crypto_rust.S.HTML
+-rw-r--r--   0        0        0      641 2024-04-13 19:19:32.260629 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/crypto/crypto_usual_features.S.HTML
+-rwxr-xr-x   0        0        0      127 2024-04-25 23:58:14.336246 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/forex/forex.s.HTML
+-rwxr-xr-x   0        0        0       75 2024-01-30 00:33:10.380046 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/futures/futures.s.HTML
+-rw-r--r--   0        0        0      186 2024-04-19 20:08:05.560255 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/gems/gems.S.HTML
+-rw-r--r--   0        0        0       48 2024-04-08 17:11:40.338334 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/greeks/greeks.S.HTML
+-rwxr-xr-x   0        0        0     1565 2024-05-04 03:01:39.948490 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py
+-rwxr-xr-x   0        0        0     1167 2023-11-23 05:20:06.387999 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML
+-rwxr-xr-x   0        0        0     2572 2024-05-04 03:01:39.944490 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/multipliers/__init__.py
+-rwxr-xr-x   0        0        0      358 2024-04-08 17:12:06.086114 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/options.s.HTML
+-rwxr-xr-x   0        0        0     1498 2024-05-04 03:01:39.948490 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py
+-rwxr-xr-x   0        0        0      489 2023-11-21 17:09:02.275163 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/shapes/shape_1/shape_1.s.HTML
+-rw-r--r--   0        0        0      147 2024-05-04 03:01:39.932490 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-08 23:27:06.857428 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/loans.S.HTML
+-rw-r--r--   0        0        0      431 2024-04-08 21:38:29.659326 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/constant.py
+-rw-r--r--   0        0        0       95 2024-04-08 21:54:20.848024 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/insurance/insurance.S.HTML
+-rw-r--r--   0        0        0      587 2024-04-08 22:05:05.892491 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML
+-rw-r--r--   0        0        0     1202 2024-04-08 22:40:59.788117 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan.S.HTML
+-rw-r--r--   0        0        0     1463 2024-04-09 00:50:23.861466 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/sources/sources.S.HTML
+-rwxr-xr-x   0        0        0      414 2024-04-08 22:42:58.322845 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/real_estate.S.HTML
+-rw-r--r--   0        0        0      437 2024-04-08 21:43:11.491928 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/sends.S.HTML
+-rw-r--r--   0        0        0      127 2024-04-08 21:37:42.099907 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/tax/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-08 21:48:11.608365 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/tax/tax.S.HTML
+-rw-r--r--   0        0        0     2434 2024-04-08 22:08:51.961985 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/varieties/varieties.S.HTML
+-rwxr-xr-x   0        0        0     1190 2024-03-31 19:49:32.365940 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML
+-rwxr-xr-x   0        0        0      114 2023-11-15 06:29:25.238807 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/comprehensive/comprehensive.s.HTML
+-rwxr-xr-x   0        0        0       42 2023-11-15 06:37:06.461104 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/sectors/airlines/airlines.r.HTML
+-rwxr-xr-x   0        0        0       45 2023-11-15 06:38:49.083268 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/sectors/electronics/semiconductors.r.HTML
+-rwxr-xr-x   0        0        0       81 2023-11-15 06:34:55.671168 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/sectors/farming/farming.r.HTML
+-rwxr-xr-x   0        0        0       84 2023-11-15 06:37:33.924880 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/sectors/real estate/real estate.r.HTML
+-rwxr-xr-x   0        0        0      157 2024-03-17 04:50:30.861349 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/sectors/sectors.S.HTML
+-rwxr-xr-x   0        0        0       14 2023-11-15 06:36:56.273187 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/sectors/vehicles/vehicles.r.HTML
+-rwxr-xr-x   0        0        0        7 2024-03-24 04:01:12.905095 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/__init__.py
+-rwxr-xr-x   0        0        0       13 2023-11-15 06:11:36.293215 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/companies/companies.s.HTML
+-rwxr-xr-x   0        0        0       11 2023-11-21 16:53:15.238020 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/__init__.py
+-rwxr-xr-x   0        0        0      135 2023-11-21 16:52:53.862265 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/shape_1.s.HTML
+-rwxr-xr-x   0        0        0      106 2024-04-08 19:07:13.173774 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/shares.s.HTML
+-rwxr-xr-x   0        0        0       43 2023-11-17 19:16:25.824071 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/splits.s.HTML
+-rwxr-xr-x   0        0        0       90 2024-04-08 19:06:53.069998 rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/treasures.s.HTML
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 rollercoaster-2.1.4/PKG-INFO
```

### Comparing `rollercoaster-2.1.3/pyproject.toml` & `rollercoaster-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "rollercoaster"
-version = "2.1.3"
+version = "2.1.4"
 description = "economic estimation"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "rollercoaster", from = "venues/stages" }
 ]
```

### Comparing `rollercoaster-2.1.3/readme.md` & `rollercoaster-2.1.4/readme.md`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/itinerary.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/itinerary.S.HTML`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 
 <pre>
 
 	<h1>itinerary</h1>
 
 	<h2>ranked</h2>
 			
+		[ ] screen by shareholder's equity percentage
+			change by quarter.
+			
+				example:
+					2023 Q4 to 2024 Q1
+					
+						2023_Q4: $120m	
+						2023_Q4: $100m
+						
+						6/5 -> 20%
+	
+			
 		[ ] multiplier (percentage change) for shares that
 			appear in the TV screener.
 		
 							percentage change
 			
 						[ 8 ] [ 9 ] [ 10 ] [ 11 ] [ 12 ]
 				HOOK	  -
```

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/sequentials/sequentials.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/sequentials/sequentials.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/___itinerary/sporatic/TradingView Screen.png` & `rollercoaster-2.1.4/venues/stages/rollercoaster/___objectives/sporatic/TradingView Screen.png`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/__data_nodes/moon/listing_status.csv` & `rollercoaster-2.1.4/venues/stages/rollercoaster/__data_nodes/moon/listing_status.csv`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/_interfaces/clique/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/_interfaces/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/_status/DB/records.json` & `rollercoaster-2.1.4/venues/stages/rollercoaster/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9838709677419355%*

 * *Differences: {"'_default'": "{'61': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'gadgets/summation/status_1.py'), ('empty', False), ('parsed', True), ('stats', "*

 * *               "OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('passed', True), ('elapsed', [8.8019999111566e-06, 'seconds'])])])]), "*

 * *               "OrderedDict([('path', 'gadgets/pandas/DF/_status/status_from_1.py'), ('empty', "*

 * *               "False), ('parsed', True), ('st […]*

```diff
@@ -12783,14 +12783,686 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 17
                 },
                 "empty": 0
             }
         },
+        "61": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.8019999111566e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "gadgets/summation/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0009608060001937702,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "gadgets/pandas/DF/_status/status_from_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07603745799997341,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_2/AS/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11834995699996398,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_2/AS/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11050606399999197,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_2/AAS/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12293967999994493,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_3/physical_span_average/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.08813717799989718,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_3/physical_span/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.06816510799990283,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_3/physical_span/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0689949269999488,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/TR/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.16434544200001255,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/TR/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.07338739400006489,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/supertrend/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11152192800000194,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/ATR/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00805113500018706,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_break_even/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14392969600021388,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_break_even/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.03556551499991656,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_PC_ratio/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0005473100000017439,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_PC_ratio/status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check",
+                            "elapsed": [
+                                7.099999947968172e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 17
+                },
+                "empty": 0
+            }
+        },
+        "62": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.73200042406097e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "gadgets/summation/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.022700809000525624,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "gadgets/pandas/DF/_status/status_from_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.05636936699738726,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_2/AS/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10686830900522182,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_2/AS/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.056904924000264145,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_2/AAS/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.12777939799707383,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_3/physical_span_average/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14810370300256182,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_3/physical_span/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.06514004400378326,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_3/physical_span/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.06381193499692017,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/TR/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.056332200998440385,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/TR/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.06557025700021768,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/supertrend/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.058570216002408415,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "rides/season_1/ATR/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.050430541996320244,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_break_even/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.17668099999718834,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_break_even/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.020171198004391044,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_PC_ratio/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00035332900006324053,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "stats/aggregate_PC_ratio/status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check",
+                            "elapsed": [
+                                7.679991540499032e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 17
+                },
+                "empty": 0
+            }
+        },
         "7": {
             "alarms": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
                             "exception": "ModuleNotFoundError(\"No module named 'propinquity'\")",
```

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/_status/clouds_status.proc.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/_status/clouds_status.proc.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/_status/status.proc.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/climate/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Clouds.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Clouds.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/bt/strategies/example_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/bt/strategies/example_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/fluctuators/fluctuators.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/fluctuators/fluctuators.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/format_percentage.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/format_percentage.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/gadgets/summation/summation.svg` & `rollercoaster-2.1.4/venues/stages/rollercoaster/gadgets/summation/summation.svg`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/home.MD` & `rollercoaster-2.1.4/venues/stages/rollercoaster/home.MD`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/home.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/home.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/rides.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/rides.S.HTML`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 		
 	<h2>description</h2>
 	
 		VHLOC indicators,
 			ideally that can be sailed.
 	
 	
-	<h2>necessities</h2>
+	<h2>objectives</h2>
+		# necessities
+		
+		[ ] https://www.tradingview.com/v/6w9Jchj6/
 		
 		[ ] one indicator:
 			[ ] pivots 
 				# pivot points
 			
 				[{
```

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/AO.pine` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/AO.pine`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/HHLL/indicator.pine` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/HHLL/indicator.pine`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/True Range.svg` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/True Range.svg`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/AS.svg` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/AS.svg`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/ST/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/ST/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/AS.svg` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/AS.svg`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/AO/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/AO/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/KernelFunctions.ps` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/KernelFunctions.ps`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/MLExtensions.ps` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/MLExtensions.ps`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/superb/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/ETF.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/ETF.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/TV.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/TV.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/scans/_clique/currency.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/scans/_clique/currency.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/1.JSON` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/1.JSON`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/2.JSON` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/2.JSON`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/0.JSON` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/0.JSON`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/1.JSON` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/1.JSON`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/2.JSON` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/2.JSON`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/clique.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/clique.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/stats/stats.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/stats/stats.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/crypto/crypto.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/crypto/crypto.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/crypto/crypto_usual_features.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/crypto/crypto_usual_features.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/multipliers/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/multipliers/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/sources/sources.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/sources/sources.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/real_estate/varieties/varieties.S.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/real_estate/varieties/varieties.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML` & `rollercoaster-2.1.4/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.3/PKG-INFO` & `rollercoaster-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rollercoaster
-Version: 2.1.3
+Version: 2.1.4
 Summary: economic estimation
 License: GPL 3.0 + CC BY-NC-SA 4.0 + Mongo SSPL
 Keywords: rain & pour,economic estimation,finance,commerce,wealth,money,treasures,treasury,subconscious trading,implicit trading
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

