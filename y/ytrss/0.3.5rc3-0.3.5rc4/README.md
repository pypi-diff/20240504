# Comparing `tmp/ytrss-0.3.5rc3.tar.gz` & `tmp/ytrss-0.3.5rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytrss-0.3.5rc3.tar", last modified: Mon Apr 22 11:15:21 2024, max compression
+gzip compressed data, was "ytrss-0.3.5rc4.tar", last modified: Sat May  4 08:46:46 2024, max compression
```

## Comparing `ytrss-0.3.5rc3.tar` & `ytrss-0.3.5rc4.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.505133 ytrss-0.3.5rc3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-22 11:15:21.505133 ytrss-0.3.5rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:15:21.505133 ytrss-0.3.5rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.489133 ytrss-0.3.5rc3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.489133 ytrss-0.3.5rc3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/integration/example_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/integration/finder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/tests/unit/controlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/unit/controlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/tests/unit/controlers/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/unit/controlers/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/unit/controlers/youtube/movie_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/unit/example_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/tests/unit/podcast_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/ytrss/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/ytrss/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/commands/website.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/ytrss/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.497134 ytrss-0.3.5rc3/ytrss/configuration/entity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/entity/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/entity/destination_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/entity/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.497134 ytrss-0.3.5rc3/ytrss/configuration/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/readers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/readers/default_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/readers/file_dict_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/readers/json_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/configuration/readers/yaml_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.497134 ytrss-0.3.5rc3/ytrss/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.497134 ytrss-0.3.5rc3/ytrss/core/algoritms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/algoritms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/algoritms/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/algoritms/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.497134 ytrss-0.3.5rc3/ytrss/core/entity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/entity/destination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/entity/downloaded_movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/entity/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/entity/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/entity/source_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.497134 ytrss-0.3.5rc3/ytrss/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/helpers/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/managers/destination_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/managers/manager_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/managers/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/managers/sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/managers/templates_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/database/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/database/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/database/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/database/sqlite/sqlite_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/default/destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/default/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/plugins/mp3_tags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/mp3_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/mp3_tags/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/plugins/rss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/rss/destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/rss/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/plugins/rss/podcast/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/rss/podcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/rss/podcast/podcast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.501134 ytrss-0.3.5rc3/ytrss/plugins/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube/base_youtube_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube/youtube_channel_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube/youtube_named_channel_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube/youtube_playlist_source_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.505133 ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/youtube_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.505133 ytrss-0.3.5rc3/ytrss/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-22 11:15:19.000000 ytrss-0.3.5rc3/ytrss/templates/podcast.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:15:21.493133 ytrss-0.3.5rc3/ytrss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-22 11:15:21.000000 ytrss-0.3.5rc3/ytrss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-22 11:15:21.000000 ytrss-0.3.5rc3/ytrss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:15:21.000000 ytrss-0.3.5rc3/ytrss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 11:15:21.000000 ytrss-0.3.5rc3/ytrss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-22 11:15:21.000000 ytrss-0.3.5rc3/ytrss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 11:15:21.000000 ytrss-0.3.5rc3/ytrss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.441810 ytrss-0.3.5rc4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.445810 ytrss-0.3.5rc4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/integration/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/integration/finder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.445810 ytrss-0.3.5rc4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.445810 ytrss-0.3.5rc4/tests/unit/controlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/unit/controlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.445810 ytrss-0.3.5rc4/tests/unit/controlers/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/unit/controlers/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/unit/controlers/youtube/movie_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/unit/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/tests/unit/podcast_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.445810 ytrss-0.3.5rc4/ytrss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/commands/website.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss/configuration/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/entity/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/entity/destination_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/entity/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss/configuration/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/readers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/readers/default_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/readers/file_dict_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/readers/json_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/configuration/readers/yaml_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss/core/algoritms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/algoritms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/algoritms/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/algoritms/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/core/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/entity/destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/entity/downloaded_movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/entity/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/entity/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/entity/source_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/helpers/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/managers/destination_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/managers/manager_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/managers/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/managers/sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/managers/templates_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/database/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/database/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/database/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/database/sqlite/sqlite_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/default/destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/default/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.453810 ytrss-0.3.5rc4/ytrss/plugins/mp3_tags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/mp3_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/mp3_tags/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/ytrss/plugins/rss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/rss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/rss/destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/rss/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/ytrss/plugins/rss/podcast/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/rss/podcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/rss/podcast/podcast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/ytrss/plugins/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube/base_youtube_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube/youtube_channel_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube/youtube_named_channel_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube/youtube_playlist_source_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/youtube_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.457810 ytrss-0.3.5rc4/ytrss/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-04 08:46:44.000000 ytrss-0.3.5rc4/ytrss/templates/podcast.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:46:46.449810 ytrss-0.3.5rc4/ytrss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-04 08:46:46.000000 ytrss-0.3.5rc4/ytrss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-04 08:46:46.000000 ytrss-0.3.5rc4/ytrss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:46:46.000000 ytrss-0.3.5rc4/ytrss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 08:46:46.000000 ytrss-0.3.5rc4/ytrss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-04 08:46:46.000000 ytrss-0.3.5rc4/ytrss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 08:46:46.000000 ytrss-0.3.5rc4/ytrss.egg-info/top_level.txt
```

### Comparing `ytrss-0.3.5rc3/LICENSE` & `ytrss-0.3.5rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/PKG-INFO` & `ytrss-0.3.5rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytrss
-Version: 0.3.5rc3
+Version: 0.3.5rc4
 Summary: Tools for downloading mp3 from YouTube subscription and playlists.
 Home-page: https://github.com/rafyco/ytrss.git
 Author: Rafal Kobel
 Author-email: rafalkobel@rafyco.pl
 License: GNU
 Project-URL: Source, https://github.com/rafyco/ytrss
 Project-URL: Tracker, https://github.com/rafyco/ytrss/issues
```

### Comparing `ytrss-0.3.5rc3/README.rst` & `ytrss-0.3.5rc4/README.rst`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/setup.py` & `ytrss-0.3.5rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         ],
         "style": [
             "pylint == 3.1.0",
             "pep8 == 1.7.1",
             "pycodestyle == 2.11.1"
         ],
         "typing": [
-            "mypy == 1.9.0",
+            "mypy == 1.10.0",
             "types-PyYAML == 6.0.12.20240311"
         ],
         "documentation": [
             "Sphinx == 6.2.0",
             "sphinx-epytext == 0.0.4",
             "sphinx-autorun == 1.1.1"
         ]
```

### Comparing `ytrss-0.3.5rc3/tests/integration/finder_test.py` & `ytrss-0.3.5rc4/tests/integration/finder_test.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/tests/unit/controlers/youtube/movie_test.py` & `ytrss-0.3.5rc4/tests/unit/controlers/youtube/movie_test.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/tests/unit/podcast_test.py` & `ytrss-0.3.5rc4/tests/unit/podcast_test.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/__init__.py` & `ytrss-0.3.5rc4/ytrss/__init__.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/client.py` & `ytrss-0.3.5rc4/ytrss/client.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/commands/__init__.py` & `ytrss-0.3.5rc4/ytrss/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/commands/configuration.py` & `ytrss-0.3.5rc4/ytrss/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/commands/download.py` & `ytrss-0.3.5rc4/ytrss/commands/download.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/commands/run.py` & `ytrss-0.3.5rc4/ytrss/commands/run.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/commands/url.py` & `ytrss-0.3.5rc4/ytrss/commands/url.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/commands/version.py` & `ytrss-0.3.5rc4/ytrss/commands/version.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/configuration.py` & `ytrss-0.3.5rc4/ytrss/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/entity/configuration_data.py` & `ytrss-0.3.5rc4/ytrss/configuration/entity/configuration_data.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/entity/destination_info.py` & `ytrss-0.3.5rc4/ytrss/configuration/entity/destination_info.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/entity/source.py` & `ytrss-0.3.5rc4/ytrss/configuration/entity/source.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/factory.py` & `ytrss-0.3.5rc4/ytrss/configuration/factory.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/readers/file_dict_configuration.py` & `ytrss-0.3.5rc4/ytrss/configuration/readers/file_dict_configuration.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/readers/json_configuration.py` & `ytrss-0.3.5rc4/ytrss/configuration/readers/json_configuration.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/configuration/readers/yaml_configuration.py` & `ytrss-0.3.5rc4/ytrss/configuration/readers/yaml_configuration.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/algoritms/download.py` & `ytrss-0.3.5rc4/ytrss/core/algoritms/download.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/algoritms/finder.py` & `ytrss-0.3.5rc4/ytrss/core/algoritms/finder.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/entity/destination.py` & `ytrss-0.3.5rc4/ytrss/core/entity/destination.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/entity/downloaded_movie.py` & `ytrss-0.3.5rc4/ytrss/core/entity/downloaded_movie.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/entity/movie.py` & `ytrss-0.3.5rc4/ytrss/core/entity/movie.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/entity/plugin.py` & `ytrss-0.3.5rc4/ytrss/core/entity/plugin.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/entity/source_downloader.py` & `ytrss-0.3.5rc4/ytrss/core/entity/source_downloader.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/helpers/files.py` & `ytrss-0.3.5rc4/ytrss/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/helpers/logging.py` & `ytrss-0.3.5rc4/ytrss/core/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/helpers/templates.py` & `ytrss-0.3.5rc4/ytrss/core/helpers/templates.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/managers/destination_manager.py` & `ytrss-0.3.5rc4/ytrss/core/managers/destination_manager.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/managers/manager_service.py` & `ytrss-0.3.5rc4/ytrss/core/managers/manager_service.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/managers/plugin_manager.py` & `ytrss-0.3.5rc4/ytrss/core/managers/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/managers/sources_manager.py` & `ytrss-0.3.5rc4/ytrss/core/managers/sources_manager.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/core/managers/templates_manager.py` & `ytrss-0.3.5rc4/ytrss/core/managers/templates_manager.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/database/database.py` & `ytrss-0.3.5rc4/ytrss/database/database.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/database/sqlite/sqlite_database.py` & `ytrss-0.3.5rc4/ytrss/database/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/default/destination.py` & `ytrss-0.3.5rc4/ytrss/plugins/default/destination.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/default/plugin.py` & `ytrss-0.3.5rc4/ytrss/plugins/default/plugin.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/mp3_tags/plugin.py` & `ytrss-0.3.5rc4/ytrss/plugins/mp3_tags/plugin.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/rss/destination.py` & `ytrss-0.3.5rc4/ytrss/plugins/rss/destination.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/rss/podcast/podcast.py` & `ytrss-0.3.5rc4/ytrss/plugins/rss/podcast/podcast.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube/base_youtube_source_downloader.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube/base_youtube_source_downloader.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube/plugin.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube/plugin.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube/youtube_channel_source_downloader.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube/youtube_channel_source_downloader.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube/youtube_named_channel_source_downloader.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube/youtube_named_channel_source_downloader.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube/youtube_playlist_source_downloader.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube/youtube_playlist_source_downloader.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/movie.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/movie.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/plugin.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/plugin.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/plugins/youtube_dl/youtube_downloader.py` & `ytrss-0.3.5rc4/ytrss/plugins/youtube_dl/youtube_downloader.py`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss/templates/podcast.xml` & `ytrss-0.3.5rc4/ytrss/templates/podcast.xml`

 * *Files identical despite different names*

### Comparing `ytrss-0.3.5rc3/ytrss.egg-info/PKG-INFO` & `ytrss-0.3.5rc4/ytrss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytrss
-Version: 0.3.5rc3
+Version: 0.3.5rc4
 Summary: Tools for downloading mp3 from YouTube subscription and playlists.
 Home-page: https://github.com/rafyco/ytrss.git
 Author: Rafal Kobel
 Author-email: rafalkobel@rafyco.pl
 License: GNU
 Project-URL: Source, https://github.com/rafyco/ytrss
 Project-URL: Tracker, https://github.com/rafyco/ytrss/issues
```

### Comparing `ytrss-0.3.5rc3/ytrss.egg-info/SOURCES.txt` & `ytrss-0.3.5rc4/ytrss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

