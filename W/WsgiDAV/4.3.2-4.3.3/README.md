# Comparing `tmp/WsgiDAV-4.3.2.tar.gz` & `tmp/wsgidav-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WsgiDAV-4.3.2.tar", last modified: Fri Mar 29 13:54:23 2024, max compression
+gzip compressed data, was "wsgidav-4.3.3.tar", last modified: Sat May  4 18:27:15 2024, max compression
```

## Comparing `WsgiDAV-4.3.2.tar` & `wsgidav-4.3.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/
--rw-rw-rw-   0        0        0    17974 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1145 2023-10-22 09:36:07.000000 WsgiDAV-4.3.2/LICENSE
--rw-rw-rw-   0        0        0     6964 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4892 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/WsgiDAV.egg-info/
--rw-rw-rw-   0        0        0     6964 2024-03-29 13:54:23.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3502 2024-03-29 13:54:23.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 13:54:23.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-29 13:54:23.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-12-12 08:40:03.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2024-03-29 13:54:23.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-29 13:54:23.000000 WsgiDAV-4.3.2/WsgiDAV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1658 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/pyproject.toml
--rw-rw-rw-   0        0        0    14587 2023-12-09 14:15:43.000000 WsgiDAV-4.3.2/sample_wsgidav.yaml
--rw-rw-rw-   0        0        0     3056 2024-03-29 13:54:23.429882 WsgiDAV-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0      144 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.383006 WsgiDAV-4.3.2/tests/
--rw-rw-rw-   0        0        0     1853 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_http.py
--rw-rw-rw-   0        0        0     4607 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_litmus.py
--rw-rw-rw-   0        0        0    13513 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_lock_manager.py
--rw-rw-rw-   0        0        0     4024 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_property_manager.py
--rw-rw-rw-   0        0        0    19318 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_scripted.py
--rw-rw-rw-   0        0        0     7196 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_streaming.py
--rw-rw-rw-   0        0        0    11921 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_util.py
--rw-rw-rw-   0        0        0     9057 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/tests/test_wsgidav_app.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.398631 WsgiDAV-4.3.2/wsgidav/
--rw-rw-rw-   0        0        0      973 2024-03-29 13:54:21.000000 WsgiDAV-4.3.2/wsgidav/__init__.py
--rw-rw-rw-   0        0        0    10576 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dav_error.py
--rw-rw-rw-   0        0        0    61752 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dav_provider.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.398631 WsgiDAV-4.3.2/wsgidav/dc/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/dc/__init__.py
--rw-rw-rw-   0        0        0     8156 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dc/base_dc.py
--rw-rw-rw-   0        0        0     8071 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dc/nt_dc.py
--rw-rw-rw-   0        0        0     2426 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dc/pam_dc.py
--rw-rw-rw-   0        0        0     4771 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dc/simple_dc.py
--rw-rw-rw-   0        0        0     5070 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/default_conf.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.398631 WsgiDAV-4.3.2/wsgidav/dir_browser/
--rw-rw-rw-   0        0        0       61 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/__init__.py
--rw-rw-rw-   0        0        0    12925 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/_dir_browser.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.398631 WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/
--rw-rw-rw-   0        0        0    12602 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/favicon.ico
--rw-rw-rw-   0        0        0      890 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/logo.png
--rw-rw-rw-   0        0        0     2762 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/script.js
--rw-rw-rw-   0        0        0     1047 2023-10-22 09:36:07.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/style.css
--rw-rw-rw-   0        0        0     2967 2023-10-22 09:36:07.000000 WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/template.html
--rw-rw-rw-   0        0        0     4627 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/error_printer.py
--rw-rw-rw-   0        0        0    18492 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/fs_dav_provider.py
--rw-rw-rw-   0        0        0    23863 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/http_authenticator.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.398631 WsgiDAV-4.3.2/wsgidav/lock_man/
--rw-rw-rw-   0        0        0        0 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/lock_man/__init__.py
--rw-rw-rw-   0        0        0    18757 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/lock_man/lock_manager.py
--rw-rw-rw-   0        0        0    13799 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/lock_man/lock_storage.py
--rw-rw-rw-   0        0        0     8585 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/lock_man/lock_storage_redis.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/wsgidav/mw/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/mw/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/mw/base_mw.py
--rw-rw-rw-   0        0        0     5005 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/mw/cors.py
--rw-rw-rw-   0        0        0     8138 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/mw/debug_filter.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/wsgidav/prop_man/
--rw-rw-rw-   0        0        0        0 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/prop_man/__init__.py
--rw-rw-rw-   0        0        0     8339 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/prop_man/couch_property_manager.py
--rw-rw-rw-   0        0        0     7156 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/prop_man/mongo_property_manager.py
--rw-rw-rw-   0        0        0    11675 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/prop_man/property_manager.py
--rw-rw-rw-   0        0        0     8817 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/request_resolver.py
--rw-rw-rw-   0        0        0    66394 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/request_server.py
--rw-rw-rw-   0        0        0    10356 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/rw_lock.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/wsgidav/samples/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/samples/__init__.py
--rw-rw-rw-   0        0        0     6434 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/samples/dav_provider_tools.py
--rw-rw-rw-   0        0        0    23133 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/samples/hg_dav_provider.py
--rw-rw-rw-   0        0        0     5564 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/samples/mongo_dav_provider.py
--rw-rw-rw-   0        0        0    21618 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/samples/mysql_dav_provider.py
--rw-rw-rw-   0        0        0    25181 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/samples/virtual_dav_provider.py
-drwxrwxrwx   0        0        0        0 2024-03-29 13:54:23.414256 WsgiDAV-4.3.2/wsgidav/server/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 WsgiDAV-4.3.2/wsgidav/server/__init__.py
--rw-rw-rw-   0        0        0    14787 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/server/ext_wsgiutils_server.py
--rw-rw-rw-   0        0        0     1402 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/server/run_reloading_server.py
--rw-rw-rw-   0        0        0    26733 2024-03-29 13:48:27.000000 WsgiDAV-4.3.2/wsgidav/server/server_cli.py
--rw-rw-rw-   0        0        0     1875 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/server/server_sample.py
--rw-rw-rw-   0        0        0     5131 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/stream_tools.py
--rw-rw-rw-   0        0        0    61165 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/util.py
--rw-rw-rw-   0        0        0    25468 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/wsgidav_app.py
--rw-rw-rw-   0        0        0     4134 2024-03-29 13:11:59.000000 WsgiDAV-4.3.2/wsgidav/xml_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.963683 wsgidav-4.3.3/
+-rw-rw-rw-   0        0        0    18265 2024-05-04 18:21:42.000000 wsgidav-4.3.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1145 2024-05-03 15:56:41.000000 wsgidav-4.3.3/LICENSE
+-rw-rw-rw-   0        0        0     7032 2024-05-04 18:27:15.948047 wsgidav-4.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4960 2024-03-29 14:44:06.000000 wsgidav-4.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.948047 wsgidav-4.3.3/WsgiDAV.egg-info/
+-rw-rw-rw-   0        0        0     7032 2024-05-04 18:27:15.000000 wsgidav-4.3.3/WsgiDAV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3502 2024-05-04 18:27:15.000000 wsgidav-4.3.3/WsgiDAV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 18:27:15.000000 wsgidav-4.3.3/WsgiDAV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-04 18:27:15.000000 wsgidav-4.3.3/WsgiDAV.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-12-12 08:40:03.000000 wsgidav-4.3.3/WsgiDAV.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2024-05-04 18:27:15.000000 wsgidav-4.3.3/WsgiDAV.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-04 18:27:15.000000 wsgidav-4.3.3/WsgiDAV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1658 2024-03-29 13:11:59.000000 wsgidav-4.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0    14587 2023-12-09 14:15:43.000000 wsgidav-4.3.3/sample_wsgidav.yaml
+-rw-rw-rw-   0        0        0     3038 2024-05-04 18:27:15.963683 wsgidav-4.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      144 2024-03-29 13:11:59.000000 wsgidav-4.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.916788 wsgidav-4.3.3/tests/
+-rw-rw-rw-   0        0        0     1853 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_http.py
+-rw-rw-rw-   0        0        0     4608 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_litmus.py
+-rw-rw-rw-   0        0        0    13513 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_lock_manager.py
+-rw-rw-rw-   0        0        0     4024 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_property_manager.py
+-rw-rw-rw-   0        0        0    19318 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_scripted.py
+-rw-rw-rw-   0        0        0     7196 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_streaming.py
+-rw-rw-rw-   0        0        0    11921 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_util.py
+-rw-rw-rw-   0        0        0     9057 2024-05-03 15:56:44.000000 wsgidav-4.3.3/tests/test_wsgidav_app.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.932432 wsgidav-4.3.3/wsgidav/
+-rw-rw-rw-   0        0        0      973 2024-05-04 18:27:13.000000 wsgidav-4.3.3/wsgidav/__init__.py
+-rw-rw-rw-   0        0        0    10576 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/dav_error.py
+-rw-rw-rw-   0        0        0    61752 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/dav_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.932432 wsgidav-4.3.3/wsgidav/dc/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/dc/__init__.py
+-rw-rw-rw-   0        0        0     8156 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/dc/base_dc.py
+-rw-rw-rw-   0        0        0     8071 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/dc/nt_dc.py
+-rw-rw-rw-   0        0        0     2426 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/dc/pam_dc.py
+-rw-rw-rw-   0        0        0     4771 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/dc/simple_dc.py
+-rw-rw-rw-   0        0        0     5070 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/default_conf.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.932432 wsgidav-4.3.3/wsgidav/dir_browser/
+-rw-rw-rw-   0        0        0       61 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/dir_browser/__init__.py
+-rw-rw-rw-   0        0        0    12925 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/dir_browser/_dir_browser.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.932432 wsgidav-4.3.3/wsgidav/dir_browser/htdocs/
+-rw-rw-rw-   0        0        0    12602 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/dir_browser/htdocs/favicon.ico
+-rw-rw-rw-   0        0        0      890 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/dir_browser/htdocs/logo.png
+-rw-rw-rw-   0        0        0     2762 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/dir_browser/htdocs/script.js
+-rw-rw-rw-   0        0        0     1047 2023-10-22 09:36:07.000000 wsgidav-4.3.3/wsgidav/dir_browser/htdocs/style.css
+-rw-rw-rw-   0        0        0     2967 2023-10-22 09:36:07.000000 wsgidav-4.3.3/wsgidav/dir_browser/htdocs/template.html
+-rw-rw-rw-   0        0        0     4627 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/error_printer.py
+-rw-rw-rw-   0        0        0    18492 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/fs_dav_provider.py
+-rw-rw-rw-   0        0        0    23863 2024-05-04 18:12:04.000000 wsgidav-4.3.3/wsgidav/http_authenticator.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.932432 wsgidav-4.3.3/wsgidav/lock_man/
+-rw-rw-rw-   0        0        0        0 2024-03-29 13:11:59.000000 wsgidav-4.3.3/wsgidav/lock_man/__init__.py
+-rw-rw-rw-   0        0        0    18757 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/lock_man/lock_manager.py
+-rw-rw-rw-   0        0        0    13799 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/lock_man/lock_storage.py
+-rw-rw-rw-   0        0        0     8585 2024-05-03 15:56:44.000000 wsgidav-4.3.3/wsgidav/lock_man/lock_storage_redis.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.948047 wsgidav-4.3.3/wsgidav/mw/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/mw/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-03-29 13:11:59.000000 wsgidav-4.3.3/wsgidav/mw/base_mw.py
+-rw-rw-rw-   0        0        0     5005 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/mw/cors.py
+-rw-rw-rw-   0        0        0     8138 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/mw/debug_filter.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.948047 wsgidav-4.3.3/wsgidav/prop_man/
+-rw-rw-rw-   0        0        0        0 2024-03-29 13:11:59.000000 wsgidav-4.3.3/wsgidav/prop_man/__init__.py
+-rw-rw-rw-   0        0        0     8309 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/prop_man/couch_property_manager.py
+-rw-rw-rw-   0        0        0     7130 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/prop_man/mongo_property_manager.py
+-rw-rw-rw-   0        0        0    11665 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/prop_man/property_manager.py
+-rw-rw-rw-   0        0        0     8817 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/request_resolver.py
+-rw-rw-rw-   0        0        0    66300 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/request_server.py
+-rw-rw-rw-   0        0        0    10356 2024-03-29 13:11:59.000000 wsgidav-4.3.3/wsgidav/rw_lock.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.948047 wsgidav-4.3.3/wsgidav/samples/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/samples/__init__.py
+-rw-rw-rw-   0        0        0     6434 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/samples/dav_provider_tools.py
+-rw-rw-rw-   0        0        0    23093 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/samples/hg_dav_provider.py
+-rw-rw-rw-   0        0        0     5564 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/samples/mongo_dav_provider.py
+-rw-rw-rw-   0        0        0    21540 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/samples/mysql_dav_provider.py
+-rw-rw-rw-   0        0        0    25207 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/samples/virtual_dav_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:27:15.948047 wsgidav-4.3.3/wsgidav/server/
+-rw-rw-rw-   0        0        0        0 2021-12-11 16:37:05.000000 wsgidav-4.3.3/wsgidav/server/__init__.py
+-rw-rw-rw-   0        0        0    14787 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/server/ext_wsgiutils_server.py
+-rw-rw-rw-   0        0        0     1402 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/server/run_reloading_server.py
+-rw-rw-rw-   0        0        0    26733 2024-03-29 13:48:27.000000 wsgidav-4.3.3/wsgidav/server/server_cli.py
+-rw-rw-rw-   0        0        0     1875 2024-05-03 15:56:43.000000 wsgidav-4.3.3/wsgidav/server/server_sample.py
+-rw-rw-rw-   0        0        0     5131 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/stream_tools.py
+-rw-rw-rw-   0        0        0    61165 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/util.py
+-rw-rw-rw-   0        0        0    25468 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/wsgidav_app.py
+-rw-rw-rw-   0        0        0     4134 2024-05-03 15:56:42.000000 wsgidav-4.3.3/wsgidav/xml_tools.py
```

### Comparing `WsgiDAV-4.3.2/CHANGELOG.md` & `wsgidav-4.3.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
-## 4.3.3 / Unreleased
+## 4.3.4 / Unreleased
+
+## 4.3.3 / 2024-05-04
+
+- Deprecate Python 3.8 (EOL: 2024-10-14)
+- Build Windows installer with Python 3.12
+- Update to Cheroot 10.8
+- [#315](https://github.com/mar10/wsgidav/issues/315) CHANGELOG.md is installed into the virtualenv or prefix root directory
 
 ## 4.3.2 / 2024-03-29
 
-- [#318](https://github.com/mar10/wsgidav/issues/318)
+- [#318](https://github.com/mar10/wsgidav/issues/318) Error when used with lxml
 - Test with Python 3.12
 - Update to black 24.3
 - Use ruff instead of flake8
 
 ## 4.3.1 / 2024-03-24
 
 - New option `suppress_version_info` to suppress WsgiDAV's version info in
```

### Comparing `WsgiDAV-4.3.2/LICENSE` & `wsgidav-4.3.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) 2009-2023 Martin Wendt, (Original PyFileServer (c) 2005 Ho Chun Wei)
+Copyright (c) 2009-2024 Martin Wendt, (Original PyFileServer (c) 2005 Ho Chun Wei)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `WsgiDAV-4.3.2/PKG-INFO` & `wsgidav-4.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WsgiDAV
-Version: 4.3.2
+Version: 4.3.3
 Summary: Generic and extendable WebDAV server based on WSGI
 Home-page: https://github.com/mar10/wsgidav
 Author: Martin Wendt
 Author-email: wsgidav@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: wsgidav@wwwendt.de
 License: MIT
@@ -87,15 +87,18 @@
     ```
     $ pip install wsgidav[pam]
     $ wsgidav --host=0.0.0.0 --port=8080 --root=/tmp --auth=pam-login
     ```
 
   - **Note:** Windows users may prefer the
     [MSI Installer](https://github.com/mar10/wsgidav/releases/latest)
-    (see <kbd>Assets</kbd> section).
+    (see <kbd>Assets</kbd> section), or use _winget_:
+    ```ps1
+    > winget install wsgidav
+    ```
 
   - WebDAV is a superset of HTTP, so WsgiDAV is also a performant, multi-threaded
     web server with SSL support.
 
   - WsgiDAV is also a Python library that implements the WSGI protocol and can
 	  be run behind any WSGI compliant web server.<br>
```

### Comparing `WsgiDAV-4.3.2/README.md` & `wsgidav-4.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     ```
     $ pip install wsgidav[pam]
     $ wsgidav --host=0.0.0.0 --port=8080 --root=/tmp --auth=pam-login
     ```
 
   - **Note:** Windows users may prefer the
     [MSI Installer](https://github.com/mar10/wsgidav/releases/latest)
-    (see <kbd>Assets</kbd> section).
+    (see <kbd>Assets</kbd> section), or use _winget_:
+    ```ps1
+    > winget install wsgidav
+    ```
 
   - WebDAV is a superset of HTTP, so WsgiDAV is also a performant, multi-threaded
     web server with SSL support.
 
   - WsgiDAV is also a Python library that implements the WSGI protocol and can
 	  be run behind any WSGI compliant web server.<br>
```

### Comparing `WsgiDAV-4.3.2/WsgiDAV.egg-info/PKG-INFO` & `wsgidav-4.3.3/WsgiDAV.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WsgiDAV
-Version: 4.3.2
+Version: 4.3.3
 Summary: Generic and extendable WebDAV server based on WSGI
 Home-page: https://github.com/mar10/wsgidav
 Author: Martin Wendt
 Author-email: wsgidav@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: wsgidav@wwwendt.de
 License: MIT
@@ -87,15 +87,18 @@
     ```
     $ pip install wsgidav[pam]
     $ wsgidav --host=0.0.0.0 --port=8080 --root=/tmp --auth=pam-login
     ```
 
   - **Note:** Windows users may prefer the
     [MSI Installer](https://github.com/mar10/wsgidav/releases/latest)
-    (see <kbd>Assets</kbd> section).
+    (see <kbd>Assets</kbd> section), or use _winget_:
+    ```ps1
+    > winget install wsgidav
+    ```
 
   - WebDAV is a superset of HTTP, so WsgiDAV is also a performant, multi-threaded
     web server with SSL support.
 
   - WsgiDAV is also a Python library that implements the WSGI protocol and can
 	  be run behind any WSGI compliant web server.<br>
```

### Comparing `WsgiDAV-4.3.2/WsgiDAV.egg-info/SOURCES.txt` & `wsgidav-4.3.3/WsgiDAV.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/pyproject.toml` & `wsgidav-4.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/sample_wsgidav.yaml` & `wsgidav-4.3.3/sample_wsgidav.yaml`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/setup.cfg` & `wsgidav-4.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -123,69 +123,68 @@
 000007a0: 7275 650d 0a65 7863 6c75 6465 203d 200d  rue..exclude = .
 000007b0: 0a09 7465 7374 730d 0a0d 0a5b 6f70 7469  ..tests....[opti
 000007c0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
 000007d0: 5d0d 0a77 7367 6964 6176 203d 200d 0a09  ]..wsgidav = ...
 000007e0: 6469 725f 6272 6f77 7365 722f 6874 646f  dir_browser/htdo
 000007f0: 6373 2f2a 2e2a 0d0a 0d0a 5b6f 7074 696f  cs/*.*....[optio
 00000800: 6e73 2e64 6174 615f 6669 6c65 735d 0d0a  ns.data_files]..
-00000810: 2e20 3d20 4348 414e 4745 4c4f 472e 6d64  . = CHANGELOG.md
-00000820: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000830: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-00000840: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-00000850: 0977 7367 6964 6176 203d 2077 7367 6964  .wsgidav = wsgid
-00000860: 6176 2e73 6572 7665 722e 7365 7276 6572  av.server.server
-00000870: 5f63 6c69 3a72 756e 0d0a 0d0a 5b63 6865  _cli:run....[che
-00000880: 636b 2d6d 616e 6966 6573 745d 0d0a 6967  ck-manifest]..ig
-00000890: 6e6f 7265 203d 200d 0a09 646f 6373 2f73  nore = ...docs/s
-000008a0: 7068 696e 782d 6275 696c 640d 0a09 646f  phinx-build...do
-000008b0: 6373 2f73 7068 696e 782d 6275 696c 642f  cs/sphinx-build/
-000008c0: 2a0d 0a0d 0a5b 616c 6961 7365 735d 0d0a  *....[aliases]..
-000008d0: 0d0a 5b63 6f76 6572 6167 653a 7275 6e5d  ..[coverage:run]
-000008e0: 0d0a 6272 616e 6368 203d 2054 7275 650d  ..branch = True.
-000008f0: 0a6f 6d69 7420 3d20 0d0a 0974 6573 7473  .omit = ...tests
-00000900: 2f2a 0d0a 0977 7367 6964 6176 2f70 726f  /*...wsgidav/pro
-00000910: 705f 6d61 6e2f 636f 7563 685f 7072 6f70  p_man/couch_prop
-00000920: 6572 7479 5f6d 616e 6167 6572 2e70 790d  erty_manager.py.
-00000930: 0a09 7773 6769 6461 762f 7072 6f70 5f6d  ..wsgidav/prop_m
-00000940: 616e 2f6d 6f6e 676f 5f70 726f 7065 7274  an/mongo_propert
-00000950: 795f 6d61 6e61 6765 722e 7079 0d0a 0977  y_manager.py...w
-00000960: 7367 6964 6176 2f73 616d 706c 6573 2f2a  sgidav/samples/*
-00000970: 0d0a 0977 7367 6964 6176 2f73 6572 7665  ...wsgidav/serve
-00000980: 722f 7275 6e5f 7265 6c6f 6164 696e 675f  r/run_reloading_
-00000990: 7365 7276 6572 2e70 790d 0a09 7773 6769  server.py...wsgi
-000009a0: 6461 762f 7365 7276 6572 2f73 6572 7665  dav/server/serve
-000009b0: 725f 7361 6d70 6c65 2e70 790d 0a0d 0a5b  r_sample.py....[
-000009c0: 636f 7665 7261 6765 3a72 6570 6f72 745d  coverage:report]
-000009d0: 0d0a 7072 6563 6973 696f 6e20 3d20 320d  ..precision = 2.
-000009e0: 0a73 6f72 7420 3d20 4e61 6d65 0d0a 6578  .sort = Name..ex
-000009f0: 636c 7564 655f 6c69 6e65 7320 3d20 0d0a  clude_lines = ..
-00000a00: 0970 7261 676d 613a 206e 6f20 636f 7665  .pragma: no cove
-00000a10: 720d 0a09 6966 205f 5f6e 616d 655f 5f20  r...if __name__ 
-00000a20: 3d3d 202e 5f5f 6d61 696e 5f5f 2e3a 0d0a  == .__main__.:..
-00000a30: 0d0a 5b63 6f76 6572 6167 653a 6874 6d6c  ..[coverage:html
-00000a40: 5d0d 0a64 6972 6563 746f 7279 203d 2062  ]..directory = b
-00000a50: 7569 6c64 2f63 6f76 6572 6167 650d 0a0d  uild/coverage...
-00000a60: 0a5b 746f 6f6c 3a70 7974 6573 745d 0d0a  .[tool:pytest]..
-00000a70: 6164 646f 7074 7320 3d20 0d0a 7465 7374  addopts = ..test
-00000a80: 7061 7468 7320 3d20 0d0a 092e 0d0a 0974  paths = .......t
-00000a90: 6573 7473 0d0a 6578 636c 7564 6520 3d20  ests..exclude = 
-00000aa0: 0d0a 095f 5f70 7963 6163 6865 5f5f 2c0d  ...__pycache__,.
-00000ab0: 0a09 2e63 6163 6865 2c0d 0a09 2e65 6767  ...cache,....egg
-00000ac0: 732c 0d0a 092e 6769 742c 0d0a 092e 746f  s,....git,....to
-00000ad0: 782c 0d0a 092e 7673 636f 6465 2c0d 0a09  x,....vscode,...
-00000ae0: 6275 696c 642c 0d0a 0964 6973 742c 0d0a  build,...dist,..
-00000af0: 0964 6f63 730d 0a6d 6178 2d6c 696e 652d  .docs..max-line-
-00000b00: 6c65 6e67 7468 203d 2039 390d 0a69 676e  length = 99..ign
-00000b10: 6f72 6520 3d20 4532 3033 2c20 4535 3031  ore = E203, E501
-00000b20: 2c20 5735 3033 2c20 5031 3031 2c20 4130  , W503, P101, A0
-00000b30: 3033 2c20 4e38 3036 2c20 5736 3035 0d0a  03, N806, W605..
-00000b40: 646f 6373 7472 696e 672d 636f 6e76 656e  docstring-conven
-00000b50: 7469 6f6e 203d 2061 6c6c 2020 2320 676f  tion = all  # go
-00000b60: 6f67 6c65 3f0d 0a69 6e6c 696e 652d 7175  ogle?..inline-qu
-00000b70: 6f74 6573 203d 2064 6f75 626c 650d 0a6d  otes = double..m
-00000b80: 756c 7469 6c69 6e65 2d71 756f 7465 7320  ultiline-quotes 
-00000b90: 3d20 2222 220d 0a64 6f63 7374 7269 6e67  = """..docstring
-00000ba0: 2d71 756f 7465 7320 3d20 2222 220d 0a61  -quotes = """..a
-00000bb0: 766f 6964 2d65 7363 6170 6520 3d20 5472  void-escape = Tr
-00000bc0: 7565 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ue....[egg_info]
-00000bd0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000be0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000810: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000820: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
+00000830: 655f 7363 7269 7074 7320 3d20 0d0a 0977  e_scripts = ...w
+00000840: 7367 6964 6176 203d 2077 7367 6964 6176  sgidav = wsgidav
+00000850: 2e73 6572 7665 722e 7365 7276 6572 5f63  .server.server_c
+00000860: 6c69 3a72 756e 0d0a 0d0a 5b63 6865 636b  li:run....[check
+00000870: 2d6d 616e 6966 6573 745d 0d0a 6967 6e6f  -manifest]..igno
+00000880: 7265 203d 200d 0a09 646f 6373 2f73 7068  re = ...docs/sph
+00000890: 696e 782d 6275 696c 640d 0a09 646f 6373  inx-build...docs
+000008a0: 2f73 7068 696e 782d 6275 696c 642f 2a0d  /sphinx-build/*.
+000008b0: 0a0d 0a5b 616c 6961 7365 735d 0d0a 0d0a  ...[aliases]....
+000008c0: 5b63 6f76 6572 6167 653a 7275 6e5d 0d0a  [coverage:run]..
+000008d0: 6272 616e 6368 203d 2054 7275 650d 0a6f  branch = True..o
+000008e0: 6d69 7420 3d20 0d0a 0974 6573 7473 2f2a  mit = ...tests/*
+000008f0: 0d0a 0977 7367 6964 6176 2f70 726f 705f  ...wsgidav/prop_
+00000900: 6d61 6e2f 636f 7563 685f 7072 6f70 6572  man/couch_proper
+00000910: 7479 5f6d 616e 6167 6572 2e70 790d 0a09  ty_manager.py...
+00000920: 7773 6769 6461 762f 7072 6f70 5f6d 616e  wsgidav/prop_man
+00000930: 2f6d 6f6e 676f 5f70 726f 7065 7274 795f  /mongo_property_
+00000940: 6d61 6e61 6765 722e 7079 0d0a 0977 7367  manager.py...wsg
+00000950: 6964 6176 2f73 616d 706c 6573 2f2a 0d0a  idav/samples/*..
+00000960: 0977 7367 6964 6176 2f73 6572 7665 722f  .wsgidav/server/
+00000970: 7275 6e5f 7265 6c6f 6164 696e 675f 7365  run_reloading_se
+00000980: 7276 6572 2e70 790d 0a09 7773 6769 6461  rver.py...wsgida
+00000990: 762f 7365 7276 6572 2f73 6572 7665 725f  v/server/server_
+000009a0: 7361 6d70 6c65 2e70 790d 0a0d 0a5b 636f  sample.py....[co
+000009b0: 7665 7261 6765 3a72 6570 6f72 745d 0d0a  verage:report]..
+000009c0: 7072 6563 6973 696f 6e20 3d20 320d 0a73  precision = 2..s
+000009d0: 6f72 7420 3d20 4e61 6d65 0d0a 6578 636c  ort = Name..excl
+000009e0: 7564 655f 6c69 6e65 7320 3d20 0d0a 0970  ude_lines = ...p
+000009f0: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
+00000a00: 0a09 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00000a10: 202e 5f5f 6d61 696e 5f5f 2e3a 0d0a 0d0a   .__main__.:....
+00000a20: 5b63 6f76 6572 6167 653a 6874 6d6c 5d0d  [coverage:html].
+00000a30: 0a64 6972 6563 746f 7279 203d 2062 7569  .directory = bui
+00000a40: 6c64 2f63 6f76 6572 6167 650d 0a0d 0a5b  ld/coverage....[
+00000a50: 746f 6f6c 3a70 7974 6573 745d 0d0a 6164  tool:pytest]..ad
+00000a60: 646f 7074 7320 3d20 0d0a 7465 7374 7061  dopts = ..testpa
+00000a70: 7468 7320 3d20 0d0a 092e 0d0a 0974 6573  ths = .......tes
+00000a80: 7473 0d0a 6578 636c 7564 6520 3d20 0d0a  ts..exclude = ..
+00000a90: 095f 5f70 7963 6163 6865 5f5f 2c0d 0a09  .__pycache__,...
+00000aa0: 2e63 6163 6865 2c0d 0a09 2e65 6767 732c  .cache,....eggs,
+00000ab0: 0d0a 092e 6769 742c 0d0a 092e 746f 782c  ....git,....tox,
+00000ac0: 0d0a 092e 7673 636f 6465 2c0d 0a09 6275  ....vscode,...bu
+00000ad0: 696c 642c 0d0a 0964 6973 742c 0d0a 0964  ild,...dist,...d
+00000ae0: 6f63 730d 0a6d 6178 2d6c 696e 652d 6c65  ocs..max-line-le
+00000af0: 6e67 7468 203d 2039 390d 0a69 676e 6f72  ngth = 99..ignor
+00000b00: 6520 3d20 4532 3033 2c20 4535 3031 2c20  e = E203, E501, 
+00000b10: 5735 3033 2c20 5031 3031 2c20 4130 3033  W503, P101, A003
+00000b20: 2c20 4e38 3036 2c20 5736 3035 0d0a 646f  , N806, W605..do
+00000b30: 6373 7472 696e 672d 636f 6e76 656e 7469  cstring-conventi
+00000b40: 6f6e 203d 2061 6c6c 2020 2320 676f 6f67  on = all  # goog
+00000b50: 6c65 3f0d 0a69 6e6c 696e 652d 7175 6f74  le?..inline-quot
+00000b60: 6573 203d 2064 6f75 626c 650d 0a6d 756c  es = double..mul
+00000b70: 7469 6c69 6e65 2d71 756f 7465 7320 3d20  tiline-quotes = 
+00000b80: 2222 220d 0a64 6f63 7374 7269 6e67 2d71  """..docstring-q
+00000b90: 756f 7465 7320 3d20 2222 220d 0a61 766f  uotes = """..avo
+00000ba0: 6964 2d65 7363 6170 6520 3d20 5472 7565  id-escape = True
+00000bb0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000bc0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000bd0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `WsgiDAV-4.3.2/tests/test_http.py` & `wsgidav-4.3.3/tests/test_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
     Functional test suite for WsgiDAV.
 
     This test suite uses requests to generate HTTP requests.
 """
```

### Comparing `WsgiDAV-4.3.2/tests/test_litmus.py` & `wsgidav-4.3.3/tests/test_litmus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
-"""
+r"""
 Run the [Litmus test suite](http://www.webdav.org/neon/litmus/) against WsgiDAV
 server.
 
 ## Usage
 
 **NOTE:** replace <HOST_IP> with the real IP address of the test client.
```

### Comparing `WsgiDAV-4.3.2/tests/test_lock_manager.py` & `wsgidav-4.3.3/tests/test_lock_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """Unit test for lock_manager.py"""
 import os
 import unittest
 from tempfile import gettempdir
 from time import sleep
```

### Comparing `WsgiDAV-4.3.2/tests/test_property_manager.py` & `wsgidav-4.3.3/tests/test_property_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """Unit test for property_manager.py"""
 import os
 import unittest
 from tempfile import gettempdir
```

### Comparing `WsgiDAV-4.3.2/tests/test_scripted.py` & `wsgidav-4.3.3/tests/test_scripted.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
     Functional test suite for WsgiDAV.
 
     This test suite uses davclient to generate WebDAV requests.
```

### Comparing `WsgiDAV-4.3.2/tests/test_streaming.py` & `wsgidav-4.3.3/tests/test_streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 
 """
 Unit tests for wsgidav.stream_tools.FileLikeQueue
 """
```

### Comparing `WsgiDAV-4.3.2/tests/test_util.py` & `wsgidav-4.3.3/tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """Unit tests for wsgidav.util"""
 
 import logging
 import logging.handlers
 import sys
```

### Comparing `WsgiDAV-4.3.2/tests/test_wsgidav_app.py` & `wsgidav-4.3.3/tests/test_wsgidav_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
     Unit test for wsgidav HTTP request functionality
 
     This test suite uses webtest.TestApp to send fake requests to the WSGI
     stack.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/__init__.py` & `wsgidav-4.3.3/wsgidav/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Developmental release (to mark 3.0.0 as 'used'. Don't publish this):
         '3.0.0.dev1'
 NOTE:
     When pywin32 is installed, number must be a.b.c for MSI builds?
     "3.0.0a4" seems not to work in this case!
 """
 
-__version__ = "4.3.2"
+__version__ = "4.3.3"
 
 # make version accessible as 'wsgidav.__version__'
 # from wsgidav._version import __version__  # noqa: F401
 
 # Initialize a silent 'wsgidav' logger
 # http://docs.python-guide.org/en/latest/writing/logging/#logging-in-a-library
 # https://docs.python.org/3/howto/logging.html#configuring-logging-for-a-library
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dav_error.py` & `wsgidav-4.3.3/wsgidav/dav_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Implements a DAVError class that is used to signal WebDAV and HTTP errors.
 """
 import datetime
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dav_provider.py` & `wsgidav-4.3.3/wsgidav/dav_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Abstract base class for DAV resource providers.
 
 This module serves these purposes:
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dc/base_dc.py` & `wsgidav-4.3.3/wsgidav/dc/base_dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Abstract base class of a domain controller (used by HTTPAuthenticator).
 
 This ABC serves as base class for DomainControllers and provides some
 default implementations.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dc/nt_dc.py` & `wsgidav-4.3.3/wsgidav/dc/nt_dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implementation of a domain controller that allows users to authenticate against
 a Windows NT domain or a local computer.
 
 Used by HTTPAuthenticator. Only available on linux and macOS.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dc/pam_dc.py` & `wsgidav-4.3.3/wsgidav/dc/pam_dc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implementation of a domain controller that allows users to authenticate against
 a Pluggable Authentication Module ('PAM').
 
 Used by HTTPAuthenticator. Only available on linux and macOS.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dc/simple_dc.py` & `wsgidav-4.3.3/wsgidav/dc/simple_dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Implementation of a domain controller that uses realm/user_name/password mappings
 from the configuration file and uses the share path as realm name.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/default_conf.py` & `wsgidav-4.3.3/wsgidav/default_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 r"""
 ::
 
      _      __         _ ___  ___ _   __
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dir_browser/_dir_browser.py` & `wsgidav-4.3.3/wsgidav/dir_browser/_dir_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI middleware that handles GET requests on collections to display directories.
 """
 import os
 import sys
```

### Comparing `WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/favicon.ico` & `wsgidav-4.3.3/wsgidav/dir_browser/htdocs/favicon.ico`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/logo.png` & `wsgidav-4.3.3/wsgidav/dir_browser/htdocs/logo.png`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/script.js` & `wsgidav-4.3.3/wsgidav/dir_browser/htdocs/script.js`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/style.css` & `wsgidav-4.3.3/wsgidav/dir_browser/htdocs/style.css`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/dir_browser/htdocs/template.html` & `wsgidav-4.3.3/wsgidav/dir_browser/htdocs/template.html`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/error_printer.py` & `wsgidav-4.3.3/wsgidav/error_printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI middleware to catch application thrown DAVErrors and return proper
 responses.
 """
```

### Comparing `WsgiDAV-4.3.2/wsgidav/fs_dav_provider.py` & `wsgidav-4.3.3/wsgidav/fs_dav_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Implementation of a DAV provider that serves resource from a file system.
 
 :class:`~wsgidav.fs_dav_provider.FilesystemProvider` implements a DAV resource
```

### Comparing `WsgiDAV-4.3.2/wsgidav/http_authenticator.py` & `wsgidav-4.3.3/wsgidav/http_authenticator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI middleware for HTTP basic and digest authentication.
 
 Usage::
```

### Comparing `WsgiDAV-4.3.2/wsgidav/lock_man/lock_manager.py` & `wsgidav-4.3.3/wsgidav/lock_man/lock_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Implements the `LockManager` object that provides the locking functionality.
 
 The LockManager requires a LockStorageDict object to implement persistence.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/lock_man/lock_storage.py` & `wsgidav-4.3.3/wsgidav/lock_man/lock_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Implements two storage providers for `LockManager`.
 
 Two alternative lock storage classes are defined here: one in-memory
```

### Comparing `WsgiDAV-4.3.2/wsgidav/lock_man/lock_storage_redis.py` & `wsgidav-4.3.3/wsgidav/lock_man/lock_storage_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 import pickle
 import time
 
 import redis
```

### Comparing `WsgiDAV-4.3.2/wsgidav/mw/base_mw.py` & `wsgidav-4.3.3/wsgidav/mw/base_mw.py`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/mw/cors.py` & `wsgidav-4.3.3/wsgidav/mw/cors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI middleware used for CORS support (optional).
 
 Respond to CORS preflight OPTIONS request and inject CORS headers.
 """
```

### Comparing `WsgiDAV-4.3.2/wsgidav/mw/debug_filter.py` & `wsgidav-4.3.3/wsgidav/mw/debug_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI middleware used for debugging (optional).
 
 This module dumps request and response information to the console, depending
```

### Comparing `WsgiDAV-4.3.2/wsgidav/prop_man/couch_property_manager.py` & `wsgidav-4.3.3/wsgidav/prop_man/couch_property_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implements a property manager based on CouchDB.
 
 
 http://wiki.apache.org/couchdb/Reference
 http://packages.python.org/CouchDB/views.html
@@ -111,15 +111,15 @@
     def _dump(self, msg="", out=None):
         pass
 
     def _find(self, url):
         """Return properties document for path."""
         # Query the permanent view to find a url
         vr = self.db.view("properties/by_url", key=url, include_docs=True)
-        _logger.debug("find(%r) returned %s" % (url, len(vr)))
+        _logger.debug(f"find({url!r}) returned {len(vr)}")
         assert len(vr) <= 1, "Found multiple matches for %r" % url
         for row in vr:
             assert row.doc
             return row.doc
         return None
 
     def _find_descendents(self, url):
@@ -144,15 +144,15 @@
         propNames = []
         if doc:
             for name in doc["properties"].keys():
                 propNames.append(name)
         return propNames
 
     def get_property(self, norm_url, name, environ=None):
-        _logger.debug("get_property(%s, %s)" % (norm_url, name))
+        _logger.debug(f"get_property({norm_url}, {name})")
         doc = self._find(norm_url)
         if not doc:
             return None
         prop = doc["properties"].get(name)
         return prop
 
     def write_property(
@@ -179,15 +179,15 @@
                 "title": quote(norm_url),
                 "type": "properties",
                 "properties": {name: property_value},
             }
         self.db.save(doc)
 
     def remove_property(self, norm_url, name, dry_run=False, environ=None):
-        _logger.debug("remove_property(%s, %s, dry_run=%s)" % (norm_url, name, dry_run))
+        _logger.debug(f"remove_property({norm_url}, {name}, dry_run={dry_run})")
         if dry_run:
             # TODO: can we check anything here?
             return
         doc = self._find(norm_url)
         # Specifying the removal of a property that does not exist is NOT an error.
         if not doc or doc["properties"].get(name) is None:
             return
@@ -201,44 +201,44 @@
             self.db.delete(doc)
         return
 
     def copy_properties(self, srcUrl, destUrl, environ=None):
         doc = self._find(srcUrl)
         if not doc:
             _logger.debug(
-                "copy_properties(%s, %s): src has no properties" % (srcUrl, destUrl)
+                f"copy_properties({srcUrl}, {destUrl}): src has no properties"
             )
             return
-        _logger.debug("copy_properties(%s, %s)" % (srcUrl, destUrl))
+        _logger.debug(f"copy_properties({srcUrl}, {destUrl})")
         assert not self._find(destUrl)
         doc2 = {
             "_id": uuid4().hex,
             "url": destUrl,
             "title": quote(destUrl),
             "type": "properties",
             "properties": doc["properties"],
         }
         self.db.save(doc2)
 
     def move_properties(self, srcUrl, destUrl, with_children, environ=None):
-        _logger.debug("move_properties(%s, %s, %s)" % (srcUrl, destUrl, with_children))
+        _logger.debug(f"move_properties({srcUrl}, {destUrl}, {with_children})")
         if with_children:
             # Match URLs that are equal to <srcUrl> or begin with '<srcUrl>/'
             docList = self._find_descendents(srcUrl)
             for doc in docList:
                 newDest = doc["url"].replace(srcUrl, destUrl)
-                _logger.debug("move property %s -> %s" % (doc["url"], newDest))
+                _logger.debug("move property {} -> {}".format(doc["url"], newDest))
                 doc["url"] = newDest
                 self.db.save(doc)
         else:
             # Move srcUrl only
             # TODO: use findAndModify()?
             doc = self._find(srcUrl)
             if doc:
-                _logger.debug("move property %s -> %s" % (doc["url"], destUrl))
+                _logger.debug("move property {} -> {}".format(doc["url"], destUrl))
                 doc["url"] = destUrl
                 self.db.save(doc)
         return
 
 
 # ============================================================================
 #
```

### Comparing `WsgiDAV-4.3.2/wsgidav/prop_man/mongo_property_manager.py` & `wsgidav-4.3.3/wsgidav/prop_man/mongo_property_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implements a property manager based on MongoDB.
 
 Usage: add this lines to wsgidav.conf::
 
     from wsgidav.prop_man.mongo_property_manager import MongoPropertyManager
@@ -108,15 +108,15 @@
         if doc:
             for name in doc.keys():
                 if name not in HIDDEN_KEYS:
                     propNames.append(decode_mongo_key(name))
         return propNames
 
     def get_property(self, norm_url, name, environ=None):
-        _logger.debug("get_property(%s, %s)" % (norm_url, name))
+        _logger.debug(f"get_property({norm_url}, {name})")
         doc = self.collection.find_one({"_url": norm_url})
         if not doc:
             return None
         prop = doc.get(encode_mongo_key(name))
         return prop
 
     def write_property(
@@ -138,15 +138,15 @@
         if not doc:
             doc = {"_url": norm_url, "_title": quote(norm_url)}
         doc[encode_mongo_key(name)] = property_value
         self.collection.save(doc)
 
     def remove_property(self, norm_url, name, dry_run=False, environ=None):
         """ """
-        _logger.debug("remove_property(%s, %s, dry_run=%s)" % (norm_url, name, dry_run))
+        _logger.debug(f"remove_property({norm_url}, {name}, dry_run={dry_run})")
         if dry_run:
             # TODO: can we check anything here?
             return
         doc = self.collection.find_one({"_url": norm_url})
         # Specifying the removal of a property that does not exist is NOT an error.
         if not doc or doc.get(encode_mongo_key(name)) is None:
             return
@@ -160,35 +160,35 @@
             self.collection.remove(doc)
         return
 
     def copy_properties(self, srcUrl, destUrl, environ=None):
         doc = self.collection.find_one({"_url": srcUrl})
         if not doc:
             _logger.debug(
-                "copy_properties(%s, %s): src has no properties" % (srcUrl, destUrl)
+                f"copy_properties({srcUrl}, {destUrl}): src has no properties"
             )
             return
-        _logger.debug("copy_properties(%s, %s)" % (srcUrl, destUrl))
+        _logger.debug(f"copy_properties({srcUrl}, {destUrl})")
         doc2 = doc.copy()
         self.collection.insert(doc2)
 
     def move_properties(self, srcUrl, destUrl, with_children, environ=None):
-        _logger.debug("move_properties(%s, %s, %s)" % (srcUrl, destUrl, with_children))
+        _logger.debug(f"move_properties({srcUrl}, {destUrl}, {with_children})")
         if with_children:
             # Match URLs that are equal to <srcUrl> or begin with '<srcUrl>/'
             matchBegin = "^" + srcUrl.rstrip("/") + "/"
             query = {"$or": [{"_url": srcUrl}, {"_url": {"$regex": matchBegin}}]}
             docList = self.collection.find(query)
             for doc in docList:
                 newDest = doc["_url"].replace(srcUrl, destUrl)
-                _logger.debug("move property %s -> %s" % (doc["_url"], newDest))
+                _logger.debug("move property {} -> {}".format(doc["_url"], newDest))
                 doc["_url"] = newDest
                 self.collection.save(doc)
         else:
             # Move srcUrl only
             # TODO: use findAndModify()?
             doc = self.collection.find_one({"_url": srcUrl})
             if doc:
-                _logger.debug("move property %s -> %s" % (doc["_url"], destUrl))
+                _logger.debug("move property {} -> {}".format(doc["_url"], destUrl))
                 doc["_url"] = destUrl
                 self.collection.save(doc)
         return
```

### Comparing `WsgiDAV-4.3.2/wsgidav/prop_man/property_manager.py` & `wsgidav-4.3.3/wsgidav/prop_man/property_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Implements two property managers: one in-memory (dict-based), and one
 persistent low performance variant using shelve.
 
@@ -87,15 +87,15 @@
             self._lock.release()
 
     def _check(self, msg=""):
         try:
             if not self._loaded:
                 return True
             for k, v in self._dict.items():
-                _dummy = "{}, {}".format(k, v)  # noqa
+                _dummy = f"{k}, {v}"  # noqa
             #            _logger.debug("{} checks ok {}".format(self.__class__.__name__, msg))
             return True
         except Exception:
             _logger.exception(f"{self.__class__.__name__} _check: ERROR {msg}")
             return False
 
     def _dump(self, msg=""):
```

### Comparing `WsgiDAV-4.3.2/wsgidav/request_resolver.py` & `wsgidav-4.3.3/wsgidav/request_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI middleware that finds the registered mapped DAV-Provider, creates a new
 RequestServer instance, and dispatches the request.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/request_server.py` & `wsgidav-4.3.3/wsgidav/request_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 WSGI application that handles one single WebDAV request.
 """
 from urllib.parse import unquote, urlparse
@@ -110,29 +110,26 @@
 
             profile = Profile()
             res = profile.runcall(
                 provider.custom_request_handler, environ, start_response, method
             )
             # sort: 0:"calls",1:"time", 2: "cumulative"
             profile.print_stats(sort=2)
-            for v in res:
-                yield v
+            yield from res
             if hasattr(res, "close"):
                 res.close()
             return
 
         # Run requesthandler (provider may override, #55)
         # _logger.warning("#1...")
         app_iter = provider.custom_request_handler(environ, start_response, method)
         # _logger.warning("#1... 2")
         try:
             # _logger.warning("#1... 3")
-            for v in app_iter:
-                # _logger.warning("#1... 4")
-                yield v
+            yield from app_iter
             # _logger.warning("#1... 5")
         # except Exception:
         #     _logger.warning("#1... 6")
         #     _logger.exception("")
         #     status = "500 Oops"
         #     response_headers = [("content-type", "text/plain")]
         #     start_response(status, response_headers, sys.exc_info())
```

### Comparing `WsgiDAV-4.3.2/wsgidav/rw_lock.py` & `wsgidav-4.3.3/wsgidav/rw_lock.py`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/samples/dav_provider_tools.py` & `wsgidav-4.3.3/wsgidav/samples/dav_provider_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Tools that make it easier to implement custom WsgiDAV providers.
 """
 import os
 import stat
```

### Comparing `WsgiDAV-4.3.2/wsgidav/samples/hg_dav_provider.py` & `wsgidav-4.3.3/wsgidav/samples/hg_dav_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 DAV provider that publishes a Mercurial repository.
 
 Note: This is **not** production code!
 
 The repository is rendered as three top level collections.
@@ -171,15 +171,15 @@
         # statresults = os.stat(self._file_path)
         # return statresults[stat.ST_CTIME]
         return None  # TODO
 
     def get_display_name(self):
         if self.is_collection or self.fctx.filerev() is None:
             return self.name
-        return "%s@%s" % (self.name, self.fctx.filerev())
+        return f"{self.name}@{self.fctx.filerev()}"
 
     def get_etag(self):
         return (
             md5(self.path).hexdigest()
             + "-"
             + util.to_str(self.get_last_modified())
             + "-"
@@ -364,41 +364,41 @@
 
     def handle_copy(self, dest_path, *, depth_infinity):
         """Handle a COPY request natively."""
         destType, destHgPath = util.pop_path(dest_path)
         destHgPath = destHgPath.strip("/")
         ui = self.provider.ui
         repo = self.provider.repo
-        _logger.info("handle_copy %s -> %s" % (self.localHgPath, destHgPath))
+        _logger.info(f"handle_copy {self.localHgPath} -> {destHgPath}")
         if self.rev is None and destType == "edit":
             # COPY /edit/a/b to /edit/c/d: turn into 'hg copy -f a/b c/d'
             commands.copy(ui, repo, self.localHgPath, destHgPath, force=True)
         elif self.rev is None and destType == "released":
             # COPY /edit/a/b to /released/c/d
             # This is interpreted as 'hg commit a/b' (ignoring the dest. path)
-            self._commit("WsgiDAV commit (COPY %s -> %s)" % (self.path, dest_path))
+            self._commit(f"WsgiDAV commit (COPY {self.path} -> {dest_path})")
         else:
             raise DAVError(HTTP_FORBIDDEN)
         # Return True: request was handled
         return True
 
     def handle_move(self, dest_path):
         """Handle a MOVE request natively."""
         destType, destHgPath = util.pop_path(dest_path)
         destHgPath = destHgPath.strip("/")
         ui = self.provider.ui
         repo = self.provider.repo
-        _logger.info("handle_copy %s -> %s" % (self.localHgPath, destHgPath))
+        _logger.info(f"handle_copy {self.localHgPath} -> {destHgPath}")
         if self.rev is None and destType == "edit":
             # MOVE /edit/a/b to /edit/c/d: turn into 'hg rename -f a/b c/d'
             commands.rename(ui, repo, self.localHgPath, destHgPath, force=True)
         elif self.rev is None and destType == "released":
             # MOVE /edit/a/b to /released/c/d
             # This is interpreted as 'hg commit a/b' (ignoring the dest. path)
-            self._commit("WsgiDAV commit (MOVE %s -> %s)" % (self.path, dest_path))
+            self._commit(f"WsgiDAV commit (MOVE {self.path} -> {dest_path})")
         else:
             raise DAVError(HTTP_FORBIDDEN)
         # Return True: request was handled
         return True
 
 
 # ============================================================================
@@ -542,22 +542,22 @@
                     p2 = parents[i]
                     dir = dirinfos.setdefault(p1, ([], []))
                     if p2 not in dir[0]:
                         dir[0].append(p2)
                     if p1 == "":
                         p1 = p2
                     else:
-                        p1 = "%s/%s" % (p1, p2)
+                        p1 = f"{p1}/{p2}"
                 dirinfos.setdefault(p1, ([], []))[1].append(parents[-1])
             filedict[file] = True
         files.sort()
 
         cache = {"files": files, "dirinfos": dirinfos, "filedict": filedict}
         caches[util.to_str(rev)] = cache
-        _logger.info("_getRepoInfo(%s) took %.3f" % (rev, time.time() - start_time))
+        _logger.info(f"_getRepoInfo({rev}) took {time.time() - start_time:.3f}")
         return cache
 
     #    def _listMembers(self, path, rev=None):
     #        """Return a list of all non-collection members"""
     #        # Pattern for direct members:
     #        glob = "glob:" + os.path.join(path, "*").lstrip("/")
     #        print(glob)
```

### Comparing `WsgiDAV-4.3.2/wsgidav/samples/mongo_dav_provider.py` & `wsgidav-4.3.3/wsgidav/samples/mongo_dav_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implementation of a WebDAV provider that provides a very basic, read-only
 resource layer emulation of a MongoDB database.
 
 Usage: add the following entries to wsgidav.conf::
```

### Comparing `WsgiDAV-4.3.2/wsgidav/samples/mysql_dav_provider.py` & `wsgidav-4.3.3/wsgidav/samples/mysql_dav_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implementation of a WebDAV provider that provides a very basic, read-only
 resource layer emulation of a MySQL database.
 
 This module is specific to the WsgiDAV application. It provides a
@@ -254,15 +254,15 @@
         propNames = super().get_property_names(is_allprop=is_allprop)
         # Add fieldnames as properties
         tableName, primKey = self.provider._split_path(self.path)
         if primKey is not None:
             conn = self.provider._init_connection()
             fieldlist = self.provider._get_field_list(conn, tableName)
             for fieldname in fieldlist:
-                propNames.append("{%s:}%s" % (tableName, fieldname))
+                propNames.append(f"{{{tableName}:}}{fieldname}")
             conn.close()
         return propNames
 
     def get_property_value(self, name):
         """Return the value of a property.
 
         The base implementation handles:
@@ -312,20 +312,15 @@
         self._host = host
         self._user = user
         self._passwd = passwd
         self._db = db
         self._count_initConnection = 0
 
     def __repr__(self):
-        return "%s for db '%s' on '%s' (user: '%s')'" % (
-            self.__class__.__name__,
-            self._db,
-            self._host,
-            self._user,
-        )
+        return f"{self.__class__.__name__} for db '{self._db}' on '{self._host}' (user: '{self._user}')'"
 
     def _split_path(self, path):
         """Return (tableName, primaryKey) tuple for a request path."""
         if path.strip() in (None, "", "/"):
             return (None, None)
         tableName, primKey = util.save_split(path.strip("/"), "/", 1)
         #        _logger.debug("'%s' -> ('%s', '%s')" % (path, tableName, primKey))
```

### Comparing `WsgiDAV-4.3.2/wsgidav/samples/virtual_dav_provider.py` & `wsgidav-4.3.3/wsgidav/samples/virtual_dav_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Sample implementation of a DAV provider that provides a browsable,
 multi-categorized resource tree.
 
 Note that this is simply an example with no concrete real world benefit.
 But it demonstrates some techniques to customize WsgiDAV.
@@ -475,20 +475,20 @@
     def get_display_info(self):
         return {"type": "Virtual info file"}
 
     def prevent_locking(self):
         return True
 
     def get_ref_url(self):
-        refPath = "/by_key/%s/%s" % (self.data["key"], self.name)
+        refPath = "/by_key/{}/{}".format(self.data["key"], self.name)
         return quote(self.provider.share_path + refPath)
 
     def get_content(self):
         fileLinks = [
-            "<a href='%s'>%s</a>\n" % (os.path.basename(f), f)
+            f"<a href='{os.path.basename(f)}'>{f}</a>\n"
             for f in self.data["resPathList"]
         ]
         dict = self.data.copy()
         dict["fileLinks"] = ", ".join(fileLinks)
         if self.name == ".Info.html":
             html = (
                 """\
@@ -574,15 +574,17 @@
         return {"type": "Content file"}
 
     def get_last_modified(self):
         statresults = os.stat(self.file_path)
         return statresults[stat.ST_MTIME]
 
     def get_ref_url(self):
-        refPath = "/by_key/%s/%s" % (self.data["key"], os.path.basename(self.file_path))
+        refPath = "/by_key/{}/{}".format(
+            self.data["key"], os.path.basename(self.file_path)
+        )
         return quote(self.provider.share_path + refPath)
 
     def get_content(self):
         # mime = self.get_content_type()
         # GC issue 57: always store as binary
         # if mime.startswith("text"):
         #     return open(self.file_path, "r", BUFFER_SIZE)
```

### Comparing `WsgiDAV-4.3.2/wsgidav/server/ext_wsgiutils_server.py` & `wsgidav-4.3.3/wsgidav/server/ext_wsgiutils_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 ext_wsgiutils_server.py is an extension of the wsgiutils server in Paste.
 It supports passing all of the HTTP and WebDAV (rfc 2518) methods.
 
 It includes code from the following sources:
```

### Comparing `WsgiDAV-4.3.2/wsgidav/server/run_reloading_server.py` & `wsgidav-4.3.3/wsgidav/server/run_reloading_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Wrapper for ``server_cli``, that restarts the server when source code is
 modified.
 """
 import os
 import sys
```

### Comparing `WsgiDAV-4.3.2/wsgidav/server/server_cli.py` & `wsgidav-4.3.3/wsgidav/server/server_cli.py`

 * *Files identical despite different names*

### Comparing `WsgiDAV-4.3.2/wsgidav/server/server_sample.py` & `wsgidav-4.3.3/wsgidav/server/server_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Simple example how to a run WsgiDAV in a 3rd-party WSGI server.
 """
 from cheroot import wsgi
```

### Comparing `WsgiDAV-4.3.2/wsgidav/stream_tools.py` & `wsgidav-4.3.3/wsgidav/stream_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Implement the FileLikeQueue helper class.
 
 This helper class is intended to handle use cases where an incoming PUT
 request should be directly streamed to a remote target.
```

### Comparing `WsgiDAV-4.3.2/wsgidav/util.py` & `wsgidav-4.3.3/wsgidav/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/m ar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/m ar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Miscellaneous support functions for WsgiDAV.
 """
 import base64
```

### Comparing `WsgiDAV-4.3.2/wsgidav/wsgidav_app.py` & `wsgidav-4.3.3/wsgidav/wsgidav_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 r"""
 ::
 
      _      __         _ ___  ___ _   __
@@ -128,15 +128,15 @@
     if errors:
         raise ValueError("Invalid configuration:\n  - " + "\n  - ".join(errors))
 
     return True
 
 
 #: Minimal Python version that is supported by WsgiDAV
-MIN_PYTHON_VERSION_INFO = (3, 8)
+MIN_PYTHON_VERSION_INFO = (3, 9)
 
 check_python_version(MIN_PYTHON_VERSION_INFO)
 
 
 # ========================================================================
 # WsgiDAVApp
 # ========================================================================
```

### Comparing `WsgiDAV-4.3.2/wsgidav/xml_tools.py` & `wsgidav-4.3.3/wsgidav/xml_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# (c) 2009-2023 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
+# (c) 2009-2024 Martin Wendt and contributors; see WsgiDAV https://github.com/mar10/wsgidav
 # Original PyFileServer (c) 2005 Ho Chun Wei.
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/mit-license.php
 """
 Small wrapper for different etree packages.
 """
 import logging
```

