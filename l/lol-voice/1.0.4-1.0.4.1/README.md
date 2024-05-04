# Comparing `tmp/lol_voice-1.0.4.tar.gz` & `tmp/lol_voice-1.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol_voice-1.0.4.tar", max compression
+gzip compressed data, was "lol_voice-1.0.4.1.tar", max compression
```

## Comparing `lol_voice-1.0.4.tar` & `lol_voice-1.0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35823 2021-03-02 14:13:12.355748 lol_voice-1.0.4/LICENSE
--rw-r--r--   0        0        0      466 2022-08-25 16:39:22.355478 lol_voice-1.0.4/lol_voice/__init__.py
--rw-r--r--   0        0        0     3763 2022-08-25 16:51:23.688081 lol_voice-1.0.4/lol_voice/base.py
--rw-r--r--   0        0        0      416 2022-08-25 16:39:07.182000 lol_voice-1.0.4/lol_voice/formats/__init__.py
--rw-r--r--   0        0        0     6158 2024-01-14 07:39:03.993615 lol_voice-1.0.4/lol_voice/formats/BIN.py
--rw-r--r--   0        0        0     2268 2022-08-25 16:51:23.689082 lol_voice-1.0.4/lol_voice/formats/BNK.py
--rw-r--r--   0        0        0      404 2022-08-25 16:51:23.692084 lol_voice-1.0.4/lol_voice/formats/section/__init__.py
--rw-r--r--   0        0        0     1186 2022-08-25 16:51:23.690083 lol_voice-1.0.4/lol_voice/formats/section/BKHD.py
--rw-r--r--   0        0        0     1356 2022-08-25 16:51:23.690083 lol_voice-1.0.4/lol_voice/formats/section/DATA.py
--rw-r--r--   0        0        0     1202 2022-08-25 16:51:23.691084 lol_voice-1.0.4/lol_voice/formats/section/DIDX.py
--rw-r--r--   0        0        0    15751 2022-08-26 17:31:43.212575 lol_voice-1.0.4/lol_voice/formats/section/HIRC.py
--rw-r--r--   0        0        0     5817 2022-08-25 16:51:23.689082 lol_voice-1.0.4/lol_voice/formats/WAD.py
--rw-r--r--   0        0        0     1691 2022-08-25 16:39:22.631724 lol_voice-1.0.4/lol_voice/formats/WPK.py
--rw-r--r--   0        0        0    12760 2024-01-14 07:42:29.005727 lol_voice-1.0.4/lol_voice/index.py
--rw-r--r--   0        0        0      250 2022-08-25 16:39:07.184001 lol_voice-1.0.4/lol_voice/tools/__init__.py
--rw-r--r--   0        0        0       89 2022-08-25 16:39:07.183000 lol_voice-1.0.4/lol_voice/tools/Binary/__init__.py
--rw-r--r--   0        0        0     4728 2022-10-10 12:47:34.537784 lol_voice-1.0.4/lol_voice/tools/Binary/reader.py
--rw-r--r--   0        0        0     1376 2024-01-14 07:50:14.631957 lol_voice-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3614 2022-08-25 16:39:22.772849 lol_voice-1.0.4/README.md
--rw-r--r--   0        0        0       30 2021-03-03 11:59:19.672290 lol_voice-1.0.4/requirements.txt
--rw-r--r--   0        0        0     4701 1970-01-01 00:00:00.000000 lol_voice-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-05-04 11:11:14.280139 lol_voice-1.0.4.1/LICENSE
+-rw-r--r--   0        0        0      466 2024-05-04 11:11:14.281140 lol_voice-1.0.4.1/lol_voice/__init__.py
+-rw-r--r--   0        0        0     3763 2024-05-04 11:11:14.281140 lol_voice-1.0.4.1/lol_voice/base.py
+-rw-r--r--   0        0        0      416 2024-05-04 11:11:14.284143 lol_voice-1.0.4.1/lol_voice/formats/__init__.py
+-rw-r--r--   0        0        0     6158 2024-05-04 11:11:14.282141 lol_voice-1.0.4.1/lol_voice/formats/BIN.py
+-rw-r--r--   0        0        0     2268 2024-05-04 11:11:14.283142 lol_voice-1.0.4.1/lol_voice/formats/BNK.py
+-rw-r--r--   0        0        0      404 2024-05-04 11:11:14.286144 lol_voice-1.0.4.1/lol_voice/formats/section/__init__.py
+-rw-r--r--   0        0        0     1186 2024-05-04 11:11:14.284143 lol_voice-1.0.4.1/lol_voice/formats/section/BKHD.py
+-rw-r--r--   0        0        0     1356 2024-05-04 11:11:14.285144 lol_voice-1.0.4.1/lol_voice/formats/section/DATA.py
+-rw-r--r--   0        0        0     1202 2024-05-04 11:11:14.285144 lol_voice-1.0.4.1/lol_voice/formats/section/DIDX.py
+-rw-r--r--   0        0        0    15751 2024-05-04 11:11:40.506158 lol_voice-1.0.4.1/lol_voice/formats/section/HIRC.py
+-rw-r--r--   0        0        0     5817 2024-05-04 11:11:14.283142 lol_voice-1.0.4.1/lol_voice/formats/WAD.py
+-rw-r--r--   0        0        0     1691 2024-05-04 11:11:14.283142 lol_voice-1.0.4.1/lol_voice/formats/WPK.py
+-rw-r--r--   0        0        0    12922 2024-05-04 11:23:21.010176 lol_voice-1.0.4.1/lol_voice/index.py
+-rw-r--r--   0        0        0      250 2024-05-04 11:11:14.288146 lol_voice-1.0.4.1/lol_voice/tools/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-04 11:11:14.287145 lol_voice-1.0.4.1/lol_voice/tools/Binary/__init__.py
+-rw-r--r--   0        0        0     4728 2024-05-04 11:11:40.508161 lol_voice-1.0.4.1/lol_voice/tools/Binary/reader.py
+-rw-r--r--   0        0        0     1378 2024-05-04 11:42:20.359538 lol_voice-1.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3816 2024-05-04 11:24:39.967186 lol_voice-1.0.4.1/README.md
+-rw-r--r--   0        0        0       30 2024-05-04 11:11:14.288146 lol_voice-1.0.4.1/requirements.txt
+-rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 lol_voice-1.0.4.1/PKG-INFO
```

### Comparing `lol_voice-1.0.4/LICENSE` & `lol_voice-1.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/base.py` & `lol_voice-1.0.4.1/lol_voice/base.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/BIN.py` & `lol_voice-1.0.4.1/lol_voice/formats/BIN.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/BNK.py` & `lol_voice-1.0.4.1/lol_voice/formats/BNK.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/section/BKHD.py` & `lol_voice-1.0.4.1/lol_voice/formats/section/BKHD.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/section/DATA.py` & `lol_voice-1.0.4.1/lol_voice/formats/section/DATA.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/section/DIDX.py` & `lol_voice-1.0.4.1/lol_voice/formats/section/DIDX.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/section/HIRC.py` & `lol_voice-1.0.4.1/lol_voice/formats/section/HIRC.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/WAD.py` & `lol_voice-1.0.4.1/lol_voice/formats/WAD.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/formats/WPK.py` & `lol_voice-1.0.4.1/lol_voice/formats/WPK.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/lol_voice/index.py` & `lol_voice-1.0.4.1/lol_voice/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,34 @@
 # @Update  : 2024/1/14 15:42
 # @Detail  : 
 
 # References : http://wiki.xentax.com/index.php/Wwise_SoundBank_(*.bnk)#HIRC_section
 
 import logging
 import os
+import warnings
 from collections import OrderedDict, defaultdict
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import List, Optional, Union
 
 from loguru import logger
 
 from lol_voice.base import WemFile
 from lol_voice.formats.BIN import BIN, StringHash
 from lol_voice.formats.BNK import BNK, HIRC
 from lol_voice.formats.WPK import WPK
 from lol_voice.tools.Binary import BinaryReader
 
+warnings.warn(
+    "Package 'lol-voice' is deprecated. Please use 'league-tools' instead.",
+    DeprecationWarning,
+    stacklevel=2,
+)
+
+
 
 def get_audio_id_by_songs(event_str, event_id, songs):
     """
     根据ID在Sound列表(迭代器)生成资源ID列表
     :param event_str:
     :param event_id:
     :param songs:
```

### Comparing `lol_voice-1.0.4/lol_voice/tools/Binary/reader.py` & `lol_voice-1.0.4.1/lol_voice/tools/Binary/reader.py`

 * *Files identical despite different names*

### Comparing `lol_voice-1.0.4/pyproject.toml` & `lol_voice-1.0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lol-voice"
-version = "1.0.4"
+version = "1.0.4.1"
 readme = "README.md"
 license = 'GPL-3.0-only'
 authors = ["Virace <Virace@aliyun.com>"]
 description = "通过解析英雄联盟游戏内WAD、BNK、WPK、BIN等文件来提取音频文件，并可以按照触发事件分类"
 homepage = "https://github.com/Virace/py-bnk-extract"
 repository = "https://github.com/Virace/py-bnk-extract"
 keywords = ["league", "wad", "bnk"]
```

### Comparing `lol_voice-1.0.4/README.md` & `lol_voice-1.0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,20 @@
+当前仓库已转移到https://github.com/Virace/league-tools
+
+当前仓库已转移到https://github.com/Virace/league-tools
+
+当前仓库已转移到https://github.com/Virace/league-tools
+
+
 # py-bnk-extract
 
 英雄联盟语音解包工具, 由Python语言编写.
 
 
+
 - [介绍](#介绍)
 - [安装](#安装)
 - [使用](#使用)
 - [问题](#问题)
 - [维护者](#维护者)
 - [感谢](#感谢)
 - [许可证](#许可证)
```

### Comparing `lol_voice-1.0.4/PKG-INFO` & `lol_voice-1.0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lol-voice
-Version: 1.0.4
+Version: 1.0.4.1
 Summary: 通过解析英雄联盟游戏内WAD、BNK、WPK、BIN等文件来提取音频文件，并可以按照触发事件分类
 Home-page: https://github.com/Virace/py-bnk-extract
 License: GPL-3.0-only
 Keywords: league,wad,bnk
 Author: Virace
 Author-email: Virace@aliyun.com
 Requires-Python: >=3.8
@@ -13,27 +13,36 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: xxhash (>=3.0.0,<4.0.0)
 Requires-Dist: zstd (>=1.5.2.5,<2.0.0.0)
 Project-URL: Bug Tracker, https://github.com/Virace/py-bnk-extract/issues
 Project-URL: Repository, https://github.com/Virace/py-bnk-extract
 Description-Content-Type: text/markdown
 
+当前仓库已转移到https://github.com/Virace/league-tools
+
+当前仓库已转移到https://github.com/Virace/league-tools
+
+当前仓库已转移到https://github.com/Virace/league-tools
+
+
 # py-bnk-extract
 
 英雄联盟语音解包工具, 由Python语言编写.
 
 
+
 - [介绍](#介绍)
 - [安装](#安装)
 - [使用](#使用)
 - [问题](#问题)
 - [维护者](#维护者)
 - [感谢](#感谢)
 - [许可证](#许可证)
```

