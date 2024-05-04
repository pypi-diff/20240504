# Comparing `tmp/justdeepit-0.2.0.tar.gz` & `tmp/JustDeepIt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justdeepit-0.2.0.tar", last modified: Tue Apr 30 05:49:13 2024, max compression
+gzip compressed data, was "justdeepit-0.2.1.tar", last modified: Sat May  4 20:25:12 2024, max compression
```

## Comparing `justdeepit-0.2.0.tar` & `JustDeepIt-0.2.1.tar`

### file list

```diff
@@ -1,67 +1,58 @@
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.659912 justdeepit-0.2.0/
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.659415 justdeepit-0.2.0/JustDeepIt.egg-info/
--rw-r--r--   0 sonk414    (501) staff       (20)     2515 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/PKG-INFO
--rw-r-----   0 sonk414    (501) staff       (20)     1554 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/SOURCES.txt
--rw-r-----   0 sonk414    (501) staff       (20)        1 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/dependency_links.txt
--rw-r-----   0 sonk414    (501) staff       (20)       58 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/entry_points.txt
--rw-r-----   0 sonk414    (501) staff       (20)      145 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/requires.txt
--rw-r-----   0 sonk414    (501) staff       (20)       11 2024-04-30 05:49:13.000000 justdeepit-0.2.0/JustDeepIt.egg-info/top_level.txt
--rw-r-----   0 sonk414    (501) staff       (20)        1 2024-04-30 05:17:09.000000 justdeepit-0.2.0/JustDeepIt.egg-info/zip-safe
--rw-r--r--   0 sonk414    (501) staff       (20)     1070 2024-04-30 05:17:10.000000 justdeepit-0.2.0/LICENSE
--rw-r--r--   0 sonk414    (501) staff       (20)      128 2024-04-30 05:17:10.000000 justdeepit-0.2.0/MANIFEST.in
--rw-r--r--   0 sonk414    (501) staff       (20)     2515 2024-04-30 05:49:13.659702 justdeepit-0.2.0/PKG-INFO
--rw-r--r--   0 sonk414    (501) staff       (20)     1426 2024-04-30 05:17:10.000000 justdeepit-0.2.0/README.md
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.651816 justdeepit-0.2.0/justdeepit/
--rw-r--r--   0 sonk414    (501) staff       (20)       95 2024-04-30 05:17:27.000000 justdeepit-0.2.0/justdeepit/__init__.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.652839 justdeepit-0.2.0/justdeepit/app/
--rw-r--r--   0 sonk414    (501) staff       (20)      162 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)    25983 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/app.py
--rw-r--r--   0 sonk414    (501) staff       (20)     5692 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/app/appbase.py
--rw-r--r--   0 sonk414    (501) staff       (20)      554 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/appis.py
--rw-r--r--   0 sonk414    (501) staff       (20)    10048 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/appod.py
--rw-r--r--   0 sonk414    (501) staff       (20)    22300 2024-04-30 05:17:29.000000 justdeepit-0.2.0/justdeepit/app/appsod.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.653648 justdeepit-0.2.0/justdeepit/models/
--rw-r--r--   0 sonk414    (501) staff       (20)      184 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)      309 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/abstract.py
--rw-r--r--   0 sonk414    (501) staff       (20)    12931 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/instance_segment.py
--rw-r--r--   0 sonk414    (501) staff       (20)    13500 2024-04-30 05:17:27.000000 justdeepit-0.2.0/justdeepit/models/object_detect.py
--rw-r--r--   0 sonk414    (501) staff       (20)    12227 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/salient_object_detect.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.654558 justdeepit-0.2.0/justdeepit/models/utils/
--rw-r--r--   0 sonk414    (501) staff       (20)        0 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)     6720 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/data.py
--rw-r--r--   0 sonk414    (501) staff       (20)    11507 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/mmdetbase.py
--rw-r--r--   0 sonk414    (501) staff       (20)    36052 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/u2net.py
--rw-r--r--   0 sonk414    (501) staff       (20)    10173 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/models/utils/unet.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.649685 justdeepit-0.2.0/justdeepit/src/
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.655154 justdeepit-0.2.0/justdeepit/src/font/
--rw-r--r--   0 sonk414    (501) staff       (20)   555264 2024-04-30 05:17:30.000000 justdeepit-0.2.0/justdeepit/src/font/NotoSans-Medium.ttf
--rw-r--r--   0 sonk414    (501) staff       (20)     4449 2024-04-30 05:17:30.000000 justdeepit-0.2.0/justdeepit/src/font/OFL.txt
--rw-r--r--   0 sonk414    (501) staff       (20)    56860 2024-04-30 05:17:28.000000 justdeepit-0.2.0/justdeepit/utils.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.656295 justdeepit-0.2.0/justdeepit/webapp/
--rw-r--r--   0 sonk414    (501) staff       (20)      174 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/__init__.py
--rw-r--r--   0 sonk414    (501) staff       (20)    28329 2024-03-08 01:38:16.000000 justdeepit-0.2.0/justdeepit/webapp/app.py
--rw-r--r--   0 sonk414    (501) staff       (20)     6844 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/appbase.py
--rw-r--r--   0 sonk414    (501) staff       (20)     1314 2023-12-26 03:14:25.000000 justdeepit-0.2.0/justdeepit/webapp/appis.py
--rw-r--r--   0 sonk414    (501) staff       (20)     8356 2023-12-26 03:13:54.000000 justdeepit-0.2.0/justdeepit/webapp/appod.py
--rw-r--r--   0 sonk414    (501) staff       (20)    22154 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/appsod.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.657363 justdeepit-0.2.0/justdeepit/webapp/static/
--rw-r--r--   0 sonk414    (501) staff       (20)    89501 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.js
--rw-r--r--   0 sonk414    (501) staff       (20)   137972 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.map
--rw-r--r--   0 sonk414    (501) staff       (20)    14309 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/styles.css
--rw-r--r--   0 sonk414    (501) staff       (20)    58702 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js
--rw-r--r--   0 sonk414    (501) staff       (20)   174878 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js.map
--rw-r--r--   0 sonk414    (501) staff       (20)    23347 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/static/utils.js
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.657803 justdeepit-0.2.0/justdeepit/webapp/templates/
--rw-r--r--   0 sonk414    (501) staff       (20)     1198 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/templates/index.html
--rw-r--r--   0 sonk414    (501) staff       (20)    15402 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/templates/module.html
--rw-r--r--   0 sonk414    (501) staff       (20)      571 2023-12-20 04:31:47.000000 justdeepit-0.2.0/justdeepit/webapp/templates/shutdown.html
--rw-r--r--   0 sonk414    (501) staff       (20)      151 2024-04-30 05:17:30.000000 justdeepit-0.2.0/requirements.txt
--rw-r--r--   0 sonk414    (501) staff       (20)       38 2024-04-30 05:49:13.659956 justdeepit-0.2.0/setup.cfg
--rw-r--r--   0 sonk414    (501) staff       (20)     1582 2024-04-30 05:47:27.000000 justdeepit-0.2.0/setup.py
-drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-04-30 05:49:13.658814 justdeepit-0.2.0/tests/
--rw-r--r--   0 sonk414    (501) staff       (20)     3656 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_det.py
--rw-r--r--   0 sonk414    (501) staff       (20)     7845 2023-12-19 06:32:04.000000 justdeepit-0.2.0/tests/test_odmodels.py
--rw-r--r--   0 sonk414    (501) staff       (20)     4943 2023-12-19 06:32:04.000000 justdeepit-0.2.0/tests/test_osmodels.py
--rw-r--r--   0 sonk414    (501) staff       (20)     2304 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_segm.py
--rw-r--r--   0 sonk414    (501) staff       (20)     3139 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_sodmodels.py
--rw-r--r--   0 sonk414    (501) staff       (20)     6933 2024-04-30 05:22:19.000000 justdeepit-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.150634 justdeepit-0.2.1/
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.150049 justdeepit-0.2.1/JustDeepIt.egg-info/
+-rw-r--r--   0 sonk414    (501) staff       (20)     2103 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/PKG-INFO
+-rw-r--r--   0 sonk414    (501) staff       (20)     1315 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/SOURCES.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)        1 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/dependency_links.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)       58 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/entry_points.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)      145 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/requires.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)       11 2024-05-04 20:25:12.000000 justdeepit-0.2.1/JustDeepIt.egg-info/top_level.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)        1 2024-05-04 20:23:49.000000 justdeepit-0.2.1/JustDeepIt.egg-info/zip-safe
+-rw-r--r--   0 sonk414    (501) staff       (20)     1070 2024-05-04 20:22:08.000000 justdeepit-0.2.1/LICENSE
+-rw-r--r--   0 sonk414    (501) staff       (20)      122 2024-05-04 20:22:31.000000 justdeepit-0.2.1/MANIFEST.in
+-rw-r--r--   0 sonk414    (501) staff       (20)     2103 2024-05-04 20:25:12.150374 justdeepit-0.2.1/PKG-INFO
+-rw-r--r--   0 sonk414    (501) staff       (20)     1426 2024-05-04 20:22:08.000000 justdeepit-0.2.1/README.md
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.132894 justdeepit-0.2.1/justdeepit/
+-rw-r--r--   0 sonk414    (501) staff       (20)       95 2024-05-04 20:23:07.000000 justdeepit-0.2.1/justdeepit/__init__.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.137290 justdeepit-0.2.1/justdeepit/app/
+-rw-r--r--   0 sonk414    (501) staff       (20)      162 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    25983 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/app.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     5692 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appbase.py
+-rw-r--r--   0 sonk414    (501) staff       (20)      554 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appis.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    10048 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appod.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    22300 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/appsod.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.141555 justdeepit-0.2.1/justdeepit/app/static/
+-rw-r--r--   0 sonk414    (501) staff       (20)    89501 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.js
+-rw-r--r--   0 sonk414    (501) staff       (20)   137972 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.map
+-rw-r--r--   0 sonk414    (501) staff       (20)    14483 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/styles.css
+-rw-r--r--   0 sonk414    (501) staff       (20)    58702 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js
+-rw-r--r--   0 sonk414    (501) staff       (20)   174878 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js.map
+-rw-r--r--   0 sonk414    (501) staff       (20)    22813 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/static/utils.js
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.142487 justdeepit-0.2.1/justdeepit/app/templates/
+-rw-r--r--   0 sonk414    (501) staff       (20)     1187 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/templates/index.html
+-rw-r--r--   0 sonk414    (501) staff       (20)    17293 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/templates/module.html
+-rw-r--r--   0 sonk414    (501) staff       (20)      560 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/app/templates/shutdown.html
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.144447 justdeepit-0.2.1/justdeepit/models/
+-rw-r--r--   0 sonk414    (501) staff       (20)      184 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)      309 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/abstract.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    12931 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/instance_segment.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    13500 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/object_detect.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    12227 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/salient_object_detect.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.146013 justdeepit-0.2.1/justdeepit/models/utils/
+-rw-r--r--   0 sonk414    (501) staff       (20)        0 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/__init__.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     6720 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/data.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    11507 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/mmdetbase.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    36052 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/u2net.py
+-rw-r--r--   0 sonk414    (501) staff       (20)    10173 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/models/utils/unet.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.130293 justdeepit-0.2.1/justdeepit/src/
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.148009 justdeepit-0.2.1/justdeepit/src/font/
+-rw-r--r--   0 sonk414    (501) staff       (20)   555264 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/src/font/NotoSans-Medium.ttf
+-rw-r--r--   0 sonk414    (501) staff       (20)     4449 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/src/font/OFL.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)    56860 2024-05-04 20:22:08.000000 justdeepit-0.2.1/justdeepit/utils.py
+-rw-r--r--   0 sonk414    (501) staff       (20)      151 2024-05-04 20:22:08.000000 justdeepit-0.2.1/requirements.txt
+-rw-r--r--   0 sonk414    (501) staff       (20)       38 2024-05-04 20:25:12.150692 justdeepit-0.2.1/setup.cfg
+-rw-r--r--   0 sonk414    (501) staff       (20)     2649 2024-05-04 20:22:08.000000 justdeepit-0.2.1/setup.py
+drwxr-xr-x   0 sonk414    (501) staff       (20)        0 2024-05-04 20:25:12.149549 justdeepit-0.2.1/tests/
+-rw-r--r--   0 sonk414    (501) staff       (20)     3656 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_det.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     2304 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_segm.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     3139 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_sodmodels.py
+-rw-r--r--   0 sonk414    (501) staff       (20)     6933 2024-05-04 20:22:08.000000 justdeepit-0.2.1/tests/test_utils.py
```

### Comparing `justdeepit-0.2.0/JustDeepIt.egg-info/PKG-INFO` & `justdeepit-0.2.1/JustDeepIt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.2.0
+Version: 0.2.1
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
-Keywords: object detection,instance segmentation
+Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: joblib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: opencv-python>=4.5.1
@@ -28,39 +27,8 @@
 Requires-Dist: uvicorn
 Requires-Dist: jinja2
 Requires-Dist: python-multipart
 Requires-Dist: torch>=1.8
 Requires-Dist: torchvision
 Requires-Dist: openmim
 
-# JustDeepIt 
-
-Image analysis based on deep learning is becoming mainstream and increasingly accessible
-for solving various scientific problems in diverse fields including plant science.
-Practical applications in plant science include species classification,
-fruit detection, plant disease and pest detection, weed detection,
-leaf segmentation, and plant segmentation.
-Python programming language and its libraries including PyTorch and MMDetection
-have made deep learning much easier and more accessible to researchers.
-However, deep learning technologies remain challenging for programming beginners
-because they require computer programming skills and a basic familiarity
-with character user interfaces (CUIs).
-JustDeepIt aims to simplify object detection, instance segmentation, and salient object detection
-using deep learning by providing a graphical user interface (GUI).
-In addition, to ensure flexibility and extensibility, JustDeepIt also provides CUI.
-It may be applicable for image analysis in various disciplines beyond plant science.
-
-
-## Documentation
-
-- https://justdeepit.readthedocs.io/en/latest/index.html
-
-
-## Citation
-
-Sun J, Cao W, Yamanaka T.
-JustDeepIt: Software tool with graphical and character user interfaces
-for deep learning-based object detection and segmentation in image analysis.
-Front. Plant Sci., 2022, 13:964058.
-doi: [10.3389/fpls.2022.964058](https://doi.org/10.3389/fpls.2022.964058)
-
-
+Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2 have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
```

### Comparing `justdeepit-0.2.0/LICENSE` & `justdeepit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/PKG-INFO` & `justdeepit-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: JustDeepIt
-Version: 0.2.0
+Version: 0.2.1
 Summary: a GUI tool for object detection and segmentation based on deep learning
 Home-page: https://github.com/biunit/JustDeepIt
 Author: Jianqiang Sun
 Author-email: sun@biunit.dev
 License: MIT
-Keywords: object detection,instance segmentation
+Keywords: object detection,object segmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: joblib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: opencv-python>=4.5.1
@@ -28,39 +27,8 @@
 Requires-Dist: uvicorn
 Requires-Dist: jinja2
 Requires-Dist: python-multipart
 Requires-Dist: torch>=1.8
 Requires-Dist: torchvision
 Requires-Dist: openmim
 
-# JustDeepIt 
-
-Image analysis based on deep learning is becoming mainstream and increasingly accessible
-for solving various scientific problems in diverse fields including plant science.
-Practical applications in plant science include species classification,
-fruit detection, plant disease and pest detection, weed detection,
-leaf segmentation, and plant segmentation.
-Python programming language and its libraries including PyTorch and MMDetection
-have made deep learning much easier and more accessible to researchers.
-However, deep learning technologies remain challenging for programming beginners
-because they require computer programming skills and a basic familiarity
-with character user interfaces (CUIs).
-JustDeepIt aims to simplify object detection, instance segmentation, and salient object detection
-using deep learning by providing a graphical user interface (GUI).
-In addition, to ensure flexibility and extensibility, JustDeepIt also provides CUI.
-It may be applicable for image analysis in various disciplines beyond plant science.
-
-
-## Documentation
-
-- https://justdeepit.readthedocs.io/en/latest/index.html
-
-
-## Citation
-
-Sun J, Cao W, Yamanaka T.
-JustDeepIt: Software tool with graphical and character user interfaces
-for deep learning-based object detection and segmentation in image analysis.
-Front. Plant Sci., 2022, 13:964058.
-doi: [10.3389/fpls.2022.964058](https://doi.org/10.3389/fpls.2022.964058)
-
-
+Deep learning has been applied to solve various problems, especially in image recognition, across many fields including the life sciences and agriculture. Many studies have reported the use of deep learning to identify plant and insect species, detect flowers and fruits, segment plant individuals from fixed-point observation cameras or drone images, and other applications. Programming languages such as Python and its libraries including PyTorch, MMDetection, and Detectron2 have made deep learning easier and more accessible to researchers. However, it remains difficult for many researchers without advanced programming skills to use deep learning and environments such as the character user interface (CUI) through keyboard input. JustDeepIt aims to support researchers by facilitating the use of deep learning for object detection and segmentation by providing both graphical user interface (GUI) and CUI operations. JustDeepIt can be used for plant detection, pest detection, and a variety of tasks in life sciences, agriculture, and other fields.
```

### Comparing `justdeepit-0.2.0/README.md` & `justdeepit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/app/app.py` & `justdeepit-0.2.1/justdeepit/app/app.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/app/appbase.py` & `justdeepit-0.2.1/justdeepit/app/appbase.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/app/appis.py` & `justdeepit-0.2.1/justdeepit/app/appis.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/app/appod.py` & `justdeepit-0.2.1/justdeepit/app/appod.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/app/appsod.py` & `justdeepit-0.2.1/justdeepit/app/appsod.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/instance_segment.py` & `justdeepit-0.2.1/justdeepit/models/instance_segment.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/object_detect.py` & `justdeepit-0.2.1/justdeepit/models/object_detect.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/salient_object_detect.py` & `justdeepit-0.2.1/justdeepit/models/salient_object_detect.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/utils/data.py` & `justdeepit-0.2.1/justdeepit/models/utils/data.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/utils/mmdetbase.py` & `justdeepit-0.2.1/justdeepit/models/utils/mmdetbase.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/utils/u2net.py` & `justdeepit-0.2.1/justdeepit/models/utils/u2net.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/models/utils/unet.py` & `justdeepit-0.2.1/justdeepit/models/utils/unet.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/src/font/NotoSans-Medium.ttf` & `justdeepit-0.2.1/justdeepit/src/font/NotoSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/src/font/OFL.txt` & `justdeepit-0.2.1/justdeepit/src/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/utils.py` & `justdeepit-0.2.1/justdeepit/utils.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.js` & `justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/webapp/static/jquery-3.6.0.min.map` & `justdeepit-0.2.1/justdeepit/app/static/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/webapp/static/styles.css` & `justdeepit-0.2.1/justdeepit/app/static/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     font-weight: 500;
     margin-top: 1em;
     margin-bottom: 0.5em;
     padding-bottom: 0.3em;
     border-bottom: dashed 1px #999;
 }
 
+.info-optional {
+    font-size: 0.95em;
+    color: #999;
+}
+
 #module-name {
     margin: 1.2em 0;
     font-size: 1.6em;
     font-weight: 900;
     position: relative;
     padding: 0 65px;
     text-align: center;
@@ -105,25 +110,29 @@
     padding: 3px 0px;
     width: 20%;
     min-width: 100px;
     border: 0px;
     overflow: hidden;
     box-sizing: border-box;
 }
-input.file-path, input.digits, input.text, input.text-full {
+input::placeholder {
+    color: #9f9f9f;
+    padding-left: 5px;
+}
+input.file-path, input.file-path-option, input.digits, input.text, input.text-full {
     font-size: 0.9em;
     line-height: 20px;
     border: 1px solid #ccc;
     padding: 3px;
     box-sizing: border-box;
 }
 input.digits {
     text-align: right;
 }
-input.file-path {
+input.file-path, input.file-path-option {
     margin-right: 3%;
     width: 97%;
 }
 input.digits, select.digits {
     margin-left: 1em;
     width: 4em;
 }
```

### Comparing `justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js` & `justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/webapp/static/tree.jquery.js.map` & `justdeepit-0.2.1/justdeepit/app/static/tree.jquery.js.map`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/justdeepit/webapp/static/utils.js` & `justdeepit-0.2.1/justdeepit/app/static/utils.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,15 @@
     'mode': null,
     'status': null,
     'timestamp': null
 };
 var focusedInputField = null;
 var msgSelectFile = 'Please select a FILE or add a file name after the selected folder.';
 var msgSelectFolder = 'Please select a FOLDER';
+var msgLeftBank = 'Left bank if no ____ dataset';
 var module = location.pathname.split('/')[1] === 'module' ? location.pathname.split('/')[2] : null;
 
 
 function node2path(node) {
     let dir_path = '';
     if (node.parent !== null) {
         dir_path = dir_path + node2path(node.parent) + '/';
@@ -30,35 +31,33 @@
 }
 
 
 function refreshParams() {
     let deferred = new $.Deferred;
     $.ajax({
         type: 'GET',
-        url: '/api/params',
+        url: '/api/config',
         data: {
             module: module
         },
         dataType: 'json',
         cache: false,
     }).done(function(formFields, textStatus, jqXHR) {
         for (let formId in formFields) {
-            if (formId !== 'module') {
-                for (let fieldId in formFields[formId]) {
-                    let fieldId_ = '#module-' + formId + '-' + fieldId;
-                    if ($(fieldId_)) {
-                        if ($(fieldId_).is(':checkbox')) {
-                            if (formFields[formId][fieldId]) {
-                                $(fieldId_).attr('checked', true).prop('checked', true).change();
-                            } else {
-                                $(fieldId_).attr('checked', false).prop('checked', false).change();
-                            }
+            for (let fieldId in formFields[formId]) {
+                let fieldId_ = '#module--' + formId + '--' + fieldId;
+                if ($(fieldId_)) {
+                    if ($(fieldId_).is(':checkbox')) {
+                        if (formFields[formId][fieldId]) {
+                            $(fieldId_).attr('checked', true).prop('checked', true).change();
                         } else {
-                            $(fieldId_).val(formFields[formId][fieldId]);
+                            $(fieldId_).attr('checked', false).prop('checked', false).change();
                         }
+                    } else {
+                        $(fieldId_).val(formFields[formId][fieldId]);
                     }
                 }
             }
         }
         deferred.resolve();
     }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
         deferred.reject();
@@ -70,34 +69,34 @@
     return deferred.promise();
 }
 
 
 function refreshModuleTabs() {
     let tabClasses = [null, null, null];
     if (moduleRunningStatus.status === null) {
-        if ($('#module-config-status').val() !== 'COMPLETED') {
+        if ($('#module--BASE--status').val() !== 'COMPLETED') {
             tabClasses = ['module-tab-active', 'module-tab-disabled', 'module-tab-disabled'];
         } else {
             tabClasses = ['module-tab-active', null, null];
         }
     } else {
         if (moduleRunningStatus.status === 'RUNNING') {
-            if (moduleRunningStatus.mode === 'config') {
+            if (moduleRunningStatus.mode === 'BASE') {
                 tabClasses = ['module-tab-active-disabled', 'module-tab-disabled', 'module-tab-disabled'];
-            } else if (moduleRunningStatus.mode === 'training') {
+            } else if (moduleRunningStatus.mode === 'TRAIN') {
                 tabClasses = ['module-tab-disabled', 'module-tab-active-disabled', 'module-tab-disabled'];
-            } else if (moduleRunningStatus.mode === 'inference') {
+            } else if (moduleRunningStatus.mode === 'INFERENCE') {
                 tabClasses = ['module-tab-disabled', 'module-tab-disabled', 'module-tab-active-disabled'];
             }
         } else {
-            if (moduleRunningStatus.mode === 'config') {
+            if (moduleRunningStatus.mode === 'BASE') {
                 tabClasses = ['module-tab-active', null, null];
-            } else if (moduleRunningStatus.mode === 'training') {
+            } else if (moduleRunningStatus.mode === 'TRAIN') {
                 tabClasses = [null, 'module-tab-active', null];
-            } else if (moduleRunningStatus.mode === 'inference') {
+            } else if (moduleRunningStatus.mode === 'INFERENCE') {
                 tabClasses = [null, null, 'module-tab-active'];
             }
         }
     }
     tabClasses.forEach(function(tabClass, i) {
         $('.module-tab').eq(i).removeClass('module-tab-disabled module-tab-active-disabled');
         if (tabClass !== null) {
@@ -121,15 +120,15 @@
         $('#shutdown').attr('disabled', false);
     }
 }
 
 
 function setSelectedFile(selectFieldId = 'filetree-selected') {
     selectedFilePath = $('#' + selectFieldId).val();
-    if (focusedInputField == 'module-training-model_weight') {
+    if (focusedInputField == 'module--TRAIN--model_weight') {
         if (selectedFilePath.slice((selectedFilePath.lastIndexOf(".") - 1 >>> 0) + 2) !== 'pth') {
             selectedFilePath = selectedFilePath + '.pth';
         }
     }
     console.log(selectedFilePath);
     $('#' + focusedInputField).val(selectedFilePath);
     focusedInputField = null;
@@ -201,23 +200,22 @@
             scrollTop: $('#app-log-msg')[0].scrollHeight - $('#app-log-msg')[0].clientHeight
         }, 1500);
     });
 }
 
 
 function refreshExecuteButtons() {
-    let forms = ['#module-config', '#module-training', '#module-inference'];
+    let forms = ['#module--BASE', '#module--TRAIN', '#module--INFERENCE'];
 
     for (let formId of forms) {
-
-        let buttonId = formId + '-run';
+        let buttonId = formId + '--run';
         let isValid = true;
         $(formId + ' .file-path').each(function() {
             required_field = true;
-            if ($(this).attr('id') === 'module-config-config') required_field = false;
+            if ($(this).attr('id') === 'module--BASE--config') required_field = false;
 
             if (required_field) {
                 if ($(this).val() === '') {
                     isValid = false;
                     $(this).addClass('highlight-empty-input');
                 } else {
                     $(this).removeClass('highlight-empty-input');
@@ -244,15 +242,15 @@
         if ((isValid) && ((moduleRunningStatus.status === null) || (moduleRunningStatus.status !== 'RUNNING'))) {
             $(buttonId).removeClass('button-disable');
             $(buttonId).attr('disabled', false);
         } else {
             $(buttonId).addClass('button-disable');
             $(buttonId).attr('disabled', true);
         }
-        if (formId == '#module-config') {
+        if (formId == '#module--BASE') {
             refreshConfigField();
         }
     }
 }
 
 
 function __refreshModuleDelay() {
@@ -276,59 +274,50 @@
     if (force_run) {
         $.when(refreshParams()).done(_refreshModuleDelay);
     }
 }
 
 
 function refreshConfigField() {
-    if ($('#module-config-architecture').val() != 'custom') {
-        $('#module-config-config').val(null);
-        $('#module-config-config').attr('readonly', true);
+    if ($('#module--BASE--architecture').val() != 'custom') {
+        $('#module--BASE--config').val(null);
+        $('#module--BASE--config').attr('readonly', true);
         $('#config-select-open').attr('disabled', true);
         $('#config-select-open').addClass('button-disable');
     } else {
-        $('#module-config-config').attr('readonly', false);
+        $('#module--BASE--config').attr('readonly', false);
         $('#config-select-open').attr('disabled', false);
         $('#config-select-open').removeClass('button-disable');
     }
 }
 
 
 function refreshTrainOptimizer() {
     default_optmizer = '';
     default_scheduler = '';
     if ($('#module').val() === 'SOD') {
         default_optmizer = 'Adam(params, lr=0.001, betas=(0.9, 0.999)';
         default_scheduler = 'ExponentialLR(optimizer, gamma=0.9)';
     } else {
-        if ($('#module-config-backend').val().toLowerCase() == 'mmdetection') {
-            default_optmizer = 'dict(type="Adam", lr=0.001)';
-            default_scheduler = 'dict(policy="CosineAnnealing", warmup="linear", warmup_iters=1000, warmup_ratio=0.1)';
-        }
+        default_optmizer = 'dict(type="Adam", lr=0.001)';
+        default_scheduler = 'dict(policy="CosineAnnealing", warmup="linear", warmup_iters=1000, warmup_ratio=0.1)';
     }
-    $('#module-training-optimizer').attr('placeholder', default_optmizer);
-    $('#module-training-scheduler').attr('placeholder', default_scheduler);
-
+    $('#module--TRAIN--optimizer').attr('placeholder', default_optmizer);
+    $('#module--TRAIN--scheduler').attr('placeholder', default_scheduler);
     if ($('#module').val() !== 'SOD') {
-        if ($('#module-config-backend').val().toLowerCase() === 'detectron2') {
-            $('#module-training-optimizer').attr('disabled', true);
-            $('#module-training-scheduler').attr('disabled', true);
-        } else {
-            $('#module-training-optimizer').attr('disabled', false);
-            $('#module-training-scheduler').attr('disabled', false);
-        }
+        $('#module--TRAIN--optimizer').attr('disabled', false);
+        $('#module--TRAIN--scheduler').attr('disabled', false);
     }
 }
 
 
 
 
 
 $(function() {
-
     // module action tabs
     $('.module-tab').on('click', function() {
         if (!$(this).hasClass('module-tab-disabled')) {
             $('.module-tab-active').removeClass('module-tab-active');
             $(this).addClass('module-tab-active');
             const i = $('.module-tab').index(this);
             if (i === 1) refreshTrainOptimizer(); // set optimizer and scheduler placeholders
@@ -342,55 +331,55 @@
     // refresh button status
     $('form').on('change keyup keypress blur mousemove', function() {
         refreshExecuteButtons();
     });
 
 
     // load workspace and enable module action tabs
-    $('#module-config-run').click(function() {
+    $('#module--BASE--run').click(function() {
         $.ajax({
             type: 'POST',
-            url: '/module/' + module + '/config',
-            data: $('#module-config').serialize(),
+            url: '/module/' + module + '/BASE',
+            data: $('#module--BASE').serialize(),
             dataType: 'json',
             cache: false,
         }).done(function(x, textStatus, jqXHR) {
             refreshModule(true);
         }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
             console.log("XMLHttpRequest : " + XMLHttpRequest.status);
             console.log("textStatus     : " + textStatus);
             console.log("errorThrown    : " + errorThrown.message);
         });
     });
 
 
     // start model training
-    $('#module-training-run').click(function() {
+    $('#module--TRAIN--run').click(function() {
         $.ajax({
             type: 'POST',
-            url: '/module/' + module + '/training',
-            data: $('#module-training').serialize(),
+            url: '/module/' + module + '/TRAIN',
+            data: $('#module--TRAIN').serialize(),
             dataType: 'json',
             cache: false,
         }).done(function(x, textStatus, jqXHR) {
             refreshModule(true);
         }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
             console.log("XMLHttpRequest : " + XMLHttpRequest.status);
             console.log("textStatus     : " + textStatus);
             console.log("errorThrown    : " + errorThrown.message);
         });
     });
 
 
     // start inference
-    $('#module-inference-run').click(function() {
+    $('#module--INFERENCE--run').click(function() {
         $.ajax({
             type: 'POST',
-            url: '/module/' + module + '/inference',
-            data: $('#module-inference').serialize(),
+            url: '/module/' + module + '/INFERENCE',
+            data: $('#module--INFERENCE').serialize(),
             dataType: 'json',
             cache: false,
         }).done(function(x, textStatus, jqXHR) {
             refreshModule(true);
         }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
             console.log("XMLHttpRequest : " + XMLHttpRequest.status);
             console.log("textStatus     : " + textStatus);
@@ -414,52 +403,27 @@
             console.log("textStatus     : " + textStatus);
             console.log("errorThrown    : " + errorThrown.message);
         });
     });
 
 
 
-    // reload NN available architectures according to the backend
-    $('#module-config-backend').on('change', function() {
-        $.ajax({
-            type: 'GET',
-            url: '/api/architecture',
-            data: {
-                module: module,
-                backend: $('#module-config-backend').val(),
-            },
-            dataType: 'json',
-            cache: false,
-        }).done(function(arch, textStatus, jqXHR) {
-            let archListHTML = '';
-            for (let i = 0; i < arch.length; i++) {
-                archListHTML = archListHTML + '<option value="' + arch[i] + '">' + arch[i] + '</option>';
-            }
-            $('#module-config-architecture').html(archListHTML);
-            refreshConfigField();
-            refreshTrainOptimizer();
-        }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
-            console.log("XMLHttpRequest : " + XMLHttpRequest.status);
-            console.log("textStatus     : " + textStatus);
-            console.log("errorThrown    : " + errorThrown.message);
-        });
-    });
-
-
     // disable config field if customized-architecture is selected
-    $('#module-config-architecture').on('change', function() {
+    $('#module--BASE--architecture').on('change', function() {
         refreshConfigField();
     });
 
 
     // open sub-window to select file/folder when clicking Select buttons
     $('button.select-file').on('click', function() {
         let _ = $(this).val().split('+');
         focusedInputField = _[0];
         let selectType = _[1];
+        let btn_id = $(this).attr('id');
+
         $.ajax({
             type: 'GET',
             url: '/api/dirtree',
             dataType: 'json',
             cache: false,
         }).done(function(dirtree, textStatus, jqXHR) {
             $('#filetree').tree('destroy');
@@ -468,20 +432,26 @@
                 closedIcon: '&#x0229E;',
                 showEmptyFolder: true,
                 autoOpen: 0,
                 selectable: true,
                 data: dirtree,
             });
             if (selectType === 'any') {
-                if ($('#module-training-annotation_format').val() === 'COCO' || $('#module-training-annotation_format').val() === 'VoTT') {
+                selectType = 'folder';
+                if ($('#module--TRAIN--trainannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--trainann--button') {
+                    selectType = 'file';
+                }
+                if ($('#module--TRAIN--validannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--validann--button') {
+                    selectType = 'file';
+                }
+                if ($('#module--TRAIN--testannfmt').val() === 'COCO' && btn_id === 'module--TRAIN--testann--button') {
                     selectType = 'file';
-                } else {
-                    selectType = 'folder';
                 }
             }
+            console.log(selectType);
             $('#filetree-required-filetype').val(selectType);
             if (selectType === 'file') {
                 $('#filetree-select-msgbox').text(msgSelectFile);
             } else {
                 $('#filetree-select-msgbox').text(msgSelectFolder);
             }
             $('#filetree-selected').val($('#' + focusedInputField).val());
@@ -546,15 +516,15 @@
 
 
     /*
     $('button#config-edition-open').on('click', function() {
         $.ajax({
             type: 'GET',
             url: '/api/modelconfig',
-            data: {config_fpath: $('#module-config-config').val()},
+            data: {config_fpath: $('#module--BASE--config').val()},
             dataType: 'json',
             cache: false,
         }).done(function(config_content, textStatus, jqXHR) {
             $('#config-edition-msgbox').text(config_content['status']);
             $('#config-edition-content').val(config_content['data']);
             $('#config-edition-popup').fadeIn();
         }).fail(function(XMLHttpRequest, textStatus, errorThrown) {
@@ -574,15 +544,15 @@
         $('#config-edition-popup').fadeOut();
     });
     $('body').on('click', '#config-edition-save', function() {
         $.ajax({
             type: 'POST',
             url: '/api/modelconfig',
             data: {
-                file_path: $('#module-config-config').val(),
+                file_path: $('#module--BASE--config').val(),
                 data: $('#config-edition-content').val()
             },
             dataType: 'json',
             cache: false,
         }).done(function(config_content, textStatus, jqXHR) {
             $('#config-edition-msgbox').fadeOut(function() {
                 $(this).text(config_content['status']).fadeIn();
@@ -595,31 +565,47 @@
             console.log("XMLHttpRequest : " + XMLHttpRequest.status);
             console.log("textStatus     : " + textStatus);
             console.log("errorThrown    : " + errorThrown.message);
         });
     });
 
 
-    $('#module-training-strategy').on('change', function() {
+    $('#module--TRAIN--strategy').on('change', function() {
         if ($(this).val() === 'resizing') {
-            $('#module-training-resizing-option').css('visibility', '').css('visibility', 'hidden');
+            $('#module--TRAIN--resizing-option').css('visibility', '').css('visibility', 'hidden');
         } else {
-            $('#module-training-resizing-option').css('visibility', '').css('visibility', 'visibile');
+            $('#module--TRAIN--resizing-option').css('visibility', '').css('visibility', 'visibile');
         }
     });
 
 
-    $('#module-inference-strategy').on('change', function() {
+    $('#module--INFERENCE--strategy').on('change', function() {
         if ($(this).val() === 'resizing') {
-            $('#module-inference-resizing-option').css('visibility', '').css('visibility', 'hidden');
+            $('#module--INFERENCE--resizing-option').css('visibility', '').css('visibility', 'hidden');
         } else {
-            $('#module-inference-resizing-option').css('visibility', '').css('visibility', 'visibile');
+            $('#module--INFERENCE--resizing-option').css('visibility', '').css('visibility', 'visibile');
         }
     });
 
+    $('#module--TRAIN--validimages,#module--TRAIN--validann').on({
+        'mouseenter': function() {
+            $(this).attr('placeholder', msgLeftBank.replace('____', 'validation'));
+        },
+        'mouseleave': function() {
+            $(this).removeAttr('placeholder');
+        }
+    });
+    $('#module--TRAIN--testimages,#module--TRAIN--testann').on({
+        'mouseenter': function() {
+            $(this).attr('placeholder', msgLeftBank.replace('____', 'test'));
+        },
+        'mouseleave': function() {
+            $(this).removeAttr('placeholder');
+        }
+    });
 });
 
 
 // check the running status and update logs
 refreshModule(true);
 window.setInterval(function() {
     refreshModule();
```

### Comparing `justdeepit-0.2.0/justdeepit/webapp/templates/index.html` & `justdeepit-0.2.1/justdeepit/app/templates/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     
     
     <a href="/module/SOD" class="card">
         <div class="card-desc"><h2>Salient Object Detection</h2></div>
     </a>
     </div>
         
-    <div id="version">JustDeepIt v{{justdeepit_version}}</div>
+    <div id="version">JustDeepIt v{{version}}</div>
     </div>
 </body> 
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 ************ JJuussttDDeeeeppIItt ************ ⊠ SHUTDOWN APP
 _**_**_**_**_**_ _OO_bb_jj_ee_cc_tt_ _DD_ee_tt_ee_cc_tt_ii_oo_nn_ _**_**_**_**_**
 _**_**_**_**_**_ _II_nn_ss_tt_aa_nn_cc_ee_ _SS_ee_gg_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _**_**_**_**_**
 _**_**_**_**_**_ _SS_aa_ll_ii_ee_nn_tt_ _OO_bb_jj_ee_cc_tt_ _DD_ee_tt_ee_cc_tt_ii_oo_nn_ _**_**_**_**_**
-JustDeepIt v{{justdeepit_version}}
+JustDeepIt v{{version}}
```

### Comparing `justdeepit-0.2.0/justdeepit/webapp/templates/shutdown.html` & `justdeepit-0.2.1/justdeepit/app/templates/shutdown.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 <body>
     <div id="app-module-panel">
     
     <h1>JustDeepIt</h1>
     
     <div id="shutdown-msg">Bye :)</div>
         
-    <div id="version">JustDeepIt v{{justdeepit_version}}</div>
+    <div id="version">JustDeepIt v{{version}}</div>
     </div>
 </body> 
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
 ************ JJuussttDDeeeeppIItt ************
 Bye :)
-JustDeepIt v{{justdeepit_version}}
+JustDeepIt v{{version}}
```

### Comparing `justdeepit-0.2.0/tests/test_det.py` & `justdeepit-0.2.1/tests/test_det.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/tests/test_segm.py` & `justdeepit-0.2.1/tests/test_segm.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/tests/test_sodmodels.py` & `justdeepit-0.2.1/tests/test_sodmodels.py`

 * *Files identical despite different names*

### Comparing `justdeepit-0.2.0/tests/test_utils.py` & `justdeepit-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

