# Comparing `tmp/pybirdbuddy-0.0.8-py3-none-any.whl.zip` & `tmp/pybirdbuddy-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 19905 bytes, number of entries: 18
--rw-r--r--  2.0 unx      143 b- defN 23-Jan-10 07:18 birdbuddy/__init__.py
--rw-r--r--  2.0 unx     8281 b- defN 23-Jan-10 07:18 birdbuddy/birds.py
--rw-r--r--  2.0 unx    21734 b- defN 23-Jan-10 07:18 birdbuddy/client.py
+Zip file size: 20296 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      143 b- defN 23-Jan-10 17:12 birdbuddy/__init__.py
+-rw-r--r--  2.0 unx     8281 b- defN 23-Jan-10 17:10 birdbuddy/birds.py
+-rw-r--r--  2.0 unx    21863 b- defN 23-Jan-14 17:08 birdbuddy/client.py
 -rw-r--r--  2.0 unx       85 b- defN 22-Dec-09 00:35 birdbuddy/const.py
 -rw-r--r--  2.0 unx     1585 b- defN 22-Dec-09 00:35 birdbuddy/exceptions.py
 -rw-r--r--  2.0 unx     3624 b- defN 23-Jan-02 00:57 birdbuddy/feed.py
--rw-r--r--  2.0 unx     5372 b- defN 23-Jan-10 07:18 birdbuddy/feeder.py
--rw-r--r--  2.0 unx     2061 b- defN 23-Jan-10 07:18 birdbuddy/media.py
+-rw-r--r--  2.0 unx     5469 b- defN 23-Jan-14 17:08 birdbuddy/feeder.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-Jan-14 17:08 birdbuddy/media.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jan-14 17:08 birdbuddy/user.py
 -rw-r--r--  2.0 unx      106 b- defN 23-Jan-01 19:15 birdbuddy/queries/__init__.py
 -rw-r--r--  2.0 unx     2894 b- defN 22-Dec-09 00:35 birdbuddy/queries/auth.py
 -rw-r--r--  2.0 unx     9310 b- defN 23-Jan-08 18:58 birdbuddy/queries/birds.py
 -rw-r--r--  2.0 unx     1214 b- defN 22-Dec-09 00:35 birdbuddy/queries/debug.py
--rw-r--r--  2.0 unx     2252 b- defN 23-Jan-10 07:18 birdbuddy/queries/feeder.py
+-rw-r--r--  2.0 unx     2252 b- defN 23-Jan-10 17:12 birdbuddy/queries/feeder.py
 -rw-r--r--  2.0 unx     9421 b- defN 22-Dec-14 01:55 birdbuddy/queries/me.py
--rw-r--r--  2.0 unx     1379 b- defN 23-Jan-10 07:18 pybirdbuddy-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-10 07:18 pybirdbuddy-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jan-10 07:18 pybirdbuddy-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1418 b- defN 23-Jan-10 07:18 pybirdbuddy-0.0.8.dist-info/RECORD
-18 files, 70981 bytes uncompressed, 17609 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx     1379 b- defN 23-Jan-14 17:50 pybirdbuddy-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-14 17:50 pybirdbuddy-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jan-14 17:50 pybirdbuddy-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1491 b- defN 23-Jan-14 17:50 pybirdbuddy-0.0.9.dist-info/RECORD
+19 files, 71763 bytes uncompressed, 17890 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -18,14 +18,17 @@
 
 Filename: birdbuddy/feeder.py
 Comment: 
 
 Filename: birdbuddy/media.py
 Comment: 
 
+Filename: birdbuddy/user.py
+Comment: 
+
 Filename: birdbuddy/queries/__init__.py
 Comment: 
 
 Filename: birdbuddy/queries/auth.py
 Comment: 
 
 Filename: birdbuddy/queries/birds.py
@@ -36,20 +39,20 @@
 
 Filename: birdbuddy/queries/feeder.py
 Comment: 
 
 Filename: birdbuddy/queries/me.py
 Comment: 
 
-Filename: pybirdbuddy-0.0.8.dist-info/METADATA
+Filename: pybirdbuddy-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pybirdbuddy-0.0.8.dist-info/WHEEL
+Filename: pybirdbuddy-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pybirdbuddy-0.0.8.dist-info/top_level.txt
+Filename: pybirdbuddy-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pybirdbuddy-0.0.8.dist-info/RECORD
+Filename: pybirdbuddy-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## birdbuddy/client.py

```diff
@@ -1,13 +1,12 @@
 """Bird Buddy client module"""
 
 from __future__ import annotations
 import asyncio
 from datetime import datetime
-from typing import Union
 
 from python_graphql_client import GraphqlClient
 
 from . import LOGGER, VERBOSE, queries
 from .birds import (
     PostcardSighting,
     Sighting,
@@ -20,16 +19,17 @@
     AuthenticationFailedError,
     AuthTokenExpiredError,
     NoResponseError,
     GraphqlError,
     UnexpectedResponseError,
 )
 from .feed import Feed, FeedNode, FeedNodeType
-from .feeder import Feeder, FeederState, FeederUpdateStatus, MetricState
+from .feeder import Feeder, FeederUpdateStatus, MetricState
 from .media import Collection, Media
+from .user import BirdBuddyUser
 
 _NO_VALUE = object()
 """Sentinel value to allow None to override a default value."""
 
 
 def _redact(data, redacted: bool = True):
     """Returns a redacted string if necessary."""
@@ -38,17 +38,17 @@
 
 class BirdBuddy:
     """Bird Buddy api client"""
 
     graphql: GraphqlClient
     _email: str
     _password: str
-    _access_token: Union[str, None]
-    _refresh_token: Union[str, None]
-    _me: Union[dict, None]
+    _access_token: str | None
+    _refresh_token: str | None
+    _me: BirdBuddyUser | None
     _feeders: dict[str, Feeder]
     _collections: dict[str, Collection]
     _last_feed_date: datetime
 
     def __init__(self, email: str, password: str) -> None:
         self.graphql = GraphqlClient(BB_URL)
         self._email = email
@@ -60,15 +60,15 @@
         self._feeders = {}
         self._collections = {}
 
     def _save_me(self, me_data: dict):
         if not me_data:
             return False
         me_data["__last_updated"] = datetime.now()
-        self._me = me_data
+        self._me = BirdBuddyUser(me_data["user"])
         # pylint: disable=invalid-name
         for f in me_data.get("feeders", []):
             if f["id"] in self._feeders:
                 # Refresh Feeder data inline
                 self._feeders[f["id"]].update(f)
             else:
                 self._feeders[f["id"]] = Feeder(f)
@@ -199,14 +199,19 @@
         if not isinstance(result, dict):
             raise UnexpectedResponseError(response)
 
         LOGGER.log(VERBOSE, "< response: %s", _redact(result, should_redact))
 
         return result
 
+    @property
+    def user(self) -> None | BirdBuddyUser:
+        """The logged in user data"""
+        return self._me
+
     async def refresh(self) -> bool:
         """Refreshes the Bird Buddy feeder data"""
         data = await self._make_request(query=queries.me.ME)
         LOGGER.debug("Feeder data refreshed successfully: %s", data)
         return self._save_me(data["me"])
 
     async def toggle_off_grid(
```

## birdbuddy/feeder.py

```diff
@@ -87,14 +87,19 @@
 
     @property
     def id(self):
         """UUID"""
         return self["id"]
 
     @property
+    def serial(self):
+        """Feeder SN"""
+        return self["serialNumber"]
+
+    @property
     def name(self):
         """Feeder name, as set in the app"""
         return self.get("name", "Bird Buddy")
 
     @property
     def is_owner(self):
         """Whether the logged in user is the owner of this feeder."""
```

## birdbuddy/media.py

```diff
@@ -35,23 +35,26 @@
     def content_url(self) -> str:
         """Large content URL"""
         return self.get("contentUrl", None)
 
     @property
     def is_expired(self) -> bool:
         """`True` if the media URL is expired"""
-        if not self.thumbnail_url:
-            return None
-        expiry = int(
-            parse_qs(urlparse(self.thumbnail_url).query).get("Expires", None).pop()
-        )
-        if not expiry:
-            return None
-        now = time.time()
-        return expiry < now
+        return is_media_expired(self.thumbnail_url)
+
+
+def is_media_expired(media_url: str) -> bool:
+    """`True` if the media URL is expired"""
+    if not media_url:
+        return None
+    expiry = int(parse_qs(urlparse(media_url).query).get("Expires", None).pop())
+    if not expiry:
+        return None
+    now = time.time()
+    return expiry < now
 
 
 class Collection(UserDict):
     """Collection of media for a particular bird species."""
 
     @property
     def bird_name(self) -> str:
```

## Comparing `pybirdbuddy-0.0.8.dist-info/METADATA` & `pybirdbuddy-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybirdbuddy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to query data about a Bird Buddy smart bird feeder
 Home-page: https://github.com/jhansche/pybirdbuddy
 Author: jhansche
 Author-email: madcoder@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: python-graphql-client
```

## Comparing `pybirdbuddy-0.0.8.dist-info/RECORD` & `pybirdbuddy-0.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 birdbuddy/__init__.py,sha256=iTQAx46sEtfhEm5TTyrMRBtfOdOtCcGsHoh86lCHi64,143
 birdbuddy/birds.py,sha256=HZKKWZjSnr0FshFathtkb1SMgOv3HFx_rWeGDbSBcLE,8281
-birdbuddy/client.py,sha256=cOLJdvgQJCj0yagXKjUQDH3uaPo9NYI1vrdCRs41nOk,21734
+birdbuddy/client.py,sha256=EVsNN1zEQ0BQoDzZNZi03K4Mgf2sqFEyT0l5lRn-0ao,21863
 birdbuddy/const.py,sha256=o2PL4TWg5LeNabPZTo4et2SqCWkrR6ru0UxHRGzlksg,85
 birdbuddy/exceptions.py,sha256=pu1gUvxJRauO6a7G__oyHBC4QoW8vs28yG4QVUK6C-o,1585
 birdbuddy/feed.py,sha256=dDBoqJrvobZlxvHZuZORPeM0QVofa01PtC9jmj9t2O4,3624
-birdbuddy/feeder.py,sha256=qFpTh_ODndNHjZrMWmzA70CtZiluy7sF-7yoKgeSjH8,5372
-birdbuddy/media.py,sha256=DK5V6aQMgtNoKqGBvFOT4gD6Hb-uS3HHDtfpTeDWnyM,2061
+birdbuddy/feeder.py,sha256=S7MdFVAkb9UZ8_TH4aHEGckrtkk_Ahcy5sJxZndGbZ0,5469
+birdbuddy/media.py,sha256=RW3jZRU6uM44UaUX0L9T_r1Zz40aFUtL8b2KZDhz5Ic,2138
+birdbuddy/user.py,sha256=fmznBajsJYmu9new0Xv2oapeCwLR0y3RuIks1nblZj8,406
 birdbuddy/queries/__init__.py,sha256=Sa4cFCf5OuvRyeqVmLhygEvj4L4SgjpG6-o1bLTrtzI,106
 birdbuddy/queries/auth.py,sha256=OM6CNgnUOttnbMiOCAx_O-yx8keMNztR50JowogTQnc,2894
 birdbuddy/queries/birds.py,sha256=OijfIKAXSYGDJAbyKxodUmTBNIVFAFS8NJV-Wl3eX2I,9310
 birdbuddy/queries/debug.py,sha256=hK6c4fhWuoGfTvtHqa_x1PO-n0brz-zFY0rWpb9mqZA,1214
 birdbuddy/queries/feeder.py,sha256=vsky2Dgs8MKbuey16736zH6UUXfcllhziSs-9xFAfkU,2252
 birdbuddy/queries/me.py,sha256=tp5mReiYtQbksVWHoIRr9PllVnbX2Q5sccd2JvcEV8A,9421
-pybirdbuddy-0.0.8.dist-info/METADATA,sha256=kM2RjqTaI1SRFWlKQASjZkn3KAUhQhP0BNu_V05MzAU,1379
-pybirdbuddy-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pybirdbuddy-0.0.8.dist-info/top_level.txt,sha256=aYLtRHkZSJz58RDiXiQKVkdkfjnn3XPf3xuVTm7lfjU,10
-pybirdbuddy-0.0.8.dist-info/RECORD,,
+pybirdbuddy-0.0.9.dist-info/METADATA,sha256=u_q1RLNH6PYXGCfpzcIb280TRsX_DvMaqcoh75pJBJ4,1379
+pybirdbuddy-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pybirdbuddy-0.0.9.dist-info/top_level.txt,sha256=aYLtRHkZSJz58RDiXiQKVkdkfjnn3XPf3xuVTm7lfjU,10
+pybirdbuddy-0.0.9.dist-info/RECORD,,
```

