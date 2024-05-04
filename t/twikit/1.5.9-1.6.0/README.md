# Comparing `tmp/twikit-1.5.9.tar.gz` & `tmp/twikit-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.9.tar", last modified: Sun Apr 28 13:04:44 2024, max compression
+gzip compressed data, was "twikit-1.6.0.tar", last modified: Fri May  3 14:37:19 2024, max compression
```

## Comparing `twikit-1.5.9.tar` & `twikit-1.6.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.979653 twikit-1.5.9/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.9/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-28 13:04:44.977661 twikit-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 13:04:44.979653 twikit-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-26 14:47:36.000000 twikit-1.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.909846 twikit-1.5.9/twikit/
--rw-rw-rw-   0        0        0      658 2024-04-28 13:04:06.000000 twikit-1.5.9/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.9/twikit/bookmark.py
--rw-rw-rw-   0        0        0   139609 2024-04-25 17:33:46.000000 twikit-1.5.9/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.9/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.9/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.9/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.9/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-25 14:48:07.000000 twikit-1.5.9/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.9/twikit/py.typed
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/trend.py
--rw-rw-rw-   0        0        0    23812 2024-04-28 13:02:12.000000 twikit-1.5.9/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.974668 twikit-1.5.9/twikit/twikit_async/
--rw-rw-rw-   0        0        0      610 2024-04-25 17:56:33.000000 twikit-1.5.9/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.9/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   141857 2024-04-26 13:42:52.000000 twikit-1.5.9/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-26 13:28:49.000000 twikit-1.5.9/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.9/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    23693 2024-04-28 13:01:46.000000 twikit-1.5.9/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-26 13:32:10.000000 twikit-1.5.9/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.9/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.9/twikit/user.py
--rw-rw-rw-   0        0        0    30253 2024-04-25 02:12:28.000000 twikit-1.5.9/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:04:44.927796 twikit-1.5.9/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 13:04:44.000000 twikit-1.5.9/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.606418 twikit-1.6.0/
+-rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3999 2024-05-03 14:37:19.604424 twikit-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3728 2024-05-01 18:21:05.000000 twikit-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 14:37:19.607416 twikit-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-05-01 18:21:05.000000 twikit-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.521647 twikit-1.6.0/twikit/
+-rw-rw-rw-   0        0        0      658 2024-05-03 14:32:19.000000 twikit-1.6.0/twikit/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   144654 2024-05-03 13:12:28.000000 twikit-1.6.0/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/community.py
+-rw-rw-rw-   0        0        0     2666 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/group.py
+-rw-rw-rw-   0        0        0     2218 2024-05-02 13:58:54.000000 twikit-1.6.0/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/py.typed
+-rw-rw-rw-   0        0        0     8065 2024-05-03 14:13:32.000000 twikit-1.6.0/twikit/streaming.py
+-rw-rw-rw-   0        0        0     1070 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/trend.py
+-rw-rw-rw-   0        0        0    23780 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.599436 twikit-1.6.0/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      610 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   147077 2024-05-03 13:20:37.000000 twikit-1.6.0/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2260 2024-05-03 13:08:32.000000 twikit-1.6.0/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     8192 2024-05-03 14:16:39.000000 twikit-1.6.0/twikit/twikit_async/streaming.py
+-rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    23661 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/user.py
+-rw-rw-rw-   0        0        0    30547 2024-05-02 18:47:12.000000 twikit-1.6.0/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.541592 twikit-1.6.0/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3999 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.9/LICENSE` & `twikit-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/PKG-INFO` & `twikit-1.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.9
+Version: 1.6.0
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,15 +28,15 @@
 
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
 
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
 
 
-If you have any questions, please ask on [Discord](https://discord.gg/nCrByrr8cX).
+If you have any questions, you can ask on [Discord](https://discord.gg/nCrByrr8cX).
 
 
 
 ## Features
 
 ### No API Key Required
 
@@ -124,22 +124,26 @@
     print(
         tweet.user.name,
         tweet.text,
         tweet.created_at
     )
 ```
 
+**Retrieve user tweets**
+```python
+tweets = client.get_user_tweets('123456', 'Tweet')
 
-More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
-
+for tweet in tweets:
+    print(tweet.text)
+```
 
+More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
 ## Contributing
 
 I would like to hear your thoughts and suggestions.
 
 If you have any features you'd like to see added or encounter any issues,
 
 please let me know in the [issues](https://github.com/d60/twikit/issues) section.
 
-
 Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
```

### Comparing `twikit-1.5.9/README.md` & `twikit-1.6.0/twikit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: twikit
+Version: 1.6.0
+Summary: Twitter API wrapper for python with **no API key required**.
+Home-page: https://github.com/d60/twikit
+License: MIT
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
 
 
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
@@ -18,15 +28,15 @@
 
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
 
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
 
 
-If you have any questions, please ask on [Discord](https://discord.gg/nCrByrr8cX).
+If you have any questions, you can ask on [Discord](https://discord.gg/nCrByrr8cX).
 
 
 
 ## Features
 
 ### No API Key Required
 
@@ -114,22 +124,26 @@
     print(
         tweet.user.name,
         tweet.text,
         tweet.created_at
     )
 ```
 
+**Retrieve user tweets**
+```python
+tweets = client.get_user_tweets('123456', 'Tweet')
 
-More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
-
+for tweet in tweets:
+    print(tweet.text)
+```
 
+More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
 ## Contributing
 
 I would like to hear your thoughts and suggestions.
 
 If you have any features you'd like to see added or encounter any issues,
 
 please let me know in the [issues](https://github.com/d60/twikit/issues) section.
 
-
-Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
+Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
```

### Comparing `twikit-1.5.9/setup.py` & `twikit-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/__init__.py` & `twikit-1.6.0/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.9'
+__version__ = '1.6.0'
 
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
```

### Comparing `twikit-1.5.9/twikit/bookmark.py` & `twikit-1.6.0/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/client.py` & `twikit-1.6.0/twikit/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
 
 import io
 import json
 import time
 import warnings
 from functools import partial
-from typing import Literal
+from typing import Generator, Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
 from .bookmark import BookmarkFolder
 from .community import Community, CommunityMember
 from .errors import (
     CouldNotTweet,
     InvalidMedia,
-    TweetNotAvailable,
     TwitterException,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
+from .streaming import Payload, StreamingSession, _payload_from_data
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import (
     BOOKMARK_FOLDER_TIMELINE_FEATURES,
     COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
     JOIN_COMMUNITY_FEATURES,
@@ -611,15 +611,16 @@
 
     def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
         status_check_interval: float = 1.0,
         media_type: str | None = None,
-        media_category: str | None = None
+        media_category: str | None = None,
+        is_long_video: bool = False
     ) -> str:
         """
         Uploads media to twitter.
 
         Parameters
         ----------
         source : :class:`str` | :class:`bytes`
@@ -631,14 +632,17 @@
             The interval (in seconds) to check the status of the
             media upload process.
         media_type : :class:`str`, default=None
             The MIME type of the media.
             If not specified, it will be guessed from the source.
         media_category : :class:`str`, default=None
             The media category.
+        is_long_video : :class:`bool`, default=False
+            If this is True, videos longer than 2:20 can be uploaded.
+            (Twitter Premium only)
 
         Returns
         -------
         :class:`str`
             The media ID of the uploaded media.
 
         Examples
@@ -685,26 +689,31 @@
                         "`media_category` must be specified to check the "
                         "upload status of gif images ('dm_gif' or 'tweet_gif')"
                     )
             elif media_type.startswith('image'):
                 # Checking the upload status of an image is impossible.
                 wait_for_completion = False
 
+        if is_long_video:
+            endpoint = Endpoint.UPLOAD_MEDIA_2
+        else:
+            endpoint = Endpoint.UPLOAD_MEDIA
+
         total_bytes = len(binary)
 
         # ============ INIT =============
         params = {
             'command': 'INIT',
             'total_bytes': total_bytes,
             'media_type': media_type
         }
         if media_category is not None:
             params['media_category'] = media_category
         response = self.http.post(
-            Endpoint.UPLOAD_MEDIA,
+            endpoint,
             params=params,
             headers=self._base_headers
         ).json()
         media_id = response['media_id']
         # =========== APPEND ============
         segment_index = 0
         bytes_sent = 0
@@ -724,15 +733,15 @@
                 'media': (
                     'blob',
                     chunk_stream,
                     'application/octet-stream',
                 )
             }
             self.http.post(
-                Endpoint.UPLOAD_MEDIA,
+                endpoint,
                 params=params,
                 headers=headers,
                 files=files
             )
 
             chunk_stream.close()
             segment_index += 1
@@ -740,32 +749,34 @@
 
         # ========== FINALIZE ===========
         params = {
             'command': 'FINALIZE',
             'media_id': media_id,
         }
         self.http.post(
-            Endpoint.UPLOAD_MEDIA,
+            endpoint,
             params=params,
             headers=self._base_headers,
         )
 
         if wait_for_completion:
             while True:
-                state = self.check_media_status(media_id)
+                state = self.check_media_status(media_id, is_long_video)
                 processing_info = state['processing_info']
                 if 'error' in processing_info:
                     raise InvalidMedia(processing_info['error'].get('message'))
                 if processing_info['state'] == 'succeeded':
                     break
                 time.sleep(status_check_interval)
 
         return media_id
 
-    def check_media_status(self, media_id: str) -> dict:
+    def check_media_status(
+        self, media_id: str, is_long_video: bool = False
+    ) -> dict:
         """
         Check the status of uploaded media.
 
         Parameters
         ----------
         media_id : :class:`str`
             The media ID of the uploaded media.
@@ -776,16 +787,20 @@
             A dictionary containing information about the status of
             the uploaded media.
         """
         params = {
             'command': 'STATUS',
             'media_id': media_id
         }
+        if is_long_video:
+            endpoint = Endpoint.UPLOAD_MEDIA_2
+        else:
+            endpoint = Endpoint.UPLOAD_MEDIA
         response = self.http.get(
-            Endpoint.UPLOAD_MEDIA,
+            endpoint,
             params=params,
             headers=self._base_headers
         ).json()
         return response
 
     def create_media_metadata(
         self,
@@ -2943,15 +2958,15 @@
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY'
         }
         if max_id is not None:
             params['max_id'] = max_id
 
         return self.http.get(
-            Endpoint.CONVERSASION.format(conversation_id),
+            Endpoint.CONVERSATION.format(conversation_id),
             params=params,
             headers=self._base_headers
         ).json()
 
     def send_dm(
         self,
         user_id: str,
@@ -3320,15 +3335,15 @@
             An object representing the retrieved group.
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY',
             'include_conversation_info': True,
         }
         response = self.http.get(
-            Endpoint.CONVERSASION.format(group_id),
+            Endpoint.CONVERSATION.format(group_id),
             params=params,
             headers=self._base_headers
         ).json()
         return Group(self, group_id, response)
 
     def add_members_to_group(
         self, group_id: str, user_ids: list[str]
@@ -4572,7 +4587,125 @@
             partial(self.search_community_tweet, community_id,
                     query, count, next_cursor),
             next_cursor,
             partial(self.search_community_tweet, community_id,
                     query, count, previous_cursor),
             previous_cursor,
         )
+
+    def _stream(self, topics: set[str]) -> Generator[tuple[str, Payload]]:
+        headers = self._base_headers
+        headers.pop('content-type')
+        params = {'topics': ','.join(topics)}
+
+        with self.http.stream(
+            'GET', Endpoint.EVENTS, params=params, timeout=None
+        ) as response:
+            self.http._remove_duplicate_ct0_cookie()
+            for line in response.iter_lines():
+                try:
+                    data = json.loads(line)
+                except json.JSONDecodeError:
+                    continue
+                payload = _payload_from_data(data['payload'])
+                yield data.get('topic'), payload
+
+    def get_streaming_session(
+        self, topics: set[str], auto_reconnect: bool = True
+    ) -> StreamingSession:
+        """
+        Returns a session for interacting with the streaming API.
+
+        Parameters
+        ----------
+        topics : set[:class:`str`]
+            The set of topics to stream.
+            Topics can be generated using :class:`.Topic`.
+        auto_reconnect : :class:`bool`, default=True
+            Whether to automatically reconnect when disconnected.
+
+        Returns
+        -------
+        :class:`.StreamingSession`
+            A stream session instance.
+
+        Examples
+        --------
+        >>> from twikit.streaming import Topic
+        >>>
+        >>> topics = {
+        ...     Topic.tweet_engagement('1739617652'), # Stream tweet engagement
+        ...     Topic.dm_update('17544932482-174455537996'), # Stream DM update
+        ...     Topic.dm_typing('17544932482-174455537996') # Stream DM typing
+        ... }
+        >>> session = client.get_streaming_session(topics)
+        >>>
+        >>> for topic, payload in session:
+        ...     if payload.dm_update:
+        ...         conversation_id = payload.dm_update.conversation_id
+        ...         user_id = payload.dm_update.user_id
+        ...         print(f'{conversation_id}: {user_id} sent a message')
+        >>>
+        >>>     if payload.dm_typing:
+        ...         conversation_id = payload.dm_typing.conversation_id
+        ...         user_id = payload.dm_typing.user_id
+        ...         print(f'{conversation_id}: {user_id} is typing')
+        >>>
+        >>>     if payload.tweet_engagement:
+        ...         like = payload.tweet_engagement.like_count
+        ...         retweet = payload.tweet_engagement.retweet_count
+        ...         view = payload.tweet_engagement.view_count
+        ...         print('Tweet engagement updated:'
+        ...               f'likes: {like} retweets: {retweet} views: {view}')
+
+        Topics to stream can be added or deleted using
+        :attr:`.StreamingSession.update_subscriptions` method.
+
+        >>> subscribe_topics = {
+        ...     Topic.tweet_engagement('1749528513'),
+        ...     Topic.tweet_engagement('1765829534')
+        ... }
+        >>> unsubscribe_topics = {
+        ...     Topic.tweet_engagement('1739617652'),
+        ...     Topic.dm_update('17544932482-174455537996'),
+        ...     Topic.dm_update('17544932482-174455537996')
+        ... }
+        >>> session.update_subscriptions(subscribe_topics, unsubscribe_topics)
+
+        See Also
+        --------
+        .StreamingSession
+        .StreamingSession.update_subscriptions
+        .Payload
+        .Topic
+        """
+        stream = self._stream(topics)
+        session_id = next(stream)[1].config.session_id
+        return StreamingSession(
+            self, session_id, stream, topics, auto_reconnect
+        )
+
+    def _update_subscriptions(
+        self,
+        session: StreamingSession,
+        subscribe: set[str] | None = None,
+        unsubscribe: set[str] | None = None
+    ) -> Payload:
+        if subscribe is None:
+            subscribe = set()
+        if unsubscribe is None:
+            unsubscribe = set()
+
+        data = urlencode({
+            'sub_topics': ','.join(subscribe),
+            'unsub_topics': ','.join(unsubscribe)
+        })
+        headers = self._base_headers
+        headers['content-type'] = 'application/x-www-form-urlencoded'
+        headers['LivePipeline-Session'] = session.id
+        response = self.http.post(
+            Endpoint.UPDATE_SUBSCRIPTIONS, data=data, headers=headers
+        ).json()
+        session.topics |= subscribe
+        session.topics -= unsubscribe
+
+        return _payload_from_data(response)
```

### Comparing `twikit-1.5.9/twikit/community.py` & `twikit-1.6.0/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/errors.py` & `twikit-1.6.0/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/group.py` & `twikit-1.6.0/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/http.py` & `twikit-1.6.0/twikit/http.py`

 * *Files 25% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 
     def get(self, url, **kwargs) -> httpx.Response:
         return self.request('GET', url, **kwargs)
 
     def post(self, url, **kwargs) -> httpx.Response:
         return self.request('POST', url, **kwargs)
 
+    def stream(self, *args, **kwargs):
+        response = self.client.stream(*args, **kwargs)
+        return response
+
     def _remove_duplicate_ct0_cookie(self) -> None:
         cookies = {}
         for cookie in self.client.cookies.jar:
             if 'ct0' in cookies and cookie.name == 'ct0':
                 continue
             cookies[cookie.name] = cookie.value
         self.client.cookies = list(cookies.items())
```

### Comparing `twikit-1.5.9/twikit/list.py` & `twikit-1.6.0/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/message.py` & `twikit-1.6.0/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/notification.py` & `twikit-1.6.0/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/trend.py` & `twikit-1.6.0/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/tweet.py` & `twikit-1.6.0/twikit/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,27 +133,37 @@
             self.retweeted_tweet: Tweet = Tweet(
                 client, retweeted_tweet, retweeted_user
             )
         else:
             self.retweeted_tweet = None
 
         note_tweet_results = find_dict(data, 'note_tweet_results')
-        self.full_text: str | None = None
+        self.full_text: str = self.text
         if note_tweet_results:
             text_list = find_dict(note_tweet_results, 'text')
             if text_list:
                 self.full_text = text_list[0]
 
+            entity_set = note_tweet_results[0]['result']['entity_set']
+            self.urls: list = entity_set.get('urls')
+            hashtags = entity_set.get('hashtags', [])
+        else:
+            self.urls: list = legacy['entities'].get('urls')
+            hashtags = legacy['entities'].get('hashtags', [])
+
+        self.hashtags: list[str] = [
+            i['text'] for i in hashtags
+        ]
+
         self.is_quote_status: bool = legacy['is_quote_status']
         self.possibly_sensitive: bool = legacy.get('possibly_sensitive')
         self.possibly_sensitive_editable: bool = legacy.get(
             'possibly_sensitive_editable')
         self.quote_count: int = legacy['quote_count']
         self.media: list = legacy['entities'].get('media')
-        self.urls: list = legacy['entities'].get('urls')
         self.reply_count: int = legacy['reply_count']
         self.favorite_count: int = legacy['favorite_count']
         self.favorited: bool = legacy['favorited']
         self.view_count: int = (data['views'].get('count')
                                 if 'views' in data else None)
         self.retweet_count: int = legacy['retweet_count']
         self.editable_until_msecs: int = data['edit_control'].get(
@@ -171,26 +181,14 @@
             community_note_data = data['birdwatch_pivot']
             if 'note' in community_note_data:
                 self.community_note = {
                     'id': community_note_data['note']['rest_id'],
                     'text': community_note_data['subtitle']['text']
                 }
 
-        if note_tweet_results:
-            hashtags_ = find_dict(note_tweet_results, 'hashtags')
-            if hashtags_:
-                hashtags = hashtags_[0]
-            else:
-                hashtags = []
-        else:
-            hashtags = legacy['entities'].get('hashtags', [])
-        self.hashtags: list[str] = [
-            i['text'] for i in hashtags
-        ]
-
         if (
             'card' in data and
             'legacy' in data['card'] and
             'name' in data['card']['legacy'] and
             data['card']['legacy']['name'].startswith('poll')
         ):
             self._poll_data = data['card']
```

### Comparing `twikit-1.5.9/twikit/twikit_async/__init__.py` & `twikit-1.6.0/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/bookmark.py` & `twikit-1.6.0/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/client.py` & `twikit-1.6.0/twikit/twikit_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import json
 import warnings
 from functools import partial
-from typing import Literal
+from typing import AsyncGenerator, Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
 from ..errors import (
     CouldNotTweet,
     InvalidMedia,
-    TweetNotAvailable,
     TwitterException,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from ..utils import (
     BOOKMARK_FOLDER_TIMELINE_FEATURES,
@@ -46,14 +45,15 @@
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
+from .streaming import Payload, StreamingSession, _payload_from_data
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import Flow, Result
 
 
 class Client:
     """
@@ -616,15 +616,16 @@
 
     async def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
         status_check_interval: float = 1.0,
         media_type: str | None = None,
-        media_category: str | None = None
+        media_category: str | None = None,
+        is_long_video: bool = False
     ) -> str:
         """
         Uploads media to twitter.
 
         Parameters
         ----------
         source : :class:`str` | :class:`bytes`
@@ -636,14 +637,17 @@
             The interval (in seconds) to check the status of the
             media upload process.
         media_type : :class:`str`, default=None
             The MIME type of the media.
             If not specified, it will be guessed from the source.
         media_category : :class:`str`, default=None
             The media category.
+        is_long_video : :class:`bool`, default=False
+            If this is True, videos longer than 2:20 can be uploaded.
+            (Twitter Premium only)
 
         Returns
         -------
         :class:`str`
             The media ID of the uploaded media.
 
         Examples
@@ -690,26 +694,31 @@
                         "`media_category` must be specified to check the "
                         "upload status of gif images ('dm_gif' or 'tweet_gif')"
                     )
             elif media_type.startswith('image'):
                 # Checking the upload status of an image is impossible.
                 wait_for_completion = False
 
+        if is_long_video:
+            endpoint = Endpoint.UPLOAD_MEDIA_2
+        else:
+            endpoint = Endpoint.UPLOAD_MEDIA
+
         total_bytes = len(binary)
 
         # ============ INIT =============
         params = {
             'command': 'INIT',
             'total_bytes': total_bytes,
             'media_type': media_type
         }
         if media_category is not None:
             params['media_category'] = media_category
         response = (await self.http.post(
-            Endpoint.UPLOAD_MEDIA,
+            endpoint,
             params=params,
             headers=self._base_headers
         )).json()
         media_id = response['media_id']
         # =========== APPEND ============
         segment_index = 0
         bytes_sent = 0
@@ -732,15 +741,15 @@
                     'blob',
                     chunk_stream,
                     'application/octet-stream',
                 )
             }
 
             coro = self.http.post(
-                Endpoint.UPLOAD_MEDIA,
+                endpoint,
                 params=params,
                 headers=headers,
                 files=files
             )
             tasks.append(asyncio.create_task(coro))
             chunk_streams.append(chunk_stream)
 
@@ -756,32 +765,34 @@
 
         # ========== FINALIZE ===========
         params = {
             'command': 'FINALIZE',
             'media_id': media_id,
         }
         await self.http.post(
-            Endpoint.UPLOAD_MEDIA,
+            endpoint,
             params=params,
             headers=self._base_headers,
         )
 
         if wait_for_completion:
             while True:
-                state = self.check_media_status(media_id)
+                state = await self.check_media_status(media_id)
                 processing_info = state['processing_info']
                 if 'error' in processing_info:
                     raise InvalidMedia(processing_info['error'].get('message'))
                 if processing_info['state'] == 'succeeded':
                     break
                 await asyncio.sleep(status_check_interval)
 
         return media_id
 
-    async def check_media_status(self, media_id: str) -> dict:
+    async def check_media_status(
+        self, media_id: str, is_long_video: bool = False
+    ) -> dict:
         """
         Check the status of uploaded media.
 
         Parameters
         ----------
         media_id : :class:`str`
             The media ID of the uploaded media.
@@ -792,16 +803,20 @@
             A dictionary containing information about the status of
             the uploaded media.
         """
         params = {
             'command': 'STATUS',
             'media_id': media_id
         }
+        if is_long_video:
+            endpoint = Endpoint.UPLOAD_MEDIA_2
+        else:
+            endpoint = Endpoint.UPLOAD_MEDIA
         response = (await self.http.get(
-            Endpoint.UPLOAD_MEDIA,
+            endpoint,
             params=params,
             headers=self._base_headers
         )).json()
         return response
 
     async def create_media_metadata(
         self,
@@ -2782,14 +2797,15 @@
                         'Some followers are excluded because '
                         '"Quality Filter" is enabled. To get all followers, '
                         'turn off it in the Twitter settings.'
                     )
                     continue
                 if user_info[0].get('__typename') == 'UserUnavailable':
                     continue
+                results.append(User(self, user_info[0]))
             elif entry_id.startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
 
         return Result(
             results,
             partial(self._get_user_friendship,
                     user_id, count, endpoint, next_cursor),
@@ -2962,15 +2978,15 @@
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY'
         }
         if max_id is not None:
             params['max_id'] = max_id
 
         return (await self.http.get(
-            Endpoint.CONVERSASION.format(conversation_id),
+            Endpoint.CONVERSATION.format(conversation_id),
             params=params,
             headers=self._base_headers
         )).json()
 
     async def send_dm(
         self,
         user_id: str,
@@ -3343,15 +3359,15 @@
             An object representing the retrieved group.
         """
         params = {
             'context': 'FETCH_DM_CONVERSATION_HISTORY',
             'include_conversation_info': True,
         }
         response = (await self.http.get(
-            Endpoint.CONVERSASION.format(group_id),
+            Endpoint.CONVERSATION.format(group_id),
             params=params,
             headers=self._base_headers
         )).json()
         return Group(self, group_id, response)
 
     async def add_members_to_group(
         self, group_id: str, user_ids: list[str]
@@ -4598,8 +4614,130 @@
             tweets,
             partial(self.search_community_tweet, community_id,
                     query, count, next_cursor),
             next_cursor,
             partial(self.search_community_tweet, community_id,
                     query, count, previous_cursor),
             previous_cursor,
-        )
+        )
+
+    async def _stream(
+        self, topics: set[str]
+    ) -> AsyncGenerator[tuple[str, Payload]]:
+        headers = self._base_headers
+        headers.pop('content-type')
+        params = {'topics': ','.join(topics)}
+
+        async with self.http.stream(
+            'GET', Endpoint.EVENTS, params=params, timeout=None
+        ) as response:
+            self.http._remove_duplicate_ct0_cookie()
+            async for line in response.aiter_lines():
+                try:
+                    data = json.loads(line)
+                except json.JSONDecodeError:
+                    continue
+                payload = _payload_from_data(data['payload'])
+                yield data.get('topic'), payload
+
+    async def get_streaming_session(
+        self, topics: set[str], auto_reconnect: bool = True
+    ) -> StreamingSession:
+        """
+        Returns a session for interacting with the streaming API.
+
+        Parameters
+        ----------
+        topics : set[:class:`str`]
+            The set of topics to stream.
+            Topics can be generated using :class:`.Topic`.
+        auto_reconnect : :class:`bool`, default=True
+            Whether to automatically reconnect when disconnected.
+
+        Returns
+        -------
+        :class:`.StreamingSession`
+            A stream session instance.
+
+        Examples
+        --------
+        >>> from twikit.streaming import Topic
+        >>>
+        >>> topics = {
+        ...     Topic.tweet_engagement('1739617652'), # Stream tweet engagement
+        ...     Topic.dm_update('17544932482-174455537996'), # Stream DM update
+        ...     Topic.dm_typing('17544932482-174455537996') # Stream DM typing
+        ... }
+        >>> session = await client.get_streaming_session(topics)
+        >>>
+        >>> async for topic, payload in session:
+        ...     if payload.dm_update:
+        ...         conversation_id = payload.dm_update.conversation_id
+        ...         user_id = payload.dm_update.user_id
+        ...         print(f'{conversation_id}: {user_id} sent a message')
+        >>>
+        >>>     if payload.dm_typing:
+        ...         conversation_id = payload.dm_typing.conversation_id
+        ...         user_id = payload.dm_typing.user_id
+        ...         print(f'{conversation_id}: {user_id} is typing')
+        >>>
+        >>>     if payload.tweet_engagement:
+        ...         like = payload.tweet_engagement.like_count
+        ...         retweet = payload.tweet_engagement.retweet_count
+        ...         view = payload.tweet_engagement.view_count
+        ...         print('Tweet engagement updated:'
+        ...               f'likes: {like} retweets: {retweet} views: {view}')
+
+        Topics to stream can be added or deleted using
+        :attr:`.StreamingSession.update_subscriptions` method.
+
+        >>> subscribe_topics = {
+        ...     Topic.tweet_engagement('1749528513'),
+        ...     Topic.tweet_engagement('1765829534')
+        ... }
+        >>> unsubscribe_topics = {
+        ...     Topic.tweet_engagement('1739617652'),
+        ...     Topic.dm_update('17544932482-174455537996'),
+        ...     Topic.dm_update('17544932482-174455537996')
+        ... }
+        >>> await session.update_subscriptions(
+        ...     subscribe_topics, unsubscribe_topics
+        ... )
+
+        See Also
+        --------
+        .StreamingSession
+        .StreamingSession.update_subscriptions
+        .Payload
+        .Topic
+        """
+        stream = self._stream(topics)
+        session_id = (await anext(stream))[1].config.session_id
+        return StreamingSession(
+            self, session_id, stream, topics, auto_reconnect
+        )
+
+    async def _update_subscriptions(
+        self,
+        session: StreamingSession,
+        subscribe: set[str] | None = None,
+        unsubscribe: set[str] | None = None
+    ) -> Payload:
+        if subscribe is None:
+            subscribe = set()
+        if unsubscribe is None:
+            unsubscribe = set()
+
+        data = urlencode({
+            'sub_topics': ','.join(subscribe),
+            'unsub_topics': ','.join(unsubscribe)
+        })
+        headers = self._base_headers
+        headers['content-type'] = 'application/x-www-form-urlencoded'
+        headers['LivePipeline-Session'] = session.id
+        response = (await self.http.post(
+            Endpoint.UPDATE_SUBSCRIPTIONS, data=data, headers=headers
+        )).json()
+        session.topics |= subscribe
+        session.topics -= unsubscribe
+
+        return _payload_from_data(response)
```

### Comparing `twikit-1.5.9/twikit/twikit_async/community.py` & `twikit-1.6.0/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/errors.py` & `twikit-1.6.0/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/group.py` & `twikit-1.6.0/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/http.py` & `twikit-1.6.0/twikit/twikit_async/http.py`

 * *Files 21% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 
     async def get(self, url, **kwargs) -> httpx.Response:
         return await self.request('GET', url, **kwargs)
 
     async def post(self, url, **kwargs) -> httpx.Response:
         return await self.request('POST', url, **kwargs)
 
+    def stream(self, *args, **kwargs):
+        response = self.client.stream(*args, **kwargs)
+        return response
+
     def _remove_duplicate_ct0_cookie(self) -> None:
         cookies = {}
         for cookie in self.client.cookies.jar:
             if 'ct0' in cookies and cookie.name == 'ct0':
                 continue
             cookies[cookie.name] = cookie.value
         self.client.cookies = list(cookies.items())
```

### Comparing `twikit-1.5.9/twikit/twikit_async/list.py` & `twikit-1.6.0/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/message.py` & `twikit-1.6.0/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/notification.py` & `twikit-1.6.0/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/trend.py` & `twikit-1.6.0/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/tweet.py` & `twikit-1.6.0/twikit/twikit_async/tweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,27 +130,37 @@
             self.retweeted_tweet: Tweet = Tweet(
                 client, retweeted_tweet, retweeted_user
             )
         else:
             self.retweeted_tweet = None
 
         note_tweet_results = find_dict(data, 'note_tweet_results')
-        self.full_text: str | None = None
+        self.full_text: str = self.text
         if note_tweet_results:
             text_list = find_dict(note_tweet_results, 'text')
             if text_list:
                 self.full_text = text_list[0]
 
+            entity_set = note_tweet_results[0]['result']['entity_set']
+            self.urls: list = entity_set.get('urls')
+            hashtags = entity_set.get('hashtags', [])
+        else:
+            self.urls: list = legacy['entities'].get('urls')
+            hashtags = legacy['entities'].get('hashtags', [])
+
+        self.hashtags: list[str] = [
+            i['text'] for i in hashtags
+        ]
+
         self.is_quote_status: bool = legacy['is_quote_status']
         self.possibly_sensitive: bool = legacy.get('possibly_sensitive')
         self.possibly_sensitive_editable: bool = legacy.get(
             'possibly_sensitive_editable')
         self.quote_count: int = legacy['quote_count']
         self.media: list = legacy['entities'].get('media')
-        self.urls: list = legacy['entities'].get('urls')
         self.reply_count: int = legacy['reply_count']
         self.favorite_count: int = legacy['favorite_count']
         self.favorited: bool = legacy['favorited']
         self.view_count: int = (data['views'].get('count')
                                 if 'views' in data else None)
         self.retweet_count: int = legacy['retweet_count']
         self.editable_until_msecs: int = data['edit_control'].get(
@@ -168,26 +178,14 @@
             community_note_data = data['birdwatch_pivot']
             if 'note' in community_note_data:
                 self.community_note = {
                     'id': community_note_data['note']['rest_id'],
                     'text': community_note_data['subtitle']['text']
                 }
 
-        if note_tweet_results:
-            hashtags_ = find_dict(note_tweet_results, 'hashtags')
-            if hashtags_:
-                hashtags = hashtags_[0]
-            else:
-                hashtags = []
-        else:
-            hashtags = legacy['entities'].get('hashtags', [])
-        self.hashtags: list[str] = [
-            i['text'] for i in hashtags
-        ]
-
         if (
             'card' in data and
             'legacy' in data['card'] and
             'name' in data['card']['legacy'] and
             data['card']['legacy']['name'].startswith('poll')
         ):
             self._poll_data = data['card']
```

### Comparing `twikit-1.5.9/twikit/twikit_async/user.py` & `twikit-1.6.0/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/twikit_async/utils.py` & `twikit-1.6.0/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/user.py` & `twikit-1.6.0/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.9/twikit/utils.py` & `twikit-1.6.0/twikit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     LOGIN_FLOW = 'https://api.twitter.com/1.1/onboarding/task.json'
     LOGOUT = 'https://api.twitter.com/1.1/account/logout.json'
     CREATE_TWEET = 'https://twitter.com/i/api/graphql/SiM_cAu83R0wnrpmKQQSEw/CreateTweet'
     CREATE_NOTE_TWEET = 'https://twitter.com/i/api/graphql/iCUB42lIfXf9qPKctjE5rQ/CreateNoteTweet'
     DELETE_TWEET = 'https://twitter.com/i/api/graphql/VaenaVgh5q5ih7kvyVjgtg/DeleteTweet'
     SEARCH_TIMELINE = 'https://twitter.com/i/api/graphql/flaR-PUMshxFWZWPNpq4zA/SearchTimeline'
     UPLOAD_MEDIA = 'https://upload.twitter.com/i/media/upload.json'
+    UPLOAD_MEDIA_2 = 'https://upload.twitter.com/i/media/upload2.json'
     CREATE_MEDIA_METADATA = 'https://api.twitter.com/1.1/media/metadata/create.json'
     GUEST_TOKEN = 'https://api.twitter.com/1.1/guest/activate.json'
     CREATE_CARD = 'https://caps.twitter.com/v2/cards/create.json'
     USER_BY_SCREEN_NAME = 'https://twitter.com/i/api/graphql/NimuplG1OB7Fd2btCLdBOw/UserByScreenName'
     USER_BY_REST_ID = 'https://twitter.com/i/api/graphql/tD8zKvQzwY3kdx5yz6YmOw/UserByRestId'
     USER_TWEETS = 'https://twitter.com/i/api/graphql/QWF3SzpHmykQHsQMixG0cg/UserTweets'
     USER_TWEETS_AND_REPLIES = 'https://twitter.com/i/api/graphql/vMkJyzx1wdmvOeeNG0n6Wg/UserTweetsAndReplies'
@@ -229,15 +230,15 @@
     BLUE_VERIFIED_FOLLOWERS = 'https://twitter.com/i/api/graphql/VmIlPJNEDVQ29HfzIhV4mw/BlueVerifiedFollowers'
     FOLLOWING = 'https://twitter.com/i/api/graphql/2vUj-_Ek-UmBVDNtd8OnQA/Following'
     FOLLOWERS_YOU_KNOW = 'https://twitter.com/i/api/graphql/f2tbuGNjfOE8mNUO5itMew/FollowersYouKnow'
     SUBSCRIPTIONS = 'https://twitter.com/i/api/graphql/Wsm5ZTCYtg2eH7mXAXPIgw/UserCreatorSubscriptions'
     SEND_DM = 'https://twitter.com/i/api/1.1/dm/new2.json'
     DELETE_DM = 'https://twitter.com/i/api/graphql/BJ6DtxA2llfjnRoRjaiIiw/DMMessageDeleteMutation'
     INBOX_INITIAL_STATE = 'https://twitter.com/i/api/1.1/dm/inbox_initial_state.json'
-    CONVERSASION = 'https://twitter.com/i/api/1.1/dm/conversation/{}.json'
+    CONVERSATION = 'https://twitter.com/i/api/1.1/dm/conversation/{}.json'
     CREATE_SCHEDULED_TWEET = 'https://twitter.com/i/api/graphql/LCVzRQGxOaGnOnYH01NQXg/CreateScheduledTweet'
     BOOKMARKS = 'https://twitter.com/i/api/graphql/qToeLeMs43Q8cr7tRYXmaQ/Bookmarks'
     BOOKMARKS_ALL_DELETE = 'https://twitter.com/i/api/graphql/skiACZKC1GDYli-M8RzEPQ/BookmarksAllDelete'
     RETWEETERS = 'https://twitter.com/i/api/graphql/X-XEqG5qHQSAwmvy00xfyQ/Retweeters'
     FAVORITERS = 'https://twitter.com/i/api/graphql/LLkw5EcVutJL6y-2gkz22A/Favoriters'
     ADD_MEMBER_TO_GROUP = 'https://twitter.com/i/api/graphql/oBwyQ0_xVbAQ8FAyG0pCRA/AddParticipantsMutation'
     CHANGE_GROUP_NAME = 'https://twitter.com/i/api/1.1/dm/conversation/{}/update_name.json'
@@ -283,14 +284,17 @@
     SIMILAR_POSTS = 'https://twitter.com/i/api/graphql/EToazR74i0rJyZYalfVEAQ/SimilarPosts'
     BOOKMARK_FOLDERS = 'https://twitter.com/i/api/graphql/i78YDd0Tza-dV4SYs58kRg/BookmarkFoldersSlice'
     EDIT_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/a6kPp1cS1Dgbsjhapz1PNw/EditBookmarkFolder'
     DELETE_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/2UTTsO-6zs93XqlEUZPsSg/DeleteBookmarkFolder'
     CREATE_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/6Xxqpq8TM_CREYiuof_h5w/createBookmarkFolder'
     BOOKMARK_FOLDER_TIMELINE = 'https://twitter.com/i/api/graphql/8HoabOvl7jl9IC1Aixj-vg/BookmarkFolderTimeline'
     BOOKMARK_TO_FOLDER = 'https://twitter.com/i/api/graphql/4KHZvvNbHNf07bsgnL9gWA/bookmarkTweetToFolder'
+    PLACE_TRENDS = 'https://api.twitter.com/1.1/trends/place.json'
+    EVENTS = 'https://api.twitter.com/live_pipeline/events'
+    UPDATE_SUBSCRIPTIONS = 'https://api.twitter.com/1.1/live_pipeline/update_subscriptions'
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
     """
     This class is for storing multiple results.
```

### Comparing `twikit-1.5.9/twikit.egg-info/PKG-INFO` & `twikit-1.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: twikit
-Version: 1.5.9
-Summary: Twitter API wrapper for python with **no API key required**.
-Home-page: https://github.com/d60/twikit
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
 
 
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
@@ -28,15 +18,15 @@
 
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
 
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
 
 
-If you have any questions, please ask on [Discord](https://discord.gg/nCrByrr8cX).
+If you have any questions, you can ask on [Discord](https://discord.gg/nCrByrr8cX).
 
 
 
 ## Features
 
 ### No API Key Required
 
@@ -124,22 +114,26 @@
     print(
         tweet.user.name,
         tweet.text,
         tweet.created_at
     )
 ```
 
+**Retrieve user tweets**
+```python
+tweets = client.get_user_tweets('123456', 'Tweet')
 
-More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
-
+for tweet in tweets:
+    print(tweet.text)
+```
 
+More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
 ## Contributing
 
 I would like to hear your thoughts and suggestions.
 
 If you have any features you'd like to see added or encounter any issues,
 
 please let me know in the [issues](https://github.com/d60/twikit/issues) section.
 
-
 Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
```

### Comparing `twikit-1.5.9/twikit.egg-info/SOURCES.txt` & `twikit-1.6.0/twikit.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 twikit/errors.py
 twikit/group.py
 twikit/http.py
 twikit/list.py
 twikit/message.py
 twikit/notification.py
 twikit/py.typed
+twikit/streaming.py
 twikit/trend.py
 twikit/tweet.py
 twikit/user.py
 twikit/utils.py
 twikit.egg-info/PKG-INFO
 twikit.egg-info/SOURCES.txt
 twikit.egg-info/dependency_links.txt
@@ -27,11 +28,12 @@
 twikit/twikit_async/community.py
 twikit/twikit_async/errors.py
 twikit/twikit_async/group.py
 twikit/twikit_async/http.py
 twikit/twikit_async/list.py
 twikit/twikit_async/message.py
 twikit/twikit_async/notification.py
+twikit/twikit_async/streaming.py
 twikit/twikit_async/trend.py
 twikit/twikit_async/tweet.py
 twikit/twikit_async/user.py
 twikit/twikit_async/utils.py
```

