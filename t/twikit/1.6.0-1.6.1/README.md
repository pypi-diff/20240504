# Comparing `tmp/twikit-1.6.0.tar.gz` & `tmp/twikit-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.6.0.tar", last modified: Fri May  3 14:37:19 2024, max compression
+gzip compressed data, was "twikit-1.6.1.tar", last modified: Sat May  4 04:22:42 2024, max compression
```

## Comparing `twikit-1.6.0.tar` & `twikit-1.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.606418 twikit-1.6.0/
--rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     3999 2024-05-03 14:37:19.604424 twikit-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3728 2024-05-01 18:21:05.000000 twikit-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 14:37:19.607416 twikit-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-05-01 18:21:05.000000 twikit-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.521647 twikit-1.6.0/twikit/
--rw-rw-rw-   0        0        0      658 2024-05-03 14:32:19.000000 twikit-1.6.0/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/bookmark.py
--rw-rw-rw-   0        0        0   144654 2024-05-03 13:12:28.000000 twikit-1.6.0/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/group.py
--rw-rw-rw-   0        0        0     2218 2024-05-02 13:58:54.000000 twikit-1.6.0/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/py.typed
--rw-rw-rw-   0        0        0     8065 2024-05-03 14:13:32.000000 twikit-1.6.0/twikit/streaming.py
--rw-rw-rw-   0        0        0     1070 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/trend.py
--rw-rw-rw-   0        0        0    23780 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.599436 twikit-1.6.0/twikit/twikit_async/
--rw-rw-rw-   0        0        0      610 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   147077 2024-05-03 13:20:37.000000 twikit-1.6.0/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2260 2024-05-03 13:08:32.000000 twikit-1.6.0/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     8192 2024-05-03 14:16:39.000000 twikit-1.6.0/twikit/twikit_async/streaming.py
--rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    23661 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-05-01 18:21:05.000000 twikit-1.6.0/twikit/user.py
--rw-rw-rw-   0        0        0    30547 2024-05-02 18:47:12.000000 twikit-1.6.0/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:37:19.541592 twikit-1.6.0/twikit.egg-info/
--rw-rw-rw-   0        0        0     3999 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      910 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 14:37:19.000000 twikit-1.6.0/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 04:22:42.688550 twikit-1.6.1/
+-rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     3999 2024-05-04 04:22:42.684560 twikit-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3728 2024-05-01 18:21:05.000000 twikit-1.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 04:22:42.688550 twikit-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-05-01 18:21:05.000000 twikit-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:22:42.540944 twikit-1.6.1/twikit/
+-rw-rw-rw-   0        0        0      658 2024-05-04 04:20:04.000000 twikit-1.6.1/twikit/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   145687 2024-05-04 04:15:26.000000 twikit-1.6.1/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/community.py
+-rw-rw-rw-   0        0        0     2666 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/group.py
+-rw-rw-rw-   0        0        0     2218 2024-05-02 13:58:54.000000 twikit-1.6.1/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/py.typed
+-rw-rw-rw-   0        0        0     8193 2024-05-04 04:14:29.000000 twikit-1.6.1/twikit/streaming.py
+-rw-rw-rw-   0        0        0     2825 2024-05-04 04:17:28.000000 twikit-1.6.1/twikit/trend.py
+-rw-rw-rw-   0        0        0    23780 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:22:42.679573 twikit-1.6.1/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      610 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   148138 2024-05-04 04:18:05.000000 twikit-1.6.1/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2260 2024-05-03 13:08:32.000000 twikit-1.6.1/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     8320 2024-05-04 04:19:04.000000 twikit-1.6.1/twikit/twikit_async/streaming.py
+-rw-rw-rw-   0        0        0     2844 2024-05-04 04:17:45.000000 twikit-1.6.1/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    23661 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-05-01 18:21:05.000000 twikit-1.6.1/twikit/user.py
+-rw-rw-rw-   0        0        0    30626 2024-05-04 03:25:31.000000 twikit-1.6.1/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 04:22:42.578843 twikit-1.6.1/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3999 2024-05-04 04:22:42.000000 twikit-1.6.1/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2024-05-04 04:22:42.000000 twikit-1.6.1/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 04:22:42.000000 twikit-1.6.1/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-04 04:22:42.000000 twikit-1.6.1/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 04:22:42.000000 twikit-1.6.1/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.6.0/LICENSE` & `twikit-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/PKG-INFO` & `twikit-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.6.0
+Version: 1.6.1
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.6.0/README.md` & `twikit-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/setup.py` & `twikit-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/__init__.py` & `twikit-1.6.1/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.6.0'
+__version__ = '1.6.1'
 
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
```

### Comparing `twikit-1.6.0/twikit/bookmark.py` & `twikit-1.6.1/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/client.py` & `twikit-1.6.1/twikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     raise_exceptions_from_response
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
-from .trend import Trend
+from .trend import PlaceTrend, PlaceTrends, Location, Trend
 from .streaming import Payload, StreamingSession, _payload_from_data
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import (
     BOOKMARK_FOLDER_TIMELINE_FEATURES,
     COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
@@ -2735,14 +2735,44 @@
         results = []
         for item in items:
             trend_info = item['item']['content']['trend']
             results.append(Trend(self, trend_info))
 
         return results
 
+    def get_available_locations(self) -> list[Location]:
+        """
+        Retrieves locations where trends can be retrieved.
+
+        Returns
+        -------
+        list[:class:`.Location`]
+        """
+        response = self.http.get(
+            Endpoint.AVAILABLE_LOCATIONS,
+            headers=self._base_headers
+        ).json()
+        return [Location(self, data) for data in response]
+
+    def get_place_trends(self, woeid: int) -> PlaceTrends:
+        """
+        Retrieves the top 50 trending topics for a specific id.
+        You can get available woeid using
+        :attr:`.Client.get_available_locations`.
+        """
+        response = self.http.get(
+            Endpoint.PLACE_TRENDS,
+            params={'id': woeid},
+            headers=self._base_headers
+        ).json()
+        trend_data = response[0]
+        trends = [PlaceTrend(self, data) for data in trend_data['trends']]
+        trend_data['trends'] = trends
+        return trend_data
+
     def _get_user_friendship(
         self,
         user_id: str,
         count: int,
         endpoint: str,
         cursor: str | None
     ) -> Result[User]:
```

### Comparing `twikit-1.6.0/twikit/community.py` & `twikit-1.6.1/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/errors.py` & `twikit-1.6.1/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/group.py` & `twikit-1.6.1/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/http.py` & `twikit-1.6.1/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/list.py` & `twikit-1.6.1/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/message.py` & `twikit-1.6.1/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/notification.py` & `twikit-1.6.1/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/streaming.py` & `twikit-1.6.1/twikit/streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,22 +107,23 @@
         errors = data['errors']
         return SubscriptionsEvent(errors)
 
     if name == 'tweet_engagement':
         like_count = data.get('like_count')
         retweet_count = data.get('retweet_count')
         quote_count = data.get('quote_count')
+        reply_count = data.get('reply_count')
         view_count = None
         view_count_state = None
         if 'view_count_info' in data:
             view_count = data['view_count_info']['count']
             view_count_state = data['view_count_info']['state']
         return TweetEngagementEvent(
-            like_count, retweet_count,
-            view_count, view_count_state, quote_count
+            like_count, retweet_count, view_count,
+            view_count_state, quote_count, reply_count
         )
 
     if name == 'dm_update':
         conversation_id = data['conversation_id']
         user_id = data['user_id']
         return DMUpdateEvent(conversation_id, user_id)
 
@@ -177,14 +178,15 @@
     Event representing tweet engagement metrics.
     """
     like_count: str | None  #: The number of likes on the tweet.
     retweet_count: str | None  #: The number of retweets of the tweet.
     view_count: str | None  #: The number of views of the tweet.
     view_count_state: str | None  #: The state of view count.
     quote_count: int | None  #: The number of quotes of the tweet.
+    reply_count: int | None  # The number of Replies of the tweet.
 
 
 class DMUpdateEvent(NamedTuple):
     """
     Event representing a (DM) update.
     """
     conversation_id: str  #: The ID of the conversation associated with the DM.
```

### Comparing `twikit-1.6.0/twikit/tweet.py` & `twikit-1.6.1/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/__init__.py` & `twikit-1.6.1/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/bookmark.py` & `twikit-1.6.1/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/client.py` & `twikit-1.6.1/twikit/twikit_async/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     CommunityMember
 )
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
-from .trend import Trend
+from .trend import Location, PlaceTrend, PlaceTrends, Trend
 from .streaming import Payload, StreamingSession, _payload_from_data
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet, tweet_from_data
 from .user import User
 from .utils import Flow, Result
 
 
 class Client:
@@ -2755,14 +2755,44 @@
         results = []
         for item in items:
             trend_info = item['item']['content']['trend']
             results.append(Trend(self, trend_info))
 
         return results
 
+    async def get_available_locations(self) -> list[Location]:
+        """
+        Retrieves locations where trends can be retrieved.
+
+        Returns
+        -------
+        list[:class:`.Location`]
+        """
+        response = (await self.http.get(
+            Endpoint.AVAILABLE_LOCATIONS,
+            headers=self._base_headers
+        )).json()
+        return [Location(self, data) for data in response]
+
+    async def get_place_trends(self, woeid: int) -> PlaceTrends:
+        """
+        Retrieves the top 50 trending topics for a specific id.
+        You can get available woeid using
+        :attr:`.Client.get_available_locations`.
+        """
+        response = (await self.http.get(
+            Endpoint.PLACE_TRENDS,
+            params={'id': woeid},
+            headers=self._base_headers
+        )).json()
+        trend_data = response[0]
+        trends = [PlaceTrend(self, data) for data in trend_data['trends']]
+        trend_data['trends'] = trends
+        return trend_data
+
     async def _get_user_friendship(
         self,
         user_id: str,
         count: int,
         endpoint: str,
         cursor: str | None
     ) -> Result[User]:
```

### Comparing `twikit-1.6.0/twikit/twikit_async/community.py` & `twikit-1.6.1/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/errors.py` & `twikit-1.6.1/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/group.py` & `twikit-1.6.1/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/http.py` & `twikit-1.6.1/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/list.py` & `twikit-1.6.1/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/message.py` & `twikit-1.6.1/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/notification.py` & `twikit-1.6.1/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/streaming.py` & `twikit-1.6.1/twikit/twikit_async/streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,22 +111,23 @@
         errors = data['errors']
         return SubscriptionsEvent(errors)
 
     if name == 'tweet_engagement':
         like_count = data.get('like_count')
         retweet_count = data.get('retweet_count')
         quote_count = data.get('quote_count')
+        reply_count = data.get('reply_count')
         view_count = None
         view_count_state = None
         if 'view_count_info' in data:
             view_count = data['view_count_info']['count']
             view_count_state = data['view_count_info']['state']
         return TweetEngagementEvent(
-            like_count, retweet_count,
-            view_count, view_count_state, quote_count
+            like_count, retweet_count, view_count,
+            view_count_state, quote_count, reply_count
         )
 
     if name == 'dm_update':
         conversation_id = data['conversation_id']
         user_id = data['user_id']
         return DMUpdateEvent(conversation_id, user_id)
 
@@ -181,14 +182,15 @@
     Event representing tweet engagement metrics.
     """
     like_count: str | None  #: The number of likes on the tweet.
     retweet_count: str | None  #: The number of retweets of the tweet.
     view_count: str | None  #: The number of views of the tweet.
     view_count_state: str | None  #: The state of view count.
     quote_count: int | None  #: The number of quotes of the tweet.
+    reply_count: int | None  # The number of Replies of the tweet.
 
 
 class DMUpdateEvent(NamedTuple):
     """
     Event representing a (DM) update.
     """
     conversation_id: str  #: The ID of the conversation associated with the DM.
```

### Comparing `twikit-1.6.0/twikit/twikit_async/tweet.py` & `twikit-1.6.1/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/user.py` & `twikit-1.6.1/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/twikit_async/utils.py` & `twikit-1.6.1/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/user.py` & `twikit-1.6.1/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.0/twikit/utils.py` & `twikit-1.6.1/twikit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,15 @@
     BOOKMARK_FOLDERS = 'https://twitter.com/i/api/graphql/i78YDd0Tza-dV4SYs58kRg/BookmarkFoldersSlice'
     EDIT_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/a6kPp1cS1Dgbsjhapz1PNw/EditBookmarkFolder'
     DELETE_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/2UTTsO-6zs93XqlEUZPsSg/DeleteBookmarkFolder'
     CREATE_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/6Xxqpq8TM_CREYiuof_h5w/createBookmarkFolder'
     BOOKMARK_FOLDER_TIMELINE = 'https://twitter.com/i/api/graphql/8HoabOvl7jl9IC1Aixj-vg/BookmarkFolderTimeline'
     BOOKMARK_TO_FOLDER = 'https://twitter.com/i/api/graphql/4KHZvvNbHNf07bsgnL9gWA/bookmarkTweetToFolder'
     PLACE_TRENDS = 'https://api.twitter.com/1.1/trends/place.json'
+    AVAILABLE_LOCATIONS = 'https://api.twitter.com/1.1/trends/available.json'
     EVENTS = 'https://api.twitter.com/live_pipeline/events'
     UPDATE_SUBSCRIPTIONS = 'https://api.twitter.com/1.1/live_pipeline/update_subscriptions'
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
```

### Comparing `twikit-1.6.0/twikit.egg-info/PKG-INFO` & `twikit-1.6.1/twikit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.6.0
+Version: 1.6.1
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.6.0/twikit.egg-info/SOURCES.txt` & `twikit-1.6.1/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

