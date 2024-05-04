# Comparing `tmp/dragonlog-1.1.2.tar.gz` & `tmp/dragonlog-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonlog-1.1.2.tar", last modified: Sun Apr 28 08:33:03 2024, max compression
+gzip compressed data, was "dragonlog-1.1.3.tar", last modified: Sat May  4 07:20:06 2024, max compression
```

## Comparing `dragonlog-1.1.2.tar` & `dragonlog-1.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.228769 dragonlog-1.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.218980 dragonlog-1.1.2/DragonLog.egg-info/
--rw-rw-rw-   0        0        0     7401 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1603 2024-04-28 08:33:03.000000 dragonlog-1.1.2/DragonLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-28 08:33:02.000000 dragonlog-1.1.2/DragonLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.1.2/LICENCE.txt
--rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7401 2024-04-28 08:33:03.224316 dragonlog-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.105147 dragonlog-1.1.2/dragonlog/
--rw-rw-rw-   0        0        0    10562 2024-04-15 18:06:37.000000 dragonlog-1.1.2/dragonlog/CallBook.py
--rw-rw-rw-   0        0        0    63750 2024-04-21 09:50:28.000000 dragonlog-1.1.2/dragonlog/DragonLog.py
--rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.1.2/dragonlog/DragonLog_AppSelect.py
--rw-rw-rw-   0        0        0     3041 2024-04-28 08:31:54.000000 dragonlog-1.1.2/dragonlog/DragonLog_AppSelect_ui.py
--rw-rw-rw-   0        0        0    17410 2024-04-28 08:31:53.000000 dragonlog-1.1.2/dragonlog/DragonLog_MainWindow_ui.py
--rw-rw-rw-   0        0        0    47332 2024-04-28 08:25:13.000000 dragonlog-1.1.2/dragonlog/DragonLog_QSOForm.py
--rw-rw-rw-   0        0        0    38980 2024-04-28 08:31:54.000000 dragonlog-1.1.2/dragonlog/DragonLog_QSOForm_ui.py
--rw-rw-rw-   0        0        0    21133 2024-04-18 06:08:40.000000 dragonlog-1.1.2/dragonlog/DragonLog_Settings.py
--rw-rw-rw-   0        0        0    39219 2024-04-28 08:31:54.000000 dragonlog-1.1.2/dragonlog/DragonLog_Settings_ui.py
--rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.1.2/dragonlog/LoTW.py
--rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.1.2/dragonlog/Logger.py
--rw-rw-rw-   0        0        0     1134 2024-04-15 17:33:29.000000 dragonlog-1.1.2/dragonlog/RegEx.py
--rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.1.2/dragonlog/__init__.py
--rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.1.2/dragonlog/__main__.py
--rw-rw-rw-   0        0        0       65 2024-04-28 08:31:53.000000 dragonlog-1.1.2/dragonlog/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.117605 dragonlog-1.1.2/dragonlog/data/
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.2/dragonlog/data/README.md
--rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.1.2/dragonlog/data/bands.json
--rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.1.2/dragonlog/data/cb_channels.json
--rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.1.2/dragonlog/data/color_map.json
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.125869 dragonlog-1.1.2/dragonlog/data/i18n/
--rw-rw-rw-   0        0        0    24604 2024-04-28 08:31:57.000000 dragonlog-1.1.2/dragonlog/data/i18n/DragonLog_de.qm
--rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.1.2/dragonlog/data/i18n/ascii_replace_de.json
--rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.1.2/dragonlog/data/modes.json
--rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.1.2/dragonlog/eQSL.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:03.211747 dragonlog-1.1.2/dragonlog/icons/
--rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.1.2/dragonlog/icons/Screenshot.png
--rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.1.2/dragonlog/icons/db.png
--rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.1.2/dragonlog/icons/edit.png
--rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.1.2/dragonlog/icons/edit_add.png
--rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.1.2/dragonlog/icons/edit_addmulti.png
--rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.1.2/dragonlog/icons/edit_addmulti.xcf
--rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.1.2/dragonlog/icons/edit_remove.png
--rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.1.2/dragonlog/icons/exit.png
--rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.1.2/dragonlog/icons/file_doc.png
--rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.1.2/dragonlog/icons/fileexport.png
--rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.1.2/dragonlog/icons/fileimport.png
--rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.1.2/dragonlog/icons/gear.png
--rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.1.2/dragonlog/icons/help.png
--rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.png
--rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.xcf
--rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.1.2/dragonlog/icons/info.png
--rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.1.2/dragonlog/icons/logo.ico
--rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.1.2/dragonlog/icons/no.png
--rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.1.2/dragonlog/icons/ok.png
--rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.1.2/dragonlog/icons/player_play.png
--rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.1.2/dragonlog/icons/player_stop.png
--rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.1.2/dragonlog/icons/upload_lotw.png
--rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.1.2/dragonlog/icons/upload_lotw.xcf
--rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.1.2/dragonlog/icons/watch.png
--rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 08:33:03.229806 dragonlog-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.1.2/setup_msi.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.155683 dragonlog-1.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.155683 dragonlog-1.1.3/DragonLog.egg-info/
+-rw-rw-rw-   0        0        0     7401 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1603 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.1.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7401 2024-05-04 07:20:06.155683 dragonlog-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.071051 dragonlog-1.1.3/dragonlog/
+-rw-rw-rw-   0        0        0    10600 2024-04-30 18:45:39.000000 dragonlog-1.1.3/dragonlog/CallBook.py
+-rw-rw-rw-   0        0        0    63825 2024-05-02 14:23:02.000000 dragonlog-1.1.3/dragonlog/DragonLog.py
+-rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.1.3/dragonlog/DragonLog_AppSelect.py
+-rw-rw-rw-   0        0        0     3041 2024-05-04 07:18:54.000000 dragonlog-1.1.3/dragonlog/DragonLog_AppSelect_ui.py
+-rw-rw-rw-   0        0        0    17410 2024-05-04 07:18:53.000000 dragonlog-1.1.3/dragonlog/DragonLog_MainWindow_ui.py
+-rw-rw-rw-   0        0        0    47609 2024-05-03 15:13:12.000000 dragonlog-1.1.3/dragonlog/DragonLog_QSOForm.py
+-rw-rw-rw-   0        0        0    38980 2024-05-04 07:18:53.000000 dragonlog-1.1.3/dragonlog/DragonLog_QSOForm_ui.py
+-rw-rw-rw-   0        0        0    22179 2024-05-03 15:13:12.000000 dragonlog-1.1.3/dragonlog/DragonLog_Settings.py
+-rw-rw-rw-   0        0        0    39219 2024-05-04 07:18:54.000000 dragonlog-1.1.3/dragonlog/DragonLog_Settings_ui.py
+-rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.1.3/dragonlog/LoTW.py
+-rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.1.3/dragonlog/Logger.py
+-rw-rw-rw-   0        0        0     1134 2024-04-15 17:33:29.000000 dragonlog-1.1.3/dragonlog/RegEx.py
+-rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.1.3/dragonlog/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.1.3/dragonlog/__main__.py
+-rw-rw-rw-   0        0        0       65 2024-05-04 07:18:52.000000 dragonlog-1.1.3/dragonlog/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.086675 dragonlog-1.1.3/dragonlog/data/
+-rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.3/dragonlog/data/README.md
+-rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.1.3/dragonlog/data/bands.json
+-rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.1.3/dragonlog/data/cb_channels.json
+-rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.1.3/dragonlog/data/color_map.json
+drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.086675 dragonlog-1.1.3/dragonlog/data/i18n/
+-rw-rw-rw-   0        0        0    24719 2024-05-04 07:18:57.000000 dragonlog-1.1.3/dragonlog/data/i18n/DragonLog_de.qm
+-rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.1.3/dragonlog/data/i18n/ascii_replace_de.json
+-rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.1.3/dragonlog/data/modes.json
+-rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.1.3/dragonlog/eQSL.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.155683 dragonlog-1.1.3/dragonlog/icons/
+-rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.1.3/dragonlog/icons/Screenshot.png
+-rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.1.3/dragonlog/icons/db.png
+-rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.1.3/dragonlog/icons/edit.png
+-rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.1.3/dragonlog/icons/edit_add.png
+-rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.1.3/dragonlog/icons/edit_addmulti.png
+-rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.1.3/dragonlog/icons/edit_addmulti.xcf
+-rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.1.3/dragonlog/icons/edit_remove.png
+-rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.1.3/dragonlog/icons/exit.png
+-rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.1.3/dragonlog/icons/file_doc.png
+-rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.1.3/dragonlog/icons/fileexport.png
+-rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.1.3/dragonlog/icons/fileimport.png
+-rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.1.3/dragonlog/icons/gear.png
+-rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.1.3/dragonlog/icons/help.png
+-rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.png
+-rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.xcf
+-rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.1.3/dragonlog/icons/info.png
+-rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.1.3/dragonlog/icons/logo.ico
+-rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.1.3/dragonlog/icons/no.png
+-rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.1.3/dragonlog/icons/ok.png
+-rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.1.3/dragonlog/icons/player_play.png
+-rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.1.3/dragonlog/icons/player_stop.png
+-rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.1.3/dragonlog/icons/upload_lotw.png
+-rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.1.3/dragonlog/icons/upload_lotw.xcf
+-rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.1.3/dragonlog/icons/watch.png
+-rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 07:20:06.155683 dragonlog-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.1.3/setup_msi.py
```

### Comparing `dragonlog-1.1.2/DragonLog.egg-info/PKG-INFO` & `dragonlog-1.1.3/DragonLog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.1.2
+Version: 1.1.3
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonlog-1.1.2/DragonLog.egg-info/SOURCES.txt` & `dragonlog-1.1.3/DragonLog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/PKG-INFO` & `dragonlog-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.1.2
+Version: 1.1.3
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonlog-1.1.2/README.md` & `dragonlog-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/CallBook.py` & `dragonlog-1.1.3/dragonlog/CallBook.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         except CommunicationException as exc:
             raise RequestException(str(exc))
 
         match res:
             case {'QRZCQDatabase': {'Session': {'Error': error}}}:
                 if error == 'Session does not exist or expired':
                     raise SessionExpiredException('QRZCQ')
-                elif error.startswith('Not found'):
+                elif error.startswith('Not found') or error.startswith('Callsign Empty'):
                     raise CallsignNotFoundException(callsign)
                 else:
                     raise RequestException(f"QRZCQ error: {error}")
             case {'QRZCQDatabase': {'Callsign': data}}:
                 if data:
                     return CallBookData(
                         callsign,
```

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog.py` & `dragonlog-1.1.3/dragonlog/DragonLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
         self.settings_form = Settings(self, self.settings, self.hamlib_status, self.__headers__, self.log)
 
         # QSOForm
         self.qso_form = QSOForm(self, self, self.bands, self.modes, self.prop, self.settings, self.settings_form,
                                 self.cb_channels, self.hamlib_error, self.log)
         self.qsoDockWidget.setWidget(self.qso_form)
         self.qsoDockWidget.visibilityChanged.connect(self.qso_form.startTimers)
+        self.qsoDockWidget.visibilityChanged.connect(self.qso_form.clear)
 
         if int(self.settings.value('ui/qso_dock_float', 0)):
             self.qsoDockWidget.setFloating(True)
         else:
             qso_dock_area = self.int2dock_area(int(self.settings.value('ui/qso_dock_area',
                                                                        QtCore.Qt.DockWidgetArea.RightDockWidgetArea.value)))
             self.addDockWidget(qso_dock_area,
```

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_AppSelect.py` & `dragonlog-1.1.3/dragonlog/DragonLog_AppSelect.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_AppSelect_ui.py` & `dragonlog-1.1.3/dragonlog/DragonLog_AppSelect_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_MainWindow_ui.py` & `dragonlog-1.1.3/dragonlog/DragonLog_MainWindow_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_QSOForm.py` & `dragonlog-1.1.3/dragonlog/DragonLog_QSOForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
                           'PKTLSB': ('SSB', 'LSB'),
                           }
         self.__last_mode__ = ''
         self.__last_band__ = ''
         self.__last_freq__ = 0.0
         self.__last_pwr__ = ''
 
+        self.settings_form.rigctldStatusChanged.connect(self.rigctldChanged)
+
         self.__change_mode__ = False
 
         self.refreshTimer = QtCore.QTimer(self)
         self.refreshTimer.timeout.connect(self.refreshRigData)
 
         self.timeTimer = QtCore.QTimer(self)
         self.timeTimer.timeout.connect(self.refreshTime)
@@ -124,14 +126,20 @@
 
         for w in view_only_widgets:
             w.setAttribute(QtCore.Qt.WidgetAttribute.WA_TransparentForMouseEvents)
             w.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
 
         self.clear()
 
+    def rigctldChanged(self, state):
+        self.__last_mode__ = ''
+        self.__last_band__ = ''
+        self.__last_freq__ = 0.0
+        self.__last_pwr__ = ''
+
     def startTimers(self, start: bool):
         if start:
             self.refreshTimer.start(500)
             self.timeTimer.start(1000)
         else:
             self.refreshTimer.stop()
             self.timeTimer.stop()
@@ -266,42 +274,39 @@
         self.nameLineEdit.clear()
         self.QTHLineEdit.clear()
         self.locatorLineEdit.clear()
         self.RSTSentLineEdit.setText('59')
         self.RSTRcvdLineEdit.setText('59')
         self.commentLineEdit.clear()
         self.remarksTextEdit.clear()
-        self.powerSpinBox.setValue(0)
 
         self.callSignChanged('')
         self.locatorChanged('')
         self.ownCallSignChanged(self.ownCallSignLineEdit.text())
         self.ownLocatorChanged(self.ownLocatorLineEdit.text())
         self.rstSentChanged(self.RSTSentLineEdit.text())
         self.rstRcvdChanged(self.RSTRcvdLineEdit.text())
 
         dt = QtCore.QDateTime.currentDateTimeUtc()
         self.dateOffEdit.setDate(dt.date())
         self.dateOnEdit.setDate(dt.date())
-        self.timeOffEdit.setText(dt.time().toString('HH:mm:ss'))
-        self.timeOffChanged(self.timeOffEdit.text())
+        if self.autoDateCheckBox.isChecked():
+            self.timeOffEdit.setText(dt.time().toString('HH:mm:ss'))
         self.timeOnEdit.setText('')
         self.timeOnChanged('')
 
         if bool(self.settings.value('station_cb/cb_by_default', 0)):
             self.bandComboBox.setCurrentText('11m')
 
         if self.bandComboBox.currentIndex() < 0:
             self.bandComboBox.setCurrentIndex(0)
+            self.submodeComboBox.setCurrentIndex(-1)
         if self.modeComboBox.currentIndex() < 0:
             self.modeComboBox.setCurrentIndex(0)
 
-        self.submodeComboBox.setCurrentIndex(-1)
-        self.propComboBox.setCurrentIndex(-1)
-
         self.qslBurDirGroupBox.setChecked(False)
         self.qslViaLineEdit.clear()
         self.qslBureauRadioButton.setChecked(False)
         self.qslDirectRadioButton.setChecked(False)
         self.qslAccBureauCheckBox.setChecked(False)
         self.qslAccDirectCheckBox.setChecked(False)
         self.qslAcceQSLCheckBox.setChecked(False)
@@ -320,14 +325,15 @@
         self.lotwSentCheckBox.setChecked(False)
         self.lotwRcvdCheckBox.setChecked(False)
         self.lotwInboxPushButton.setEnabled(False)
 
         self.hamQTHCheckBox.setChecked(False)
 
         self.toolBox.setCurrentIndex(0)
+        self.callSignLineEdit.setFocus()
 
     def reset(self):
         self.autoDateCheckBox.setEnabled(True)
         self.autoDateCheckBox.setChecked(True)
         self.stationGroupBox.setChecked(True)
         self.identityGroupBox.setChecked(True)
 
@@ -353,14 +359,15 @@
             self.identityGroupBox.setTitle(self.tr('Configured identity'))
             self.identityGroupBox.setChecked(True)
             self.autoDateCheckBox.setChecked(True)
             self.autoDateCheckBox.setEnabled(True)
             self.timeNowPushButton.setEnabled(True)
 
     def bandChanged(self, band: str):
+        self.__last_band__ = band
         self.freqDoubleSpinBox.setMinimum(self.bands[band][0] - self.bands[band][2])
         self.freqDoubleSpinBox.setValue(self.bands[band][0] - self.bands[band][2])
         self.freqDoubleSpinBox.setMaximum(self.bands[band][1])
         self.freqDoubleSpinBox.setSingleStep(self.bands[band][2])
 
         self.modeComboBox.clear()
         if band == '11m':
@@ -398,14 +405,15 @@
                 self.radioLineEdit.setText(self.settings.value('station/radio', ''))
                 self.antennaLineEdit.setText(self.settings.value('station/antenna', ''))
 
             if self.identityGroupBox.isChecked():
                 self.ownCallSignLineEdit.setText(self.settings.value('station/callSign', ''))
 
     def modeChanged(self, mode: str):
+        self.__last_mode__ = mode
         self.submodeComboBox.clear()
         self.submodeComboBox.setEnabled(True)
         if self.bandComboBox.currentText() == '11m':
             if mode in self.modes['CB'] and self.modes['CB'][mode]:
                 self.submodeComboBox.insertItems(0, [''] + self.modes['CB'][mode])
             else:
                 self.submodeComboBox.setEnabled(False)
```

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_QSOForm_ui.py` & `dragonlog-1.1.3/dragonlog/DragonLog_QSOForm_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_Settings.py` & `dragonlog-1.1.3/dragonlog/DragonLog_Settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     from keyring.backends import Windows
 
     keyring.set_keyring(Windows.WinVaultKeyring())
 
 
 class Settings(QtWidgets.QDialog, DragonLog_Settings_ui.Ui_Dialog):
     callbookChanged = QtCore.pyqtSignal(str)
+    rigctldStatusChanged = QtCore.pyqtSignal(bool)
 
     def __init__(self, parent, settings: QtCore.QSettings, rig_status: QtWidgets.QLabel, cols: typing.Iterable,
                  logger: Logger):
         super().__init__(parent)
         self.setupUi(self)
 
         self.log = logging.getLogger('Settings')
@@ -116,20 +117,30 @@
         if self.__is_exe__(rigctld_path[0]):
             self.init_hamlib(rigctld_path[0])
         else:
             self.checkHamlibLabel.setText(self.tr('Selected file is not the executable'))
 
     def init_hamlib(self, rigctld_path):
         if rigctld_path:
-            res = subprocess.run([rigctld_path, '-l'], capture_output=True)
-            stdout = str(res.stdout, sys.getdefaultencoding()).replace('\r', '')
-            if res.returncode != 0 or not stdout:
-                self.checkHamlibLabel.setText(self.tr('Error executing rigctld'))
+            try:
+                res = subprocess.run([rigctld_path, '-l'], capture_output=True)
+                stdout = str(res.stdout, sys.getdefaultencoding()).replace('\r', '')
+                if res.returncode != 0 or not stdout:
+                    self.log.error(f'Error executing rigctld: {res.returncode}')
+                    self.checkHamlibLabel.setText(self.tr('Error executing rigctld'))
+                    self.settings.setValue('cat/rigctldPath', '')
+                    self.hamlibPathLineEdit.setText('')
+                    return
+                self.log.debug('Executed rigctld to list rigs')
+            except FileNotFoundError:
+                self.log.info('rigctld is not available')
+                self.checkHamlibLabel.setText(self.tr('rigctld is not available'))
                 self.settings.setValue('cat/rigctldPath', '')
                 self.hamlibPathLineEdit.setText('')
+                return
 
             first = True
             rig_pos = 0
             mfr_pos = 0
             model_pos = 0
             end_pos = 0
             self.rigs = {}
@@ -187,14 +198,21 @@
                 cap, able = ln.split(':')
                 if able.strip() == 'Y':
                     self.rig_caps.append(cap[4:].lower())
 
     # noinspection PyUnresolvedReferences
     def ctrlRigctld(self, start):
         if start:
+            if not self.rigctld_path:
+                self.log.warning('rigctld is not available')
+                self.ctrlRigctldPushButton.setChecked(False)
+                self.parent().actionStart_hamlib_TB.setChecked(False)
+                self.parent().actionStart_hamlib_TB.setText(self.tr('Start hamlib'))
+                return
+
             if not self.rigctld:
                 rig_mfr = self.settings.value('cat/rigMfr')
                 rig_model = self.settings.value('cat/rigModel')
                 rig_if = self.settings.value("cat/interface")
                 rig_speed = self.settings.value("cat/baud")
                 if not rig_mfr or not rig_model or not rig_if or not rig_speed:
                     QtWidgets.QMessageBox.critical(self, self.tr('CAT settings error'),
@@ -227,26 +245,28 @@
                     self.ctrlRigctldPushButton.setChecked(True)
                     self.ctrlRigctldPushButton.setText(self.tr('Stop'))
                     self.parent().actionStart_hamlib_TB.setChecked(True)
                     self.parent().actionStart_hamlib_TB.setText(self.tr('Stop hamlib'))
                     self.log.info(f'rigctld is running with pid #{self.rigctld.pid} and arguments {self.rigctld.args}')
                     self.checkHamlibTimer.start(1000)
                     self.rig_status.setText(self.tr('Hamlib') + ': ' + self.tr('activ'))
+                    self.rigctldStatusChanged.emit(True)
         else:
             self.checkHamlibTimer.stop()
             if self.rigctld and not self.rigctld.poll():
                 os.kill(self.rigctld.pid, 9)
                 self.log.info('Killed rigctld')
             self.rigctld = None
             self.ctrlRigctldPushButton.setChecked(False)
             self.ctrlRigctldPushButton.setText(self.tr('Start'))
             self.parent().actionStart_hamlib_TB.setChecked(False)
             self.parent().actionStart_hamlib_TB.setText(self.tr('Start hamlib'))
             self.rig_status.setText(self.tr('Hamlib') + ': ' + self.tr('inactiv'))
             self.rig_caps = []
+            self.rigctldStatusChanged.emit(False)
 
     def locatorChanged(self, txt):
         if not txt:
             self.locatorLineEdit.setPalette(self.palette_empty)
         elif check_format(REGEX_LOCATOR, txt):
             self.locatorLineEdit.setPalette(self.palette_ok)
         else:
```

### Comparing `dragonlog-1.1.2/dragonlog/DragonLog_Settings_ui.py` & `dragonlog-1.1.3/dragonlog/DragonLog_Settings_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/LoTW.py` & `dragonlog-1.1.3/dragonlog/LoTW.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/Logger.py` & `dragonlog-1.1.3/dragonlog/Logger.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/RegEx.py` & `dragonlog-1.1.3/dragonlog/RegEx.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/data/README.md` & `dragonlog-1.1.3/dragonlog/data/README.md`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/data/bands.json` & `dragonlog-1.1.3/dragonlog/data/bands.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/data/cb_channels.json` & `dragonlog-1.1.3/dragonlog/data/cb_channels.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/data/color_map.json` & `dragonlog-1.1.3/dragonlog/data/color_map.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/data/i18n/DragonLog_de.qm` & `dragonlog-1.1.3/dragonlog/data/i18n/DragonLog_de.qm`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0564 655f 4445 4200 0009 f000  .....de_DEB.....
+00000010: a700 0000 0564 655f 4445 4200 0009 f800  .....de_DEB.....
 00000020: 0000 3c00 0001 5c00 0000 3e00 0001 7800  ..<...\...>...x.
-00000030: 0000 4d00 0054 1f00 0000 4e00 0054 5900  ..M..T....N..TY.
-00000040: 0000 5200 0054 8b00 0000 5900 0054 c700  ..R..T....Y..T..
+00000030: 0000 4d00 0054 8a00 0000 4e00 0054 c400  ..M..T....N..T..
+00000040: 0000 5200 0054 f600 0000 5900 0055 3200  ..R..T....Y..U2.
 00000050: 0002 5700 0035 7400 0003 8900 0035 b200  ..W..5t......5..
 00000060: 0005 5b00 0023 9900 000c d000 0011 7100  ..[..#........q.
 00000070: 0031 0e00 0000 0000 0047 6400 0001 fe00  .1.......Gd.....
 00000080: 004c 4400 003e aa00 0052 8400 0007 8600  .LD..>...R......
 00000090: 0053 5e00 0008 b400 0055 6700 0043 2d00  .S^......Ug..C-.
 000000a0: 0056 7c00 0045 3500 0056 7f00 0026 5600  .V|..E5..V...&V.
 000000b0: 0056 8800 000a 9200 0056 8800 0026 fe00  .V.......V...&..
@@ -29,15 +29,15 @@
 000001c0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
 000001d0: 376f f400 004b b800 38a9 3000 0001 1d00  7o...K..8.0.....
 000001e0: 4796 c400 0013 7f00 4796 c400 002e eb00  G.......G.......
 000001f0: 47ab 7600 002e b800 47ab 7600 0053 6800  G.v.....G.v..Sh.
 00000200: 4a2b 8200 003c a800 4c99 6200 001b a400  J+...<..L.b.....
 00000210: 4c99 6200 003e d100 52cc bc00 0007 b000  L.b..>..R.......
 00000220: 556a c300 0023 6800 567e 8100 0045 1400  Uj...#h.V~...E..
-00000230: 56ae c200 0055 2000 576d c200 0024 c800  V....U .Wm...$..
+00000230: 56ae c200 0055 8b00 576d c200 0024 c800  V....U..Wm...$..
 00000240: 576d c200 0044 9e00 587a ff00 000a b000  Wm...D..Xz......
 00000250: 587a ff00 0027 8d00 587a ff00 0048 6800  Xz...'..Xz...Hh.
 00000260: 5aa8 9400 000e 1600 5aa8 9400 0049 cf00  Z.......Z....I..
 00000270: 5aa8 9400 0052 7400 67ab 0600 0053 3c00  Z....Rt.g....S<.
 00000280: 6d92 9400 0051 1400 753c 2300 0044 5d00  m....Q..u<#..D].
 00000290: 8cd2 1500 0010 4200 aa80 2500 001a 6300  ......B...%...c.
 000002a0: ab72 4500 0009 cf00 bf5b b400 0005 f700  .rE......[......
@@ -51,15 +51,15 @@
 00000320: ac2b 0200 0041 7e02 e7d6 5e00 0002 4102  .+...A~...^...A.
 00000330: e7d6 5e00 0015 8b02 e7d6 5e00 0039 b802  ..^.......^..9..
 00000340: e81d 2400 003d fb03 004d 1200 000c 5d03  ..$..=...M....].
 00000350: 0149 e600 0021 4003 0cac 0500 000f cc03  .I...!@.........
 00000360: 0f6b 1200 0043 dc03 0f6b 3200 0023 b903  .k...C...k2..#..
 00000370: 1bec 1200 0013 de03 4485 3000 0000 1e03  ........D.0.....
 00000380: 45b3 3000 0000 5e03 4ecb 9200 0034 0f03  E.0...^.N....4..
-00000390: 4ecb 9200 0052 9603 533f be00 0055 4903  N....R..S?...UI.
+00000390: 4ecb 9200 0052 9603 533f be00 0055 b403  N....R..S?...U..
 000003a0: 598b 3200 0007 f903 598b 3200 0020 ee03  Y.2.....Y.2.. ..
 000003b0: 598b 3200 0040 c503 5d96 0b00 0040 e803  Y.2..@..]....@..
 000003c0: 6cc3 0400 000b c703 881f d400 0006 2003  l............. .
 000003d0: 9ce3 f400 001e 3f03 9ce9 a500 0025 3a03  ......?......%:.
 000003e0: f5e0 0700 002d 9804 07f6 ee00 0024 7904  .....-.......$y.
 000003f0: 07f6 ee00 0043 8f04 2b4e 0500 001d 6c04  .....C..+N....l.
 00000400: 6c90 3200 0041 0b04 8c96 8100 0014 5f04  l.2..A........_.
@@ -74,1465 +74,1472 @@
 00000490: e842 f200 0051 8a04 edd3 6400 0036 5604  .B...Q....d..6V.
 000004a0: f5b6 e700 002a 3705 0476 9400 0032 4105  .....*7..v...2A.
 000004b0: 1f06 1500 0051 ad05 3268 c400 0004 1805  .....Q..2h......
 000004c0: 34db 8200 0021 d605 3ddf a300 000a d005  4....!..=.......
 000004d0: 4466 8200 0049 0b05 5776 4500 0045 a305  Df...I..WvE..E..
 000004e0: 6336 9e00 0032 aa05 647d 0e00 002f 9405  c6...2..d}.../..
 000004f0: 7865 9800 0047 a605 7865 b800 0047 c805  xe...G..xe...G..
-00000500: c7f7 2800 0055 ad05 c984 e900 0030 a106  ..(..U.......0..
-00000510: 011e c400 0002 9c06 778d 0800 0006 cf06  ........w.......
-00000520: 778d 0800 001f 2106 7e7c a100 0026 2306  w.....!.~|...&#.
-00000530: 7e7c a100 0046 6906 830d be00 0029 f106  ~|...Fi......)..
-00000540: bdf0 a400 0019 8f06 be94 d200 0052 fa06  .............R..
-00000550: d2af d900 0055 d706 db4d 4200 0027 f206  .....U...MB..'..
-00000560: e056 d800 0024 3e06 e056 d800 0043 5606  .V...$>..V...CV.
-00000570: f895 8e00 0015 f507 2f4a 1500 004a 3607  ......../J...J6.
-00000580: 366b 9300 0005 1a07 50be 3900 0053 9a07  6k......P.9..S..
-00000590: 68f8 4400 004e ab07 693d fe00 0031 a307  h.D..N..i=...1..
-000005a0: 6941 4e00 0032 6607 6cbb 6300 000e 7707  iAN..2f.l.c...w.
-000005b0: 7f18 a400 004b ec07 86be 4800 0036 d507  .....K....H..6..
-000005c0: 8f3a 3e00 0024 fb07 8f3a 3e00 0044 cf07  .:>..$...:>..D..
-000005d0: e67a d700 0030 ee07 e76d c800 0025 7d07  .z...0...m...%}.
-000005e0: e78f a400 0025 b307 e79f 3400 0025 eb07  .....%....4..%..
-000005f0: e79f 3400 0046 2d07 e7e0 a400 002e 4207  ..4..F-.......B.
-00000600: e7f2 3400 002e 7d07 e7f2 3400 004e 4408  ..4...}...4..ND.
-00000610: 14d3 ed00 0032 eb08 14d3 ed00 0046 9a08  .....2.......F..
-00000620: 3292 cb00 0002 7908 3587 6a00 002b a608  2.....y.5.j..+..
-00000630: 36b6 5400 0012 8a08 5ac5 0100 0001 9408  6.T.....Z.......
-00000640: 5ac5 0100 0014 2c08 5ac5 0100 0038 5908  Z.....,.Z....8Y.
-00000650: 678f b400 0027 1f08 679f 2400 0027 5708  g....'..g.$..'W.
-00000660: 679f 2400 0048 2c08 7f52 2500 002a e608  g.$..H,..R%..*..
-00000670: 8879 1400 0019 2108 aae3 e400 0009 9c08  .y....!.........
-00000680: b63d de00 0034 fd08 bd74 5e00 0022 ff08  .=...4...t^.."..
-00000690: d39b 6400 0040 3f08 f89a cb00 0035 d009  ..d..@?......5..
-000006a0: 14be 9200 0049 6309 1c52 9500 002d f709  .....Ic..R...-..
-000006b0: 238c 7500 0016 f209 3f8c ad00 000c da09  #.u.....?.......
-000006c0: 564e 4200 004c 2409 6c61 f400 0013 aa09  VNB..L$.la......
-000006d0: 6c61 f400 002f 1709 6fe6 7e00 0011 8e09  la.../..o.~.....
-000006e0: 8fa3 8700 002f 4c09 97c9 1400 0020 b309  ...../L...... ..
-000006f0: 97c9 1400 0040 8409 97d9 8400 0020 7809  .....@....... x.
-00000700: 9c7f 1a00 0037 7209 a118 8500 0011 0d09  .....7r.........
-00000710: c004 d700 0003 df09 c4e8 d700 0001 c409  ................
-00000720: c8df a200 001e 9409 c943 f500 0010 0709  .........C......
-00000730: c9cf c500 000c 2f09 df31 3800 0047 1709  ....../..18..G..
-00000740: e854 fc00 0015 c609 e854 fc00 003b 1a09  .T.......T...;..
-00000750: f42c fb00 001b 7e0a 16bb 3400 0046 d60a  .,....~...4..F..
-00000760: 2087 bc00 003b f80a 2190 e200 0006 860a   ....;..!.......
-00000770: 2190 e200 001e d50a 3f0e 9500 0028 ea0a  !.......?....(..
-00000780: 5e68 d900 0026 770a 643c 1400 0016 bb0a  ^h...&w.d<......
-00000790: 6789 3b00 0007 0e0a 6789 3b00 001f 630a  g.;.....g.;...c.
-000007a0: 67a9 0200 0007 4a0a 67a9 0200 001f a20a  g.....J.g.......
-000007b0: 6dc8 3e00 0034 960a 7833 e400 0039 790a  m.>..4..x3...9y.
-000007c0: 7d6b 2400 0018 550a 92a2 e500 0029 9d0a  }k$...U......)..
-000007d0: 9612 e500 0028 900a a8b0 0e00 000e 360a  .....(........6.
-000007e0: a8b0 0e00 0049 f00a acdb 7e00 0002 1c0a  .....I....~.....
-000007f0: b945 f500 002b 220a b945 f500 004a 130a  .E...+"..E...J..
-00000800: c389 2500 0028 590a c5b4 4900 003f a40a  ..%..(Y...I..?..
-00000810: c897 c500 0006 480a d2f0 b500 0003 090a  ......H.........
-00000820: d382 7700 0003 570a e2b5 9600 0004 b50a  ..w...W.........
-00000830: f31c 2200 003b 840b 1562 0700 004f 300b  .."..;...b...O0.
-00000840: 1805 3900 0015 3b0b 4597 5500 0008 1b0b  ..9...;.E.U.....
-00000850: 5d8a f400 001f e10b 6628 d200 0034 540b  ].......f(...4T.
-00000860: 7fe2 de00 0033 2a0b ad17 7800 001b 500b  .....3*...x...P.
-00000870: ff25 ce00 001c 7e0c 08f5 6c00 003d b60c  .%....~...l..=..
-00000880: 107d 9300 0003 a10c 10ba b200 0027 b00c  .}...........'..
-00000890: 1536 f700 002d 190c 1f2f 0200 004c 750c  .6...-.../...Lu.
-000008a0: 29f2 a400 004f 0a0c 6a19 e900 003c e10c  )....O..j....<..
-000008b0: 8c09 2900 001d 350c 8c09 2900 003f 4d0c  ..)...5...)..?M.
-000008c0: 9688 9500 0014 830c a3fa 5f00 001a 250c  .........._...%.
-000008d0: a6e8 d400 003a 5e0c bb01 7300 000c 9d0c  .....:^...s.....
-000008e0: bb01 7300 0033 810c c9a0 0e00 002d 730d  ..s..3.......-s.
-000008f0: 0218 6400 0048 bb0d 07a4 f800 003b 470d  ..d..H.......;G.
-00000900: 1f27 b200 0014 d70d 3504 b400 003a ba0d  .'......5....:..
-00000910: 76f7 5900 001b d30d 825f 7300 000f 1a0d  v.Y......_s.....
-00000920: a03c 1200 0050 020d d0ff 4c00 002c cd0d  .<...P....L..,..
-00000930: f2ea c200 003c 3e0d fe4e 2400 0019 d80d  .....<>..N$.....
-00000940: fe4e 2400 0050 c80e 0543 5500 0024 000e  .N$..P...CU..$..
-00000950: 05d1 b500 0050 610e 0743 5500 0044 210e  .....Pa..CU..D!.
-00000960: 0906 8800 0037 ac0e 233d d500 004c bb0e  .....7..#=...L..
-00000970: 87ac 6400 0020 2a0e 93fa 5200 0017 970e  ..d.. *...R.....
-00000980: a32f e400 003e fe0e c497 a200 000b 3e0e  ./...>........>.
-00000990: c72a a600 0005 820e de3d a200 0039 f10e  .*.......=...9..
-000009a0: e46b 3400 0047 ea0e fdeb 3400 0045 eb0f  .k4..G....4..E..
-000009b0: 165e c400 0045 540f 3562 ce00 0017 f80f  .^...ET.5b......
-000009c0: 6963 bc00 000d 1f0f 6963 bc00 002a ac0f  ic......ic...*..
-000009d0: 6963 bc00 0052 3b0f 6978 c700 0033 c20f  ic...R;.ix...3..
-000009e0: 6c98 6c00 0054 f50f 7ddd 2800 004d 630f  l.l..T..}.(..Mc.
-000009f0: 8007 d400 0038 c90f 8313 8900 0013 130f  .....8..........
-00000a00: cb15 5200 0018 d70f e6f6 3400 003f cc69  ..R.......4..?.i
-00000a10: 0000 5601 03ff ffff ff08 0000 0000 0600  ..V.............
-00000a20: 0000 032e 2e2e 0700 0000 0644 6961 6c6f  ...........Dialo
-00000a30: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00000a40: 0631 3135 3230 3007 0000 0006 4469 616c  .115200.....Dial
-00000a50: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00000a60: 0004 3132 3030 0700 0000 0644 6961 6c6f  ..1200.....Dialo
-00000a70: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00000a80: 0631 3238 3030 3007 0000 0006 4469 616c  .128000.....Dial
-00000a90: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00000aa0: 0005 3134 3430 3007 0000 0006 4469 616c  ..14400.....Dial
-00000ab0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00000ac0: 0005 3139 3230 3007 0000 0006 4469 616c  ..19200.....Dial
-00000ad0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00000ae0: 0004 3234 3030 0700 0000 0644 6961 6c6f  ..2400.....Dialo
-00000af0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00000b00: 0533 3834 3030 0700 0000 0644 6961 6c6f  .38400.....Dialo
-00000b10: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00000b20: 0434 3830 3007 0000 0006 4469 616c 6f67  .4800.....Dialog
-00000b30: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
-00000b40: 3537 3630 3007 0000 0006 4469 616c 6f67  57600.....Dialog
-00000b50: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
-00000b60: 3936 3030 0700 0000 0644 6961 6c6f 6701  9600.....Dialog.
-00000b70: 03ff ffff ff08 0000 0000 0600 0000 013c  ...............<
-00000b80: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
-00000b90: ff08 0000 0000 0600 0000 013e 0700 0000  ...........>....
-00000ba0: 0644 6961 6c6f 6701 0300 0000 0e00 4100  .Dialog.......A.
-00000bb0: 6e00 7400 6500 6e00 6e00 6508 0000 0000  n.t.e.n.n.e.....
-00000bc0: 0600 0000 0741 6e74 656e 6e61 0700 0000  .....Antenna....
-00000bd0: 0644 6961 6c6f 6701 0300 0000 1600 4100  .Dialog.......A.
-00000be0: 7500 6600 7300 7400 6500 6900 6700 6500  u.f.s.t.e.i.g.e.
-00000bf0: 6e00 6408 0000 0000 0600 0000 0941 7363  n.d..........Asc
-00000c00: 656e 6469 6e67 0700 0000 0644 6961 6c6f  ending.....Dialo
-00000c10: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00000c20: 0343 4154 0700 0000 0644 6961 6c6f 6701  .CAT.....Dialog.
-00000c30: 03ff ffff ff08 0000 0000 0600 0000 0a43  ...............C
-00000c40: 422d 5374 6174 696f 6e07 0000 0006 4469  B-Station.....Di
-00000c50: 616c 6f67 0103 0000 0014 0052 0075 0066  alog.......R.u.f
-00000c60: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
-00000c70: 0000 0006 0000 0009 4361 6c6c 2073 6967  ........Call sig
-00000c80: 6e07 0000 0006 4469 616c 6f67 0103 ffff  n.....Dialog....
-00000c90: ffff 0800 0000 0006 0000 0008 4361 6c6c  ............Call
-00000ca0: 626f 6f6b 0700 0000 0644 6961 6c6f 6701  book.....Dialog.
-00000cb0: 0300 0000 3800 5a00 6500 7200 7400 6900  ....8.Z.e.r.t.i.
-00000cc0: 6600 6900 6b00 6100 7400 2000 6200 6500  f.i.k.a.t. .b.e.
-00000cd0: 6e00 f600 7400 6900 6700 7400 2000 5000  n...t.i.g.t. .P.
-00000ce0: 6100 7300 7300 7700 6f00 7200 7408 0000  a.s.s.w.o.r.t...
-00000cf0: 0000 0600 0000 1a43 6572 7469 6669 6361  .......Certifica
-00000d00: 7465 206e 6565 6473 2070 6173 7377 6f72  te needs passwor
-00000d10: 6407 0000 0006 4469 616c 6f67 0103 0000  d.....Dialog....
-00000d20: 0024 0053 0070 0061 006c 0074 0065 006e  .$.S.p.a.l.t.e.n
-00000d30: 0020 0076 0065 0072 0073 0074 0065 0063  . .v.e.r.s.t.e.c
-00000d40: 006b 0065 006e 0800 0000 0006 0000 000f  .k.e.n..........
-00000d50: 436f 6c75 6d6e 7320 746f 2068 6964 6507  Columns to hide.
-00000d60: 0000 0006 4469 616c 6f67 0103 0000 0020  ....Dialog..... 
-00000d70: 0053 0070 0061 006c 0074 0065 006e 0020  .S.p.a.l.t.e.n. 
-00000d80: 0061 006e 007a 0065 0069 0067 0065 006e  .a.n.z.e.i.g.e.n
-00000d90: 0800 0000 0006 0000 000f 436f 6c75 6d6e  ..........Column
-00000da0: 7320 746f 2073 686f 7707 0000 0006 4469  s to show.....Di
-00000db0: 616c 6f67 0103 0000 0018 0041 006e 006d  alog.......A.n.m
-00000dc0: 0065 006c 0064 0065 0064 0061 0074 0065  .e.l.d.e.d.a.t.e
-00000dd0: 006e 0800 0000 0006 0000 000b 4372 6564  .n..........Cred
-00000de0: 656e 7469 616c 7307 0000 0006 4469 616c  entials.....Dial
-00000df0: 6f67 0103 0000 0014 0041 0062 0073 0074  og.......A.b.s.t
-00000e00: 0065 0069 0067 0065 006e 0064 0800 0000  .e.i.g.e.n.d....
-00000e10: 0006 0000 000a 4465 7363 656e 6469 6e67  ......Descending
-00000e20: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-00000e30: 3e00 5700 6900 7200 6b00 7300 6100 6d00  >.W.i.r.k.s.a.m.
-00000e40: 2000 6e00 6100 6300 6800 2000 4100 6e00   .n.a.c.h. .A.n.
-00000e50: 7700 6500 6e00 6400 7500 6e00 6700 7300  w.e.n.d.u.n.g.s.
-00000e60: 6e00 6500 7500 7300 7400 6100 7200 7408  n.e.u.s.t.a.r.t.
-00000e70: 0000 0000 0600 0000 2345 6666 6563 7469  ........#Effecti
-00000e80: 7665 2061 6674 6572 2061 7070 6c69 6361  ve after applica
-00000e90: 7469 6f6e 2072 6573 7461 7274 0700 0000  tion restart....
-00000ea0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000eb0: 0000 0600 0000 0645 7870 6f72 7407 0000  .......Export...
-00000ec0: 0006 4469 616c 6f67 0103 0000 0034 0045  ..Dialog.....4.E
-00000ed0: 0078 0070 006f 0072 0074 0069 0065 0072  .x.p.o.r.t.i.e.r
-00000ee0: 0065 0020 0043 0042 002d 0051 0053 004f  .e. .C.B.-.Q.S.O
-00000ef0: 0073 0020 0069 006e 0020 0041 0044 0049  .s. .i.n. .A.D.I
-00000f00: 0046 0800 0000 0006 0000 0016 4578 706f  .F..........Expo
-00000f10: 7274 2043 4220 5153 4f73 2074 6f20 4144  rt CB QSOs to AD
-00000f20: 4946 0700 0000 0644 6961 6c6f 6701 0300  IF.....Dialog...
-00000f30: 0000 3600 4500 7800 7000 6f00 7200 7400  ..6.E.x.p.o.r.t.
-00000f40: 6900 6500 7200 6500 2000 6e00 7500 7200  i.e.r.e. .n.u.r.
-00000f50: 2000 6e00 6500 7500 6500 7300 7400 6500   .n.e.u.e.s.t.e.
-00000f60: 2000 5100 5300 4f00 7308 0000 0000 0600   .Q.S.O.s.......
-00000f70: 0000 1745 7870 6f72 7420 6f6e 6c79 2072  ...Export only r
-00000f80: 6563 656e 7420 5153 4f73 0700 0000 0644  ecent QSOs.....D
-00000f90: 6961 6c6f 6701 0300 0000 4200 4500 7800  ialog.....B.E.x.
-00000fa0: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
-00000fb0: 2000 6500 6900 6700 6500 6e00 6500 2000   .e.i.g.e.n.e. .
-00000fc0: 4e00 6f00 7400 6900 7a00 6500 6e00 2000  N.o.t.i.z.e.n. .
-00000fd0: 6900 6e00 2000 4100 4400 4900 4608 0000  i.n. .A.D.I.F...
-00000fe0: 0000 0600 0000 1845 7870 6f72 7420 6f77  .......Export ow
-00000ff0: 6e20 6e6f 7465 7320 746f 2041 4449 4607  n notes to ADIF.
-00001000: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00001010: 0800 0000 0006 0000 000e 4861 6d6c 6962  ..........Hamlib
-00001020: 2072 6967 6374 6c64 0700 0000 0644 6961   rigctld.....Dia
-00001030: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00001040: 0000 0d49 6d70 6f72 742f 4578 706f 7274  ...Import/Export
-00001050: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-00001060: 1a00 5300 6300 6800 6e00 6900 7400 7400  ..S.c.h.n.i.t.t.
-00001070: 7300 7400 6500 6c00 6c00 6508 0000 0000  s.t.e.l.l.e.....
-00001080: 0600 0000 0949 6e74 6572 6661 6365 0700  .....Interface..
-00001090: 0000 0644 6961 6c6f 6701 0300 0000 2000  ...Dialog..... .
-000010a0: 6c00 6500 7400 7a00 7400 6500 7300 2000  l.e.t.z.t.e.s. .
-000010b0: 4800 6100 6c00 6200 6a00 6100 6800 7208  H.a.l.b.j.a.h.r.
-000010c0: 0000 0000 0600 0000 0e4c 6173 7420 6861  .........Last ha
-000010d0: 6c66 2079 6561 7207 0000 0006 4469 616c  lf year.....Dial
-000010e0: 6f67 0103 0000 001a 006c 0065 0074 007a  og.......l.e.t.z
-000010f0: 0074 0065 006e 0020 004d 006f 006e 0061  .t.e.n. .M.o.n.a
-00001100: 0074 0800 0000 0006 0000 000a 4c61 7374  .t..........Last
-00001110: 206d 6f6e 7468 0700 0000 0644 6961 6c6f   month.....Dialo
-00001120: 6701 0300 0000 1800 6c00 6500 7400 7a00  g.......l.e.t.z.
-00001130: 7400 6500 2000 5700 6f00 6300 6800 6508  t.e. .W.o.c.h.e.
-00001140: 0000 0000 0600 0000 094c 6173 7420 7765  .........Last we
-00001150: 656b 0700 0000 0644 6961 6c6f 6701 0300  ek.....Dialog...
-00001160: 0000 1800 6c00 6500 7400 7a00 7400 6500  ....l.e.t.z.t.e.
-00001170: 7300 2000 4a00 6100 6800 7208 0000 0000  s. .J.a.h.r.....
-00001180: 0600 0000 094c 6173 7420 7965 6172 0700  .....Last year..
-00001190: 0000 0644 6961 6c6f 6701 0300 0000 0c00  ...Dialog.......
-000011a0: 4200 7200 6500 6900 7400 6508 0000 0000  B.r.e.i.t.e.....
-000011b0: 0600 0000 034c 6174 0700 0000 0644 6961  .....Lat.....Dia
-000011c0: 6c6f 6701 0300 0000 0a00 5300 7400 7500  log.......S.t.u.
-000011d0: 6600 6508 0000 0000 0600 0000 054c 6576  f.e..........Lev
-000011e0: 656c 0700 0000 0644 6961 6c6f 6701 03ff  el.....Dialog...
-000011f0: ffff ff08 0000 0000 0600 0000 044c 6f54  .............LoT
-00001200: 5707 0000 0006 4469 616c 6f67 0103 ffff  W.....Dialog....
-00001210: ffff 0800 0000 0006 0000 0007 4c6f 6361  ............Loca
-00001220: 746f 7207 0000 0006 4469 616c 6f67 0103  tor.....Dialog..
-00001230: 0000 002c 004c 006f 0067 0020 0069 006e  ...,.L.o.g. .i.n
-00001240: 0020 0044 0061 0074 0065 0069 0020 0073  . .D.a.t.e.i. .s
-00001250: 0063 0068 0072 0065 0069 0062 0065 006e  .c.h.r.e.i.b.e.n
-00001260: 0800 0000 0006 0000 000b 4c6f 6720 746f  ..........Log to
-00001270: 2066 696c 6507 0000 0006 4469 616c 6f67   file.....Dialog
-00001280: 0103 0000 001e 004c 006f 0067 0067 0069  .......L.o.g.g.i
-00001290: 006e 0067 002d 0041 0075 0073 0067 0061  .n.g.-.A.u.s.g.a
-000012a0: 0062 0065 0800 0000 0006 0000 000e 4c6f  .b.e..........Lo
-000012b0: 6767 696e 6720 6f75 7470 7574 0700 0000  gging output....
-000012c0: 0644 6961 6c6f 6701 0300 0000 0a00 4c00  .Dialog.......L.
-000012d0: e400 6e00 6700 6508 0000 0000 0600 0000  ..n.g.e.........
-000012e0: 034c 6f6e 0700 0000 0644 6961 6c6f 6701  .Lon.....Dialog.
-000012f0: 03ff ffff ff08 0000 0000 0600 0000 044e  ...............N
-00001300: 616d 6507 0000 0006 4469 616c 6f67 0103  ame.....Dialog..
-00001310: 0000 005e 0043 0042 0020 0051 0053 004f  ...^.C.B. .Q.S.O
-00001320: 0073 0020 0077 0065 0072 0064 0065 006e  .s. .w.e.r.d.e.n
-00001330: 0020 0062 0065 0069 006d 0020 0049 006d  . .b.e.i.m. .I.m
-00001340: 0070 006f 0072 0074 0020 0069 006d 006d  .p.o.r.t. .i.m.m
-00001350: 0065 0072 0020 0062 0065 0072 00fc 0063  .e.r. .b.e.r...c
-00001360: 006b 0073 0069 0063 0068 0074 0069 0067  .k.s.i.c.h.t.i.g
-00001370: 0074 0800 0000 0006 0000 0028 4f6e 2069  .t.........(On i
-00001380: 6d70 6f72 7420 4342 2051 534f 7320 7769  mport CB QSOs wi
-00001390: 6c6c 2061 6c77 6179 7320 6265 2068 616e  ll always be han
-000013a0: 646c 6564 0700 0000 0644 6961 6c6f 6701  dled.....Dialog.
-000013b0: 0300 0000 1000 5000 6100 7300 7300 7700  ......P.a.s.s.w.
-000013c0: 6f00 7200 7408 0000 0000 0600 0000 0850  o.r.t..........P
-000013d0: 6173 7377 6f72 6407 0000 0006 4469 616c  assword.....Dial
-000013e0: 6f67 0103 0000 0070 0050 0061 0073 0073  og.....p.P.a.s.s
-000013f0: 0077 006f 0072 0074 0020 0064 0065 0073  .w.o.r.t. .d.e.s
-00001400: 0020 004c 006f 0054 0057 002d 004f 006e  . .L.o.T.W.-.O.n
-00001410: 006c 0069 006e 0065 002d 0041 0063 0063  .l.i.n.e.-.A.c.c
-00001420: 006f 0075 006e 0074 0073 002c 0020 006e  .o.u.n.t.s.,. .n
-00001430: 0069 0063 0068 0074 0020 0064 0065 0073  .i.c.h.t. .d.e.s
-00001440: 0020 005a 0065 0072 0074 0069 0066 0069  . .Z.e.r.t.i.f.i
-00001450: 006b 0061 0074 0073 0800 0000 0006 0000  .k.a.t.s........
-00001460: 0038 5061 7373 776f 7264 2066 6f72 204c  .8Password for L
-00001470: 6f54 5720 6f6e 6c69 6e65 2061 6363 6f75  oTW online accou
-00001480: 6e74 206e 6f74 2066 6f72 2074 6865 2063  nt not for the c
-00001490: 6572 7469 6669 6361 7465 0700 0000 0644  ertificate.....D
-000014a0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-000014b0: 0600 0000 0351 5448 0700 0000 0644 6961  .....QTH.....Dia
-000014c0: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-000014d0: 0000 0552 6164 696f 0700 0000 0644 6961  ...Radio.....Dia
-000014e0: 6c6f 6701 0300 0000 1800 4e00 6500 7500  log.......N.e.u.
-000014f0: 6500 7300 7400 6500 2000 5100 5300 4f00  e.s.t.e. .Q.S.O.
-00001500: 7308 0000 0000 0600 0000 0b52 6563 656e  s..........Recen
-00001510: 7420 5153 4f73 0700 0000 0644 6961 6c6f  t QSOs.....Dialo
-00001520: 6701 0300 0000 1200 4600 7500 6e00 6b00  g.......F.u.n.k.
-00001530: 6700 6500 7200 e400 7408 0000 0000 0600  g.e.r...t.......
-00001540: 0000 0352 6967 0700 0000 0644 6961 6c6f  ...Rig.....Dialo
-00001550: 6701 0300 0000 4c00 5300 6900 6500 6800  g.....L.S.i.e.h.
-00001560: 6500 2000 4500 6900 6e00 7300 7400 6500  e. .E.i.n.s.t.e.
-00001570: 6c00 6c00 7500 6e00 6700 6500 6e00 2000  l.l.u.n.g.e.n. .
-00001580: 5200 6500 6900 7400 6500 7200 2000 2200  R.e.i.t.e.r. .".
-00001590: 4100 6e00 7700 6500 6e00 6400 7500 6e00  A.n.w.e.n.d.u.n.
-000015a0: 6700 2208 0000 0000 0600 0000 2253 6565  g."........."See
-000015b0: 2073 6574 7469 6e67 7320 7061 6765 2022   settings page "
-000015c0: 5573 6572 2069 6e74 6572 6661 6365 2207  User interface".
-000015d0: 0000 0006 4469 616c 6f67 0103 0000 0034  ....Dialog.....4
-000015e0: 0043 0042 002d 0042 0061 006e 0064 0020  .C.B.-.B.a.n.d. 
-000015f0: 0061 0075 0074 006f 006d 0061 0074 0069  .a.u.t.o.m.a.t.i
-00001600: 0073 0063 0068 0020 0077 00e4 0068 006c  .s.c.h. .w...h.l
-00001610: 0065 006e 0800 0000 0006 0000 0019 5365  .e.n..........Se
-00001620: 6c65 6374 2043 4220 6261 6e64 2062 7920  lect CB band by 
-00001630: 6465 6661 756c 7407 0000 0006 4469 616c  default.....Dial
-00001640: 6f67 0103 0000 000c 0044 0069 0065 006e  og.......D.i.e.n
-00001650: 0073 0074 0800 0000 0006 0000 0007 5365  .s.t..........Se
-00001660: 7276 6963 6507 0000 0006 4469 616c 6f67  rvice.....Dialog
-00001670: 0103 0000 001a 0053 0065 0074 007a 0065  .......S.e.t.z.e
-00001680: 0020 004c 006f 0063 0061 0074 006f 0072  . .L.o.c.a.t.o.r
-00001690: 0800 0000 0006 0000 000b 5365 7420 6c6f  ..........Set lo
-000016a0: 6361 746f 7207 0000 0006 4469 616c 6f67  cator.....Dialog
-000016b0: 0103 0000 001a 0045 0069 006e 0073 0074  .......E.i.n.s.t
-000016c0: 0065 006c 006c 0075 006e 0067 0065 006e  .e.l.l.u.n.g.e.n
-000016d0: 0800 0000 0006 0000 0008 5365 7474 696e  ..........Settin
-000016e0: 6773 0700 0000 0644 6961 6c6f 6701 0300  gs.....Dialog...
-000016f0: 0000 1c00 5a00 6500 6900 6700 6500 2000  ....Z.e.i.g.e. .
-00001700: 5100 5300 4f00 7300 2000 6600 fc00 7208  Q.S.O.s. .f...r.
-00001710: 0000 0000 0600 0000 0e53 686f 7720 5153  .........Show QS
-00001720: 4f73 2066 726f 6d07 0000 0006 4469 616c  Os from.....Dial
-00001730: 6f67 0103 0000 0014 007a 0065 0069 0067  og.......z.e.i.g
-00001740: 0065 0020 0061 006c 006c 0065 0800 0000  .e. .a.l.l.e....
-00001750: 0006 0000 0008 5368 6f77 2061 6c6c 0700  ......Show all..
-00001760: 0000 0644 6961 6c6f 6701 0300 0000 4000  ...Dialog.....@.
-00001770: 5300 7000 6100 6c00 7400 6500 6e00 2000  S.p.a.l.t.e.n. .
-00001780: 6100 6e00 7a00 6500 6900 6700 6500 6e00  a.n.z.e.i.g.e.n.
-00001790: 2000 6f00 6400 6500 7200 2000 7600 6500   .o.d.e.r. .v.e.
-000017a0: 7200 7300 7400 6500 6300 6b00 6500 6e08  r.s.t.e.c.k.e.n.
-000017b0: 0000 0000 0600 0000 1453 686f 7720 6f72  .........Show or
-000017c0: 2068 6964 6520 636f 6c75 6d6e 7307 0000   hide columns...
-000017d0: 0006 4469 616c 6f67 0103 0000 0028 0053  ..Dialog.....(.S
-000017e0: 006f 0072 0074 0069 0065 0072 0065 0020  .o.r.t.i.e.r.e. 
-000017f0: 006e 0061 0063 0068 0020 0053 0070 0061  .n.a.c.h. .S.p.a
-00001800: 006c 0074 0065 0800 0000 0006 0000 000e  .l.t.e..........
-00001810: 536f 7274 206f 6e20 636f 6c75 6d6e 0700  Sort on column..
-00001820: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00001830: 0000 0000 0600 0000 0553 7461 7274 0700  .........Start..
-00001840: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00001850: 0000 0000 0600 0000 0753 7461 7469 6f6e  .........Station
-00001860: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
-00001870: ff08 0000 0000 0600 0000 0454 5153 4c07  ...........TQSL.
-00001880: 0000 0006 4469 616c 6f67 0103 0000 0064  ....Dialog.....d
-00001890: 0056 0065 0072 0077 0065 006e 0064 0065  .V.e.r.w.e.n.d.e
-000018a0: 0020 0064 0069 0065 0020 006b 006f 006e  . .d.i.e. .k.o.n
-000018b0: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
-000018c0: 0074 0065 0020 0049 0044 0020 0062 0065  .t.e. .I.D. .b.e
-000018d0: 0069 0020 0066 0065 0068 006c 0065 006e  .i. .f.e.h.l.e.n
-000018e0: 0064 0065 006e 0020 0057 0065 0072 0074  .d.e.n. .W.e.r.t
-000018f0: 0065 006e 0800 0000 0006 0000 0024 5573  .e.n.........$Us
-00001900: 6520 636f 6e66 6967 7572 6564 2049 4420  e configured ID 
-00001910: 666f 7220 6d69 7373 696e 6720 7661 6c75  for missing valu
-00001920: 6573 0700 0000 0644 6961 6c6f 6701 0300  es.....Dialog...
-00001930: 0000 6e00 5600 6500 7200 7700 6500 6e00  ..n.V.e.r.w.e.n.
-00001940: 6400 6500 2000 6400 6900 6500 2000 6b00  d.e. .d.i.e. .k.
-00001950: 6f00 6e00 6600 6900 6700 7500 7200 6900  o.n.f.i.g.u.r.i.
-00001960: 6500 7200 7400 6500 2000 5300 7400 6100  e.r.t.e. .S.t.a.
-00001970: 7400 6900 6f00 6e00 2000 6200 6500 6900  t.i.o.n. .b.e.i.
-00001980: 2000 6600 6500 6800 6c00 6500 6e00 6400   .f.e.h.l.e.n.d.
-00001990: 6500 6e00 2000 5700 6500 7200 7400 6500  e.n. .W.e.r.t.e.
-000019a0: 6e08 0000 0000 0600 0000 2955 7365 2063  n.........)Use c
-000019b0: 6f6e 6669 6775 7265 6420 5374 6174 696f  onfigured Statio
-000019c0: 6e20 666f 7220 6d69 7373 696e 6720 7661  n for missing va
-000019d0: 6c75 6573 0700 0000 0644 6961 6c6f 6701  lues.....Dialog.
-000019e0: 0300 0000 1200 4100 6e00 7700 6500 6e00  ......A.n.w.e.n.
-000019f0: 6400 7500 6e00 6708 0000 0000 0600 0000  d.u.n.g.........
-00001a00: 0e55 7365 7220 696e 7465 7266 6163 6507  .User interface.
-00001a10: 0000 0006 4469 616c 6f67 0103 0000 0018  ....Dialog......
-00001a20: 0042 0065 006e 0075 0074 007a 0065 0072  .B.e.n.u.t.z.e.r
-00001a30: 006e 0061 006d 0065 0800 0000 0006 0000  .n.a.m.e........
-00001a40: 0008 5573 6572 6e61 6d65 0700 0000 0644  ..Username.....D
-00001a50: 6961 6c6f 6701 0300 0000 7800 4200 6500  ialog.....x.B.e.
-00001a60: 6e00 7500 7400 7a00 6500 7200 6e00 6100  n.u.t.z.e.r.n.a.
-00001a70: 6d00 6500 2000 6400 6500 7300 2000 4c00  m.e. .d.e.s. .L.
-00001a80: 6f00 5400 5700 2d00 4f00 6e00 6c00 6900  o.T.W.-.O.n.l.i.
-00001a90: 6e00 6500 2d00 4100 6300 6300 6f00 7500  n.e.-.A.c.c.o.u.
-00001aa0: 6e00 7400 7300 2c00 2000 6e00 6900 6300  n.t.s.,. .n.i.c.
-00001ab0: 6800 7400 2000 6400 6500 7300 2000 5a00  h.t. .d.e.s. .Z.
-00001ac0: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
-00001ad0: 7400 7308 0000 0000 0600 0000 3855 7365  t.s.........8Use
-00001ae0: 726e 616d 6520 666f 7220 4c6f 5457 206f  rname for LoTW o
-00001af0: 6e6c 696e 6520 6163 636f 756e 7420 6e6f  nline account no
-00001b00: 7420 666f 7220 7468 6520 6365 7274 6966  t for the certif
-00001b10: 6963 6174 6507 0000 0006 4469 616c 6f67  icate.....Dialog
-00001b20: 0103 0000 0020 0044 0061 0074 0065 0069  ..... .D.a.t.e.i
-00001b30: 00fc 0062 0065 0072 0077 0061 0063 0068  ...b.e.r.w.a.c.h
-00001b40: 0075 006e 0067 0800 0000 0006 0000 000a  .u.n.g..........
-00001b50: 5761 7463 6820 4669 6c65 0700 0000 0644  Watch File.....D
-00001b60: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-00001b70: 0600 0000 0465 5153 4c07 0000 0006 4469  .....eQSL.....Di
-00001b80: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
-00001b90: 0000 0002 c2b0 0700 0000 0644 6961 6c6f  ...........Dialo
-00001ba0: 6701 0300 0000 9e00 4500 6900 6e00 2000  g.......E.i.n. .
-00001bb0: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
-00001bc0: 6b00 2d00 4200 6100 6300 6b00 7500 7000  k.-.B.a.c.k.u.p.
-00001bd0: 2000 6b00 6f00 6e00 6e00 7400 6500 2000   .k.o.n.n.t.e. .
-00001be0: 6e00 6900 6300 6800 7400 2000 6500 7200  n.i.c.h.t. .e.r.
-00001bf0: 7300 7400 6500 6c00 6c00 7400 2000 7700  s.t.e.l.l.t. .w.
-00001c00: 6500 7200 6400 6500 6e00 2e00 0a00 4400  e.r.d.e.n.....D.
-00001c10: 6900 6500 2000 4400 6100 7400 6500 6900  i.e. .D.a.t.e.i.
-00001c20: 2000 6500 7800 6900 7300 7400 6900 6500   .e.x.i.s.t.i.e.
-00001c30: 7200 7400 2000 6200 6500 7200 6500 6900  r.t. .b.e.r.e.i.
-00001c40: 7400 7300 2e08 0000 0000 0600 0000 4041  t.s...........@A
-00001c50: 2064 6174 6162 6173 6520 6261 636b 7570   database backup
-00001c60: 2063 6f75 6c64 206e 6f74 2062 6520 6372   could not be cr
-00001c70: 6561 7465 642e 0a54 6865 2066 696c 6520  eated..The file 
-00001c80: 616c 7265 6164 7920 6578 6973 7473 2e07  already exists..
-00001c90: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00001ca0: 0000 4e00 4500 6900 6e00 2000 4100 4400  ..N.E.i.n. .A.D.
-00001cb0: 4900 4600 2d00 4600 6500 6c00 6400 2000  I.F.-.F.e.l.d. .
-00001cc0: 6600 6500 6800 6c00 7400 2000 6600 fc00  f.e.h.l.t. .f...
-00001cd0: 7200 2000 6400 6500 6e00 2000 4c00 6f00  r. .d.e.n. .L.o.
-00001ce0: 5400 5700 2d00 5500 7000 6c00 6f00 6100  T.W.-.U.p.l.o.a.
-00001cf0: 6408 0000 0000 0600 0000 1d41 2066 6965  d..........A fie
-00001d00: 6c64 2069 7320 6d69 7373 696e 6720 666f  ld is missing fo
-00001d10: 7220 7570 6c6f 6164 0700 0000 0944 7261  r upload.....Dra
-00001d20: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00001d30: 0006 0000 0015 4144 4946 2033 2028 2a2e  ......ADIF 3 (*.
-00001d40: 6164 6920 2a2e 6164 6966 2907 0000 0009  adi *.adif).....
-00001d50: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-00001d60: 0000 0000 0600 0000 1b41 4449 4620 3320  .........ADIF 3 
-00001d70: 282a 2e61 6478 202a 2e61 6469 202a 2e61  (*.adx *.adi *.a
-00001d80: 6469 6629 0700 0000 0944 7261 676f 6e4c  dif).....DragonL
-00001d90: 6f67 0103 0000 0008 00dc 0062 0065 0072  og.........b.e.r
-00001da0: 0800 0000 0006 0000 0005 4162 6f75 7407  ..........About.
-00001db0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00001dc0: 0000 0e00 dc00 6200 6500 7200 2000 5100  ......b.e.r. .Q.
-00001dd0: 7408 0000 0000 0600 0000 0841 626f 7574  t..........About
-00001de0: 2051 7407 0000 0009 4472 6167 6f6e 4c6f   Qt.....DragonLo
-00001df0: 6701 0300 0000 2000 4100 6900 7200 6300  g..... .A.i.r.c.
-00001e00: 7200 6100 6600 7400 2d00 5300 6300 6100  r.a.f.t.-.S.c.a.
-00001e10: 7400 7400 6500 7208 0000 0000 0600 0000  t.t.e.r.........
-00001e20: 1041 6972 6372 6166 7420 5363 6174 7465  .Aircraft Scatte
-00001e30: 7207 0000 0009 4472 6167 6f6e 4c6f 6701  r.....DragonLog.
-00001e40: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
-00001e50: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
-00001e60: 656e 6e61 0700 0000 0944 7261 676f 6e4c  enna.....DragonL
-00001e70: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00001e80: 0006 4175 726f 7261 0700 0000 0944 7261  ..Aurora.....Dra
-00001e90: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00001ea0: 0006 0000 0008 4175 726f 7261 2d45 0700  ......Aurora-E..
-00001eb0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00001ec0: 000a 0041 0075 0074 006f 0072 0800 0000  ...A.u.t.o.r....
-00001ed0: 0006 0000 0006 4175 7468 6f72 0700 0000  ......Author....
-00001ee0: 0944 7261 676f 6e4c 6f67 0103 0000 0018  .DragonLog......
-00001ef0: 0042 0061 0063 006b 002d 0053 0063 0061  .B.a.c.k.-.S.c.a
-00001f00: 0074 0074 0065 0072 0800 0000 0006 0000  .t.t.e.r........
-00001f10: 000c 4261 636b 2073 6361 7474 6572 0700  ..Back scatter..
-00001f20: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
-00001f30: ffff 0800 0000 0006 0000 0004 4261 6e64  ............Band
-00001f40: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001f50: 0000 0022 0043 0053 0056 002d 0044 0061  ...".C.S.V.-.D.a
-00001f60: 0074 0065 0069 0020 0028 002a 002e 0063  .t.e.i. .(.*...c
-00001f70: 0073 0076 0029 0800 0000 0006 0000 0010  .s.v.)..........
-00001f80: 4353 562d 4669 6c65 2028 2a2e 6373 7629  CSV-File (*.csv)
-00001f90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001fa0: 0000 0014 0052 0075 0066 007a 0065 0069  .....R.u.f.z.e.i
-00001fb0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-00001fc0: 0009 4361 6c6c 2073 6967 6e07 0000 0009  ..Call sign.....
-00001fd0: 4472 6167 6f6e 4c6f 6701 0300 0000 0a00  DragonLog.......
-00001fe0: 4b00 6100 6e00 6100 6c08 0000 0000 0600  K.a.n.a.l.......
-00001ff0: 0000 0743 6861 6e6e 656c 0700 0000 0944  ...Channel.....D
-00002000: 7261 676f 6e4c 6f67 0103 0000 0074 0050  ragonLog.....t.P
-00002010: 0072 00fc 0066 0075 006e 0067 0020 0064  .r...f.u.n.g. .d
-00002020: 0065 0072 0020 0044 0061 0074 0065 006e  .e.r. .D.a.t.e.n
-00002030: 0062 0061 006e 006b 0020 0066 0065 0068  .b.a.n.k. .f.e.h
-00002040: 006c 0067 0065 0073 0063 0068 006c 0061  .l.g.e.s.c.h.l.a
-00002050: 0067 0065 006e 002e 0020 0049 006e 0068  .g.e.n... .I.n.h
-00002060: 0061 006c 0074 0020 006e 0069 0063 0068  .a.l.t. .n.i.c.h
-00002070: 0074 0020 006c 0065 0073 0062 0061 0072  .t. .l.e.s.b.a.r
-00002080: 002e 0800 0000 0006 0000 0034 4368 6563  ...........4Chec
-00002090: 6b69 6e67 2064 6174 6162 6173 6520 6661  king database fa
-000020a0: 696c 6564 2e20 436f 6e74 656e 7420 6973  iled. Content is
-000020b0: 206e 6f74 2061 6363 6573 7361 626c 652e   not accessable.
-000020c0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-000020d0: 0000 0012 004b 006f 006d 006d 0065 006e  .....K.o.m.m.e.n
-000020e0: 0074 0061 0072 0800 0000 0006 0000 0007  .t.a.r..........
-000020f0: 436f 6d6d 656e 7407 0000 0009 4472 6167  Comment.....Drag
-00002100: 6f6e 4c6f 6701 0300 0000 6000 5600 6500  onLog.....`.V.e.
-00002110: 7200 6200 6900 6e00 6400 7500 6e00 6700  r.b.i.n.d.u.n.g.
-00002120: 7300 6600 6500 6800 6c00 6500 7200 2000  s.f.e.h.l.e.r. .
-00002130: 6f00 6400 6500 7200 2000 4e00 6500 7400  o.d.e.r. .N.e.t.
-00002140: 7a00 7700 6500 7200 6b00 2000 6e00 6900  z.w.e.r.k. .n.i.
-00002150: 6300 6800 7400 2000 6500 7200 7200 6500  c.h.t. .e.r.r.e.
-00002160: 6900 6300 6800 6200 6100 7208 0000 0000  i.c.h.b.a.r.....
-00002170: 0600 0000 2743 6f6e 6e65 6374 696f 6e20  ....'Connection 
-00002180: 6572 726f 7220 6f72 206e 6574 776f 726b  error or network
-00002190: 2075 6e72 6561 6368 6162 6c65 0700 0000   unreachable....
-000021a0: 0944 7261 676f 6e4c 6f67 0103 0000 002e  .DragonLog......
-000021b0: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
-000021c0: 006b 002d 0042 0061 0063 006b 0075 0070  .k.-.B.a.c.k.u.p
-000021d0: 0020 0046 0065 0068 006c 0065 0072 0800  . .F.e.h.l.e.r..
-000021e0: 0000 0006 0000 0015 4461 7461 6261 7365  ........Database
-000021f0: 2062 6163 6b75 7020 6572 726f 7207 0000   backup error...
-00002200: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002210: 2c00 4400 6100 7400 6500 6e00 6200 6100  ,.D.a.t.e.n.b.a.
-00002220: 6e00 6b00 6b00 6f00 6e00 7600 6500 7200  n.k.k.o.n.v.e.r.
-00002230: 7400 6900 6500 7200 7500 6e00 6708 0000  t.i.e.r.u.n.g...
-00002240: 0000 0600 0000 1344 6174 6162 6173 6520  .......Database 
-00002250: 636f 6e76 6572 7369 6f6e 0700 0000 0944  conversion.....D
-00002260: 7261 676f 6e4c 6f67 0103 0000 0048 0044  ragonLog.....H.D
-00002270: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
-00002280: 006b 006f 006e 0076 0065 0072 0074 0069  .k.o.n.v.e.r.t.i
-00002290: 0065 0072 0075 006e 0067 0020 0061 0062  .e.r.u.n.g. .a.b
-000022a0: 0067 0065 0073 0063 0068 006c 006f 0073  .g.e.s.c.h.l.o.s
-000022b0: 0073 0065 006e 0800 0000 0006 0000 001c  .s.e.n..........
-000022c0: 4461 7461 6261 7365 2063 6f6e 7665 7273  Database convers
-000022d0: 696f 6e20 6669 6e69 7368 6564 0700 0000  ion finished....
-000022e0: 0944 7261 676f 6e4c 6f67 0103 0000 001e  .DragonLog......
-000022f0: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
-00002300: 006b 0066 0065 0068 006c 0065 0072 0800  .k.f.e.h.l.e.r..
-00002310: 0000 0006 0000 000e 4461 7461 6261 7365  ........Database
-00002320: 2065 7272 6f72 0700 0000 0944 7261 676f   error.....Drago
-00002330: 6e4c 6f67 0103 0000 0034 0044 0061 0074  nLog.....4.D.a.t
-00002340: 0065 006e 0062 0061 006e 006b 0073 0074  .e.n.b.a.n.k.s.t
-00002350: 0072 0075 006b 0074 0075 0072 0020 0076  .r.u.k.t.u.r. .v
-00002360: 0065 0072 0061 006c 0074 0065 0074 0800  .e.r.a.l.t.e.t..
-00002370: 0000 0006 0000 001c 4461 7461 6261 7365  ........Database
-00002380: 2073 7472 7563 7475 7265 206f 7574 2d64   structure out-d
-00002390: 6174 6564 0700 0000 0944 7261 676f 6e4c  ated.....DragonL
-000023a0: 6f67 0103 0000 001e 0044 0061 0074 0075  og.......D.a.t.u
-000023b0: 006d 002f 005a 0065 0069 0074 0020 0045  .m./.Z.e.i.t. .E
-000023c0: 006e 0064 0065 0800 0000 0006 0000 000d  .n.d.e..........
-000023d0: 4461 7465 2f54 696d 6520 656e 6407 0000  Date/Time end...
-000023e0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-000023f0: 2000 4400 6100 7400 7500 6d00 2f00 5a00   .D.a.t.u.m./.Z.
-00002400: 6500 6900 7400 2000 5300 7400 6100 7200  e.i.t. .S.t.a.r.
-00002410: 7408 0000 0000 0600 0000 0f44 6174 652f  t..........Date/
-00002420: 5469 6d65 2073 7461 7274 0700 0000 0944  Time start.....D
-00002430: 7261 676f 6e4c 6f67 0103 0000 0016 0051  ragonLog.......Q
-00002440: 0053 004f 0020 006c 00f6 0073 0063 0068  .S.O. .l...s.c.h
-00002450: 0065 006e 0800 0000 0006 0000 000a 4465  .e.n..........De
-00002460: 6c65 7465 2051 534f 0700 0000 0944 7261  lete QSO.....Dra
-00002470: 676f 6e4c 6f67 0103 0000 0014 0045 006e  gonLog.......E.n
-00002480: 0074 0066 0065 0072 006e 0075 006e 0067  .t.f.e.r.n.u.n.g
-00002490: 0800 0000 0006 0000 0008 4469 7374 616e  ..........Distan
-000024a0: 6365 0700 0000 0944 7261 676f 6e4c 6f67  ce.....DragonLog
-000024b0: 0103 0000 0064 0057 006f 006c 006c 0065  .....d.W.o.l.l.e
-000024c0: 006e 0020 0073 0069 0065 0020 0064 0069  .n. .s.i.e. .d.i
-000024d0: 0065 0020 0073 0065 006c 0065 006b 0074  .e. .s.e.l.e.k.t
-000024e0: 0069 0065 0072 0074 0065 006e 0020 0051  .i.e.r.t.e.n. .Q
-000024f0: 0053 004f 0073 0020 0077 0069 0072 006b  .S.O.s. .w.i.r.k
-00002500: 006c 0069 0063 0068 0020 006c 00f6 0073  .l.i.c.h. .l...s
-00002510: 0063 0068 0065 006e 003f 0800 0000 0006  .c.h.e.n.?......
-00002520: 0000 0031 446f 2079 6f75 2072 6561 6c6c  ...1Do you reall
-00002530: 7920 7761 6e74 2074 6f20 6465 6c65 7465  y want to delete
-00002540: 2074 6865 2073 656c 6563 7465 6420 5153   the selected QS
-00002550: 4f28 7329 3f07 0000 0009 4472 6167 6f6e  O(s)?.....Dragon
-00002560: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
-00002570: 0000 1045 6172 7468 2d4d 6f6f 6e2d 4561  ...Earth-Moon-Ea
-00002580: 7274 6807 0000 0009 4472 6167 6f6e 4c6f  rth.....DragonLo
-00002590: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-000025a0: 0845 6368 6f4c 696e 6b07 0000 0009 4472  .EchoLink.....Dr
-000025b0: 6167 6f6e 4c6f 6701 0300 0000 0c00 4600  agonLog.......F.
-000025c0: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
-000025d0: 0000 0545 7272 6f72 0700 0000 0944 7261  ...Error.....Dra
-000025e0: 676f 6e4c 6f67 0103 0000 0028 0045 0078  gonLog.....(.E.x
-000025f0: 0063 0065 006c 002d 0044 0061 0074 0065  .c.e.l.-.D.a.t.e
-00002600: 0069 0020 0028 002a 002e 0078 006c 0073  .i. .(.*...x.l.s
-00002610: 0078 0029 0800 0000 0006 0000 0013 4578  .x.)..........Ex
-00002620: 6365 6c2d 4669 6c65 2028 2a2e 786c 7378  cel-File (*.xlsx
-00002630: 2907 0000 0009 4472 6167 6f6e 4c6f 6701  ).....DragonLog.
-00002640: 0300 0000 2400 4500 7800 7000 6f00 7200  ....$.E.x.p.o.r.
-00002650: 7400 6900 6500 7200 6500 2000 5100 5300  t.i.e.r.e. .Q.S.
-00002660: 4f00 2000 6c00 6f00 6708 0000 0000 0600  O. .l.o.g.......
-00002670: 0000 1045 7870 6f72 7465 6420 5153 4f20  ...Exported QSO 
-00002680: 6c6f 6707 0000 0009 4472 6167 6f6e 4c6f  log.....DragonLo
-00002690: 6701 0300 0000 1a00 4600 3200 2d00 5200  g.......F.2.-.R.
-000026a0: 6500 6600 6c00 6500 6b00 7400 6900 6f00  e.f.l.e.k.t.i.o.
-000026b0: 6e08 0000 0000 0600 0000 0d46 3220 5265  n..........F2 Re
-000026c0: 666c 6563 7469 6f6e 0700 0000 0944 7261  flection.....Dra
-000026d0: 676f 6e4c 6f67 0103 0000 0038 0046 0069  gonLog.....8.F.i
-000026e0: 0065 006c 0064 002d 0041 006c 0069 0067  .e.l.d.-.A.l.i.g
-000026f0: 006e 0065 0064 002d 0049 0072 0072 0065  .n.e.d.-.I.r.r.e
-00002700: 0067 0075 006c 0061 0072 0069 0074 0069  .g.u.l.a.r.i.t.i
-00002710: 0065 0073 0800 0000 0006 0000 001c 4669  .e.s..........Fi
-00002720: 656c 6420 416c 6967 6e65 6420 4972 7265  eld Aligned Irre
-00002730: 6775 6c61 7269 7469 6573 0700 0000 0944  gularities.....D
-00002740: 7261 676f 6e4c 6f67 0103 0000 0010 0046  ragonLog.......F
-00002750: 0072 0065 0071 0075 0065 006e 007a 0800  .r.e.q.u.e.n.z..
-00002760: 0000 0006 0000 0009 4672 6571 7565 6e63  ........Frequenc
-00002770: 7907 0000 0009 4472 6167 6f6e 4c6f 6701  y.....DragonLog.
-00002780: 0300 0000 1400 4200 6f00 6400 6500 6e00  ......B.o.d.e.n.
-00002790: 7700 6500 6c00 6c00 6508 0000 0000 0600  w.e.l.l.e.......
-000027a0: 0000 0b47 726f 756e 6420 5761 7665 0700  ...Ground Wave..
-000027b0: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
-000027c0: ffff 0800 0000 0006 0000 0006 4861 6d51  ............HamQ
-000027d0: 5448 0700 0000 0944 7261 676f 6e4c 6f67  TH.....DragonLog
-000027e0: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
-000027f0: 4861 6d6c 6962 0700 0000 0944 7261 676f  Hamlib.....Drago
-00002800: 6e4c 6f67 0103 0000 000a 0048 0069 006c  nLog.......H.i.l
-00002810: 0066 0065 0800 0000 0006 0000 0004 4865  .f.e..........He
-00002820: 6c70 0700 0000 0944 7261 676f 6e4c 6f67  lp.....DragonLog
-00002830: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
-00002840: 4952 4c50 0700 0000 0944 7261 676f 6e4c  IRLP.....DragonL
-00002850: 6f67 0103 0000 0026 0049 006e 0074 0065  og.....&.I.n.t.e
-00002860: 0072 006e 0065 0074 0075 006e 0074 0065  .r.n.e.t.u.n.t.e
-00002870: 0072 0073 0074 00fc 0074 007a 0074 0800  .r.s.t...t.z.t..
-00002880: 0000 0006 0000 0011 496e 7465 726e 6574  ........Internet
-00002890: 2d61 7373 6973 7465 6407 0000 0009 4472  -assisted.....Dr
-000028a0: 6167 6f6e 4c6f 6701 0300 0000 1800 4900  agonLog.......I.
-000028b0: 6f00 6e00 6f00 2d00 5300 6300 6100 7400  o.n.o.-.S.c.a.t.
-000028c0: 7400 6500 7208 0000 0000 0600 0000 0b49  t.e.r..........I
-000028d0: 6f6e 6f73 6361 7474 6572 0700 0000 0944  onoscatter.....D
-000028e0: 7261 676f 6e4c 6f67 0103 0000 0020 006c  ragonLog..... .l
-000028f0: 0065 0074 007a 0074 0065 0073 0020 0048  .e.t.z.t.e.s. .H
-00002900: 0061 006c 0062 006a 0061 0068 0072 0800  .a.l.b.j.a.h.r..
-00002910: 0000 0006 0000 000e 4c61 7374 2068 616c  ........Last hal
-00002920: 6620 7965 6172 0700 0000 0944 7261 676f  f year.....Drago
-00002930: 6e4c 6f67 0103 0000 001a 006c 0065 0074  nLog.......l.e.t
-00002940: 007a 0074 0065 006e 0020 004d 006f 006e  .z.t.e.n. .M.o.n
-00002950: 0061 0074 0800 0000 0006 0000 000a 4c61  .a.t..........La
-00002960: 7374 206d 6f6e 7468 0700 0000 0944 7261  st month.....Dra
-00002970: 676f 6e4c 6f67 0103 0000 0018 006c 0065  gonLog.......l.e
-00002980: 0074 007a 0074 0065 0020 0057 006f 0063  .t.z.t.e. .W.o.c
-00002990: 0068 0065 0800 0000 0006 0000 0009 4c61  .h.e..........La
-000029a0: 7374 2077 6565 6b07 0000 0009 4472 6167  st week.....Drag
-000029b0: 6f6e 4c6f 6701 0300 0000 1800 6c00 6500  onLog.......l.e.
-000029c0: 7400 7a00 7400 6500 7300 2000 4a00 6100  t.z.t.e.s. .J.a.
-000029d0: 6800 7208 0000 0000 0600 0000 094c 6173  h.r..........Las
-000029e0: 7420 7965 6172 0700 0000 0944 7261 676f  t year.....Drago
-000029f0: 6e4c 6f67 0103 0000 001e 0053 0069 0063  nLog.......S.i.c
-00002a00: 0068 0074 0076 0065 0072 0062 0069 006e  .h.t.v.e.r.b.i.n
-00002a10: 0064 0075 006e 0067 0800 0000 0006 0000  .d.u.n.g........
-00002a20: 000d 4c69 6e65 206f 6620 5369 6768 7407  ..Line of Sight.
-00002a30: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002a40: 0000 2000 4c00 6f00 5400 5700 2d00 4100  .. .L.o.T.W.-.A.
-00002a50: 4400 4900 4600 2d00 5500 7000 6c00 6f00  D.I.F.-.U.p.l.o.
-00002a60: 6100 6408 0000 0000 0600 0000 104c 6f54  a.d..........LoT
-00002a70: 5720 4144 4946 2075 706c 6f61 6407 0000  W ADIF upload...
-00002a80: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002a90: 1400 4c00 6f00 5400 5700 2000 6500 6d00  ..L.o.T.W. .e.m.
-00002aa0: 7000 6600 2e08 0000 0000 0600 0000 094c  p.f............L
-00002ab0: 6f54 5720 7263 7664 0700 0000 0944 7261  oTW rcvd.....Dra
-00002ac0: 676f 6e4c 6f67 0103 0000 0014 004c 006f  gonLog.......L.o
-00002ad0: 0054 0057 0020 0076 0065 0072 0073 002e  .T.W. .v.e.r.s..
-00002ae0: 0800 0000 0006 0000 0009 4c6f 5457 2073  ..........LoTW s
-00002af0: 656e 7407 0000 0009 4472 6167 6f6e 4c6f  ent.....DragonLo
-00002b00: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00002b10: 074c 6f63 6174 6f72 0700 0000 0944 7261  .Locator.....Dra
-00002b20: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00002b30: 0006 0000 000f 4c6f 6720 696d 706f 7274  ......Log import
-00002b40: 2041 4449 4607 0000 0009 4472 6167 6f6e   ADIF.....Dragon
-00002b50: 4c6f 6701 0300 0000 1c00 4c00 6f00 6700  Log.......L.o.g.
-00002b60: 2000 4900 6d00 7000 6f00 7200 7400 2000   .I.m.p.o.r.t. .
-00002b70: 4300 5300 5608 0000 0000 0600 0000 0e4c  C.S.V..........L
-00002b80: 6f67 2069 6d70 6f72 7420 4353 5607 0000  og import CSV...
-00002b90: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002ba0: 2000 4c00 6f00 6700 2000 4900 6d00 7000   .L.o.g. .I.m.p.
-00002bb0: 6f00 7200 7400 2000 4500 7800 6300 6500  o.r.t. .E.x.c.e.
-00002bc0: 6c08 0000 0000 0600 0000 104c 6f67 2069  l..........Log i
-00002bd0: 6d70 6f72 7420 4578 6365 6c07 0000 0009  mport Excel.....
-00002be0: 4472 6167 6f6e 4c6f 6701 0300 0000 1c00  DragonLog.......
-00002bf0: 4d00 6500 7400 6500 6f00 7200 2d00 5300  M.e.t.e.o.r.-.S.
-00002c00: 6300 6100 7400 7400 6500 7208 0000 0000  c.a.t.t.e.r.....
-00002c10: 0600 0000 0e4d 6574 656f 7220 7363 6174  .....Meteor scat
-00002c20: 7465 7207 0000 0009 4472 6167 6f6e 4c6f  ter.....DragonLo
-00002c30: 6701 0300 0000 5a00 4b00 6500 6900 6e00  g.....Z.K.e.i.n.
-00002c40: 6500 2000 5300 7400 6100 7400 6900 6f00  e. .S.t.a.t.i.o.
-00002c50: 6e00 7300 6b00 6f00 6e00 6600 6900 6700  n.s.k.o.n.f.i.g.
-00002c60: 7500 7200 6100 7400 6900 6f00 6e00 2000  u.r.a.t.i.o.n. .
-00002c70: 6900 6e00 2000 5400 5100 5300 4c00 2000  i.n. .T.Q.S.L. .
-00002c80: 7600 6500 7200 6600 fc00 6700 6200 6100  v.e.r.f...g.b.a.
-00002c90: 7208 0000 0000 0600 0000 254d 6973 7369  r.........%Missi
-00002ca0: 6e67 2073 7461 7469 6f6e 2063 6f6e 6669  ng station confi
-00002cb0: 6775 7261 7469 6f6e 2069 6e20 5451 534c  guration in TQSL
-00002cc0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002cd0: ffff ffff 0800 0000 0006 0000 0004 4d6f  ..............Mo
-00002ce0: 6465 0700 0000 0944 7261 676f 6e4c 6f67  de.....DragonLog
-00002cf0: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
-00002d00: 4e61 6d65 0700 0000 0944 7261 676f 6e4c  Name.....DragonL
-00002d10: 6f67 0103 0000 0034 004b 0065 0069 006e  og.....4.K.e.i.n
-00002d20: 0065 0020 0051 0053 004f 0073 0020 0066  .e. .Q.S.O.s. .f
-00002d30: 00fc 0072 0020 0064 0065 006e 0020 004c  ...r. .d.e.n. .L
-00002d40: 006f 0063 0061 0074 006f 0072 0800 0000  .o.c.a.t.o.r....
-00002d50: 0006 0000 0017 4e6f 2072 6563 6f72 6473  ......No records
-00002d60: 2066 6f72 206c 6f63 6174 696f 6e07 0000   for location...
-00002d70: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002d80: 0e00 4e00 6f00 7400 6900 7a00 6500 6e08  ..N.o.t.i.z.e.n.
-00002d90: 0000 0000 0600 0000 054e 6f74 6573 0700  .........Notes..
-00002da0: 0000 0944 7261 676f 6e4c 6f67 0103 ffff  ...DragonLog....
-00002db0: ffff 0800 0000 0006 0000 0002 4f6b 0700  ............Ok..
-00002dc0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002dd0: 001e 0045 0069 0067 0065 006e 0065 0072  ...E.i.g.e.n.e.r
-00002de0: 0020 004c 006f 0063 0061 0074 006f 0072  . .L.o.c.a.t.o.r
-00002df0: 0800 0000 0006 0000 000b 4f77 6e20 4c6f  ..........Own Lo
-00002e00: 6361 746f 7207 0000 0009 4472 6167 6f6e  cator.....Dragon
-00002e10: 4c6f 6701 0300 0000 1800 4500 6900 6700  Log.......E.i.g.
-00002e20: 6500 6e00 6500 7200 2000 4e00 6100 6d00  e.n.e.r. .N.a.m.
-00002e30: 6508 0000 0000 0600 0000 084f 776e 204e  e..........Own N
-00002e40: 616d 6507 0000 0009 4472 6167 6f6e 4c6f  ame.....DragonLo
-00002e50: 6701 0300 0000 1600 4500 6900 6700 6500  g.......E.i.g.e.
-00002e60: 6e00 6500 7200 2000 5100 5400 4808 0000  n.e.r. .Q.T.H...
-00002e70: 0000 0600 0000 074f 776e 2051 5448 0700  .......Own QTH..
-00002e80: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002e90: 0024 0045 0069 0067 0065 006e 0065 0073  .$.E.i.g.e.n.e.s
-00002ea0: 0020 0052 0075 0066 007a 0065 0069 0063  . .R.u.f.z.e.i.c
-00002eb0: 0068 0065 006e 0800 0000 0006 0000 000d  .h.e.n..........
-00002ec0: 4f77 6e20 6361 6c6c 2073 6967 6e07 0000  Own call sign...
-00002ed0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002ee0: 1000 4c00 6500 6900 7300 7400 7500 6e00  ..L.e.i.s.t.u.n.
-00002ef0: 6708 0000 0000 0600 0000 0550 6f77 6572  g..........Power
-00002f00: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002f10: 0000 0016 0041 0075 0073 0062 0072 0065  .....A.u.s.b.r.e
-00002f20: 0069 0074 0075 006e 0067 0800 0000 0006  .i.t.u.n.g......
-00002f30: 0000 000b 5072 6f70 6167 6174 696f 6e07  ....Propagation.
-00002f40: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002f50: 0000 1a00 5100 5300 4c00 2d00 4e00 6100  ....Q.S.L.-.N.a.
-00002f60: 6300 6800 7200 6900 6300 6800 7408 0000  c.h.r.i.c.h.t...
-00002f70: 0000 0600 0000 0b51 534c 206d 6573 7361  .......QSL messa
-00002f80: 6765 0700 0000 0944 7261 676f 6e4c 6f67  ge.....DragonLog
-00002f90: 0103 0000 0010 0051 0053 004c 002d 0050  .......Q.S.L.-.P
-00002fa0: 0066 0061 0064 0800 0000 0006 0000 0008  .f.a.d..........
-00002fb0: 5153 4c20 7061 7468 0700 0000 0944 7261  QSL path.....Dra
-00002fc0: 676f 6e4c 6f67 0103 0000 0012 0051 0053  gonLog.......Q.S
-00002fd0: 004c 0020 0065 006d 0070 0066 002e 0800  .L. .e.m.p.f....
-00002fe0: 0000 0006 0000 0008 5153 4c20 7263 7664  ........QSL rcvd
-00002ff0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003000: 0000 0012 0051 0053 004c 0020 0076 0065  .....Q.S.L. .v.e
-00003010: 0072 0073 002e 0800 0000 0006 0000 0008  .r.s............
-00003020: 5153 4c20 7365 6e74 0700 0000 0944 7261  QSL sent.....Dra
-00003030: 676f 6e4c 6f67 0103 0000 000e 0051 0053  gonLog.......Q.S
-00003040: 004c 002d 0056 0069 0061 0800 0000 0006  .L.-.V.i.a......
-00003050: 0000 0007 5153 4c20 7669 6107 0000 0009  ....QSL via.....
-00003060: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-00003070: 0000 0000 0600 0000 0351 534f 0700 0000  .........QSO....
-00003080: 0944 7261 676f 6e4c 6f67 0103 0000 0048  .DragonLog.....H
-00003090: 0051 0053 004f 002d 004c 006f 0067 0020  .Q.S.O.-.L.o.g. 
-000030a0: 0028 002a 002e 0071 006c 006f 0067 0029  .(.*...q.l.o.g.)
-000030b0: 003b 003b 0041 006c 006c 0065 0020 0044  .;.;.A.l.l.e. .D
-000030c0: 0061 0074 0065 0069 0065 006e 0020 0028  .a.t.e.i.e.n. .(
-000030d0: 002a 002e 002a 0029 0800 0000 0006 0000  .*...*.)........
-000030e0: 0021 5153 4f2d 4c6f 6720 282a 2e71 6c6f  .!QSO-Log (*.qlo
-000030f0: 6729 3b3b 416c 6c20 4669 6c65 7320 282a  g);;All Files (*
-00003100: 2e2a 2907 0000 0009 4472 6167 6f6e 4c6f  .*).....DragonLo
-00003110: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00003120: 0351 5448 0700 0000 0944 7261 676f 6e4c  .QTH.....DragonL
-00003130: 6f67 0103 0000 0012 0052 0053 0054 0020  og.......R.S.T. 
-00003140: 0065 006d 0070 0066 002e 0800 0000 0006  .e.m.p.f........
-00003150: 0000 0008 5253 5420 7263 7664 0700 0000  ....RST rcvd....
-00003160: 0944 7261 676f 6e4c 6f67 0103 0000 0010  .DragonLog......
-00003170: 0052 0053 0054 0020 0067 0065 0073 002e  .R.S.T. .g.e.s..
-00003180: 0800 0000 0006 0000 0008 5253 5420 7365  ..........RST se
-00003190: 6e74 0700 0000 0944 7261 676f 6e4c 6f67  nt.....DragonLog
-000031a0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
-000031b0: 5261 6469 6f07 0000 0009 4472 6167 6f6e  Radio.....Dragon
-000031c0: 4c6f 6701 0300 0000 1800 5200 6100 6900  Log.......R.a.i.
-000031d0: 6e00 2d00 5300 6300 6100 7400 7400 6500  n.-.S.c.a.t.t.e.
-000031e0: 7208 0000 0000 0600 0000 0c52 6169 6e20  r..........Rain 
-000031f0: 7363 6174 7465 7207 0000 0009 4472 6167  scatter.....Drag
-00003200: 6f6e 4c6f 6701 0300 0000 3200 5200 6500  onLog.....2.R.e.
-00003210: 7000 6500 6100 7400 6500 7200 2000 6f00  p.e.a.t.e.r. .o.
-00003220: 6400 6500 7200 2000 5400 7200 6100 6e00  d.e.r. .T.r.a.n.
-00003230: 7300 7000 6f00 6e00 6400 6500 7208 0000  s.p.o.n.d.e.r...
-00003240: 0000 0600 0000 1752 6570 6561 7465 7220  .......Repeater 
-00003250: 6f72 2054 7261 6e73 706f 6e64 6572 0700  or Transponder..
-00003260: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00003270: 0010 0053 0061 0074 0065 006c 006c 0069  ...S.a.t.e.l.l.i
-00003280: 0074 0800 0000 0006 0000 0009 5361 7465  .t..........Sate
-00003290: 6c6c 6974 6507 0000 0009 4472 6167 6f6e  llite.....Dragon
-000032a0: 4c6f 6701 0300 0000 2a00 4500 7800 7000  Log.....*.E.x.p.
-000032b0: 6f00 7200 7400 6400 6100 7400 6500 6900  o.r.t.d.a.t.e.i.
-000032c0: 2000 7300 7000 6500 6900 6300 6800 6500   .s.p.e.i.c.h.e.
-000032d0: 7200 6e08 0000 0000 0600 0000 1253 656c  r.n..........Sel
-000032e0: 6563 7420 6578 706f 7274 2066 696c 6507  ect export file.
-000032f0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00003300: 0000 2000 4400 6100 7400 6500 6e00 6200  .. .D.a.t.e.n.b.
-00003310: 6100 6e00 6b00 2000 f600 6600 6600 6e00  a.n.k. ...f.f.n.
-00003320: 6500 6e08 0000 0000 0600 0000 0b53 656c  e.n..........Sel
-00003330: 6563 7420 6669 6c65 0700 0000 0944 7261  ect file.....Dra
-00003340: 676f 6e4c 6f67 0103 0000 0038 005a 0075  gonLog.....8.Z.u
-00003350: 0020 00fc 0062 0065 0072 0077 0061 0063  . ...b.e.r.w.a.c
-00003360: 0068 0065 006e 0064 0065 0020 0044 0061  .h.e.n.d.e. .D.a
-00003370: 0074 0065 0069 0020 0077 00e4 0068 006c  .t.e.i. .w...h.l
-00003380: 0065 006e 0800 0000 0006 0000 0014 5365  .e.n..........Se
-00003390: 6c65 6374 2066 696c 6520 746f 2077 6174  lect file to wat
-000033a0: 6368 0700 0000 0944 7261 676f 6e4c 6f67  ch.....DragonLog
-000033b0: 0103 0000 0024 0049 006d 0070 006f 0072  .....$.I.m.p.o.r
-000033c0: 0074 0064 0061 0074 0065 0069 0020 00f6  .t.d.a.t.e.i. ..
-000033d0: 0066 0066 006e 0065 006e 0800 0000 0006  .f.f.n.e.n......
-000033e0: 0000 0012 5365 6c65 6374 2069 6d70 6f72  ....Select impor
-000033f0: 7420 6669 6c65 0700 0000 0944 7261 676f  t file.....Drago
-00003400: 6e4c 6f67 0103 0000 001a 0057 00e4 0068  nLog.......W...h
-00003410: 006c 0065 0020 0053 0074 0061 0074 0069  .l.e. .S.t.a.t.i
-00003420: 006f 006e 0800 0000 0006 0000 000e 5365  .o.n..........Se
-00003430: 6c65 6374 2073 7461 7469 6f6e 0700 0000  lect station....
-00003440: 0944 7261 676f 6e4c 6f67 0103 0000 0044  .DragonLog.....D
-00003450: 004c 006f 0054 0057 002d 0053 0065 0072  .L.o.T.W.-.S.e.r
-00003460: 0076 0065 0072 0020 0068 0061 0074 0020  .v.e.r. .h.a.t. 
-00003470: 0064 0061 0073 0020 004c 006f 0067 0020  .d.a.s. .L.o.g. 
-00003480: 0061 0062 0067 0065 0077 0069 0065 0073  .a.b.g.e.w.i.e.s
-00003490: 0065 006e 0800 0000 0006 0000 0013 5365  .e.n..........Se
-000034a0: 7276 6572 2072 656a 6563 7465 6420 6c6f  rver rejected lo
-000034b0: 6707 0000 0009 4472 6167 6f6e 4c6f 6701  g.....DragonLog.
-000034c0: 0300 0000 1400 7a00 6500 6900 6700 6500  ......z.e.i.g.e.
-000034d0: 2000 6100 6c00 6c00 6508 0000 0000 0600   .a.l.l.e.......
-000034e0: 0000 0853 686f 7720 616c 6c07 0000 0009  ...Show all.....
-000034f0: 4472 6167 6f6e 4c6f 6701 0300 0000 1400  DragonLog.......
-00003500: 5300 7000 6f00 7200 6100 6400 6900 6300  S.p.o.r.a.d.i.c.
-00003510: 2d00 4508 0000 0000 0600 0000 0a53 706f  -.E..........Spo
-00003520: 7261 6469 6320 4507 0000 0009 4472 6167  radic E.....Drag
-00003530: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
-00003540: 0600 0000 0753 7562 6d6f 6465 0700 0000  .....Submode....
-00003550: 0944 7261 676f 6e4c 6f67 0103 0000 002a  .DragonLog.....*
-00003560: 0054 0051 0053 004c 002d 0053 0069 0067  .T.Q.S.L.-.S.i.g
-00003570: 006e 0061 0074 0075 0072 0070 0061 0073  .n.a.t.u.r.p.a.s
-00003580: 0073 0077 006f 0072 0074 0800 0000 0006  .s.w.o.r.t......
-00003590: 0000 0017 5451 534c 2073 6967 6e61 7475  ....TQSL signatu
-000035a0: 7265 2070 6173 7377 6f72 6407 0000 0009  re password.....
-000035b0: 4472 6167 6f6e 4c6f 6701 0300 0000 b200  DragonLog.......
-000035c0: 4400 6900 6500 2000 4400 6100 7400 6500  D.i.e. .D.a.t.e.
-000035d0: 6e00 6200 6100 6e00 6b00 7300 7400 7200  n.b.a.n.k.s.t.r.
-000035e0: 7500 6b00 7400 7500 7200 2000 6900 7300  u.k.t.u.r. .i.s.
-000035f0: 7400 2000 7600 6500 7200 6100 6c00 7400  t. .v.e.r.a.l.t.
-00003600: 6500 7400 2000 7500 6e00 6400 2000 6d00  e.t. .u.n.d. .m.
-00003610: 7500 7300 7300 2000 6b00 6f00 6e00 7600  u.s.s. .k.o.n.v.
-00003620: 6500 7200 7400 6900 6500 7200 7400 2000  e.r.t.i.e.r.t. .
-00003630: 7700 6500 7200 6400 6500 6e00 0a00 0a00  w.e.r.d.e.n.....
-00003640: 4500 6900 6e00 2000 4200 6100 6300 6b00  E.i.n. .B.a.c.k.
-00003650: 7500 7000 2000 7700 6900 7200 6400 2000  u.p. .w.i.r.d. .
-00003660: 6500 7200 7300 7400 6500 6c00 6c00 7400  e.r.s.t.e.l.l.t.
-00003670: 3a08 0000 0000 0600 0000 5754 6865 2064  :.........WThe d
-00003680: 6174 6162 6173 6520 7374 7275 6374 7572  atabase structur
-00003690: 6520 6973 206f 7574 2d64 6174 6564 2061  e is out-dated a
-000036a0: 6e64 206e 6565 6473 2061 2063 6f6e 7665  nd needs a conve
-000036b0: 7273 696f 6e0a 0a41 2062 6163 6b75 7020  rsion..A backup 
-000036c0: 7769 6c6c 2062 6520 6765 6e65 7261 7465  will be generate
-000036d0: 643a 0700 0000 0944 7261 676f 6e4c 6f67  d:.....DragonLog
-000036e0: 0103 0000 001e 0054 0072 0061 006e 0073  .......T.r.a.n.s
-000036f0: 0065 0071 0075 0061 0074 006f 0072 0069  .e.q.u.a.t.o.r.i
-00003700: 0061 006c 0800 0000 0006 0000 0010 5472  .a.l..........Tr
-00003710: 616e 732d 6571 7561 746f 7269 616c 0700  ans-equatorial..
-00003720: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00003730: 0028 0054 0072 006f 0070 006f 0073 0070  .(.T.r.o.p.o.s.p
-00003740: 0068 0065 0072 0069 0063 002d 0044 0075  .h.e.r.i.c.-.D.u
-00003750: 0063 0074 0069 006e 0067 0800 0000 0006  .c.t.i.n.g......
-00003760: 0000 0014 5472 6f70 6f73 7068 6572 6963  ....Tropospheric
-00003770: 2064 7563 7469 6e67 0700 0000 0944 7261   ducting.....Dra
-00003780: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00003790: 0006 0000 0007 5665 7273 696f 6e07 0000  ......Version...
-000037a0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-000037b0: 2c00 5000 7200 6f00 6700 7200 6100 6d00  ,.P.r.o.g.r.a.m.
-000037c0: 6d00 6c00 6f00 6700 2000 fc00 6200 6500  m.l.o.g. ...b.e.
-000037d0: 7200 7700 6100 6300 6800 6500 6e08 0000  r.w.a.c.h.e.n...
-000037e0: 0000 0600 0000 1557 6174 6368 2061 7070  .......Watch app
-000037f0: 6c69 6361 7469 6f6e 206c 6f67 0700 0000  lication log....
-00003800: 0944 7261 676f 6e4c 6f67 0103 0000 0020  .DragonLog..... 
-00003810: 0044 0061 0074 0065 0069 00fc 0062 0065  .D.a.t.e.i...b.e
-00003820: 0072 0077 0061 0063 0068 0075 006e 0067  .r.w.a.c.h.u.n.g
-00003830: 0800 0000 0006 0000 000d 5761 7463 6869  ..........Watchi
-00003840: 6e67 2066 696c 6507 0000 0009 4472 6167  ng file.....Drag
-00003850: 6f6e 4c6f 6701 0300 0000 1400 6500 5100  onLog.......e.Q.
-00003860: 5300 4c00 2000 6500 6d00 7000 6600 2e08  S.L. .e.m.p.f...
-00003870: 0000 0000 0600 0000 0965 5153 4c20 7263  .........eQSL rc
-00003880: 7664 0700 0000 0944 7261 676f 6e4c 6f67  vd.....DragonLog
-00003890: 0103 0000 0014 0065 0051 0053 004c 0020  .......e.Q.S.L. 
-000038a0: 0076 0065 0072 0073 002e 0800 0000 0006  .v.e.r.s........
-000038b0: 0000 0009 6551 534c 2073 656e 7407 0000  ....eQSL sent...
-000038c0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-000038d0: 0e00 6900 6e00 6100 6b00 7400 6900 7608  ..i.n.a.k.t.i.v.
-000038e0: 0000 0000 0600 0000 0769 6e61 6374 6976  .........inactiv
-000038f0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003900: 0000 0008 00dc 0062 0065 0072 0800 0000  .......b.e.r....
-00003910: 0006 0000 0005 4162 6f75 7407 0000 000a  ......About.....
-00003920: 4d61 696e 5769 6e64 6f77 0103 0000 000e  MainWindow......
-00003930: 00dc 0062 0065 0072 0020 0051 0074 0800  ...b.e.r. .Q.t..
-00003940: 0000 0006 0000 0008 4162 6f75 7420 5174  ........About Qt
-00003950: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003960: 0300 0000 1a00 4100 6e00 7700 6500 6e00  ......A.n.w.e.n.
-00003970: 6400 7500 6e00 6700 7300 6c00 6f00 6708  d.u.n.g.s.l.o.g.
-00003980: 0000 0000 0600 0000 0f41 7070 6c69 6361  .........Applica
-00003990: 7469 6f6e 204c 6f67 0700 0000 0a4d 6169  tion Log.....Mai
-000039a0: 6e57 696e 646f 7701 0300 0000 2200 4500  nWindow.....".E.
-000039b0: 6900 6e00 7400 7200 6100 6700 2000 e400  i.n.t.r.a.g. ...
-000039c0: 6e00 6400 6500 7200 6e00 2e00 2e00 2e08  n.d.e.r.n.......
-000039d0: 0000 0000 0600 0000 1343 6861 6e67 6520  .........Change 
-000039e0: 6c6f 6720 656e 7472 792e 2e2e 0700 0000  log entry.......
-000039f0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
-00003a00: ff08 0000 0000 0600 0000 0643 7472 6c2b  ...........Ctrl+
-00003a10: 4507 0000 000a 4d61 696e 5769 6e64 6f77  E.....MainWindow
-00003a20: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
-00003a30: 4374 726c 2b4c 0700 0000 0a4d 6169 6e57  Ctrl+L.....MainW
-00003a40: 696e 646f 7701 03ff ffff ff08 0000 0000  indow...........
-00003a50: 0600 0000 0643 7472 6c2b 5107 0000 000a  .....Ctrl+Q.....
-00003a60: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
-00003a70: 0800 0000 0006 0000 0006 4374 726c 2b57  ..........Ctrl+W
-00003a80: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003a90: 03ff ffff ff08 0000 0000 0600 0000 0643  ...............C
-00003aa0: 7472 6c2b 5807 0000 000a 4d61 696e 5769  trl+X.....MainWi
-00003ab0: 6e64 6f77 0103 0000 001e 0045 0069 006e  ndow.......E.i.n
-00003ac0: 0074 0072 0061 0067 0020 006c 00f6 0073  .t.r.a.g. .l...s
-00003ad0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-00003ae0: 0010 4465 6c65 7465 206c 6f67 2065 6e74  ..Delete log ent
-00003af0: 7279 0700 0000 0a4d 6169 6e57 696e 646f  ry.....MainWindo
-00003b00: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
-00003b10: 0944 7261 676f 6e4c 6f67 0700 0000 0a4d  .DragonLog.....M
-00003b20: 6169 6e57 696e 646f 7701 0300 0000 1400  ainWindow.......
-00003b30: 4200 6500 6100 7200 6200 6500 6900 7400  B.e.a.r.b.e.i.t.
-00003b40: 6500 6e08 0000 0000 0600 0000 0445 6469  e.n..........Edi
-00003b50: 7407 0000 000a 4d61 696e 5769 6e64 6f77  t.....MainWindow
-00003b60: 0103 0000 000e 0042 0065 0065 006e 0064  .......B.e.e.n.d
-00003b70: 0065 006e 0800 0000 0006 0000 0004 4578  .e.n..........Ex
-00003b80: 6974 0700 0000 0a4d 6169 6e57 696e 646f  it.....MainWindo
-00003b90: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
-00003ba0: 0645 7870 6f72 7407 0000 000a 4d61 696e  .Export.....Main
-00003bb0: 5769 6e64 6f77 0103 0000 001c 0045 0078  Window.......E.x
-00003bc0: 0070 006f 0072 0074 0069 0065 0072 0065  .p.o.r.t.i.e.r.e
-00003bd0: 006e 002e 002e 002e 0800 0000 0006 0000  .n..............
-00003be0: 0009 4578 706f 7274 2e2e 2e07 0000 000a  ..Export........
-00003bf0: 4d61 696e 5769 6e64 6f77 0103 0000 000a  MainWindow......
-00003c00: 0044 0061 0074 0065 0069 0800 0000 0006  .D.a.t.e.i......
-00003c10: 0000 0004 4669 6c65 0700 0000 0a4d 6169  ....File.....Mai
-00003c20: 6e57 696e 646f 7701 0300 0000 0a00 4800  nWindow.......H.
-00003c30: 6900 6c00 6600 6508 0000 0000 0600 0000  i.l.f.e.........
-00003c40: 0448 656c 7007 0000 000a 4d61 696e 5769  .Help.....MainWi
-00003c50: 6e64 6f77 0103 ffff ffff 0800 0000 0006  ndow............
-00003c60: 0000 0006 496d 706f 7274 0700 0000 0a4d  ....Import.....M
-00003c70: 6169 6e57 696e 646f 7701 0300 0000 1c00  ainWindow.......
-00003c80: 4900 6d00 7000 6f00 7200 7400 6900 6500  I.m.p.o.r.t.i.e.
-00003c90: 7200 6500 6e00 2e00 2e00 2e08 0000 0000  r.e.n...........
-00003ca0: 0600 0000 0949 6d70 6f72 742e 2e2e 0700  .....Import.....
-00003cb0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00003cc0: 0000 1800 4c00 6f00 6700 6700 6500 2000  ....L.o.g.g.e. .
-00003cd0: 5100 5300 4f00 2e00 2e00 2e08 0000 0000  Q.S.O...........
-00003ce0: 0600 0000 0a4c 6f67 2051 534f 2e2e 2e07  .....Log QSO....
-00003cf0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-00003d00: 0000 0018 0051 0053 004f 002d 0046 006f  .....Q.S.O.-.F.o
-00003d10: 0072 006d 0075 006c 0061 0072 0800 0000  .r.m.u.l.a.r....
-00003d20: 0006 0000 0008 5153 4f20 466f 726d 0700  ......QSO Form..
-00003d30: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00003d40: 0000 2600 4400 6100 7400 6500 6e00 6200  ..&.D.a.t.e.n.b.
-00003d50: 6100 6e00 6b00 2000 7700 e400 6800 6c00  a.n.k. .w...h.l.
-00003d60: 6500 6e00 2e00 2e00 2e08 0000 0000 0600  e.n.............
-00003d70: 0000 1253 656c 6563 7420 6461 7461 6261  ...Select databa
-00003d80: 7365 2e2e 2e07 0000 000a 4d61 696e 5769  se........MainWi
-00003d90: 6e64 6f77 0103 0000 001a 0045 0069 006e  ndow.......E.i.n
-00003da0: 0073 0074 0065 006c 006c 0075 006e 0067  .s.t.e.l.l.u.n.g
-00003db0: 0065 006e 0800 0000 0006 0000 0008 5365  .e.n..........Se
-00003dc0: 7474 696e 6773 0700 0000 0a4d 6169 6e57  ttings.....MainW
-00003dd0: 696e 646f 7701 0300 0000 2600 5a00 6500  indow.....&.Z.e.
-00003de0: 6900 6700 6500 2000 4100 6e00 7700 6500  i.g.e. .A.n.w.e.
-00003df0: 6e00 6400 7500 6e00 6700 7300 6c00 6f00  n.d.u.n.g.s.l.o.
-00003e00: 6708 0000 0000 0600 0000 0853 686f 7720  g..........Show 
-00003e10: 6c6f 6707 0000 000a 4d61 696e 5769 6e64  log.....MainWind
-00003e20: 6f77 0103 0000 001a 0053 0074 0061 0072  ow.......S.t.a.r
-00003e30: 0074 0065 0020 0048 0061 006d 006c 0069  .t.e. .H.a.m.l.i
-00003e40: 0062 0800 0000 0006 0000 000c 5374 6172  .b..........Star
-00003e50: 7420 6861 6d6c 6962 0700 0000 0a4d 6169  t hamlib.....Mai
-00003e60: 6e57 696e 646f 7701 0300 0000 1c00 5700  nWindow.......W.
-00003e70: 6500 7200 6b00 7a00 6500 7500 6700 6c00  e.r.k.z.e.u.g.l.
-00003e80: 6500 6900 7300 7400 6508 0000 0000 0600  e.i.s.t.e.......
-00003e90: 0000 0754 6f6f 6c62 6172 0700 0000 0a4d  ...Toolbar.....M
-00003ea0: 6169 6e57 696e 646f 7701 0300 0000 3200  ainWindow.....2.
-00003eb0: 4c00 6f00 6700 7300 2000 7a00 7500 2000  L.o.g.s. .z.u. .
-00003ec0: 4c00 6f00 5400 5700 2000 6800 6f00 6300  L.o.T.W. .h.o.c.
-00003ed0: 6800 6c00 6100 6400 6500 6e00 2e00 2e00  h.l.a.d.e.n.....
-00003ee0: 2e08 0000 0000 0600 0000 1655 706c 6f61  ...........Uploa
-00003ef0: 6420 6c6f 6773 2074 6f20 4c6f 5457 2e2e  d logs to LoTW..
-00003f00: 2e07 0000 000a 4d61 696e 5769 6e64 6f77  ......MainWindow
-00003f10: 0103 0000 0042 0044 0061 0074 0065 0069  .....B.D.a.t.e.i
-00003f20: 0020 0061 0075 0066 0020 006e 0065 0075  . .a.u.f. .n.e.u
-00003f30: 0065 0020 0051 0053 004f 0073 0020 00fc  .e. .Q.S.O.s. ..
-00003f40: 0062 0065 0072 0077 0061 0063 0068 0065  .b.e.r.w.a.c.h.e
-00003f50: 006e 002e 002e 002e 0800 0000 0006 0000  .n..............
-00003f60: 0016 5761 7463 6820 6669 6c65 2066 6f72  ..Watch file for
-00003f70: 2051 534f 732e 2e2e 0700 0000 0a4d 6169   QSOs........Mai
-00003f80: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
-00003f90: 0000 0600 0000 0220 5707 0000 0007 5153  ....... W.....QS
-00003fa0: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00003fb0: 0600 0000 0420 6b48 7a07 0000 0007 5153  ..... kHz.....QS
-00003fc0: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00003fd0: 0600 0000 0235 3907 0000 0007 5153 4f46  .....59.....QSOF
-00003fe0: 6f72 6d01 0300 0000 4800 4500 6900 6e00  orm.....H.E.i.n.
-00003ff0: 2000 4600 6500 6c00 6400 2000 6600 6500   .F.e.l.d. .f.e.
-00004000: 6800 6c00 7400 2000 6600 fc00 7200 2000  h.l.t. .f...r. .
-00004010: 6400 6900 6500 2000 4900 6e00 6200 6f00  d.i.e. .I.n.b.o.
-00004020: 7800 2d00 5000 7200 fc00 6600 7500 6e00  x.-.P.r...f.u.n.
-00004030: 6708 0000 0000 0600 0000 2241 2066 6965  g........."A fie
-00004040: 6c64 2069 7320 6d69 7373 696e 6720 666f  ld is missing fo
-00004050: 7220 696e 626f 7820 6368 6563 6b07 0000  r inbox check...
-00004060: 0007 5153 4f46 6f72 6d01 0300 0000 4200  ..QSOForm.....B.
-00004070: 4600 6500 6800 6c00 6500 6e00 6400 6500  F.e.h.l.e.n.d.e.
-00004080: 7300 2000 4600 6500 6c00 6400 2000 6600  s. .F.e.l.d. .f.
-00004090: fc00 7200 2000 6400 6500 6e00 2000 4c00  ..r. .d.e.n. .L.
-000040a0: 6f00 6700 2d00 5500 7000 6c00 6f00 6100  o.g.-.U.p.l.o.a.
-000040b0: 6408 0000 0000 0600 0000 2141 2066 6965  d.........!A fie
-000040c0: 6c64 2069 7320 6d69 7373 696e 6720 666f  ld is missing fo
-000040d0: 7220 6c6f 6720 7570 6c6f 6164 0700 0000  r log upload....
-000040e0: 0751 534f 466f 726d 0103 0000 0056 0046  .QSOForm.....V.F
-000040f0: 0065 0068 006c 0065 006e 0064 0065 0073  .e.h.l.e.n.d.e.s
-00004100: 0020 0046 0065 006c 0064 0020 0066 00fc  . .F.e.l.d. .f..
-00004110: 0072 0020 0064 0065 006e 0020 004c 006f  .r. .d.e.n. .L.o
-00004120: 0067 002d 0055 0070 006c 006f 0061 0064  .g.-.U.p.l.o.a.d
-00004130: 0020 007a 0075 0020 0048 0061 006d 0051  . .z.u. .H.a.m.Q
-00004140: 0054 0048 0800 0000 0006 0000 002b 4120  .T.H.........+A 
-00004150: 6669 656c 6420 6973 206d 6973 7369 6e67  field is missing
-00004160: 2066 6f72 206c 6f67 2075 706c 6f61 6420   for log upload 
-00004170: 746f 2048 616d 5154 4807 0000 0007 5153  to HamQTH.....QS
-00004180: 4f46 6f72 6d01 0300 0000 1600 4100 6b00  OForm.......A.k.
-00004190: 7a00 6500 7000 7400 6900 6500 7200 7400  z.e.p.t.i.e.r.t.
-000041a0: 3a08 0000 0000 0600 0000 0841 6363 6570  :..........Accep
-000041b0: 7473 3a07 0000 0007 5153 4f46 6f72 6d01  ts:.....QSOForm.
-000041c0: 0300 0000 6a00 4500 6900 6e00 2000 4600  ....j.E.i.n. .F.
-000041d0: 6500 6800 6c00 6500 7200 2000 7400 7200  e.h.l.e.r. .t.r.
-000041e0: 6100 7400 2000 7700 e400 6800 7200 6500  a.t. .w...h.r.e.
-000041f0: 6e00 6400 2000 6400 6500 7200 2000 dc00  n.d. .d.e.r. ...
-00004200: 6200 6500 7200 7400 7200 6100 6700 7500  b.e.r.t.r.a.g.u.
-00004210: 6e00 6700 2000 7a00 7500 2000 4800 6100  n.g. .z.u. .H.a.
-00004220: 6d00 5100 5400 4800 2000 6100 7500 6608  m.Q.T.H. .a.u.f.
-00004230: 0000 0000 0600 0000 2741 6e20 6572 726f  ........'An erro
-00004240: 7220 6f63 6375 7265 6420 6f6e 2075 706c  r occured on upl
-00004250: 6f61 6469 6e67 2074 6f20 4861 6d51 5448  oading to HamQTH
-00004260: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004270: 000e 0041 006e 0074 0065 006e 006e 0065  ...A.n.t.e.n.n.e
-00004280: 0800 0000 0006 0000 0007 416e 7465 6e6e  ..........Antenn
-00004290: 6107 0000 0007 5153 4f46 6f72 6d01 0300  a.....QSOForm...
-000042a0: 0000 1600 4100 7500 7400 6f00 6d00 6100  ....A.u.t.o.m.a.
-000042b0: 7400 6900 7300 6300 6808 0000 0000 0600  t.i.s.c.h.......
-000042c0: 0000 0d41 7574 6f6d 6174 6963 616c 6c79  ...Automatically
-000042d0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-000042e0: 0038 0046 0065 0068 006c 0065 0072 0068  .8.F.e.h.l.e.r.h
-000042f0: 0061 0066 0074 0065 0073 0020 0041 0062  .a.f.t.e.s. .A.b
-00004300: 0066 0072 0061 0067 0065 0065 0072 0067  .f.r.a.g.e.e.r.g
-00004310: 0065 0062 006e 0069 0073 0800 0000 0006  .e.b.n.i.s......
-00004320: 0000 0012 4261 6420 7265 7175 6573 7420  ....Bad request 
-00004330: 7265 7375 6c74 0700 0000 0751 534f 466f  result.....QSOFo
-00004340: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-00004350: 0004 4261 6e64 0700 0000 0751 534f 466f  ..Band.....QSOFo
-00004360: 726d 0103 0000 0008 0042 00fc 0072 006f  rm.......B...r.o
-00004370: 0800 0000 0006 0000 0006 4275 7265 6175  ..........Bureau
-00004380: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004390: 0016 0042 00fc 0072 006f 002f 0044 0069  ...B...r.o./.D.i
-000043a0: 0072 0065 006b 0074 0800 0000 0006 0000  .r.e.k.t........
-000043b0: 000d 4275 7265 6175 2f44 6972 6563 7407  ..Bureau/Direct.
-000043c0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000043d0: 1400 5200 7500 6600 7a00 6500 6900 6300  ..R.u.f.z.e.i.c.
-000043e0: 6800 6500 6e08 0000 0000 0600 0000 0943  h.e.n..........C
-000043f0: 616c 6c20 7369 676e 0700 0000 0751 534f  all sign.....QSO
-00004400: 466f 726d 0103 0000 003c 0046 0065 0068  Form.....<.F.e.h
-00004410: 006c 0065 0072 0020 0062 0065 0069 0020  .l.e.r. .b.e.i. 
-00004420: 0064 0065 0072 0020 0052 0075 0066 007a  .d.e.r. .R.u.f.z
-00004430: 0065 0069 0063 0068 0065 006e 0073 0075  .e.i.c.h.e.n.s.u
-00004440: 0063 0068 0065 0800 0000 0006 0000 0015  .c.h.e..........
-00004450: 4361 6c6c 626f 6f6b 2073 6561 7263 6820  Callbook search 
-00004460: 6572 726f 7207 0000 0007 5153 4f46 6f72  error.....QSOFor
-00004470: 6d01 0300 0000 2a00 4300 6100 6c00 6c00  m.....*.C.a.l.l.
-00004480: 6200 6f00 6f00 6b00 2d00 5300 7500 6300  b.o.o.k.-.S.u.c.
-00004490: 6800 6500 7200 6700 6500 6200 6e00 6900  h.e.r.g.e.b.n.i.
-000044a0: 7308 0000 0000 0600 0000 1643 616c 6c62  s..........Callb
-000044b0: 6f6f 6b20 7365 6172 6368 2072 6573 756c  ook search resul
-000044c0: 7407 0000 0007 5153 4f46 6f72 6d01 0300  t.....QSOForm...
-000044d0: 0000 3200 5200 7500 6600 7a00 6500 6900  ..2.R.u.f.z.e.i.
-000044e0: 6300 6800 6500 6e00 2000 6e00 6900 6300  c.h.e.n. .n.i.c.
-000044f0: 6800 7400 2000 6700 6500 6600 7500 6e00  h.t. .g.e.f.u.n.
-00004500: 6400 6500 6e08 0000 0000 0600 0000 1243  d.e.n..........C
-00004510: 616c 6c73 6967 6e20 6e6f 7420 666f 756e  allsign not foun
-00004520: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
-00004530: 0000 0a00 4b00 6100 6e00 6100 6c08 0000  ....K.a.n.a.l...
-00004540: 0000 0600 0000 0743 6861 6e6e 656c 0700  .......Channel..
-00004550: 0000 0751 534f 466f 726d 0103 0000 0016  ...QSOForm......
-00004560: 0050 0072 00fc 0066 0065 0020 0049 006e  .P.r...f.e. .I.n
-00004570: 0062 006f 0078 0800 0000 0006 0000 000b  .b.o.x..........
-00004580: 4368 6563 6b20 496e 626f 7807 0000 0007  Check Inbox.....
-00004590: 5153 4f46 6f72 6d01 0300 0000 4200 4600  QSOForm.....B.F.
-000045a0: 6500 6800 6c00 6500 7200 2000 6200 6500  e.h.l.e.r. .b.e.
-000045b0: 6900 6d00 2000 5000 7200 fc00 6600 6500  i.m. .P.r...f.e.
-000045c0: 6e00 2000 6400 6500 7200 2000 4c00 6f00  n. .d.e.r. .L.o.
-000045d0: 5400 5700 2d00 4900 6e00 6200 6f00 7808  T.W.-.I.n.b.o.x.
-000045e0: 0000 0000 0600 0000 1643 6865 636b 204c  .........Check L
-000045f0: 6f54 5720 496e 626f 7820 6572 726f 7207  oTW Inbox error.
-00004600: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00004610: 1c00 5000 7200 fc00 6600 6500 2000 4c00  ..P.r...f.e. .L.
-00004620: 6f00 5400 5700 2000 5100 5300 4c08 0000  o.T.W. .Q.S.L...
-00004630: 0000 0600 0000 0e43 6865 636b 204c 6f54  .......Check LoT
-00004640: 5720 5153 4c07 0000 0007 5153 4f46 6f72  W QSL.....QSOFor
-00004650: 6d01 0300 0000 3800 6500 5100 5300 4c00  m.....8.e.Q.S.L.
-00004660: 2d00 4600 6500 6800 6c00 6500 7200 2000  -.F.e.h.l.e.r. .
-00004670: 7000 7200 fc00 6600 6500 6e00 2000 6400  p.r...f.e.n. .d.
-00004680: 6500 7200 2000 4900 6e00 6200 6f00 7808  e.r. .I.n.b.o.x.
-00004690: 0000 0000 0600 0000 1643 6865 636b 2065  .........Check e
-000046a0: 5153 4c20 496e 626f 7820 6572 726f 7207  QSL Inbox error.
-000046b0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000046c0: 1800 5a00 7500 7200 fc00 6300 6b00 7300  ..Z.u.r...c.k.s.
-000046d0: 6500 7400 7a00 6500 6e08 0000 0000 0600  e.t.z.e.n.......
-000046e0: 0000 0543 6c65 6172 0700 0000 0751 534f  ...Clear.....QSO
-000046f0: 466f 726d 0103 0000 0020 004b 006f 006e  Form..... .K.o.n
-00004700: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
-00004710: 0074 0065 0020 0049 0044 0800 0000 0006  .t.e. .I.D......
-00004720: 0000 0013 436f 6e66 6967 7572 6564 2069  ....Configured i
-00004730: 6465 6e74 6974 7907 0000 0007 5153 4f46  dentity.....QSOF
-00004740: 6f72 6d01 0300 0000 2a00 4b00 6f00 6e00  orm.....*.K.o.n.
-00004750: 6600 6900 6700 7500 7200 6900 6500 7200  f.i.g.u.r.i.e.r.
-00004760: 7400 6500 2000 5300 7400 6100 7400 6900  t.e. .S.t.a.t.i.
-00004770: 6f00 6e08 0000 0000 0600 0000 1243 6f6e  o.n..........Con
-00004780: 6669 6775 7265 6420 7374 6174 696f 6e07  figured station.
-00004790: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000047a0: 0c00 6400 6900 7200 6500 6b00 7408 0000  ..d.i.r.e.k.t...
-000047b0: 0000 0600 0000 0644 6972 6563 7407 0000  .......Direct...
-000047c0: 0007 5153 4f46 6f72 6d01 0300 0000 1c00  ..QSOForm.......
-000047d0: 6500 5100 5300 4c00 2000 7300 7000 6500  e.Q.S.L. .s.p.e.
-000047e0: 6900 6300 6800 6500 7200 6e08 0000 0000  i.c.h.e.r.n.....
-000047f0: 0600 0000 0d44 6f77 6e6c 6f61 6420 6551  .....Download eQ
-00004800: 534c 0700 0000 0751 534f 466f 726d 0103  SL.....QSOForm..
-00004810: 0000 006c 0057 00e4 0068 0072 0065 006e  ...l.W...h.r.e.n
-00004820: 0064 0020 0064 0065 0072 0020 0052 0075  .d. .d.e.r. .R.u
-00004830: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
-00004840: 0073 0075 0063 0068 0065 0020 0069 0073  .s.u.c.h.e. .i.s
-00004850: 0074 0020 0065 0069 006e 0020 0046 0065  .t. .e.i.n. .F.e
-00004860: 0068 006c 0065 0072 0020 0061 0075 0066  .h.l.e.r. .a.u.f
-00004870: 0067 0065 0074 0072 0065 0074 0065 006e  .g.e.t.r.e.t.e.n
-00004880: 0800 0000 0006 0000 0027 4475 7269 6e67  .........'During
-00004890: 2063 616c 6c62 6f6f 6b20 7365 6172 6368   callbook search
-000048a0: 2061 6e20 6572 726f 7220 6f63 6375 7265   an error occure
-000048b0: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
-000048c0: 0000 0800 4500 6e00 6400 6508 0000 0000  ....E.n.d.e.....
-000048d0: 0600 0000 0345 6e64 0700 0000 0751 534f  .....End.....QSO
-000048e0: 466f 726d 0103 0000 000c 0046 0065 0068  Form.......F.e.h
-000048f0: 006c 0065 0072 0800 0000 0006 0000 0005  .l.e.r..........
-00004900: 4572 726f 7207 0000 0007 5153 4f46 6f72  Error.....QSOFor
-00004910: 6d01 0300 0000 2400 6500 5100 5300 4c00  m.....$.e.Q.S.L.
-00004920: 2d00 5500 7000 6c00 6f00 6100 6400 2d00  -.U.p.l.o.a.d.-.
-00004930: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-00004940: 0600 0000 0f45 7272 6f72 206f 6e20 7570  .....Error on up
-00004950: 6c6f 6164 0700 0000 0751 534f 466f 726d  load.....QSOForm
-00004960: 0103 0000 0010 0046 0072 0065 0071 0075  .......F.r.e.q.u
-00004970: 0065 006e 007a 0800 0000 0006 0000 0009  .e.n.z..........
-00004980: 4672 6571 7565 6e63 7907 0000 0007 5153  Frequency.....QS
-00004990: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-000049a0: 0600 0000 0648 616d 5154 4807 0000 0007  .....HamQTH.....
-000049b0: 5153 4f46 6f72 6d01 0300 0000 0400 4900  QSOForm.......I.
-000049c0: 4408 0000 0000 0600 0000 0849 6465 6e74  D..........Ident
-000049d0: 6974 7907 0000 0007 5153 4f46 6f72 6d01  ity.....QSOForm.
-000049e0: 0300 0000 2600 4c00 6900 6e00 6b00 2000  ....&.L.i.n.k. .
-000049f0: 7a00 7500 7200 2000 6500 5100 5300 4c00  z.u.r. .e.Q.S.L.
-00004a00: 2d00 4b00 6100 7200 7400 6508 0000 0000  -.K.a.r.t.e.....
-00004a10: 0600 0000 114c 696e 6b20 746f 2065 5153  .....Link to eQS
-00004a20: 4c20 4361 7264 0700 0000 0751 534f 466f  L Card.....QSOFo
-00004a30: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-00004a40: 0004 4c6f 5457 0700 0000 0751 534f 466f  ..LoTW.....QSOFo
-00004a50: 726d 0103 0000 001c 004c 006f 0054 0057  rm.......L.o.T.W
-00004a60: 0020 0065 006d 0070 0066 0061 006e 0067  . .e.m.p.f.a.n.g
-00004a70: 0065 006e 0800 0000 0006 0000 000d 4c6f  .e.n..........Lo
-00004a80: 5457 2072 6563 6569 7665 6407 0000 0007  TW received.....
-00004a90: 5153 4f46 6f72 6d01 0300 0000 1c00 4c00  QSOForm.......L.
-00004aa0: 6f00 5400 5700 2000 7600 6500 7200 7300  o.T.W. .v.e.r.s.
-00004ab0: 6500 6e00 6400 6500 7408 0000 0000 0600  e.n.d.e.t.......
-00004ac0: 0000 094c 6f54 5720 7365 6e74 0700 0000  ...LoTW sent....
-00004ad0: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
-00004ae0: 0000 0006 0000 0007 4c6f 6361 746f 7207  ........Locator.
-00004af0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-00004b00: ff08 0000 0000 0600 0000 074c 6f67 626f  ...........Logbo
-00004b10: 6f6b 0700 0000 0751 534f 466f 726d 0103  ok.....QSOForm..
-00004b20: 0000 0042 004c 006f 0067 0069 006e 0020  ...B.L.o.g.i.n. 
-00004b30: 0066 0065 0068 006c 0067 0065 0073 0063  .f.e.h.l.g.e.s.c
-00004b40: 0068 006c 0061 0067 0065 006e 0020 0066  .h.l.a.g.e.n. .f
-00004b50: 00fc 0072 0020 0042 0065 006e 0075 0074  ...r. .B.e.n.u.t
-00004b60: 007a 0065 0072 0800 0000 0006 0000 0015  .z.e.r..........
-00004b70: 4c6f 6769 6e20 6661 696c 6564 2066 6f72  Login failed for
-00004b80: 2075 7365 7207 0000 0007 5153 4f46 6f72   user.....QSOFor
-00004b90: 6d01 0300 0000 5800 4c00 6f00 6700 6900  m.....X.L.o.g.i.
-00004ba0: 6e00 2000 6200 6500 6900 2000 4800 6100  n. .b.e.i. .H.a.
-00004bb0: 6d00 5100 5400 4800 2000 6600 6500 6800  m.Q.T.H. .f.e.h.
-00004bc0: 6c00 6700 6500 7300 6300 6800 6c00 6100  l.g.e.s.c.h.l.a.
-00004bd0: 6700 6500 6e00 2000 6600 fc00 7200 2000  g.e.n. .f...r. .
-00004be0: 4200 6500 6e00 7500 7400 7a00 6500 7208  B.e.n.u.t.z.e.r.
-00004bf0: 0000 0000 0600 0000 1f4c 6f67 696e 2074  .........Login t
-00004c00: 6f20 4861 6d51 5448 2066 6169 6c65 6420  o HamQTH failed 
-00004c10: 666f 7220 7573 6572 0700 0000 0751 534f  for user.....QSO
-00004c20: 466f 726d 0103 0000 0014 0048 0061 0075  Form.......H.a.u
-00004c30: 0070 0074 0064 0061 0074 0065 006e 0800  .p.t.d.a.t.e.n..
-00004c40: 0000 0006 0000 0009 4d61 696e 2064 6174  ........Main dat
-00004c50: 6107 0000 0007 5153 4f46 6f72 6d01 03ff  a.....QSOForm...
-00004c60: ffff ff08 0000 0000 0600 0000 044d 6f64  .............Mod
-00004c70: 6507 0000 0007 5153 4f46 6f72 6d01 03ff  e.....QSOForm...
-00004c80: ffff ff08 0000 0000 0600 0000 044e 616d  .............Nam
-00004c90: 6507 0000 0007 5153 4f46 6f72 6d01 0300  e.....QSOForm...
-00004ca0: 0000 2400 4b00 6500 6900 6e00 2000 5100  ..$.K.e.i.n. .Q.
-00004cb0: 5300 4c00 2000 7600 6500 7200 6600 fc00  S.L. .v.e.r.f...
-00004cc0: 6700 6200 6100 7208 0000 0000 0600 0000  g.b.a.r.........
-00004cd0: 104e 6f20 5153 4c20 6176 6169 6c61 626c  .No QSL availabl
-00004ce0: 6507 0000 0007 5153 4f46 6f72 6d01 0300  e.....QSOForm...
-00004cf0: 0000 2600 4b00 6500 6900 6e00 2000 6500  ..&.K.e.i.n. .e.
-00004d00: 5100 5300 4c00 2000 7600 6500 7200 6600  Q.S.L. .v.e.r.f.
-00004d10: fc00 6700 6200 6100 7208 0000 0000 0600  ..g.b.a.r.......
-00004d20: 0000 114e 6f20 6551 534c 2061 7661 696c  ...No eQSL avail
-00004d30: 6162 6c65 0700 0000 0751 534f 466f 726d  able.....QSOForm
-00004d40: 0103 0000 000a 004a 0065 0074 007a 0074  .......J.e.t.z.t
-00004d50: 0800 0000 0006 0000 0003 4e6f 7707 0000  ..........Now...
-00004d60: 0007 5153 4f46 6f72 6d01 0300 0000 1600  ..QSOForm.......
-00004d70: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
-00004d80: 5100 5400 4808 0000 0000 0600 0000 074f  Q.T.H..........O
-00004d90: 776e 2051 5448 0700 0000 0751 534f 466f  wn QTH.....QSOFo
-00004da0: 726d 0103 0000 0024 0045 0069 0067 0065  rm.....$.E.i.g.e
-00004db0: 006e 0065 0073 0020 0052 0075 0066 007a  .n.e.s. .R.u.f.z
-00004dc0: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
-00004dd0: 0006 0000 000d 4f77 6e20 6361 6c6c 2073  ......Own call s
-00004de0: 6967 6e07 0000 0007 5153 4f46 6f72 6d01  ign.....QSOForm.
-00004df0: 0300 0000 1e00 4500 6900 6700 6500 6e00  ......E.i.g.e.n.
-00004e00: 6500 7200 2000 4c00 6f00 6300 6100 7400  e.r. .L.o.c.a.t.
-00004e10: 6f00 7208 0000 0000 0600 0000 0b4f 776e  o.r..........Own
-00004e20: 206c 6f63 6174 6f72 0700 0000 0751 534f   locator.....QSO
-00004e30: 466f 726d 0103 0000 0018 0045 0069 0067  Form.......E.i.g
-00004e40: 0065 006e 0065 0072 0020 004e 0061 006d  .e.n.e.r. .N.a.m
-00004e50: 0065 0800 0000 0006 0000 0008 4f77 6e20  .e..........Own 
-00004e60: 6e61 6d65 0700 0000 0751 534f 466f 726d  name.....QSOForm
-00004e70: 0103 0000 001c 0045 0069 0067 0065 006e  .......E.i.g.e.n
-00004e80: 0065 0020 004e 006f 0074 0069 007a 0065  .e. .N.o.t.i.z.e
-00004e90: 006e 0800 0000 0006 0000 0009 4f77 6e20  .n..........Own 
-00004ea0: 6e6f 7465 7307 0000 0007 5153 4f46 6f72  notes.....QSOFor
-00004eb0: 6d01 0300 0000 1000 4c00 6500 6900 7300  m.......L.e.i.s.
-00004ec0: 7400 7500 6e00 6708 0000 0000 0600 0000  t.u.n.g.........
-00004ed0: 0550 6f77 6572 0700 0000 0751 534f 466f  .Power.....QSOFo
-00004ee0: 726d 0103 0000 001e 0041 0075 0073 0062  rm.......A.u.s.b
-00004ef0: 0072 0065 0069 0074 0075 006e 0067 0073  .r.e.i.t.u.n.g.s
-00004f00: 0061 0072 0074 0800 0000 0006 0000 000b  .a.r.t..........
-00004f10: 5072 6f70 6167 6174 696f 6e07 0000 0007  Propagation.....
-00004f20: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
-00004f30: 0000 0600 0000 0551 525a 4351 0700 0000  .......QRZCQ....
-00004f40: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
-00004f50: 0000 0006 0000 0003 5153 4c07 0000 0007  ........QSL.....
-00004f60: 5153 4f46 6f72 6d01 0300 0000 2200 5100  QSOForm.....".Q.
-00004f70: 5300 4c00 2000 2600 2600 2000 4c00 6f00  S.L. .&.&. .L.o.
-00004f80: 6700 2d00 5500 7000 6c00 6f00 6100 6408  g.-.U.p.l.o.a.d.
-00004f90: 0000 0000 0600 0000 1151 534c 2026 2620  .........QSL && 
-00004fa0: 4c6f 6720 7570 6c6f 6164 0700 0000 0751  Log upload.....Q
-00004fb0: 534f 466f 726d 0103 0000 001c 0051 0053  SOForm.......Q.S
-00004fc0: 004c 002d 004b 0061 0072 0074 0065 006e  .L.-.K.a.r.t.e.n
-00004fd0: 0074 0065 0078 0074 0800 0000 0006 0000  .t.e.x.t........
-00004fe0: 0010 5153 4c20 6361 7264 206d 6573 7361  ..QSL card messa
-00004ff0: 6765 0700 0000 0751 534f 466f 726d 0103  ge.....QSOForm..
-00005000: 0000 001a 0051 0053 004c 0020 0065 006d  .....Q.S.L. .e.m
-00005010: 0070 0066 0061 006e 0067 0065 006e 0800  .p.f.a.n.g.e.n..
-00005020: 0000 0006 0000 000c 5153 4c20 7265 6365  ........QSL rece
-00005030: 6976 6564 0700 0000 0751 534f 466f 726d  ived.....QSOForm
-00005040: 0103 0000 0018 0051 0053 004c 0020 0067  .......Q.S.L. .g
-00005050: 0065 0073 0065 006e 0064 0065 0074 0800  .e.s.e.n.d.e.t..
-00005060: 0000 0006 0000 0008 5153 4c20 7365 6e74  ........QSL sent
-00005070: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00005080: 000e 0051 0053 004c 002d 0056 0069 0061  ...Q.S.L.-.V.i.a
-00005090: 0800 0000 0006 0000 0007 5153 4c20 7669  ..........QSL vi
-000050a0: 6107 0000 0007 5153 4f46 6f72 6d01 0300  a.....QSOForm...
-000050b0: 0000 1800 5100 5300 4f00 2d00 4600 6f00  ....Q.S.O.-.F.o.
-000050c0: 7200 6d00 7500 6c00 6100 7208 0000 0000  r.m.u.l.a.r.....
-000050d0: 0600 0000 0851 534f 2046 6f72 6d07 0000  .....QSO Form...
-000050e0: 0007 5153 4f46 6f72 6d01 0300 0000 1a00  ..QSOForm.......
-000050f0: 5100 5300 4f00 2d00 4b00 6f00 6d00 6d00  Q.S.O.-.K.o.m.m.
-00005100: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
-00005110: 0000 0b51 534f 2063 6f6d 6d65 6e74 0700  ...QSO comment..
-00005120: 0000 0751 534f 466f 726d 0103 0000 003e  ...QSOForm.....>
-00005130: 0051 0053 004f 0020 0077 0075 0072 0064  .Q.S.O. .w.u.r.d
-00005140: 0065 0020 0076 006f 006e 0020 0048 0061  .e. .v.o.n. .H.a
-00005150: 006d 0051 0054 0048 0020 0061 0062 0067  .m.Q.T.H. .a.b.g
-00005160: 0065 0077 0069 0065 0073 0065 006e 0800  .e.w.i.e.s.e.n..
-00005170: 0000 0006 0000 0016 5153 4f20 7265 6a65  ........QSO reje
-00005180: 6374 6564 206f 6e20 4861 6d51 5448 0700  cted on HamQTH..
-00005190: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-000051a0: 0800 0000 0006 0000 0003 5154 4807 0000  ..........QTH...
-000051b0: 0007 5153 4f46 6f72 6d01 03ff ffff ff08  ..QSOForm.......
-000051c0: 0000 0000 0600 0000 0652 5354 2052 7807  .........RST Rx.
-000051d0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-000051e0: ff08 0000 0000 0600 0000 0652 5354 2054  ...........RST T
-000051f0: 7807 0000 0007 5153 4f46 6f72 6d01 0300  x.....QSOForm...
-00005200: 0000 1a00 5200 5300 5400 2000 6500 6d00  ....R.S.T. .e.m.
-00005210: 7000 6600 6100 6e00 6700 6500 6e08 0000  p.f.a.n.g.e.n...
-00005220: 0000 0600 0000 0c52 5354 2072 6563 6569  .......RST recei
-00005230: 7665 6407 0000 0007 5153 4f46 6f72 6d01  ved.....QSOForm.
-00005240: 0300 0000 1800 5200 5300 5400 2000 6700  ......R.S.T. .g.
-00005250: 6500 7300 6500 6e00 6400 6500 7408 0000  e.s.e.n.d.e.t...
-00005260: 0000 0600 0000 0852 5354 2073 656e 7407  .......RST sent.
-00005270: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-00005280: ff08 0000 0000 0600 0000 0552 6164 696f  ...........Radio
-00005290: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-000052a0: 0012 0053 0070 0065 0069 0063 0068 0065  ...S.p.e.i.c.h.e
-000052b0: 0072 006e 0800 0000 0006 0000 0004 5361  .r.n..........Sa
-000052c0: 7665 0700 0000 0751 534f 466f 726d 0103  ve.....QSOForm..
-000052d0: 0000 0026 0053 0070 0065 0069 0063 0068  ...&.S.p.e.i.c.h
-000052e0: 0065 0072 006e 0020 0026 0026 0020 0055  .e.r.n. .&.&. .U
-000052f0: 0070 006c 006f 0061 0064 0800 0000 0006  .p.l.o.a.d......
-00005300: 0000 000e 5361 7665 2026 2620 5570 6c6f  ....Save && Uplo
-00005310: 6164 0700 0000 0751 534f 466f 726d 0103  ad.....QSOForm..
-00005320: 0000 002a 0065 0051 0053 004c 002d 004f  ...*.e.Q.S.L.-.O
-00005330: 0072 0064 006e 0065 0072 0020 0061 0075  .r.d.n.e.r. .a.u
-00005340: 0073 0077 00e4 0068 006c 0065 006e 0800  .s.w...h.l.e.n..
-00005350: 0000 0006 0000 0012 5365 6c65 6374 2065  ........Select e
-00005360: 5153 4c20 666f 6c64 6572 0700 0000 0751  QSL folder.....Q
-00005370: 534f 466f 726d 0103 0000 0036 0053 0065  SOForm.....6.S.e
-00005380: 0072 0076 0065 0072 006b 006f 006d 006d  .r.v.e.r.k.o.m.m
-00005390: 0075 006e 0069 006b 0061 0074 0069 006f  .u.n.i.k.a.t.i.o
-000053a0: 006e 0073 002d 0046 0065 0068 006c 0065  .n.s.-.F.e.h.l.e
-000053b0: 0072 0800 0000 0006 0000 001a 5365 7276  .r..........Serv
-000053c0: 6572 2063 6f6d 6d75 6e69 6361 7469 6f6e  er communication
-000053d0: 2065 7272 6f72 0700 0000 0751 534f 466f   error.....QSOFo
-000053e0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-000053f0: 0005 5374 6172 7407 0000 0007 5153 4f46  ..Start.....QSOF
-00005400: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
-00005410: 0000 0753 7461 7469 6f6e 0700 0000 0751  ...Station.....Q
-00005420: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
-00005430: 0006 0000 0007 5375 626d 6f64 6507 0000  ......Submode...
-00005440: 0007 5153 4f46 6f72 6d01 0300 0000 3000  ..QSOForm.....0.
-00005450: 4400 6100 7300 2000 5100 5300 4f00 2000  D.a.s. .Q.S.O. .
-00005460: 6900 7300 7400 2000 6500 6900 6e00 2000  i.s.t. .e.i.n. .
-00005470: 4400 7500 7000 6c00 6900 6b00 6100 7408  D.u.p.l.i.k.a.t.
-00005480: 0000 0000 0600 0000 1654 6865 2051 534f  .........The QSO
-00005490: 2069 7320 6120 6475 706c 6963 6174 6507   is a duplicate.
-000054a0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000054b0: b800 4400 6900 6500 2000 5100 5300 4c00  ..D.i.e. .Q.S.L.
-000054c0: 2d00 5200 6f00 7500 7400 6500 2000 6400  -.R.o.u.t.e. .d.
-000054d0: 6500 7200 2000 6b00 6f00 6e00 7400 6100  e.r. .k.o.n.t.a.
-000054e0: 6b00 7400 6900 6500 7200 7400 6500 6e00  k.t.i.e.r.t.e.n.
-000054f0: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
-00005500: 2e00 0a00 4400 6900 6500 7300 2000 6900  ....D.i.e.s. .i.
-00005510: 7300 7400 2000 6e00 6900 6300 6800 7400  s.t. .n.i.c.h.t.
-00005520: 2000 6400 6900 6500 2000 4100 6400 7200   .d.i.e. .A.d.r.
-00005530: 6500 7300 7300 6500 2000 6400 6500 7300  e.s.s.e. .d.e.s.
-00005540: 2000 5100 5300 4c00 2d00 4d00 6100 6e00   .Q.S.L.-.M.a.n.
-00005550: 6100 6700 6500 7200 7300 2f00 2d00 4200  a.g.e.r.s./.-.B.
-00005560: fc00 7200 6f00 7300 2e08 0000 0000 0600  ..r.o.s.........
-00005570: 0000 4c54 6865 2063 6f6e 7461 6374 6564  ..LThe contacted
-00005580: 2073 7461 7469 6f6e 2051 534c 2072 6f75   station QSL rou
-00005590: 7465 2e0a 5468 6973 2069 7320 6e6f 7420  te..This is not 
-000055a0: 7468 6520 5153 4c20 6d61 6e61 6765 722f  the QSL manager/
-000055b0: 6275 7265 6175 2061 6464 7265 7373 2e07  bureau address..
-000055c0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-000055d0: 1000 4500 6e00 6400 6500 7a00 6500 6900  ..E.n.d.e.z.e.i.
-000055e0: 7408 0000 0000 0600 0000 0854 696d 6520  t..........Time 
-000055f0: 656e 6407 0000 0007 5153 4f46 6f72 6d01  end.....QSOForm.
-00005600: 0300 0000 1200 5300 7400 6100 7200 7400  ......S.t.a.r.t.
-00005610: 7a00 6500 6900 7408 0000 0000 0600 0000  z.e.i.t.........
-00005620: 0a54 696d 6520 7374 6172 7407 0000 0007  .Time start.....
-00005630: 5153 4f46 6f72 6d01 0300 0000 2400 6500  QSOForm.....$.e.
-00005640: 5100 5300 4c00 2d00 5500 7000 6c00 6f00  Q.S.L.-.U.p.l.o.
-00005650: 6100 6400 2d00 4600 6500 6800 6c00 6500  a.d.-.F.e.h.l.e.
-00005660: 7208 0000 0000 0600 0000 1155 706c 6f61  r..........Uploa
-00005670: 6420 6551 534c 2065 7272 6f72 0700 0000  d eQSL error....
-00005680: 0751 534f 466f 726d 0103 0000 001a 0055  .QSOForm.......U
-00005690: 0070 006c 006f 0061 0064 002d 0046 0065  .p.l.o.a.d.-.F.e
-000056a0: 0068 006c 0065 0072 0800 0000 0006 0000  .h.l.e.r........
-000056b0: 0010 5570 6c6f 6164 206c 6f67 2065 7272  ..Upload log err
-000056c0: 6f72 0700 0000 0751 534f 466f 726d 0103  or.....QSOForm..
-000056d0: 0000 0068 0055 0070 006c 006f 0061 0064  ...h.U.p.l.o.a.d
-000056e0: 0020 0065 0072 0066 006f 006c 0067 0074  . .e.r.f.o.l.g.t
-000056f0: 0020 006e 0075 0072 0020 0077 0065 006e  . .n.u.r. .w.e.n
-00005700: 006e 0020 0061 0075 0066 0020 0064 0065  .n. .a.u.f. .d.e
-00005710: 0072 0020 0051 0053 004c 002d 0053 0065  .r. .Q.S.L.-.S.e
-00005720: 0069 0074 0065 0020 0061 0075 0073 0067  .i.t.e. .a.u.s.g
-00005730: 0065 0077 00e4 0068 006c 0074 0800 0000  .e.w...h.l.t....
-00005740: 0006 0000 0024 5570 6c6f 6164 7320 6f6e  .....$Uploads on
-00005750: 6c79 2069 6620 7365 6c65 6374 6564 206f  ly if selected o
-00005760: 6e20 5153 4c20 7061 6765 0700 0000 0751  n QSL page.....Q
-00005770: 534f 466f 726d 0103 0000 0048 0044 0065  SOForm.....H.D.e
-00005780: 0072 0020 004e 0075 0074 007a 0065 0072  .r. .N.u.t.z.e.r
-00005790: 0020 0043 0061 006c 006c 0020 0073 0074  . .C.a.l.l. .s.t
-000057a0: 0069 006d 006d 0074 0020 006e 0069 0063  .i.m.m.t. .n.i.c
-000057b0: 0068 0074 0020 00fc 0062 0065 0072 0065  .h.t. ...b.e.r.e
-000057c0: 0069 006e 0800 0000 0006 0000 0018 5573  .i.n..........Us
-000057d0: 6572 2063 616c 6c20 646f 6573 206e 6f74  er call does not
-000057e0: 206d 6174 6368 0700 0000 0751 534f 466f   match.....QSOFo
-000057f0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-00005800: 0004 6551 534c 0700 0000 0751 534f 466f  ..eQSL.....QSOFo
-00005810: 726d 0103 0000 001c 0065 0051 0053 004c  rm.......e.Q.S.L
-00005820: 0020 0065 006d 0070 0066 0061 006e 0067  . .e.m.p.f.a.n.g
-00005830: 0065 006e 0800 0000 0006 0000 000d 6551  .e.n..........eQ
-00005840: 534c 2072 6563 6569 7665 6407 0000 0007  SL received.....
-00005850: 5153 4f46 6f72 6d01 0300 0000 1a00 6500  QSOForm.......e.
-00005860: 5100 5300 4c00 2000 6700 6500 7300 6500  Q.S.L. .g.e.s.e.
-00005870: 6e00 6400 6500 7408 0000 0000 0600 0000  n.d.e.t.........
-00005880: 0965 5153 4c20 7365 6e74 0700 0000 0751  .eQSL sent.....Q
-00005890: 534f 466f 726d 0103 0000 0008 006b 002e  SOForm.......k..
-000058a0: 0041 002e 0800 0000 0006 0000 0004 6e2e  .A............n.
-000058b0: 612e 0700 0000 0751 534f 466f 726d 0103  a......QSOForm..
-000058c0: 0000 0034 0072 0069 0067 0063 0074 006c  ...4.r.i.g.c.t.l
-000058d0: 0064 0020 005a 0065 0069 0074 00fc 0062  .d. .Z.e.i.t...b
-000058e0: 0065 0072 0073 0063 0068 0072 0065 0069  .e.r.s.c.h.r.e.i
-000058f0: 0074 0075 006e 0067 0800 0000 0006 0000  .t.u.n.g........
-00005900: 000f 7269 6763 746c 6420 7469 6d65 6f75  ..rigctld timeou
-00005910: 7407 0000 0007 5153 4f46 6f72 6d01 03ff  t.....QSOForm...
-00005920: ffff ff08 0000 0000 0600 0000 0a79 7979  .............yyy
-00005930: 792d 4d4d 2d64 6407 0000 0007 5153 4f46  y-MM-dd.....QSOF
-00005940: 6f72 6d01 0300 0000 7a00 4300 4100 5400  orm.....z.C.A.T.
-00005950: 2d00 4500 6900 6e00 7300 7400 6500 6c00  -.E.i.n.s.t.e.l.
-00005960: 6c00 7500 6e00 6700 2000 7700 7500 7200  l.u.n.g. .w.u.r.
-00005970: 6400 2000 6e00 6f00 6300 6800 2000 6e00  d. .n.o.c.h. .n.
-00005980: 6900 6500 2000 6700 6500 7300 7000 6500  i.e. .g.e.s.p.e.
-00005990: 6900 6300 6800 6500 7200 7400 2000 6f00  i.c.h.e.r.t. .o.
-000059a0: 7200 2000 5000 6100 7200 6100 6d00 6500  r. .P.a.r.a.m.e.
-000059b0: 7400 6500 7200 2000 6600 6500 6800 6c00  t.e.r. .f.e.h.l.
-000059c0: 6500 6e08 0000 0000 0600 0000 3b43 4154  e.n.........;CAT
-000059d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2077   configuration w
-000059e0: 6173 206e 6576 6572 2073 6176 6564 206f  as never saved o
-000059f0: 7220 6120 7061 7261 6d65 7465 7220 6973  r a parameter is
-00005a00: 206d 6973 7369 6e67 0700 0000 0853 6574   missing.....Set
-00005a10: 7469 6e67 7301 0300 0000 3000 4300 4100  tings.....0.C.A.
-00005a20: 5400 2d00 4500 6900 6e00 7300 7400 6500  T.-.E.i.n.s.t.e.
-00005a30: 6c00 6c00 7500 6e00 6700 6500 6e00 2000  l.l.u.n.g.e.n. .
-00005a40: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-00005a50: 0600 0000 1243 4154 2073 6574 7469 6e67  .....CAT setting
-00005a60: 7320 6572 726f 7207 0000 0008 5365 7474  s error.....Sett
-00005a70: 696e 6773 0103 0000 002a 0048 0061 006d  ings.....*.H.a.m
-00005a80: 006c 0069 0062 0020 0072 0069 0067 0063  .l.i.b. .r.i.g.c
-00005a90: 0074 006c 0064 0020 0077 00e4 0068 006c  .t.l.d. .w...h.l
-00005aa0: 0065 006e 0800 0000 0006 0000 0020 4368  .e.n......... Ch
-00005ab0: 6f6f 7365 2068 616d 6c69 6220 7269 6763  oose hamlib rigc
-00005ac0: 746c 6420 6578 6563 7574 6162 6c65 0700  tld executable..
-00005ad0: 0000 0853 6574 7469 6e67 7301 0300 0000  ...Settings.....
-00005ae0: 2000 4400 6100 7400 7500 6d00 2f00 5a00   .D.a.t.u.m./.Z.
-00005af0: 6500 6900 7400 2000 5300 7400 6100 7200  e.i.t. .S.t.a.r.
-00005b00: 7408 0000 0000 0600 0000 0f44 6174 652f  t..........Date/
-00005b10: 5469 6d65 2073 7461 7274 0700 0000 0853  Time start.....S
-00005b20: 6574 7469 6e67 7301 0300 0000 4200 4600  ettings.....B.F.
-00005b30: 6500 6800 6c00 6500 7200 2000 6200 6500  e.h.l.e.r. .b.e.
-00005b40: 6900 6d00 2000 4100 7500 7300 6600 fc00  i.m. .A.u.s.f...
-00005b50: 6800 7200 6500 6e00 2000 7600 6f00 6e00  h.r.e.n. .v.o.n.
-00005b60: 2000 7200 6900 6700 6300 7400 6c00 6408   .r.i.g.c.t.l.d.
-00005b70: 0000 0000 0600 0000 1745 7272 6f72 2065  .........Error e
-00005b80: 7865 6375 7469 6e67 2072 6967 6374 6c64  xecuting rigctld
-00005b90: 0700 0000 0853 6574 7469 6e67 7301 03ff  .....Settings...
-00005ba0: ffff ff08 0000 0000 0600 0000 0648 616d  .............Ham
-00005bb0: 6c69 6207 0000 0008 5365 7474 696e 6773  lib.....Settings
-00005bc0: 0103 0000 004e 0044 0069 0065 0020 0067  .....N.D.i.e. .g
-00005bd0: 0065 0077 00e4 0068 006c 0074 0065 0020  .e.w...h.l.t.e. 
-00005be0: 0044 0061 0074 0065 0069 0020 0069 0073  .D.a.t.e.i. .i.s
-00005bf0: 0074 0020 006e 0069 0063 0068 0074 0020  .t. .n.i.c.h.t. 
-00005c00: 0061 0075 0073 0066 00fc 0068 0072 0062  .a.u.s.f...h.r.b
-00005c10: 0061 0072 0800 0000 0006 0000 0023 5365  .a.r.........#Se
-00005c20: 6c65 6374 6564 2066 696c 6520 6973 206e  lected file is n
-00005c30: 6f74 2074 6865 2065 7865 6375 7461 626c  ot the executabl
-00005c40: 6507 0000 0008 5365 7474 696e 6773 0103  e.....Settings..
-00005c50: 0000 0014 007a 0065 0069 0067 0065 0020  .....z.e.i.g.e. 
-00005c60: 0061 006c 006c 0065 0800 0000 0006 0000  .a.l.l.e........
-00005c70: 0008 5368 6f77 2061 6c6c 0700 0000 0853  ..Show all.....S
-00005c80: 6574 7469 6e67 7301 03ff ffff ff08 0000  ettings.........
-00005c90: 0000 0600 0000 0553 7461 7274 0700 0000  .......Start....
-00005ca0: 0853 6574 7469 6e67 7301 0300 0000 1a00  .Settings.......
-00005cb0: 5300 7400 6100 7200 7400 6500 2000 4800  S.t.a.r.t.e. .H.
-00005cc0: 6100 6d00 6c00 6900 6208 0000 0000 0600  a.m.l.i.b.......
-00005cd0: 0000 0c53 7461 7274 2068 616d 6c69 6207  ...Start hamlib.
-00005ce0: 0000 0008 5365 7474 696e 6773 0103 ffff  ....Settings....
-00005cf0: ffff 0800 0000 0006 0000 0004 5374 6f70  ............Stop
-00005d00: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
-00005d10: 0000 1a00 5300 7400 6f00 7000 7000 6500  ....S.t.o.p.p.e.
-00005d20: 2000 4800 6100 6d00 6c00 6900 6208 0000   .H.a.m.l.i.b...
-00005d30: 0000 0600 0000 0b53 746f 7020 6861 6d6c  .......Stop haml
-00005d40: 6962 0700 0000 0853 6574 7469 6e67 7301  ib.....Settings.
-00005d50: 0300 0000 0a00 6100 6b00 7400 6900 7608  ......a.k.t.i.v.
-00005d60: 0000 0000 0600 0000 0561 6374 6976 0700  .........activ..
-00005d70: 0000 0853 6574 7469 6e67 7301 0300 0000  ...Settings.....
-00005d80: 0e00 6900 6e00 6100 6b00 7400 6900 7608  ..i.n.a.k.t.i.v.
-00005d90: 0000 0000 0600 0000 0769 6e61 6374 6976  .........inactiv
-00005da0: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
-00005db0: 0000 4a00 7200 6900 6700 6300 7400 6c00  ..J.r.i.g.c.t.l.
-00005dc0: 6400 2000 6b00 6f00 6e00 6e00 7400 6500  d. .k.o.n.n.t.e.
-00005dd0: 2000 6e00 6900 6300 6800 7400 2000 6700   .n.i.c.h.t. .g.
-00005de0: 6500 7300 7400 6100 7200 7400 6500 7400  e.s.t.a.r.t.e.t.
-00005df0: 2000 7700 6500 7200 6400 6500 6e08 0000   .w.e.r.d.e.n...
-00005e00: 0000 0600 0000 1e72 6967 6374 6c64 2064  .......rigctld d
-00005e10: 6964 206e 6f74 2073 7461 7274 2070 726f  id not start pro
-00005e20: 7065 726c 7907 0000 0008 5365 7474 696e  perly.....Settin
-00005e30: 6773 0103 0000 0010 0067 0065 00e4 006e  gs.......g.e...n
-00005e40: 0064 0065 0072 0074 0800 0000 0006 0000  .d.e.r.t........
-00005e50: 0001 4d07 0000 0014 5472 616e 736c 6174  ..M.....Translat
-00005e60: 6564 5461 626c 654d 6f64 656c 0103 0000  edTableModel....
-00005e70: 0008 004e 0065 0069 006e 0800 0000 0006  ...N.e.i.n......
-00005e80: 0000 0001 4e07 0000 0014 5472 616e 736c  ....N.....Transl
-00005e90: 6174 6564 5461 626c 654d 6f64 656c 0103  atedTableModel..
-00005ea0: 0000 0012 0061 006e 0067 0065 0066 0072  .....a.n.g.e.f.r
-00005eb0: 0061 0067 0074 0800 0000 0006 0000 0001  .a.g.t..........
-00005ec0: 5207 0000 0014 5472 616e 736c 6174 6564  R.....Translated
-00005ed0: 5461 626c 654d 6f64 656c 0103 0000 0004  TableModel......
-00005ee0: 004a 0061 0800 0000 0006 0000 0001 5907  .J.a..........Y.
-00005ef0: 0000 0014 5472 616e 736c 6174 6564 5461  ....TranslatedTa
-00005f00: 626c 654d 6f64 656c 0103 ffff ffff 0800  bleModel........
-00005f10: 0000 0006 0000 0007 4a53 3843 616c 6c07  ........JS8Call.
-00005f20: 0000 000f 6170 7053 656c 6563 7444 6961  ....appSelectDia
-00005f30: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00005f40: 0000 054f 7468 6572 0700 0000 0f61 7070  ...Other.....app
-00005f50: 5365 6c65 6374 4469 616c 6f67 0103 0000  SelectDialog....
-00005f60: 002a 0041 0075 0073 0077 0061 0068 006c  .*.A.u.s.w.a.h.l
-00005f70: 0020 0064 0065 0073 0020 0050 0072 006f  . .d.e.s. .P.r.o
-00005f80: 0067 0072 0061 006d 006d 0073 0800 0000  .g.r.a.m.m.s....
-00005f90: 0006 0000 0016 5365 6c65 6374 2074 6865  ......Select the
-00005fa0: 2061 7070 6c69 6361 7469 6f6e 0700 0000   application....
-00005fb0: 0f61 7070 5365 6c65 6374 4469 616c 6f67  .appSelectDialog
-00005fc0: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
-00005fd0: 5753 4a54 2d58 0700 0000 0f61 7070 5365  WSJT-X.....appSe
-00005fe0: 6c65 6374 4469 616c 6f67 0103 ffff ffff  lectDialog......
-00005ff0: 0800 0000 0006 0000 0006 666c 6469 6769  ..........fldigi
-00006000: 0700 0000 0f61 7070 5365 6c65 6374 4469  .....appSelectDi
-00006010: 616c 6f67 0188 0000 0002 0101            alog........
+00000500: 8ed0 0500 0054 1f05 c7f7 2800 0056 1805  .....T....(..V..
+00000510: c984 e900 0030 a106 011e c400 0002 9c06  .....0..........
+00000520: 778d 0800 0006 cf06 778d 0800 001f 2106  w.......w.....!.
+00000530: 7e7c a100 0026 2306 7e7c a100 0046 6906  ~|...&#.~|...Fi.
+00000540: 830d be00 0029 f106 bdf0 a400 0019 8f06  .....)..........
+00000550: be94 d200 0052 fa06 d2af d900 0056 4206  .....R.......VB.
+00000560: db4d 4200 0027 f206 e056 d800 0024 3e06  .MB..'...V...$>.
+00000570: e056 d800 0043 5606 f895 8e00 0015 f507  .V...CV.........
+00000580: 2f4a 1500 004a 3607 366b 9300 0005 1a07  /J...J6.6k......
+00000590: 50be 3900 0053 9a07 68f8 4400 004e ab07  P.9..S..h.D..N..
+000005a0: 693d fe00 0031 a307 6941 4e00 0032 6607  i=...1..iAN..2f.
+000005b0: 6cbb 6300 000e 7707 7f18 a400 004b ec07  l.c...w......K..
+000005c0: 86be 4800 0036 d507 8f3a 3e00 0024 fb07  ..H..6...:>..$..
+000005d0: 8f3a 3e00 0044 cf07 e67a d700 0030 ee07  .:>..D...z...0..
+000005e0: e76d c800 0025 7d07 e78f a400 0025 b307  .m...%}......%..
+000005f0: e79f 3400 0025 eb07 e79f 3400 0046 2d07  ..4..%....4..F-.
+00000600: e7e0 a400 002e 4207 e7f2 3400 002e 7d07  ......B...4...}.
+00000610: e7f2 3400 004e 4408 14d3 ed00 0032 eb08  ..4..ND......2..
+00000620: 14d3 ed00 0046 9a08 3292 cb00 0002 7908  .....F..2.....y.
+00000630: 3587 6a00 002b a608 36b6 5400 0012 8a08  5.j..+..6.T.....
+00000640: 5ac5 0100 0001 9408 5ac5 0100 0014 2c08  Z.......Z.....,.
+00000650: 5ac5 0100 0038 5908 678f b400 0027 1f08  Z....8Y.g....'..
+00000660: 679f 2400 0027 5708 679f 2400 0048 2c08  g.$..'W.g.$..H,.
+00000670: 7f52 2500 002a e608 8879 1400 0019 2108  .R%..*...y....!.
+00000680: aae3 e400 0009 9c08 b63d de00 0034 fd08  .........=...4..
+00000690: bd74 5e00 0022 ff08 d39b 6400 0040 3f08  .t^.."....d..@?.
+000006a0: f89a cb00 0035 d009 14be 9200 0049 6309  .....5.......Ic.
+000006b0: 1c52 9500 002d f709 238c 7500 0016 f209  .R...-..#.u.....
+000006c0: 3f8c ad00 000c da09 564e 4200 004c 2409  ?.......VNB..L$.
+000006d0: 6c61 f400 0013 aa09 6c61 f400 002f 1709  la......la.../..
+000006e0: 6fe6 7e00 0011 8e09 8fa3 8700 002f 4c09  o.~........../L.
+000006f0: 97c9 1400 0020 b309 97c9 1400 0040 8409  ..... .......@..
+00000700: 97d9 8400 0020 7809 9c7f 1a00 0037 7209  ..... x......7r.
+00000710: a118 8500 0011 0d09 c004 d700 0003 df09  ................
+00000720: c4e8 d700 0001 c409 c8df a200 001e 9409  ................
+00000730: c943 f500 0010 0709 c9cf c500 000c 2f09  .C............/.
+00000740: df31 3800 0047 1709 e854 fc00 0015 c609  .18..G...T......
+00000750: e854 fc00 003b 1a09 f42c fb00 001b 7e0a  .T...;...,....~.
+00000760: 16bb 3400 0046 d60a 2087 bc00 003b f80a  ..4..F.. ....;..
+00000770: 2190 e200 0006 860a 2190 e200 001e d50a  !.......!.......
+00000780: 3f0e 9500 0028 ea0a 5e68 d900 0026 770a  ?....(..^h...&w.
+00000790: 643c 1400 0016 bb0a 6789 3b00 0007 0e0a  d<......g.;.....
+000007a0: 6789 3b00 001f 630a 67a9 0200 0007 4a0a  g.;...c.g.....J.
+000007b0: 67a9 0200 001f a20a 6dc8 3e00 0034 960a  g.......m.>..4..
+000007c0: 7833 e400 0039 790a 7d6b 2400 0018 550a  x3...9y.}k$...U.
+000007d0: 92a2 e500 0029 9d0a 9612 e500 0028 900a  .....).......(..
+000007e0: a8b0 0e00 000e 360a a8b0 0e00 0049 f00a  ......6......I..
+000007f0: acdb 7e00 0002 1c0a b945 f500 002b 220a  ..~......E...+".
+00000800: b945 f500 004a 130a c389 2500 0028 590a  .E...J....%..(Y.
+00000810: c5b4 4900 003f a40a c897 c500 0006 480a  ..I..?........H.
+00000820: d2f0 b500 0003 090a d382 7700 0003 570a  ..........w...W.
+00000830: e2b5 9600 0004 b50a f31c 2200 003b 840b  .........."..;..
+00000840: 1562 0700 004f 300b 1805 3900 0015 3b0b  .b...O0...9...;.
+00000850: 4597 5500 0008 1b0b 5d8a f400 001f e10b  E.U.....].......
+00000860: 6628 d200 0034 540b 7fe2 de00 0033 2a0b  f(...4T......3*.
+00000870: ad17 7800 001b 500b ff25 ce00 001c 7e0c  ..x...P..%....~.
+00000880: 08f5 6c00 003d b60c 107d 9300 0003 a10c  ..l..=...}......
+00000890: 10ba b200 0027 b00c 1536 f700 002d 190c  .....'...6...-..
+000008a0: 1f2f 0200 004c 750c 29f2 a400 004f 0a0c  ./...Lu.)....O..
+000008b0: 6a19 e900 003c e10c 8c09 2900 001d 350c  j....<....)...5.
+000008c0: 8c09 2900 003f 4d0c 9688 9500 0014 830c  ..)..?M.........
+000008d0: a3fa 5f00 001a 250c a6e8 d400 003a 5e0c  .._...%......:^.
+000008e0: bb01 7300 000c 9d0c bb01 7300 0033 810c  ..s.......s..3..
+000008f0: c9a0 0e00 002d 730d 0218 6400 0048 bb0d  .....-s...d..H..
+00000900: 07a4 f800 003b 470d 1f27 b200 0014 d70d  .....;G..'......
+00000910: 3504 b400 003a ba0d 76f7 5900 001b d30d  5....:..v.Y.....
+00000920: 825f 7300 000f 1a0d a03c 1200 0050 020d  ._s......<...P..
+00000930: d0ff 4c00 002c cd0d f2ea c200 003c 3e0d  ..L..,.......<>.
+00000940: fe4e 2400 0019 d80d fe4e 2400 0050 c80e  .N$......N$..P..
+00000950: 0543 5500 0024 000e 05d1 b500 0050 610e  .CU..$.......Pa.
+00000960: 0743 5500 0044 210e 0906 8800 0037 ac0e  .CU..D!......7..
+00000970: 233d d500 004c bb0e 87ac 6400 0020 2a0e  #=...L....d.. *.
+00000980: 93fa 5200 0017 970e a32f e400 003e fe0e  ..R....../...>..
+00000990: c497 a200 000b 3e0e c72a a600 0005 820e  ......>..*......
+000009a0: de3d a200 0039 f10e e46b 3400 0047 ea0e  .=...9...k4..G..
+000009b0: fdeb 3400 0045 eb0f 165e c400 0045 540f  ..4..E...^...ET.
+000009c0: 3562 ce00 0017 f80f 6963 bc00 000d 1f0f  5b......ic......
+000009d0: 6963 bc00 002a ac0f 6963 bc00 0052 3b0f  ic...*..ic...R;.
+000009e0: 6978 c700 0033 c20f 6c98 6c00 0055 600f  ix...3..l.l..U`.
+000009f0: 7ddd 2800 004d 630f 8007 d400 0038 c90f  }.(..Mc......8..
+00000a00: 8313 8900 0013 130f cb15 5200 0018 d70f  ..........R.....
+00000a10: e6f6 3400 003f cc69 0000 566c 03ff ffff  ..4..?.i..Vl....
+00000a20: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
+00000a30: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000a40: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
+00000a50: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000a60: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
+00000a70: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000a80: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
+00000a90: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000aa0: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
+00000ab0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000ac0: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
+00000ad0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000ae0: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
+00000af0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000b00: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
+00000b10: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000b20: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
+00000b30: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000b40: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
+00000b50: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000b60: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
+00000b70: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000b80: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
+00000b90: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00000ba0: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
+00000bb0: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
+00000bc0: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
+00000bd0: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
+00000be0: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
+00000bf0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
+00000c00: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
+00000c10: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000c20: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
+00000c30: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000c40: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
+00000c50: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
+00000c60: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
+00000c70: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
+00000c80: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
+00000c90: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
+00000ca0: 0000 0008 4361 6c6c 626f 6f6b 0700 0000  ....Callbook....
+00000cb0: 0644 6961 6c6f 6701 0300 0000 3800 5a00  .Dialog.....8.Z.
+00000cc0: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
+00000cd0: 7400 2000 6200 6500 6e00 f600 7400 6900  t. .b.e.n...t.i.
+00000ce0: 6700 7400 2000 5000 6100 7300 7300 7700  g.t. .P.a.s.s.w.
+00000cf0: 6f00 7200 7408 0000 0000 0600 0000 1a43  o.r.t..........C
+00000d00: 6572 7469 6669 6361 7465 206e 6565 6473  ertificate needs
+00000d10: 2070 6173 7377 6f72 6407 0000 0006 4469   password.....Di
+00000d20: 616c 6f67 0103 0000 0024 0053 0070 0061  alog.....$.S.p.a
+00000d30: 006c 0074 0065 006e 0020 0076 0065 0072  .l.t.e.n. .v.e.r
+00000d40: 0073 0074 0065 0063 006b 0065 006e 0800  .s.t.e.c.k.e.n..
+00000d50: 0000 0006 0000 000f 436f 6c75 6d6e 7320  ........Columns 
+00000d60: 746f 2068 6964 6507 0000 0006 4469 616c  to hide.....Dial
+00000d70: 6f67 0103 0000 0020 0053 0070 0061 006c  og..... .S.p.a.l
+00000d80: 0074 0065 006e 0020 0061 006e 007a 0065  .t.e.n. .a.n.z.e
+00000d90: 0069 0067 0065 006e 0800 0000 0006 0000  .i.g.e.n........
+00000da0: 000f 436f 6c75 6d6e 7320 746f 2073 686f  ..Columns to sho
+00000db0: 7707 0000 0006 4469 616c 6f67 0103 0000  w.....Dialog....
+00000dc0: 0018 0041 006e 006d 0065 006c 0064 0065  ...A.n.m.e.l.d.e
+00000dd0: 0064 0061 0074 0065 006e 0800 0000 0006  .d.a.t.e.n......
+00000de0: 0000 000b 4372 6564 656e 7469 616c 7307  ....Credentials.
+00000df0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
+00000e00: 0041 0062 0073 0074 0065 0069 0067 0065  .A.b.s.t.e.i.g.e
+00000e10: 006e 0064 0800 0000 0006 0000 000a 4465  .n.d..........De
+00000e20: 7363 656e 6469 6e67 0700 0000 0644 6961  scending.....Dia
+00000e30: 6c6f 6701 0300 0000 3e00 5700 6900 7200  log.....>.W.i.r.
+00000e40: 6b00 7300 6100 6d00 2000 6e00 6100 6300  k.s.a.m. .n.a.c.
+00000e50: 6800 2000 4100 6e00 7700 6500 6e00 6400  h. .A.n.w.e.n.d.
+00000e60: 7500 6e00 6700 7300 6e00 6500 7500 7300  u.n.g.s.n.e.u.s.
+00000e70: 7400 6100 7200 7408 0000 0000 0600 0000  t.a.r.t.........
+00000e80: 2345 6666 6563 7469 7665 2061 6674 6572  #Effective after
+00000e90: 2061 7070 6c69 6361 7469 6f6e 2072 6573   application res
+00000ea0: 7461 7274 0700 0000 0644 6961 6c6f 6701  tart.....Dialog.
+00000eb0: 03ff ffff ff08 0000 0000 0600 0000 0645  ...............E
+00000ec0: 7870 6f72 7407 0000 0006 4469 616c 6f67  xport.....Dialog
+00000ed0: 0103 0000 0034 0045 0078 0070 006f 0072  .....4.E.x.p.o.r
+00000ee0: 0074 0069 0065 0072 0065 0020 0043 0042  .t.i.e.r.e. .C.B
+00000ef0: 002d 0051 0053 004f 0073 0020 0069 006e  .-.Q.S.O.s. .i.n
+00000f00: 0020 0041 0044 0049 0046 0800 0000 0006  . .A.D.I.F......
+00000f10: 0000 0016 4578 706f 7274 2043 4220 5153  ....Export CB QS
+00000f20: 4f73 2074 6f20 4144 4946 0700 0000 0644  Os to ADIF.....D
+00000f30: 6961 6c6f 6701 0300 0000 3600 4500 7800  ialog.....6.E.x.
+00000f40: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
+00000f50: 2000 6e00 7500 7200 2000 6e00 6500 7500   .n.u.r. .n.e.u.
+00000f60: 6500 7300 7400 6500 2000 5100 5300 4f00  e.s.t.e. .Q.S.O.
+00000f70: 7308 0000 0000 0600 0000 1745 7870 6f72  s..........Expor
+00000f80: 7420 6f6e 6c79 2072 6563 656e 7420 5153  t only recent QS
+00000f90: 4f73 0700 0000 0644 6961 6c6f 6701 0300  Os.....Dialog...
+00000fa0: 0000 4200 4500 7800 7000 6f00 7200 7400  ..B.E.x.p.o.r.t.
+00000fb0: 6900 6500 7200 6500 2000 6500 6900 6700  i.e.r.e. .e.i.g.
+00000fc0: 6500 6e00 6500 2000 4e00 6f00 7400 6900  e.n.e. .N.o.t.i.
+00000fd0: 7a00 6500 6e00 2000 6900 6e00 2000 4100  z.e.n. .i.n. .A.
+00000fe0: 4400 4900 4608 0000 0000 0600 0000 1845  D.I.F..........E
+00000ff0: 7870 6f72 7420 6f77 6e20 6e6f 7465 7320  xport own notes 
+00001000: 746f 2041 4449 4607 0000 0006 4469 616c  to ADIF.....Dial
+00001010: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00001020: 000e 4861 6d6c 6962 2072 6967 6374 6c64  ..Hamlib rigctld
+00001030: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
+00001040: ff08 0000 0000 0600 0000 0d49 6d70 6f72  ...........Impor
+00001050: 742f 4578 706f 7274 0700 0000 0644 6961  t/Export.....Dia
+00001060: 6c6f 6701 0300 0000 1a00 5300 6300 6800  log.......S.c.h.
+00001070: 6e00 6900 7400 7400 7300 7400 6500 6c00  n.i.t.t.s.t.e.l.
+00001080: 6c00 6508 0000 0000 0600 0000 0949 6e74  l.e..........Int
+00001090: 6572 6661 6365 0700 0000 0644 6961 6c6f  erface.....Dialo
+000010a0: 6701 0300 0000 2000 6c00 6500 7400 7a00  g..... .l.e.t.z.
+000010b0: 7400 6500 7300 2000 4800 6100 6c00 6200  t.e.s. .H.a.l.b.
+000010c0: 6a00 6100 6800 7208 0000 0000 0600 0000  j.a.h.r.........
+000010d0: 0e4c 6173 7420 6861 6c66 2079 6561 7207  .Last half year.
+000010e0: 0000 0006 4469 616c 6f67 0103 0000 001a  ....Dialog......
+000010f0: 006c 0065 0074 007a 0074 0065 006e 0020  .l.e.t.z.t.e.n. 
+00001100: 004d 006f 006e 0061 0074 0800 0000 0006  .M.o.n.a.t......
+00001110: 0000 000a 4c61 7374 206d 6f6e 7468 0700  ....Last month..
+00001120: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
+00001130: 6c00 6500 7400 7a00 7400 6500 2000 5700  l.e.t.z.t.e. .W.
+00001140: 6f00 6300 6800 6508 0000 0000 0600 0000  o.c.h.e.........
+00001150: 094c 6173 7420 7765 656b 0700 0000 0644  .Last week.....D
+00001160: 6961 6c6f 6701 0300 0000 1800 6c00 6500  ialog.......l.e.
+00001170: 7400 7a00 7400 6500 7300 2000 4a00 6100  t.z.t.e.s. .J.a.
+00001180: 6800 7208 0000 0000 0600 0000 094c 6173  h.r..........Las
+00001190: 7420 7965 6172 0700 0000 0644 6961 6c6f  t year.....Dialo
+000011a0: 6701 0300 0000 0c00 4200 7200 6500 6900  g.......B.r.e.i.
+000011b0: 7400 6508 0000 0000 0600 0000 034c 6174  t.e..........Lat
+000011c0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+000011d0: 0a00 5300 7400 7500 6600 6508 0000 0000  ..S.t.u.f.e.....
+000011e0: 0600 0000 054c 6576 656c 0700 0000 0644  .....Level.....D
+000011f0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
+00001200: 0600 0000 044c 6f54 5707 0000 0006 4469  .....LoTW.....Di
+00001210: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
+00001220: 0000 0007 4c6f 6361 746f 7207 0000 0006  ....Locator.....
+00001230: 4469 616c 6f67 0103 0000 002c 004c 006f  Dialog.....,.L.o
+00001240: 0067 0020 0069 006e 0020 0044 0061 0074  .g. .i.n. .D.a.t
+00001250: 0065 0069 0020 0073 0063 0068 0072 0065  .e.i. .s.c.h.r.e
+00001260: 0069 0062 0065 006e 0800 0000 0006 0000  .i.b.e.n........
+00001270: 000b 4c6f 6720 746f 2066 696c 6507 0000  ..Log to file...
+00001280: 0006 4469 616c 6f67 0103 0000 001e 004c  ..Dialog.......L
+00001290: 006f 0067 0067 0069 006e 0067 002d 0041  .o.g.g.i.n.g.-.A
+000012a0: 0075 0073 0067 0061 0062 0065 0800 0000  .u.s.g.a.b.e....
+000012b0: 0006 0000 000e 4c6f 6767 696e 6720 6f75  ......Logging ou
+000012c0: 7470 7574 0700 0000 0644 6961 6c6f 6701  tput.....Dialog.
+000012d0: 0300 0000 0a00 4c00 e400 6e00 6700 6508  ......L...n.g.e.
+000012e0: 0000 0000 0600 0000 034c 6f6e 0700 0000  .........Lon....
+000012f0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00001300: 0000 0600 0000 044e 616d 6507 0000 0006  .......Name.....
+00001310: 4469 616c 6f67 0103 0000 005e 0043 0042  Dialog.....^.C.B
+00001320: 0020 0051 0053 004f 0073 0020 0077 0065  . .Q.S.O.s. .w.e
+00001330: 0072 0064 0065 006e 0020 0062 0065 0069  .r.d.e.n. .b.e.i
+00001340: 006d 0020 0049 006d 0070 006f 0072 0074  .m. .I.m.p.o.r.t
+00001350: 0020 0069 006d 006d 0065 0072 0020 0062  . .i.m.m.e.r. .b
+00001360: 0065 0072 00fc 0063 006b 0073 0069 0063  .e.r...c.k.s.i.c
+00001370: 0068 0074 0069 0067 0074 0800 0000 0006  .h.t.i.g.t......
+00001380: 0000 0028 4f6e 2069 6d70 6f72 7420 4342  ...(On import CB
+00001390: 2051 534f 7320 7769 6c6c 2061 6c77 6179   QSOs will alway
+000013a0: 7320 6265 2068 616e 646c 6564 0700 0000  s be handled....
+000013b0: 0644 6961 6c6f 6701 0300 0000 1000 5000  .Dialog.......P.
+000013c0: 6100 7300 7300 7700 6f00 7200 7408 0000  a.s.s.w.o.r.t...
+000013d0: 0000 0600 0000 0850 6173 7377 6f72 6407  .......Password.
+000013e0: 0000 0006 4469 616c 6f67 0103 0000 0070  ....Dialog.....p
+000013f0: 0050 0061 0073 0073 0077 006f 0072 0074  .P.a.s.s.w.o.r.t
+00001400: 0020 0064 0065 0073 0020 004c 006f 0054  . .d.e.s. .L.o.T
+00001410: 0057 002d 004f 006e 006c 0069 006e 0065  .W.-.O.n.l.i.n.e
+00001420: 002d 0041 0063 0063 006f 0075 006e 0074  .-.A.c.c.o.u.n.t
+00001430: 0073 002c 0020 006e 0069 0063 0068 0074  .s.,. .n.i.c.h.t
+00001440: 0020 0064 0065 0073 0020 005a 0065 0072  . .d.e.s. .Z.e.r
+00001450: 0074 0069 0066 0069 006b 0061 0074 0073  .t.i.f.i.k.a.t.s
+00001460: 0800 0000 0006 0000 0038 5061 7373 776f  .........8Passwo
+00001470: 7264 2066 6f72 204c 6f54 5720 6f6e 6c69  rd for LoTW onli
+00001480: 6e65 2061 6363 6f75 6e74 206e 6f74 2066  ne account not f
+00001490: 6f72 2074 6865 2063 6572 7469 6669 6361  or the certifica
+000014a0: 7465 0700 0000 0644 6961 6c6f 6701 03ff  te.....Dialog...
+000014b0: ffff ff08 0000 0000 0600 0000 0351 5448  .............QTH
+000014c0: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
+000014d0: ff08 0000 0000 0600 0000 0552 6164 696f  ...........Radio
+000014e0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+000014f0: 1800 4e00 6500 7500 6500 7300 7400 6500  ..N.e.u.e.s.t.e.
+00001500: 2000 5100 5300 4f00 7308 0000 0000 0600   .Q.S.O.s.......
+00001510: 0000 0b52 6563 656e 7420 5153 4f73 0700  ...Recent QSOs..
+00001520: 0000 0644 6961 6c6f 6701 0300 0000 1200  ...Dialog.......
+00001530: 4600 7500 6e00 6b00 6700 6500 7200 e400  F.u.n.k.g.e.r...
+00001540: 7408 0000 0000 0600 0000 0352 6967 0700  t..........Rig..
+00001550: 0000 0644 6961 6c6f 6701 0300 0000 4c00  ...Dialog.....L.
+00001560: 5300 6900 6500 6800 6500 2000 4500 6900  S.i.e.h.e. .E.i.
+00001570: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
+00001580: 6700 6500 6e00 2000 5200 6500 6900 7400  g.e.n. .R.e.i.t.
+00001590: 6500 7200 2000 2200 4100 6e00 7700 6500  e.r. .".A.n.w.e.
+000015a0: 6e00 6400 7500 6e00 6700 2208 0000 0000  n.d.u.n.g.".....
+000015b0: 0600 0000 2253 6565 2073 6574 7469 6e67  ...."See setting
+000015c0: 7320 7061 6765 2022 5573 6572 2069 6e74  s page "User int
+000015d0: 6572 6661 6365 2207 0000 0006 4469 616c  erface".....Dial
+000015e0: 6f67 0103 0000 0034 0043 0042 002d 0042  og.....4.C.B.-.B
+000015f0: 0061 006e 0064 0020 0061 0075 0074 006f  .a.n.d. .a.u.t.o
+00001600: 006d 0061 0074 0069 0073 0063 0068 0020  .m.a.t.i.s.c.h. 
+00001610: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
+00001620: 0006 0000 0019 5365 6c65 6374 2043 4220  ......Select CB 
+00001630: 6261 6e64 2062 7920 6465 6661 756c 7407  band by default.
+00001640: 0000 0006 4469 616c 6f67 0103 0000 000c  ....Dialog......
+00001650: 0044 0069 0065 006e 0073 0074 0800 0000  .D.i.e.n.s.t....
+00001660: 0006 0000 0007 5365 7276 6963 6507 0000  ......Service...
+00001670: 0006 4469 616c 6f67 0103 0000 001a 0053  ..Dialog.......S
+00001680: 0065 0074 007a 0065 0020 004c 006f 0063  .e.t.z.e. .L.o.c
+00001690: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+000016a0: 000b 5365 7420 6c6f 6361 746f 7207 0000  ..Set locator...
+000016b0: 0006 4469 616c 6f67 0103 0000 001a 0045  ..Dialog.......E
+000016c0: 0069 006e 0073 0074 0065 006c 006c 0075  .i.n.s.t.e.l.l.u
+000016d0: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
+000016e0: 0008 5365 7474 696e 6773 0700 0000 0644  ..Settings.....D
+000016f0: 6961 6c6f 6701 0300 0000 1c00 5a00 6500  ialog.......Z.e.
+00001700: 6900 6700 6500 2000 5100 5300 4f00 7300  i.g.e. .Q.S.O.s.
+00001710: 2000 6600 fc00 7208 0000 0000 0600 0000   .f...r.........
+00001720: 0e53 686f 7720 5153 4f73 2066 726f 6d07  .Show QSOs from.
+00001730: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
+00001740: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
+00001750: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
+00001760: 6f77 2061 6c6c 0700 0000 0644 6961 6c6f  ow all.....Dialo
+00001770: 6701 0300 0000 4000 5300 7000 6100 6c00  g.....@.S.p.a.l.
+00001780: 7400 6500 6e00 2000 6100 6e00 7a00 6500  t.e.n. .a.n.z.e.
+00001790: 6900 6700 6500 6e00 2000 6f00 6400 6500  i.g.e.n. .o.d.e.
+000017a0: 7200 2000 7600 6500 7200 7300 7400 6500  r. .v.e.r.s.t.e.
+000017b0: 6300 6b00 6500 6e08 0000 0000 0600 0000  c.k.e.n.........
+000017c0: 1453 686f 7720 6f72 2068 6964 6520 636f  .Show or hide co
+000017d0: 6c75 6d6e 7307 0000 0006 4469 616c 6f67  lumns.....Dialog
+000017e0: 0103 0000 0028 0053 006f 0072 0074 0069  .....(.S.o.r.t.i
+000017f0: 0065 0072 0065 0020 006e 0061 0063 0068  .e.r.e. .n.a.c.h
+00001800: 0020 0053 0070 0061 006c 0074 0065 0800  . .S.p.a.l.t.e..
+00001810: 0000 0006 0000 000e 536f 7274 206f 6e20  ........Sort on 
+00001820: 636f 6c75 6d6e 0700 0000 0644 6961 6c6f  column.....Dialo
+00001830: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001840: 0553 7461 7274 0700 0000 0644 6961 6c6f  .Start.....Dialo
+00001850: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001860: 0753 7461 7469 6f6e 0700 0000 0644 6961  .Station.....Dia
+00001870: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00001880: 0000 0454 5153 4c07 0000 0006 4469 616c  ...TQSL.....Dial
+00001890: 6f67 0103 0000 0064 0056 0065 0072 0077  og.....d.V.e.r.w
+000018a0: 0065 006e 0064 0065 0020 0064 0069 0065  .e.n.d.e. .d.i.e
+000018b0: 0020 006b 006f 006e 0066 0069 0067 0075  . .k.o.n.f.i.g.u
+000018c0: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
+000018d0: 0044 0020 0062 0065 0069 0020 0066 0065  .D. .b.e.i. .f.e
+000018e0: 0068 006c 0065 006e 0064 0065 006e 0020  .h.l.e.n.d.e.n. 
+000018f0: 0057 0065 0072 0074 0065 006e 0800 0000  .W.e.r.t.e.n....
+00001900: 0006 0000 0024 5573 6520 636f 6e66 6967  .....$Use config
+00001910: 7572 6564 2049 4420 666f 7220 6d69 7373  ured ID for miss
+00001920: 696e 6720 7661 6c75 6573 0700 0000 0644  ing values.....D
+00001930: 6961 6c6f 6701 0300 0000 6e00 5600 6500  ialog.....n.V.e.
+00001940: 7200 7700 6500 6e00 6400 6500 2000 6400  r.w.e.n.d.e. .d.
+00001950: 6900 6500 2000 6b00 6f00 6e00 6600 6900  i.e. .k.o.n.f.i.
+00001960: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
+00001970: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
+00001980: 2000 6200 6500 6900 2000 6600 6500 6800   .b.e.i. .f.e.h.
+00001990: 6c00 6500 6e00 6400 6500 6e00 2000 5700  l.e.n.d.e.n. .W.
+000019a0: 6500 7200 7400 6500 6e08 0000 0000 0600  e.r.t.e.n.......
+000019b0: 0000 2955 7365 2063 6f6e 6669 6775 7265  ..)Use configure
+000019c0: 6420 5374 6174 696f 6e20 666f 7220 6d69  d Station for mi
+000019d0: 7373 696e 6720 7661 6c75 6573 0700 0000  ssing values....
+000019e0: 0644 6961 6c6f 6701 0300 0000 1200 4100  .Dialog.......A.
+000019f0: 6e00 7700 6500 6e00 6400 7500 6e00 6708  n.w.e.n.d.u.n.g.
+00001a00: 0000 0000 0600 0000 0e55 7365 7220 696e  .........User in
+00001a10: 7465 7266 6163 6507 0000 0006 4469 616c  terface.....Dial
+00001a20: 6f67 0103 0000 0018 0042 0065 006e 0075  og.......B.e.n.u
+00001a30: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
+00001a40: 0800 0000 0006 0000 0008 5573 6572 6e61  ..........Userna
+00001a50: 6d65 0700 0000 0644 6961 6c6f 6701 0300  me.....Dialog...
+00001a60: 0000 7800 4200 6500 6e00 7500 7400 7a00  ..x.B.e.n.u.t.z.
+00001a70: 6500 7200 6e00 6100 6d00 6500 2000 6400  e.r.n.a.m.e. .d.
+00001a80: 6500 7300 2000 4c00 6f00 5400 5700 2d00  e.s. .L.o.T.W.-.
+00001a90: 4f00 6e00 6c00 6900 6e00 6500 2d00 4100  O.n.l.i.n.e.-.A.
+00001aa0: 6300 6300 6f00 7500 6e00 7400 7300 2c00  c.c.o.u.n.t.s.,.
+00001ab0: 2000 6e00 6900 6300 6800 7400 2000 6400   .n.i.c.h.t. .d.
+00001ac0: 6500 7300 2000 5a00 6500 7200 7400 6900  e.s. .Z.e.r.t.i.
+00001ad0: 6600 6900 6b00 6100 7400 7308 0000 0000  f.i.k.a.t.s.....
+00001ae0: 0600 0000 3855 7365 726e 616d 6520 666f  ....8Username fo
+00001af0: 7220 4c6f 5457 206f 6e6c 696e 6520 6163  r LoTW online ac
+00001b00: 636f 756e 7420 6e6f 7420 666f 7220 7468  count not for th
+00001b10: 6520 6365 7274 6966 6963 6174 6507 0000  e certificate...
+00001b20: 0006 4469 616c 6f67 0103 0000 0020 0044  ..Dialog..... .D
+00001b30: 0061 0074 0065 0069 00fc 0062 0065 0072  .a.t.e.i...b.e.r
+00001b40: 0077 0061 0063 0068 0075 006e 0067 0800  .w.a.c.h.u.n.g..
+00001b50: 0000 0006 0000 000a 5761 7463 6820 4669  ........Watch Fi
+00001b60: 6c65 0700 0000 0644 6961 6c6f 6701 03ff  le.....Dialog...
+00001b70: ffff ff08 0000 0000 0600 0000 0465 5153  .............eQS
+00001b80: 4c07 0000 0006 4469 616c 6f67 0103 ffff  L.....Dialog....
+00001b90: ffff 0800 0000 0006 0000 0002 c2b0 0700  ................
+00001ba0: 0000 0644 6961 6c6f 6701 0300 0000 9e00  ...Dialog.......
+00001bb0: 4500 6900 6e00 2000 4400 6100 7400 6500  E.i.n. .D.a.t.e.
+00001bc0: 6e00 6200 6100 6e00 6b00 2d00 4200 6100  n.b.a.n.k.-.B.a.
+00001bd0: 6300 6b00 7500 7000 2000 6b00 6f00 6e00  c.k.u.p. .k.o.n.
+00001be0: 6e00 7400 6500 2000 6e00 6900 6300 6800  n.t.e. .n.i.c.h.
+00001bf0: 7400 2000 6500 7200 7300 7400 6500 6c00  t. .e.r.s.t.e.l.
+00001c00: 6c00 7400 2000 7700 6500 7200 6400 6500  l.t. .w.e.r.d.e.
+00001c10: 6e00 2e00 0a00 4400 6900 6500 2000 4400  n.....D.i.e. .D.
+00001c20: 6100 7400 6500 6900 2000 6500 7800 6900  a.t.e.i. .e.x.i.
+00001c30: 7300 7400 6900 6500 7200 7400 2000 6200  s.t.i.e.r.t. .b.
+00001c40: 6500 7200 6500 6900 7400 7300 2e08 0000  e.r.e.i.t.s.....
+00001c50: 0000 0600 0000 4041 2064 6174 6162 6173  ......@A databas
+00001c60: 6520 6261 636b 7570 2063 6f75 6c64 206e  e backup could n
+00001c70: 6f74 2062 6520 6372 6561 7465 642e 0a54  ot be created..T
+00001c80: 6865 2066 696c 6520 616c 7265 6164 7920  he file already 
+00001c90: 6578 6973 7473 2e07 0000 0009 4472 6167  exists......Drag
+00001ca0: 6f6e 4c6f 6701 0300 0000 4e00 4500 6900  onLog.....N.E.i.
+00001cb0: 6e00 2000 4100 4400 4900 4600 2d00 4600  n. .A.D.I.F.-.F.
+00001cc0: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
+00001cd0: 7400 2000 6600 fc00 7200 2000 6400 6500  t. .f...r. .d.e.
+00001ce0: 6e00 2000 4c00 6f00 5400 5700 2d00 5500  n. .L.o.T.W.-.U.
+00001cf0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
+00001d00: 0000 1d41 2066 6965 6c64 2069 7320 6d69  ...A field is mi
+00001d10: 7373 696e 6720 666f 7220 7570 6c6f 6164  ssing for upload
+00001d20: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001d30: ffff ffff 0800 0000 0006 0000 0015 4144  ..............AD
+00001d40: 4946 2033 2028 2a2e 6164 6920 2a2e 6164  IF 3 (*.adi *.ad
+00001d50: 6966 2907 0000 0009 4472 6167 6f6e 4c6f  if).....DragonLo
+00001d60: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001d70: 1b41 4449 4620 3320 282a 2e61 6478 202a  .ADIF 3 (*.adx *
+00001d80: 2e61 6469 202a 2e61 6469 6629 0700 0000  .adi *.adif)....
+00001d90: 0944 7261 676f 6e4c 6f67 0103 0000 0008  .DragonLog......
+00001da0: 00dc 0062 0065 0072 0800 0000 0006 0000  ...b.e.r........
+00001db0: 0005 4162 6f75 7407 0000 0009 4472 6167  ..About.....Drag
+00001dc0: 6f6e 4c6f 6701 0300 0000 0e00 dc00 6200  onLog.........b.
+00001dd0: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
+00001de0: 0000 0841 626f 7574 2051 7407 0000 0009  ...About Qt.....
+00001df0: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
+00001e00: 4100 6900 7200 6300 7200 6100 6600 7400  A.i.r.c.r.a.f.t.
+00001e10: 2d00 5300 6300 6100 7400 7400 6500 7208  -.S.c.a.t.t.e.r.
+00001e20: 0000 0000 0600 0000 1041 6972 6372 6166  .........Aircraf
+00001e30: 7420 5363 6174 7465 7207 0000 0009 4472  t Scatter.....Dr
+00001e40: 6167 6f6e 4c6f 6701 0300 0000 0e00 4100  agonLog.......A.
+00001e50: 6e00 7400 6500 6e00 6e00 6508 0000 0000  n.t.e.n.n.e.....
+00001e60: 0600 0000 0741 6e74 656e 6e61 0700 0000  .....Antenna....
+00001e70: 0944 7261 676f 6e4c 6f67 0103 ffff ffff  .DragonLog......
+00001e80: 0800 0000 0006 0000 0006 4175 726f 7261  ..........Aurora
+00001e90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001ea0: ffff ffff 0800 0000 0006 0000 0008 4175  ..............Au
+00001eb0: 726f 7261 2d45 0700 0000 0944 7261 676f  rora-E.....Drago
+00001ec0: 6e4c 6f67 0103 0000 000a 0041 0075 0074  nLog.......A.u.t
+00001ed0: 006f 0072 0800 0000 0006 0000 0006 4175  .o.r..........Au
+00001ee0: 7468 6f72 0700 0000 0944 7261 676f 6e4c  thor.....DragonL
+00001ef0: 6f67 0103 0000 0018 0042 0061 0063 006b  og.......B.a.c.k
+00001f00: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
+00001f10: 0800 0000 0006 0000 000c 4261 636b 2073  ..........Back s
+00001f20: 6361 7474 6572 0700 0000 0944 7261 676f  catter.....Drago
+00001f30: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
+00001f40: 0000 0004 4261 6e64 0700 0000 0944 7261  ....Band.....Dra
+00001f50: 676f 6e4c 6f67 0103 0000 0022 0043 0053  gonLog.....".C.S
+00001f60: 0056 002d 0044 0061 0074 0065 0069 0020  .V.-.D.a.t.e.i. 
+00001f70: 0028 002a 002e 0063 0073 0076 0029 0800  .(.*...c.s.v.)..
+00001f80: 0000 0006 0000 0010 4353 562d 4669 6c65  ........CSV-File
+00001f90: 2028 2a2e 6373 7629 0700 0000 0944 7261   (*.csv).....Dra
+00001fa0: 676f 6e4c 6f67 0103 0000 0014 0052 0075  gonLog.......R.u
+00001fb0: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
+00001fc0: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
+00001fd0: 6967 6e07 0000 0009 4472 6167 6f6e 4c6f  ign.....DragonLo
+00001fe0: 6701 0300 0000 0a00 4b00 6100 6e00 6100  g.......K.a.n.a.
+00001ff0: 6c08 0000 0000 0600 0000 0743 6861 6e6e  l..........Chann
+00002000: 656c 0700 0000 0944 7261 676f 6e4c 6f67  el.....DragonLog
+00002010: 0103 0000 0074 0050 0072 00fc 0066 0075  .....t.P.r...f.u
+00002020: 006e 0067 0020 0064 0065 0072 0020 0044  .n.g. .d.e.r. .D
+00002030: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
+00002040: 0020 0066 0065 0068 006c 0067 0065 0073  . .f.e.h.l.g.e.s
+00002050: 0063 0068 006c 0061 0067 0065 006e 002e  .c.h.l.a.g.e.n..
+00002060: 0020 0049 006e 0068 0061 006c 0074 0020  . .I.n.h.a.l.t. 
+00002070: 006e 0069 0063 0068 0074 0020 006c 0065  .n.i.c.h.t. .l.e
+00002080: 0073 0062 0061 0072 002e 0800 0000 0006  .s.b.a.r........
+00002090: 0000 0034 4368 6563 6b69 6e67 2064 6174  ...4Checking dat
+000020a0: 6162 6173 6520 6661 696c 6564 2e20 436f  abase failed. Co
+000020b0: 6e74 656e 7420 6973 206e 6f74 2061 6363  ntent is not acc
+000020c0: 6573 7361 626c 652e 0700 0000 0944 7261  essable......Dra
+000020d0: 676f 6e4c 6f67 0103 0000 0012 004b 006f  gonLog.......K.o
+000020e0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+000020f0: 0000 0006 0000 0007 436f 6d6d 656e 7407  ........Comment.
+00002100: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002110: 0000 6000 5600 6500 7200 6200 6900 6e00  ..`.V.e.r.b.i.n.
+00002120: 6400 7500 6e00 6700 7300 6600 6500 6800  d.u.n.g.s.f.e.h.
+00002130: 6c00 6500 7200 2000 6f00 6400 6500 7200  l.e.r. .o.d.e.r.
+00002140: 2000 4e00 6500 7400 7a00 7700 6500 7200   .N.e.t.z.w.e.r.
+00002150: 6b00 2000 6e00 6900 6300 6800 7400 2000  k. .n.i.c.h.t. .
+00002160: 6500 7200 7200 6500 6900 6300 6800 6200  e.r.r.e.i.c.h.b.
+00002170: 6100 7208 0000 0000 0600 0000 2743 6f6e  a.r.........'Con
+00002180: 6e65 6374 696f 6e20 6572 726f 7220 6f72  nection error or
+00002190: 206e 6574 776f 726b 2075 6e72 6561 6368   network unreach
+000021a0: 6162 6c65 0700 0000 0944 7261 676f 6e4c  able.....DragonL
+000021b0: 6f67 0103 0000 002e 0044 0061 0074 0065  og.......D.a.t.e
+000021c0: 006e 0062 0061 006e 006b 002d 0042 0061  .n.b.a.n.k.-.B.a
+000021d0: 0063 006b 0075 0070 0020 0046 0065 0068  .c.k.u.p. .F.e.h
+000021e0: 006c 0065 0072 0800 0000 0006 0000 0015  .l.e.r..........
+000021f0: 4461 7461 6261 7365 2062 6163 6b75 7020  Database backup 
+00002200: 6572 726f 7207 0000 0009 4472 6167 6f6e  error.....Dragon
+00002210: 4c6f 6701 0300 0000 2c00 4400 6100 7400  Log.....,.D.a.t.
+00002220: 6500 6e00 6200 6100 6e00 6b00 6b00 6f00  e.n.b.a.n.k.k.o.
+00002230: 6e00 7600 6500 7200 7400 6900 6500 7200  n.v.e.r.t.i.e.r.
+00002240: 7500 6e00 6708 0000 0000 0600 0000 1344  u.n.g..........D
+00002250: 6174 6162 6173 6520 636f 6e76 6572 7369  atabase conversi
+00002260: 6f6e 0700 0000 0944 7261 676f 6e4c 6f67  on.....DragonLog
+00002270: 0103 0000 0048 0044 0061 0074 0065 006e  .....H.D.a.t.e.n
+00002280: 0062 0061 006e 006b 006b 006f 006e 0076  .b.a.n.k.k.o.n.v
+00002290: 0065 0072 0074 0069 0065 0072 0075 006e  .e.r.t.i.e.r.u.n
+000022a0: 0067 0020 0061 0062 0067 0065 0073 0063  .g. .a.b.g.e.s.c
+000022b0: 0068 006c 006f 0073 0073 0065 006e 0800  .h.l.o.s.s.e.n..
+000022c0: 0000 0006 0000 001c 4461 7461 6261 7365  ........Database
+000022d0: 2063 6f6e 7665 7273 696f 6e20 6669 6e69   conversion fini
+000022e0: 7368 6564 0700 0000 0944 7261 676f 6e4c  shed.....DragonL
+000022f0: 6f67 0103 0000 001e 0044 0061 0074 0065  og.......D.a.t.e
+00002300: 006e 0062 0061 006e 006b 0066 0065 0068  .n.b.a.n.k.f.e.h
+00002310: 006c 0065 0072 0800 0000 0006 0000 000e  .l.e.r..........
+00002320: 4461 7461 6261 7365 2065 7272 6f72 0700  Database error..
+00002330: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002340: 0034 0044 0061 0074 0065 006e 0062 0061  .4.D.a.t.e.n.b.a
+00002350: 006e 006b 0073 0074 0072 0075 006b 0074  .n.k.s.t.r.u.k.t
+00002360: 0075 0072 0020 0076 0065 0072 0061 006c  .u.r. .v.e.r.a.l
+00002370: 0074 0065 0074 0800 0000 0006 0000 001c  .t.e.t..........
+00002380: 4461 7461 6261 7365 2073 7472 7563 7475  Database structu
+00002390: 7265 206f 7574 2d64 6174 6564 0700 0000  re out-dated....
+000023a0: 0944 7261 676f 6e4c 6f67 0103 0000 001e  .DragonLog......
+000023b0: 0044 0061 0074 0075 006d 002f 005a 0065  .D.a.t.u.m./.Z.e
+000023c0: 0069 0074 0020 0045 006e 0064 0065 0800  .i.t. .E.n.d.e..
+000023d0: 0000 0006 0000 000d 4461 7465 2f54 696d  ........Date/Tim
+000023e0: 6520 656e 6407 0000 0009 4472 6167 6f6e  e end.....Dragon
+000023f0: 4c6f 6701 0300 0000 2000 4400 6100 7400  Log..... .D.a.t.
+00002400: 7500 6d00 2f00 5a00 6500 6900 7400 2000  u.m./.Z.e.i.t. .
+00002410: 5300 7400 6100 7200 7408 0000 0000 0600  S.t.a.r.t.......
+00002420: 0000 0f44 6174 652f 5469 6d65 2073 7461  ...Date/Time sta
+00002430: 7274 0700 0000 0944 7261 676f 6e4c 6f67  rt.....DragonLog
+00002440: 0103 0000 0016 0051 0053 004f 0020 006c  .......Q.S.O. .l
+00002450: 00f6 0073 0063 0068 0065 006e 0800 0000  ...s.c.h.e.n....
+00002460: 0006 0000 000a 4465 6c65 7465 2051 534f  ......Delete QSO
+00002470: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002480: 0000 0014 0045 006e 0074 0066 0065 0072  .....E.n.t.f.e.r
+00002490: 006e 0075 006e 0067 0800 0000 0006 0000  .n.u.n.g........
+000024a0: 0008 4469 7374 616e 6365 0700 0000 0944  ..Distance.....D
+000024b0: 7261 676f 6e4c 6f67 0103 0000 0064 0057  ragonLog.....d.W
+000024c0: 006f 006c 006c 0065 006e 0020 0073 0069  .o.l.l.e.n. .s.i
+000024d0: 0065 0020 0064 0069 0065 0020 0073 0065  .e. .d.i.e. .s.e
+000024e0: 006c 0065 006b 0074 0069 0065 0072 0074  .l.e.k.t.i.e.r.t
+000024f0: 0065 006e 0020 0051 0053 004f 0073 0020  .e.n. .Q.S.O.s. 
+00002500: 0077 0069 0072 006b 006c 0069 0063 0068  .w.i.r.k.l.i.c.h
+00002510: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
+00002520: 003f 0800 0000 0006 0000 0031 446f 2079  .?.........1Do y
+00002530: 6f75 2072 6561 6c6c 7920 7761 6e74 2074  ou really want t
+00002540: 6f20 6465 6c65 7465 2074 6865 2073 656c  o delete the sel
+00002550: 6563 7465 6420 5153 4f28 7329 3f07 0000  ected QSO(s)?...
+00002560: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+00002570: ff08 0000 0000 0600 0000 1045 6172 7468  ...........Earth
+00002580: 2d4d 6f6f 6e2d 4561 7274 6807 0000 0009  -Moon-Earth.....
+00002590: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+000025a0: 0000 0000 0600 0000 0845 6368 6f4c 696e  .........EchoLin
+000025b0: 6b07 0000 0009 4472 6167 6f6e 4c6f 6701  k.....DragonLog.
+000025c0: 0300 0000 0c00 4600 6500 6800 6c00 6500  ......F.e.h.l.e.
+000025d0: 7208 0000 0000 0600 0000 0545 7272 6f72  r..........Error
+000025e0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000025f0: 0000 0028 0045 0078 0063 0065 006c 002d  ...(.E.x.c.e.l.-
+00002600: 0044 0061 0074 0065 0069 0020 0028 002a  .D.a.t.e.i. .(.*
+00002610: 002e 0078 006c 0073 0078 0029 0800 0000  ...x.l.s.x.)....
+00002620: 0006 0000 0013 4578 6365 6c2d 4669 6c65  ......Excel-File
+00002630: 2028 2a2e 786c 7378 2907 0000 0009 4472   (*.xlsx).....Dr
+00002640: 6167 6f6e 4c6f 6701 0300 0000 2400 4500  agonLog.....$.E.
+00002650: 7800 7000 6f00 7200 7400 6900 6500 7200  x.p.o.r.t.i.e.r.
+00002660: 6500 2000 5100 5300 4f00 2000 6c00 6f00  e. .Q.S.O. .l.o.
+00002670: 6708 0000 0000 0600 0000 1045 7870 6f72  g..........Expor
+00002680: 7465 6420 5153 4f20 6c6f 6707 0000 0009  ted QSO log.....
+00002690: 4472 6167 6f6e 4c6f 6701 0300 0000 1a00  DragonLog.......
+000026a0: 4600 3200 2d00 5200 6500 6600 6c00 6500  F.2.-.R.e.f.l.e.
+000026b0: 6b00 7400 6900 6f00 6e08 0000 0000 0600  k.t.i.o.n.......
+000026c0: 0000 0d46 3220 5265 666c 6563 7469 6f6e  ...F2 Reflection
+000026d0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000026e0: 0000 0038 0046 0069 0065 006c 0064 002d  ...8.F.i.e.l.d.-
+000026f0: 0041 006c 0069 0067 006e 0065 0064 002d  .A.l.i.g.n.e.d.-
+00002700: 0049 0072 0072 0065 0067 0075 006c 0061  .I.r.r.e.g.u.l.a
+00002710: 0072 0069 0074 0069 0065 0073 0800 0000  .r.i.t.i.e.s....
+00002720: 0006 0000 001c 4669 656c 6420 416c 6967  ......Field Alig
+00002730: 6e65 6420 4972 7265 6775 6c61 7269 7469  ned Irregulariti
+00002740: 6573 0700 0000 0944 7261 676f 6e4c 6f67  es.....DragonLog
+00002750: 0103 0000 0010 0046 0072 0065 0071 0075  .......F.r.e.q.u
+00002760: 0065 006e 007a 0800 0000 0006 0000 0009  .e.n.z..........
+00002770: 4672 6571 7565 6e63 7907 0000 0009 4472  Frequency.....Dr
+00002780: 6167 6f6e 4c6f 6701 0300 0000 1400 4200  agonLog.......B.
+00002790: 6f00 6400 6500 6e00 7700 6500 6c00 6c00  o.d.e.n.w.e.l.l.
+000027a0: 6508 0000 0000 0600 0000 0b47 726f 756e  e..........Groun
+000027b0: 6420 5761 7665 0700 0000 0944 7261 676f  d Wave.....Drago
+000027c0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
+000027d0: 0000 0006 4861 6d51 5448 0700 0000 0944  ....HamQTH.....D
+000027e0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+000027f0: 0000 0006 0000 0006 4861 6d6c 6962 0700  ........Hamlib..
+00002800: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002810: 000a 0048 0069 006c 0066 0065 0800 0000  ...H.i.l.f.e....
+00002820: 0006 0000 0004 4865 6c70 0700 0000 0944  ......Help.....D
+00002830: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+00002840: 0000 0006 0000 0004 4952 4c50 0700 0000  ........IRLP....
+00002850: 0944 7261 676f 6e4c 6f67 0103 0000 0026  .DragonLog.....&
+00002860: 0049 006e 0074 0065 0072 006e 0065 0074  .I.n.t.e.r.n.e.t
+00002870: 0075 006e 0074 0065 0072 0073 0074 00fc  .u.n.t.e.r.s.t..
+00002880: 0074 007a 0074 0800 0000 0006 0000 0011  .t.z.t..........
+00002890: 496e 7465 726e 6574 2d61 7373 6973 7465  Internet-assiste
+000028a0: 6407 0000 0009 4472 6167 6f6e 4c6f 6701  d.....DragonLog.
+000028b0: 0300 0000 1800 4900 6f00 6e00 6f00 2d00  ......I.o.n.o.-.
+000028c0: 5300 6300 6100 7400 7400 6500 7208 0000  S.c.a.t.t.e.r...
+000028d0: 0000 0600 0000 0b49 6f6e 6f73 6361 7474  .......Ionoscatt
+000028e0: 6572 0700 0000 0944 7261 676f 6e4c 6f67  er.....DragonLog
+000028f0: 0103 0000 0020 006c 0065 0074 007a 0074  ..... .l.e.t.z.t
+00002900: 0065 0073 0020 0048 0061 006c 0062 006a  .e.s. .H.a.l.b.j
+00002910: 0061 0068 0072 0800 0000 0006 0000 000e  .a.h.r..........
+00002920: 4c61 7374 2068 616c 6620 7965 6172 0700  Last half year..
+00002930: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002940: 001a 006c 0065 0074 007a 0074 0065 006e  ...l.e.t.z.t.e.n
+00002950: 0020 004d 006f 006e 0061 0074 0800 0000  . .M.o.n.a.t....
+00002960: 0006 0000 000a 4c61 7374 206d 6f6e 7468  ......Last month
+00002970: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002980: 0000 0018 006c 0065 0074 007a 0074 0065  .....l.e.t.z.t.e
+00002990: 0020 0057 006f 0063 0068 0065 0800 0000  . .W.o.c.h.e....
+000029a0: 0006 0000 0009 4c61 7374 2077 6565 6b07  ......Last week.
+000029b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+000029c0: 0000 1800 6c00 6500 7400 7a00 7400 6500  ....l.e.t.z.t.e.
+000029d0: 7300 2000 4a00 6100 6800 7208 0000 0000  s. .J.a.h.r.....
+000029e0: 0600 0000 094c 6173 7420 7965 6172 0700  .....Last year..
+000029f0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002a00: 001e 0053 0069 0063 0068 0074 0076 0065  ...S.i.c.h.t.v.e
+00002a10: 0072 0062 0069 006e 0064 0075 006e 0067  .r.b.i.n.d.u.n.g
+00002a20: 0800 0000 0006 0000 000d 4c69 6e65 206f  ..........Line o
+00002a30: 6620 5369 6768 7407 0000 0009 4472 6167  f Sight.....Drag
+00002a40: 6f6e 4c6f 6701 0300 0000 2000 4c00 6f00  onLog..... .L.o.
+00002a50: 5400 5700 2d00 4100 4400 4900 4600 2d00  T.W.-.A.D.I.F.-.
+00002a60: 5500 7000 6c00 6f00 6100 6408 0000 0000  U.p.l.o.a.d.....
+00002a70: 0600 0000 104c 6f54 5720 4144 4946 2075  .....LoTW ADIF u
+00002a80: 706c 6f61 6407 0000 0009 4472 6167 6f6e  pload.....Dragon
+00002a90: 4c6f 6701 0300 0000 1400 4c00 6f00 5400  Log.......L.o.T.
+00002aa0: 5700 2000 6500 6d00 7000 6600 2e08 0000  W. .e.m.p.f.....
+00002ab0: 0000 0600 0000 094c 6f54 5720 7263 7664  .......LoTW rcvd
+00002ac0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002ad0: 0000 0014 004c 006f 0054 0057 0020 0076  .....L.o.T.W. .v
+00002ae0: 0065 0072 0073 002e 0800 0000 0006 0000  .e.r.s..........
+00002af0: 0009 4c6f 5457 2073 656e 7407 0000 0009  ..LoTW sent.....
+00002b00: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00002b10: 0000 0000 0600 0000 074c 6f63 6174 6f72  .........Locator
+00002b20: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002b30: ffff ffff 0800 0000 0006 0000 000f 4c6f  ..............Lo
+00002b40: 6720 696d 706f 7274 2041 4449 4607 0000  g import ADIF...
+00002b50: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002b60: 1c00 4c00 6f00 6700 2000 4900 6d00 7000  ..L.o.g. .I.m.p.
+00002b70: 6f00 7200 7400 2000 4300 5300 5608 0000  o.r.t. .C.S.V...
+00002b80: 0000 0600 0000 0e4c 6f67 2069 6d70 6f72  .......Log impor
+00002b90: 7420 4353 5607 0000 0009 4472 6167 6f6e  t CSV.....Dragon
+00002ba0: 4c6f 6701 0300 0000 2000 4c00 6f00 6700  Log..... .L.o.g.
+00002bb0: 2000 4900 6d00 7000 6f00 7200 7400 2000   .I.m.p.o.r.t. .
+00002bc0: 4500 7800 6300 6500 6c08 0000 0000 0600  E.x.c.e.l.......
+00002bd0: 0000 104c 6f67 2069 6d70 6f72 7420 4578  ...Log import Ex
+00002be0: 6365 6c07 0000 0009 4472 6167 6f6e 4c6f  cel.....DragonLo
+00002bf0: 6701 0300 0000 1c00 4d00 6500 7400 6500  g.......M.e.t.e.
+00002c00: 6f00 7200 2d00 5300 6300 6100 7400 7400  o.r.-.S.c.a.t.t.
+00002c10: 6500 7208 0000 0000 0600 0000 0e4d 6574  e.r..........Met
+00002c20: 656f 7220 7363 6174 7465 7207 0000 0009  eor scatter.....
+00002c30: 4472 6167 6f6e 4c6f 6701 0300 0000 5a00  DragonLog.....Z.
+00002c40: 4b00 6500 6900 6e00 6500 2000 5300 7400  K.e.i.n.e. .S.t.
+00002c50: 6100 7400 6900 6f00 6e00 7300 6b00 6f00  a.t.i.o.n.s.k.o.
+00002c60: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
+00002c70: 6900 6f00 6e00 2000 6900 6e00 2000 5400  i.o.n. .i.n. .T.
+00002c80: 5100 5300 4c00 2000 7600 6500 7200 6600  Q.S.L. .v.e.r.f.
+00002c90: fc00 6700 6200 6100 7208 0000 0000 0600  ..g.b.a.r.......
+00002ca0: 0000 254d 6973 7369 6e67 2073 7461 7469  ..%Missing stati
+00002cb0: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
+00002cc0: 2069 6e20 5451 534c 0700 0000 0944 7261   in TQSL.....Dra
+00002cd0: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00002ce0: 0006 0000 0004 4d6f 6465 0700 0000 0944  ......Mode.....D
+00002cf0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+00002d00: 0000 0006 0000 0004 4e61 6d65 0700 0000  ........Name....
+00002d10: 0944 7261 676f 6e4c 6f67 0103 0000 0034  .DragonLog.....4
+00002d20: 004b 0065 0069 006e 0065 0020 0051 0053  .K.e.i.n.e. .Q.S
+00002d30: 004f 0073 0020 0066 00fc 0072 0020 0064  .O.s. .f...r. .d
+00002d40: 0065 006e 0020 004c 006f 0063 0061 0074  .e.n. .L.o.c.a.t
+00002d50: 006f 0072 0800 0000 0006 0000 0017 4e6f  .o.r..........No
+00002d60: 2072 6563 6f72 6473 2066 6f72 206c 6f63   records for loc
+00002d70: 6174 696f 6e07 0000 0009 4472 6167 6f6e  ation.....Dragon
+00002d80: 4c6f 6701 0300 0000 0e00 4e00 6f00 7400  Log.......N.o.t.
+00002d90: 6900 7a00 6500 6e08 0000 0000 0600 0000  i.z.e.n.........
+00002da0: 054e 6f74 6573 0700 0000 0944 7261 676f  .Notes.....Drago
+00002db0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
+00002dc0: 0000 0002 4f6b 0700 0000 0944 7261 676f  ....Ok.....Drago
+00002dd0: 6e4c 6f67 0103 0000 001e 0045 0069 0067  nLog.......E.i.g
+00002de0: 0065 006e 0065 0072 0020 004c 006f 0063  .e.n.e.r. .L.o.c
+00002df0: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+00002e00: 000b 4f77 6e20 4c6f 6361 746f 7207 0000  ..Own Locator...
+00002e10: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002e20: 1800 4500 6900 6700 6500 6e00 6500 7200  ..E.i.g.e.n.e.r.
+00002e30: 2000 4e00 6100 6d00 6508 0000 0000 0600   .N.a.m.e.......
+00002e40: 0000 084f 776e 204e 616d 6507 0000 0009  ...Own Name.....
+00002e50: 4472 6167 6f6e 4c6f 6701 0300 0000 1600  DragonLog.......
+00002e60: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
+00002e70: 5100 5400 4808 0000 0000 0600 0000 074f  Q.T.H..........O
+00002e80: 776e 2051 5448 0700 0000 0944 7261 676f  wn QTH.....Drago
+00002e90: 6e4c 6f67 0103 0000 0024 0045 0069 0067  nLog.....$.E.i.g
+00002ea0: 0065 006e 0065 0073 0020 0052 0075 0066  .e.n.e.s. .R.u.f
+00002eb0: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+00002ec0: 0000 0006 0000 000d 4f77 6e20 6361 6c6c  ........Own call
+00002ed0: 2073 6967 6e07 0000 0009 4472 6167 6f6e   sign.....Dragon
+00002ee0: 4c6f 6701 0300 0000 1000 4c00 6500 6900  Log.......L.e.i.
+00002ef0: 7300 7400 7500 6e00 6708 0000 0000 0600  s.t.u.n.g.......
+00002f00: 0000 0550 6f77 6572 0700 0000 0944 7261  ...Power.....Dra
+00002f10: 676f 6e4c 6f67 0103 0000 0016 0041 0075  gonLog.......A.u
+00002f20: 0073 0062 0072 0065 0069 0074 0075 006e  .s.b.r.e.i.t.u.n
+00002f30: 0067 0800 0000 0006 0000 000b 5072 6f70  .g..........Prop
+00002f40: 6167 6174 696f 6e07 0000 0009 4472 6167  agation.....Drag
+00002f50: 6f6e 4c6f 6701 0300 0000 1a00 5100 5300  onLog.......Q.S.
+00002f60: 4c00 2d00 4e00 6100 6300 6800 7200 6900  L.-.N.a.c.h.r.i.
+00002f70: 6300 6800 7408 0000 0000 0600 0000 0b51  c.h.t..........Q
+00002f80: 534c 206d 6573 7361 6765 0700 0000 0944  SL message.....D
+00002f90: 7261 676f 6e4c 6f67 0103 0000 0010 0051  ragonLog.......Q
+00002fa0: 0053 004c 002d 0050 0066 0061 0064 0800  .S.L.-.P.f.a.d..
+00002fb0: 0000 0006 0000 0008 5153 4c20 7061 7468  ........QSL path
+00002fc0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002fd0: 0000 0012 0051 0053 004c 0020 0065 006d  .....Q.S.L. .e.m
+00002fe0: 0070 0066 002e 0800 0000 0006 0000 0008  .p.f............
+00002ff0: 5153 4c20 7263 7664 0700 0000 0944 7261  QSL rcvd.....Dra
+00003000: 676f 6e4c 6f67 0103 0000 0012 0051 0053  gonLog.......Q.S
+00003010: 004c 0020 0076 0065 0072 0073 002e 0800  .L. .v.e.r.s....
+00003020: 0000 0006 0000 0008 5153 4c20 7365 6e74  ........QSL sent
+00003030: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003040: 0000 000e 0051 0053 004c 002d 0056 0069  .....Q.S.L.-.V.i
+00003050: 0061 0800 0000 0006 0000 0007 5153 4c20  .a..........QSL 
+00003060: 7669 6107 0000 0009 4472 6167 6f6e 4c6f  via.....DragonLo
+00003070: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00003080: 0351 534f 0700 0000 0944 7261 676f 6e4c  .QSO.....DragonL
+00003090: 6f67 0103 0000 0048 0051 0053 004f 002d  og.....H.Q.S.O.-
+000030a0: 004c 006f 0067 0020 0028 002a 002e 0071  .L.o.g. .(.*...q
+000030b0: 006c 006f 0067 0029 003b 003b 0041 006c  .l.o.g.).;.;.A.l
+000030c0: 006c 0065 0020 0044 0061 0074 0065 0069  .l.e. .D.a.t.e.i
+000030d0: 0065 006e 0020 0028 002a 002e 002a 0029  .e.n. .(.*...*.)
+000030e0: 0800 0000 0006 0000 0021 5153 4f2d 4c6f  .........!QSO-Lo
+000030f0: 6720 282a 2e71 6c6f 6729 3b3b 416c 6c20  g (*.qlog);;All 
+00003100: 4669 6c65 7320 282a 2e2a 2907 0000 0009  Files (*.*).....
+00003110: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00003120: 0000 0000 0600 0000 0351 5448 0700 0000  .........QTH....
+00003130: 0944 7261 676f 6e4c 6f67 0103 0000 0012  .DragonLog......
+00003140: 0052 0053 0054 0020 0065 006d 0070 0066  .R.S.T. .e.m.p.f
+00003150: 002e 0800 0000 0006 0000 0008 5253 5420  ............RST 
+00003160: 7263 7664 0700 0000 0944 7261 676f 6e4c  rcvd.....DragonL
+00003170: 6f67 0103 0000 0010 0052 0053 0054 0020  og.......R.S.T. 
+00003180: 0067 0065 0073 002e 0800 0000 0006 0000  .g.e.s..........
+00003190: 0008 5253 5420 7365 6e74 0700 0000 0944  ..RST sent.....D
+000031a0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+000031b0: 0000 0006 0000 0005 5261 6469 6f07 0000  ........Radio...
+000031c0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000031d0: 1800 5200 6100 6900 6e00 2d00 5300 6300  ..R.a.i.n.-.S.c.
+000031e0: 6100 7400 7400 6500 7208 0000 0000 0600  a.t.t.e.r.......
+000031f0: 0000 0c52 6169 6e20 7363 6174 7465 7207  ...Rain scatter.
+00003200: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00003210: 0000 3200 5200 6500 7000 6500 6100 7400  ..2.R.e.p.e.a.t.
+00003220: 6500 7200 2000 6f00 6400 6500 7200 2000  e.r. .o.d.e.r. .
+00003230: 5400 7200 6100 6e00 7300 7000 6f00 6e00  T.r.a.n.s.p.o.n.
+00003240: 6400 6500 7208 0000 0000 0600 0000 1752  d.e.r..........R
+00003250: 6570 6561 7465 7220 6f72 2054 7261 6e73  epeater or Trans
+00003260: 706f 6e64 6572 0700 0000 0944 7261 676f  ponder.....Drago
+00003270: 6e4c 6f67 0103 0000 0010 0053 0061 0074  nLog.......S.a.t
+00003280: 0065 006c 006c 0069 0074 0800 0000 0006  .e.l.l.i.t......
+00003290: 0000 0009 5361 7465 6c6c 6974 6507 0000  ....Satellite...
+000032a0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000032b0: 2a00 4500 7800 7000 6f00 7200 7400 6400  *.E.x.p.o.r.t.d.
+000032c0: 6100 7400 6500 6900 2000 7300 7000 6500  a.t.e.i. .s.p.e.
+000032d0: 6900 6300 6800 6500 7200 6e08 0000 0000  i.c.h.e.r.n.....
+000032e0: 0600 0000 1253 656c 6563 7420 6578 706f  .....Select expo
+000032f0: 7274 2066 696c 6507 0000 0009 4472 6167  rt file.....Drag
+00003300: 6f6e 4c6f 6701 0300 0000 2000 4400 6100  onLog..... .D.a.
+00003310: 7400 6500 6e00 6200 6100 6e00 6b00 2000  t.e.n.b.a.n.k. .
+00003320: f600 6600 6600 6e00 6500 6e08 0000 0000  ..f.f.n.e.n.....
+00003330: 0600 0000 0b53 656c 6563 7420 6669 6c65  .....Select file
+00003340: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003350: 0000 0038 005a 0075 0020 00fc 0062 0065  ...8.Z.u. ...b.e
+00003360: 0072 0077 0061 0063 0068 0065 006e 0064  .r.w.a.c.h.e.n.d
+00003370: 0065 0020 0044 0061 0074 0065 0069 0020  .e. .D.a.t.e.i. 
+00003380: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
+00003390: 0006 0000 0014 5365 6c65 6374 2066 696c  ......Select fil
+000033a0: 6520 746f 2077 6174 6368 0700 0000 0944  e to watch.....D
+000033b0: 7261 676f 6e4c 6f67 0103 0000 0024 0049  ragonLog.....$.I
+000033c0: 006d 0070 006f 0072 0074 0064 0061 0074  .m.p.o.r.t.d.a.t
+000033d0: 0065 0069 0020 00f6 0066 0066 006e 0065  .e.i. ...f.f.n.e
+000033e0: 006e 0800 0000 0006 0000 0012 5365 6c65  .n..........Sele
+000033f0: 6374 2069 6d70 6f72 7420 6669 6c65 0700  ct import file..
+00003400: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003410: 001a 0057 00e4 0068 006c 0065 0020 0053  ...W...h.l.e. .S
+00003420: 0074 0061 0074 0069 006f 006e 0800 0000  .t.a.t.i.o.n....
+00003430: 0006 0000 000e 5365 6c65 6374 2073 7461  ......Select sta
+00003440: 7469 6f6e 0700 0000 0944 7261 676f 6e4c  tion.....DragonL
+00003450: 6f67 0103 0000 0044 004c 006f 0054 0057  og.....D.L.o.T.W
+00003460: 002d 0053 0065 0072 0076 0065 0072 0020  .-.S.e.r.v.e.r. 
+00003470: 0068 0061 0074 0020 0064 0061 0073 0020  .h.a.t. .d.a.s. 
+00003480: 004c 006f 0067 0020 0061 0062 0067 0065  .L.o.g. .a.b.g.e
+00003490: 0077 0069 0065 0073 0065 006e 0800 0000  .w.i.e.s.e.n....
+000034a0: 0006 0000 0013 5365 7276 6572 2072 656a  ......Server rej
+000034b0: 6563 7465 6420 6c6f 6707 0000 0009 4472  ected log.....Dr
+000034c0: 6167 6f6e 4c6f 6701 0300 0000 1400 7a00  agonLog.......z.
+000034d0: 6500 6900 6700 6500 2000 6100 6c00 6c00  e.i.g.e. .a.l.l.
+000034e0: 6508 0000 0000 0600 0000 0853 686f 7720  e..........Show 
+000034f0: 616c 6c07 0000 0009 4472 6167 6f6e 4c6f  all.....DragonLo
+00003500: 6701 0300 0000 1400 5300 7000 6f00 7200  g.......S.p.o.r.
+00003510: 6100 6400 6900 6300 2d00 4508 0000 0000  a.d.i.c.-.E.....
+00003520: 0600 0000 0a53 706f 7261 6469 6320 4507  .....Sporadic E.
+00003530: 0000 0009 4472 6167 6f6e 4c6f 6701 03ff  ....DragonLog...
+00003540: ffff ff08 0000 0000 0600 0000 0753 7562  .............Sub
+00003550: 6d6f 6465 0700 0000 0944 7261 676f 6e4c  mode.....DragonL
+00003560: 6f67 0103 0000 002a 0054 0051 0053 004c  og.....*.T.Q.S.L
+00003570: 002d 0053 0069 0067 006e 0061 0074 0075  .-.S.i.g.n.a.t.u
+00003580: 0072 0070 0061 0073 0073 0077 006f 0072  .r.p.a.s.s.w.o.r
+00003590: 0074 0800 0000 0006 0000 0017 5451 534c  .t..........TQSL
+000035a0: 2073 6967 6e61 7475 7265 2070 6173 7377   signature passw
+000035b0: 6f72 6407 0000 0009 4472 6167 6f6e 4c6f  ord.....DragonLo
+000035c0: 6701 0300 0000 b200 4400 6900 6500 2000  g.......D.i.e. .
+000035d0: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
+000035e0: 6b00 7300 7400 7200 7500 6b00 7400 7500  k.s.t.r.u.k.t.u.
+000035f0: 7200 2000 6900 7300 7400 2000 7600 6500  r. .i.s.t. .v.e.
+00003600: 7200 6100 6c00 7400 6500 7400 2000 7500  r.a.l.t.e.t. .u.
+00003610: 6e00 6400 2000 6d00 7500 7300 7300 2000  n.d. .m.u.s.s. .
+00003620: 6b00 6f00 6e00 7600 6500 7200 7400 6900  k.o.n.v.e.r.t.i.
+00003630: 6500 7200 7400 2000 7700 6500 7200 6400  e.r.t. .w.e.r.d.
+00003640: 6500 6e00 0a00 0a00 4500 6900 6e00 2000  e.n.....E.i.n. .
+00003650: 4200 6100 6300 6b00 7500 7000 2000 7700  B.a.c.k.u.p. .w.
+00003660: 6900 7200 6400 2000 6500 7200 7300 7400  i.r.d. .e.r.s.t.
+00003670: 6500 6c00 6c00 7400 3a08 0000 0000 0600  e.l.l.t.:.......
+00003680: 0000 5754 6865 2064 6174 6162 6173 6520  ..WThe database 
+00003690: 7374 7275 6374 7572 6520 6973 206f 7574  structure is out
+000036a0: 2d64 6174 6564 2061 6e64 206e 6565 6473  -dated and needs
+000036b0: 2061 2063 6f6e 7665 7273 696f 6e0a 0a41   a conversion..A
+000036c0: 2062 6163 6b75 7020 7769 6c6c 2062 6520   backup will be 
+000036d0: 6765 6e65 7261 7465 643a 0700 0000 0944  generated:.....D
+000036e0: 7261 676f 6e4c 6f67 0103 0000 001e 0054  ragonLog.......T
+000036f0: 0072 0061 006e 0073 0065 0071 0075 0061  .r.a.n.s.e.q.u.a
+00003700: 0074 006f 0072 0069 0061 006c 0800 0000  .t.o.r.i.a.l....
+00003710: 0006 0000 0010 5472 616e 732d 6571 7561  ......Trans-equa
+00003720: 746f 7269 616c 0700 0000 0944 7261 676f  torial.....Drago
+00003730: 6e4c 6f67 0103 0000 0028 0054 0072 006f  nLog.....(.T.r.o
+00003740: 0070 006f 0073 0070 0068 0065 0072 0069  .p.o.s.p.h.e.r.i
+00003750: 0063 002d 0044 0075 0063 0074 0069 006e  .c.-.D.u.c.t.i.n
+00003760: 0067 0800 0000 0006 0000 0014 5472 6f70  .g..........Trop
+00003770: 6f73 7068 6572 6963 2064 7563 7469 6e67  ospheric ducting
+00003780: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003790: ffff ffff 0800 0000 0006 0000 0007 5665  ..............Ve
+000037a0: 7273 696f 6e07 0000 0009 4472 6167 6f6e  rsion.....Dragon
+000037b0: 4c6f 6701 0300 0000 2c00 5000 7200 6f00  Log.....,.P.r.o.
+000037c0: 6700 7200 6100 6d00 6d00 6c00 6f00 6700  g.r.a.m.m.l.o.g.
+000037d0: 2000 fc00 6200 6500 7200 7700 6100 6300   ...b.e.r.w.a.c.
+000037e0: 6800 6500 6e08 0000 0000 0600 0000 1557  h.e.n..........W
+000037f0: 6174 6368 2061 7070 6c69 6361 7469 6f6e  atch application
+00003800: 206c 6f67 0700 0000 0944 7261 676f 6e4c   log.....DragonL
+00003810: 6f67 0103 0000 0020 0044 0061 0074 0065  og..... .D.a.t.e
+00003820: 0069 00fc 0062 0065 0072 0077 0061 0063  .i...b.e.r.w.a.c
+00003830: 0068 0075 006e 0067 0800 0000 0006 0000  .h.u.n.g........
+00003840: 000d 5761 7463 6869 6e67 2066 696c 6507  ..Watching file.
+00003850: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00003860: 0000 1400 6500 5100 5300 4c00 2000 6500  ....e.Q.S.L. .e.
+00003870: 6d00 7000 6600 2e08 0000 0000 0600 0000  m.p.f...........
+00003880: 0965 5153 4c20 7263 7664 0700 0000 0944  .eQSL rcvd.....D
+00003890: 7261 676f 6e4c 6f67 0103 0000 0014 0065  ragonLog.......e
+000038a0: 0051 0053 004c 0020 0076 0065 0072 0073  .Q.S.L. .v.e.r.s
+000038b0: 002e 0800 0000 0006 0000 0009 6551 534c  ............eQSL
+000038c0: 2073 656e 7407 0000 0009 4472 6167 6f6e   sent.....Dragon
+000038d0: 4c6f 6701 0300 0000 0e00 6900 6e00 6100  Log.......i.n.a.
+000038e0: 6b00 7400 6900 7608 0000 0000 0600 0000  k.t.i.v.........
+000038f0: 0769 6e61 6374 6976 0700 0000 0944 7261  .inactiv.....Dra
+00003900: 676f 6e4c 6f67 0103 0000 0008 00dc 0062  gonLog.........b
+00003910: 0065 0072 0800 0000 0006 0000 0005 4162  .e.r..........Ab
+00003920: 6f75 7407 0000 000a 4d61 696e 5769 6e64  out.....MainWind
+00003930: 6f77 0103 0000 000e 00dc 0062 0065 0072  ow.........b.e.r
+00003940: 0020 0051 0074 0800 0000 0006 0000 0008  . .Q.t..........
+00003950: 4162 6f75 7420 5174 0700 0000 0a4d 6169  About Qt.....Mai
+00003960: 6e57 696e 646f 7701 0300 0000 1a00 4100  nWindow.......A.
+00003970: 6e00 7700 6500 6e00 6400 7500 6e00 6700  n.w.e.n.d.u.n.g.
+00003980: 7300 6c00 6f00 6708 0000 0000 0600 0000  s.l.o.g.........
+00003990: 0f41 7070 6c69 6361 7469 6f6e 204c 6f67  .Application Log
+000039a0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+000039b0: 0300 0000 2200 4500 6900 6e00 7400 7200  ....".E.i.n.t.r.
+000039c0: 6100 6700 2000 e400 6e00 6400 6500 7200  a.g. ...n.d.e.r.
+000039d0: 6e00 2e00 2e00 2e08 0000 0000 0600 0000  n...............
+000039e0: 1343 6861 6e67 6520 6c6f 6720 656e 7472  .Change log entr
+000039f0: 792e 2e2e 0700 0000 0a4d 6169 6e57 696e  y........MainWin
+00003a00: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
+00003a10: 0000 0643 7472 6c2b 4507 0000 000a 4d61  ...Ctrl+E.....Ma
+00003a20: 696e 5769 6e64 6f77 0103 ffff ffff 0800  inWindow........
+00003a30: 0000 0006 0000 0006 4374 726c 2b4c 0700  ........Ctrl+L..
+00003a40: 0000 0a4d 6169 6e57 696e 646f 7701 03ff  ...MainWindow...
+00003a50: ffff ff08 0000 0000 0600 0000 0643 7472  .............Ctr
+00003a60: 6c2b 5107 0000 000a 4d61 696e 5769 6e64  l+Q.....MainWind
+00003a70: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00003a80: 0006 4374 726c 2b57 0700 0000 0a4d 6169  ..Ctrl+W.....Mai
+00003a90: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
+00003aa0: 0000 0600 0000 0643 7472 6c2b 5807 0000  .......Ctrl+X...
+00003ab0: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
+00003ac0: 001e 0045 0069 006e 0074 0072 0061 0067  ...E.i.n.t.r.a.g
+00003ad0: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
+00003ae0: 0800 0000 0006 0000 0010 4465 6c65 7465  ..........Delete
+00003af0: 206c 6f67 2065 6e74 7279 0700 0000 0a4d   log entry.....M
+00003b00: 6169 6e57 696e 646f 7701 03ff ffff ff08  ainWindow.......
+00003b10: 0000 0000 0600 0000 0944 7261 676f 6e4c  .........DragonL
+00003b20: 6f67 0700 0000 0a4d 6169 6e57 696e 646f  og.....MainWindo
+00003b30: 7701 0300 0000 1400 4200 6500 6100 7200  w.......B.e.a.r.
+00003b40: 6200 6500 6900 7400 6500 6e08 0000 0000  b.e.i.t.e.n.....
+00003b50: 0600 0000 0445 6469 7407 0000 000a 4d61  .....Edit.....Ma
+00003b60: 696e 5769 6e64 6f77 0103 0000 000e 0042  inWindow.......B
+00003b70: 0065 0065 006e 0064 0065 006e 0800 0000  .e.e.n.d.e.n....
+00003b80: 0006 0000 0004 4578 6974 0700 0000 0a4d  ......Exit.....M
+00003b90: 6169 6e57 696e 646f 7701 03ff ffff ff08  ainWindow.......
+00003ba0: 0000 0000 0600 0000 0645 7870 6f72 7407  .........Export.
+00003bb0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00003bc0: 0000 001c 0045 0078 0070 006f 0072 0074  .....E.x.p.o.r.t
+00003bd0: 0069 0065 0072 0065 006e 002e 002e 002e  .i.e.r.e.n......
+00003be0: 0800 0000 0006 0000 0009 4578 706f 7274  ..........Export
+00003bf0: 2e2e 2e07 0000 000a 4d61 696e 5769 6e64  ........MainWind
+00003c00: 6f77 0103 0000 000a 0044 0061 0074 0065  ow.......D.a.t.e
+00003c10: 0069 0800 0000 0006 0000 0004 4669 6c65  .i..........File
+00003c20: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003c30: 0300 0000 0a00 4800 6900 6c00 6600 6508  ......H.i.l.f.e.
+00003c40: 0000 0000 0600 0000 0448 656c 7007 0000  .........Help...
+00003c50: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
+00003c60: ffff 0800 0000 0006 0000 0006 496d 706f  ............Impo
+00003c70: 7274 0700 0000 0a4d 6169 6e57 696e 646f  rt.....MainWindo
+00003c80: 7701 0300 0000 1c00 4900 6d00 7000 6f00  w.......I.m.p.o.
+00003c90: 7200 7400 6900 6500 7200 6500 6e00 2e00  r.t.i.e.r.e.n...
+00003ca0: 2e00 2e08 0000 0000 0600 0000 0949 6d70  .............Imp
+00003cb0: 6f72 742e 2e2e 0700 0000 0a4d 6169 6e57  ort........MainW
+00003cc0: 696e 646f 7701 0300 0000 1800 4c00 6f00  indow.......L.o.
+00003cd0: 6700 6700 6500 2000 5100 5300 4f00 2e00  g.g.e. .Q.S.O...
+00003ce0: 2e00 2e08 0000 0000 0600 0000 0a4c 6f67  .............Log
+00003cf0: 2051 534f 2e2e 2e07 0000 000a 4d61 696e   QSO........Main
+00003d00: 5769 6e64 6f77 0103 0000 0018 0051 0053  Window.......Q.S
+00003d10: 004f 002d 0046 006f 0072 006d 0075 006c  .O.-.F.o.r.m.u.l
+00003d20: 0061 0072 0800 0000 0006 0000 0008 5153  .a.r..........QS
+00003d30: 4f20 466f 726d 0700 0000 0a4d 6169 6e57  O Form.....MainW
+00003d40: 696e 646f 7701 0300 0000 2600 4400 6100  indow.....&.D.a.
+00003d50: 7400 6500 6e00 6200 6100 6e00 6b00 2000  t.e.n.b.a.n.k. .
+00003d60: 7700 e400 6800 6c00 6500 6e00 2e00 2e00  w...h.l.e.n.....
+00003d70: 2e08 0000 0000 0600 0000 1253 656c 6563  ...........Selec
+00003d80: 7420 6461 7461 6261 7365 2e2e 2e07 0000  t database......
+00003d90: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
+00003da0: 001a 0045 0069 006e 0073 0074 0065 006c  ...E.i.n.s.t.e.l
+00003db0: 006c 0075 006e 0067 0065 006e 0800 0000  .l.u.n.g.e.n....
+00003dc0: 0006 0000 0008 5365 7474 696e 6773 0700  ......Settings..
+00003dd0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
+00003de0: 0000 2600 5a00 6500 6900 6700 6500 2000  ..&.Z.e.i.g.e. .
+00003df0: 4100 6e00 7700 6500 6e00 6400 7500 6e00  A.n.w.e.n.d.u.n.
+00003e00: 6700 7300 6c00 6f00 6708 0000 0000 0600  g.s.l.o.g.......
+00003e10: 0000 0853 686f 7720 6c6f 6707 0000 000a  ...Show log.....
+00003e20: 4d61 696e 5769 6e64 6f77 0103 0000 001a  MainWindow......
+00003e30: 0053 0074 0061 0072 0074 0065 0020 0048  .S.t.a.r.t.e. .H
+00003e40: 0061 006d 006c 0069 0062 0800 0000 0006  .a.m.l.i.b......
+00003e50: 0000 000c 5374 6172 7420 6861 6d6c 6962  ....Start hamlib
+00003e60: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003e70: 0300 0000 1c00 5700 6500 7200 6b00 7a00  ......W.e.r.k.z.
+00003e80: 6500 7500 6700 6c00 6500 6900 7300 7400  e.u.g.l.e.i.s.t.
+00003e90: 6508 0000 0000 0600 0000 0754 6f6f 6c62  e..........Toolb
+00003ea0: 6172 0700 0000 0a4d 6169 6e57 696e 646f  ar.....MainWindo
+00003eb0: 7701 0300 0000 3200 4c00 6f00 6700 7300  w.....2.L.o.g.s.
+00003ec0: 2000 7a00 7500 2000 4c00 6f00 5400 5700   .z.u. .L.o.T.W.
+00003ed0: 2000 6800 6f00 6300 6800 6c00 6100 6400   .h.o.c.h.l.a.d.
+00003ee0: 6500 6e00 2e00 2e00 2e08 0000 0000 0600  e.n.............
+00003ef0: 0000 1655 706c 6f61 6420 6c6f 6773 2074  ...Upload logs t
+00003f00: 6f20 4c6f 5457 2e2e 2e07 0000 000a 4d61  o LoTW........Ma
+00003f10: 696e 5769 6e64 6f77 0103 0000 0042 0044  inWindow.....B.D
+00003f20: 0061 0074 0065 0069 0020 0061 0075 0066  .a.t.e.i. .a.u.f
+00003f30: 0020 006e 0065 0075 0065 0020 0051 0053  . .n.e.u.e. .Q.S
+00003f40: 004f 0073 0020 00fc 0062 0065 0072 0077  .O.s. ...b.e.r.w
+00003f50: 0061 0063 0068 0065 006e 002e 002e 002e  .a.c.h.e.n......
+00003f60: 0800 0000 0006 0000 0016 5761 7463 6820  ..........Watch 
+00003f70: 6669 6c65 2066 6f72 2051 534f 732e 2e2e  file for QSOs...
+00003f80: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003f90: 03ff ffff ff08 0000 0000 0600 0000 0220  ............... 
+00003fa0: 5707 0000 0007 5153 4f46 6f72 6d01 03ff  W.....QSOForm...
+00003fb0: ffff ff08 0000 0000 0600 0000 0420 6b48  ............. kH
+00003fc0: 7a07 0000 0007 5153 4f46 6f72 6d01 03ff  z.....QSOForm...
+00003fd0: ffff ff08 0000 0000 0600 0000 0235 3907  .............59.
+00003fe0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00003ff0: 4800 4500 6900 6e00 2000 4600 6500 6c00  H.E.i.n. .F.e.l.
+00004000: 6400 2000 6600 6500 6800 6c00 7400 2000  d. .f.e.h.l.t. .
+00004010: 6600 fc00 7200 2000 6400 6900 6500 2000  f...r. .d.i.e. .
+00004020: 4900 6e00 6200 6f00 7800 2d00 5000 7200  I.n.b.o.x.-.P.r.
+00004030: fc00 6600 7500 6e00 6708 0000 0000 0600  ..f.u.n.g.......
+00004040: 0000 2241 2066 6965 6c64 2069 7320 6d69  .."A field is mi
+00004050: 7373 696e 6720 666f 7220 696e 626f 7820  ssing for inbox 
+00004060: 6368 6563 6b07 0000 0007 5153 4f46 6f72  check.....QSOFor
+00004070: 6d01 0300 0000 4200 4600 6500 6800 6c00  m.....B.F.e.h.l.
+00004080: 6500 6e00 6400 6500 7300 2000 4600 6500  e.n.d.e.s. .F.e.
+00004090: 6c00 6400 2000 6600 fc00 7200 2000 6400  l.d. .f...r. .d.
+000040a0: 6500 6e00 2000 4c00 6f00 6700 2d00 5500  e.n. .L.o.g.-.U.
+000040b0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
+000040c0: 0000 2141 2066 6965 6c64 2069 7320 6d69  ..!A field is mi
+000040d0: 7373 696e 6720 666f 7220 6c6f 6720 7570  ssing for log up
+000040e0: 6c6f 6164 0700 0000 0751 534f 466f 726d  load.....QSOForm
+000040f0: 0103 0000 0056 0046 0065 0068 006c 0065  .....V.F.e.h.l.e
+00004100: 006e 0064 0065 0073 0020 0046 0065 006c  .n.d.e.s. .F.e.l
+00004110: 0064 0020 0066 00fc 0072 0020 0064 0065  .d. .f...r. .d.e
+00004120: 006e 0020 004c 006f 0067 002d 0055 0070  .n. .L.o.g.-.U.p
+00004130: 006c 006f 0061 0064 0020 007a 0075 0020  .l.o.a.d. .z.u. 
+00004140: 0048 0061 006d 0051 0054 0048 0800 0000  .H.a.m.Q.T.H....
+00004150: 0006 0000 002b 4120 6669 656c 6420 6973  .....+A field is
+00004160: 206d 6973 7369 6e67 2066 6f72 206c 6f67   missing for log
+00004170: 2075 706c 6f61 6420 746f 2048 616d 5154   upload to HamQT
+00004180: 4807 0000 0007 5153 4f46 6f72 6d01 0300  H.....QSOForm...
+00004190: 0000 1600 4100 6b00 7a00 6500 7000 7400  ....A.k.z.e.p.t.
+000041a0: 6900 6500 7200 7400 3a08 0000 0000 0600  i.e.r.t.:.......
+000041b0: 0000 0841 6363 6570 7473 3a07 0000 0007  ...Accepts:.....
+000041c0: 5153 4f46 6f72 6d01 0300 0000 6a00 4500  QSOForm.....j.E.
+000041d0: 6900 6e00 2000 4600 6500 6800 6c00 6500  i.n. .F.e.h.l.e.
+000041e0: 7200 2000 7400 7200 6100 7400 2000 7700  r. .t.r.a.t. .w.
+000041f0: e400 6800 7200 6500 6e00 6400 2000 6400  ..h.r.e.n.d. .d.
+00004200: 6500 7200 2000 dc00 6200 6500 7200 7400  e.r. ...b.e.r.t.
+00004210: 7200 6100 6700 7500 6e00 6700 2000 7a00  r.a.g.u.n.g. .z.
+00004220: 7500 2000 4800 6100 6d00 5100 5400 4800  u. .H.a.m.Q.T.H.
+00004230: 2000 6100 7500 6608 0000 0000 0600 0000   .a.u.f.........
+00004240: 2741 6e20 6572 726f 7220 6f63 6375 7265  'An error occure
+00004250: 6420 6f6e 2075 706c 6f61 6469 6e67 2074  d on uploading t
+00004260: 6f20 4861 6d51 5448 0700 0000 0751 534f  o HamQTH.....QSO
+00004270: 466f 726d 0103 0000 000e 0041 006e 0074  Form.......A.n.t
+00004280: 0065 006e 006e 0065 0800 0000 0006 0000  .e.n.n.e........
+00004290: 0007 416e 7465 6e6e 6107 0000 0007 5153  ..Antenna.....QS
+000042a0: 4f46 6f72 6d01 0300 0000 1600 4100 7500  OForm.......A.u.
+000042b0: 7400 6f00 6d00 6100 7400 6900 7300 6300  t.o.m.a.t.i.s.c.
+000042c0: 6808 0000 0000 0600 0000 0d41 7574 6f6d  h..........Autom
+000042d0: 6174 6963 616c 6c79 0700 0000 0751 534f  atically.....QSO
+000042e0: 466f 726d 0103 0000 0038 0046 0065 0068  Form.....8.F.e.h
+000042f0: 006c 0065 0072 0068 0061 0066 0074 0065  .l.e.r.h.a.f.t.e
+00004300: 0073 0020 0041 0062 0066 0072 0061 0067  .s. .A.b.f.r.a.g
+00004310: 0065 0065 0072 0067 0065 0062 006e 0069  .e.e.r.g.e.b.n.i
+00004320: 0073 0800 0000 0006 0000 0012 4261 6420  .s..........Bad 
+00004330: 7265 7175 6573 7420 7265 7375 6c74 0700  request result..
+00004340: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00004350: 0800 0000 0006 0000 0004 4261 6e64 0700  ..........Band..
+00004360: 0000 0751 534f 466f 726d 0103 0000 0008  ...QSOForm......
+00004370: 0042 00fc 0072 006f 0800 0000 0006 0000  .B...r.o........
+00004380: 0006 4275 7265 6175 0700 0000 0751 534f  ..Bureau.....QSO
+00004390: 466f 726d 0103 0000 0016 0042 00fc 0072  Form.......B...r
+000043a0: 006f 002f 0044 0069 0072 0065 006b 0074  .o./.D.i.r.e.k.t
+000043b0: 0800 0000 0006 0000 000d 4275 7265 6175  ..........Bureau
+000043c0: 2f44 6972 6563 7407 0000 0007 5153 4f46  /Direct.....QSOF
+000043d0: 6f72 6d01 0300 0000 1400 5200 7500 6600  orm.......R.u.f.
+000043e0: 7a00 6500 6900 6300 6800 6500 6e08 0000  z.e.i.c.h.e.n...
+000043f0: 0000 0600 0000 0943 616c 6c20 7369 676e  .......Call sign
+00004400: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004410: 003c 0046 0065 0068 006c 0065 0072 0020  .<.F.e.h.l.e.r. 
+00004420: 0062 0065 0069 0020 0064 0065 0072 0020  .b.e.i. .d.e.r. 
+00004430: 0052 0075 0066 007a 0065 0069 0063 0068  .R.u.f.z.e.i.c.h
+00004440: 0065 006e 0073 0075 0063 0068 0065 0800  .e.n.s.u.c.h.e..
+00004450: 0000 0006 0000 0015 4361 6c6c 626f 6f6b  ........Callbook
+00004460: 2073 6561 7263 6820 6572 726f 7207 0000   search error...
+00004470: 0007 5153 4f46 6f72 6d01 0300 0000 2a00  ..QSOForm.....*.
+00004480: 4300 6100 6c00 6c00 6200 6f00 6f00 6b00  C.a.l.l.b.o.o.k.
+00004490: 2d00 5300 7500 6300 6800 6500 7200 6700  -.S.u.c.h.e.r.g.
+000044a0: 6500 6200 6e00 6900 7308 0000 0000 0600  e.b.n.i.s.......
+000044b0: 0000 1643 616c 6c62 6f6f 6b20 7365 6172  ...Callbook sear
+000044c0: 6368 2072 6573 756c 7407 0000 0007 5153  ch result.....QS
+000044d0: 4f46 6f72 6d01 0300 0000 3200 5200 7500  OForm.....2.R.u.
+000044e0: 6600 7a00 6500 6900 6300 6800 6500 6e00  f.z.e.i.c.h.e.n.
+000044f0: 2000 6e00 6900 6300 6800 7400 2000 6700   .n.i.c.h.t. .g.
+00004500: 6500 6600 7500 6e00 6400 6500 6e08 0000  e.f.u.n.d.e.n...
+00004510: 0000 0600 0000 1243 616c 6c73 6967 6e20  .......Callsign 
+00004520: 6e6f 7420 666f 756e 6407 0000 0007 5153  not found.....QS
+00004530: 4f46 6f72 6d01 0300 0000 0a00 4b00 6100  OForm.......K.a.
+00004540: 6e00 6100 6c08 0000 0000 0600 0000 0743  n.a.l..........C
+00004550: 6861 6e6e 656c 0700 0000 0751 534f 466f  hannel.....QSOFo
+00004560: 726d 0103 0000 0016 0050 0072 00fc 0066  rm.......P.r...f
+00004570: 0065 0020 0049 006e 0062 006f 0078 0800  .e. .I.n.b.o.x..
+00004580: 0000 0006 0000 000b 4368 6563 6b20 496e  ........Check In
+00004590: 626f 7807 0000 0007 5153 4f46 6f72 6d01  box.....QSOForm.
+000045a0: 0300 0000 4200 4600 6500 6800 6c00 6500  ....B.F.e.h.l.e.
+000045b0: 7200 2000 6200 6500 6900 6d00 2000 5000  r. .b.e.i.m. .P.
+000045c0: 7200 fc00 6600 6500 6e00 2000 6400 6500  r...f.e.n. .d.e.
+000045d0: 7200 2000 4c00 6f00 5400 5700 2d00 4900  r. .L.o.T.W.-.I.
+000045e0: 6e00 6200 6f00 7808 0000 0000 0600 0000  n.b.o.x.........
+000045f0: 1643 6865 636b 204c 6f54 5720 496e 626f  .Check LoTW Inbo
+00004600: 7820 6572 726f 7207 0000 0007 5153 4f46  x error.....QSOF
+00004610: 6f72 6d01 0300 0000 1c00 5000 7200 fc00  orm.......P.r...
+00004620: 6600 6500 2000 4c00 6f00 5400 5700 2000  f.e. .L.o.T.W. .
+00004630: 5100 5300 4c08 0000 0000 0600 0000 0e43  Q.S.L..........C
+00004640: 6865 636b 204c 6f54 5720 5153 4c07 0000  heck LoTW QSL...
+00004650: 0007 5153 4f46 6f72 6d01 0300 0000 3800  ..QSOForm.....8.
+00004660: 6500 5100 5300 4c00 2d00 4600 6500 6800  e.Q.S.L.-.F.e.h.
+00004670: 6c00 6500 7200 2000 7000 7200 fc00 6600  l.e.r. .p.r...f.
+00004680: 6500 6e00 2000 6400 6500 7200 2000 4900  e.n. .d.e.r. .I.
+00004690: 6e00 6200 6f00 7808 0000 0000 0600 0000  n.b.o.x.........
+000046a0: 1643 6865 636b 2065 5153 4c20 496e 626f  .Check eQSL Inbo
+000046b0: 7820 6572 726f 7207 0000 0007 5153 4f46  x error.....QSOF
+000046c0: 6f72 6d01 0300 0000 1800 5a00 7500 7200  orm.......Z.u.r.
+000046d0: fc00 6300 6b00 7300 6500 7400 7a00 6500  ..c.k.s.e.t.z.e.
+000046e0: 6e08 0000 0000 0600 0000 0543 6c65 6172  n..........Clear
+000046f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004700: 0020 004b 006f 006e 0066 0069 0067 0075  . .K.o.n.f.i.g.u
+00004710: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
+00004720: 0044 0800 0000 0006 0000 0013 436f 6e66  .D..........Conf
+00004730: 6967 7572 6564 2069 6465 6e74 6974 7907  igured identity.
+00004740: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00004750: 2a00 4b00 6f00 6e00 6600 6900 6700 7500  *.K.o.n.f.i.g.u.
+00004760: 7200 6900 6500 7200 7400 6500 2000 5300  r.i.e.r.t.e. .S.
+00004770: 7400 6100 7400 6900 6f00 6e08 0000 0000  t.a.t.i.o.n.....
+00004780: 0600 0000 1243 6f6e 6669 6775 7265 6420  .....Configured 
+00004790: 7374 6174 696f 6e07 0000 0007 5153 4f46  station.....QSOF
+000047a0: 6f72 6d01 0300 0000 0c00 6400 6900 7200  orm.......d.i.r.
+000047b0: 6500 6b00 7408 0000 0000 0600 0000 0644  e.k.t..........D
+000047c0: 6972 6563 7407 0000 0007 5153 4f46 6f72  irect.....QSOFor
+000047d0: 6d01 0300 0000 1c00 6500 5100 5300 4c00  m.......e.Q.S.L.
+000047e0: 2000 7300 7000 6500 6900 6300 6800 6500   .s.p.e.i.c.h.e.
+000047f0: 7200 6e08 0000 0000 0600 0000 0d44 6f77  r.n..........Dow
+00004800: 6e6c 6f61 6420 6551 534c 0700 0000 0751  nload eQSL.....Q
+00004810: 534f 466f 726d 0103 0000 006c 0057 00e4  SOForm.....l.W..
+00004820: 0068 0072 0065 006e 0064 0020 0064 0065  .h.r.e.n.d. .d.e
+00004830: 0072 0020 0052 0075 0066 007a 0065 0069  .r. .R.u.f.z.e.i
+00004840: 0063 0068 0065 006e 0073 0075 0063 0068  .c.h.e.n.s.u.c.h
+00004850: 0065 0020 0069 0073 0074 0020 0065 0069  .e. .i.s.t. .e.i
+00004860: 006e 0020 0046 0065 0068 006c 0065 0072  .n. .F.e.h.l.e.r
+00004870: 0020 0061 0075 0066 0067 0065 0074 0072  . .a.u.f.g.e.t.r
+00004880: 0065 0074 0065 006e 0800 0000 0006 0000  .e.t.e.n........
+00004890: 0027 4475 7269 6e67 2063 616c 6c62 6f6f  .'During callboo
+000048a0: 6b20 7365 6172 6368 2061 6e20 6572 726f  k search an erro
+000048b0: 7220 6f63 6375 7265 6407 0000 0007 5153  r occured.....QS
+000048c0: 4f46 6f72 6d01 0300 0000 0800 4500 6e00  OForm.......E.n.
+000048d0: 6400 6508 0000 0000 0600 0000 0345 6e64  d.e..........End
+000048e0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+000048f0: 000c 0046 0065 0068 006c 0065 0072 0800  ...F.e.h.l.e.r..
+00004900: 0000 0006 0000 0005 4572 726f 7207 0000  ........Error...
+00004910: 0007 5153 4f46 6f72 6d01 0300 0000 2400  ..QSOForm.....$.
+00004920: 6500 5100 5300 4c00 2d00 5500 7000 6c00  e.Q.S.L.-.U.p.l.
+00004930: 6f00 6100 6400 2d00 4600 6500 6800 6c00  o.a.d.-.F.e.h.l.
+00004940: 6500 7208 0000 0000 0600 0000 0f45 7272  e.r..........Err
+00004950: 6f72 206f 6e20 7570 6c6f 6164 0700 0000  or on upload....
+00004960: 0751 534f 466f 726d 0103 0000 0010 0046  .QSOForm.......F
+00004970: 0072 0065 0071 0075 0065 006e 007a 0800  .r.e.q.u.e.n.z..
+00004980: 0000 0006 0000 0009 4672 6571 7565 6e63  ........Frequenc
+00004990: 7907 0000 0007 5153 4f46 6f72 6d01 03ff  y.....QSOForm...
+000049a0: ffff ff08 0000 0000 0600 0000 0648 616d  .............Ham
+000049b0: 5154 4807 0000 0007 5153 4f46 6f72 6d01  QTH.....QSOForm.
+000049c0: 0300 0000 0400 4900 4408 0000 0000 0600  ......I.D.......
+000049d0: 0000 0849 6465 6e74 6974 7907 0000 0007  ...Identity.....
+000049e0: 5153 4f46 6f72 6d01 0300 0000 2600 4c00  QSOForm.....&.L.
+000049f0: 6900 6e00 6b00 2000 7a00 7500 7200 2000  i.n.k. .z.u.r. .
+00004a00: 6500 5100 5300 4c00 2d00 4b00 6100 7200  e.Q.S.L.-.K.a.r.
+00004a10: 7400 6508 0000 0000 0600 0000 114c 696e  t.e..........Lin
+00004a20: 6b20 746f 2065 5153 4c20 4361 7264 0700  k to eQSL Card..
+00004a30: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00004a40: 0800 0000 0006 0000 0004 4c6f 5457 0700  ..........LoTW..
+00004a50: 0000 0751 534f 466f 726d 0103 0000 001c  ...QSOForm......
+00004a60: 004c 006f 0054 0057 0020 0065 006d 0070  .L.o.T.W. .e.m.p
+00004a70: 0066 0061 006e 0067 0065 006e 0800 0000  .f.a.n.g.e.n....
+00004a80: 0006 0000 000d 4c6f 5457 2072 6563 6569  ......LoTW recei
+00004a90: 7665 6407 0000 0007 5153 4f46 6f72 6d01  ved.....QSOForm.
+00004aa0: 0300 0000 1c00 4c00 6f00 5400 5700 2000  ......L.o.T.W. .
+00004ab0: 7600 6500 7200 7300 6500 6e00 6400 6500  v.e.r.s.e.n.d.e.
+00004ac0: 7408 0000 0000 0600 0000 094c 6f54 5720  t..........LoTW 
+00004ad0: 7365 6e74 0700 0000 0751 534f 466f 726d  sent.....QSOForm
+00004ae0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+00004af0: 4c6f 6361 746f 7207 0000 0007 5153 4f46  Locator.....QSOF
+00004b00: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
+00004b10: 0000 074c 6f67 626f 6f6b 0700 0000 0751  ...Logbook.....Q
+00004b20: 534f 466f 726d 0103 0000 0042 004c 006f  SOForm.....B.L.o
+00004b30: 0067 0069 006e 0020 0066 0065 0068 006c  .g.i.n. .f.e.h.l
+00004b40: 0067 0065 0073 0063 0068 006c 0061 0067  .g.e.s.c.h.l.a.g
+00004b50: 0065 006e 0020 0066 00fc 0072 0020 0042  .e.n. .f...r. .B
+00004b60: 0065 006e 0075 0074 007a 0065 0072 0800  .e.n.u.t.z.e.r..
+00004b70: 0000 0006 0000 0015 4c6f 6769 6e20 6661  ........Login fa
+00004b80: 696c 6564 2066 6f72 2075 7365 7207 0000  iled for user...
+00004b90: 0007 5153 4f46 6f72 6d01 0300 0000 5800  ..QSOForm.....X.
+00004ba0: 4c00 6f00 6700 6900 6e00 2000 6200 6500  L.o.g.i.n. .b.e.
+00004bb0: 6900 2000 4800 6100 6d00 5100 5400 4800  i. .H.a.m.Q.T.H.
+00004bc0: 2000 6600 6500 6800 6c00 6700 6500 7300   .f.e.h.l.g.e.s.
+00004bd0: 6300 6800 6c00 6100 6700 6500 6e00 2000  c.h.l.a.g.e.n. .
+00004be0: 6600 fc00 7200 2000 4200 6500 6e00 7500  f...r. .B.e.n.u.
+00004bf0: 7400 7a00 6500 7208 0000 0000 0600 0000  t.z.e.r.........
+00004c00: 1f4c 6f67 696e 2074 6f20 4861 6d51 5448  .Login to HamQTH
+00004c10: 2066 6169 6c65 6420 666f 7220 7573 6572   failed for user
+00004c20: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004c30: 0014 0048 0061 0075 0070 0074 0064 0061  ...H.a.u.p.t.d.a
+00004c40: 0074 0065 006e 0800 0000 0006 0000 0009  .t.e.n..........
+00004c50: 4d61 696e 2064 6174 6107 0000 0007 5153  Main data.....QS
+00004c60: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00004c70: 0600 0000 044d 6f64 6507 0000 0007 5153  .....Mode.....QS
+00004c80: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00004c90: 0600 0000 044e 616d 6507 0000 0007 5153  .....Name.....QS
+00004ca0: 4f46 6f72 6d01 0300 0000 2400 4b00 6500  OForm.....$.K.e.
+00004cb0: 6900 6e00 2000 5100 5300 4c00 2000 7600  i.n. .Q.S.L. .v.
+00004cc0: 6500 7200 6600 fc00 6700 6200 6100 7208  e.r.f...g.b.a.r.
+00004cd0: 0000 0000 0600 0000 104e 6f20 5153 4c20  .........No QSL 
+00004ce0: 6176 6169 6c61 626c 6507 0000 0007 5153  available.....QS
+00004cf0: 4f46 6f72 6d01 0300 0000 2600 4b00 6500  OForm.....&.K.e.
+00004d00: 6900 6e00 2000 6500 5100 5300 4c00 2000  i.n. .e.Q.S.L. .
+00004d10: 7600 6500 7200 6600 fc00 6700 6200 6100  v.e.r.f...g.b.a.
+00004d20: 7208 0000 0000 0600 0000 114e 6f20 6551  r..........No eQ
+00004d30: 534c 2061 7661 696c 6162 6c65 0700 0000  SL available....
+00004d40: 0751 534f 466f 726d 0103 0000 000a 004a  .QSOForm.......J
+00004d50: 0065 0074 007a 0074 0800 0000 0006 0000  .e.t.z.t........
+00004d60: 0003 4e6f 7707 0000 0007 5153 4f46 6f72  ..Now.....QSOFor
+00004d70: 6d01 0300 0000 1600 4500 6900 6700 6500  m.......E.i.g.e.
+00004d80: 6e00 6500 7200 2000 5100 5400 4808 0000  n.e.r. .Q.T.H...
+00004d90: 0000 0600 0000 074f 776e 2051 5448 0700  .......Own QTH..
+00004da0: 0000 0751 534f 466f 726d 0103 0000 0024  ...QSOForm.....$
+00004db0: 0045 0069 0067 0065 006e 0065 0073 0020  .E.i.g.e.n.e.s. 
+00004dc0: 0052 0075 0066 007a 0065 0069 0063 0068  .R.u.f.z.e.i.c.h
+00004dd0: 0065 006e 0800 0000 0006 0000 000d 4f77  .e.n..........Ow
+00004de0: 6e20 6361 6c6c 2073 6967 6e07 0000 0007  n call sign.....
+00004df0: 5153 4f46 6f72 6d01 0300 0000 1e00 4500  QSOForm.......E.
+00004e00: 6900 6700 6500 6e00 6500 7200 2000 4c00  i.g.e.n.e.r. .L.
+00004e10: 6f00 6300 6100 7400 6f00 7208 0000 0000  o.c.a.t.o.r.....
+00004e20: 0600 0000 0b4f 776e 206c 6f63 6174 6f72  .....Own locator
+00004e30: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004e40: 0018 0045 0069 0067 0065 006e 0065 0072  ...E.i.g.e.n.e.r
+00004e50: 0020 004e 0061 006d 0065 0800 0000 0006  . .N.a.m.e......
+00004e60: 0000 0008 4f77 6e20 6e61 6d65 0700 0000  ....Own name....
+00004e70: 0751 534f 466f 726d 0103 0000 001c 0045  .QSOForm.......E
+00004e80: 0069 0067 0065 006e 0065 0020 004e 006f  .i.g.e.n.e. .N.o
+00004e90: 0074 0069 007a 0065 006e 0800 0000 0006  .t.i.z.e.n......
+00004ea0: 0000 0009 4f77 6e20 6e6f 7465 7307 0000  ....Own notes...
+00004eb0: 0007 5153 4f46 6f72 6d01 0300 0000 1000  ..QSOForm.......
+00004ec0: 4c00 6500 6900 7300 7400 7500 6e00 6708  L.e.i.s.t.u.n.g.
+00004ed0: 0000 0000 0600 0000 0550 6f77 6572 0700  .........Power..
+00004ee0: 0000 0751 534f 466f 726d 0103 0000 001e  ...QSOForm......
+00004ef0: 0041 0075 0073 0062 0072 0065 0069 0074  .A.u.s.b.r.e.i.t
+00004f00: 0075 006e 0067 0073 0061 0072 0074 0800  .u.n.g.s.a.r.t..
+00004f10: 0000 0006 0000 000b 5072 6f70 6167 6174  ........Propagat
+00004f20: 696f 6e07 0000 0007 5153 4f46 6f72 6d01  ion.....QSOForm.
+00004f30: 03ff ffff ff08 0000 0000 0600 0000 0551  ...............Q
+00004f40: 525a 4351 0700 0000 0751 534f 466f 726d  RZCQ.....QSOForm
+00004f50: 0103 ffff ffff 0800 0000 0006 0000 0003  ................
+00004f60: 5153 4c07 0000 0007 5153 4f46 6f72 6d01  QSL.....QSOForm.
+00004f70: 0300 0000 2200 5100 5300 4c00 2000 2600  ....".Q.S.L. .&.
+00004f80: 2600 2000 4c00 6f00 6700 2d00 5500 7000  &. .L.o.g.-.U.p.
+00004f90: 6c00 6f00 6100 6408 0000 0000 0600 0000  l.o.a.d.........
+00004fa0: 1151 534c 2026 2620 4c6f 6720 7570 6c6f  .QSL && Log uplo
+00004fb0: 6164 0700 0000 0751 534f 466f 726d 0103  ad.....QSOForm..
+00004fc0: 0000 001c 0051 0053 004c 002d 004b 0061  .....Q.S.L.-.K.a
+00004fd0: 0072 0074 0065 006e 0074 0065 0078 0074  .r.t.e.n.t.e.x.t
+00004fe0: 0800 0000 0006 0000 0010 5153 4c20 6361  ..........QSL ca
+00004ff0: 7264 206d 6573 7361 6765 0700 0000 0751  rd message.....Q
+00005000: 534f 466f 726d 0103 0000 001a 0051 0053  SOForm.......Q.S
+00005010: 004c 0020 0065 006d 0070 0066 0061 006e  .L. .e.m.p.f.a.n
+00005020: 0067 0065 006e 0800 0000 0006 0000 000c  .g.e.n..........
+00005030: 5153 4c20 7265 6365 6976 6564 0700 0000  QSL received....
+00005040: 0751 534f 466f 726d 0103 0000 0018 0051  .QSOForm.......Q
+00005050: 0053 004c 0020 0067 0065 0073 0065 006e  .S.L. .g.e.s.e.n
+00005060: 0064 0065 0074 0800 0000 0006 0000 0008  .d.e.t..........
+00005070: 5153 4c20 7365 6e74 0700 0000 0751 534f  QSL sent.....QSO
+00005080: 466f 726d 0103 0000 000e 0051 0053 004c  Form.......Q.S.L
+00005090: 002d 0056 0069 0061 0800 0000 0006 0000  .-.V.i.a........
+000050a0: 0007 5153 4c20 7669 6107 0000 0007 5153  ..QSL via.....QS
+000050b0: 4f46 6f72 6d01 0300 0000 1800 5100 5300  OForm.......Q.S.
+000050c0: 4f00 2d00 4600 6f00 7200 6d00 7500 6c00  O.-.F.o.r.m.u.l.
+000050d0: 6100 7208 0000 0000 0600 0000 0851 534f  a.r..........QSO
+000050e0: 2046 6f72 6d07 0000 0007 5153 4f46 6f72   Form.....QSOFor
+000050f0: 6d01 0300 0000 1a00 5100 5300 4f00 2d00  m.......Q.S.O.-.
+00005100: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00005110: 7208 0000 0000 0600 0000 0b51 534f 2063  r..........QSO c
+00005120: 6f6d 6d65 6e74 0700 0000 0751 534f 466f  omment.....QSOFo
+00005130: 726d 0103 0000 003e 0051 0053 004f 0020  rm.....>.Q.S.O. 
+00005140: 0077 0075 0072 0064 0065 0020 0076 006f  .w.u.r.d.e. .v.o
+00005150: 006e 0020 0048 0061 006d 0051 0054 0048  .n. .H.a.m.Q.T.H
+00005160: 0020 0061 0062 0067 0065 0077 0069 0065  . .a.b.g.e.w.i.e
+00005170: 0073 0065 006e 0800 0000 0006 0000 0016  .s.e.n..........
+00005180: 5153 4f20 7265 6a65 6374 6564 206f 6e20  QSO rejected on 
+00005190: 4861 6d51 5448 0700 0000 0751 534f 466f  HamQTH.....QSOFo
+000051a0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+000051b0: 0003 5154 4807 0000 0007 5153 4f46 6f72  ..QTH.....QSOFor
+000051c0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+000051d0: 0652 5354 2052 7807 0000 0007 5153 4f46  .RST Rx.....QSOF
+000051e0: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
+000051f0: 0000 0652 5354 2054 7807 0000 0007 5153  ...RST Tx.....QS
+00005200: 4f46 6f72 6d01 0300 0000 1a00 5200 5300  OForm.......R.S.
+00005210: 5400 2000 6500 6d00 7000 6600 6100 6e00  T. .e.m.p.f.a.n.
+00005220: 6700 6500 6e08 0000 0000 0600 0000 0c52  g.e.n..........R
+00005230: 5354 2072 6563 6569 7665 6407 0000 0007  ST received.....
+00005240: 5153 4f46 6f72 6d01 0300 0000 1800 5200  QSOForm.......R.
+00005250: 5300 5400 2000 6700 6500 7300 6500 6e00  S.T. .g.e.s.e.n.
+00005260: 6400 6500 7408 0000 0000 0600 0000 0852  d.e.t..........R
+00005270: 5354 2073 656e 7407 0000 0007 5153 4f46  ST sent.....QSOF
+00005280: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
+00005290: 0000 0552 6164 696f 0700 0000 0751 534f  ...Radio.....QSO
+000052a0: 466f 726d 0103 0000 0012 0053 0070 0065  Form.......S.p.e
+000052b0: 0069 0063 0068 0065 0072 006e 0800 0000  .i.c.h.e.r.n....
+000052c0: 0006 0000 0004 5361 7665 0700 0000 0751  ......Save.....Q
+000052d0: 534f 466f 726d 0103 0000 0026 0053 0070  SOForm.....&.S.p
+000052e0: 0065 0069 0063 0068 0065 0072 006e 0020  .e.i.c.h.e.r.n. 
+000052f0: 0026 0026 0020 0055 0070 006c 006f 0061  .&.&. .U.p.l.o.a
+00005300: 0064 0800 0000 0006 0000 000e 5361 7665  .d..........Save
+00005310: 2026 2620 5570 6c6f 6164 0700 0000 0751   && Upload.....Q
+00005320: 534f 466f 726d 0103 0000 002a 0065 0051  SOForm.....*.e.Q
+00005330: 0053 004c 002d 004f 0072 0064 006e 0065  .S.L.-.O.r.d.n.e
+00005340: 0072 0020 0061 0075 0073 0077 00e4 0068  .r. .a.u.s.w...h
+00005350: 006c 0065 006e 0800 0000 0006 0000 0012  .l.e.n..........
+00005360: 5365 6c65 6374 2065 5153 4c20 666f 6c64  Select eQSL fold
+00005370: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
+00005380: 0000 0036 0053 0065 0072 0076 0065 0072  ...6.S.e.r.v.e.r
+00005390: 006b 006f 006d 006d 0075 006e 0069 006b  .k.o.m.m.u.n.i.k
+000053a0: 0061 0074 0069 006f 006e 0073 002d 0046  .a.t.i.o.n.s.-.F
+000053b0: 0065 0068 006c 0065 0072 0800 0000 0006  .e.h.l.e.r......
+000053c0: 0000 001a 5365 7276 6572 2063 6f6d 6d75  ....Server commu
+000053d0: 6e69 6361 7469 6f6e 2065 7272 6f72 0700  nication error..
+000053e0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+000053f0: 0800 0000 0006 0000 0005 5374 6172 7407  ..........Start.
+00005400: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+00005410: ff08 0000 0000 0600 0000 0753 7461 7469  ...........Stati
+00005420: 6f6e 0700 0000 0751 534f 466f 726d 0103  on.....QSOForm..
+00005430: ffff ffff 0800 0000 0006 0000 0007 5375  ..............Su
+00005440: 626d 6f64 6507 0000 0007 5153 4f46 6f72  bmode.....QSOFor
+00005450: 6d01 0300 0000 3000 4400 6100 7300 2000  m.....0.D.a.s. .
+00005460: 5100 5300 4f00 2000 6900 7300 7400 2000  Q.S.O. .i.s.t. .
+00005470: 6500 6900 6e00 2000 4400 7500 7000 6c00  e.i.n. .D.u.p.l.
+00005480: 6900 6b00 6100 7408 0000 0000 0600 0000  i.k.a.t.........
+00005490: 1654 6865 2051 534f 2069 7320 6120 6475  .The QSO is a du
+000054a0: 706c 6963 6174 6507 0000 0007 5153 4f46  plicate.....QSOF
+000054b0: 6f72 6d01 0300 0000 b800 4400 6900 6500  orm.......D.i.e.
+000054c0: 2000 5100 5300 4c00 2d00 5200 6f00 7500   .Q.S.L.-.R.o.u.
+000054d0: 7400 6500 2000 6400 6500 7200 2000 6b00  t.e. .d.e.r. .k.
+000054e0: 6f00 6e00 7400 6100 6b00 7400 6900 6500  o.n.t.a.k.t.i.e.
+000054f0: 7200 7400 6500 6e00 2000 5300 7400 6100  r.t.e.n. .S.t.a.
+00005500: 7400 6900 6f00 6e00 2e00 0a00 4400 6900  t.i.o.n.....D.i.
+00005510: 6500 7300 2000 6900 7300 7400 2000 6e00  e.s. .i.s.t. .n.
+00005520: 6900 6300 6800 7400 2000 6400 6900 6500  i.c.h.t. .d.i.e.
+00005530: 2000 4100 6400 7200 6500 7300 7300 6500   .A.d.r.e.s.s.e.
+00005540: 2000 6400 6500 7300 2000 5100 5300 4c00   .d.e.s. .Q.S.L.
+00005550: 2d00 4d00 6100 6e00 6100 6700 6500 7200  -.M.a.n.a.g.e.r.
+00005560: 7300 2f00 2d00 4200 fc00 7200 6f00 7300  s./.-.B...r.o.s.
+00005570: 2e08 0000 0000 0600 0000 4c54 6865 2063  ..........LThe c
+00005580: 6f6e 7461 6374 6564 2073 7461 7469 6f6e  ontacted station
+00005590: 2051 534c 2072 6f75 7465 2e0a 5468 6973   QSL route..This
+000055a0: 2069 7320 6e6f 7420 7468 6520 5153 4c20   is not the QSL 
+000055b0: 6d61 6e61 6765 722f 6275 7265 6175 2061  manager/bureau a
+000055c0: 6464 7265 7373 2e07 0000 0007 5153 4f46  ddress......QSOF
+000055d0: 6f72 6d01 0300 0000 1000 4500 6e00 6400  orm.......E.n.d.
+000055e0: 6500 7a00 6500 6900 7408 0000 0000 0600  e.z.e.i.t.......
+000055f0: 0000 0854 696d 6520 656e 6407 0000 0007  ...Time end.....
+00005600: 5153 4f46 6f72 6d01 0300 0000 1200 5300  QSOForm.......S.
+00005610: 7400 6100 7200 7400 7a00 6500 6900 7408  t.a.r.t.z.e.i.t.
+00005620: 0000 0000 0600 0000 0a54 696d 6520 7374  .........Time st
+00005630: 6172 7407 0000 0007 5153 4f46 6f72 6d01  art.....QSOForm.
+00005640: 0300 0000 2400 6500 5100 5300 4c00 2d00  ....$.e.Q.S.L.-.
+00005650: 5500 7000 6c00 6f00 6100 6400 2d00 4600  U.p.l.o.a.d.-.F.
+00005660: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
+00005670: 0000 1155 706c 6f61 6420 6551 534c 2065  ...Upload eQSL e
+00005680: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
+00005690: 0103 0000 001a 0055 0070 006c 006f 0061  .......U.p.l.o.a
+000056a0: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
+000056b0: 0800 0000 0006 0000 0010 5570 6c6f 6164  ..........Upload
+000056c0: 206c 6f67 2065 7272 6f72 0700 0000 0751   log error.....Q
+000056d0: 534f 466f 726d 0103 0000 0068 0055 0070  SOForm.....h.U.p
+000056e0: 006c 006f 0061 0064 0020 0065 0072 0066  .l.o.a.d. .e.r.f
+000056f0: 006f 006c 0067 0074 0020 006e 0075 0072  .o.l.g.t. .n.u.r
+00005700: 0020 0077 0065 006e 006e 0020 0061 0075  . .w.e.n.n. .a.u
+00005710: 0066 0020 0064 0065 0072 0020 0051 0053  .f. .d.e.r. .Q.S
+00005720: 004c 002d 0053 0065 0069 0074 0065 0020  .L.-.S.e.i.t.e. 
+00005730: 0061 0075 0073 0067 0065 0077 00e4 0068  .a.u.s.g.e.w...h
+00005740: 006c 0074 0800 0000 0006 0000 0024 5570  .l.t.........$Up
+00005750: 6c6f 6164 7320 6f6e 6c79 2069 6620 7365  loads only if se
+00005760: 6c65 6374 6564 206f 6e20 5153 4c20 7061  lected on QSL pa
+00005770: 6765 0700 0000 0751 534f 466f 726d 0103  ge.....QSOForm..
+00005780: 0000 0048 0044 0065 0072 0020 004e 0075  ...H.D.e.r. .N.u
+00005790: 0074 007a 0065 0072 0020 0043 0061 006c  .t.z.e.r. .C.a.l
+000057a0: 006c 0020 0073 0074 0069 006d 006d 0074  .l. .s.t.i.m.m.t
+000057b0: 0020 006e 0069 0063 0068 0074 0020 00fc  . .n.i.c.h.t. ..
+000057c0: 0062 0065 0072 0065 0069 006e 0800 0000  .b.e.r.e.i.n....
+000057d0: 0006 0000 0018 5573 6572 2063 616c 6c20  ......User call 
+000057e0: 646f 6573 206e 6f74 206d 6174 6368 0700  does not match..
+000057f0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
+00005800: 0800 0000 0006 0000 0004 6551 534c 0700  ..........eQSL..
+00005810: 0000 0751 534f 466f 726d 0103 0000 001c  ...QSOForm......
+00005820: 0065 0051 0053 004c 0020 0065 006d 0070  .e.Q.S.L. .e.m.p
+00005830: 0066 0061 006e 0067 0065 006e 0800 0000  .f.a.n.g.e.n....
+00005840: 0006 0000 000d 6551 534c 2072 6563 6569  ......eQSL recei
+00005850: 7665 6407 0000 0007 5153 4f46 6f72 6d01  ved.....QSOForm.
+00005860: 0300 0000 1a00 6500 5100 5300 4c00 2000  ......e.Q.S.L. .
+00005870: 6700 6500 7300 6500 6e00 6400 6500 7408  g.e.s.e.n.d.e.t.
+00005880: 0000 0000 0600 0000 0965 5153 4c20 7365  .........eQSL se
+00005890: 6e74 0700 0000 0751 534f 466f 726d 0103  nt.....QSOForm..
+000058a0: 0000 0008 006b 002e 0041 002e 0800 0000  .....k...A......
+000058b0: 0006 0000 0004 6e2e 612e 0700 0000 0751  ......n.a......Q
+000058c0: 534f 466f 726d 0103 0000 0034 0072 0069  SOForm.....4.r.i
+000058d0: 0067 0063 0074 006c 0064 0020 005a 0065  .g.c.t.l.d. .Z.e
+000058e0: 0069 0074 00fc 0062 0065 0072 0073 0063  .i.t...b.e.r.s.c
+000058f0: 0068 0072 0065 0069 0074 0075 006e 0067  .h.r.e.i.t.u.n.g
+00005900: 0800 0000 0006 0000 000f 7269 6763 746c  ..........rigctl
+00005910: 6420 7469 6d65 6f75 7407 0000 0007 5153  d timeout.....QS
+00005920: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00005930: 0600 0000 0a79 7979 792d 4d4d 2d64 6407  .....yyyy-MM-dd.
+00005940: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005950: 7a00 4300 4100 5400 2d00 4500 6900 6e00  z.C.A.T.-.E.i.n.
+00005960: 7300 7400 6500 6c00 6c00 7500 6e00 6700  s.t.e.l.l.u.n.g.
+00005970: 2000 7700 7500 7200 6400 2000 6e00 6f00   .w.u.r.d. .n.o.
+00005980: 6300 6800 2000 6e00 6900 6500 2000 6700  c.h. .n.i.e. .g.
+00005990: 6500 7300 7000 6500 6900 6300 6800 6500  e.s.p.e.i.c.h.e.
+000059a0: 7200 7400 2000 6f00 7200 2000 5000 6100  r.t. .o.r. .P.a.
+000059b0: 7200 6100 6d00 6500 7400 6500 7200 2000  r.a.m.e.t.e.r. .
+000059c0: 6600 6500 6800 6c00 6500 6e08 0000 0000  f.e.h.l.e.n.....
+000059d0: 0600 0000 3b43 4154 2063 6f6e 6669 6775  ....;CAT configu
+000059e0: 7261 7469 6f6e 2077 6173 206e 6576 6572  ration was never
+000059f0: 2073 6176 6564 206f 7220 6120 7061 7261   saved or a para
+00005a00: 6d65 7465 7220 6973 206d 6973 7369 6e67  meter is missing
+00005a10: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
+00005a20: 0000 3000 4300 4100 5400 2d00 4500 6900  ..0.C.A.T.-.E.i.
+00005a30: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
+00005a40: 6700 6500 6e00 2000 4600 6500 6800 6c00  g.e.n. .F.e.h.l.
+00005a50: 6500 7208 0000 0000 0600 0000 1243 4154  e.r..........CAT
+00005a60: 2073 6574 7469 6e67 7320 6572 726f 7207   settings error.
+00005a70: 0000 0008 5365 7474 696e 6773 0103 0000  ....Settings....
+00005a80: 002a 0048 0061 006d 006c 0069 0062 0020  .*.H.a.m.l.i.b. 
+00005a90: 0072 0069 0067 0063 0074 006c 0064 0020  .r.i.g.c.t.l.d. 
+00005aa0: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
+00005ab0: 0006 0000 0020 4368 6f6f 7365 2068 616d  ..... Choose ham
+00005ac0: 6c69 6220 7269 6763 746c 6420 6578 6563  lib rigctld exec
+00005ad0: 7574 6162 6c65 0700 0000 0853 6574 7469  utable.....Setti
+00005ae0: 6e67 7301 0300 0000 2000 4400 6100 7400  ngs..... .D.a.t.
+00005af0: 7500 6d00 2f00 5a00 6500 6900 7400 2000  u.m./.Z.e.i.t. .
+00005b00: 5300 7400 6100 7200 7408 0000 0000 0600  S.t.a.r.t.......
+00005b10: 0000 0f44 6174 652f 5469 6d65 2073 7461  ...Date/Time sta
+00005b20: 7274 0700 0000 0853 6574 7469 6e67 7301  rt.....Settings.
+00005b30: 0300 0000 4200 4600 6500 6800 6c00 6500  ....B.F.e.h.l.e.
+00005b40: 7200 2000 6200 6500 6900 6d00 2000 4100  r. .b.e.i.m. .A.
+00005b50: 7500 7300 6600 fc00 6800 7200 6500 6e00  u.s.f...h.r.e.n.
+00005b60: 2000 7600 6f00 6e00 2000 7200 6900 6700   .v.o.n. .r.i.g.
+00005b70: 6300 7400 6c00 6408 0000 0000 0600 0000  c.t.l.d.........
+00005b80: 1745 7272 6f72 2065 7865 6375 7469 6e67  .Error executing
+00005b90: 2072 6967 6374 6c64 0700 0000 0853 6574   rigctld.....Set
+00005ba0: 7469 6e67 7301 03ff ffff ff08 0000 0000  tings...........
+00005bb0: 0600 0000 0648 616d 6c69 6207 0000 0008  .....Hamlib.....
+00005bc0: 5365 7474 696e 6773 0103 0000 004e 0044  Settings.....N.D
+00005bd0: 0069 0065 0020 0067 0065 0077 00e4 0068  .i.e. .g.e.w...h
+00005be0: 006c 0074 0065 0020 0044 0061 0074 0065  .l.t.e. .D.a.t.e
+00005bf0: 0069 0020 0069 0073 0074 0020 006e 0069  .i. .i.s.t. .n.i
+00005c00: 0063 0068 0074 0020 0061 0075 0073 0066  .c.h.t. .a.u.s.f
+00005c10: 00fc 0068 0072 0062 0061 0072 0800 0000  ...h.r.b.a.r....
+00005c20: 0006 0000 0023 5365 6c65 6374 6564 2066  .....#Selected f
+00005c30: 696c 6520 6973 206e 6f74 2074 6865 2065  ile is not the e
+00005c40: 7865 6375 7461 626c 6507 0000 0008 5365  xecutable.....Se
+00005c50: 7474 696e 6773 0103 0000 0014 007a 0065  ttings.......z.e
+00005c60: 0069 0067 0065 0020 0061 006c 006c 0065  .i.g.e. .a.l.l.e
+00005c70: 0800 0000 0006 0000 0008 5368 6f77 2061  ..........Show a
+00005c80: 6c6c 0700 0000 0853 6574 7469 6e67 7301  ll.....Settings.
+00005c90: 03ff ffff ff08 0000 0000 0600 0000 0553  ...............S
+00005ca0: 7461 7274 0700 0000 0853 6574 7469 6e67  tart.....Setting
+00005cb0: 7301 0300 0000 1a00 5300 7400 6100 7200  s.......S.t.a.r.
+00005cc0: 7400 6500 2000 4800 6100 6d00 6c00 6900  t.e. .H.a.m.l.i.
+00005cd0: 6208 0000 0000 0600 0000 0c53 7461 7274  b..........Start
+00005ce0: 2068 616d 6c69 6207 0000 0008 5365 7474   hamlib.....Sett
+00005cf0: 696e 6773 0103 ffff ffff 0800 0000 0006  ings............
+00005d00: 0000 0004 5374 6f70 0700 0000 0853 6574  ....Stop.....Set
+00005d10: 7469 6e67 7301 0300 0000 1a00 5300 7400  tings.......S.t.
+00005d20: 6f00 7000 7000 6500 2000 4800 6100 6d00  o.p.p.e. .H.a.m.
+00005d30: 6c00 6900 6208 0000 0000 0600 0000 0b53  l.i.b..........S
+00005d40: 746f 7020 6861 6d6c 6962 0700 0000 0853  top hamlib.....S
+00005d50: 6574 7469 6e67 7301 0300 0000 0a00 6100  ettings.......a.
+00005d60: 6b00 7400 6900 7608 0000 0000 0600 0000  k.t.i.v.........
+00005d70: 0561 6374 6976 0700 0000 0853 6574 7469  .activ.....Setti
+00005d80: 6e67 7301 0300 0000 0e00 6900 6e00 6100  ngs.......i.n.a.
+00005d90: 6b00 7400 6900 7608 0000 0000 0600 0000  k.t.i.v.........
+00005da0: 0769 6e61 6374 6976 0700 0000 0853 6574  .inactiv.....Set
+00005db0: 7469 6e67 7301 0300 0000 4a00 7200 6900  tings.....J.r.i.
+00005dc0: 6700 6300 7400 6c00 6400 2000 6b00 6f00  g.c.t.l.d. .k.o.
+00005dd0: 6e00 6e00 7400 6500 2000 6e00 6900 6300  n.n.t.e. .n.i.c.
+00005de0: 6800 7400 2000 6700 6500 7300 7400 6100  h.t. .g.e.s.t.a.
+00005df0: 7200 7400 6500 7400 2000 7700 6500 7200  r.t.e.t. .w.e.r.
+00005e00: 6400 6500 6e08 0000 0000 0600 0000 1e72  d.e.n..........r
+00005e10: 6967 6374 6c64 2064 6964 206e 6f74 2073  igctld did not s
+00005e20: 7461 7274 2070 726f 7065 726c 7907 0000  tart properly...
+00005e30: 0008 5365 7474 696e 6773 0103 0000 0036  ..Settings.....6
+00005e40: 0072 0069 0067 0063 0074 006c 0064 0020  .r.i.g.c.t.l.d. 
+00005e50: 0069 0073 0074 0020 006e 0069 0063 0068  .i.s.t. .n.i.c.h
+00005e60: 0074 0020 0076 0065 0072 0066 00fc 0067  .t. .v.e.r.f...g
+00005e70: 0062 0061 0072 0800 0000 0006 0000 0018  .b.a.r..........
+00005e80: 7269 6763 746c 6420 6973 206e 6f74 2061  rigctld is not a
+00005e90: 7661 696c 6162 6c65 0700 0000 0853 6574  vailable.....Set
+00005ea0: 7469 6e67 7301 0300 0000 1000 6700 6500  tings.......g.e.
+00005eb0: e400 6e00 6400 6500 7200 7408 0000 0000  ..n.d.e.r.t.....
+00005ec0: 0600 0000 014d 0700 0000 1454 7261 6e73  .....M.....Trans
+00005ed0: 6c61 7465 6454 6162 6c65 4d6f 6465 6c01  latedTableModel.
+00005ee0: 0300 0000 0800 4e00 6500 6900 6e08 0000  ......N.e.i.n...
+00005ef0: 0000 0600 0000 014e 0700 0000 1454 7261  .......N.....Tra
+00005f00: 6e73 6c61 7465 6454 6162 6c65 4d6f 6465  nslatedTableMode
+00005f10: 6c01 0300 0000 1200 6100 6e00 6700 6500  l.......a.n.g.e.
+00005f20: 6600 7200 6100 6700 7408 0000 0000 0600  f.r.a.g.t.......
+00005f30: 0000 0152 0700 0000 1454 7261 6e73 6c61  ...R.....Transla
+00005f40: 7465 6454 6162 6c65 4d6f 6465 6c01 0300  tedTableModel...
+00005f50: 0000 0400 4a00 6108 0000 0000 0600 0000  ....J.a.........
+00005f60: 0159 0700 0000 1454 7261 6e73 6c61 7465  .Y.....Translate
+00005f70: 6454 6162 6c65 4d6f 6465 6c01 03ff ffff  dTableModel.....
+00005f80: ff08 0000 0000 0600 0000 074a 5338 4361  ...........JS8Ca
+00005f90: 6c6c 0700 0000 0f61 7070 5365 6c65 6374  ll.....appSelect
+00005fa0: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
+00005fb0: 0006 0000 0005 4f74 6865 7207 0000 000f  ......Other.....
+00005fc0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
+00005fd0: 0300 0000 2a00 4100 7500 7300 7700 6100  ....*.A.u.s.w.a.
+00005fe0: 6800 6c00 2000 6400 6500 7300 2000 5000  h.l. .d.e.s. .P.
+00005ff0: 7200 6f00 6700 7200 6100 6d00 6d00 7308  r.o.g.r.a.m.m.s.
+00006000: 0000 0000 0600 0000 1653 656c 6563 7420  .........Select 
+00006010: 7468 6520 6170 706c 6963 6174 696f 6e07  the application.
+00006020: 0000 000f 6170 7053 656c 6563 7444 6961  ....appSelectDia
+00006030: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00006040: 0000 0657 534a 542d 5807 0000 000f 6170  ...WSJT-X.....ap
+00006050: 7053 656c 6563 7444 6961 6c6f 6701 03ff  pSelectDialog...
+00006060: ffff ff08 0000 0000 0600 0000 0666 6c64  .............fld
+00006070: 6967 6907 0000 000f 6170 7053 656c 6563  igi.....appSelec
+00006080: 7444 6961 6c6f 6701 8800 0000 0201 01    tDialog........
```

### Comparing `dragonlog-1.1.2/dragonlog/data/modes.json` & `dragonlog-1.1.3/dragonlog/data/modes.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/eQSL.py` & `dragonlog-1.1.3/dragonlog/eQSL.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/Screenshot.png` & `dragonlog-1.1.3/dragonlog/icons/Screenshot.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/db.png` & `dragonlog-1.1.3/dragonlog/icons/db.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/edit.png` & `dragonlog-1.1.3/dragonlog/icons/edit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/edit_add.png` & `dragonlog-1.1.3/dragonlog/icons/edit_add.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/edit_addmulti.png` & `dragonlog-1.1.3/dragonlog/icons/edit_addmulti.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/edit_addmulti.xcf` & `dragonlog-1.1.3/dragonlog/icons/edit_addmulti.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/edit_remove.png` & `dragonlog-1.1.3/dragonlog/icons/edit_remove.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/exit.png` & `dragonlog-1.1.3/dragonlog/icons/exit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/file_doc.png` & `dragonlog-1.1.3/dragonlog/icons/file_doc.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/fileexport.png` & `dragonlog-1.1.3/dragonlog/icons/fileexport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/fileimport.png` & `dragonlog-1.1.3/dragonlog/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/gear.png` & `dragonlog-1.1.3/dragonlog/icons/gear.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/help.png` & `dragonlog-1.1.3/dragonlog/icons/help.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.png` & `dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/icons8-dragon-96.xcf` & `dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/info.png` & `dragonlog-1.1.3/dragonlog/icons/info.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/logo.ico` & `dragonlog-1.1.3/dragonlog/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/no.png` & `dragonlog-1.1.3/dragonlog/icons/no.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/ok.png` & `dragonlog-1.1.3/dragonlog/icons/ok.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/player_play.png` & `dragonlog-1.1.3/dragonlog/icons/player_play.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/player_stop.png` & `dragonlog-1.1.3/dragonlog/icons/player_stop.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/upload_lotw.png` & `dragonlog-1.1.3/dragonlog/icons/upload_lotw.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/upload_lotw.xcf` & `dragonlog-1.1.3/dragonlog/icons/upload_lotw.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/dragonlog/icons/watch.png` & `dragonlog-1.1.3/dragonlog/icons/watch.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/pyproject.toml` & `dragonlog-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.2/setup_msi.py` & `dragonlog-1.1.3/setup_msi.py`

 * *Files identical despite different names*

