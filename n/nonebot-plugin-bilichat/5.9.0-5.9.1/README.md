# Comparing `tmp/nonebot_plugin_bilichat-5.9.0.tar.gz` & `tmp/nonebot_plugin_bilichat-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.9.0.tar", last modified: Fri May  3 08:18:40 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.9.1.tar", last modified: Fri May  3 08:44:34 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.9.0.tar` & `nonebot_plugin_bilichat-5.9.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    34523 2024-05-03 08:18:36.623330 nonebot_plugin_bilichat-5.9.0/LICENSE
--rw-r--r--   0        0        0    18173 2024-05-03 08:18:36.623330 nonebot_plugin_bilichat-5.9.0/README.md
--rw-r--r--   0        0        0     2718 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2176 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1622 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2655 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7996 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1280 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0     3916 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3848 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5196 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9296 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3210 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     5270 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     4033 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      494 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6142 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2346 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      366 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3379 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1136 2024-05-03 08:18:36.643330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7275 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3187 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3091 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1701 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1739 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     3988 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      552 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      809 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      532 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3030 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1016 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      596 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/const.py
--rw-r--r--   0        0        0     1163 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      291 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     3111 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7187 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    16423 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4894 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2243 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1578 2024-05-03 08:18:36.647330 nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1647 2024-05-03 08:18:40.095334 nonebot_plugin_bilichat-5.9.0/pyproject.toml
--rw-r--r--   0        0        0    19870 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.9.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-03 08:44:30.795784 nonebot_plugin_bilichat-5.9.1/LICENSE
+-rw-r--r--   0        0        0    18173 2024-05-03 08:44:30.795784 nonebot_plugin_bilichat-5.9.1/README.md
+-rw-r--r--   0        0        0     2718 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2176 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1622 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2655 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7996 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1280 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0     3925 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3848 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5196 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9296 2024-05-03 08:44:30.815784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3210 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     5286 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     4033 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      494 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6142 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      366 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3379 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1136 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7275 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3187 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3091 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1701 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1739 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     3988 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      552 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      809 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      532 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3030 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1016 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      596 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/const.py
+-rw-r--r--   0        0        0     1163 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      291 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     3111 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7187 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    16423 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4894 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2243 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1578 2024-05-03 08:44:30.823784 nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1647 2024-05-03 08:44:34.211783 nonebot_plugin_bilichat-5.9.1/pyproject.toml
+-rw-r--r--   0        0        0    19870 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.9.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.9.0/LICENSE` & `nonebot_plugin_bilichat-5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/README.md` & `nonebot_plugin_bilichat-5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,19 @@
     if isinstance(up, str):
         await bili_check_dyn.finish(up)
     if dyn := await fetch_last_dynamic(up):
         if image := await dyn.get_image(plugin_config.bilichat_dynamic_style):
             await UniMessage(Image(raw=image)).send(target=target)
 
 
-async def _bili_check(state: T_State, msg: UniMsg, target: MsgTarget) -> bool:
+bili_fetch_content = bilichat.command("fetch", aliases=set(plugin_config.bilichat_cmd_fetch), block=True)
+
+
+@bili_fetch_content.handle()
+async def fetch_check(state: T_State, msg: UniMsg, target: MsgTarget):
     _msgs = msg.copy()
     if Reply in msg:
         # 如果是回复消息
         # 1. 如果是自身消息且允许自身消息
         # 2. 如果被回复消息中包含对自身的at
         # 满足上述任一条件，则将被回复的消息的内容添加到待解析的内容中
         _msgs.append(Text(str(msg[Reply, 0].msg)))
@@ -52,15 +56,15 @@
         # av bv cv 格式和动态的链接
         for seg in ("av", "bv", "cv", "dynamic", "opus", "t.bilibili.com"):
             if seg in _msg_str.lower():
                 bililink = _msg_str
                 break
 
     if not bililink:
-        return False
+        raise FinishedException
 
     content: Column | Video | Dynamic | None = None
 
     try:
         ## video handle
         if matched := re.search(r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", bililink):
             _id = matched.group()
@@ -76,26 +80,19 @@
             content = await Dynamic.from_id(_id)
 
         if content:
             check_cd(f"{target.id}_-_{content.id}", check=False)
             state["_content_"] = content
         else:
             raise AbortError(f"查询 {bililink} 返回内容为空")
-
-        return True
     except AbortError as e:
         logger.info(e)
-        return False
+        raise FinishedException
     except FinishedException:
-        return False
-
-
-bili_fetch_content = bilichat.command(
-    "fetch", aliases=set(plugin_config.bilichat_cmd_fetch), rule=_bili_check, block=True
-)
+        raise FinishedException
 
 
 @bili_fetch_content.handle()
 async def fetch_content(target: MsgTarget, state: T_State):
     content: Video | Dynamic = state["_content_"]
     if isinstance(content, Video):
         raise FinishedException
```

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,16 +108,16 @@
         result = []
         # 获取图文动态中的图片
         if self.dynamic_type == DynamicType.draw:
             if self.raw_type == "web":
                 items = self.raw["modules"]["module_dynamic"]["major"]["draw"]["items"]
             elif self.raw_type == "grpc":
                 for module in self.raw["modules"]:
-                    if module["module_type"] == "module_dynamic":
-                        items = module["dynDraw"]["items"]
+                    if module["moduleType"] == "module_dynamic":
+                        items = module["moduleDynamic"]["dynDraw"]["items"]
                         break
             for item in items:
                 resq = await hc.get(item["src"])
                 result.append(resq.content)
         else:
             logger.debug(f"动态类型 {self.dynamic_type} 不是图文动态")
         return result
```

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/arguments.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/arguments.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/const.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.9.1/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.9.0/pyproject.toml` & `nonebot_plugin_bilichat-5.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.9.0"
+version = "5.9.1"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.13",
```

### Comparing `nonebot_plugin_bilichat-5.9.0/PKG-INFO` & `nonebot_plugin_bilichat-5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.9.0
+Version: 5.9.1
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.10
 Requires-Dist: bilireq>=0.2.13
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.9.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.9.1 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.10 Requires-Dist:
 bilireq>=0.2.13 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
```

