# Comparing `tmp/fei_crypto-0.2.5.tar.gz` & `tmp/fei_crypto-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fei_crypto-0.2.5.tar", max compression
+gzip compressed data, was "fei_crypto-0.2.6.tar", max compression
```

## Comparing `fei_crypto-0.2.5.tar` & `fei_crypto-0.2.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       78 2024-04-16 13:51:49.192517 fei_crypto-0.2.5/fei_crypto/__init__.py
--rw-r--r--   0        0        0     3229 2024-05-03 12:57:32.523406 fei_crypto-0.2.5/fei_crypto/binance_signal.py
--rw-r--r--   0        0        0      876 2024-04-16 13:53:17.866879 fei_crypto-0.2.5/fei_crypto/captcha.py
--rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.2.5/fei_crypto/crypto.py
--rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.2.5/fei_crypto/discord_webhook.py
--rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.2.5/fei_crypto/env.py
--rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.2.5/fei_crypto/md5.py
--rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.2.5/fei_crypto/os.py
--rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.2.5/fei_crypto/rmw.py
--rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.2.5/fei_crypto/rnd_emoj.py
--rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.2.5/fei_crypto/t2m.py
--rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.2.5/fei_crypto/time.py
--rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.2.5/LICENSE
--rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.2.5/main/__init__.py
--rw-r--r--   0        0        0      158 2024-05-02 14:53:54.287100 fei_crypto-0.2.5/main/binance_signal.py
--rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.2.5/main/btc_eth.py
--rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.2.5/main/captcha.py
--rw-r--r--   0        0        0      139 2024-04-21 00:43:55.013673 fei_crypto-0.2.5/main/dc_webhook_send.py
--rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.2.5/main/emoj.py
--rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.2.5/main/env.py
--rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.2.5/main/main.py
--rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.2.5/main/os.py
--rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.2.5/main/rmw.py
--rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.2.5/main/say.py
--rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.2.5/main/t2m.py
--rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.2.5/main/tg_forward.py
--rw-r--r--   0        0        0      156 2024-04-17 12:01:33.870269 fei_crypto-0.2.5/main/tg_koltime_menu.py
--rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.2.5/main/tg_login.py
--rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.2.5/main/ts.py
--rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.2.5/main/uu_id.py
--rw-r--r--   0        0        0     1721 2024-05-03 12:58:11.329840 fei_crypto-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3627 2024-04-19 14:51:10.754145 fei_crypto-0.2.5/README.md
--rw-r--r--   0        0        0      389 2024-04-16 14:59:52.401824 fei_crypto-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      196 2024-04-03 09:48:00.078906 fei_crypto-0.2.5/tests/calc.py
--rw-r--r--   0        0        0      356 2024-04-02 16:40:47.033897 fei_crypto-0.2.5/tests/console.py
--rw-r--r--   0        0        0      183 2024-04-03 03:01:53.459809 fei_crypto-0.2.5/tests/dict.py
--rw-r--r--   0        0        0      463 2024-04-16 14:07:08.378494 fei_crypto-0.2.5/tests/enum_test.py
--rw-r--r--   0        0        0       88 2024-04-17 10:03:49.057111 fei_crypto-0.2.5/tests/env_test.py
--rw-r--r--   0        0        0       63 2024-05-02 15:14:00.673971 fei_crypto-0.2.5/tests/format_test.py
--rw-r--r--   0        0        0      206 2024-04-02 15:53:35.170989 fei_crypto-0.2.5/tests/getattr.py
--rw-r--r--   0        0        0       53 2024-03-21 03:22:41.838133 fei_crypto-0.2.5/tests/hello.py
--rw-r--r--   0        0        0     1155 2024-03-21 04:51:46.085571 fei_crypto-0.2.5/tests/image_base64.py
--rw-r--r--   0        0        0      349 2024-04-15 08:49:16.084219 fei_crypto-0.2.5/tests/logging_test.py
--rw-r--r--   0        0        0     1665 2024-03-28 19:19:29.326677 fei_crypto-0.2.5/tests/manim.py
--rw-r--r--   0        0        0      186 2024-04-03 08:27:11.338227 fei_crypto-0.2.5/tests/open.py
--rw-r--r--   0        0        0      545 2024-03-29 07:27:10.711077 fei_crypto-0.2.5/tests/path.py
--rw-r--r--   0        0        0     1315 2024-05-02 06:15:24.476403 fei_crypto-0.2.5/tests/redis_hash.py
--rw-r--r--   0        0        0      641 2024-05-03 06:30:12.789088 fei_crypto-0.2.5/tests/redis_json.py
--rw-r--r--   0        0        0      208 2024-05-03 06:31:15.736761 fei_crypto-0.2.5/tests/redis_json_ticker_price.py
--rw-r--r--   0        0        0     2695 2024-05-02 06:15:54.379887 fei_crypto-0.2.5/tests/redis_koltime_channels.py
--rw-r--r--   0        0        0     1036 2024-04-17 09:58:52.863717 fei_crypto-0.2.5/tests/redis_set_test.py
--rw-r--r--   0        0        0      158 2024-04-17 10:41:30.695499 fei_crypto-0.2.5/tests/scope_test.py
--rw-r--r--   0        0        0      655 2024-05-02 16:29:08.842877 fei_crypto-0.2.5/tests/str_test.py
--rw-r--r--   0        0        0     4083 2024-04-16 15:12:18.915950 fei_crypto-0.2.5/tests/tg_arbitrarycallbackdatabot.py
--rw-r--r--   0        0        0     3228 2024-04-16 14:04:46.204833 fei_crypto-0.2.5/tests/tg_inlinebot.py
--rw-r--r--   0        0        0     2468 2024-04-16 14:04:52.248862 fei_crypto-0.2.5/tests/tg_inlinekeyboard.py
--rw-r--r--   0        0        0     6858 2024-04-16 14:05:05.464671 fei_crypto-0.2.5/tests/tg_inlinekeyboard2.py
--rw-r--r--   0        0        0    13620 2024-04-16 14:05:18.553946 fei_crypto-0.2.5/tests/tg_nestedconversationbot.py
--rw-r--r--   0        0        0     6587 2024-04-16 13:40:50.781376 fei_crypto-0.2.5/tests/tg_pollbot.py
--rw-r--r--   0        0        0     2382 2024-04-16 13:40:28.566730 fei_crypto-0.2.5/tests/tg_rawapibot.py
--rw-r--r--   0        0        0     2707 2024-04-16 14:06:07.187762 fei_crypto-0.2.5/tests/tg_webappbot.py
--rw-r--r--   0        0        0      244 2024-05-02 06:41:48.454180 fei_crypto-0.2.5/tests/time_test.py
--rw-r--r--   0        0        0      924 2024-04-03 02:55:54.333858 fei_crypto-0.2.5/tests/tuple.py
--rw-r--r--   0        0        0      143 2024-04-17 06:38:57.801384 fei_crypto-0.2.5/tests/tuple_list.py
--rw-r--r--   0        0        0      455 2023-11-29 13:21:57.903302 fei_crypto-0.2.5/tests/typer.py
--rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.2.5/tg/__init__.py
--rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.2.5/tg/bot/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-16 05:45:45.842618 fei_crypto-0.2.5/tg/bot/live_bot.py
--rw-r--r--   0        0        0     1757 2024-04-16 05:44:27.008518 fei_crypto-0.2.5/tg/bot/utils.py
--rw-r--r--   0        0        0     3966 2024-04-16 03:35:51.804389 fei_crypto-0.2.5/tg/cli_forward.py
--rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.2.5/tg/cli_login.py
--rw-r--r--   0        0        0     6472 2024-04-15 12:37:24.327913 fei_crypto-0.2.5/tg/config.py
--rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.2.5/tg/const.py
--rw-r--r--   0        0        0     5836 2024-04-22 19:32:40.263679 fei_crypto-0.2.5/tg/koltime_menu_bot.py
--rw-r--r--   0        0        0     5247 2024-04-22 12:43:47.737306 fei_crypto-0.2.5/tg/koltime_menu_bot1.py
--rw-r--r--   0        0        0     3903 2024-04-15 12:46:20.229789 fei_crypto-0.2.5/tg/live.py
--rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.2.5/tg/login.py
--rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.2.5/tg/message.py
--rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.2.5/tg/parse.py
--rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.2.5/tg/past.py
--rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.2.5/tg/plugin_models.py
--rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.2.5/tg/plugins/__init__.py
--rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.2.5/tg/plugins/caption.py
--rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.2.5/tg/plugins/filter.py
--rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.2.5/tg/plugins/fmt.py
--rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.2.5/tg/plugins/replace.py
--rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.2.5/tg/storage.py
--rw-r--r--   0        0        0     1954 2024-04-16 05:44:49.091593 fei_crypto-0.2.5/tg/utils.py
--rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 fei_crypto-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       78 2024-04-16 13:51:49.192517 fei_crypto-0.2.6/fei_crypto/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-03 21:06:28.935834 fei_crypto-0.2.6/fei_crypto/binance_signal.py
+-rw-r--r--   0        0        0      876 2024-04-16 13:53:17.866879 fei_crypto-0.2.6/fei_crypto/captcha.py
+-rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.2.6/fei_crypto/crypto.py
+-rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.2.6/fei_crypto/discord_webhook.py
+-rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.2.6/fei_crypto/env.py
+-rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.2.6/fei_crypto/md5.py
+-rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.2.6/fei_crypto/os_info.py
+-rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.2.6/fei_crypto/rmw.py
+-rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.2.6/fei_crypto/rnd_emoj.py
+-rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.2.6/fei_crypto/t2m.py
+-rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.2.6/fei_crypto/time.py
+-rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.2.6/LICENSE
+-rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.2.6/main/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-02 14:53:54.287100 fei_crypto-0.2.6/main/binance_signal.py
+-rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.2.6/main/btc_eth.py
+-rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.2.6/main/captcha.py
+-rw-r--r--   0        0        0      139 2024-04-21 00:43:55.013673 fei_crypto-0.2.6/main/dc_webhook_send.py
+-rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.2.6/main/emoj.py
+-rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.2.6/main/env.py
+-rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.2.6/main/main.py
+-rw-r--r--   0        0        0      103 2024-05-03 20:58:13.432575 fei_crypto-0.2.6/main/os_info.py
+-rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.2.6/main/rmw.py
+-rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.2.6/main/say.py
+-rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.2.6/main/t2m.py
+-rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.2.6/main/tg_forward.py
+-rw-r--r--   0        0        0      156 2024-04-17 12:01:33.870269 fei_crypto-0.2.6/main/tg_koltime_menu.py
+-rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.2.6/main/tg_login.py
+-rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.2.6/main/ts.py
+-rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.2.6/main/uu_id.py
+-rw-r--r--   0        0        0     1721 2024-05-03 21:08:51.150965 fei_crypto-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3627 2024-04-19 14:51:10.754145 fei_crypto-0.2.6/README.md
+-rw-r--r--   0        0        0      389 2024-04-16 14:59:52.401824 fei_crypto-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-03 09:48:00.078906 fei_crypto-0.2.6/tests/calc.py
+-rw-r--r--   0        0        0      356 2024-04-02 16:40:47.033897 fei_crypto-0.2.6/tests/console.py
+-rw-r--r--   0        0        0      183 2024-04-03 03:01:53.459809 fei_crypto-0.2.6/tests/dict.py
+-rw-r--r--   0        0        0      463 2024-04-16 14:07:08.378494 fei_crypto-0.2.6/tests/enum_test.py
+-rw-r--r--   0        0        0       88 2024-04-17 10:03:49.057111 fei_crypto-0.2.6/tests/env_test.py
+-rw-r--r--   0        0        0       63 2024-05-02 15:14:00.673971 fei_crypto-0.2.6/tests/format_test.py
+-rw-r--r--   0        0        0      206 2024-04-02 15:53:35.170989 fei_crypto-0.2.6/tests/getattr.py
+-rw-r--r--   0        0        0       53 2024-03-21 03:22:41.838133 fei_crypto-0.2.6/tests/hello.py
+-rw-r--r--   0        0        0     1155 2024-03-21 04:51:46.085571 fei_crypto-0.2.6/tests/image_base64.py
+-rw-r--r--   0        0        0      349 2024-04-15 08:49:16.084219 fei_crypto-0.2.6/tests/logging_test.py
+-rw-r--r--   0        0        0     1665 2024-03-28 19:19:29.326677 fei_crypto-0.2.6/tests/manim.py
+-rw-r--r--   0        0        0      186 2024-04-03 08:27:11.338227 fei_crypto-0.2.6/tests/open.py
+-rw-r--r--   0        0        0      545 2024-03-29 07:27:10.711077 fei_crypto-0.2.6/tests/path.py
+-rw-r--r--   0        0        0     1315 2024-05-02 06:15:24.476403 fei_crypto-0.2.6/tests/redis_hash.py
+-rw-r--r--   0        0        0      641 2024-05-03 06:30:12.789088 fei_crypto-0.2.6/tests/redis_json.py
+-rw-r--r--   0        0        0      208 2024-05-03 06:31:15.736761 fei_crypto-0.2.6/tests/redis_json_ticker_price.py
+-rw-r--r--   0        0        0     2695 2024-05-02 06:15:54.379887 fei_crypto-0.2.6/tests/redis_koltime_channels.py
+-rw-r--r--   0        0        0     1036 2024-04-17 09:58:52.863717 fei_crypto-0.2.6/tests/redis_set_test.py
+-rw-r--r--   0        0        0      158 2024-04-17 10:41:30.695499 fei_crypto-0.2.6/tests/scope_test.py
+-rw-r--r--   0        0        0      655 2024-05-02 16:29:08.842877 fei_crypto-0.2.6/tests/str_test.py
+-rw-r--r--   0        0        0     4083 2024-04-16 15:12:18.915950 fei_crypto-0.2.6/tests/tg_arbitrarycallbackdatabot.py
+-rw-r--r--   0        0        0     3228 2024-04-16 14:04:46.204833 fei_crypto-0.2.6/tests/tg_inlinebot.py
+-rw-r--r--   0        0        0     2468 2024-04-16 14:04:52.248862 fei_crypto-0.2.6/tests/tg_inlinekeyboard.py
+-rw-r--r--   0        0        0     6858 2024-04-16 14:05:05.464671 fei_crypto-0.2.6/tests/tg_inlinekeyboard2.py
+-rw-r--r--   0        0        0    13620 2024-04-16 14:05:18.553946 fei_crypto-0.2.6/tests/tg_nestedconversationbot.py
+-rw-r--r--   0        0        0     6587 2024-04-16 13:40:50.781376 fei_crypto-0.2.6/tests/tg_pollbot.py
+-rw-r--r--   0        0        0     2382 2024-04-16 13:40:28.566730 fei_crypto-0.2.6/tests/tg_rawapibot.py
+-rw-r--r--   0        0        0     2707 2024-04-16 14:06:07.187762 fei_crypto-0.2.6/tests/tg_webappbot.py
+-rw-r--r--   0        0        0      244 2024-05-02 06:41:48.454180 fei_crypto-0.2.6/tests/time_test.py
+-rw-r--r--   0        0        0      924 2024-04-03 02:55:54.333858 fei_crypto-0.2.6/tests/tuple.py
+-rw-r--r--   0        0        0      143 2024-04-17 06:38:57.801384 fei_crypto-0.2.6/tests/tuple_list.py
+-rw-r--r--   0        0        0      455 2023-11-29 13:21:57.903302 fei_crypto-0.2.6/tests/typer.py
+-rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.2.6/tg/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.2.6/tg/bot/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-16 05:45:45.842618 fei_crypto-0.2.6/tg/bot/live_bot.py
+-rw-r--r--   0        0        0     1757 2024-04-16 05:44:27.008518 fei_crypto-0.2.6/tg/bot/utils.py
+-rw-r--r--   0        0        0     3966 2024-04-16 03:35:51.804389 fei_crypto-0.2.6/tg/cli_forward.py
+-rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.2.6/tg/cli_login.py
+-rw-r--r--   0        0        0     6472 2024-04-15 12:37:24.327913 fei_crypto-0.2.6/tg/config.py
+-rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.2.6/tg/const.py
+-rw-r--r--   0        0        0     5836 2024-04-22 19:32:40.263679 fei_crypto-0.2.6/tg/koltime_menu_bot.py
+-rw-r--r--   0        0        0     5247 2024-04-22 12:43:47.737306 fei_crypto-0.2.6/tg/koltime_menu_bot1.py
+-rw-r--r--   0        0        0     3903 2024-04-15 12:46:20.229789 fei_crypto-0.2.6/tg/live.py
+-rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.2.6/tg/login.py
+-rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.2.6/tg/message.py
+-rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.2.6/tg/parse.py
+-rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.2.6/tg/past.py
+-rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.2.6/tg/plugin_models.py
+-rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.2.6/tg/plugins/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.2.6/tg/plugins/caption.py
+-rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.2.6/tg/plugins/filter.py
+-rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.2.6/tg/plugins/fmt.py
+-rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.2.6/tg/plugins/replace.py
+-rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.2.6/tg/storage.py
+-rw-r--r--   0        0        0     1954 2024-04-16 05:44:49.091593 fei_crypto-0.2.6/tg/utils.py
+-rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 fei_crypto-0.2.6/PKG-INFO
```

### Comparing `fei_crypto-0.2.5/fei_crypto/binance_signal.py` & `fei_crypto-0.2.6/fei_crypto/binance_signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,24 +58,22 @@
     if pre_doc is None:
         print("ERR:pre doc is None")
         return
 
     ms = milliseconds()
     with connection:
         for item in doc:
+            symbol = item["symbol"]
+            if not str.endswith(symbol, "USDT"):
+                continue
             for p_item in pre_doc[0]:
-                symbol = item["symbol"]
                 if p_item["symbol"] == symbol:
-                    if not str.endswith(symbol, "USDT"):
-                        break
                     price_diff = (float(item["price"]) - float(p_item["price"])) / float(p_item["price"])
                     timestamp_diff = item["time"] - p_item["time"]
-                    if 0 < ms - item["time"] < 100000 and 30 * 60 * 1000 > timestamp_diff >= 60 * 1000 and abs(
-                            price_diff) > ratio:
-
+                    if 0 < ms - item["time"] < 60 * 1000 <= timestamp_diff < 30 * 60 * 1000 and abs(price_diff) > ratio:
                         print(f'🔥【{symbol}】')
 
                         pos_side = "LONG"
                         if price_diff < 0:
                             pos_side = "SHORT"
 
                         with connection.cursor() as cursor:
@@ -87,7 +85,11 @@
                                 format(price_diff, ".4f"),
                                 timestamp_diff))
 
                         connection.commit()
                     break
 
     print("🐸 执行成功")
+
+
+if __name__ == '__main__':
+    binance_signal(0.017)
```

### Comparing `fei_crypto-0.2.5/fei_crypto/captcha.py` & `fei_crypto-0.2.6/fei_crypto/captcha.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/fei_crypto/discord_webhook.py` & `fei_crypto-0.2.6/fei_crypto/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/fei_crypto/rmw.py` & `fei_crypto-0.2.6/fei_crypto/rmw.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/fei_crypto/rnd_emoj.py` & `fei_crypto-0.2.6/fei_crypto/rnd_emoj.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/fei_crypto/t2m.py` & `fei_crypto-0.2.6/fei_crypto/t2m.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/LICENSE` & `fei_crypto-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/pyproject.toml` & `fei_crypto-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = [
     { include = "fei_crypto" },
     { include = "tg" },
     { include = "main" },
     { include = "tests" },
 ]
 readme = "README.md"
-version = "0.2.5"
+version = "0.2.6"
 
 [tool.poetry.dependencies]
 cowsay = "^6.1"
 filestools = "^0.2.1"
 pillow = "^9.5.0"
 python = "<3.12,>=3.10"
 discord-webhook = "^1.3.1"
```

### Comparing `fei_crypto-0.2.5/README.md` & `fei_crypto-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/image_base64.py` & `fei_crypto-0.2.6/tests/image_base64.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/manim.py` & `fei_crypto-0.2.6/tests/manim.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/path.py` & `fei_crypto-0.2.6/tests/path.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/redis_hash.py` & `fei_crypto-0.2.6/tests/redis_hash.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/redis_json.py` & `fei_crypto-0.2.6/tests/redis_json.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/redis_koltime_channels.py` & `fei_crypto-0.2.6/tests/redis_koltime_channels.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/redis_set_test.py` & `fei_crypto-0.2.6/tests/redis_set_test.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/str_test.py` & `fei_crypto-0.2.6/tests/str_test.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_arbitrarycallbackdatabot.py` & `fei_crypto-0.2.6/tests/tg_arbitrarycallbackdatabot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_inlinebot.py` & `fei_crypto-0.2.6/tests/tg_inlinebot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_inlinekeyboard.py` & `fei_crypto-0.2.6/tests/tg_inlinekeyboard.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_inlinekeyboard2.py` & `fei_crypto-0.2.6/tests/tg_inlinekeyboard2.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_nestedconversationbot.py` & `fei_crypto-0.2.6/tests/tg_nestedconversationbot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_pollbot.py` & `fei_crypto-0.2.6/tests/tg_pollbot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_rawapibot.py` & `fei_crypto-0.2.6/tests/tg_rawapibot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tg_webappbot.py` & `fei_crypto-0.2.6/tests/tg_webappbot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tests/tuple.py` & `fei_crypto-0.2.6/tests/tuple.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/bot/live_bot.py` & `fei_crypto-0.2.6/tg/bot/live_bot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/bot/utils.py` & `fei_crypto-0.2.6/tg/bot/utils.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/cli_forward.py` & `fei_crypto-0.2.6/tg/cli_forward.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/cli_login.py` & `fei_crypto-0.2.6/tg/cli_login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/config.py` & `fei_crypto-0.2.6/tg/config.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/koltime_menu_bot.py` & `fei_crypto-0.2.6/tg/koltime_menu_bot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/koltime_menu_bot1.py` & `fei_crypto-0.2.6/tg/koltime_menu_bot1.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/live.py` & `fei_crypto-0.2.6/tg/live.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/login.py` & `fei_crypto-0.2.6/tg/login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/message.py` & `fei_crypto-0.2.6/tg/message.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/past.py` & `fei_crypto-0.2.6/tg/past.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/plugin_models.py` & `fei_crypto-0.2.6/tg/plugin_models.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/plugins/__init__.py` & `fei_crypto-0.2.6/tg/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/plugins/filter.py` & `fei_crypto-0.2.6/tg/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/plugins/fmt.py` & `fei_crypto-0.2.6/tg/plugins/fmt.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/plugins/replace.py` & `fei_crypto-0.2.6/tg/plugins/replace.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/storage.py` & `fei_crypto-0.2.6/tg/storage.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/tg/utils.py` & `fei_crypto-0.2.6/tg/utils.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.2.5/PKG-INFO` & `fei_crypto-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fei-crypto
-Version: 0.2.5
+Version: 0.2.6
 Summary: fei crypto command utils
 License: MIT
 Author: feicrypto
 Author-email: feicrypto@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

