# Comparing `tmp/drawlib-0.1.1.tar.gz` & `tmp/drawlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawlib-0.1.1.tar", max compression
+gzip compressed data, was "drawlib-0.1.2.tar", max compression
```

## Comparing `drawlib-0.1.1.tar` & `drawlib-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-05-01 07:22:19.104529 drawlib-0.1.1/README.md
--rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.1/drawlib/.pylintrc
--rw-r--r--   0        0        0     1039 2024-04-07 03:49:32.030240 drawlib-0.1.1/drawlib/__init__.py
--rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.1/drawlib/__main__.py
--rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.1/drawlib/apis.py
--rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.1/drawlib/assets/__init__.py
--rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.1/drawlib/assets/v0_1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.1/drawlib/assets/v0_1/fonticons/__init__.py
--rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.1/drawlib/assets/v0_1/fonts/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.1/drawlib/v0_1/__init__.py
--rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.1/drawlib/v0_1/__main__.py
--rw-r--r--   0        0        0     2438 2024-04-29 17:11:20.522452 drawlib-0.1.1/drawlib/v0_1/apis.py
--rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.1/drawlib/v0_1/private/__init__.py
--rw-r--r--   0        0        0     5949 2024-04-27 06:45:13.999149 drawlib-0.1.1/drawlib/v0_1/private/arg_validator.py
--rw-r--r--   0        0        0     6207 2024-04-27 06:44:59.377242 drawlib-0.1.1/drawlib/v0_1/private/command.py
--rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.1/drawlib/v0_1/private/core/__init__.py
--rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.1/drawlib/v0_1/private/core/colors.py
--rw-r--r--   0        0        0    13577 2024-04-28 11:41:37.164049 drawlib-0.1.1/drawlib/v0_1/private/core/dimage.py
--rw-r--r--   0        0        0    14228 2024-05-01 15:22:54.625259 drawlib-0.1.1/drawlib/v0_1/private/core/fonts.py
--rw-r--r--   0        0        0    31889 2024-04-30 02:48:39.419245 drawlib-0.1.1/drawlib/v0_1/private/core/model.py
--rw-r--r--   0        0        0     7060 2024-04-27 01:01:21.281062 drawlib-0.1.1/drawlib/v0_1/private/core/model_validator.py
--rw-r--r--   0        0        0    26872 2024-04-28 15:48:39.619919 drawlib-0.1.1/drawlib/v0_1/private/core/theme.py
--rw-r--r--   0        0        0    26316 2024-05-01 14:16:45.894958 drawlib-0.1.1/drawlib/v0_1/private/core/util.py
--rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/__init__.py
--rw-r--r--   0        0        0    20588 2024-04-29 14:29:33.370357 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/base.py
--rw-r--r--   0        0        0     2328 2024-04-29 17:11:04.449382 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/canvas.py
--rw-r--r--   0        0        0     5197 2024-04-30 01:18:42.581902 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/image.py
--rw-r--r--   0        0        0     7634 2024-04-27 05:11:32.344915 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/line.py
--rw-r--r--   0        0        0     4932 2024-04-27 01:12:47.668699 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/original_arrow.py
--rw-r--r--   0        0        0    19327 2024-04-28 07:52:54.173121 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/original_polygon.py
--rw-r--r--   0        0        0    18919 2024-04-30 01:17:49.340153 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/patches.py
--rw-r--r--   0        0        0     3862 2024-04-29 17:10:15.748016 drawlib-0.1.1/drawlib/v0_1/private/core_canvas/text.py
--rw-r--r--   0        0        0     1893 2024-05-01 15:32:01.352630 drawlib-0.1.1/drawlib/v0_1/private/download.py
--rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.1/drawlib/v0_1/private/dutil.py
--rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.1/drawlib/v0_1/private/icons/__init__.py
--rw-r--r--   0        0        0   888358 2024-05-02 12:57:38.655722 drawlib-0.1.1/drawlib/v0_1/private/icons/phosphor.py
--rw-r--r--   0        0        0     2610 2024-04-27 12:23:04.888509 drawlib-0.1.1/drawlib/v0_1/private/icons/util.py
--rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.1/drawlib/v0_1/private/logging.py
--rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.1/drawlib/v0_1/private/settings.py
--rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.1/drawlib/v0_1/private/smartarts/__init__.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.1/drawlib/v0_1/private/smartarts/cycle.py
--rw-r--r--   0        0        0      617 2024-04-14 10:51:41.389757 drawlib-0.1.1/drawlib/v0_1/private/smartarts/dsart.py
--rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.1/drawlib/v0_1/private/smartarts/groups.py
--rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.1/drawlib/v0_1/private/smartarts/pyramid.py
--rw-r--r--   0        0        0     6787 2024-05-01 15:20:41.772611 drawlib-0.1.1/drawlib/v0_1/private/smartarts/sourcecode.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.1/drawlib/v0_1/private/smartarts/table.py
--rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.1/drawlib/v0_1/private/smartarts/tree.py
--rw-r--r--   0        0        0     5807 2024-04-27 01:15:26.015254 drawlib-0.1.1/drawlib/v0_1/private/tools.py
--rw-r--r--   0        0        0    10163 2024-05-02 13:00:08.257932 drawlib-0.1.1/drawlib/v0_1/private/util.py
--rw-r--r--   0        0        0      647 2024-05-01 14:01:16.080695 drawlib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 drawlib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2038 2024-05-03 16:21:06.453599 drawlib-0.1.2/README.md
+-rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.2/drawlib/.pylintrc
+-rw-r--r--   0        0        0     1039 2024-05-02 14:31:25.994374 drawlib-0.1.2/drawlib/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.2/drawlib/__main__.py
+-rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.2/drawlib/apis.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.2/drawlib/assets/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.2/drawlib/assets/v0_1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.2/drawlib/assets/v0_1/fonticons/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.2/drawlib/assets/v0_1/fonts/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.2/drawlib/v0_1/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.2/drawlib/v0_1/__main__.py
+-rw-r--r--   0        0        0     2438 2024-04-29 17:11:20.522452 drawlib-0.1.2/drawlib/v0_1/apis.py
+-rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.2/drawlib/v0_1/private/__init__.py
+-rw-r--r--   0        0        0     5949 2024-04-27 06:45:13.999149 drawlib-0.1.2/drawlib/v0_1/private/arg_validator.py
+-rw-r--r--   0        0        0     6207 2024-04-27 06:44:59.377242 drawlib-0.1.2/drawlib/v0_1/private/command.py
+-rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.2/drawlib/v0_1/private/core/__init__.py
+-rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.2/drawlib/v0_1/private/core/colors.py
+-rw-r--r--   0        0        0    13577 2024-04-28 11:41:37.164049 drawlib-0.1.2/drawlib/v0_1/private/core/dimage.py
+-rw-r--r--   0        0        0    14228 2024-05-01 15:22:54.625259 drawlib-0.1.2/drawlib/v0_1/private/core/fonts.py
+-rw-r--r--   0        0        0    31889 2024-04-30 02:48:39.419245 drawlib-0.1.2/drawlib/v0_1/private/core/model.py
+-rw-r--r--   0        0        0     7060 2024-04-27 01:01:21.281062 drawlib-0.1.2/drawlib/v0_1/private/core/model_validator.py
+-rw-r--r--   0        0        0    26872 2024-04-28 15:48:39.619919 drawlib-0.1.2/drawlib/v0_1/private/core/theme.py
+-rw-r--r--   0        0        0    26316 2024-05-01 14:16:45.894958 drawlib-0.1.2/drawlib/v0_1/private/core/util.py
+-rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/__init__.py
+-rw-r--r--   0        0        0    20588 2024-04-29 14:29:33.370357 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/base.py
+-rw-r--r--   0        0        0     2328 2024-04-29 17:11:04.449382 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/canvas.py
+-rw-r--r--   0        0        0     5197 2024-04-30 01:18:42.581902 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/image.py
+-rw-r--r--   0        0        0     7634 2024-04-27 05:11:32.344915 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/line.py
+-rw-r--r--   0        0        0     4932 2024-04-27 01:12:47.668699 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/original_arrow.py
+-rw-r--r--   0        0        0    19327 2024-04-28 07:52:54.173121 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/original_polygon.py
+-rw-r--r--   0        0        0    18919 2024-04-30 01:17:49.340153 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/patches.py
+-rw-r--r--   0        0        0     3862 2024-04-29 17:10:15.748016 drawlib-0.1.2/drawlib/v0_1/private/core_canvas/text.py
+-rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.2/drawlib/v0_1/private/download.py
+-rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.2/drawlib/v0_1/private/dutil.py
+-rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.2/drawlib/v0_1/private/icons/__init__.py
+-rw-r--r--   0        0        0   888358 2024-05-02 12:57:38.655722 drawlib-0.1.2/drawlib/v0_1/private/icons/phosphor.py
+-rw-r--r--   0        0        0     2610 2024-04-27 12:23:04.888509 drawlib-0.1.2/drawlib/v0_1/private/icons/util.py
+-rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.2/drawlib/v0_1/private/logging.py
+-rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.2/drawlib/v0_1/private/settings.py
+-rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.2/drawlib/v0_1/private/smartarts/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.2/drawlib/v0_1/private/smartarts/cycle.py
+-rw-r--r--   0        0        0      617 2024-04-14 10:51:41.389757 drawlib-0.1.2/drawlib/v0_1/private/smartarts/dsart.py
+-rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.2/drawlib/v0_1/private/smartarts/groups.py
+-rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.2/drawlib/v0_1/private/smartarts/pyramid.py
+-rw-r--r--   0        0        0     6787 2024-05-01 15:20:41.772611 drawlib-0.1.2/drawlib/v0_1/private/smartarts/sourcecode.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.2/drawlib/v0_1/private/smartarts/table.py
+-rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.2/drawlib/v0_1/private/smartarts/tree.py
+-rw-r--r--   0        0        0     5807 2024-04-27 01:15:26.015254 drawlib-0.1.2/drawlib/v0_1/private/tools.py
+-rw-r--r--   0        0        0    10163 2024-05-02 13:00:08.257932 drawlib-0.1.2/drawlib/v0_1/private/util.py
+-rw-r--r--   0        0        0      758 2024-05-03 16:56:12.484006 drawlib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 drawlib-0.1.2/PKG-INFO
```

### Comparing `drawlib-0.1.1/LICENSE.txt` & `drawlib-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/__init__.py` & `drawlib-0.1.2/drawlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 - drawlib.v0_1: API v0.1 interface (latest)
 
 """
 
 from typing import Final
 
 # please update here when you release new version
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 
 # might not be changed
 LIB_NAME: Final[str] = "drawlib"
 AUTHOR: Final[str] = "Yuichi Ito"
 CONTACT: Final[str] = "yuichi@yuichi.com"
 __version__: Final[str] = VERSION
```

### Comparing `drawlib-0.1.1/drawlib/__main__.py` & `drawlib-0.1.2/drawlib/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/apis.py` & `drawlib-0.1.2/drawlib/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/__init__.py` & `drawlib-0.1.2/drawlib/v0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/__main__.py` & `drawlib-0.1.2/drawlib/v0_1/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/apis.py` & `drawlib-0.1.2/drawlib/v0_1/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/__init__.py` & `drawlib-0.1.2/drawlib/v0_1/private/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/arg_validator.py` & `drawlib-0.1.2/drawlib/v0_1/private/arg_validator.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/command.py` & `drawlib-0.1.2/drawlib/v0_1/private/command.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/__init__.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/colors.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/colors.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/dimage.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/dimage.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/fonts.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/fonts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/model.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/model.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/model_validator.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/model_validator.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/theme.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/theme.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core/util.py` & `drawlib-0.1.2/drawlib/v0_1/private/core/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/__init__.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/base.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/base.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/canvas.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/image.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/image.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/line.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/original_arrow.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/original_arrow.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/original_polygon.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/original_polygon.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/patches.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/patches.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/core_canvas/text.py` & `drawlib-0.1.2/drawlib/v0_1/private/core_canvas/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/dutil.py` & `drawlib-0.1.2/drawlib/v0_1/private/dutil.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/icons/__init__.py` & `drawlib-0.1.2/drawlib/v0_1/private/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/icons/phosphor.py` & `drawlib-0.1.2/drawlib/v0_1/private/icons/phosphor.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/icons/util.py` & `drawlib-0.1.2/drawlib/v0_1/private/icons/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/logging.py` & `drawlib-0.1.2/drawlib/v0_1/private/logging.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/settings.py` & `drawlib-0.1.2/drawlib/v0_1/private/settings.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/smartarts/__init__.py` & `drawlib-0.1.2/drawlib/v0_1/private/smartarts/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/smartarts/dsart.py` & `drawlib-0.1.2/drawlib/v0_1/private/smartarts/dsart.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/smartarts/groups.py` & `drawlib-0.1.2/drawlib/v0_1/private/smartarts/groups.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/smartarts/pyramid.py` & `drawlib-0.1.2/drawlib/v0_1/private/smartarts/pyramid.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/smartarts/sourcecode.py` & `drawlib-0.1.2/drawlib/v0_1/private/smartarts/sourcecode.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/smartarts/tree.py` & `drawlib-0.1.2/drawlib/v0_1/private/smartarts/tree.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/tools.py` & `drawlib-0.1.2/drawlib/v0_1/private/tools.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/drawlib/v0_1/private/util.py` & `drawlib-0.1.2/drawlib/v0_1/private/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.1/pyproject.toml` & `drawlib-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+[build-system]
+requires = [ "poetry-core",]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "drawlib"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python drawing library. Illustration as Code."
-authors = ["Yuichi Ito <yuichi@yuichi.com>"]
+homepage = "https://www.drawlib.com"
+repository = "https://github.com/yuichi110/drawlib"
+authors = [ "Yuichi Ito <yuichi@yuichi.com>",]
 readme = "README.md"
 
+[tool.black]
+line-length = 120
+
 [tool.poetry.dependencies]
 python = "^3.9"
 matplotlib = "^3.8.3"
 pygments = "^2.17.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
@@ -18,14 +27,8 @@
 types-pillow = "^10.2.0.20240311"
 radon = "^6.0.1"
 bandit = "^1.7.8"
 pytest-cov = "^5.0.0"
 pydocstyle = "^6.3.0"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
-
-[tool.black]
-line-length = 120
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+toml = "^0.10.2"
```

