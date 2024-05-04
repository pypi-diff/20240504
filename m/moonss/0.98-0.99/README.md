# Comparing `tmp/moonss-0.98.tar.gz` & `tmp/moonss-0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonss-0.98.tar", last modified: Thu May  2 09:49:58 2024, max compression
+gzip compressed data, was "moonss-0.99.tar", last modified: Sat May  4 08:41:06 2024, max compression
```

## Comparing `moonss-0.98.tar` & `moonss-0.99.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:49:58.716976 moonss-0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 09:49:48.000000 moonss-0.98/DownloadHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-02 09:49:58.716976 moonss-0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 09:49:48.000000 moonss-0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-02 09:49:48.000000 moonss-0.98/SourceDataHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:49:58.716976 moonss-0.98/moonss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-02 09:49:58.000000 moonss-0.98/moonss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-02 09:49:58.000000 moonss-0.98/moonss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:49:58.000000 moonss-0.98/moonss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 09:49:58.000000 moonss-0.98/moonss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 09:49:58.000000 moonss-0.98/moonss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-02 09:49:48.000000 moonss-0.98/moonss.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:49:58.716976 moonss-0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 09:49:48.000000 moonss-0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:41:06.388706 moonss-0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-04 08:40:53.000000 moonss-0.99/DownloadHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-04 08:41:06.388706 moonss-0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 08:40:53.000000 moonss-0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-04 08:40:53.000000 moonss-0.99/SourceDataHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:41:06.388706 moonss-0.99/moonss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-04 08:41:06.000000 moonss-0.99/moonss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-04 08:41:06.000000 moonss-0.99/moonss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:41:06.000000 moonss-0.99/moonss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 08:41:06.000000 moonss-0.99/moonss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 08:41:06.000000 moonss-0.99/moonss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-04 08:40:53.000000 moonss-0.99/moonss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:41:06.388706 moonss-0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-04 08:40:53.000000 moonss-0.99/setup.py
```

### Comparing `moonss-0.98/DownloadHelper.py` & `moonss-0.99/DownloadHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,9 +70,14 @@
 def donwload_artlistio_video(crawl_data_txt):
     crawl_data = json.loads(crawl_data_txt)
     if "video_m3u8" in crawl_data:
         url=crawl_data['video_m3u8'].replace("_playlist","_1080p")
         return download_ffmpeg(url)
     else:
         return None
-    
+def donwload_canva_video(crawl_data_txt):
+    crawl_data = json.loads(crawl_data_txt)
+    if "video_url" in crawl_data:
+        return download_file(crawl_data['video_url'],None, "mp4")
+    else:
+        return None
 # print(donwload_artlistio_video('{"video_url":"https:\/\/cms-artifacts.artlist.io\/content\/artgrid\/footage-hd\/1269510_hdgraded_1157601_Habitas_V1-0011.mp4?d=true&filename=218447_Woman%20Forest%20Jungle%20Smoke_By_Robert_Pilichowski_Artlist_HD.mp4&Expires=1714642023288&Key-Pair-Id=K2ZDLYDZI2R1DF&Signature=cKKt-jNIu8Ad9~J5QUbyZxJb8ycV-8eVxRHsb~F7kYLm38eFLJRj3vdWDvmwfXI0tM0KegrLuVGDk6ECDiHEbrxn52CIm5Y7fX2fdRnu3uGKttaTO0JA1K0oDOW4ctjyWQ8tud~Bi7K5L09LujhNW-60ryLz2T7F7ncZpKqLl7N2qwev2mQGmhZN2CB21VuhNdZPndRFivkBYAwNOHMn6Cpfwg3LLBPWdzCqxrXhDk6RisAyAPrfxuQCiFd2yyymJKM6ijrJBkXKleEDIe0bLUIl3A5Qucu99vJUszAT~JCbCfkspedrRLZ75~-tp3Ey5hz6eioq~xG6qbL0wMJXHA__","video_m3u8":"https:\/\/cms-public-artifacts.artlist.io\/content\/artgrid\/footage-hls\/218447_playlist.m3u8","thumbnail_url":"https:\/\/artgrid.imgix.net\/footage-graded-thumbnail\/7d29ad821b_1157601_0-second_w800px.jpeg"}'))
```

### Comparing `moonss-0.98/PKG-INFO` & `moonss-0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.98
+Version: 0.99
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.98/SourceDataHelper.py` & `moonss-0.99/SourceDataHelper.py`

 * *Files identical despite different names*

### Comparing `moonss-0.98/moonss.egg-info/PKG-INFO` & `moonss-0.99/moonss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.98
+Version: 0.99
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.98/moonss.py` & `moonss-0.99/moonss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from DownloadHelper import download_ytdlp, download_tiktok_video, download_douyin_video, donwload_instagram_video, donwload_artlistio_video
+from DownloadHelper import download_ytdlp, download_tiktok_video, download_douyin_video, donwload_instagram_video, donwload_artlistio_video, donwload_canva_video
 from SourceDataHelper import process_video_sd
 import requests
 
 URL_HOME="https://moonseo.app"
 URL_GET_JOB=f"{URL_HOME}/api/source/data/crawl"
 URL_UPDATE_JOB=f"{URL_HOME}/api/source/data/update-by-id"
 headers={"platform":"autowin"}
@@ -22,14 +22,16 @@
             video_path = download_ytdlp(obj['ori_link'])
         if obj['platform'] =='douyin':
             video_path = download_douyin_video(obj['platform_id'])
         if obj['platform'] == 'instagram':
             video_path = donwload_instagram_video(obj['crawl_data'])
         if obj['platform'] == 'artlistio':
             video_path = donwload_artlistio_video(obj['crawl_data'])
+        if obj['platform'] == 'canva':
+            video_path = donwload_canva_video(obj['crawl_data'])
         sc_new = process_video_sd(video_path)
         if not sc_new:
             sc_new={"id": obj['id']}
             if(obj['crawl_retries']<3):
                 sc_new['crawl_retries']=obj['crawl_retries']+1
                 sc_new['status'] = 1 #retries
             else:
```

### Comparing `moonss-0.98/setup.py` & `moonss-0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='moonss',
-    version='0.98',
+    version='0.99',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of moonss",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/vtandroid/dokr",
     packages=setuptools.find_packages(),
```

