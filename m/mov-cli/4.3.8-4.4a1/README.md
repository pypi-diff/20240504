# Comparing `tmp/mov_cli-4.3.8.tar.gz` & `tmp/mov_cli-4.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.3.8.tar", last modified: Fri Apr 26 00:23:58 2024, max compression
+gzip compressed data, was "mov_cli-4.4a1.tar", last modified: Sat May  4 16:39:46 2024, max compression
```

## Comparing `mov_cli-4.3.8.tar` & `mov_cli-4.4a1.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.871339 mov_cli-4.3.8/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.871339 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.871339 mov_cli-4.3.8/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.3.8/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.8/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.3.8/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.3.8/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-26 00:23:58.881339 mov_cli-4.3.8/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-04-19 20:31:56.000000 mov_cli-4.3.8/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.3.8/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.874672 mov_cli-4.3.8/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-26 00:22:56.000000 mov_cli-4.3.8/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.3.8/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5588 2024-04-25 23:19:21.000000 mov_cli-4.3.8/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2937 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1785 2024-04-25 15:53:32.000000 mov_cli-4.3.8/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      159 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/random_tips.json
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4095 2024-04-26 00:20:10.000000 mov_cli-4.3.8/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1259 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6434 2024-04-25 23:19:21.000000 mov_cli-4.3.8/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      585 2024-04-25 23:19:21.000000 mov_cli-4.3.8/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1002 2024-04-19 20:51:26.000000 mov_cli-4.3.8/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.3.8/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.3.8/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.3.8/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2914 2024-04-19 20:51:26.000000 mov_cli-4.3.8/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      113 2024-04-25 15:53:32.000000 mov_cli-4.3.8/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3133 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2707 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/players/syncplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3868 2024-04-25 20:43:50.000000 mov_cli-4.3.8/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.878005 mov_cli-4.3.8/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.3.8/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.3.8/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.3.8/mov_cli/utils/paths.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.3.8/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-19 20:31:56.000000 mov_cli-4.3.8/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1486 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-26 00:23:58.000000 mov_cli-4.3.8/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1757 2024-04-26 00:22:19.000000 mov_cli-4.3.8/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.3.8/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-26 00:23:58.881339 mov_cli-4.3.8/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.3.8/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-26 00:23:58.881339 mov_cli-4.3.8/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.279717 mov_cli-4.4a1/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.279717 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.279717 mov_cli-4.4a1/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a1/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a1/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a1/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.4a1/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8018 2024-05-04 16:39:46.289717 mov_cli-4.4a1/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-05-03 21:25:09.000000 mov_cli-4.4a1/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.4a1/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.283050 mov_cli-4.4a1/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      135 2024-05-04 16:39:41.000000 mov_cli-4.4a1/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a1/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5935 2024-05-04 16:39:20.000000 mov_cli-4.4a1/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3640 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a1/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      159 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/cli/random_tips.json
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-03 22:20:27.000000 mov_cli-4.4a1/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1259 2024-04-25 20:43:50.000000 mov_cli-4.4a1/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 20:43:50.000000 mov_cli-4.4a1/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7617 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      621 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2245 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3434 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a1/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a1/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a1/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.4a1/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2953 2024-04-29 18:49:16.000000 mov_cli-4.4a1/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.286383 mov_cli-4.4a1/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      134 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/iina.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1885 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/syncplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3632 2024-05-03 21:25:09.000000 mov_cli-4.4a1/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a1/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1776 2024-05-03 22:17:47.000000 mov_cli-4.4a1/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.4a1/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.4a1/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.4a1/mov_cli/utils/paths.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.4a1/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.4a1/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2824 2024-05-01 08:46:47.000000 mov_cli-4.4a1/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8018 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1510 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      228 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-04 16:39:46.000000 mov_cli-4.4a1/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1778 2024-05-03 22:13:19.000000 mov_cli-4.4a1/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a1/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-04 16:39:46.289717 mov_cli-4.4a1/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a1/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-04 16:39:46.289717 mov_cli-4.4a1/setup.cfg
```

### Comparing `mov_cli-4.3.8/.github/ISSUE_TEMPLATE/bug-report.md` & `mov_cli-4.4a1/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/.github/workflows/pypi.yml` & `mov_cli-4.4a1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/.github/workflows/ruff.yml` & `mov_cli-4.4a1/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/LICENSE` & `mov_cli-4.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/PKG-INFO` & `mov_cli-4.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.8
+Version: 4.4a1
 Summary: Watch everything from your terminal.
-Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
+Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -39,21 +39,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: toml
-Requires-Dist: devgoldyutils>=2.5.7
+Requires-Dist: devgoldyutils>=3.0.0beta1
 Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer
 Requires-Dist: beautifulsoup4
 Requires-Dist: Unidecode
 Requires-Dist: deprecation
 Requires-Dist: packaging
+Requires-Dist: thefuzz
 Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.8 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a1 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
-r3tr0ananas.lol>, Goldy
+r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -23,23 +23,24 @@
 Windows 10 Classifier: Operating System :: POSIX :: Linux Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
-toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer>=0.12.2 Requires-
-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode Requires-
-Dist: deprecation Requires-Dist: packaging Requires-Dist: mov-cli-test>=1.1.0
-Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build;
-extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
-[Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions][python-
-shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url]
+toml Requires-Dist: devgoldyutils>=3.0.0beta1 Requires-Dist: typer>=0.12.2
+Requires-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode
+Requires-Dist: deprecation Requires-Dist: packaging Requires-Dist: thefuzz
+Requires-Dist: mov-cli-test>=1.1.0 Provides-Extra: dev Requires-Dist: ruff;
+extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist:
+devgoldyutils[pprint]>=2.5.7; extra == "dev" [![Stargazers][stars-shield]]
+[stars-url] [![Pypi Version][pypi-shield]][pypi-url] [![Pypi Downloads][pypi-
+dl-shield]][pypi-stats-url] [![Python Versions][python-shield]][pypi-url] [!
+[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
+url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
```

### Comparing `mov_cli-4.3.8/README.md` & `mov_cli-4.4a1/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/disclaimer.md` & `mov_cli-4.4a1/disclaimer.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/cli/__main__.py` & `mov_cli-4.4a1/mov_cli/cli/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .episode import handle_episode
 from .plugins import show_all_plugins
 from .scraper import select_scraper, use_scraper, scrape, steal_scraper_args
 from .configuration import open_config_file, set_cli_config
 
 from ..config import Config
 from ..download import Download
+from ..media import MetadataType
 from ..logger import mov_cli_logger
 from ..http_client import HTTPClient
 
 __all__ = ("mov_cli",)
 
 uwu_app = typer.Typer(pretty_exceptions_enable = False) # NOTE: goldy has an uwu complex.
 
@@ -80,24 +81,26 @@
         # This allows passing arguments to scrapers like this: 
         # https://github.com/mov-cli/mov-cli-youtube/commit/b538d82745a743cd74a02530d6a3d476cd60b808#diff-4e5b064838aa74a5375265f4dfbd94024b655ee24a191290aacd3673abed921a
 
         query: str = " ".join(query)
 
         http_client = HTTPClient(config)
 
-        selected_scraper = select_scraper(plugins, config.fzf_enabled, config.default_scraper)
+        selected_scraper = select_scraper(plugins, config.scrapers, config.fzf_enabled, config.default_scraper)
 
         if selected_scraper is None:
             mov_cli_logger.error(
                 "You must choose a scraper to scrape with! " \
                     "You can set a default scraper with the default key in config.toml."
             )
             return False
 
-        chosen_scraper = use_scraper(selected_scraper, config, http_client, scrape_options)
+        selected_scraper[2].update(scrape_options)
+
+        chosen_scraper = use_scraper(selected_scraper, config, http_client)
 
         choice = search(query, auto_select, chosen_scraper, config.fzf_enabled)
 
         if choice is None:
             mov_cli_logger.error("There was no results or you didn't select anything.")
             return False
 
@@ -110,27 +113,31 @@
 
         if chosen_episode is None:
             mov_cli_logger.error("You didn't select a season/episode.")
             return False
 
         media = scrape(choice, chosen_episode, chosen_scraper)
 
-        if media.url is None:
+        if media is None:
+            episode_details_string = f" ep {chosen_episode.episode} season {chosen_episode.season} of" if choice.type == MetadataType.MULTI else ""
+
             mov_cli_logger.error(
-                "Scraper didn't return a streamable url." \
-                    "\nThis is NOT a mov-cli issue. This IS an plugin issue"
+                f"The scraper '{chosen_scraper.__class__.__name__}' couldn't find{episode_details_string} '{choice.title}'! " \
+                    "Don't report this to mov-cli, report this to the plugin itself."
             )
             return False
 
         if download:
             dl = Download(config)
             mov_cli_logger.debug(f"Downloading from this url -> '{media.url}'")
 
             popen = dl.download(media)
-            popen.wait()
+            
+            if popen:
+                popen.wait()
 
         else:
             option = play(media, choice, chosen_scraper, chosen_episode, config)
 
             if option == "search":
                 query = input(Colours.BLUE.apply("  Enter Query: "))
```

### Comparing `mov_cli-4.3.8/mov_cli/cli/configuration.py` & `mov_cli-4.4a1/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/cli/episode.py` & `mov_cli-4.4a1/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/cli/play.py` & `mov_cli-4.4a1/mov_cli/cli/play.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,34 +12,53 @@
 
 from devgoldyutils import Colours
 
 from .scraper import scrape
 from .episode import handle_episode
 from .watch_options import watch_options
 
+from ..media import MetadataType
 from ..utils import what_platform
 from ..logger import mov_cli_logger
 
 def play(media: Media, metadata: Metadata, scraper: Scraper, episode: EpisodeSelector, config: Config) -> Optional[Literal["search"]]:
     platform = what_platform()
 
     chosen_player = config.player
 
-    mov_cli_logger.info(f"Playing '{Colours.BLUE.apply(media.display_name)}' with the '{chosen_player.__class__.__name__}' player...")
+    episode_details_string = ""
+
+    if metadata.type == MetadataType.MULTI:
+        season_string = Colours.CLAY.apply(str(episode.season))
+        episode_string = Colours.ORANGE.apply(str(episode.episode))
+
+        episode_details_string = f"episode {episode_string} in season {season_string} of " if episode.season > 1 else f"episode {episode_string} of "
+
+    mov_cli_logger.info(
+        f"Playing {episode_details_string}'{Colours.BLUE.apply(media.title)}' " \
+            f"with {chosen_player.display_name}..."
+    )
     mov_cli_logger.debug(f"Streaming with this url -> '{media.url}'")
 
-    popen = chosen_player.play(media)
+    try:
+        popen = chosen_player.play(media)
+    except FileNotFoundError as e:
+        mov_cli_logger.error(
+            f"The player '{chosen_player.display_name}' was not found! " \
+                f"Are you sure you have it installed? Are you sure it's in path? \nError: {e}"
+        )
+        return None
 
     if popen is None and platform != "iOS":
         mov_cli_logger.error(
-            f"The player '{config.player.__class__.__name__.lower()}' is not supported on this platform ({platform}). " \
-            "We recommend VLC for iOS and MPV for every other platform."
+            f"The player '{chosen_player.display_name}' is not supported on this platform ({platform}). " \
+            "We recommend VLC for iOS, IINA for MacOS and MPV for every other platform."
         )
 
-        return False
+        return None
 
     option = watch_options(popen, chosen_player, platform, media, config.fzf_enabled)
 
     if option == "search":
         popen.kill()
         return option
```

### Comparing `mov_cli-4.3.8/mov_cli/cli/plugins.py` & `mov_cli-4.4a1/mov_cli/cli/plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,47 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Tuple, List, Dict, NoReturn
 
-    from ..plugins import PluginHookData
+    from ..plugins import Plugin
+    PluginsDataT = List[Tuple[str, str, Plugin]]
 
 from devgoldyutils import Colours
 
 from ..plugins import load_plugin
 from ..logger import mov_cli_logger
 
-def get_plugins_data(plugins: Dict[str, str]) -> List[Tuple[str, str, PluginHookData]]:
-    plugins_data: List[Tuple[str, str, PluginHookData]] = []
+def get_plugins_data(plugins: Dict[str, str]) -> PluginsDataT:
+    plugins_data: PluginsDataT = []
 
     for plugin_namespace, plugin_module_name in plugins.items():
         plugin = load_plugin(plugin_module_name)
 
         if plugin is None:
             continue
 
-        plugin_data, _ = plugin
-
-        if plugin_data is None:
-            continue
-
         plugins_data.append(
-            (plugin_namespace, plugin_module_name, plugin_data, plugin)
+            (plugin_namespace, plugin_module_name, plugin)
         )
 
     return plugins_data
 
 def show_all_plugins(plugins: Dict[str, str]) -> None:
 
-    for plugin_namespace, plugin_module_name, plugin_hook_data, plugin in get_plugins_data(plugins):
+    for plugin_namespace, plugin_module_name, plugin in get_plugins_data(plugins):
 
         if plugin is not None:
-            plugin_module = plugin[1]
-
-            plugin_version = getattr(plugin_module, "__version__", "N/A")
+            plugin_version = getattr(plugin.module, "__version__", "N/A")
 
             print(f"- {Colours.PURPLE.apply(plugin_module_name)} ({plugin_namespace}) [{Colours.BLUE.apply(plugin_version)}]")
 
-            for scraper_name in plugin_hook_data["scrapers"]:
-                if scraper_name == "DEFAULT":
-                    continue
-
-                print(f"  - {Colours.PINK_GREY.apply(scraper_name)}")
+            for scraper_name in plugin.scrapers:
+                print(f"  - {Colours.PINK_GREY.apply(scraper_name[0])}")
 
 def handle_internal_plugin_error(e: Exception) -> NoReturn:
     mov_cli_logger.critical(
         "An error occurred inside a plugin. This is MOST LIKELY not a mov-cli error, " \
             f"make SURE mov-cli and your plugins are up to date. Also report this to the plugin, not mov-cli! \nError: {e}"
     )
```

### Comparing `mov_cli-4.3.8/mov_cli/cli/search.py` & `mov_cli-4.4a1/mov_cli/cli/search.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/cli/ui.py` & `mov_cli-4.4a1/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/cli/watch_options.py` & `mov_cli-4.4a1/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/config.py` & `mov_cli-4.4a1/mov_cli/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, TypedDict, final
 from typing_extensions import NotRequired
 
 if TYPE_CHECKING:
     from .players import Player
-    from typing import Dict, Union, Literal, Any, Optional
+    from typing import Dict, Literal, Any, Optional
 
-    JSON_VALUES = Union[str, bool, int, dict]
-    SUPPORTED_PARSERS = Literal["lxml", "html.parser"]
+    SupportedParsersT = Literal["lxml", "html.parser"]
+
+    @final
+    class ScraperData(TypedDict):
+        namespace: str
+        options: Dict[str, str | bool]
+
+    ScrapersConfigT = Dict[Literal["default"], str] | Dict[str, ScraperData]
 
 import os
 import toml
 import shutil
 from pathlib import Path
 from importlib.util import find_spec
 from devgoldyutils import LoggerAdapter
 
 from . import players, utils
 from .logger import mov_cli_logger
 from .utils import get_appdata_directory
 
-__all__ = ("Config", )
+__all__ = ("Config",)
 
 @final
 class ConfigUIData(TypedDict):
     fzf: bool
 
 @final
 class ConfigHTTPData(TypedDict):
     headers: Dict[str, str]
 
 @final
 class ConfigDownloadsData(TypedDict):
     save_path: str
-
-@final
-class ScrapersData(TypedDict):
-    default: str
+    yt_dlp: bool
 
 @final
 class ConfigData(TypedDict):
     version: int
     debug: bool
     player: str
-    parser: SUPPORTED_PARSERS
+    editor: str
+    parser: SupportedParsersT
     ui: ConfigUIData
     http: ConfigHTTPData
     downloads: ConfigDownloadsData
-    scrapers: ScrapersData
+    scrapers: ScrapersConfigT | Dict[str, str]
     plugins: Dict[str, str]
     resolution: int
 
 HttpHeadersData = TypedDict(
     "HttpHeadersData", 
     {
         "User-Agent": NotRequired[str],
@@ -96,25 +100,50 @@
 
         if value.lower() == "mpv":
             return players.MPV(platform, self)
         elif value.lower() == "vlc":
             return players.VLC(platform, self)
         elif value.lower() == "syncplay":
             return players.SyncPlay(platform, self)
+        elif value.lower() == "iina":
+            return players.IINA(platform, self)
 
         return players.CustomPlayer(value)
 
     @property
     def plugins(self) -> Dict[str, str]:
         return self.data.get("plugins", {"test": "mov-cli-test"})
 
     @property
+    def scrapers(self) -> ScrapersConfigT:
+        scrapers = self.data.get("scrapers", {})
+
+        consistent_scrapers: Dict[str, ScraperData] = {}
+
+        for scraper, plugin_namespace_or_dict in scrapers.items():
+
+            if scraper == "default":
+                consistent_scrapers["default"] = plugin_namespace_or_dict
+
+            elif isinstance(plugin_namespace_or_dict, str):
+                consistent_scrapers[scraper] = {"namespace": plugin_namespace_or_dict, "options": {}}
+
+            else:
+                dict = plugin_namespace_or_dict
+                consistent_scrapers[scraper] = {
+                    "namespace": dict["namespace"], 
+                    "options": dict["options"]
+                }
+
+        return consistent_scrapers
+
+    @property
     def editor(self) -> Optional[str]:
         """Returns the editor that should be opened while editing."""
-        return self.data.get("editor")
+        return self.data.get("editor", None)
 
     @property
     def skip_update_checker(self) -> bool:
         return self.data.get("skip_update_checker", False)
 
     @property
     def default_scraper(self) -> Optional[str]:
@@ -123,25 +152,30 @@
 
     @property
     def fzf_enabled(self) -> bool:
         """Returns whether fzf is allowed to be used. Defaults to True of fzf is available."""
         return self.data.get("ui", {}).get("fzf", True if shutil.which("fzf") is not None else False)
 
     @property
-    def parser(self) -> SUPPORTED_PARSERS | Any:
+    def parser(self) -> SupportedParsersT | Any:
         """Returns the parser type configured by the user else it just returns the default."""
         default_parser = "lxml" if find_spec("lxml") else "html.parser"
         return self.data.get("parser", default_parser)
 
     @property
     def download_location(self) -> str:
-        """Returns download location. Defaults to OS's download location."""
+        """Returns download location. Defaults to current working directory."""
         return self.data.get("downloads", {}).get("save_path", os.getcwd())
 
     @property
+    def use_yt_dlp(self) -> bool:
+        """Returns if yt-dlp should be used. Defaults to True."""
+        return self.data.get("downloads", {}).get("yt_dlp", True)
+
+    @property
     def debug(self) -> bool:
         """Returns whether debug should be enabled or not."""
         return self.data.get("debug", False)
 
     @property
     def proxy(self) -> dict | None:
         """Returns proxy data. Defaults to None"""
```

### Comparing `mov_cli-4.3.8/mov_cli/config.template.toml` & `mov_cli-4.4a1/mov_cli/config.template.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 
 # [mov-cli.ui]
 # fzf = true
 
 [mov-cli.plugins] # E.g: namespace = "package-name"
 test = "mov-cli-test"
 
-# [mov-cli.scrapers]
+[mov-cli.scrapers]
 # default = "films"
+test = "test.DEFAULT"
 
 # [mov-cli.http] # Don't mess with it if you don't know what you are doing!
 # headers = { User-Agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0" }
 
 # [mov-cli.downloads] # Do not use backslashes use forward slashes
 # save_path = "~/Downloads"
+# yt_dlp = true
 
 # [mov-cli.quality]
 # resolution = 720
```

### Comparing `mov_cli-4.3.8/mov_cli/http_client.py` & `mov_cli-4.4a1/mov_cli/http_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         redirect: bool = False, 
         **kwargs
     ) -> Response:
         """Performs a GET request and returns httpx.Response."""
         self.logger.debug(Colours.GREEN.apply("GET") + f" -> {url}")
 
         if include_default_headers is True:
-            headers.update({"Referer": url})
+            if headers.get("Referer") is None:
+                headers.update({"Referer": url})
+                
             headers.update(self.config.http_headers)
 
         try:
             response = self.__httpx_client.get(
                 url, 
                 headers = headers, 
                 follow_redirects = redirect, 
@@ -68,20 +70,45 @@
 
         except httpx.ConnectError as e:
             if "[SSL: CERTIFICATE_VERIFY_FAILED]" in str(e):
                 raise SiteMaybeBlocked(url, e)
 
             raise e
 
-    def post(self, url: str, data: dict = None, json: dict = None, **kwargs) -> Response: 
+    def post(
+        self, 
+        url: str,
+        data: dict = {},
+        json: dict = {}, 
+        headers: dict = {}, 
+        include_default_headers: bool = True, 
+        redirect: bool = False, 
+        **kwargs
+    ) -> Response:
         """Performs a POST request and returns httpx.Response."""
-        self.logger.debug(Colours.ORANGE.apply("POST") + f": {url}")
+        self.logger.debug(Colours.GREEN.apply("POST") + f" -> {url}")
 
-        self.__httpx_client.headers["Referer"] = url
+        if include_default_headers is True:
+            if headers.get("Referer") is None:
+                headers.update({"Referer": url})
 
-        return self.__httpx_client.post(
-            url, data = data, json = json, **kwargs
+            headers.update(self.config.http_headers)
+
+        response = self.__httpx_client.post(
+            url,
+            data = data,
+            json = json,
+            headers = headers, 
+            follow_redirects = redirect, 
+            **kwargs
         )
 
+        if response.is_error:
+            self.logger.debug(
+                f"POST Request to '{response.url}' failed! ({response})"
+            )
+
+        return response
+
     def set_cookies(self, cookies: dict) -> None:
         """Sets cookies."""
         self.__httpx_client.cookies = cookies
```

### Comparing `mov_cli-4.3.8/mov_cli/iterfzf/LICENSE.txt` & `mov_cli-4.4a1/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/iterfzf/__init__.py` & `mov_cli-4.4a1/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/media/media.py` & `mov_cli-4.4a1/mov_cli/media/media.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,14 @@
             audio_url = audio_url, 
             referrer = referrer,
             subtitles = subtitles
         )
 
     @property
     def display_name(self) -> str:
-        return f"{self.title} ({self.year})"
+        return f"{self.title} ({self.year})" if self.year is not None else self.title
 
-# Backwards compatibility for post v4.3.0 extensions.
+# Backwards compatibility for post v4.3 extensions.
 Series = Multi
 """DEPRECATED!!! USE 'Multi' INSTEAD! This will be removed after v4.4."""
 Movie = Single
 """DEPRECATED!!! USE 'Single' INSTEAD! This will be removed after v4.4."""
```

### Comparing `mov_cli-4.3.8/mov_cli/media/metadata.py` & `mov_cli-4.4a1/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/players/custom_player.py` & `mov_cli-4.4a1/mov_cli/players/custom_player.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 if TYPE_CHECKING:
     from ..media import Media
 
 import subprocess
 from devgoldyutils import Colours, LoggerAdapter
 
-from .. import errors
 from ..logger import mov_cli_logger
 from .player import Player
 
 __all__ = ("CustomPlayer",)
 
 logger = LoggerAdapter(mov_cli_logger, prefix = Colours.GREY.apply("CustomPlayer"))
 
@@ -22,15 +21,12 @@
     def __init__(self, player_command: str, **kwargs) -> None:
         self.player_command = player_command
 
         super().__init__(**kwargs)
 
     def play(self, media: Media) -> subprocess.Popen:
         """Plays this media in a custom player."""
-        logger.info(f"Launching your custom media player '{self.player_command}'...")
+        logger.debug(f"Launching your custom media player '{self.player_command}'...")
 
-        try:
-            return subprocess.Popen(
-                [self.player_command, media.url]
-            )
-        except ModuleNotFoundError:
-            raise errors.PlayerNotFound(self)
+        return subprocess.Popen(
+            [self.player_command, media.url]
+        )
```

### Comparing `mov_cli-4.3.8/mov_cli/players/mpv.py` & `mov_cli-4.4a1/mov_cli/players/syncplay.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,93 +4,67 @@
 if TYPE_CHECKING:
     from typing import Optional
     from ..media import Media
     from .. import Config
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import subprocess
-from devgoldyutils import Colours, LoggerAdapter
+from devgoldyutils import Colours
 
-from .. import errors
-from ..logger import mov_cli_logger
 from .player import Player
 
-__all__ = ("MPV",)
+__all__ = ("SyncPlay",)
 
-logger = LoggerAdapter(mov_cli_logger, prefix = Colours.PURPLE.apply("MPV"))
-
-class MPV(Player):
+class SyncPlay(Player):
     def __init__(self, platform: SUPPORTED_PLATFORMS, config: Config, **kwargs) -> None:
         self.platform = platform
         self.config = config
 
-        super().__init__(**kwargs)
+        super().__init__(display_name = Colours.BLUE.apply("Syncplay"), **kwargs)
 
     def play(self, media: Media) -> Optional[subprocess.Popen]:
-        """Plays this media in the MPV media player."""
-
-        logger.info("Launching MPV Media Player...")
-
-        if self.platform == "Android":
-            return subprocess.Popen(
-                [
-                    "am",
-                    "start",
-                    "-n",
-                    "is.xyz.mpv/is.xyz.mpv.MPVActivity",
-                    "-e",
-                    "filepath",
-                    media.url,
-                ]
-            )
-
-        try:
-
-            if self.platform == "Linux" or self.platform == "Windows":
-                args = [
-                    "mpv",
-                    media.url,
-                    f"--force-media-title={media.display_name}",
-                    "--no-terminal",
-                ]
-
-                if media.referrer is not None:
-                    args.append(f"--referrer={media.referrer}")
-
-                if media.audio_url is not None:
-                    args.append(f"--audio-file={media.audio_url}")
-
-                if media.subtitles is not None:
-                    args.append(f"--sub-file={media.subtitles}")
-
-                if self.config.resolution is not None:
-                    args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
-
-                return subprocess.Popen(args)
-
-            elif self.platform == "Darwin":
-                args = [
-                    "iina",
-                    "--no-stdin",
-                    "--keep-running",
-                    media.url,
-                    f"--mpv-force-media-title={media.display_name}",
-                ]
-
-                if media.referrer is not None:
-                    args.append(f"--mpv-referrer={media.referrer}")
-
-                if media.audio_url is not None: # TODO: This will need testing.
-                    args.append(f"--mpv-audio-file={media.audio_url}")
-
-                if media.subtitles is not None: # TODO: This will need testing.
-                    args.append(f"--mpv-sub-file={media.subtitles}")
+        """Plays this media in SyncPlay."""
+        if self.platform == "Windows" or self.platform == "Linux":
+            args = [
+                "syncplay",
+                media.url,
+                "--",
+                f"--force-media-title={media.display_name}",
+            ]
+
+            if media.referrer is not None:
+                args.append(f"--referrer={media.referrer}")
+
+            if media.audio_url is not None:
+                args.append(f"--audio-file={media.audio_url}")
+
+            if media.subtitles is not None:
+                args.append(f"--sub-file={media.subtitles}")
+
+            if self.config.resolution is not None:
+                args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: Only M3U8
+
+            return subprocess.Popen(args)
+
+        elif self.platform == "Darwin": # NOTE: Limits you to IINA
+            args = [
+                "syncplay",
+                media.url,
+                "--",
+                f"--mpv-force-media-title={media.display_name}",
+            ]
+
+            if media.referrer is not None:
+                args.append(f"--mpv-referrer={media.referrer}")
+
+            if media.audio_url is not None: # TODO: This will need testing.
+                args.append(f"--mpv-audio-file={media.audio_url}")
 
-                if self.config.resolution is not None:
-                    args.append(f"--mpv-hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
+            if media.subtitles is not None: # TODO: This will need testing.
+                args.append(f"--mpv-sub-file={media.subtitles}")
 
-                return subprocess.Popen(args)
+            if self.config.resolution is not None: # TODO: This will need testing.
+                args.append(f"--mpv-hls-bitrate={self.config.resolution}")
 
-        except (ModuleNotFoundError, FileNotFoundError):
-            raise errors.PlayerNotFound(self)
+            return subprocess.Popen(args)
 
         return None
```

### Comparing `mov_cli-4.3.8/mov_cli/players/player.py` & `mov_cli-4.4a1/mov_cli/players/player.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 
 if TYPE_CHECKING:
     from typing import Optional
 
     from ..media import Media
 
 import subprocess
+from devgoldyutils import Colours
 from abc import ABC, abstractmethod
 
 __all__ = ("Player",)
 
 class Player(ABC):
     """A base class for all players in mov-cli."""
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, display_name: Optional[str] = None, **kwargs) -> None:
+        self.display_name = display_name or Colours.PINK_GREY.apply(self.__class__.__name__)
+
         super().__init__()
 
     @abstractmethod
     def play(self, media: Media) -> Optional[subprocess.Popen]:
         """Method to be overridden with code to play media in that specific player."""
         ...
```

### Comparing `mov_cli-4.3.8/mov_cli/players/syncplay.py` & `mov_cli-4.4a1/mov_cli/players/mpv.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,79 +4,59 @@
 if TYPE_CHECKING:
     from typing import Optional
     from ..media import Media
     from .. import Config
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import subprocess
-from devgoldyutils import Colours, LoggerAdapter
+from devgoldyutils import Colours
 
-from .. import errors
-from ..logger import mov_cli_logger
 from .player import Player
 
-__all__ = ("SyncPlay",)
+__all__ = ("MPV",)
 
-logger = LoggerAdapter(mov_cli_logger, prefix = Colours.PURPLE.apply("SyncPlay"))
-
-class SyncPlay(Player):
+class MPV(Player):
     def __init__(self, platform: SUPPORTED_PLATFORMS, config: Config, **kwargs) -> None:
         self.platform = platform
         self.config = config
 
-        super().__init__(**kwargs)
+        super().__init__(display_name = Colours.PURPLE.apply("MPV"), **kwargs)
 
     def play(self, media: Media) -> Optional[subprocess.Popen]:
-        """Plays this media in SyncPlay."""
-
-        logger.info("Launching SyncPlay...")
-
-        try:
-
-            if self.platform == "Windows" or self.platform == "Linux":
-                args = [
-                    "syncplay",
-                    media.url,
-                    "--",
-                    f"--force-media-title={media.display_name}",
-                ]
-
-                if media.referrer is not None:
-                    args.append(f"--referrer={media.referrer}")
-
-                if media.audio_url is not None:
-                    args.append(f"--audio-file={media.audio_url}")
-
-                if media.subtitles is not None:
-                    args.append(f"--sub-file={media.subtitles}")
-
-                if self.config.resolution is not None:
-                    args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: Only M3U8
-
-                return subprocess.Popen(args)
+        """Plays this media in the MPV media player."""
 
-            elif self.platform == "Darwin": # NOTE: Limits you to IINA
-                args = [
-                    "syncplay",
+        if self.platform == "Android":
+            return subprocess.Popen(
+                [
+                    "am",
+                    "start",
+                    "-n",
+                    "is.xyz.mpv/is.xyz.mpv.MPVActivity",
+                    "-e",
+                    "filepath",
                     media.url,
-                    "--",
-                    f"--mpv-force-media-title={media.display_name}",
                 ]
+            )
 
-                if media.referrer is not None:
-                    args.append(f"--mpv-referrer={media.referrer}")
+        elif self.platform == "Linux" or self.platform == "Windows" or self.platform == "Darwin":
+            args = [
+                "mpv",
+                media.url,
+                f"--force-media-title={media.display_name}",
+                "--no-terminal",
+            ]
 
-                if media.audio_url is not None: # TODO: This will need testing.
-                    args.append(f"--mpv-audio-file={media.audio_url}")
+            if media.referrer is not None:
+                args.append(f"--referrer={media.referrer}")
 
-                if media.subtitles is not None: # TODO: This will need testing.
-                    args.append(f"--mpv-sub-file={media.subtitles}")
+            if media.audio_url is not None:
+                args.append(f"--audio-file={media.audio_url}")
 
-                if self.config.resolution is not None: # TODO: This will need testing.
-                    args.append(f"--mpv-hls-bitrate={self.config.resolution}")
+            if media.subtitles is not None:
+                args.append(f"--sub-file={media.subtitles}")
 
-                return subprocess.Popen(args)
+            if self.config.resolution is not None:
+                args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
 
-        except (ModuleNotFoundError, FileNotFoundError):
-            raise errors.PlayerNotFound(self)
+            return subprocess.Popen(args)
 
         return None
```

### Comparing `mov_cli-4.3.8/mov_cli/players/vlc.py` & `mov_cli-4.4a1/mov_cli/players/vlc.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,33 +10,31 @@
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import httpx
 import subprocess
 import unicodedata
 from devgoldyutils import Colours, LoggerAdapter
 
-from .. import errors
 from .player import Player
 from ..logger import mov_cli_logger
 from ..utils import get_temp_directory
 
 __all__ = ("VLC",)
 
 logger = LoggerAdapter(mov_cli_logger, prefix = Colours.ORANGE.apply("VLC"))
 
 class VLC(Player):
     def __init__(self, platform: SUPPORTED_PLATFORMS, config: Config, **kwargs) -> None:
         self.platform = platform
         self.config = config
 
-        super().__init__(**kwargs)
+        super().__init__(display_name = Colours.ORANGE.apply("VLC"), **kwargs)
 
     def play(self, media: Media) -> Optional[subprocess.Popen]:
         """Plays this media in the VLC media player."""
-        logger.info("Launching VLC Media Player...")
 
         if self.platform == "Android":
             return subprocess.Popen(
                 [
                     "am",
                     "start",
                     "-n",
@@ -53,44 +51,40 @@
                 f.write(f"vlc://{media.url}")
 
             logger.info("The URL was copied into your clipboard. To play it, open a browser and paste the URL.")
 
             return None
 
         elif self.platform == "Linux" or self.platform == "Windows":
-            try:
-                args = [
-                    "vlc", 
-                    f'--meta-title="{media.display_name}"', 
-                    media.url, 
-                    "--quiet"
-                ]
-
-                if media.referrer is not None:
-                    args.append(f'--http-referrer="{media.referrer}"')
+            args = [
+                "vlc", 
+                f'--meta-title="{media.display_name}"', 
+                media.url, 
+                "--quiet"
+            ]
 
-                if media.audio_url is not None:
-                    args.append(f"--input-slave={media.audio_url}") # WHY IS THIS UNDOCUMENTED!!!
+            if media.referrer is not None:
+                args.append(f'--http-referrer="{media.referrer}"')
 
-                if media.subtitles is not None:
-                    subtitles = media.subtitles
+            if media.audio_url is not None:
+                args.append(f"--input-slave={media.audio_url}") # WHY IS THIS UNDOCUMENTED!!!
 
-                    if subtitles.startswith("https://"):
-                        logger.debug("Subtitles detected as a url.")
-                        subtitles = str(self.__url_subtitles_to_file(media, subtitles))
+            if media.subtitles is not None:
+                subtitles = media.subtitles
 
-                    args.append(f"--sub-file={subtitles}")
+                if subtitles.startswith("https://"):
+                    logger.debug("Subtitles detected as a url.")
+                    subtitles = str(self.__url_subtitles_to_file(media, subtitles))
 
-                if self.config.resolution is not None:
-                    args.append(f"--adaptive-maxwidth={self.config.resolution}") # NOTE: I don't really know if that works ~ Ananas
+                args.append(f"--sub-file={subtitles}")
 
-                return subprocess.Popen(args)
+            if self.config.resolution is not None:
+                args.append(f"--adaptive-maxwidth={self.config.resolution}") # NOTE: I don't really know if that works ~ Ananas
 
-            except (ModuleNotFoundError, FileNotFoundError):
-                raise errors.PlayerNotFound(self)
+            return subprocess.Popen(args)
 
         return None
 
     def __url_subtitles_to_file(self, media: Media, subtitles_url: str) -> Path:
         sub_file_exists_already = False
         temp_dir = get_temp_directory(self.platform)
```

### Comparing `mov_cli-4.3.8/mov_cli/plugins.py` & `mov_cli-4.4a1/mov_cli/plugins.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,43 +2,71 @@
 Module containing mov-cli plugin related stuff.
 """
 from __future__ import annotations
 from typing import TYPE_CHECKING, TypedDict
 
 if TYPE_CHECKING:
     from types import ModuleType
-    from typing import Optional, Dict, Literal, Tuple
+    from typing import Optional, Dict, Literal, List, Tuple
 
     from .scraper import Scraper
 
 import importlib
+from dataclasses import dataclass
 from devgoldyutils import LoggerAdapter
 
 from .logger import mov_cli_logger
 
 __all__ = (
     "load_plugin", 
-    "PluginHookData"
+    "PluginHookData", 
+    "Plugin"
 )
 
 logger = LoggerAdapter(mov_cli_logger, prefix = "Plugins")
 
 class PluginHookData(TypedDict):
     version: int
     """The version of the plugin hook to use. Version 1 is latest currently."""
     package_name: str
     """The name of the pypi package. This is required for the plugin update notifier to work."""
     scrapers: Dict[str, Scraper] | Dict[Literal["DEFAULT"], Scraper]
 
-def load_plugin(module_name: str) -> Optional[Tuple[Optional[PluginHookData], ModuleType]]:
+@dataclass
+class Plugin:
+    module: ModuleType
+    hook_data: PluginHookData
+
+    @property
+    def scrapers(self) -> List[Tuple[str, Scraper]]:
+        non_default_scrapers = []
+
+        for scraper_namespace, scraper_class in self.hook_data["scrapers"].items():
+
+            if scraper_namespace.endswith("DEFAULT"):
+                continue
+
+            non_default_scrapers.append((scraper_namespace, scraper_class))
+
+        return non_default_scrapers
+
+    @property
+    def version(self) -> Optional[str]:
+        return getattr(self.module, "__version__", None)
+
+def load_plugin(module_name: str) -> Optional[Plugin]:
     try:
         plugin_module = importlib.import_module(module_name.replace("-", "_"))
     except ModuleNotFoundError as e:
         logger.error(f"Failed to import a plugin from the module '{module_name}'! Error --> {e}")
         return None
 
-    plugin_data = getattr(plugin_module, "plugin", None)
+    plugin_data: PluginHookData = getattr(plugin_module, "plugin", None)
 
     if plugin_data is None:
         logger.warning(f"Failed to load the plugin '{module_name}'! It doesn't contain a plugin hook!")
+        return None
 
-    return plugin_data, plugin_module
+    return Plugin(
+        module = plugin_module, 
+        hook_data = plugin_data
+    )
```

### Comparing `mov_cli-4.3.8/mov_cli/scraper.py` & `mov_cli-4.4a1/mov_cli/scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 
     ScraperOptionsT = Dict[str, str | bool]
 
 from bs4 import BeautifulSoup
 from abc import ABC, abstractmethod
 from devgoldyutils import LoggerAdapter
 
-from . import errors
 from .logger import mov_cli_logger
 
-__all__ = ("Scraper", "MediaNotFound")
+__all__ = (
+    "Scraper",
+)
 
 class Scraper(ABC):
     """A base class for building scrapers from."""
     def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
         self.config = config
         self.http_client = http_client
         self.options = options or {}
@@ -37,26 +38,18 @@
 
     @abstractmethod
     def search(self, query: str, limit: int = 20) -> Iterable[Metadata]:
         """Where your searching for media should be done. Should return or yield Metadata."""
         ...
 
     @abstractmethod
-    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:
+    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Optional[Multi | Single]:
         """
         Where your scraping for the media should be performed. 
         Should return or yield an instance of Media.
         """
         ...
 
     @abstractmethod
     def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
         """Returns episode count for each season in that Movie/Series."""
-        ...
-
-class MediaNotFound(errors.MovCliException):
-    """Raises when a scraper fails to find a show/movie/tv-station."""
-    def __init__(self, message, scraper: Scraper) -> None:
-        super().__init__(
-            f"Failed to find media: {message}",
-            logger = scraper.logger
-        )
+        ...
```

### Comparing `mov_cli-4.3.8/mov_cli/utils/episode_selector.py` & `mov_cli-4.4a1/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/utils/paths.py` & `mov_cli-4.4a1/mov_cli/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/utils/platform.py` & `mov_cli-4.4a1/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.4a1/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.3.8/mov_cli/utils/version.py` & `mov_cli-4.4a1/mov_cli/utils/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Tuple, List, Optional, Dict
+    from typing import Tuple, List, Dict
 
 import httpx
 from packaging import version
 from devgoldyutils import LoggerAdapter, Colours
 
 import mov_cli
 from ..plugins import load_plugin
 from ..logger import mov_cli_logger
 
 __all__ = (
     "update_available", 
-    "plugin_update_available",
-    "get_plugin_version_hook"
+    "plugin_update_available"
 )
 
 logger = LoggerAdapter(mov_cli_logger, prefix = Colours.GREEN.apply("version"))
 
 def update_available() -> bool:
     logger.debug("Checking if mov-cli needs updating...")
 
@@ -44,25 +43,29 @@
     return False
 
 def plugin_update_available(plugins: Dict[str, str]) -> Tuple[bool, List[str]]:
     plugins_with_updates: List[str] = []
     logger.debug("Checking if plugins need updating...")
 
     for _, module_name in plugins.items():
-        plugin_version, plugin_hook_data = get_plugin_version_hook(module_name)
+        plugin = load_plugin(module_name)
+
+        if plugin is None:
+            continue
+
+        plugin_version = plugin.version
+        pypi_package_name = plugin.hook_data.get("package_name", None)
 
         if plugin_version is None:
             logger.debug(
-                f"Skipped update check for '{module_name}' as the plugin " \
-                    "doesn't expose '__version__' in it's root module ('__init__.py')."
+                f"The plugin '{module_name}' doesn't expose '__version__' in" \
+                    "it's root module ('__init__.py') so it the update checker will skip it."
             )
             continue
 
-        pypi_package_name = plugin_hook_data.get("package_name", None)
-
         if pypi_package_name is None:
             logger.debug(
                 f"Skipped update check for '{module_name}' as the plugin " \
                     "doesn't contain 'package_name' in it's hook data."
             )
             continue
 
@@ -81,29 +84,8 @@
 
         if version.parse(pypi_version) > version.parse(plugin_version):
             plugins_with_updates.append(pypi_package_name)
 
     if not plugins_with_updates == []:
         return True, plugins_with_updates
 
-    return False, []
-
-def get_plugin_version_hook(module_name: str):
-    plugin = load_plugin(module_name)
-
-    if plugin is None:
-        return None, None
-
-    plugin_module = plugin[1]
-    plugin_hook_data = plugin[0]
-
-    plugin_version: Optional[str] = getattr(plugin_module, "__version__", None)
-
-    if plugin_version is None:
-        logger.debug(
-            f"Skipped update check for '{module_name}' as the plugin " \
-                "doesn't expose '__version__' in it's root module ('__init__.py')."
-        )
-
-        return None, None
-    
-    return plugin_version, plugin_hook_data
+    return False, []
```

### Comparing `mov_cli-4.3.8/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.4a1/mov_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.8
+Version: 4.4a1
 Summary: Watch everything from your terminal.
-Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
+Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -39,21 +39,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: toml
-Requires-Dist: devgoldyutils>=2.5.7
+Requires-Dist: devgoldyutils>=3.0.0beta1
 Requires-Dist: typer>=0.12.2
 Requires-Dist: inquirer
 Requires-Dist: beautifulsoup4
 Requires-Dist: Unidecode
 Requires-Dist: deprecation
 Requires-Dist: packaging
+Requires-Dist: thefuzz
 Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.8 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a1 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
-r3tr0ananas.lol>, Goldy
+r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -23,23 +23,24 @@
 Windows 10 Classifier: Operating System :: POSIX :: Linux Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
-toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer>=0.12.2 Requires-
-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode Requires-
-Dist: deprecation Requires-Dist: packaging Requires-Dist: mov-cli-test>=1.1.0
-Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build;
-extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
-[Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions][python-
-shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url]
+toml Requires-Dist: devgoldyutils>=3.0.0beta1 Requires-Dist: typer>=0.12.2
+Requires-Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode
+Requires-Dist: deprecation Requires-Dist: packaging Requires-Dist: thefuzz
+Requires-Dist: mov-cli-test>=1.1.0 Provides-Extra: dev Requires-Dist: ruff;
+extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist:
+devgoldyutils[pprint]>=2.5.7; extra == "dev" [![Stargazers][stars-shield]]
+[stars-url] [![Pypi Version][pypi-shield]][pypi-url] [![Pypi Downloads][pypi-
+dl-shield]][pypi-stats-url] [![Python Versions][python-shield]][pypi-url] [!
+[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
+url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
```

### Comparing `mov_cli-4.3.8/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.4a1/mov_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 mov_cli/iterfzf/LICENSE.txt
 mov_cli/iterfzf/__init__.py
 mov_cli/media/__init__.py
 mov_cli/media/media.py
 mov_cli/media/metadata.py
 mov_cli/players/__init__.py
 mov_cli/players/custom_player.py
+mov_cli/players/iina.py
 mov_cli/players/mpv.py
 mov_cli/players/player.py
 mov_cli/players/syncplay.py
 mov_cli/players/vlc.py
 mov_cli/utils/__init__.py
 mov_cli/utils/episode_selector.py
 mov_cli/utils/paths.py
```

### Comparing `mov_cli-4.3.8/pyproject.toml` & `mov_cli-4.4a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "mov-cli"
 description = "Watch everything from your terminal."
 authors = [
     {name = "Pain", email = "painedposeidon444@gmail.com"},
-    {name = "Ananas", email = "ananas@r3tr0ananas.lol"},
+    {name = "Ananas", email = "ananas@r3tr0ananas.pro"},
     {name = "Goldy", email = "goldy@devgoldy.xyz"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = [
     "movie-cli", "mov_cli"
@@ -23,21 +23,22 @@
 	'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12'
 ]
 dependencies = [
     "httpx",
     "importlib-metadata; python_version<'3.8'",
     "toml",
-    "devgoldyutils>=2.5.7",
+    "devgoldyutils>=3.0.0beta1",
     "typer>=0.12.2",
     "inquirer",
     "beautifulsoup4",
     "Unidecode",
     "deprecation",
     "packaging",
+    "thefuzz",
 
     # Included plugins
     "mov-cli-test>=1.1.0"
 ]
 
 dynamic = ["version"]
 
@@ -62,8 +63,8 @@
 [tool.setuptools.packages.find]
 include = ["mov_cli*"]
 
 [tool.setuptools.package-data]
 "mov_cli" = ["config.template.toml", "cli/random_tips.json"]
 
 [project.scripts]
-mov-cli = "mov_cli.cli.__main__:app"
+mov-cli = "mov_cli.cli.__main__:app"
```

