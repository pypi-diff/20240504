# Comparing `tmp/DrissionPage-4.0.4.8.tar.gz` & `tmp/DrissionPage-4.0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DrissionPage-4.0.4.8.tar", last modified: Sun Mar  3 08:28:12 2024, max compression
+gzip compressed data, was "DrissionPage-4.0.4.9.tar", last modified: Sun Mar 10 15:27:07 2024, max compression
```

## Comparing `DrissionPage-4.0.4.8.tar` & `DrissionPage-4.0.4.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.989109 DrissionPage-4.0.4.8/
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.521405 DrissionPage-4.0.4.8/DrissionPage/
--rw-rw-rw-   0        0        0      560 2024-03-03 08:27:31.000000 DrissionPage-4.0.4.8/DrissionPage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.590916 DrissionPage-4.0.4.8/DrissionPage/_base/
--rw-rw-rw-   0        0        0    18845 2024-02-27 09:16:50.000000 DrissionPage-4.0.4.8/DrissionPage/_base/base.py
--rw-rw-rw-   0        0        0     8015 2024-02-20 09:53:03.000000 DrissionPage-4.0.4.8/DrissionPage/_base/base.pyi
--rw-rw-rw-   0        0        0     9429 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_base/browser.py
--rw-rw-rw-   0        0        0     1990 2024-02-27 09:16:50.000000 DrissionPage-4.0.4.8/DrissionPage/_base/browser.pyi
--rw-rw-rw-   0        0        0    10583 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_base/driver.py
--rw-rw-rw-   0        0        0     2079 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_base/driver.pyi
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.647690 DrissionPage-4.0.4.8/DrissionPage/_configs/
--rw-rw-rw-   0        0        0    20694 2024-01-30 14:55:56.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/chromium_options.py
--rw-rw-rw-   0        0        0     5447 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/chromium_options.pyi
--rw-rw-rw-   0        0        0     1034 2024-01-26 08:44:40.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/configs.ini
--rw-rw-rw-   0        0        0     7206 2024-01-30 14:55:56.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/options_manage.py
--rw-rw-rw-   0        0        0      911 2024-01-30 14:55:56.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/options_manage.pyi
--rw-rw-rw-   0        0        0    15380 2024-01-30 14:55:56.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/session_options.py
--rw-rw-rw-   0        0        0     4122 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_configs/session_options.pyi
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.677747 DrissionPage-4.0.4.8/DrissionPage/_elements/
--rw-rw-rw-   0        0        0    66108 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_elements/chromium_element.py
--rw-rw-rw-   0        0        0    13542 2024-02-27 09:16:50.000000 DrissionPage-4.0.4.8/DrissionPage/_elements/chromium_element.pyi
--rw-rw-rw-   0        0        0     1706 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_elements/none_element.py
--rw-rw-rw-   0        0        0    18005 2024-02-20 02:27:13.000000 DrissionPage-4.0.4.8/DrissionPage/_elements/session_element.py
--rw-rw-rw-   0        0        0     4972 2024-02-08 04:20:06.000000 DrissionPage-4.0.4.8/DrissionPage/_elements/session_element.pyi
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.718123 DrissionPage-4.0.4.8/DrissionPage/_functions/
--rw-rw-rw-   0        0        0    11861 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/browser.py
--rw-rw-rw-   0        0        0      633 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/browser.pyi
--rw-rw-rw-   0        0        0      401 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/by.py
--rw-rw-rw-   0        0        0     1614 2024-01-08 12:23:06.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/cli.py
--rw-rw-rw-   0        0        0    22902 2024-01-08 22:26:56.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/keys.py
--rw-rw-rw-   0        0        0     1764 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/keys.pyi
--rw-rw-rw-   0        0        0    16010 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/locator.py
--rw-rw-rw-   0        0        0      531 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/locator.pyi
--rw-rw-rw-   0        0        0      356 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/settings.py
--rw-rw-rw-   0        0        0     8444 2024-02-09 13:45:14.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/tools.py
--rw-rw-rw-   0        0        0     1235 2024-02-09 13:45:14.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/tools.pyi
--rw-rw-rw-   0        0        0    14088 2024-02-10 14:54:44.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/web.py
--rw-rw-rw-   0        0        0     1487 2024-02-07 11:26:52.000000 DrissionPage-4.0.4.8/DrissionPage/_functions/web.pyi
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.800573 DrissionPage-4.0.4.8/DrissionPage/_pages/
--rw-rw-rw-   0        0        0    51670 2024-03-03 08:26:20.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_base.py
--rw-rw-rw-   0        0        0    10111 2024-02-10 03:15:00.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_base.pyi
--rw-rw-rw-   0        0        0    25421 2024-02-10 03:55:20.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_frame.py
--rw-rw-rw-   0        0        0     6896 2024-02-10 03:43:26.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_frame.pyi
--rw-rw-rw-   0        0        0    13243 2024-02-10 03:15:00.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_page.py
--rw-rw-rw-   0        0        0     3698 2024-02-10 03:15:00.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_page.pyi
--rw-rw-rw-   0        0        0    15998 2024-02-10 03:15:00.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_tab.py
--rw-rw-rw-   0        0        0     6663 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_tab.pyi
--rw-rw-rw-   0        0        0    15571 2024-02-08 04:20:06.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/session_page.py
--rw-rw-rw-   0        0        0     5889 2024-02-08 04:20:06.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/session_page.pyi
--rw-rw-rw-   0        0        0    17211 2024-01-29 14:50:24.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/web_page.py
--rw-rw-rw-   0        0        0     6304 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_pages/web_page.pyi
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.982363 DrissionPage-4.0.4.8/DrissionPage/_units/
--rw-rw-rw-   0        0        0    12147 2024-02-20 06:17:59.000000 DrissionPage-4.0.4.8/DrissionPage/_units/actions.py
--rw-rw-rw-   0        0        0     5004 2024-02-20 06:15:57.000000 DrissionPage-4.0.4.8/DrissionPage/_units/actions.pyi
--rw-rw-rw-   0        0        0     9354 2024-02-20 09:58:07.000000 DrissionPage-4.0.4.8/DrissionPage/_units/clicker.py
--rw-rw-rw-   0        0        0     1644 2024-02-08 01:58:42.000000 DrissionPage-4.0.4.8/DrissionPage/_units/clicker.pyi
--rw-rw-rw-   0        0        0     3675 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_units/cookies_setter.py
--rw-rw-rw-   0        0        0     1522 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_units/cookies_setter.pyi
--rw-rw-rw-   0        0        0    11519 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_units/downloader.py
--rw-rw-rw-   0        0        0     2696 2024-02-04 14:32:32.000000 DrissionPage-4.0.4.8/DrissionPage/_units/downloader.pyi
--rw-rw-rw-   0        0        0    23157 2024-02-27 09:16:50.000000 DrissionPage-4.0.4.8/DrissionPage/_units/listener.py
--rw-rw-rw-   0        0        0     7820 2024-02-04 14:32:32.000000 DrissionPage-4.0.4.8/DrissionPage/_units/listener.pyi
--rw-rw-rw-   0        0        0     8286 2024-02-10 03:21:06.000000 DrissionPage-4.0.4.8/DrissionPage/_units/rect.py
--rw-rw-rw-   0        0        0     3146 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_units/rect.pyi
--rw-rw-rw-   0        0        0     7556 2024-01-29 01:11:22.000000 DrissionPage-4.0.4.8/DrissionPage/_units/screencast.py
--rw-rw-rw-   0        0        0     1267 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_units/screencast.pyi
--rw-rw-rw-   0        0        0     6216 2024-02-10 03:21:06.000000 DrissionPage-4.0.4.8/DrissionPage/_units/scroller.py
--rw-rw-rw-   0        0        0     2300 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_units/scroller.pyi
--rw-rw-rw-   0        0        0    10364 2024-02-21 03:25:03.000000 DrissionPage-4.0.4.8/DrissionPage/_units/selector.py
--rw-rw-rw-   0        0        0     2694 2024-01-29 01:11:38.000000 DrissionPage-4.0.4.8/DrissionPage/_units/selector.pyi
--rw-rw-rw-   0        0        0    22330 2024-02-10 03:21:06.000000 DrissionPage-4.0.4.8/DrissionPage/_units/setter.py
--rw-rw-rw-   0        0        0     6729 2024-02-07 12:26:56.000000 DrissionPage-4.0.4.8/DrissionPage/_units/setter.pyi
--rw-rw-rw-   0        0        0     5540 2024-02-10 03:55:20.000000 DrissionPage-4.0.4.8/DrissionPage/_units/states.py
--rw-rw-rw-   0        0        0     2126 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.8/DrissionPage/_units/states.pyi
--rw-rw-rw-   0        0        0    22078 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_units/waiter.py
--rw-rw-rw-   0        0        0     4317 2024-03-03 07:18:11.000000 DrissionPage-4.0.4.8/DrissionPage/_units/waiter.pyi
--rw-rw-rw-   0        0        0      594 2024-02-07 11:26:52.000000 DrissionPage-4.0.4.8/DrissionPage/common.py
--rw-rw-rw-   0        0        0     2307 2024-01-12 02:54:40.000000 DrissionPage-4.0.4.8/DrissionPage/errors.py
--rw-rw-rw-   0        0        0      583 2024-01-19 03:24:28.000000 DrissionPage-4.0.4.8/DrissionPage/items.py
-drwxrwxrwx   0        0        0        0 2024-03-03 08:28:11.543710 DrissionPage-4.0.4.8/DrissionPage.egg-info/
--rw-rw-rw-   0        0        0     5379 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2701 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       84 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-03 08:28:11.000000 DrissionPage-4.0.4.8/DrissionPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1534 2020-04-26 07:01:29.000000 DrissionPage-4.0.4.8/LICENSE
--rw-rw-rw-   0        0        0      128 2024-01-05 07:17:27.000000 DrissionPage-4.0.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5379 2024-03-03 08:28:11.989109 DrissionPage-4.0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4813 2024-02-20 09:53:49.000000 DrissionPage-4.0.4.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-03 08:28:11.989109 DrissionPage-4.0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1275 2024-02-04 02:33:14.000000 DrissionPage-4.0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.749270 DrissionPage-4.0.4.9/
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.684296 DrissionPage-4.0.4.9/DrissionPage/
+-rw-rw-rw-   0        0        0      560 2024-03-09 15:33:22.000000 DrissionPage-4.0.4.9/DrissionPage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.693766 DrissionPage-4.0.4.9/DrissionPage/_base/
+-rw-rw-rw-   0        0        0    18845 2024-02-26 14:43:47.000000 DrissionPage-4.0.4.9/DrissionPage/_base/base.py
+-rw-rw-rw-   0        0        0     8015 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_base/base.pyi
+-rw-rw-rw-   0        0        0     9380 2024-03-09 15:04:25.000000 DrissionPage-4.0.4.9/DrissionPage/_base/browser.py
+-rw-rw-rw-   0        0        0     1961 2024-03-09 15:01:25.000000 DrissionPage-4.0.4.9/DrissionPage/_base/browser.pyi
+-rw-rw-rw-   0        0        0    10553 2024-03-09 15:33:22.000000 DrissionPage-4.0.4.9/DrissionPage/_base/driver.py
+-rw-rw-rw-   0        0        0     2079 2024-03-02 12:50:44.000000 DrissionPage-4.0.4.9/DrissionPage/_base/driver.pyi
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.700364 DrissionPage-4.0.4.9/DrissionPage/_configs/
+-rw-rw-rw-   0        0        0    20694 2024-01-30 14:55:55.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/chromium_options.py
+-rw-rw-rw-   0        0        0     5447 2024-01-29 01:11:36.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/chromium_options.pyi
+-rw-rw-rw-   0        0        0     1034 2024-03-02 08:12:08.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/configs.ini
+-rw-rw-rw-   0        0        0     7206 2024-01-30 14:55:55.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/options_manage.py
+-rw-rw-rw-   0        0        0      911 2024-01-30 14:55:55.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/options_manage.pyi
+-rw-rw-rw-   0        0        0    15443 2024-03-04 15:36:30.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/session_options.py
+-rw-rw-rw-   0        0        0     4127 2024-03-04 15:36:30.000000 DrissionPage-4.0.4.9/DrissionPage/_configs/session_options.pyi
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.704451 DrissionPage-4.0.4.9/DrissionPage/_elements/
+-rw-rw-rw-   0        0        0    65943 2024-03-10 15:19:36.000000 DrissionPage-4.0.4.9/DrissionPage/_elements/chromium_element.py
+-rw-rw-rw-   0        0        0    13542 2024-02-26 14:12:51.000000 DrissionPage-4.0.4.9/DrissionPage/_elements/chromium_element.pyi
+-rw-rw-rw-   0        0        0     1706 2024-01-29 01:11:36.000000 DrissionPage-4.0.4.9/DrissionPage/_elements/none_element.py
+-rw-rw-rw-   0        0        0    18360 2024-03-07 11:32:43.000000 DrissionPage-4.0.4.9/DrissionPage/_elements/session_element.py
+-rw-rw-rw-   0        0        0     4972 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_elements/session_element.pyi
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.715361 DrissionPage-4.0.4.9/DrissionPage/_functions/
+-rw-rw-rw-   0        0        0    11861 2024-03-02 08:09:03.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/browser.py
+-rw-rw-rw-   0        0        0      633 2024-01-29 01:11:36.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/browser.pyi
+-rw-rw-rw-   0        0        0      401 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/by.py
+-rw-rw-rw-   0        0        0     1614 2024-01-08 12:23:06.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/cli.py
+-rw-rw-rw-   0        0        0    22902 2024-01-08 22:26:56.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/keys.py
+-rw-rw-rw-   0        0        0     1764 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/keys.pyi
+-rw-rw-rw-   0        0        0    16010 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/locator.py
+-rw-rw-rw-   0        0        0      531 2024-01-08 12:22:36.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/locator.pyi
+-rw-rw-rw-   0        0        0      356 2024-01-29 01:11:36.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/settings.py
+-rw-rw-rw-   0        0        0     8450 2024-03-06 16:00:57.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/tools.py
+-rw-rw-rw-   0        0        0     1235 2024-03-06 16:05:31.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/tools.pyi
+-rw-rw-rw-   0        0        0    14547 2024-03-10 15:15:42.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/web.py
+-rw-rw-rw-   0        0        0     1535 2024-03-04 15:36:30.000000 DrissionPage-4.0.4.9/DrissionPage/_functions/web.pyi
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.725961 DrissionPage-4.0.4.9/DrissionPage/_pages/
+-rw-rw-rw-   0        0        0    50711 2024-03-10 15:10:57.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_base.py
+-rw-rw-rw-   0        0        0    10068 2024-03-07 11:32:43.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_base.pyi
+-rw-rw-rw-   0        0        0    25421 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_frame.py
+-rw-rw-rw-   0        0        0     6896 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_frame.pyi
+-rw-rw-rw-   0        0        0    14907 2024-03-09 15:53:31.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_page.py
+-rw-rw-rw-   0        0        0     4001 2024-03-09 15:53:31.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_page.pyi
+-rw-rw-rw-   0        0        0    15998 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_tab.py
+-rw-rw-rw-   0        0        0     6663 2024-01-29 01:11:36.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_tab.pyi
+-rw-rw-rw-   0        0        0    15598 2024-03-07 11:32:43.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/session_page.py
+-rw-rw-rw-   0        0        0     5911 2024-03-04 15:36:30.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/session_page.pyi
+-rw-rw-rw-   0        0        0    18845 2024-03-09 15:53:31.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/web_page.py
+-rw-rw-rw-   0        0        0     6846 2024-03-09 15:53:31.000000 DrissionPage-4.0.4.9/DrissionPage/_pages/web_page.pyi
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.748066 DrissionPage-4.0.4.9/DrissionPage/_units/
+-rw-rw-rw-   0        0        0    12147 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_units/actions.py
+-rw-rw-rw-   0        0        0     5004 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_units/actions.pyi
+-rw-rw-rw-   0        0        0     8863 2024-03-06 12:51:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/clicker.py
+-rw-rw-rw-   0        0        0     1644 2024-02-08 01:58:40.000000 DrissionPage-4.0.4.9/DrissionPage/_units/clicker.pyi
+-rw-rw-rw-   0        0        0     3843 2024-03-06 15:32:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/cookies_setter.py
+-rw-rw-rw-   0        0        0     1525 2024-03-06 15:32:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/cookies_setter.pyi
+-rw-rw-rw-   0        0        0    11519 2024-03-02 08:55:13.000000 DrissionPage-4.0.4.9/DrissionPage/_units/downloader.py
+-rw-rw-rw-   0        0        0     2711 2024-03-06 16:19:32.000000 DrissionPage-4.0.4.9/DrissionPage/_units/downloader.pyi
+-rw-rw-rw-   0        0        0    23173 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/listener.py
+-rw-rw-rw-   0        0        0     7825 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/listener.pyi
+-rw-rw-rw-   0        0        0     8433 2024-03-07 11:32:43.000000 DrissionPage-4.0.4.9/DrissionPage/_units/rect.py
+-rw-rw-rw-   0        0        0     3148 2024-03-07 11:32:43.000000 DrissionPage-4.0.4.9/DrissionPage/_units/rect.pyi
+-rw-rw-rw-   0        0        0     7574 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/screencast.py
+-rw-rw-rw-   0        0        0     1269 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/screencast.pyi
+-rw-rw-rw-   0        0        0     6223 2024-03-10 15:12:08.000000 DrissionPage-4.0.4.9/DrissionPage/_units/scroller.py
+-rw-rw-rw-   0        0        0     2301 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/scroller.pyi
+-rw-rw-rw-   0        0        0    10364 2024-02-26 12:28:34.000000 DrissionPage-4.0.4.9/DrissionPage/_units/selector.py
+-rw-rw-rw-   0        0        0     2694 2024-01-29 01:11:36.000000 DrissionPage-4.0.4.9/DrissionPage/_units/selector.pyi
+-rw-rw-rw-   0        0        0    22601 2024-03-06 16:10:39.000000 DrissionPage-4.0.4.9/DrissionPage/_units/setter.py
+-rw-rw-rw-   0        0        0     6706 2024-03-09 03:45:31.000000 DrissionPage-4.0.4.9/DrissionPage/_units/setter.pyi
+-rw-rw-rw-   0        0        0     5548 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/states.py
+-rw-rw-rw-   0        0        0     2128 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/states.pyi
+-rw-rw-rw-   0        0        0    22052 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/waiter.py
+-rw-rw-rw-   0        0        0     4319 2024-03-06 15:53:28.000000 DrissionPage-4.0.4.9/DrissionPage/_units/waiter.pyi
+-rw-rw-rw-   0        0        0     1889 2024-03-06 12:13:53.000000 DrissionPage-4.0.4.9/DrissionPage/common.py
+-rw-rw-rw-   0        0        0     2307 2024-01-12 02:54:40.000000 DrissionPage-4.0.4.9/DrissionPage/errors.py
+-rw-rw-rw-   0        0        0      583 2024-01-19 03:24:28.000000 DrissionPage-4.0.4.9/DrissionPage/items.py
+drwxrwxrwx   0        0        0        0 2024-03-10 15:27:07.687964 DrissionPage-4.0.4.9/DrissionPage.egg-info/
+-rw-rw-rw-   0        0        0     5379 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2701 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       84 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-10 15:27:07.000000 DrissionPage-4.0.4.9/DrissionPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1534 2024-01-08 12:17:37.000000 DrissionPage-4.0.4.9/LICENSE
+-rw-rw-rw-   0        0        0      128 2024-01-08 12:22:34.000000 DrissionPage-4.0.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5379 2024-03-10 15:27:07.749270 DrissionPage-4.0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4813 2024-02-07 11:26:51.000000 DrissionPage-4.0.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-10 15:27:07.749270 DrissionPage-4.0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2024-01-30 15:16:08.000000 DrissionPage-4.0.4.9/setup.py
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/__init__.py` & `DrissionPage-4.0.4.9/DrissionPage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from ._pages.web_page import WebPage
 
 # 启动配置类
 from ._configs.chromium_options import ChromiumOptions
 from ._configs.session_options import SessionOptions
 
 __all__ = ['ChromiumPage', 'ChromiumOptions', 'SessionOptions', 'SessionPage', 'WebPage', '__version__']
-__version__ = '4.0.4.8'
+__version__ = '4.0.4.9'
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_base/base.py` & `DrissionPage-4.0.4.9/DrissionPage/_base/base.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_base/base.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_base/base.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_base/browser.py` & `DrissionPage-4.0.4.9/DrissionPage/_base/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,44 +125,42 @@
     @property
     def tabs_count(self):
         """返回标签页数量"""
         j = self.run_cdp('Target.getTargets')['targetInfos']  # 不要改用get，避免卡死
         return len([i for i in j if i['type'] in ('page', 'webview') and not i['url'].startswith('devtools://')])
 
     @property
-    def tabs(self):
+    def tab_ids(self):
         """返回所有标签页id组成的列表"""
         j = self._driver.get(f'http://{self.address}/json').json()  # 不要改用cdp，因为顺序不对
         return [i['id'] for i in j if i['type'] in ('page', 'webview') and not i['url'].startswith('devtools://')]
 
     @property
     def process_id(self):
         """返回浏览器进程id"""
         return self._process_id
 
-    def find_tabs(self, title=None, url=None, tab_type=None, single=True):
-        """查找符合条件的tab，返回它们的id组成的列表
+    def find_tabs(self, title=None, url=None, tab_type=None):
+        """查找符合条件的tab，返回它们组成的列表
         :param title: 要匹配title的文本
         :param url: 要匹配url的文本
         :param tab_type: tab类型，可用列表输入多个
-        :param single: 是否返回首个结果的id，为False返回所有信息
-        :return: tab id或tab列表
+        :return: dict格式的tab信息列表列表
         """
         tabs = self._driver.get(f'http://{self.address}/json').json()  # 不要改用cdp
 
         if isinstance(tab_type, str):
             tab_type = {tab_type}
         elif isinstance(tab_type, (list, tuple, set)):
             tab_type = set(tab_type)
         elif tab_type is not None:
             raise TypeError('tab_type只能是set、list、tuple、str、None。')
 
-        r = [i for i in tabs if ((title is None or title in i['title']) and (url is None or url in i['url'])
-                                 and (tab_type is None or i['type'] in tab_type))]
-        return r[0]['id'] if r and single else r
+        return [i for i in tabs if ((title is None or title in i['title']) and (url is None or url in i['url'])
+                                    and (tab_type is None or i['type'] in tab_type))]
 
     def close_tab(self, tab_id):
         """关闭标签页
         :param tab_id: 标签页id
         :return: None
         """
         self._onTargetDestroyed(targetId=tab_id)
@@ -209,15 +207,18 @@
         for tab in self._all_drivers.values():
             for driver in tab:
                 driver.stop()
 
         if force:
             from psutil import Process
             for pid in pids:
-                Process(pid).kill()
+                try:
+                    Process(pid).kill()
+                except:
+                    pass
         else:
             try:
                 self.run_cdp('Browser.close')
                 self.driver.stop()
             except PageDisconnectedError:
                 self.driver.stop()
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_base/browser.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/downloader.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,91 @@
 # -*- coding:utf-8 -*-
 """
 @Author   : g1879
 @Contact  : g1879@qq.com
 @Copyright: (c) 2024 by g1879, Inc. All Rights Reserved.
 @License  : BSD 3-Clause.
 """
-from typing import List, Optional, Union, Set, Dict
+from typing import Dict, Optional, Union, Literal
 
-from .driver import BrowserDriver, Driver
+from .._base.browser import Browser
+from .._pages.chromium_base import ChromiumBase
 from .._pages.chromium_page import ChromiumPage
-from .._units.downloader import DownloadManager
 
 
-class Browser(object):
-    BROWSERS: dict = ...
-    page: ChromiumPage = ...
-    _driver: BrowserDriver = ...
-    id: str = ...
-    address: str = ...
-    _frames: dict = ...
-    _drivers: Dict[str, Driver] = ...
-    _all_drivers: Dict[str, Set[Driver]] = ...
-    _process_id: Optional[int] = ...
-    _dl_mgr: DownloadManager = ...
-    _connected: bool = ...
+class DownloadManager(object):
+    _browser: Browser = ...
+    _page: ChromiumPage = ...
+    _missions: Dict[str, DownloadMission] = ...
+    _tab_missions: dict = ...
+    _flags: dict = ...
+    _running: bool = ...
+    _save_path: Optional[str] = ...
 
-    def __new__(cls, address: str, browser_id: str, page: ChromiumPage): ...
+    def __init__(self, browser: Browser): ...
 
-    def __init__(self, address: str, browser_id: str, page: ChromiumPage): ...
+    @property
+    def missions(self) -> Dict[str, DownloadMission]: ...
 
-    def _get_driver(self, tab_id: str, owner=None) -> Driver: ...
+    def set_path(self, tab: ChromiumBase, path: str) -> None: ...
 
-    def run_cdp(self, cmd, **cmd_args) -> dict: ...
+    def set_rename(self, tab_id: str, rename: str = None, suffix: str = None) -> None: ...
 
-    @property
-    def driver(self) -> BrowserDriver: ...
+    def set_file_exists(self, tab_id: str, mode: Literal['skip', 'rename', 'overwrite', 's', 'r', 'o']) -> None: ...
 
-    @property
-    def tabs_count(self) -> int: ...
+    def set_flag(self, tab_id: str, flag: Union[bool, DownloadMission, None]) -> None: ...
 
-    @property
-    def tabs(self) -> List[str]: ...
+    def get_flag(self, tab_id: str) -> Union[bool, DownloadMission, None]: ...
 
-    @property
-    def process_id(self) -> Optional[int]: ...
+    def get_tab_missions(self, tab_id: str) -> list: ...
+
+    def set_done(self, mission: DownloadMission, state: str, final_path: str = None) -> None: ...
 
-    def find_tabs(self, title: str = None, url: str = None,
-                  tab_type: Union[str, list, tuple] = None, single: bool = True) -> Union[str, List[str]]: ...
+    def cancel(self, mission: DownloadMission) -> None: ...
 
-    def close_tab(self, tab_id: str) -> None: ...
+    def skip(self, mission: DownloadMission) -> None: ...
 
-    def stop_driver(self, driver: Driver) -> None: ...
+    def clear_tab_info(self, tab_id: str) -> None: ...
 
-    def activate_tab(self, tab_id: str) -> None: ...
+    def _onDownloadWillBegin(self, **kwargs) -> None: ...
 
-    def get_window_bounds(self, tab_id: str = None) -> dict: ...
+    def _onDownloadProgress(self, **kwargs) -> None: ...
 
-    def reconnect(self) -> None: ...
 
-    def connect_to_page(self) -> None: ...
+class TabDownloadSettings(object):
+    TABS: dict = ...
+    tab_id: str = ...
+    waiting_flag: Union[bool, dict, None] = ...
+    rename: Optional[str] = ...
+    suffix: Optional[str] = ...
+    path: Optional[str] = ...
+    when_file_exists: str = ...
 
-    def _onTargetCreated(self, **kwargs) -> None: ...
+    def __init__(self, tab_id: str): ...
 
-    def _onTargetDestroyed(self, **kwargs) -> None: ...
 
-    def quit(self, timeout: float = 5, force: bool = False) -> None: ...
+class DownloadMission(object):
+    tab_id: str = ...
+    _mgr: DownloadManager = ...
+    url: str = ...
+    id: str = ...
+    path: str = ...
+    name: str = ...
+    state: str = ...
+    total_bytes: Optional[int] = ...
+    received_bytes: int = ...
+    final_path: Optional[str] = ...
+    save_path: str = ...
+    _is_done: bool = ...
+
+    def __init__(self, mgr: DownloadManager, tab_id: str, _id: str, path: str, name: str, url: str,
+                 save_path: str): ...
+
+    @property
+    def rate(self) -> float: ...
+
+    @property
+    def is_done(self) -> bool: ...
+
+    def cancel(self) -> None: ...
 
-    def _on_disconnect(self) -> None: ...
+    def wait(self, show: bool = True, timeout=None, cancel_if_timeout=True) -> Union[bool, str]: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_base/driver.py` & `DrissionPage-4.0.4.9/DrissionPage/_base/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         :param address: 浏览器连接地址
         :param owner: 创建这个驱动的对象
         """
         self.id = tab_id
         self.address = address
         self.type = tab_type
         self.owner = owner
-        self._debug = False
+        # self._debug = False
         self.alert_flag = False  # 标记alert出现，跳过一条请求后复原
 
         self._websocket_url = f'ws://{address}/devtools/{tab_type}/{tab_id}'
         self._cur_id = 0
         self._ws = None
 
         self._recv_th = Thread(target=self._recv_loop)
@@ -176,15 +176,14 @@
             self._handle_immediate_event_th = Thread(target=self._handle_immediate_event_loop)
             self._handle_immediate_event_th.daemon = True
             self._handle_immediate_event_th.start()
 
     def run(self, _method, **kwargs):
         """执行cdp方法
         :param _method: cdp方法名
-        :param args: cdp参数
         :param kwargs: cdp参数
         :return: 执行结果
         """
         if self._stopped.is_set():
             return {'error': 'connection disconnected', 'type': 'connection_error'}
 
         timeout = kwargs.pop('_timeout', Settings.cdp_timeout)
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_base/driver.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_base/driver.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/chromium_options.py` & `DrissionPage-4.0.4.9/DrissionPage/_configs/chromium_options.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/chromium_options.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_configs/chromium_options.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/configs.ini` & `DrissionPage-4.0.4.9/DrissionPage/_configs/configs.ini`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/options_manage.py` & `DrissionPage-4.0.4.9/DrissionPage/_configs/options_manage.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/options_manage.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_configs/options_manage.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/session_options.py` & `DrissionPage-4.0.4.9/DrissionPage/_configs/session_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from pathlib import Path
 
 from requests import Session
 from requests.structures import CaseInsensitiveDict
 
 from .options_manage import OptionsManager
-from .._functions.web import cookies_to_tuple, set_session_cookies
+from .._functions.web import cookies_to_tuple, set_session_cookies, format_headers
 
 
 class SessionOptions(object):
     """requests的Session对象配置类"""
 
     def __init__(self, read_file=True, ini_path=None):
         """
@@ -167,14 +167,15 @@
         :param headers: 参数值，传入None可在ini文件标记删除
         :return: 返回当前对象
         """
         if headers is None:
             self._headers = None
             self._del_set.add('headers')
         else:
+            headers = format_headers(headers)
             self._headers = {key.lower(): headers[key] for key in headers}
         return self
 
     def set_a_header(self, name, value):
         """设置headers中一个项
         :param name: 设置名称
         :param value: 设置值
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_configs/session_options.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_configs/session_options.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def timeout(self) -> float: ...
 
     def set_timeout(self, second: float) -> SessionOptions: ...
 
     @property
     def headers(self) -> dict: ...
 
-    def set_headers(self, headers: Union[dict, None]) -> SessionOptions: ...
+    def set_headers(self, headers: Union[dict, str, None]) -> SessionOptions: ...
 
     def set_a_header(self, name: str, value: str) -> SessionOptions: ...
 
     def remove_a_header(self, name: str) -> SessionOptions: ...
 
     def clear_headers(self) -> SessionOptions: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_elements/chromium_element.py` & `DrissionPage-4.0.4.9/DrissionPage/_elements/chromium_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             return {attrs[i]: attrs[i + 1] for i in range(0, len(attrs), 2)}
         except CDPError:  # 文档根元素不能调用此方法
             return {}
 
     @property
     def text(self):
         """返回元素内所有文本，文本已格式化"""
-        return get_ele_txt(make_session_ele(self.html))
+        return get_ele_txt(make_session_ele(self))
 
     @property
     def raw_text(self):
         """返回未格式化处理的元素内文本"""
         return self.property('innerText')
 
     # -----------------d模式独有属性-------------------
@@ -443,33 +443,28 @@
 
     def s_ele(self, locator=None, index=1):
         """查找一个符合条件的元素，以SessionElement形式返回
         :param locator: 元素的定位信息，可以是loc元组，或查询字符串
         :param index: 获取第几个，从1开始，可传入负数获取倒数第几个
         :return: SessionElement对象或属性、文本
         """
-        if self.tag in __FRAME_ELEMENT__:
-            r = make_session_ele(self.inner_html, locator, index=index)
-        else:
-            r = make_session_ele(self, locator, index=index)
+        r = make_session_ele(self, locator, index=index)
         if isinstance(r, NoneElement):
             if Settings.raise_when_ele_not_found:
                 raise ElementNotFoundError(None, 's_ele()', {'locator': locator})
             else:
                 r.method = 's_ele()'
                 r.args = {'locator': locator}
         return r
 
     def s_eles(self, locator=None):
         """查找所有符合条件的元素，以SessionElement列表形式返回
         :param locator: 定位符
         :return: SessionElement或属性、文本组成的列表
         """
-        if self.tag in __FRAME_ELEMENT__:
-            return make_session_ele(self.inner_html, locator, index=None)
         return make_session_ele(self, locator, index=None)
 
     def _find_elements(self, locator, timeout=None, index=1, relative=False, raise_err=None):
         """返回当前元素下级符合条件的子元素、属性或节点文本，默认返回第一个
         :param locator: 元素的定位信息，可以是loc元组，或查询字符串
         :param timeout: 查找元素超时时间（秒）
         :param index: 第几个结果，从1开始，可传入负数获取倒数第几个，为None返回所有
@@ -501,19 +496,20 @@
                   '&& this.naturalWidth > 0 && typeof this.naturalHeight != "undefined" '
                   '&& this.naturalHeight > 0')
             end_time = perf_counter() + timeout
             while not self.run_js(js) and perf_counter() < end_time:
                 sleep(.1)
 
         src = self.attr('src')
+        if not src:
+            raise RuntimeError('元素没有src值或该值为空。')
         if src.lower().startswith('data:image'):
             if base64_to_bytes:
                 from base64 import b64decode
                 return b64decode(src.split(',', 1)[-1])
-
             else:
                 return src.split(',', 1)[-1]
 
         is_blob = src.startswith('blob')
         result = None
         end_time = perf_counter() + timeout
         while perf_counter() < end_time:
@@ -722,15 +718,15 @@
         n = self.owner.run_cdp('DOM.describeNode', nodeId=node_id)['node']
         self._tag = n['localName']
         return n['backendNodeId']
 
     def _get_ele_path(self, mode):
         """返获取绝对的css路径或xpath路径"""
         if mode == 'xpath':
-            txt1 = 'var tag = el.nodeName.toLowerCase();'
+            txt1 = 'let tag = el.nodeName.toLowerCase();'
             txt3 = ''' && sib.nodeName.toLowerCase()==tag'''
             txt4 = '''
             if(nth>1){path = '/' + tag + '[' + nth + ']' + path;}
                     else{path = '/' + tag + path;}'''
             txt5 = '''return path;'''
 
         elif mode == 'css':
@@ -741,18 +737,18 @@
 
         else:
             raise ValueError(f"mode参数只能是'xpath'或'css'，现在是：'{mode}'。")
 
         js = '''function(){
         function e(el) {
             if (!(el instanceof Element)) return;
-            var path = '';
+            let path = '';
             while (el.nodeType === Node.ELEMENT_NODE) {
                 ''' + txt1 + '''
-                    var sib = el, nth = 0;
+                    let sib = el, nth = 0;
                     while (sib) {
                         if(sib.nodeType === Node.ELEMENT_NODE''' + txt3 + '''){nth += 1;}
                         sib = sib.previousSibling;
                     }
                     ''' + txt4 + '''
                 el = el.parentNode;
             }
@@ -1075,15 +1071,15 @@
                 else:
                     nod_ids = self.owner.run_cdp('DOM.querySelectorAll',
                                                  nodeId=self._node_id, selector=loc[1])['nodeId']
                     r = make_chromium_eles(self.owner, _ids=nod_ids, index=index, is_obj_id=False)
                     return None if r is False else r
 
             else:
-                eles = make_session_ele(self.html).eles(loc)
+                eles = make_session_ele(self, loc, index=None)
                 if not eles:
                     return None
 
                 css = [i.css_path[61:] for i in eles]
                 if index is not None:
                     try:
                         node_id = self.owner.run_cdp('DOM.querySelector', nodeId=self._node_id,
@@ -1372,31 +1368,31 @@
 else if(e.singleNodeValue.constructor.name=="Attr"){return e.singleNodeValue.nodeValue;}
 else if(e.singleNodeValue.constructor.name=="Comment"){return e.singleNodeValue.nodeValue;}
 else{return e.singleNodeValue;}'''
 
     # 按顺序获取所有元素、节点或属性
     elif type_txt == '7':
         for_txt = """
-var a=new Array();
-for(var i = 0; i <e.snapshotLength ; i++){
+let a=new Array();
+for(let i = 0; i <e.snapshotLength ; i++){
 if(e.snapshotItem(i).constructor.name=="Text"){a.push(e.snapshotItem(i).data);}
 else if(e.snapshotItem(i).constructor.name=="Attr"){a.push(e.snapshotItem(i).nodeValue);}
 else if(e.snapshotItem(i).constructor.name=="Comment"){a.push(e.snapshotItem(i).nodeValue);}
 else{a.push(e.snapshotItem(i));}}"""
         return_txt = 'return a;'
 
     elif type_txt == '2':
         return_txt = 'return e.stringValue;'
     elif type_txt == '1':
         return_txt = 'return e.numberValue;'
     else:
         return_txt = 'return e.singleNodeValue;'
 
     xpath = xpath.replace(r"'", r"\'")
-    js = f'function(){{var e=document.evaluate(\'{xpath}\',{node_txt},null,{type_txt},null);\n{for_txt}\n{return_txt}}}'
+    js = f'function(){{let e=document.evaluate(\'{xpath}\',{node_txt},null,{type_txt},null);\n{for_txt}\n{return_txt}}}'
 
     return js
 
 
 def run_js(page_or_ele, script, as_expr, timeout, args=None):
     """运行javascript代码
     :param page_or_ele: 页面对象或元素对象
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_elements/chromium_element.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_elements/chromium_element.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_elements/none_element.py` & `DrissionPage-4.0.4.9/DrissionPage/_elements/none_element.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_elements/session_element.py` & `DrissionPage-4.0.4.9/DrissionPage/_elements/session_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,23 @@
     def inner_ele(self):
         return self._inner_ele
 
     def __repr__(self):
         attrs = [f"{k}='{v}'" for k, v in self.attrs.items()]
         return f'<SessionElement {self.tag} {" ".join(attrs)}>'
 
-    def __call__(self, locator, timeout=None):
+    def __call__(self, locator, index=1, timeout=None):
         """在内部查找元素
         例：ele2 = ele1('@id=ele_id')
         :param locator: 元素的定位信息，可以是loc元组，或查询字符串
+        :param index: 第几个元素，从1开始，可传入负数获取倒数第几个
         :param timeout: 不起实际作用
         :return: SessionElement对象或属性、文本
         """
-        return self.ele(locator)
+        return self.ele(locator, index=index)
 
     def __eq__(self, other):
         return self.xpath == getattr(other, 'xpath', None)
 
     @property
     def tag(self):
         """返回元素类型"""
@@ -195,20 +196,20 @@
         """
         # 获取href属性时返回绝对url
         if name == 'href':
             link = self.inner_ele.get('href')
             # 若为链接为None、js或邮件，直接返回
             if not link or link.lower().startswith(('javascript:', 'mailto:')):
                 return link
-
             else:  # 其它情况直接返回绝对url
-                return make_absolute_link(link, self.owner.url)
+                return make_absolute_link(link, self.owner.url) if self.owner else link
 
         elif name == 'src':
-            return make_absolute_link(self.inner_ele.get('src'), self.owner.url)
+            return make_absolute_link(self.inner_ele.get('src'),
+                                      self.owner.url) if self.owner else self.inner_ele.get('src')
 
         elif name == 'text':
             return self.text
 
         elif name == 'innerText':
             return self.raw_text
 
@@ -346,14 +347,18 @@
         xpath = html_or_ele.xpath
         # ChromiumElement，兼容传入的元素在iframe内的情况
         html = html_or_ele.owner.run_cdp('DOM.getOuterHTML', objectId=html_or_ele._doc_id)['outerHTML'] \
             if html_or_ele._doc_id else html_or_ele.owner.html
         html_or_ele = fromstring(html)
         html_or_ele = html_or_ele.xpath(xpath)[0]
 
+    elif html_or_ele._type == 'ChromiumFrame':
+        page = html_or_ele
+        html_or_ele = fromstring(html_or_ele.inner_html)
+
     # 各种页面对象
     elif isinstance(html_or_ele, BasePage):
         page = html_or_ele
         html = html_or_ele.html
         if html.startswith('<?xml '):
             html = sub(r'^<\?xml.*?>', '', html)
         html_or_ele = fromstring(html)
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_elements/session_element.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_elements/session_element.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/browser.py` & `DrissionPage-4.0.4.9/DrissionPage/_functions/browser.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/browser.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_functions/browser.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/cli.py` & `DrissionPage-4.0.4.9/DrissionPage/_functions/cli.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/keys.py` & `DrissionPage-4.0.4.9/DrissionPage/_functions/keys.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/keys.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_functions/keys.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/locator.py` & `DrissionPage-4.0.4.9/DrissionPage/_functions/locator.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/locator.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_functions/locator.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/tools.py` & `DrissionPage-4.0.4.9/DrissionPage/_functions/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     try:
         from win32gui import ShowWindow
         from win32con import SW_HIDE, SW_SHOW
     except ImportError:
         raise ImportError('请先安装：pip install pypiwin32')
 
-    pid = page.process_id
+    pid = page._page.process_id
     if not pid:
         return None
     hds = get_hwnds_from_pid(pid, page.title)
     sw = SW_HIDE if hide else SW_SHOW
     for hd in hds:
         ShowWindow(hd, sw)
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/tools.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_functions/tools.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @License  : BSD 3-Clause.
 """
 from os import popen
 from pathlib import Path
 from threading import Lock
 from typing import Union, Tuple
 
-from .._pages.chromium_page import ChromiumPage
+from .._pages.chromium_base import ChromiumBase
 
 
 class PortFinder(object):
     used_port: dict = ...
     lock: Lock = ...
     tmp_dir: Path = ...
 
@@ -26,15 +26,15 @@
 
 def port_is_using(ip: str, port: Union[str, int]) -> bool: ...
 
 
 def clean_folder(folder_path: Union[str, Path], ignore: Union[tuple, list] = None) -> None: ...
 
 
-def show_or_hide_browser(page: ChromiumPage, hide: bool = True) -> None: ...
+def show_or_hide_browser(page: ChromiumBase, hide: bool = True) -> None: ...
 
 
 def get_browser_progress_id(progress: Union[popen, None], address: str) -> Union[str, None]: ...
 
 
 def get_hwnds_from_pid(pid: Union[str, int], title: str) -> list: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/web.py` & `DrissionPage-4.0.4.9/DrissionPage/_functions/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 def location_in_viewport(page, loc_x, loc_y):
     """判断给定的坐标是否在视口中          |n
     :param page: ChromePage对象
     :param loc_x: 页面绝对坐标x
     :param loc_y: 页面绝对坐标y
     :return: bool
     """
-    js = f'''function(){{var x = {loc_x}; var y = {loc_y};
+    js = f'''function(){{let x = {loc_x}; let y = {loc_y};
     const scrollLeft = document.documentElement.scrollLeft;
     const scrollTop = document.documentElement.scrollTop;
     const vWidth = document.documentElement.clientWidth;
     const vHeight = document.documentElement.clientHeight;
     if (x< scrollLeft || y < scrollTop || x > vWidth + scrollLeft || y > vHeight + scrollTop){{return false;}}
     return true;}}'''
     return page.run_js(js)
@@ -338,18 +338,18 @@
     :return: 资源内容
     """
     if not url.startswith('blob'):
         raise TypeError('该链接非blob类型。')
     js = """
        function fetchData(url) {
       return new Promise((resolve, reject) => {
-        var xhr = new XMLHttpRequest();
+        let xhr = new XMLHttpRequest();
         xhr.responseType = 'blob';
         xhr.onload = function() {
-          var reader  = new FileReader();
+          let reader  = new FileReader();
           reader.onloadend = function(){resolve(reader.result);}
           reader.readAsDataURL(xhr.response);
         };
         xhr.open('GET', url, true);
         xhr.send();
       });
     }
@@ -390,7 +390,22 @@
 
                 _tree(e, new_last_one, new_body)
 
     ele = ele_or_page.s_ele()
     attrs = ' '.join([f"{k}='{v}'" for k, v in ele.attrs.items()])
     print(f'<{ele.tag} {attrs}>'.replace('\n', ' '))
     _tree(ele)
+
+
+def format_headers(txt):
+    """从浏览器复制的文本生成dict格式headers，文本用换行分隔
+    :param txt: 从浏览器复制的原始文本格式headers
+    :return: dict格式headers
+    """
+    if not isinstance(txt, str):
+        return txt
+    headers = {}
+    for header in txt.split('\n'):
+        if header:
+            name, value = header.split(': ', maxsplit=1)
+            headers[name] = value
+    return headers
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_functions/web.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_functions/web.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -48,8 +48,11 @@
 
 def is_cookie_in_driver(page: ChromiumBase, cookie: dict) -> bool: ...
 
 
 def get_blob(page: ChromiumBase, url: str, as_bytes: bool = True) -> bytes: ...
 
 
-def tree(ele_or_page:BaseParser) -> None: ...
+def tree(ele_or_page: BaseParser) -> None: ...
+
+
+def format_headers(txt: str) -> dict: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_base.py` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         self._is_reading = True
         timeout = timeout if timeout >= .5 else .5
         end_time = perf_counter() + timeout
         while perf_counter() < end_time:
             try:
                 b_id = self.run_cdp('DOM.getDocument', _timeout=timeout)['root']['backendNodeId']
                 timeout = end_time - perf_counter()
-                timeout = .5 if timeout <= 0 else timeout
+                timeout = 1 if timeout <= 1 else timeout
                 self._root_id = self.run_cdp('DOM.resolveNode', backendNodeId=b_id,
                                              _timeout=timeout)['object']['objectId']
                 result = True
                 break
 
             except:
                 timeout = end_time - perf_counter()
@@ -749,50 +749,24 @@
         return [i for i in frames if i._type == 'ChromiumFrame']
 
     def session_storage(self, item=None):
         """返回sessionStorage信息，不设置item则获取全部
         :param item: 要获取的项，不设置则返回全部
         :return: sessionStorage一个或所有项内容
         """
-        if item:
-            js = f'sessionStorage.getItem("{item}");'
-            return self.run_js_loaded(js, as_expr=True)
-        else:
-            js = '''
-            var dp_ls_len = sessionStorage.length;
-            var dp_ls_arr = new Array();
-            for(var i = 0; i < dp_ls_len; i++) {
-                var getKey = sessionStorage.key(i);
-                var getVal = sessionStorage.getItem(getKey);
-                dp_ls_arr[i] = {'key': getKey, 'val': getVal}
-            }
-            return dp_ls_arr;
-            '''
-            return {i['key']: i['val'] for i in self.run_js_loaded(js)}
+        js = f'sessionStorage.getItem("{item}")' if item else 'sessionStorage'
+        return self.run_js_loaded(js, as_expr=True)
 
     def local_storage(self, item=None):
         """返回localStorage信息，不设置item则获取全部
         :param item: 要获取的项目，不设置则返回全部
         :return: localStorage一个或所有项内容
         """
-        if item:
-            js = f'localStorage.getItem("{item}");'
-            return self.run_js_loaded(js, as_expr=True)
-        else:
-            js = '''
-            var dp_ls_len = localStorage.length;
-            var dp_ls_arr = new Array();
-            for(var i = 0; i < dp_ls_len; i++) {
-                var getKey = localStorage.key(i);
-                var getVal = localStorage.getItem(getKey);
-                dp_ls_arr[i] = {'key': getKey, 'val': getVal}
-            }
-            return dp_ls_arr;
-            '''
-            return {i['key']: i['val'] for i in self.run_js_loaded(js)}
+        js = f'localStorage.getItem("{item}")' if item else 'localStorage'
+        return self.run_js_loaded(js, as_expr=True)
 
     def get_screenshot(self, path=None, name=None, as_bytes=None, as_base64=None,
                        full_page=False, left_top=None, right_bottom=None):
         """对页面进行截图，可对整个网页、可见网页、指定范围截图。对可视范围外截图需要90以上版本浏览器支持
         :param path: 保存路径
         :param name: 完整文件名，后缀可选 'jpg','jpeg','png','webp'
         :param as_bytes: 是否以字节形式返回图片，可选 'jpg','jpeg','png','webp'，生效时path参数和as_base64参数无效
@@ -1229,15 +1203,15 @@
     r = page.run_cdp('Page.captureSnapshot')['data']
     if path is None and name is None:
         return r
     path = path or '.'
     Path(path).mkdir(parents=True, exist_ok=True)
     name = make_valid_name(name or page.title)
     with open(f'{path}{sep}{name}.mhtml', 'w', encoding='utf-8') as f:
-        f.write(r)
+        f.write(r.replace('\r\n', '\n'))
     return r
 
 
 def get_pdf(page, path=None, name=None, kwargs=None):
     """把当前页面保存为pdf文件，如果path和name参数都为None，只返回字节
     :param page: 要保存的页面对象
     :param path: 保存路径，为None且name不为None时保存在当前路径
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_base.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_base.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 @Contact  : g1879@qq.com
 @Copyright: (c) 2024 by g1879, Inc. All Rights Reserved.
 @License  : BSD 3-Clause.
 """
 from pathlib import Path
 from typing import Union, Tuple, List, Any, Optional, Literal
 
-from .chromium_tab import ChromiumTab, WebPageTab
-from .web_page import WebPage
+from .chromium_tab import ChromiumTab
 from .._base.base import BasePage
 from .._base.browser import Browser
 from .._base.driver import Driver
 from .._elements.chromium_element import ChromiumElement
 from .._elements.session_element import SessionElement
 from .._pages.chromium_frame import ChromiumFrame
 from .._pages.chromium_page import ChromiumPage
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_frame.py` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_frame.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_frame.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_frame.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_page.py` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,22 +120,22 @@
 
     @property
     def tabs_count(self):
         """返回标签页数量"""
         return self.browser.tabs_count
 
     @property
-    def tabs(self):
+    def tab_ids(self):
         """返回所有标签页id组成的列表"""
-        return self.browser.tabs
+        return self.browser.tab_ids
 
     @property
     def latest_tab(self):
-        """返回最新的标签页id，最新标签页指最后创建或最后被激活的"""
-        return self.tabs[0]
+        """返回最新的标签页对象，最新标签页指最后创建或最后被激活的"""
+        return self.get_tab(self.tab_ids[0])
 
     @property
     def process_id(self):
         """返回浏览器进程id"""
         return self.browser.process_id
 
     def save(self, path=None, name=None, as_pdf=False, **kwargs):
@@ -144,40 +144,59 @@
         :param name: 文件名，为None且path不为None时用title属性值
         :param as_pdf: 为Ture保存为pdf，否则为mhtml且忽略kwargs参数
         :param kwargs: pdf生成参数
         :return: as_pdf为True时返回bytes，否则返回文件文本
         """
         return get_pdf(self, path, name, kwargs) if as_pdf else get_mhtml(self, path, name)
 
-    def get_tab(self, id_or_num=None):
-        """获取一个标签页对象
-        :param id_or_num: 要获取的标签页id或序号，为None时获取当前tab，序号从1开始，可传入负数获取倒数第几个，不是视觉排列顺序，而是激活顺序
-        :return: 标签页对象
+    def get_tab(self, id_or_num=None, title=None, url=None, tab_type=None, as_id=False):
+        """获取一个标签页对象，id_or_num不为None时，后面几个参数无效
+        :param id_or_num: 要获取的标签页id或序号，序号从1开始，可传入负数获取倒数第几个，不是视觉排列顺序，而是激活顺序
+        :param title: 要匹配title的文本，模糊匹配，为None则匹配所有
+        :param url: 要匹配url的文本，模糊匹配，为None则匹配所有
+        :param tab_type: tab类型，可用列表输入多个，如 'page', 'iframe' 等，为None则匹配所有
+        :param as_id: 是否返回标签页id而不是标签页对象
+        :return: ChromiumTab对象
         """
-        with self._lock:
+        if id_or_num is not None:
             if isinstance(id_or_num, str):
-                return ChromiumTab(self, id_or_num)
+                id_or_num = id_or_num
             elif isinstance(id_or_num, int):
-                return ChromiumTab(self, self.tabs[id_or_num - 1 if id_or_num > 0 else id_or_num])
-            elif id_or_num is None:
-                return ChromiumTab(self, self.tab_id)
+                id_or_num = self.tab_ids[id_or_num - 1 if id_or_num > 0 else id_or_num]
             elif isinstance(id_or_num, ChromiumTab):
-                return id_or_num
+                return id_or_num.tab_id if as_id else id_or_num
+
+        elif title == url == tab_type is None:
+            id_or_num = self.tab_id
+
+        else:
+            id_or_num = self._browser.find_tabs(title, url, tab_type)
+            if id_or_num:
+                id_or_num = id_or_num[0]
             else:
-                raise TypeError(f'id_or_num需传入tab id或序号，非{id_or_num}。')
+                return None
 
-    def find_tabs(self, title=None, url=None, tab_type=None, single=True):
-        """查找符合条件的tab，返回它们的id组成的列表
-        :param title: 要匹配title的文本
-        :param url: 要匹配url的文本
-        :param tab_type: tab类型，可用列表输入多个
-        :param single: 是否返回首个结果的id，为False返回所有信息
-        :return: tab id或tab列表
+        if as_id:
+            return id_or_num
+
+        with self._lock:
+            return ChromiumTab(self, id_or_num)
+
+    def get_tabs(self, title=None, url=None, tab_type=None, as_id=False):
+        """查找符合条件的tab，返回它们组成的列表
+        :param title: 要匹配title的文本，模糊匹配，为None则匹配所有
+        :param url: 要匹配url的文本，模糊匹配，为None则匹配所有
+        :param tab_type: tab类型，可用列表输入多个，如 'page', 'iframe' 等，为None则匹配所有
+        :param as_id: 是否返回标签页id而不是标签页对象
+        :return: ChromiumTab对象组成的列表
         """
-        return self._browser.find_tabs(title, url, tab_type, single)
+        if as_id:
+            return [tab['id'] for tab in self._browser.find_tabs(title, url, tab_type)]
+        with self._lock:
+            return [ChromiumTab(self, tab['id']) for tab in self._browser.find_tabs(title, url, tab_type)]
 
     def new_tab(self, url=None, new_window=False, background=False, new_context=False):
         """新建一个标签页
         :param url: 新标签页跳转到的网址
         :param new_window: 是否在新窗口打开标签页
         :param background: 是否不激活新标签页，如new_window为True则无效
         :param new_context: 是否创建新的上下文
@@ -215,15 +234,15 @@
 
     def close_tabs(self, tabs_or_ids=None, others=False):
         """关闭传入的标签页，默认关闭当前页。可传入多个
         :param tabs_or_ids: 要关闭的标签页对象或id，可传入列表或元组，为None时关闭当前页
         :param others: 是否关闭指定标签页之外的
         :return: None
         """
-        all_tabs = set(self.tabs)
+        all_tabs = set(self.tab_ids)
         if isinstance(tabs_or_ids, str):
             tabs = {tabs_or_ids}
         elif isinstance(tabs_or_ids, ChromiumTab):
             tabs = {tabs_or_ids.tab_id}
         elif tabs_or_ids is None:
             tabs = {self.tab_id}
         elif isinstance(tabs_or_ids, (list, tuple)):
@@ -265,14 +284,30 @@
     def close_other_tabs(self, tabs_or_ids=None):
         """关闭传入的标签页以外标签页，默认保留当前页。可传入多个
         :param tabs_or_ids: 要保留的标签页对象或id，可传入列表或元组，为None时保存当前页
         :return: None
         """
         self.close_tabs(tabs_or_ids, True)
 
+    @property
+    def tabs(self):
+        """返回所有标签页id组成的列表"""
+        return self.browser.tab_ids
+
+    def find_tabs(self, title=None, url=None, tab_type=None, single=True):
+        """查找符合条件的tab，返回它们组成的列表
+        :param title: 要匹配title的文本
+        :param url: 要匹配url的文本
+        :param tab_type: tab类型，可用列表输入多个
+        :param single: 是否返回首个结果的id，为False返回所有信息
+        :return: tab id或tab列表
+        """
+        r = self._browser.find_tabs(title, url, tab_type)
+        return r[0]['id'] if r and single else r
+
 
 def handle_options(addr_or_opts):
     """设置浏览器启动属性
     :param addr_or_opts: 'ip:port'、ChromiumOptions、Driver
     :return: 返回ChromiumOptions对象
     """
     if not addr_or_opts:
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_page.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_page.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     @property
     def browser(self) -> Browser: ...
 
     @property
     def tabs_count(self) -> int: ...
 
     @property
-    def tabs(self) -> List[str]: ...
+    def tab_ids(self) -> List[str]: ...
 
     @property
     def wait(self) -> PageWaiter: ...
 
     @property
-    def latest_tab(self) -> str: ...
+    def latest_tab(self) -> Union[ChromiumTab, ChromiumPage]: ...
 
     @property
     def process_id(self) -> Optional[int]: ...
 
     @property
     def set(self) -> ChromiumPageSetter: ...
 
@@ -82,18 +82,26 @@
              pageRanges: str = ...,
              headerTemplate: str = ...,
              footerTemplate: str = ...,
              preferCSSPageSize: bool = ...,
              generateTaggedPDF: bool = ...,
              generateDocumentOutline: bool = ...) -> Union[bytes, str]: ...
 
-    def get_tab(self, tab_id: Union[str, ChromiumTab, int] = None) -> ChromiumTab: ...
-
-    def find_tabs(self, title: str = None, url: str = None,
-                  tab_type: Union[str, list, tuple] = None, single: bool = True) -> Union[str, List[str]]: ...
+    def get_tab(self,
+                id_or_num: Union[str, ChromiumTab, int] = None,
+                title: str = None,
+                url: str = None,
+                tab_type: Union[str, list, tuple] = None,
+                as_id: bool = False) -> Union[ChromiumTab, str, None]: ...
+
+    def get_tabs(self,
+                 title: str = None,
+                 url: str = None,
+                 tab_type: Union[str, list, tuple] = None,
+                 as_id: bool = False) -> Union[List[ChromiumTab], List[str]]: ...
 
     def new_tab(self, url: str = None, new_window: bool = False, background: bool = False,
                 new_context: bool = False) -> ChromiumTab: ...
 
     def _new_tab(self, new_window: bool = False, background: bool = False, new_context: bool = False) -> str: ...
 
     def close(self) -> None: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_tab.py` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_tab.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/chromium_tab.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_pages/chromium_tab.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/session_page.py` & `DrissionPage-4.0.4.9/DrissionPage/_pages/session_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from requests import Session, Response
 from requests.structures import CaseInsensitiveDict
 from tldextract import extract
 
 from .._base.base import BasePage
 from .._configs.session_options import SessionOptions
 from .._elements.session_element import SessionElement, make_session_ele
-from .._functions.web import cookie_to_dict
+from .._functions.web import cookie_to_dict, format_headers
 from .._units.setter import SessionPageSetter
 
 
 class SessionPage(BasePage):
     """SessionPage封装了页面操作的常用功能，使用requests来获取、解析网页"""
 
     def __init__(self, session_or_options=None, timeout=None):
@@ -196,15 +196,15 @@
 
     def s_ele(self, locator=None, index=1):
         """返回页面中符合条件的一个元素、属性或节点文本
         :param locator: 元素的定位信息，可以是元素对象，loc元组，或查询字符串
         :param index: 获取第几个，从1开始，可传入负数获取倒数第几个
         :return: SessionElement对象或属性、文本
         """
-        return make_session_ele(self.html) if locator is None else self._ele(locator, index=index, method='s_ele()')
+        return make_session_ele(self) if locator is None else self._ele(locator, index=index, method='s_ele()')
 
     def s_eles(self, locator):
         """返回页面中符合条件的所有元素、属性或节点文本
         :param locator: 元素的定位信息，可以是元素对象，loc元组，或查询字符串
         :return: SessionElement对象或属性、文本
         """
         return self._ele(locator, index=None)
@@ -289,15 +289,15 @@
         :param kwargs: 其它参数
         :return: tuple，第一位为Response或None，第二位为出错信息或 'Success'
         """
         kwargs = CaseInsensitiveDict(kwargs)
         if 'headers' not in kwargs:
             kwargs['headers'] = {}
         else:
-            kwargs['headers'] = CaseInsensitiveDict(kwargs['headers'])
+            kwargs['headers'] = CaseInsensitiveDict(format_headers(kwargs['headers']))
 
         # 设置referer和host值
         parsed_url = urlparse(url)
         hostname = parsed_url.hostname
         scheme = parsed_url.scheme
         if not check_headers(kwargs['headers'], self._headers, 'Referer'):
             kwargs['headers']['Referer'] = self.url if self.url else f'{scheme}://{hostname}'
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/session_page.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_pages/session_page.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             show_errmsg: bool | None = False,
             retry: int | None = None,
             interval: float | None = None,
             timeout: float | None = None,
             params: dict | None = ...,
             data: Union[dict, str, None] = ...,
             json: Union[dict, str, None] = ...,
-            headers: dict | None = ...,
+            headers: Union[dict, str, None] = ...,
             cookies: Any | None = ...,
             files: Any | None = ...,
             auth: Any | None = ...,
             allow_redirects: bool = ...,
             proxies: dict | None = ...,
             hooks: Any | None = ...,
             stream: Any | None = ...,
@@ -136,15 +136,15 @@
              show_errmsg: bool = False,
              retry: int | None = None,
              interval: float | None = None,
              data: Union[dict, str, None] = ...,
              timeout: float | None = ...,
              params: dict | None = ...,
              json: Union[dict, str, None] = ...,
-             headers: dict | None = ...,
+             headers: Union[dict, str, None] = ...,
              cookies: Any | None = ...,
              files: Any | None = ...,
              auth: Any | None = ...,
              allow_redirects: bool = ...,
              proxies: dict | None = ...,
              hooks: Any | None = ...,
              stream: Any | None = ...,
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/web_page.py` & `DrissionPage-4.0.4.9/DrissionPage/_pages/web_page.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         opts = chromium_options or driver_or_options
         return super().__new__(cls, opts)
 
     def __init__(self, mode='d', timeout=None, chromium_options=None, session_or_options=None, driver_or_options=None):
         """初始化函数
         :param mode: 'd' 或 's'，即driver模式和session模式
         :param timeout: 超时时间（秒），d模式时为寻找元素时间，s模式时为连接时间，默认10秒
-        :param chromium_options: Driver对象，只使用s模式时应传入False
+        :param chromium_options: ChromiumOptions对象，只使用s模式时应传入False
         :param session_or_options: Session对象或SessionOptions对象，只使用d模式时应传入False
         """
         if hasattr(self, '_created'):
             return
 
         self._mode = mode.lower()
         if self._mode not in ('s', 'd'):
@@ -304,29 +304,59 @@
         :return: cookies信息
         """
         if self._mode == 's':
             return super().cookies(as_dict, all_domains, all_info)
         elif self._mode == 'd':
             return super(SessionPage, self).cookies(as_dict, all_domains, all_info)
 
-    def get_tab(self, id_or_num=None):
-        """获取一个标签页对象
-        :param id_or_num: 要获取的标签页id或序号，为None时获取当前tab，序号不是视觉排列顺序，而是激活顺序
-        :return: 标签页对象
-        """
-        if isinstance(id_or_num, str):
-            return WebPageTab(self, id_or_num)
-        elif isinstance(id_or_num, int):
-            return WebPageTab(self, self.tabs[id_or_num])
-        elif id_or_num is None:
-            return WebPageTab(self, self.tab_id)
-        elif isinstance(id_or_num, WebPageTab):
-            return id_or_num
+    def get_tab(self, id_or_num=None, title=None, url=None, tab_type=None, as_id=False):
+        """获取一个标签页对象，id_or_num不为None时，后面几个参数无效
+        :param id_or_num: 要获取的标签页id或序号，序号从1开始，可传入负数获取倒数第几个，不是视觉排列顺序，而是激活顺序
+        :param title: 要匹配title的文本，模糊匹配，为None则匹配所有
+        :param url: 要匹配url的文本，模糊匹配，为None则匹配所有
+        :param tab_type: tab类型，可用列表输入多个，如 'page', 'iframe' 等，为None则匹配所有
+        :param as_id: 是否返回标签页id而不是标签页对象
+        :return: WebPageTab对象
+        """
+        if id_or_num is not None:
+            if isinstance(id_or_num, str):
+                id_or_num = id_or_num
+            elif isinstance(id_or_num, int):
+                id_or_num = self.tab_ids[id_or_num - 1 if id_or_num > 0 else id_or_num]
+            elif isinstance(id_or_num, WebPageTab):
+                return id_or_num.tab_id if as_id else id_or_num
+
+        elif title == url == tab_type is None:
+            id_or_num = self.tab_id
+
         else:
-            raise TypeError(f'id_or_num需传入tab id或序号，非{id_or_num}。')
+            id_or_num = self._browser.find_tabs(title, url, tab_type)
+            if id_or_num:
+                id_or_num = id_or_num[0]
+            else:
+                return None
+
+        if as_id:
+            return id_or_num
+
+        with self._lock:
+            return WebPageTab(self, id_or_num)
+
+    def get_tabs(self, title=None, url=None, tab_type=None, as_id=False):
+        """查找符合条件的tab，返回它们组成的列表
+        :param title: 要匹配title的文本，模糊匹配，为None则匹配所有
+        :param url: 要匹配url的文本，模糊匹配，为None则匹配所有
+        :param tab_type: tab类型，可用列表输入多个，如 'page', 'iframe' 等，为None则匹配所有
+        :param as_id: 是否返回标签页id而不是标签页对象
+        :return: ChromiumTab对象组成的列表
+        """
+        if as_id:
+            return [tab['id'] for tab in self._browser.find_tabs(title, url, tab_type)]
+        with self._lock:
+            return [WebPageTab(self, tab['id']) for tab in self._browser.find_tabs(title, url, tab_type)]
 
     def new_tab(self, url=None, new_window=False, background=False, new_context=False):
         """新建一个标签页
         :param url: 新标签页跳转到的网址
         :param new_window: 是否在新窗口打开标签页
         :param background: 是否不激活新标签页，如new_window为True则无效
         :param new_context: 是否创建新的上下文
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_pages/web_page.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_pages/web_page.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             show_errmsg: bool = False,
             retry: int | None = None,
             interval: float | None = None,
             timeout: float | None = None,
             params: dict | None = ...,
             data: Union[dict, str, None] = ...,
             json: Union[dict, str, None] = ...,
-            headers: dict | None = ...,
+            headers: Union[dict, str, None] = ...,
             cookies: Any | None = ...,
             files: Any | None = ...,
             auth: Any | None = ...,
             allow_redirects: bool = ...,
             proxies: dict | None = ...,
             hooks: Any | None = ...,
             stream: Any | None = ...,
@@ -123,15 +123,26 @@
     def cookies_to_browser(self) -> None: ...
 
     def cookies(self,
                 as_dict: bool = False,
                 all_domains: bool = False,
                 all_info: bool = False) -> Union[dict, list]: ...
 
-    def get_tab(self, id_or_num: Union[str, WebPageTab, int] = None) -> WebPageTab: ...
+    def get_tab(self,
+                id_or_num: Union[str, WebPageTab, int] = None,
+                title: str = None,
+                url: str = None,
+                tab_type: Union[str, list, tuple] = None,
+                as_id: bool = False) -> Union[WebPageTab, str, None]: ...
+
+    def get_tabs(self,
+                 title: str = None,
+                 url: str = None,
+                 tab_type: Union[str, list, tuple] = None,
+                 as_id: bool = False) -> Union[List[WebPageTab], List[str]]: ...
 
     def new_tab(self,
                 url: str = None,
                 new_window: bool = False,
                 background: bool = False,
                 new_context: bool = False) -> WebPageTab: ...
 
@@ -147,26 +158,29 @@
              data: Union[dict, str, None] = None,
              show_errmsg: bool = False,
              retry: int | None = None,
              interval: float | None = None,
              timeout: float | None = ...,
              params: dict | None = ...,
              json: Union[dict, str, None] = ...,
-             headers: dict | None = ...,
+             headers: Union[dict, str, None] = ...,
              cookies: Any | None = ...,
              files: Any | None = ...,
              auth: Any | None = ...,
              allow_redirects: bool = ...,
              proxies: dict | None = ...,
              hooks: Any | None = ...,
              stream: Any | None = ...,
              verify: Any | None = ...,
              cert: Any | None = ...) -> Union[bool, Response]: ...
 
     @property
+    def latest_tab(self) -> Union[WebPageTab, WebPage]: ...
+
+    @property
     def set(self) -> WebPageSetter: ...
 
     def _find_elements(self,
                        locator: Union[Tuple[str, str], str, ChromiumElement, SessionElement, ChromiumFrame],
                        timeout: float = None,
                        index: Optional[int] = 1,
                        relative: bool = False,
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/actions.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/actions.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/actions.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/actions.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/clicker.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/clicker.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,25 +180,14 @@
         """
         self.left(by_js=by_js)
         tid = self._ele.page.wait.new_tab()
         if not tid:
             raise RuntimeError('没有出现新标签页。')
         return self._ele.page.get_tab(tid)
 
-    def for_new_tab(self, by_js=False):
-        """点击后等待新tab出现并返回其对象
-        :param by_js: 是否使用js点击，逻辑与click()一致
-        :return: 新标签页对象，如果没有等到新标签页出现则抛出异常
-        """
-        self.left(by_js=by_js)
-        tid = self._ele.page._page.wait.new_tab()
-        if not tid:
-            raise RuntimeError('没有出现新标签页。')
-        return self._ele.page._page.get_tab(tid)
-
     def _click(self, client_x, client_y, button='left', count=1):
         """实施点击
         :param client_x: 视口中的x坐标
         :param client_y: 视口中的y坐标
         :param button: 'left' 'right' 'middle'  'back' 'forward'
         :param count: 点击次数
         :return: None
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/clicker.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/clicker.pyi`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/cookies_setter.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/cookies_setter.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,99 +7,104 @@
 """
 from http.cookiejar import Cookie
 
 from .._functions.web import set_browser_cookies, set_session_cookies
 
 
 class CookiesSetter(object):
-    def __init__(self, page):
-        self._page = page
+    def __init__(self, owner):
+        """
+        :param owner: ChromiumBase对象
+        """
+        self._owner = owner
 
     def __call__(self, cookies):
         """设置一个或多个cookie
         :param cookies: cookies信息
         :return: None
         """
         if (isinstance(cookies, dict) and 'name' in cookies and 'value' in cookies) or isinstance(cookies, Cookie):
             cookies = [cookies]
-        set_browser_cookies(self._page, cookies)
+        set_browser_cookies(self._owner, cookies)
 
     def remove(self, name, url=None, domain=None, path=None):
         """删除一个cookie
         :param name: cookie的name字段
         :param url: cookie的url字段，可选
         :param domain: cookie的domain字段，可选
         :param path: cookie的path字段，可选
         :return: None
         """
         d = {'name': name}
         if url is not None:
             d['url'] = url
         if domain is not None:
             d['domain'] = domain
+        if not url and not domain:
+            d['url'] = self._owner.url
         if path is not None:
             d['path'] = path
-        self._page.run_cdp('Network.deleteCookies', **d)
+        self._owner.run_cdp('Network.deleteCookies', **d)
 
     def clear(self):
         """清除cookies"""
-        self._page.run_cdp('Network.clearBrowserCookies')
+        self._owner.run_cdp('Network.clearBrowserCookies')
 
 
 class SessionCookiesSetter(object):
-    def __init__(self, page):
-        self._page = page
+    def __init__(self, owner):
+        self._owner = owner
 
     def __call__(self, cookies):
         """设置多个cookie，注意不要传入单个
         :param cookies: cookies信息
         :return: None
         """
         if (isinstance(cookies, dict) and 'name' in cookies and 'value' in cookies) or isinstance(cookies, Cookie):
             cookies = [cookies]
-        set_session_cookies(self._page.session, cookies)
+        set_session_cookies(self._owner.session, cookies)
 
     def remove(self, name):
         """删除一个cookie
         :param name: cookie的name字段
         :return: None
         """
-        self._page.session.cookies.set(name, None)
+        self._owner.session.cookies.set(name, None)
 
     def clear(self):
         """清除cookies"""
-        self._page.session.cookies.clear()
+        self._owner.session.cookies.clear()
 
 
 class WebPageCookiesSetter(CookiesSetter, SessionCookiesSetter):
 
     def __call__(self, cookies):
         """设置多个cookie，注意不要传入单个
         :param cookies: cookies信息
         :return: None
         """
-        if self._page.mode == 'd' and self._page._has_driver:
+        if self._owner.mode == 'd' and self._owner._has_driver:
             super().__call__(cookies)
-        elif self._page.mode == 's' and self._page._has_session:
+        elif self._owner.mode == 's' and self._owner._has_session:
             super(CookiesSetter, self).__call__(cookies)
 
     def remove(self, name, url=None, domain=None, path=None):
         """删除一个cookie
         :param name: cookie的name字段
         :param url: cookie的url字段，可选，d模式时才有效
         :param domain: cookie的domain字段，可选，d模式时才有效
         :param path: cookie的path字段，可选，d模式时才有效
         :return: None
         """
-        if self._page.mode == 'd' and self._page._has_driver:
+        if self._owner.mode == 'd' and self._owner._has_driver:
             super().remove(name, url, domain, path)
-        elif self._page.mode == 's' and self._page._has_session:
+        elif self._owner.mode == 's' and self._owner._has_session:
             if url or domain or path:
                 raise AttributeError('url、domain、path参数只有d模式下有效。')
             super(CookiesSetter, self).remove(name)
 
     def clear(self):
         """清除cookies"""
-        if self._page.mode == 'd' and self._page._has_driver:
+        if self._owner.mode == 'd' and self._owner._has_driver:
             super().clear()
-        elif self._page.mode == 's' and self._page._has_session:
+        elif self._owner.mode == 's' and self._owner._has_session:
             super(CookiesSetter, self).clear()
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/cookies_setter.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/cookies_setter.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 from .._pages.chromium_base import ChromiumBase
 from .._pages.chromium_tab import WebPageTab
 from .._pages.session_page import SessionPage
 from .._pages.web_page import WebPage
 
 
 class CookiesSetter(object):
-    _page: ChromiumBase
+    _owner: ChromiumBase
 
     def __init__(self, page: ChromiumBase): ...
 
     def __call__(self, cookies: Union[RequestsCookieJar, Cookie, list, tuple, str, dict]) -> None: ...
 
     def remove(self, name: str, url: str = None, domain: str = None, path: str = None) -> None: ...
 
     def clear(self) -> None: ...
 
 
 class SessionCookiesSetter(object):
-    _page: SessionPage
+    _owner: SessionPage
 
     def __init__(self, page: SessionPage): ...
 
     def __call__(self, cookies: Union[RequestsCookieJar, Cookie, list, tuple, str, dict]) -> None: ...
 
     def remove(self, name: str) -> None: ...
 
     def clear(self) -> None: ...
 
 
 class WebPageCookiesSetter(CookiesSetter, SessionCookiesSetter):
-    _page: Union[WebPage, WebPageTab]
+    _owner: Union[WebPage, WebPageTab]
 
     def __init__(self, page: SessionPage): ...
 
     def __call__(self, cookies: Union[RequestsCookieJar, Cookie, list, tuple, str, dict]) -> None: ...
 
     def remove(self, name: str, url: str = None, domain: str = None, path: str = None) -> None: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/downloader.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/downloader.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/downloader.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/selector.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,73 @@
 # -*- coding:utf-8 -*-
 """
 @Author   : g1879
 @Contact  : g1879@qq.com
 @Copyright: (c) 2024 by g1879, Inc. All Rights Reserved.
 @License  : BSD 3-Clause.
 """
-from typing import Dict, Optional, Union, Literal
+from typing import Union, Tuple, List
 
-from .._base.browser import Browser
-from .._pages.chromium_base import ChromiumBase
-from .._pages.chromium_page import ChromiumPage
-
-
-class DownloadManager(object):
-    _browser: Browser = ...
-    _page: ChromiumPage = ...
-    _missions: Dict[str, DownloadMission] = ...
-    _tab_missions: dict = ...
-    _flags: dict = ...
-    _running: bool = ...
-    _save_path: Optional[str] = ...
+from .._elements.chromium_element import ChromiumElement
 
-    def __init__(self, browser: Browser): ...
+
+class SelectElement(object):
+    def __init__(self, ele: ChromiumElement):
+        self._ele: ChromiumElement = ...
+
+    def __call__(self, text_or_index: Union[str, int, list, tuple], timeout: float = None) -> bool: ...
 
     @property
-    def missions(self) -> Dict[str, DownloadMission]: ...
+    def is_multi(self) -> bool: ...
 
-    def set_path(self, tab: ChromiumBase, path: str) -> None: ...
+    @property
+    def options(self) -> List[ChromiumElement]: ...
 
-    def set_rename(self, tab_id: str, rename: str = None, suffix: str = None) -> None: ...
+    @property
+    def selected_option(self) -> Union[ChromiumElement, None]: ...
 
-    def set_file_exists(self, tab_id: str, mode: Literal['rename', 'skip', 'overwrite']) -> None: ...
+    @property
+    def selected_options(self) -> List[ChromiumElement]: ...
 
-    def set_flag(self, tab_id: str, flag: Union[bool, DownloadMission, None]) -> None: ...
+    def clear(self) -> None: ...
 
-    def get_flag(self, tab_id: str) -> Union[bool, DownloadMission, None]: ...
+    def all(self) -> None: ...
 
-    def get_tab_missions(self, tab_id: str) -> list: ...
+    def by_text(self, text: Union[str, list, tuple], timeout: float = None) -> bool: ...
 
-    def set_done(self, mission: DownloadMission, state: str, final_path: str = None) -> None: ...
+    def by_value(self, value: Union[str, list, tuple], timeout: float = None) -> bool: ...
 
-    def cancel(self, mission: DownloadMission) -> None: ...
+    def by_index(self, index: Union[int, list, tuple], timeout: float = None) -> bool: ...
 
-    def skip(self, mission: DownloadMission) -> None: ...
+    def by_locator(self, locator: Union[Tuple[str, str], str], timeout: float = None) -> bool: ...
 
-    def clear_tab_info(self, tab_id: str) -> None: ...
+    def by_option(self, option: Union[ChromiumElement, List[ChromiumElement], Tuple[ChromiumElement]]) -> None: ...
 
-    def _onDownloadWillBegin(self, **kwargs) -> None: ...
+    def cancel_by_text(self, text: Union[str, list, tuple], timeout: float = None) -> bool: ...
 
-    def _onDownloadProgress(self, **kwargs) -> None: ...
+    def cancel_by_value(self, value: Union[str, list, tuple], timeout: float = None) -> bool: ...
 
+    def cancel_by_index(self, index: Union[int, list, tuple], timeout: float = None) -> bool: ...
 
-class TabDownloadSettings(object):
-    TABS: dict = ...
-    tab_id: str = ...
-    waiting_flag: Union[bool, dict, None] = ...
-    rename: Optional[str] = ...
-    suffix: Optional[str] = ...
-    path: Optional[str] = ...
-    when_file_exists: str = ...
+    def cancel_by_locator(self, locator: Union[Tuple[str, str], str], timeout: float = None) -> bool: ...
 
-    def __init__(self, tab_id: str): ...
+    def cancel_by_option(self,
+                         option: Union[ChromiumElement, List[ChromiumElement], Tuple[ChromiumElement]]) -> None: ...
 
+    def invert(self) -> None: ...
 
-class DownloadMission(object):
-    tab_id: str = ...
-    _mgr: DownloadManager = ...
-    url: str = ...
-    id: str = ...
-    path: str = ...
-    name: str = ...
-    state: str = ...
-    total_bytes: Optional[int] = ...
-    received_bytes: int = ...
-    final_path: Optional[str] = ...
-    save_path: str = ...
-    _is_done: bool = ...
+    def _by_loc(self, loc: Union[str, Tuple[str, str]], timeout: float = None, cancel: bool = False) -> bool: ...
 
-    def __init__(self, mgr: DownloadManager, tab_id: str, _id: str, path: str, name: str, url: str,
-                 save_path: str): ...
+    def _select(self,
+                condition: Union[str, int, list, tuple] = None,
+                para_type: str = 'text',
+                cancel: bool = False,
+                timeout: float = None) -> bool: ...
 
-    @property
-    def rate(self) -> float: ...
+    def _text_value(self, condition: Union[list, set], para_type: str, mode: str, timeout: float) -> bool: ...
 
-    @property
-    def is_done(self) -> bool: ...
+    def _index(self, condition: set, mode: str, timeout: float) -> bool: ...
 
-    def cancel(self) -> None: ...
+    def _select_options(self, option: Union[ChromiumElement, List[ChromiumElement], Tuple[ChromiumElement]],
+                        mode: str) -> None: ...
 
-    def wait(self, show: bool = True, timeout=None, cancel_if_timeout=True) -> Union[bool, str]: ...
+    def _dispatch_change(self) -> None: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/listener.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 from .._functions.settings import Settings
 from ..errors import WaitTimeoutError
 
 
 class Listener(object):
     """监听器基类"""
 
-    def __init__(self, page):
+    def __init__(self, owner):
         """
-        :param page: ChromiumBase对象
+        :param owner: ChromiumBase对象
         """
-        self._page = page
-        self._address = page.address
-        self._target_id = page._target_id
+        self._owner = owner
+        self._address = owner.address
+        self._target_id = owner._target_id
         self._driver = None
         self._running_requests = 0
         self._running_targets = 0
 
         self._caught = None
         self._request_ids = None
         self._extra_info_ids = None
@@ -233,24 +233,24 @@
         while perf_counter() < end_time:
             if (not targets_only and self._running_requests <= 0) or (targets_only and self._running_targets <= 0):
                 return True
             sleep(.1)
         else:
             return False
 
-    def _to_target(self, target_id, address, page):
+    def _to_target(self, target_id, address, owner):
         """切换监听的页面对象
         :param target_id: 新页面对象_target_id
         :param address: 新页面对象address
-        :param page: 新页面对象
+        :param owner: 新页面对象
         :return: None
         """
         self._target_id = target_id
         self._address = address
-        self._page = page
+        self._owner = owner
         debug = False
         if self._driver:
             debug = self._driver._debug
             self._driver.stop()
         if self.listening:
             self._driver = Driver(self._target_id, 'page', self._address)
             self._driver._debug = debug
@@ -271,29 +271,29 @@
         self._running_requests += 1
         p = None
         if self._targets is True:
             if ((self._method is True or kwargs['request']['method'] in self._method)
                     and (self._res_type is True or kwargs.get('type', '').upper() in self._res_type)):
                 self._running_targets += 1
                 rid = kwargs['requestId']
-                p = self._request_ids.setdefault(rid, DataPacket(self._page.tab_id, True))
+                p = self._request_ids.setdefault(rid, DataPacket(self._owner.tab_id, True))
                 p._raw_request = kwargs
                 if kwargs['request'].get('hasPostData', None) and not kwargs['request'].get('postData', None):
                     p._raw_post_data = self._driver.run('Network.getRequestPostData',
                                                         requestId=rid).get('postData', None)
 
         else:
             rid = kwargs['requestId']
             for target in self._targets:
                 if (((self._is_regex and search(target, kwargs['request']['url']))
                      or (not self._is_regex and target in kwargs['request']['url']))
                         and (self._method is True or kwargs['request']['method'] in self._method)
                         and (self._res_type is True or kwargs.get('type', '').upper() in self._res_type)):
                     self._running_targets += 1
-                    p = self._request_ids.setdefault(rid, DataPacket(self._page.tab_id, target))
+                    p = self._request_ids.setdefault(rid, DataPacket(self._owner.tab_id, target))
                     p._raw_request = kwargs
                     break
 
         self._extra_info_ids.setdefault(kwargs['requestId'], {})['obj'] = p if p else False
 
     def _requestWillBeSentExtraInfo(self, **kwargs):
         """接收到请求额外信息时的回调函数"""
@@ -386,21 +386,21 @@
             self._caught.put(data_packet)
             self._running_targets -= 1
 
 
 class FrameListener(Listener):
     def _requestWillBeSent(self, **kwargs):
         """接收到请求时的回调函数"""
-        if not self._page._is_diff_domain and kwargs.get('frameId', None) != self._page._frame_id:
+        if not self._owner._is_diff_domain and kwargs.get('frameId', None) != self._owner._frame_id:
             return
         super()._requestWillBeSent(**kwargs)
 
     def _response_received(self, **kwargs):
         """接收到返回信息时处理方法"""
-        if not self._page._is_diff_domain and kwargs.get('frameId', None) != self._page._frame_id:
+        if not self._owner._is_diff_domain and kwargs.get('frameId', None) != self._owner._frame_id:
             return
         super()._response_received(**kwargs)
 
 
 class DataPacket(object):
     """返回的数据包管理类"""
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/listener.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/listener.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from .._pages.chromium_frame import ChromiumFrame
 
 __RES_TYPE__ = Literal['Document', 'Stylesheet', 'Image', 'Media', 'Font', 'Script', 'TextTrack', 'XHR', 'Fetch',
 'Prefetch', 'EventSource', 'WebSocket', 'Manifest', 'SignedExchange', 'Ping', 'CSPViolationReport', 'Preflight', 'Other']
 
 
 class Listener(object):
-    def __init__(self, page: ChromiumBase):
-        self._page: ChromiumBase = ...
+    def __init__(self, owner: ChromiumBase):
+        self._owner: ChromiumBase = ...
         self._address: str = ...
         self._target_id: str = ...
         self._targets: Union[str, dict, None] = ...
         self._method: set = ...
         self._res_type: set = ...
         self._caught: Queue = ...
         self._is_regex: bool = ...
@@ -65,15 +65,15 @@
     @property
     def results(self) -> Union[DataPacket, Dict[str, List[DataPacket]], False]: ...
 
     def clear(self) -> None: ...
 
     def wait_silent(self, timeout: float = None, targets_only: bool = False) -> bool: ...
 
-    def _to_target(self, target_id: str, address: str, page: ChromiumBase) -> None: ...
+    def _to_target(self, target_id: str, address: str, owner: ChromiumBase) -> None: ...
 
     def _requestWillBeSent(self, **kwargs) -> None: ...
 
     def _requestWillBeSentExtraInfo(self, **kwargs) -> None: ...
 
     def _response_received(self, **kwargs) -> None: ...
 
@@ -88,16 +88,16 @@
               timeout: float = None,
               gap=1) -> Iterable[Union[DataPacket, List[DataPacket]]]: ...
 
     def _set_callback(self) -> None: ...
 
 
 class FrameListener(Listener):
-    def __init__(self, page: ChromiumFrame):
-        self._page: ChromiumFrame = ...
+    def __init__(self, owner: ChromiumFrame):
+        self._owner: ChromiumFrame = ...
         self._is_diff: bool = ...
 
 
 class DataPacket(object):
     """返回的数据包管理类"""
 
     def __init__(self, tab_id: str, target: [str, bool]):
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/rect.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/rect.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,20 +109,23 @@
         r = self._ele.owner.run_cdp_loaded('Page.getLayoutMetrics')['visualViewport']
         sx = r['pageX']
         sy = r['pageY']
         return x + sx, y + sy
 
 
 class TabRect(object):
-    def __init__(self, page):
-        self._page = page
+    def __init__(self, owner):
+        """
+        :param owner: Page对象和Tab对象
+        """
+        self._owner = owner
 
     @property
     def window_state(self):
-        """返回窗口状态：normal、fullscreen、maximized、 minimized"""
+        """返回窗口状态：normal、fullscreen、maximized、minimized"""
         return self._get_window_rect()['windowState']
 
     @property
     def window_location(self):
         """返回窗口在屏幕上的坐标，左上角为(0, 0)"""
         r = self._get_window_rect()
         if r['windowState'] in ('maximized', 'fullscreen'):
@@ -166,31 +169,34 @@
         """返回视口宽高，不包括滚动条，格式：(宽, 高)"""
         r = self._get_page_rect()['visualViewport']
         return r['clientWidth'], r['clientHeight']
 
     @property
     def viewport_size_with_scrollbar(self):
         """返回视口宽高，包括滚动条，格式：(宽, 高)"""
-        r = self._page.run_js('return window.innerWidth.toString() + " " + window.innerHeight.toString();')
+        r = self._owner.run_js('return window.innerWidth.toString() + " " + window.innerHeight.toString();')
         w, h = r.split(' ')
         return int(w), int(h)
 
     def _get_page_rect(self):
         """获取页面范围信息"""
-        return self._page.run_cdp_loaded('Page.getLayoutMetrics')
+        return self._owner.run_cdp_loaded('Page.getLayoutMetrics')
 
     def _get_window_rect(self):
         """获取窗口范围信息"""
-        return self._page.browser.get_window_bounds(self._page.tab_id)
+        return self._owner.browser.get_window_bounds(self._owner.tab_id)
 
 
 class FrameRect(object):
     """异域iframe使用"""
 
     def __init__(self, frame):
+        """
+        :param frame: ChromiumFrame对象
+        """
         self._frame = frame
 
     @property
     def location(self):
         """返回iframe元素左上角的绝对坐标"""
         return self._frame.frame_ele.rect.location
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/rect.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/rect.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
     def _get_viewport_rect(self, quad: str) -> Union[list, None]: ...
 
     def _get_page_coord(self, x: float, y: float) -> Tuple[float, float]: ...
 
 
 class TabRect(object):
-    def __init__(self, page: ChromiumBase):
-        self._page: Union[ChromiumPage, ChromiumTab, WebPage, WebPageTab] = ...
+    def __init__(self, owner: ChromiumBase):
+        self._owner: Union[ChromiumPage, ChromiumTab, WebPage, WebPageTab] = ...
 
     @property
     def window_state(self) -> str: ...
 
     @property
     def window_location(self) -> Tuple[int, int]: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/screencast.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/screencast.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from shutil import rmtree
 from tempfile import gettempdir
 from threading import Thread
 from time import sleep, time
 
 
 class Screencast(object):
-    def __init__(self, page):
-        self._page = page
+    def __init__(self, owner):
+        self._owner = owner
         self._path = None
         self._tmp_path = None
         self._running = False
         self._enable = False
         self._mode = 'video'
 
     @property
@@ -35,24 +35,24 @@
         :return: None
         """
         self.set_save_path(save_path)
         if self._path is None:
             raise ValueError('save_path必须设置。')
 
         if self._mode in ('frugal_video', 'video'):
-            if self._page.browser.page._chromium_options.tmp_path:
+            if self._owner.browser.page._chromium_options.tmp_path:
                 self._tmp_path = Path(
-                    self._page.browser.page._chromium_options.tmp_path) / f'screencast_tmp_{time()}_{randint(0, 100)}'
+                    self._owner.browser.page._chromium_options.tmp_path) / f'screencast_tmp_{time()}_{randint(0, 100)}'
             else:
                 self._tmp_path = Path(gettempdir()) / 'DrissionPage' / f'screencast_tmp_{time()}_{randint(0, 100)}'
             self._tmp_path.mkdir(parents=True, exist_ok=True)
 
         if self._mode.startswith('frugal'):
-            self._page.driver.set_callback('Page.screencastFrame', self._onScreencastFrame)
-            self._page.run_cdp('Page.startScreencast', everyNthFrame=1, quality=100)
+            self._owner.driver.set_callback('Page.screencastFrame', self._onScreencastFrame)
+            self._owner.run_cdp('Page.startScreencast', everyNthFrame=1, quality=100)
 
         elif not self._mode.startswith('js'):
             self._running = True
             self._enable = True
             Thread(target=self._run).start()
 
         else:  # js模式
@@ -75,41 +75,41 @@
                     while(DrissionPage_Screencast_blob_ok==false){}
                     DrissionPage_Screencast_blob = new Blob(DrissionPage_Screencast_chunks, 
                                                             {type: DrissionPage_Screencast_chunks[0].type});
                 })
               }
             '''
             print('请手动选择要录制的目标。')
-            self._page.run_js('var DrissionPage_Screencast_blob;var DrissionPage_Screencast_blob_ok=false;')
-            self._page.run_js(js)
+            self._owner.run_js('var DrissionPage_Screencast_blob;var DrissionPage_Screencast_blob_ok=false;')
+            self._owner.run_js(js)
 
     def stop(self, video_name=None):
         """停止录屏
         :param video_name: 视频文件名，为None时以当前时间名命
         :return: 文件路径
         """
         if video_name and not video_name.endswith('mp4'):
             video_name = f'{video_name}.mp4'
         name = f'{time()}.mp4' if not video_name else video_name
         path = f'{self._path}{sep}{name}'
 
         if self._mode.startswith('js'):
-            self._page.run_js('mediaRecorder.stop();', as_expr=True)
-            while not self._page.run_js('return DrissionPage_Screencast_blob_ok;'):
+            self._owner.run_js('mediaRecorder.stop();', as_expr=True)
+            while not self._owner.run_js('return DrissionPage_Screencast_blob_ok;'):
                 sleep(.1)
-            blob = self._page.run_js('return DrissionPage_Screencast_blob;')
-            uuid = self._page.run_cdp('IO.resolveBlob', objectId=blob['result']['objectId'])['uuid']
-            data = self._page.run_cdp('IO.read', handle=f'blob:{uuid}')['data']
+            blob = self._owner.run_js('return DrissionPage_Screencast_blob;')
+            uuid = self._owner.run_cdp('IO.resolveBlob', objectId=blob['result']['objectId'])['uuid']
+            data = self._owner.run_cdp('IO.read', handle=f'blob:{uuid}')['data']
             with open(path, 'wb') as f:
                 f.write(b64decode(data))
             return path
 
         if self._mode.startswith('frugal'):
-            self._page.driver.set_callback('Page.screencastFrame', None)
-            self._page.run_cdp('Page.stopScreencast')
+            self._owner.driver.set_callback('Page.screencastFrame', None)
+            self._owner.run_cdp('Page.stopScreencast')
         else:
             self._enable = False
             while self._running:
                 sleep(.1)
 
         if self._mode.endswith('imgs'):
             return str(Path(self._path).absolute())
@@ -151,24 +151,24 @@
             self._path = save_path
 
     def _run(self):
         """非节俭模式运行方法"""
         self._running = True
         path = self._tmp_path or self._path
         while self._enable:
-            self._page.get_screenshot(path=path, name=f'{time()}.jpg')
+            self._owner.get_screenshot(path=path, name=f'{time()}.jpg')
             sleep(.04)
         self._running = False
 
     def _onScreencastFrame(self, **kwargs):
         """节俭模式运行方法"""
         path = self._tmp_path or self._path
         with open(f'{path}{sep}{kwargs["metadata"]["timestamp"]}.jpg', 'wb') as f:
             f.write(b64decode(kwargs['data']))
-        self._page.run_cdp('Page.screencastFrameAck', sessionId=kwargs['sessionId'])
+        self._owner.run_cdp('Page.screencastFrameAck', sessionId=kwargs['sessionId'])
 
 
 class ScreencastMode(object):
     def __init__(self, screencast):
         self._screencast = screencast
 
     def video_mode(self):
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/screencast.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/screencast.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from pathlib import Path
 from typing import Union
 
 from .._pages.chromium_base import ChromiumBase
 
 
 class Screencast(object):
-    def __init__(self, page: ChromiumBase):
-        self._page: ChromiumBase = ...
+    def __init__(self, owner: ChromiumBase):
+        self._owner: ChromiumBase = ...
         self._path: Path = ...
         self._tmp_path: Path = ...
         self._running: bool = ...
         self._enable: bool = ...
         self._mode: str = ...
 
     @property
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/scroller.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/scroller.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,23 +83,23 @@
         self._run_js(f'{{}}.scrollBy({pixel}, 0);')
 
     def _wait_scrolled(self):
         """等待滚动结束"""
         if not self._wait_complete:
             return
 
-        page = self._driver.owner if self._driver._type == 'ChromiumElement' else self._driver
-        r = page.run_cdp('Page.getLayoutMetrics')
+        owner = self._driver.owner if self._driver._type == 'ChromiumElement' else self._driver
+        r = owner.run_cdp('Page.getLayoutMetrics')
         x = r['layoutViewport']['pageX']
         y = r['layoutViewport']['pageY']
 
-        end_time = perf_counter() + page.timeout
+        end_time = perf_counter() + owner.timeout
         while perf_counter() < end_time:
             sleep(.1)
-            r = page.run_cdp('Page.getLayoutMetrics')
+            r = owner.run_cdp('Page.getLayoutMetrics')
             x1 = r['layoutViewport']['pageX']
             y1 = r['layoutViewport']['pageY']
 
             if x == x1 and y == y1:
                 break
 
             x = x1
@@ -116,19 +116,19 @@
 
     def to_center(self):
         """元素尽量滚动到视口中间"""
         self._driver.owner.scroll.to_see(self._driver, center=True)
 
 
 class PageScroller(Scroller):
-    def __init__(self, page):
+    def __init__(self, owner):
         """
-        :param page: 页面对象
+        :param owner: 页面对象
         """
-        super().__init__(page)
+        super().__init__(owner)
         self.t1 = 'window'
         self.t2 = 'document.documentElement'
 
     def to_see(self, loc_or_ele, center=None):
         """滚动页面直到元素可见
         :param loc_or_ele: 元素的定位信息，可以是loc元组，或查询字符串
         :param center: 是否尽量滚动到页面正中，为None时如果被遮挡，则滚动到页面正中
@@ -142,15 +142,15 @@
         :param ele: 元素对象
         :param center: 是否尽量滚动到页面正中，为None时如果被遮挡，则滚动到页面正中
         :return: None
         """
         txt = 'true' if center else 'false'
         ele.run_js(f'this.scrollIntoViewIfNeeded({txt});')
         if center or (center is not False and ele.states.is_covered):
-            ele.run_js('''function getWindowScrollTop() {var scroll_top = 0;
+            ele.run_js('''function getWindowScrollTop() {let scroll_top = 0;
                     if (document.documentElement && document.documentElement.scrollTop) {
                       scroll_top = document.documentElement.scrollTop;
                     } else if (document.body) {scroll_top = document.body.scrollTop;}
                     return scroll_top;}
             const { top, height } = this.getBoundingClientRect();
                     const elCenter = top + height / 2;
                     const center = window.innerHeight / 2;
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/scroller.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/scroller.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def to_see(self, center: Union[bool, None] = None) -> None: ...
 
     def to_center(self) -> None: ...
 
 
 class PageScroller(Scroller):
-    def __init__(self, page: ChromiumBase): ...
+    def __init__(self, owner: ChromiumBase): ...
 
     def to_see(self, loc_or_ele: Union[str, tuple, ChromiumElement], center: Union[bool, None] = None) -> None: ...
 
     def _to_see(self, ele: ChromiumElement, center: Union[bool, None]) -> None: ...
 
 
 class FrameScroller(PageScroller):
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/selector.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/selector.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/setter.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/setter.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,444 +8,449 @@
 from pathlib import Path
 from time import sleep
 
 from requests.structures import CaseInsensitiveDict
 
 from .cookies_setter import SessionCookiesSetter, CookiesSetter, WebPageCookiesSetter
 from .._functions.tools import show_or_hide_browser
+from .._functions.web import format_headers
 
 
 class BasePageSetter(object):
-    def __init__(self, page):
-        self._page = page
+    def __init__(self, owner):
+        """
+        :param owner: BasePage对象
+        """
+        self._owner = owner
 
     def NoneElement_value(self, value=None, on_off=True):
         """设置空元素是否返回设定值
         :param value: 返回的设定值
         :param on_off: 是否启用
         :return: None
         """
-        self._page._none_ele_return_value = on_off
-        self._page._none_ele_value = value
+        self._owner._none_ele_return_value = on_off
+        self._owner._none_ele_value = value
 
 
 class ChromiumBaseSetter(BasePageSetter):
-    def __init__(self, page):
-        super().__init__(page)
+    def __init__(self, owner):
+        """
+        :param owner: ChromiumBase对象
+        """
+        super().__init__(owner)
         self._cookies_setter = None
 
     @property
     def load_mode(self):
         """返回用于设置页面加载策略的对象"""
-        return LoadMode(self._page)
+        return LoadMode(self._owner)
 
     @property
     def scroll(self):
         """返回用于设置页面滚动设置的对象"""
-        return PageScrollSetter(self._page.scroll)
+        return PageScrollSetter(self._owner.scroll)
 
     @property
     def cookies(self):
         """返回用于设置cookies的对象"""
         if self._cookies_setter is None:
-            self._cookies_setter = CookiesSetter(self._page)
+            self._cookies_setter = CookiesSetter(self._owner)
         return self._cookies_setter
 
     def retry_times(self, times):
         """设置连接失败重连次数"""
-        self._page.retry_times = times
+        self._owner.retry_times = times
 
     def retry_interval(self, interval):
         """设置连接失败重连间隔"""
-        self._page.retry_interval = interval
+        self._owner.retry_interval = interval
 
     def timeouts(self, base=None, page_load=None, script=None, implicit=None):
         """设置超时时间，单位为秒
         :param base: 基本等待时间，除页面加载和脚本超时，其它等待默认使用
         :param page_load: 页面加载超时时间
         :param script: 脚本运行超时时间
         :return: None
         """
         base = base if base is not None else implicit
         if base is not None:
-            self._page.timeouts.base = base
-            self._page._timeout = base
+            self._owner.timeouts.base = base
+            self._owner._timeout = base
 
         if page_load is not None:
-            self._page.timeouts.page_load = page_load
+            self._owner.timeouts.page_load = page_load
 
         if script is not None:
-            self._page.timeouts.script = script
+            self._owner.timeouts.script = script
 
     def user_agent(self, ua, platform=None):
         """为当前tab设置user agent，只在当前tab有效
         :param ua: user agent字符串
         :param platform: platform字符串
         :return: None
         """
         keys = {'userAgent': ua}
         if platform:
             keys['platform'] = platform
-        self._page.run_cdp('Emulation.setUserAgentOverride', **keys)
+        self._owner.run_cdp('Emulation.setUserAgentOverride', **keys)
 
     def session_storage(self, item, value):
         """设置或删除某项sessionStorage信息
         :param item: 要设置的项
         :param value: 项的值，设置为False时，删除该项
         :return: None
         """
-        self._page.run_cdp_loaded('DOMStorage.enable')
-        i = self._page.run_cdp('Storage.getStorageKeyForFrame', frameId=self._page._frame_id)['storageKey']
+        self._owner.run_cdp_loaded('DOMStorage.enable')
+        i = self._owner.run_cdp('Storage.getStorageKeyForFrame', frameId=self._owner._frame_id)['storageKey']
         if value is False:
-            self._page.run_cdp('DOMStorage.removeDOMStorageItem',
-                               storageId={'storageKey': i, 'isLocalStorage': False}, key=item)
+            self._owner.run_cdp('DOMStorage.removeDOMStorageItem',
+                                storageId={'storageKey': i, 'isLocalStorage': False}, key=item)
         else:
-            self._page.run_cdp('DOMStorage.setDOMStorageItem', storageId={'storageKey': i, 'isLocalStorage': False},
-                               key=item, value=value)
-        self._page.run_cdp_loaded('DOMStorage.disable')
+            self._owner.run_cdp('DOMStorage.setDOMStorageItem', storageId={'storageKey': i, 'isLocalStorage': False},
+                                key=item, value=value)
+        self._owner.run_cdp_loaded('DOMStorage.disable')
 
     def local_storage(self, item, value):
         """设置或删除某项localStorage信息
         :param item: 要设置的项
         :param value: 项的值，设置为False时，删除该项
         :return: None
         """
-        self._page.run_cdp_loaded('DOMStorage.enable')
-        i = self._page.run_cdp('Storage.getStorageKeyForFrame', frameId=self._page._frame_id)['storageKey']
+        self._owner.run_cdp_loaded('DOMStorage.enable')
+        i = self._owner.run_cdp('Storage.getStorageKeyForFrame', frameId=self._owner._frame_id)['storageKey']
         if value is False:
-            self._page.run_cdp('DOMStorage.removeDOMStorageItem',
-                               storageId={'storageKey': i, 'isLocalStorage': True}, key=item)
+            self._owner.run_cdp('DOMStorage.removeDOMStorageItem',
+                                storageId={'storageKey': i, 'isLocalStorage': True}, key=item)
         else:
-            self._page.run_cdp('DOMStorage.setDOMStorageItem', storageId={'storageKey': i, 'isLocalStorage': True},
-                               key=item, value=value)
-        self._page.run_cdp_loaded('DOMStorage.disable')
+            self._owner.run_cdp('DOMStorage.setDOMStorageItem', storageId={'storageKey': i, 'isLocalStorage': True},
+                                key=item, value=value)
+        self._owner.run_cdp_loaded('DOMStorage.disable')
 
     def upload_files(self, files):
         """等待上传的文件路径
         :param files: 文件路径列表或字符串，字符串时多个文件用回车分隔
         :return: None
         """
-        if not self._page._upload_list:
-            self._page.driver.set_callback('Page.fileChooserOpened', self._page._onFileChooserOpened)
-            self._page.run_cdp('Page.setInterceptFileChooserDialog', enabled=True)
+        if not self._owner._upload_list:
+            self._owner.driver.set_callback('Page.fileChooserOpened', self._owner._onFileChooserOpened)
+            self._owner.run_cdp('Page.setInterceptFileChooserDialog', enabled=True)
 
         if isinstance(files, str):
             files = files.split('\n')
         elif isinstance(files, Path):
-            files = (files, )
-        self._page._upload_list = [str(Path(i).absolute()) for i in files]
+            files = (files,)
+        self._owner._upload_list = [str(Path(i).absolute()) for i in files]
 
-    def headers(self, headers: dict) -> None:
+    def headers(self, headers) -> None:
         """设置固定发送的headers
         :param headers: dict格式的headers数据
         :return: None
         """
-        self._page.run_cdp('Network.enable')
-        self._page.run_cdp('Network.setExtraHTTPHeaders', headers=headers)
+        self._owner.run_cdp('Network.enable')
+        self._owner.run_cdp('Network.setExtraHTTPHeaders', headers=format_headers(headers))
 
     def auto_handle_alert(self, on_off=True, accept=True):
         """设置是否启用自动处理弹窗
         :param on_off: bool表示开或关
         :param accept: bool表示确定还是取消
         :return: None
         """
-        self._page._alert.auto = accept if on_off else None
+        self._owner._alert.auto = accept if on_off else None
 
     def blocked_urls(self, urls):
         """设置要忽略的url
         :param urls: 要忽略的url，可用*通配符，可输入多个，传入None时清空已设置的内容
         :return: None
         """
         if not urls:
             urls = []
         elif isinstance(urls, str):
             urls = (urls,)
         if not isinstance(urls, (list, tuple)):
             raise TypeError('urls需传入str、list或tuple类型。')
-        self._page.run_cdp('Network.enable')
-        self._page.run_cdp('Network.setBlockedURLs', urls=urls)
+        self._owner.run_cdp('Network.enable')
+        self._owner.run_cdp('Network.setBlockedURLs', urls=urls)
 
     # --------------即将废弃---------------
 
     @property
     def load_strategy(self):
         """返回用于设置页面加载策略的对象"""
-        return LoadMode(self._page)
+        return LoadMode(self._owner)
 
 
 class TabSetter(ChromiumBaseSetter):
-    def __init__(self, page):
-        super().__init__(page)
+    def __init__(self, owner):
+        """
+        :param owner: 标签页对象
+        """
+        super().__init__(owner)
 
     @property
     def window(self):
         """返回用于设置浏览器窗口的对象"""
-        return WindowSetter(self._page)
+        return WindowSetter(self._owner)
 
     def download_path(self, path):
         """设置下载路径
         :param path: 下载路径
         :return: None
         """
         path = str(Path(path).absolute())
-        self._page._download_path = path
-        self._page.browser._dl_mgr.set_path(self._page, path)
-        if self._page._DownloadKit:
-            self._page._DownloadKit.set.goal_path(path)
+        self._owner._download_path = path
+        self._owner.browser._dl_mgr.set_path(self._owner, path)
+        if self._owner._DownloadKit:
+            self._owner._DownloadKit.set.goal_path(path)
 
     def download_file_name(self, name=None, suffix=None):
         """设置下一个被下载文件的名称
         :param name: 文件名，可不含后缀，会自动使用远程文件后缀
         :param suffix: 后缀名，显式设置后缀名，不使用远程文件后缀
         :return: None
         """
-        self._page.browser._dl_mgr.set_rename(self._page.tab_id, name, suffix)
+        self._owner.browser._dl_mgr.set_rename(self._owner.tab_id, name, suffix)
 
     def when_download_file_exists(self, mode):
         """设置当存在同名文件时的处理方式
         :param mode: 可在 'rename', 'overwrite', 'skip', 'r', 'o', 's'中选择
         :return: None
         """
         types = {'rename': 'rename', 'overwrite': 'overwrite', 'skip': 'skip', 'r': 'rename', 'o': 'overwrite',
                  's': 'skip'}
         mode = types.get(mode, mode)
         if mode not in types:
             raise ValueError(f'''mode参数只能是 '{"', '".join(types.keys())}' 之一，现在是：{mode}''')
 
-        self._page.browser._dl_mgr.set_file_exists(self._page.tab_id, mode)
+        self._owner.browser._dl_mgr.set_file_exists(self._owner.tab_id, mode)
 
     def activate(self):
         """使标签页处于最前面"""
-        self._page.browser.activate_tab(self._page.tab_id)
+        self._owner.browser.activate_tab(self._owner.tab_id)
 
 
 class ChromiumPageSetter(TabSetter):
 
     def tab_to_front(self, tab_or_id=None):
         """激活标签页使其处于最前面
         :param tab_or_id: 标签页对象或id，为None表示当前标签页
         :return: None
         """
         if not tab_or_id:
-            tab_or_id = self._page.tab_id
+            tab_or_id = self._owner.tab_id
         elif not isinstance(tab_or_id, str):  # 传入Tab对象
             tab_or_id = tab_or_id.tab_id
-        self._page.browser.activate_tab(tab_or_id)
-
-    @property
-    def window(self):
-        """返回用于设置浏览器窗口的对象"""
-        return PageWindowSetter(self._page)
+        self._owner.browser.activate_tab(tab_or_id)
 
 
 class SessionPageSetter(BasePageSetter):
-    def __init__(self, page):
+    def __init__(self, owner):
         """
-        :param page: SessionPage对象
+        :param owner: SessionPage对象
         """
-        super().__init__(page)
+        super().__init__(owner)
         self._cookies_setter = None
 
     @property
     def cookies(self):
         """返回用于设置cookies的对象"""
         if self._cookies_setter is None:
-            self._cookies_setter = SessionCookiesSetter(self._page)
+            self._cookies_setter = SessionCookiesSetter(self._owner)
         return self._cookies_setter
 
     def retry_times(self, times):
         """设置连接失败时重连次数"""
-        self._page.retry_times = times
+        self._owner.retry_times = times
 
     def retry_interval(self, interval):
         """设置连接失败时重连间隔"""
-        self._page.retry_interval = interval
+        self._owner.retry_interval = interval
 
     def download_path(self, path):
         """设置下载路径
         :param path: 下载路径
         :return: None
         """
         path = str(Path(path).absolute())
-        self._page._download_path = path
-        if self._page._DownloadKit:
-            self._page._DownloadKit.set.goal_path(path)
+        self._owner._download_path = path
+        if self._owner._DownloadKit:
+            self._owner._DownloadKit.set.goal_path(path)
 
     def timeout(self, second):
         """设置连接超时时间
         :param second: 秒数
         :return: None
         """
-        self._page.timeout = second
+        self._owner.timeout = second
 
     def encoding(self, encoding, set_all=True):
         """设置编码
         :param encoding: 编码名称，如果要取消之前的设置，传入None
         :param set_all: 是否设置对象参数，为False则只设置当前Response
         :return: None
         """
         if set_all:
-            self._page._encoding = encoding if encoding else None
-        if self._page.response:
-            self._page.response.encoding = encoding
+            self._owner._encoding = encoding if encoding else None
+        if self._owner.response:
+            self._owner.response.encoding = encoding
 
     def headers(self, headers):
         """设置通用的headers
         :param headers: dict形式的headers
         :return: None
         """
-        self._page._headers = CaseInsensitiveDict(headers)
+        self._owner._headers = CaseInsensitiveDict(format_headers(headers))
 
     def header(self, name, value):
         """设置headers中一个项
         :param name: 设置名称
         :param value: 设置值
         :return: None
         """
-        self._page._headers[name] = value
+        self._owner._headers[name] = value
 
     def user_agent(self, ua):
         """设置user agent
         :param ua: user agent
         :return: None
         """
-        self._page._headers['user-agent'] = ua
+        self._owner._headers['user-agent'] = ua
 
     def proxies(self, http=None, https=None):
         """设置proxies参数
         :param http: http代理地址
         :param https: https代理地址
         :return: None
         """
-        self._page.session.proxies = {'http': http, 'https': https}
+        self._owner.session.proxies = {'http': http, 'https': https}
 
     def auth(self, auth):
         """设置认证元组或对象
         :param auth: 认证元组或对象
         :return: None
         """
-        self._page.session.auth = auth
+        self._owner.session.auth = auth
 
     def hooks(self, hooks):
         """设置回调方法
         :param hooks: 回调方法
         :return: None
         """
-        self._page.session.hooks = hooks
+        self._owner.session.hooks = hooks
 
     def params(self, params):
         """设置查询参数字典
         :param params: 查询参数字典
         :return: None
         """
-        self._page.session.params = params
+        self._owner.session.params = params
 
     def verify(self, on_off):
         """设置是否验证SSL证书
         :param on_off: 是否验证 SSL 证书
         :return: None
         """
-        self._page.session.verify = on_off
+        self._owner.session.verify = on_off
 
     def cert(self, cert):
         """SSL客户端证书文件的路径(.pem格式)，或(‘cert’, ‘key’)元组
         :param cert: 证书路径或元组
         :return: None
         """
-        self._page.session.cert = cert
+        self._owner.session.cert = cert
 
     def stream(self, on_off):
         """设置是否使用流式响应内容
         :param on_off: 是否使用流式响应内容
         :return: None
         """
-        self._page.session.stream = on_off
+        self._owner.session.stream = on_off
 
     def trust_env(self, on_off):
         """设置是否信任环境
         :param on_off: 是否信任环境
         :return: None
         """
-        self._page.session.trust_env = on_off
+        self._owner.session.trust_env = on_off
 
     def max_redirects(self, times):
         """设置最大重定向次数
         :param times: 最大重定向次数
         :return: None
         """
-        self._page.session.max_redirects = times
+        self._owner.session.max_redirects = times
 
     def add_adapter(self, url, adapter):
         """添加适配器
         :param url: 适配器对应url
         :param adapter: 适配器对象
         :return: None
         """
-        self._page.session.mount(url, adapter)
+        self._owner.session.mount(url, adapter)
 
 
 class WebPageSetter(ChromiumPageSetter):
-    def __init__(self, page):
-        super().__init__(page)
-        self._session_setter = SessionPageSetter(self._page)
-        self._chromium_setter = ChromiumPageSetter(self._page)
+    def __init__(self, owner):
+        super().__init__(owner)
+        self._session_setter = SessionPageSetter(self._owner)
+        self._chromium_setter = ChromiumPageSetter(self._owner)
 
     @property
     def cookies(self):
         """返回用于设置cookies的对象"""
         if self._cookies_setter is None:
-            self._cookies_setter = WebPageCookiesSetter(self._page)
+            self._cookies_setter = WebPageCookiesSetter(self._owner)
         return self._cookies_setter
 
     def headers(self, headers) -> None:
         """设置固定发送的headers
         :param headers: dict格式的headers数据
         :return: None
         """
-        if self._page.mode == 's':
+        if self._owner.mode == 's':
             self._session_setter.headers(headers)
         else:
             self._chromium_setter.headers(headers)
 
     def user_agent(self, ua, platform=None):
         """设置user agent，d模式下只有当前tab有效"""
-        if self._page.mode == 's':
+        if self._owner.mode == 's':
             self._session_setter.user_agent(ua)
         else:
             self._chromium_setter.user_agent(ua, platform)
 
 
 class WebPageTabSetter(TabSetter):
-    def __init__(self, page):
-        super().__init__(page)
-        self._session_setter = SessionPageSetter(self._page)
-        self._chromium_setter = ChromiumBaseSetter(self._page)
+    def __init__(self, owner):
+        super().__init__(owner)
+        self._session_setter = SessionPageSetter(self._owner)
+        self._chromium_setter = ChromiumBaseSetter(self._owner)
 
     @property
     def cookies(self):
         """返回用于设置cookies的对象"""
         if self._cookies_setter is None:
-            self._cookies_setter = WebPageCookiesSetter(self._page)
+            self._cookies_setter = WebPageCookiesSetter(self._owner)
         return self._cookies_setter
 
     def headers(self, headers) -> None:
         """设置固定发送的headers
         :param headers: dict格式的headers数据
         :return: None
         """
-        if self._page._has_session:
+        if self._owner._has_session:
             self._session_setter.headers(headers)
-        if self._page._has_driver:
+        if self._owner._has_driver:
             self._chromium_setter.headers(headers)
 
     def user_agent(self, ua, platform=None):
         """设置user agent，d模式下只有当前tab有效"""
-        if self._page._has_session:
+        if self._owner._has_session:
             self._session_setter.user_agent(ua)
-        if self._page._has_driver:
+        if self._owner._has_driver:
             self._chromium_setter.user_agent(ua, platform)
 
 
 class ChromiumElementSetter(object):
     def __init__(self, ele):
         """
         :param ele: ChromiumElement
@@ -487,50 +492,53 @@
 class ChromiumFrameSetter(ChromiumBaseSetter):
     def attr(self, name, value):
         """设置frame元素attribute属性
         :param name: 属性名
         :param value: 属性值
         :return: None
         """
-        self._page.frame_ele.set.attr(name, value)
+        self._owner.frame_ele.set.attr(name, value)
 
 
 class LoadMode(object):
     """用于设置页面加载策略的类"""
 
-    def __init__(self, page):
+    def __init__(self, owner):
         """
-        :param page: ChromiumBase对象
+        :param owner: ChromiumBase对象
         """
-        self._page = page
+        self._owner = owner
 
     def __call__(self, value):
         """设置加载策略
         :param value: 可选 'normal', 'eager', 'none'
         :return: None
         """
         if value.lower() not in ('normal', 'eager', 'none'):
             raise ValueError("只能选择 'normal', 'eager', 'none'。")
-        self._page._load_mode = value
+        self._owner._load_mode = value
 
     def normal(self):
         """设置页面加载策略为normal"""
-        self._page._load_mode = 'normal'
+        self._owner._load_mode = 'normal'
 
     def eager(self):
         """设置页面加载策略为eager"""
-        self._page._load_mode = 'eager'
+        self._owner._load_mode = 'eager'
 
     def none(self):
         """设置页面加载策略为none"""
-        self._page._load_mode = 'none'
+        self._owner._load_mode = 'none'
 
 
 class PageScrollSetter(object):
     def __init__(self, scroll):
+        """
+        :param scroll: PageScroller对象
+        """
         self._scroll = scroll
 
     def wait_complete(self, on_off=True):
         """设置滚动命令后是否等待完成
         :param on_off: 开或关
         :return: None
         """
@@ -549,19 +557,19 @@
         self._scroll._driver.run_js(f'document.documentElement.style.setProperty("scroll-behavior","{b}");')
         self._scroll._wait_complete = on_off
 
 
 class WindowSetter(object):
     """用于设置窗口大小的类"""
 
-    def __init__(self, page):
+    def __init__(self, owner):
         """
-        :param page: 页面对象
+        :param owner: 页面对象
         """
-        self._page = page
+        self._owner = owner
         self._window_id = self._get_info()['windowId']
 
     def max(self):
         """窗口最大化"""
         s = self._get_info()['bounds']['windowState']
         if s in ('fullscreen', 'minimized'):
             self._perform({'windowState': 'normal'})
@@ -616,25 +624,25 @@
             y = y if y is not None else info['top']
             self._perform({'left': x - 8, 'top': y})
 
     def _get_info(self):
         """获取窗口位置及大小信息"""
         for _ in range(50):
             try:
-                return self._page.run_cdp('Browser.getWindowForTarget')
+                return self._owner.run_cdp('Browser.getWindowForTarget')
             except:
                 sleep(.1)
 
     def _perform(self, bounds):
         """执行改变窗口大小操作
         :param bounds: 控制数据
         :return: None
         """
         try:
-            self._page.run_cdp('Browser.setWindowBounds', windowId=self._window_id, bounds=bounds)
+            self._owner.run_cdp('Browser.setWindowBounds', windowId=self._window_id, bounds=bounds)
         except:
             raise RuntimeError('浏览器全屏或最小化状态时请先调用set.window.normal()恢复正常状态。')
 
     # ------------即将废除----------
 
     def maximized(self):
         """窗口最大化"""
@@ -644,16 +652,14 @@
         """窗口最小化"""
         self.mini()
 
     def fullscreen(self):
         """设置窗口为全屏"""
         self.full()
 
-
-class PageWindowSetter(WindowSetter):
     def hide(self):
         """隐藏浏览器窗口，只在Windows系统可用"""
-        show_or_hide_browser(self._page, hide=True)
+        show_or_hide_browser(self._owner, hide=True)
 
     def show(self):
         """显示浏览器窗口，只在Windows系统可用"""
-        show_or_hide_browser(self._page, hide=False)
+        show_or_hide_browser(self._owner, hide=False)
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/setter.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/setter.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 """
 @Author   : g1879
 @Contact  : g1879@qq.com
 @Copyright: (c) 2024 by g1879, Inc. All Rights Reserved.
 @License  : BSD 3-Clause.
 """
 from pathlib import Path
-from typing import Union, Tuple, Literal, Any
+from typing import Union, Tuple, Literal, Any, Optional
 
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
 
 from .cookies_setter import SessionCookiesSetter, CookiesSetter, WebPageCookiesSetter
 from .scroller import PageScroller
 from .._base.base import BasePage
 from .._elements.chromium_element import ChromiumElement
 from .._pages.chromium_base import ChromiumBase
 from .._pages.chromium_frame import ChromiumFrame
 from .._pages.chromium_page import ChromiumPage
-from .._pages.chromium_tab import ChromiumTab
+from .._pages.chromium_tab import ChromiumTab, WebPageTab
 from .._pages.session_page import SessionPage
 from .._pages.web_page import WebPage
 
 FILE_EXISTS = Literal['skip', 'rename', 'overwrite', 's', 'r', 'o']
 
 
 class BasePageSetter(object):
-    def __init__(self, page: BasePage):
-        self._page: BasePage = ...
+    def __init__(self, owner: BasePage):
+        self._owner: BasePage = ...
 
     def NoneElement_value(self, value: Any = None, on_off: bool = True) -> None: ...
 
 
 class ChromiumBaseSetter(BasePageSetter):
-    def __init__(self, page):
-        self._page: ChromiumBase = ...
+    def __init__(self, owner):
+        self._owner: ChromiumBase = ...
         self._cookies_setter: CookiesSetter = ...
 
     @property
     def load_mode(self) -> LoadMode: ...
 
     @property
     def scroll(self) -> PageScrollSetter: ...
@@ -54,68 +54,66 @@
 
     def user_agent(self, ua: str, platform: str = None) -> None: ...
 
     def session_storage(self, item: str, value: Union[str, bool]) -> None: ...
 
     def local_storage(self, item: str, value: Union[str, bool]) -> None: ...
 
-    def headers(self, headers: dict) -> None: ...
+    def headers(self, headers: Union[dict, str]) -> None: ...
 
     def auto_handle_alert(self, on_off: bool = True, accept: bool = True) -> None: ...
 
     def upload_files(self, files: Union[str, Path, list, tuple]) -> None: ...
 
     def blocked_urls(self, urls: Union[list, tuple, str, None]) -> None: ...
 
 
 class TabSetter(ChromiumBaseSetter):
-    def __init__(self, page): ...
+    _owner: ChromiumTab = ...
+
+    def __init__(self, owner: Union[ChromiumTab, WebPageTab, WebPage, ChromiumPage]): ...
 
     @property
     def window(self) -> WindowSetter: ...
 
     def download_path(self, path: Union[str, Path]) -> None: ...
 
     def download_file_name(self, name: str = None, suffix: str = None) -> None: ...
 
     def when_download_file_exists(self, mode: FILE_EXISTS) -> None: ...
 
     def activate(self) -> None: ...
 
 
 class ChromiumPageSetter(TabSetter):
-    _page: ChromiumPage = ...
-
-    @property
-    def window(self) -> PageWindowSetter: ...
-
-    def main_tab(self, tab_id: str = None) -> None: ...
+    _owner: ChromiumPage = ...
 
     def tab_to_front(self, tab_or_id: Union[str, ChromiumTab] = None) -> None: ...
 
 
 class SessionPageSetter(BasePageSetter):
-    def __init__(self, page: SessionPage):
-        self._page: SessionPage = ...
-        self._cookies_setter: SessionCookiesSetter = ...
+    _owner: SessionPage = ...
+    _cookies_setter: Optional[SessionCookiesSetter] = ...
+
+    def __init__(self, owner: SessionPage): ...
 
     @property
     def cookies(self) -> SessionCookiesSetter: ...
 
     def retry_times(self, times: int) -> None: ...
 
     def retry_interval(self, interval: float) -> None: ...
 
     def download_path(self, path: Union[str, Path]) -> None: ...
 
     def timeout(self, second: float) -> None: ...
 
     def encoding(self, encoding: Union[str, None], set_all: bool = True) -> None: ...
 
-    def headers(self, headers: dict) -> None: ...
+    def headers(self, headers: Union[str, dict]) -> None: ...
 
     def header(self, name: str, value: str) -> None: ...
 
     def user_agent(self, ua: str) -> None: ...
 
     def proxies(self, http: str = None, https: str = None) -> None: ...
 
@@ -135,34 +133,34 @@
 
     def max_redirects(self, times: Union[int, None]) -> None: ...
 
     def add_adapter(self, url: str, adapter: HTTPAdapter) -> None: ...
 
 
 class WebPageSetter(ChromiumPageSetter):
-    _page: WebPage = ...
+    _owner: WebPage = ...
     _session_setter: SessionPageSetter = ...
     _chromium_setter: ChromiumPageSetter = ...
 
     def user_agent(self, ua: str, platform: str = None) -> None: ...
 
-    def headers(self, headers: dict) -> None: ...
+    def headers(self, headers: Union[str, dict]) -> None: ...
 
     @property
     def cookies(self) -> WebPageCookiesSetter: ...
 
 
 class WebPageTabSetter(TabSetter):
-    _page: WebPage = ...
+    _owner: WebPageTab = ...
     _session_setter: SessionPageSetter = ...
     _chromium_setter: ChromiumBaseSetter = ...
 
     def user_agent(self, ua: str, platform: str = None) -> None: ...
 
-    def headers(self, headers: dict) -> None: ...
+    def headers(self, headers: Union[str, dict]) -> None: ...
 
     @property
     def cookies(self) -> WebPageCookiesSetter: ...
 
 
 class ChromiumElementSetter(object):
     def __init__(self, ele: ChromiumElement):
@@ -174,22 +172,22 @@
 
     def innerHTML(self, html: str) -> None: ...
 
     def value(self, value: str) -> None: ...
 
 
 class ChromiumFrameSetter(ChromiumBaseSetter):
-    _page: ChromiumFrame = ...
+    _owner: ChromiumFrame = ...
 
     def attr(self, name: str, value: str) -> None: ...
 
 
 class LoadMode(object):
-    def __init__(self, page: ChromiumBase):
-        self._page: ChromiumBase = ...
+    def __init__(self, owner: ChromiumBase):
+        self._owner: ChromiumBase = ...
 
     def __call__(self, value: str) -> None: ...
 
     def normal(self) -> None: ...
 
     def eager(self) -> None: ...
 
@@ -202,16 +200,16 @@
 
     def wait_complete(self, on_off: bool = True): ...
 
     def smooth(self, on_off: bool = True): ...
 
 
 class WindowSetter(object):
-    def __init__(self, page: ChromiumBase):
-        self._page: ChromiumBase = ...
+    def __init__(self, owner: ChromiumBase):
+        self._owner: ChromiumBase = ...
         self._window_id: str = ...
 
     def max(self) -> None: ...
 
     def mini(self) -> None: ...
 
     def full(self) -> None: ...
@@ -222,14 +220,10 @@
 
     def location(self, x: int = None, y: int = None) -> None: ...
 
     def _get_info(self) -> dict: ...
 
     def _perform(self, bounds: dict) -> None: ...
 
-
-class PageWindowSetter(WindowSetter):
-    _page: ChromiumPage = ...
-
     def hide(self) -> None: ...
 
     def show(self) -> None: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/states.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/states.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,43 +101,43 @@
         except Exception:
             return False
 
 
 class PageStates(object):
     """Page对象、Tab对象使用"""
 
-    def __init__(self, page):
+    def __init__(self, owner):
         """
-        :param page: ChromiumBase对象
+        :param owner: ChromiumBase对象
         """
-        self._page = page
+        self._owner = owner
 
     @property
     def is_loading(self):
         """返回页面是否在加载状态"""
-        return self._page._is_loading
+        return self._owner._is_loading
 
     @property
     def is_alive(self):
         """返回页面对象是否仍然可用"""
         try:
-            self._page.run_cdp('Page.getLayoutMetrics')
+            self._owner.run_cdp('Page.getLayoutMetrics')
             return True
         except PageDisconnectedError:
             return False
 
     @property
     def ready_state(self):
         """返回当前页面加载状态，'connecting' 'loading' 'interactive' 'complete'"""
-        return self._page._ready_state
+        return self._owner._ready_state
 
     @property
     def has_alert(self):
         """返回当前页面是否存在弹窗"""
-        return self._page._has_alert
+        return self._owner._has_alert
 
 
 class FrameStates(object):
     def __init__(self, frame):
         """
         :param frame: ChromiumFrame对象
         """
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/states.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/states.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     def is_enabled(self) -> bool: ...
 
     @property
     def is_alive(self) -> bool: ...
 
 
 class PageStates(object):
-    def __init__(self, page: ChromiumBase):
-        self._page: ChromiumBase = ...
+    def __init__(self, owner: ChromiumBase):
+        self._owner: ChromiumBase = ...
 
     @property
     def is_loading(self) -> bool: ...
 
     @property
     def is_alive(self) -> bool: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/waiter.py` & `DrissionPage-4.0.4.9/DrissionPage/_units/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,14 @@
         while self._driver.states.has_alert:
             sleep(.2)
 
 
 class PageWaiter(TabWaiter):
     def __init__(self, page):
         super().__init__(page)
-        # self._listener = None
 
     def new_tab(self, timeout=None, raise_err=None):
         """等待新标签页出现
         :param timeout: 等待超时时间，为None则使用页面对象timeout属性
         :param raise_err: 等待失败时是否报错，为None时根据Settings设置
         :return: 等到新标签页返回其id，否则返回False
         """
@@ -321,20 +320,20 @@
             else:
                 return True
 
 
 class ElementWaiter(object):
     """等待元素在dom中某种状态，如删除、显示、隐藏"""
 
-    def __init__(self, page, ele):
+    def __init__(self, owner, ele):
         """等待元素在dom中某种状态，如删除、显示、隐藏
-        :param page: 元素所在页面
+        :param owner: 元素所在页面
         :param ele: 要等待的元素
         """
-        self._page = page
+        self._owner = owner
         self._ele = ele
 
     def __call__(self, second, scope=None):
         """等待若干秒，如传入两个参数，等待时间为这两个数间的一个随机数
         :param second: 秒数
         :param scope: 随机数范围
         :return: None
@@ -404,15 +403,15 @@
     def disabled_or_deleted(self, timeout=None, raise_err=None):
         """等待当前元素变成不可用或从DOM移除
         :param timeout: 超时时间，为None使用元素所在页面timeout属性
         :param raise_err: 等待失败时是否报错，为None时根据Settings设置
         :return: 是否等待成功
         """
         if timeout is None:
-            timeout = self._page.timeout
+            timeout = self._owner.timeout
         end_time = perf_counter() + timeout
         while perf_counter() < end_time:
             if not self._ele.states.is_enabled or not self._ele.states.is_alive:
                 return True
             sleep(.05)
 
         if raise_err is True or Settings.raise_when_wait_failed is True:
@@ -424,15 +423,15 @@
         """等待当前元素停止运动
         :param gap: 检测间隔时间
         :param timeout: 超时时间，为None使用元素所在页面timeout属性
         :param raise_err: 等待失败时是否报错，为None时根据Settings设置
         :return: 是否等待成功
         """
         if timeout is None:
-            timeout = self._page.timeout
+            timeout = self._owner.timeout
         end_time = perf_counter() + timeout
         while perf_counter() < end_time:
             try:
                 size = self._ele.states.has_rect
                 location = self._ele.rect.location
                 break
             except NoRectError:
@@ -467,15 +466,15 @@
         :param timeout: 超时时间，为None使用元素所在页面timeout属性
         :param raise_err: 等待失败时是否报错，为None时根据Settings设置
         :param err_text: 抛出错误时显示的信息
         :return: 是否等待成功
         """
         err_text = err_text or '等待元素状态改变失败（等待{}秒）。'
         if timeout is None:
-            timeout = self._page.timeout
+            timeout = self._owner.timeout
         end_time = perf_counter() + timeout
         while perf_counter() < end_time:
             a = self._ele.states.__getattribute__(attr)
             if (a and mode) or (not a and not mode):
                 return True
             sleep(.05)
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/_units/waiter.pyi` & `DrissionPage-4.0.4.9/DrissionPage/_units/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 
     def new_tab(self, timeout: float = None, raise_err: bool = None) -> Union[str, bool]: ...
 
     def all_downloads_done(self, timeout: float = None, cancel_if_timeout: bool = True) -> bool: ...
 
 
 class ElementWaiter(object):
-    def __init__(self, page: ChromiumBase, ele: ChromiumElement):
+    def __init__(self, owner: ChromiumBase, ele: ChromiumElement):
         self._ele: ChromiumElement = ...
-        self._page: ChromiumBase = ...
+        self._owner: ChromiumBase = ...
 
     def __call__(self, second: float, scope: float = None) -> None: ...
 
     def deleted(self, timeout: float = None, raise_err: bool = None) -> bool: ...
 
     def displayed(self, timeout: float = None, raise_err: bool = None) -> bool: ...
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage/errors.py` & `DrissionPage-4.0.4.9/DrissionPage/errors.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage/items.py` & `DrissionPage-4.0.4.9/DrissionPage/items.py`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/DrissionPage.egg-info/PKG-INFO` & `DrissionPage-4.0.4.9/DrissionPage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DrissionPage
-Version: 4.0.4.8
+Version: 4.0.4.9
 Summary: Python based web automation tool. It can control the browser and send and receive data packets.
 Home-page: https://gitee.com/g1879/DrissionPage
 Author: g1879
 Author-email: g1879@qq.com
 License: BSD
 Keywords: DrissionPage
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DrissionPage Version: 4.0.4.8 Summary: Python based
+Metadata-Version: 2.1 Name: DrissionPage Version: 4.0.4.9 Summary: Python based
 web automation tool. It can control the browser and send and receive data
 packets. Home-page: https://gitee.com/g1879/DrissionPage Author: g1879 Author-
 email: g1879@qq.com License: BSD Keywords: DrissionPage Classifier: Programming
 Language :: Python :: 3.6 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities Classifier: License :: OSI Approved :: BSD
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # â¨ï¸ æ¦è¿° DrissionPage æ¯ä¸ä¸ªåºäº python
```

### Comparing `DrissionPage-4.0.4.8/DrissionPage.egg-info/SOURCES.txt` & `DrissionPage-4.0.4.9/DrissionPage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/LICENSE` & `DrissionPage-4.0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/PKG-INFO` & `DrissionPage-4.0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DrissionPage
-Version: 4.0.4.8
+Version: 4.0.4.9
 Summary: Python based web automation tool. It can control the browser and send and receive data packets.
 Home-page: https://gitee.com/g1879/DrissionPage
 Author: g1879
 Author-email: g1879@qq.com
 License: BSD
 Keywords: DrissionPage
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DrissionPage Version: 4.0.4.8 Summary: Python based
+Metadata-Version: 2.1 Name: DrissionPage Version: 4.0.4.9 Summary: Python based
 web automation tool. It can control the browser and send and receive data
 packets. Home-page: https://gitee.com/g1879/DrissionPage Author: g1879 Author-
 email: g1879@qq.com License: BSD Keywords: DrissionPage Classifier: Programming
 Language :: Python :: 3.6 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities Classifier: License :: OSI Approved :: BSD
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # â¨ï¸ æ¦è¿° DrissionPage æ¯ä¸ä¸ªåºäº python
```

### Comparing `DrissionPage-4.0.4.8/README.md` & `DrissionPage-4.0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `DrissionPage-4.0.4.8/setup.py` & `DrissionPage-4.0.4.9/setup.py`

 * *Files identical despite different names*

