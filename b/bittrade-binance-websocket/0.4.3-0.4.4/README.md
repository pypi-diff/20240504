# Comparing `tmp/bittrade_binance_websocket-0.4.3.tar.gz` & `tmp/bittrade_binance_websocket-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_binance_websocket-0.4.3.tar", max compression
+gzip compressed data, was "bittrade_binance_websocket-0.4.4.tar", max compression
```

## Comparing `bittrade_binance_websocket-0.4.3.tar` & `bittrade_binance_websocket-0.4.4.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.4.3/README.md
--rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/__init__.py
--rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/__init__.py
--rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/book_ticker.py
--rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/depth.py
--rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/message.py
--rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/open_orders.py
--rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/subscribe.py
--rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/__init__.py
--rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/connection_operators.py
--rw-r--r--   0        0        0     3531 2023-03-26 22:59:27.837091 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/generic.py
--rw-r--r--   0        0        0     2836 2024-03-31 00:34:09.193021 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/http.py
--rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/private.py
--rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/private_user_stream.py
--rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/public_stream.py
--rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/reconnect.py
--rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/__init__.py
--rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/add_order.py
--rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/cancel_order.py
--rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/ping.py
--rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/request_response.py
--rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/time.py
--rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/framework/__init__.py
--rw-r--r--   0        0        0    10862 2024-03-24 01:17:26.653196 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/framework/framework.py
--rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/filters/__init__.py
--rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/filters/kind.py
--rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/heartbeat.py
--rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/json.py
--rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/listen.py
--rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/__init__.py
--rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/accounts.py
--rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/contingency_type.py
--rw-r--r--   0        0        0     2186 2024-03-24 01:13:41.661806 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/endpoints.py
--rw-r--r--   0        0        0     1597 2023-04-12 10:32:29.217681 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0     5572 2024-03-24 01:15:19.833562 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/framework.py
--rw-r--r--   0        0        0      872 2024-03-07 07:45:37.550442 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/loan.py
--rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/message.py
--rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/oco_list_status.py
--rw-r--r--   0        0        0     5822 2023-12-29 07:38:44.204038 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/order.py
--rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/order_status.py
--rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/permission.py
--rw-r--r--   0        0        0      289 2024-01-31 20:08:59.754811 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/portfolio.py
--rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/private.py
--rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/request.py
--rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/response_message.py
--rw-r--r--   0        0        0       15 2023-03-07 05:38:31.457289 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/get_time.py
--rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/listen_key.py
--rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/margin_account.py
--rw-r--r--   0        0        0     4822 2024-03-20 05:48:12.475535 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/subaccount.py
--rw-r--r--   0        0        0      155 2023-08-11 03:01:00.567477 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/symbol_price_book_ticker.py
--rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/symbol_status.py
--rw-r--r--   0        0        0     1112 2023-04-13 04:00:27.126562 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/trade.py
--rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/operators/__init__.py
--rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/operators/orderbook/__init__.py
--rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/operators/stream/response_messages.py
--rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/__init__.py
--rw-r--r--   0        0        0     1428 2024-03-21 03:36:28.175760 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/account_information.py
--rw-r--r--   0        0        0     1199 2024-03-21 03:40:41.482848 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/cancel_order.py
--rw-r--r--   0        0        0     1198 2024-03-21 03:39:54.416229 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/create_order.py
--rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/current_open_orders.py
--rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/get_time.py
--rw-r--r--   0        0        0     1408 2024-03-21 03:54:13.880279 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/http_factory_decorator.py
--rw-r--r--   0        0        0     3288 2024-03-13 06:37:04.186727 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/listen_key.py
--rw-r--r--   0        0        0     2295 2024-03-07 08:46:32.989830 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/margin_loan.py
--rw-r--r--   0        0        0      541 2024-01-31 20:10:47.047786 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/margin_portfolio.py
--rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_margin_account.py
--rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_margin_fee_data.py
--rw-r--r--   0        0        0      553 2024-03-07 08:45:29.544664 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_margin_price_index.py
--rw-r--r--   0        0        0      697 2024-03-24 01:17:20.975687 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py
--rw-r--r--   0        0        0     2232 2024-03-20 05:56:59.028919 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/subaccount.py
--rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/symbol_orders_cancel.py
--rw-r--r--   0        0        0      687 2023-08-11 03:01:27.219437 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/symbol_price_book_ticker.py
--rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/symbol_price_ticker.py
--rw-r--r--   0        0        0     2271 2023-04-13 07:43:16.471911 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/trade_list.py
--rw-r--r--   0        0        0     3824 2023-03-30 09:47:19.704651 bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/sign.py
--rw-r--r--   0        0        0     1769 2024-03-31 00:46:21.248192 bittrade_binance_websocket-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.3/setup.py
--rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     4488 2023-03-07 05:41:03.026348 bittrade_binance_websocket-0.4.4/README.md
+-rw-r--r--   0        0        0       24 2023-03-07 05:17:43.720880 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/__init__.py
+-rw-r--r--   0        0        0      169 2023-03-24 09:56:30.829676 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/__init__.py
+-rw-r--r--   0        0        0     1349 2023-03-24 09:56:30.829844 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/book_ticker.py
+-rw-r--r--   0        0        0     1310 2023-03-24 09:56:30.829984 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/depth.py
+-rw-r--r--   0        0        0      238 2023-03-24 09:56:30.830247 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/message.py
+-rw-r--r--   0        0        0      437 2023-03-26 22:59:27.836025 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/open_orders.py
+-rw-r--r--   0        0        0     2150 2023-03-24 09:56:30.830917 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/subscribe.py
+-rw-r--r--   0        0        0      387 2023-03-24 09:56:30.831631 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/__init__.py
+-rw-r--r--   0        0        0      984 2023-03-26 22:59:27.836890 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/connection_operators.py
+-rw-r--r--   0        0        0     3559 2024-04-05 01:44:17.205438 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2836 2024-03-31 00:34:09.193021 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/http.py
+-rw-r--r--   0        0        0     1020 2023-03-24 09:56:30.834946 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/private.py
+-rw-r--r--   0        0        0     2843 2023-03-28 23:26:32.900253 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/private_user_stream.py
+-rw-r--r--   0        0        0      866 2023-03-24 09:56:30.835882 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/public_stream.py
+-rw-r--r--   0        0        0     3556 2023-03-07 05:17:43.704616 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/reconnect.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:56:30.836219 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/__init__.py
+-rw-r--r--   0        0        0     3411 2023-04-04 10:06:55.441962 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/add_order.py
+-rw-r--r--   0        0        0     4603 2023-04-04 10:06:55.443228 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/cancel_order.py
+-rw-r--r--   0        0        0     1222 2023-03-24 09:56:30.837752 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/ping.py
+-rw-r--r--   0        0        0     1955 2023-03-26 22:59:27.837933 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/request_response.py
+-rw-r--r--   0        0        0     1160 2023-03-24 09:56:30.838014 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/time.py
+-rw-r--r--   0        0        0      109 2023-03-24 09:56:30.843408 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/framework/__init__.py
+-rw-r--r--   0        0        0    11013 2024-04-16 08:51:05.177221 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/framework/framework.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.701890 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:17:43.699712 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/filters/__init__.py
+-rw-r--r--   0        0        0      628 2023-03-24 09:56:30.844042 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/filters/kind.py
+-rw-r--r--   0        0        0      197 2023-03-07 05:17:43.702941 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/heartbeat.py
+-rw-r--r--   0        0        0      709 2023-03-07 05:17:43.703639 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/json.py
+-rw-r--r--   0        0        0      710 2023-03-24 09:56:30.844242 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/listen.py
+-rw-r--r--   0        0        0      500 2023-03-26 22:59:27.838272 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/__init__.py
+-rw-r--r--   0        0        0      200 2023-03-26 22:59:27.838358 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/accounts.py
+-rw-r--r--   0        0        0       76 2023-03-24 09:56:30.844826 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/contingency_type.py
+-rw-r--r--   0        0        0     2461 2024-05-03 22:43:05.431269 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/endpoints.py
+-rw-r--r--   0        0        0     1597 2023-04-12 10:32:29.217681 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0     5670 2024-04-16 08:51:09.517146 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/framework.py
+-rw-r--r--   0        0        0      872 2024-03-07 07:45:37.550442 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/loan.py
+-rw-r--r--   0        0        0      430 2023-03-26 22:59:27.838973 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/message.py
+-rw-r--r--   0        0        0      404 2023-03-24 09:56:30.847283 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/oco_list_status.py
+-rw-r--r--   0        0        0     5822 2023-12-29 07:38:44.204038 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/order.py
+-rw-r--r--   0        0        0      951 2023-03-24 09:56:30.847605 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/order_status.py
+-rw-r--r--   0        0        0      316 2023-03-24 09:56:30.847749 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/permission.py
+-rw-r--r--   0        0        0      289 2024-01-31 20:08:59.754811 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/portfolio.py
+-rw-r--r--   0        0        0      170 2023-04-04 10:06:55.444253 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/private.py
+-rw-r--r--   0        0        0      441 2023-03-24 09:56:30.848482 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/request.py
+-rw-r--r--   0        0        0      280 2023-03-26 23:08:09.996282 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/response_message.py
+-rw-r--r--   0        0        0      556 2024-05-03 22:39:51.170025 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0     2258 2024-05-03 22:58:13.147490 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/api_key.py
+-rw-r--r--   0        0        0       85 2023-03-07 06:12:01.053861 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/get_time.py
+-rw-r--r--   0        0        0       91 2023-03-24 09:56:30.849188 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/listen_key.py
+-rw-r--r--   0        0        0      595 2023-03-28 03:30:34.779137 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/margin_account.py
+-rw-r--r--   0        0        0     4822 2024-03-20 05:48:12.475535 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/subaccount.py
+-rw-r--r--   0        0        0      155 2023-08-11 03:01:00.567477 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/symbol_price_book_ticker.py
+-rw-r--r--   0        0        0       98 2023-03-26 22:59:27.839358 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0      254 2023-03-24 09:56:30.849325 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/symbol_status.py
+-rw-r--r--   0        0        0     1112 2023-04-13 04:00:27.126562 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/trade.py
+-rw-r--r--   0        0        0       16 2023-03-07 05:17:43.713863 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/operators/__init__.py
+-rw-r--r--   0        0        0      740 2023-03-07 05:17:43.715065 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/operators/orderbook/__init__.py
+-rw-r--r--   0        0        0      696 2023-03-26 22:59:27.840157 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/operators/stream/response_messages.py
+-rw-r--r--   0        0        0        0 2023-03-07 05:21:43.314741 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/__init__.py
+-rw-r--r--   0        0        0     1428 2024-03-21 03:36:28.175760 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/account_information.py
+-rw-r--r--   0        0        0     4562 2024-05-03 22:50:11.064813 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/api_key.py
+-rw-r--r--   0        0        0     1199 2024-03-21 03:40:41.482848 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/cancel_order.py
+-rw-r--r--   0        0        0     1198 2024-03-21 03:39:54.416229 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/create_order.py
+-rw-r--r--   0        0        0      724 2023-04-01 05:17:10.507682 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/current_open_orders.py
+-rw-r--r--   0        0        0      533 2023-03-07 07:26:25.278031 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/get_time.py
+-rw-r--r--   0        0        0     1408 2024-03-21 03:54:13.880279 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/http_factory_decorator.py
+-rw-r--r--   0        0        0     3288 2024-03-13 06:37:04.186727 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/listen_key.py
+-rw-r--r--   0        0        0     2295 2024-03-07 08:46:32.989830 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/margin_loan.py
+-rw-r--r--   0        0        0      541 2024-01-31 20:10:47.047786 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/margin_portfolio.py
+-rw-r--r--   0        0        0      680 2023-03-28 03:38:33.700120 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_margin_account.py
+-rw-r--r--   0        0        0      718 2023-03-28 03:39:36.381947 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_margin_fee_data.py
+-rw-r--r--   0        0        0      553 2024-03-07 08:45:29.544664 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_margin_price_index.py
+-rw-r--r--   0        0        0      697 2024-03-24 01:17:20.975687 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py
+-rw-r--r--   0        0        0     2731 2024-04-16 08:49:52.006258 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/subaccount.py
+-rw-r--r--   0        0        0     1241 2023-04-01 05:22:24.238266 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/symbol_orders_cancel.py
+-rw-r--r--   0        0        0      687 2023-08-11 03:01:27.219437 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/symbol_price_book_ticker.py
+-rw-r--r--   0        0        0      669 2023-03-26 22:59:27.840905 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/symbol_price_ticker.py
+-rw-r--r--   0        0        0     2271 2023-04-13 07:43:16.471911 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/trade_list.py
+-rw-r--r--   0        0        0     3848 2024-05-03 01:25:21.922596 bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/sign.py
+-rw-r--r--   0        0        0     1770 2024-05-03 22:22:57.145307 bittrade_binance_websocket-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6057 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.4/setup.py
+-rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 bittrade_binance_websocket-0.4.4/PKG-INFO
```

### Comparing `bittrade_binance_websocket-0.4.3/README.md` & `bittrade_binance_websocket-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/book_ticker.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/book_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/depth.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/depth.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/channels/subscribe.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/channels/subscribe.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/connection_operators.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/connection_operators.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/generic.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 category = WEBSOCKET_MESSAGE
                 raw_logger.debug(message)
                 logger.debug("[SOCKET][RAW] %s", message)
 
                 try:
                     observer.on_next((enhanced, category, pass_message))
                 except:
-                    logger.exception("[SOCKET] Error on socket message")
+                    logger.error("[SOCKET] Error on socket message", stack_info=True, exc_info=True)
 
             connection = WebSocketApp(
                 url,
                 on_open=on_open,
                 on_close=on_close,
                 on_error=on_error,
                 on_message=on_message,
```

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/http.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/private.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/private.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/private_user_stream.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/private_user_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/public_stream.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/public_stream.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/connection/reconnect.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/connection/reconnect.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/add_order.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/add_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/cancel_order.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/ping.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/ping.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/request_response.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/request_response.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/events/time.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/events/time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/framework/framework.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/framework/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     cancel_symbol_orders_factory,
 )
 from bittrade_binance_websocket.rest.account_information import (
     get_account_information_http_factory,
 )
 from bittrade_binance_websocket.rest.subaccount import (
     query_subaccount_list_http_factory, query_subaccount_margin_summary_http_factory, subaccount_universal_transfer_http_factory, query_subaccount_margin_detail_http_factory, subaccount_transfer_to_master_http_factory, subaccount_transfer_to_subaccount_http_factory,
-    user_universal_transfer_http_factory
+    user_universal_transfer_http_factory, subaccount_add_ip_restriction_http_factory,
 )
 from bittrade_binance_websocket.rest.cancel_order import cancel_order_http_factory
 from bittrade_binance_websocket.rest.margin_portfolio import portfolio_margin_account_info_http_factory
 from bittrade_binance_websocket.rest.query_margin_account import (
     query_margin_account_details_http_factory,
 )
 from bittrade_binance_websocket.rest.query_max_transfer_out_amount import (
@@ -209,14 +209,15 @@
         spot_symbol_orders_cancel=spot_symbol_orders_cancel,
         subaccount_query_list_http=query_subaccount_list_http_factory(trade_signer_http),
         subaccount_query_margin_summary_http=query_subaccount_margin_summary_http_factory(trade_signer_http),
         subaccount_query_margin_detail_http=query_subaccount_margin_detail_http_factory(trade_signer_http),
         subaccount_universal_transfer_http=subaccount_universal_transfer_http_factory(trade_signer_http),
         subaccount_transfer_to_master_http=subaccount_transfer_to_master_http_factory(trade_signer_http),
         subaccount_transfer_to_subaccount_http=subaccount_transfer_to_subaccount_http_factory(trade_signer_http),
+        subaccount_add_ip_restriction_http=subaccount_add_ip_restriction_http_factory(trade_signer_http),
         user_universal_transfer_http=user_universal_transfer_http_factory(trade_signer_http),
         order_create_http=create_order_http_factory(trade_signer_http),
         order_cancel_http=cancel_order_http_factory(trade_signer_http),
         trade_list_http=account_trade_list_http_factory(trade_signer_http),
         symbol_orders_cancel_http=symbol_orders_cancel_http,
         current_open_orders_http=open_orders_http,
         user_data_stream_messages=user_data_stream_messages,
```

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/filters/kind.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/filters/kind.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/json.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/json.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/messages/listen.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/messages/listen.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/endpoints.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 # https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md
 class BinanceEndpoints(Enum):
     SPOT_OPEN_ORDERS = "/api/v3/openOrders"
     ACCOUNT_INFORMATION = "/api/v3/account"
     GET_TIME = "/api/v3/time"
     CROSS_MARGIN_LISTEN_KEY = "/sapi/v1/userDataStream"
     ISOLATED_MARGIN_LISTEN_KEY = "/sapi/v1/userDataStream/isolated"
+    MARGIN_SPECIAL_MARGIN_KEY = "/sapi/v1/margin/apiKey"
+    MARGIN_SPECIAL_MARGIN_KEY_IP = "/sapi/v1/margin/apiKey/ip"
+    MARGIN_SPECIAL_MARGIN_KEY_LIST = "/sapi/v1/margin/api-key-list"
     LISTEN_KEY = "/api/v3/userDataStream"
     MARGIN_OPEN_ORDERS = "/sapi/v1/margin/openOrders"
     MARGIN_ORDER = "/sapi/v1/margin/order"
     MARGIN_MAX_BORROWABLE = "/sapi/v1/margin/maxBorrowable"
     MARGIN_LOAN = "/sapi/v1/margin/loan"
     MARGIN_PORTFOLIO_ACCOUNT_INFORMATION = "/sapi/v1/portfolio/account"
     MARGIN_REPAY = "/sapi/v1/margin/repay"
@@ -29,12 +32,13 @@
     QUERY_CROSS_MARGIN_FEE_DATA = "/sapi/v1/margin/crossMarginData"
     SYMBOL_PRICE_TICKER = "/api/v3/ticker/price"
     SYMBOL_BOOK_TICKER = "/api/v3/ticker/bookTicker"
     SUBACCOUNT_LIST = "/sapi/v1/sub-account/list"
     SUBACCOUNT_SUMMARY = "/sapi/v1/sub-account/margin/accountSummary"
     SUBACCOUNT_MARGIN_DETAIL = "/sapi/v1/sub-account/margin/account"
     SUBACCOUNT_ASSETS = "/sapi/v3/sub-account/assets"
+    SUBACCOUNT_ADD_IP_RESTRICTION = "/sapi/v2/sub-account/subAccountApi/ipRestriction"
     SUBACCOUNT_TRANSFER = "/sapi/v1/sub-account/margin/transfer"
     SUBACCOUNT_UNIVERSAL_TRANSFER = "/sapi/v1/sub-account/universalTransfer"
     SUBACCOUNT_TO_MASTER_TRANSFER = "/sapi/v1/sub-account/transfer/subToMaster"
     SUBACCOUNT_TO_SUBACCOUNT_TRANSFER = "/sapi/v1/sub-account/transfer/subToSub"
     USER_UNIVERSAL_TRANSFER = "/sapi/v1/asset/transfer"
```

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/enhanced_websocket.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/framework.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     spot_order_cancel: Callable[[OrderCancelRequest], Observable[dict]]
     subaccount_query_list_http: Callable[[], Observable[dict]]
     subaccount_query_margin_summary_http: Callable[[], Observable[dict]]
     subaccount_query_margin_detail_http: Callable[[str], Observable[dict]]
     subaccount_universal_transfer_http: Callable[[UniversalTransferRequest], Observable[dict]]
     subaccount_transfer_to_master_http: Callable[[str, str], Observable[dict]]
     subaccount_transfer_to_subaccount_http: Callable[[str, str, str], Observable[dict]]
+    subaccount_add_ip_restriction_http: Callable[[str, str, Literal[1,2], str], Observable[dict]]
     order_create_http: Callable[[PlaceOrderRequest], Observable[SymbolOrderResponseItem]]
     order_cancel_http: Callable[[OrderCancelRequest], Observable[SymbolOrderResponseItem]]
     trade_list_http: Callable[[TradeDataRequest], Observable[list[TradeDict]]]
     margin_account_borrow_http: Callable[[AccountBorrowRequest], Observable[dict]]
     margin_account_repay_http: Callable[[AccountBorrowRequest], Observable[dict]]
     margin_portfolio_account_information: Callable[[], Observable[PortfolioMarginAccountInfo]]
     available_inventory_http: Callable[[bool], Observable[dict]]
```

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/loan.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/loan.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/order.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/order_status.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/order_status.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/margin_account.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/rest/subaccount.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/rest/subaccount.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/models/trade.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/models/trade.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/operators/orderbook/__init__.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/operators/orderbook/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/operators/stream/response_messages.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/operators/stream/response_messages.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/account_information.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/account_information.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/cancel_order.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/create_order.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/create_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/current_open_orders.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/current_open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/get_time.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/get_time.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/http_factory_decorator.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/http_factory_decorator.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/listen_key.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/listen_key.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/margin_loan.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/margin_loan.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/margin_portfolio.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_margin_account.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_margin_account.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_margin_fee_data.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_margin_fee_data.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_margin_price_index.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_margin_price_index.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/query_max_transfer_out_amount.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/subaccount.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/subaccount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Literal
 from bittrade_binance_websocket.models import endpoints, request
 from bittrade_binance_websocket.models.rest.subaccount import UniversalTransferRequest, UserUniversalTransferRequest
 from bittrade_binance_websocket.rest.http_factory_decorator import http_factory
 
 
 @http_factory(None)  # type: ignore
 def query_subaccount_list_http_factory():
@@ -61,8 +62,21 @@
 
 @http_factory(None)  # type: ignore
 def query_subaccount_margin_detail_http_factory(email: str):
     return request.RequestMessage(
         method="GET",
         endpoint=endpoints.BinanceEndpoints.SUBACCOUNT_MARGIN_DETAIL,
         params={"email": email},
+    )
+
+@http_factory(None)  # type: ignore
+def subaccount_add_ip_restriction_http_factory(email: str, api_key: str, status: Literal[1,2], ip_addresses: list[str]):
+    return request.RequestMessage(
+        method="POST",
+        endpoint=endpoints.BinanceEndpoints.SUBACCOUNT_ADD_IP_RESTRICTION,
+        params={
+            "email": email,
+            "subAccountApiKey": api_key,
+            "status": status,
+            "ipAddress": ",".join(ip_addresses),
+        }
     )
```

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/symbol_orders_cancel.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/symbol_orders_cancel.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/symbol_price_book_ticker.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/symbol_price_book_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/symbol_price_ticker.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/symbol_price_ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/rest/trade_list.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/rest/trade_list.py`

 * *Files identical despite different names*

### Comparing `bittrade_binance_websocket-0.4.3/bittrade_binance_websocket/sign.py` & `bittrade_binance_websocket-0.4.4/bittrade_binance_websocket/sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 import hashlib
 import hmac
 from typing import Any, Dict, Tuple, Union, cast
-from urllib.parse import urlencode
+from urllib.parse import urlencode, quote
 
 from expression import curry_flip
 from datetime import datetime
 
 import requests
 
 
@@ -98,15 +98,15 @@
         request.headers.update({"X-MBX-APIKEY": key})
         if request.method == "GET":
             payload = request.params
         else:
             payload = request.data
         payload = del_none(payload)
         # Code adapted from https://github.com/binance/binance-signature-examples/blob/master/python/spot/spot.py
-        query_string = urlencode(payload, True)
+        query_string = urlencode(payload, True, quote_via=quote)
         ts = int(datetime.now().timestamp() * 1000)
         if query_string:
             query_string = "{}&timestamp={}".format(query_string, ts)
         else:
             query_string = "timestamp={}".format(ts)
 
         url = request.url + "?" + query_string + "&signature=" + hashing(query_string)
```

### Comparing `bittrade_binance_websocket-0.4.3/pyproject.toml` & `bittrade_binance_websocket-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-binance-websocket"
-version = "0.4.3"
+version = "0.4.4"
 description = "Reactive Websocket for Binance"
 authors = ["mat <matt@techspace.asia>"]
 readme = "README.md"
 repository = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 homepage = "https://github.com/TechSpaceAsia/bittrade-binance-websocket"
 license = "MIT"
 classifiers = [
@@ -50,14 +50,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `bittrade_binance_websocket-0.4.3/setup.py` & `bittrade_binance_websocket-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.4.2,<2.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'bittrade-binance-websocket',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'Reactive Websocket for Binance',
     'long_description': '# Binance Websocket\n\n[NOT RELEASED] This is very much a work in progress, despite being on pypi.\nMost things might be wrongly documented; API **will** change\n\n## Features\n\n- Reconnect with incremental backoff \n- Respond to ping\n- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API\n- ... but provides more info than a simple request/response; \n  for instance, `add_order` goes through each stage submitted->pending->open or canceled, \n  emitting a notification at each stage\n\n## Installing\n\n`pip install bittrade-binance-websocket` or `poetry add bittrade-binance-websocket`\n\n## General considerations\n\n### Observables/Reactivex\n\nThe whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).\n\nThough Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.\n\nFor simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below\n\n### Concurrency\n\nInternally the library uses threads.\nFor your main program you don\'t have to worry about threads; you can block the main thread.\n\n## Getting started\n\n### Connect to the public feeds\n\n```python\nfrom bittrade_huobi_websocket import public_websocket_connection, subscribe_ticker\nfrom bittrade_huobi_websocket.operators import keep_messages_only, filter_new_socket_only\n\n# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method\nsocket_connection = public_websocket_connection()\n# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…\nmessages = socket_connection.pipe(\n    keep_messages_only(),\n)\nsocket_connection.pipe(\n    filter_new_socket_only(),\n    subscribe_ticker(\'USDT/USD\', messages)\n).subscribe(\n    print, print, print  # you can do anything with the messages; here we simply print them out\n)\nsocket_connection.connect()\n```\n\n_(This script is complete, it should run "as is")_\n\n\n## Logging\n\nWe use Python\'s standard logging.\nYou can modify what logs you see as follows:\n\n```\nlogging.getLogger(\'bittrade_huobi_websocket\').addHandler(logging.StreamHandler())\n```\n\nIn addition, two special logger logs every message sent/received from the socket (except heartbeat) at the `DEBUG` level: `bittrade_huobi_websocket.raw_socket.sent` and `bittrade_huobi_websocket.raw_socket.received`\n\nTo view a full, timestamped history of the socket exchanges use\n\n```\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.sent")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d <== %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\nhandler = FileHandler("logs/raw_socket.log")\nhandler.setLevel(DEBUG)\nlogger = logging.getLogger("bittrade_huobi_websocket.raw_socket.received")\nformatter = logging.Formatter("%(asctime)s.%(msecs)03d --> %(message)s", datefmt="%H:%M:%S")\nhandler.setFormatter(formatter)\nlogger.addHandler(handler)\n```\n\n## Private feeds\n\nSimilar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.\n\nThis means that you\'ll need to implement the signature token yourself. The library never has access to your API secret.\n\nSee `examples/sign.py` for an example of implementation but it is generally as simple as:\n\n```python\nauthenticated_sockets = connection.pipe(\n    filter_new_socket_only(),\n    operators.map(add_token),\n    operators.share(),\n)\n```\n\n# Development guidelines\n\n## `*_http` methods\n\nREST functions over http should be suffixed with `_http` e.g. `get_book_http`.\nThey should return an Observable containing the *full* json body; this is easily achieved via `prepare_request` and `send_request`.\n\nWhere possible models should be defined to describe the *raw* result and *parsed result* if available/useful.\n\nReactive operators may be provided for parsing, but they should never be included in the *raw* functionality of the `*_http` function, only optional.\n\nAny operator that maps to CCXT types should be suffixed with `_ccxt` e.g. `parse_book_ccxt`.',
     'author': 'mat',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TechSpaceAsia/bittrade-binance-websocket',
```

### Comparing `bittrade_binance_websocket-0.4.3/PKG-INFO` & `bittrade_binance_websocket-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-binance-websocket
-Version: 0.4.3
+Version: 0.4.4
 Summary: Reactive Websocket for Binance
 Home-page: https://github.com/TechSpaceAsia/bittrade-binance-websocket
 License: MIT
 Author: mat
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

