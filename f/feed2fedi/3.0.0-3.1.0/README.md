# Comparing `tmp/feed2fedi-3.0.0.tar.gz` & `tmp/feed2fedi-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed2fedi-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "feed2fedi-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `feed2fedi-3.0.0.tar` & `feed2fedi-3.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4434 2024-01-17 05:15:22.877778 feed2fedi-3.0.0/README.rst
--rw-r--r--   0        0        0     2578 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      462 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/__init__.py
--rw-r--r--   0        0        0     3816 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/app.py
--rw-r--r--   0        0        0     5501 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/collect.py
--rw-r--r--   0        0        0    12998 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/control.py
--rw-r--r--   0        0        0     9349 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/publish.py
--rw-r--r--   0        0        0     2656 2024-04-07 23:31:13.163821 feed2fedi-3.0.0/src/feed2fedi/utils.py
--rw-r--r--   0        0        0     5776 1970-01-01 00:00:00.000000 feed2fedi-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4434 2024-05-04 05:27:37.711571 feed2fedi-3.1.0/README.rst
+-rw-r--r--   0        0        0     2654 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/src/feed2fedi/__init__.py
+-rw-r--r--   0        0        0     4431 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/src/feed2fedi/app.py
+-rw-r--r--   0        0        0     5625 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/src/feed2fedi/collect.py
+-rw-r--r--   0        0        0    12998 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/src/feed2fedi/control.py
+-rw-r--r--   0        0        0     9759 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/src/feed2fedi/publish.py
+-rw-r--r--   0        0        0     2656 2024-05-04 05:27:37.715571 feed2fedi-3.1.0/src/feed2fedi/utils.py
+-rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 feed2fedi-3.1.0/PKG-INFO
```

### Comparing `feed2fedi-3.0.0/README.rst` & `feed2fedi-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `feed2fedi-3.0.0/pyproject.toml` & `feed2fedi-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
+requires = ["flit_core>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "feed2fedi"
 description = "Makes posts to Fediverse from one or more feeds"
 readme = "README.rst"
 authors = [
     {name = "marvin8", email = "marvin8@tuta.io"},
 ]
 requires-python = ">=3.9,<3.13"
 license = {text = "AGPL-3.0-or-later"}
-version = "3.0.0"
+version = "3.1.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -31,28 +31,32 @@
     "httpx>=0.27.0",
     "markdownify>=0.12.1",
     "minimal-activitypub>=1.2.0",
     "msgspec>=0.18.6",
     "pycryptodomex>=3.20.0",
     "python-magic>=0.4.27",
     "stamina>=24.2.0",
-    "typer>=0.12.1",
-    "yt-dlp>=2024.3.10",
+    "typer>=0.12.3",
+    "yt-dlp>=2024.4.9",
 ]
 
 [project.scripts]
 feed2fedi = "feed2fedi.app:start_main"
 feed2fedi_import_cache = "feed2fedi.app:start_import"
 feed2fedi_convert_config = "feed2fedi.utils:start_conversion"
 
 [project.urls]
 Issues = "https://codeberg.org/MarvinsMastodonTools/feed2fedi/issues"
 Source = "https://codeberg.org/MarvinsMastodonTools/feed2fedi"
 Changelog = "https://codeberg.org/MarvinsMastodonTools/feed2fedi/src/branch/main/CHANGELOG.rst"
 
+[project.optional-dependencies]
+dev = [
+    "constable>=0.3.1",
+]
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
 ignore-property-decorators = false
@@ -86,7 +90,9 @@
 warn_unused_configs = true
 no_implicit_reexport = true
 
 [tool.scriv]
 categories = "Breaking, Added, Changed, Deprecated, Removed, Fixed, Security"
 format = "rst"
 version = "literal: pyproject.toml: project.version"
+
+[tool.pdm]
```

### Comparing `feed2fedi-3.0.0/src/feed2fedi/app.py` & `feed2fedi-3.1.0/src/feed2fedi/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 """Main processing and main entry point methods for Feed2Fedi."""
 
 import asyncio
 import sys
 import traceback
 from pathlib import Path
+from typing import Optional
 
 import typer
 from minimal_activitypub.client_2_server import ActivityPubError
 from typing_extensions import Annotated
 
 from feed2fedi import DISPLAY_NAME
 from feed2fedi import __version__
 from feed2fedi.collect import FeedReader
 from feed2fedi.control import Configuration
 from feed2fedi.control import PostRecorder
 from feed2fedi.publish import Fediverse
 
 
-async def main(config_file: Path):
+async def main(config_file: Path, post_limit: Optional[int] = None):
     """Read configuration and feeds, then make posts while avoiding duplicates.
 
+    :param post_limit: Optional; number of new statuses to post before exiting. Default is "None" and if so we process
+        all entries in all configured RSS/Atom feeds.
     :param config_file: Path and file name of file to use for reading and storing configuration from
     """
     error_encountered = False
 
     print(f"Welcome to {DISPLAY_NAME} {__version__}")
 
     config = await Configuration.load_config(config_file_path=Path(config_file))
 
     async with PostRecorder(history_db_path=config.cache_db_path) as post_recorder:
         await post_recorder.prune(max_age_in_days=config.cache_max_age)
 
         fediverse = Fediverse(config=config, post_recorder=post_recorder)
 
+        statuses_posted = 0
         for feed in config.feeds:
             items = FeedReader(feed=feed.url).items
 
             try:
-                await fediverse.publish(items=items, feed=feed)
+                statuses_posted += await fediverse.publish(items=items, feed=feed, post_limit=post_limit)
             except ActivityPubError as publishing_error:
                 error_encountered = True
                 print(f"Encountered the following error during publishing feed items:\n{publishing_error}")
                 traceback.print_tb(publishing_error.__traceback__)
                 break
 
+            if post_limit and statuses_posted >= post_limit:
+                break
+
     if error_encountered:
         sys.exit(1)
 
 
 async def import_urls(config_file: Path, url_file: Path) -> None:
     """Start import of URLS into cache db.
 
@@ -84,17 +91,25 @@
             file_okay=True,
             dir_okay=False,
             writable=True,
             resolve_path=True,
             help="filename and optional path to config file",
         ),
     ] = Path("./config.json"),
+    post_limit: Annotated[
+        Optional[int],
+        typer.Option(
+            "--limit",
+            "-l",
+            help="Limit how many new statuses should be posted",
+        ),
+    ] = None,
 ) -> None:
     """Start Feed2Fedi."""
-    asyncio.run(main(config_file=config_file))
+    asyncio.run(main(config_file=config_file, post_limit=post_limit))
 
 
 def start_import_shim(
     url_file: Annotated[
         Path,
         typer.Option(
             "--url-file",
```

### Comparing `feed2fedi-3.0.0/src/feed2fedi/collect.py` & `feed2fedi-3.1.0/src/feed2fedi/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,17 @@
         if len(images):
             return images
 
         if item.has_key("description"):
             parsed_content = BeautifulSoup(item.get("description"), features="html.parser")
             images = [image.attrs["src"] for image in parsed_content.select(image_selector)]
 
+        if item.has_key("link"):
+            images = [link.get("href") for link in item.links if "image" in link.get("type")]
+
         if len(images):
             return images
 
         if image_url := item.get("media_thumbnail", [{}])[0].get("url"):
             images = [image_url]
 
         if len(images):
@@ -124,15 +127,15 @@
     :returns:
         mime-type in a String or None
     """
     # First check if URL starts with http:// or https://
     regex = r"^https?://"
     match = re.search(regex, img_url, flags=0)
     if not match:
-        print("Post link is not a full link: %s" % img_url)
+        print(f"Post link is not a full link: {img_url}")
         return None
 
     # Acceptable image formats
     image_formats = (
         "image/png",
         "image/jpeg",
         "image/gif",
@@ -156,9 +159,9 @@
 
     if content_type in image_formats:
         return str(content_type)
 
     if content_type == "application/octet-stream" and file_name.suffix == ".webp":
         return "image/webp"
 
-    print("URL does not point to a valid image file: %s" % img_url)
+    print(f"URL does not point to a valid image file: {img_url}")
     return None
```

### Comparing `feed2fedi-3.0.0/src/feed2fedi/control.py` & `feed2fedi-3.1.0/src/feed2fedi/control.py`

 * *Files identical despite different names*

### Comparing `feed2fedi-3.0.0/src/feed2fedi/publish.py` & `feed2fedi-3.1.0/src/feed2fedi/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import re
 import tempfile
 import traceback
 from datetime import datetime
 from pathlib import Path
 from typing import List
+from typing import Optional
 
 import magic
 import yt_dlp
 from feedparser import FeedParserDict
 from httpx import AsyncClient
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ClientError
@@ -36,21 +37,26 @@
         self.config = config
         self.post_recorder = post_recorder
 
     async def publish(  # noqa: C901, PLR0915
         self,
         items: List[FeedParserDict],
         feed: FeedInfo,
-    ) -> None:
+        post_limit: Optional[int],
+    ) -> int:
         """Publish posts to fediverse instance from content in the items list.
 
+        :param post_limit: Optional; Number of statuses to post before returning
         :param items: Rss feed items to post
         :param feed: Section of config for current feed
+
+        :returns int: Number of new statuses posted.
         """
-        async with AsyncClient(http2=True) as client:
+        statuses_posted = 0
+        async with AsyncClient(http2=True, timeout=30) as client:
             fediverse = ActivityPub(
                 instance=self.config.fedi_instance,
                 client=client,
                 access_token=self.config.fedi_access_token,
             )
             for attempt in retry_context(on=NetworkError, attempts=3):
                 with attempt:
@@ -118,14 +124,18 @@
                                 spoiler_text=spoiler_text,
                             )
 
                     print(f"Posted {posted_status['content']} to Fediverse at\n{posted_status['url']}")
 
                     await self.post_recorder.log_post(shared_url=item.link)
 
+                    statuses_posted += 1
+                    if post_limit and statuses_posted >= post_limit:
+                        break
+
                 except RatelimitError:
                     reset = fediverse.ratelimit_reset
                     seconds = reset.timestamp() - datetime.now(tz=UTC).timestamp()
                     print(
                         f'!!! Server "cool down" - waiting until {reset:%Y-%m-%d %H:%M:%S %z} '
                         f"({round(number=seconds)} seconds)"
                     )
@@ -133,14 +143,16 @@
 
                 except ClientError as error:
                     print(f"!!! Encountered error: {error}")
                     traceback.print_tb(error.__traceback__)
                     print("\nLog article to avoid repeat of error")
                     await self.post_recorder.log_post(shared_url=item.link)
 
+        return statuses_posted
+
     @staticmethod
     @retry(on=NetworkError, attempts=3)
     async def _post_video(
         fediverse: ActivityPub,
         item: FeedParserDict,
     ) -> List[str]:
         """Post media to fediverse instance and return media ID.
```

### Comparing `feed2fedi-3.0.0/src/feed2fedi/utils.py` & `feed2fedi-3.1.0/src/feed2fedi/utils.py`

 * *Files identical despite different names*

### Comparing `feed2fedi-3.0.0/PKG-INFO` & `feed2fedi-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed2fedi
-Version: 3.0.0
+Version: 3.1.0
 Summary: Makes posts to Fediverse from one or more feeds
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -20,19 +20,21 @@
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: markdownify>=0.12.1
 Requires-Dist: minimal-activitypub>=1.2.0
 Requires-Dist: msgspec>=0.18.6
 Requires-Dist: pycryptodomex>=3.20.0
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: stamina>=24.2.0
-Requires-Dist: typer>=0.12.1
-Requires-Dist: yt-dlp>=2024.3.10
+Requires-Dist: typer>=0.12.3
+Requires-Dist: yt-dlp>=2024.4.9
+Requires-Dist: constable>=0.3.1 ; extra == "dev"
 Project-URL: Changelog, https://codeberg.org/MarvinsMastodonTools/feed2fedi/src/branch/main/CHANGELOG.rst
 Project-URL: Issues, https://codeberg.org/MarvinsMastodonTools/feed2fedi/issues
 Project-URL: Source, https://codeberg.org/MarvinsMastodonTools/feed2fedi
+Provides-Extra: dev
 
 Feed2Fedi
 =========
 
 |Repo| |CI - Woodpecker| |Downloads|
 
 |Checked against| |Checked with| |CodeLimit|
```

